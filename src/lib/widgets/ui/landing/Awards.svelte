<script>
  import {awards} from '$shared'
</script>



<section  class="section_inscription">
  <div class="padding-global padding-section-medium padding-bottom-huge">
    <!-- <a name=""></a> -->
    <div class="container-medium">
<div class="flex flex-row flex-wrap flex-wrap justify-center ">
    {#each awards as award}

        <div style="background-image: url({award.img}); " class="card-award m-2 -mt-10 items-end flex max-w-sm">
            <div style="min-height: 200px; height: auto; width: 100%; " class="bg-[#111111] rounded-lg border border-[#146ef5] shadow-md flex max-w-sm flex-col p-4 sm:p-6">
                <span class="text-6xl mb-4 tracking-tight text-white text-center">
                    {award.title} <br/> miejsce
                </span>

                <ul class="text-color-neutral max-w-md list-disc list-inside space-y-1">
                    {#each award.awards as award}
                    <li class="">
                        {award}
                    </li>
                    {/each}
                </ul>
                <!-- {#if award.hackerspace}
                <span class="text-1xl mt-6 tracking-tight text-white text-center">
                    Serdeczne podziękowania dla  <a class="inline-flex items-center hover:underline font-normal text-light underline hover:no-underline" href="https://44hackerspace.vercel.app/">44Hackerspace</a> za udostępnienie sprzętu do druku 3D.
                </span>

                {/if} -->
            </div>

        </div>
    {/each}
</div>
   <div class="inscription_background"></div>
  <div  class="inscription_canvas"></div>
</div>
</div>
</section>

<style>
    .card-award {
        height: 520px;
        background-repeat: no-repeat;
        background-position: center;
        background-size: contain;
    }
</style>
