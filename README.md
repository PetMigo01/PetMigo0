<!DOCTYPE html>
<html>
  <head>
    <link rel="preconnect" href="https://fonts.gstatic.com/" crossorigin="" />
    <link
      rel="stylesheet"
      as="style"
      onload="this.rel='stylesheet'"
      href="https://fonts.googleapis.com/css2?display=swap&amp;family=Noto+Sans%3Awght%40400%3B500%3B700%3B900&amp;family=Plus+Jakarta+Sans%3Awght%40400%3B500%3B700%3B800"
    />

    <title>PetMigo - Your Pet's Best Friend</title>
    <link rel="icon" type="image/x-icon" href="data:image/x-icon;base64," />

    <script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
    <style>
      .page {
        display: none;
      }
      .active-page {
        display: block;
      }
    </style>
  </head>
  <body>
    <div class="relative flex size-full min-h-screen flex-col bg-white group/design-root overflow-x-hidden" style='font-family: "Plus Jakarta Sans", "Noto Sans", sans-serif;'>
      <!-- Navigation Header -->
      <header class="flex items-center justify-between whitespace-nowrap border-b border-solid border-b-[#f2f4f0] px-10 py-3">
        <div class="flex items-center gap-4 text-[#151811]">
          <div class="size-4">
            <svg viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M6 6H42L36 24L42 42H6L12 24L6 6Z" fill="currentColor"></path></svg>
          </div>
          <h2 class="text-[#151811] text-lg font-bold leading-tight tracking-[-0.015em]">PetMigo</h2>
        </div>
        <div class="flex flex-1 justify-end gap-8">
          <div class="flex items-center gap-9">
            <a class="text-[#151811] text-sm font-medium leading-normal nav-link" href="#" data-page="home">Home</a>
            <a class="text-[#151811] text-sm font-medium leading-normal nav-link" href="#" data-page="recommendation">PetRecommendation</a>
            <a class="text-[#151811] text-sm font-medium leading-normal nav-link" href="#" data-page="education">PetEduZone</a>
            <a class="text-[#151811] text-sm font-medium leading-normal nav-link" href="#" data-page="community">PawnUnity</a>
            <a class="text-[#151811] text-sm font-medium leading-normal nav-link" href="#" data-page="login">Login</a>
          </div>
          <button
            class="flex max-w-[480px] cursor-pointer items-center justify-center overflow-hidden rounded-xl h-10 bg-[#f2f4f0] text-[#151811] gap-2 text-sm font-bold leading-normal tracking-[0.015em] min-w-0 px-2.5"
          >
            <div class="text-[#151811]" data-icon="List" data-size="20px" data-weight="regular">
              <svg xmlns="http://www.w3.org/2000/svg" width="20px" height="20px" fill="currentColor" viewBox="0 0 256 256">
                <path
                  d="M224,128a8,8,0,0,1-8,8H40a8,8,0,0,1,0-16H216A8,8,0,0,1,224,128ZM40,72H216a8,8,0,0,0,0-16H40a8,8,0,0,0,0,16ZM216,184H40a8,8,0,0,0,0,16H216a8,8,0,0,0,0-16Z"
                ></path>
              </svg>
            </div>
          </button>
        </div>
      </header>

      <!-- Home Page -->
      <div id="home" class="page active-page">
        <div class="px-40 flex flex-1 justify-center py-5">
          <div class="layout-content-container flex flex-col max-w-[960px] flex-1">
            <div class="@container">
              <div class="@[480px]:p-4">
                <div
                  class="flex min-h-[480px] flex-col gap-6 bg-cover bg-center bg-no-repeat @[480px]:gap-8 @[480px]:rounded-xl items-start justify-end px-4 pb-10 @[480px]:px-10"
                  style='background-image: linear-gradient(rgba(0, 0, 0, 0.1) 0%, rgba(0, 0, 0, 0.4) 100%), url("https://cdn.usegalileo.ai/sdxl10/6a14b84e-5589-4d12-b54b-5bf56a053f5c.png");'
                >
                  <div class="flex flex-col gap-2 text-left">
                    <h1
                      class="text-white text-4xl font-black leading-tight tracking-[-0.033em] @[480px]:text-5xl @[480px]:font-black @[480px]:leading-tight @[480px]:tracking-[-0.033em]"
                    >
                      Your pet's best friend
                    </h1>
                    <h2 class="text-white text-sm font-normal leading-normal @[480px]:text-base @[480px]:font-normal @[480px]:leading-normal">
                      PetMigo is a community of pet owners, with digital services to help you take care of your pets
                    </h2>
                  </div>
                  <label class="flex flex-col min-w-40 h-14 w-full max-w-[480px] @[480px]:h-16">
                    <div class="flex w-full flex-1 items-stretch rounded-xl h-full">
                      <div
                        class="text-[#778863] flex border border-[#e1e5dc] bg-white items-center justify-center pl-[15px] rounded-l-xl border-r-0"
                        data-icon="MagnifyingGlass"
                        data-size="20px"
                        data-weight="regular"
                      >
                        <svg xmlns="http://www.w3.org/2000/svg" width="20px" height="20px" fill="currentColor" viewBox="0 0 256 256">
                          <path
                            d="M229.66,218.34l-50.07-50.06a88.11,88.11,0,1,0-11.31,11.31l50.06,50.07a8,8,0,0,0,11.32-11.32ZM40,112a72,72,0,1,1,72,72A72.08,72.08,0,0,1,40,112Z"
                          ></path>
                        </svg>
                      </div>
                      <input
                        placeholder="Search for anything"
                        class="form-input flex w-full min-w-0 flex-1 resize-none overflow-hidden rounded-xl text-[#151811] focus:outline-0 focus:ring-0 border border-[#e1e5dc] bg-white focus:border-[#e1e5dc] h-full placeholder:text-[#778863] px-[15px] rounded-r-none border-r-0 pr-2 rounded-l-none border-l-0 pl-2 text-sm font-normal leading-normal @[480px]:text-base @[480px]:font-normal @[480px]:leading-normal"
                        value=""
                      />
                      <div class="flex items-center justify-center rounded-r-xl border-l-0 border border-[#e1e5dc] bg-white pr-[7px]">
                        <button
                          class="flex min-w-[84px] max-w-[480px] cursor-pointer items-center justify-center overflow-hidden rounded-xl h-10 px-4 @[480px]:h-12 @[480px]:px-5 bg-[#86e31c] text-[#151811] text-sm font-bold leading-normal tracking-[0.015em] @[480px]:text-base @[480px]:font-bold @[480px]:leading-normal @[480px]:tracking-[0.015em]"
                        >
                          <span class="truncate">Submit</span>
                        </button>
                      </div>
                    </div>
                  </label>
                </div>
              </div>
            </div>
            <h2 class="text-[#151811] text-[22px] font-bold leading-tight tracking-[-0.015em] px-4 pb-3 pt-5">PetRecommendation</h2>
            <div class="grid grid-cols-[repeat(auto-fit,minmax(158px,1fr))] gap-3 p-4">
              <div class="flex flex-col gap-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-square bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/dc238cb3-91f4-4ed0-a955-e4bf5b700869.png");'
                ></div>
              </div>
              <div class="flex flex-col gap-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-square bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/06ce5b3e-74b6-452e-a82b-8ac6b3c24c30.png");'
                ></div>
              </div>
              <div class="flex flex-col gap-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-square bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/eea404fc-fb6d-42a4-af60-b608dcd30d39.png");'
                ></div>
              </div>
              <div class="flex flex-col gap-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-square bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/3f9c4cbb-aacb-48d3-a4c2-b6cc8f6409b4.png");'
                ></div>
              </div>
            </div>
            <h2 class="text-[#151811] text-[22px] font-bold leading-tight tracking-[-0.015em] px-4 pb-3 pt-5">PetEduZone</h2>
            <div class="grid grid-cols-[repeat(auto-fit,minmax(158px,1fr))] gap-3 p-4">
              <div class="flex flex-1 gap-3 rounded-lg border border-[#e1e5dc] bg-white p-4 items-center">
                <div
                  class="bg-center bg-no-repeat aspect-square bg-cover rounded-full w-10 shrink-0"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/23347bb1-54a1-4a64-9166-7c1085ccbffc.png");'
                ></div>
                <h2 class="text-[#151811] text-base font-bold leading-tight">Puppy</h2>
              </div>
              <div class="flex flex-1 gap-3 rounded-lg border border-[#e1e5dc] bg-white p-4 items-center">
                <div
                  class="bg-center bg-no-repeat aspect-square bg-cover rounded-full w-10 shrink-0"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/950ef782-8993-4d97-bffa-03fc26c902ed.png");'
                ></div>
                <h2 class="text-[#151811] text-base font-bold leading-tight">Kitten</h2>
              </div>
              <div class="flex flex-1 gap-3 rounded-lg border border-[#e1e5dc] bg-white p-4 items-center">
                <div
                  class="bg-center bg-no-repeat aspect-square bg-cover rounded-full w-10 shrink-0"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/4e02d131-7ab4-47ce-951e-5c65fdbfdd4c.png");'
                ></div>
                <h2 class="text-[#151811] text-base font-bold leading-tight">Dog</h2>
              </div>
              <div class="flex flex-1 gap-3 rounded-lg border border-[#e1e5dc] bg-white p-4 items-center">
                <div
                  class="bg-center bg-no-repeat aspect-square bg-cover rounded-full w-10 shrink-0"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/1d6f124b-ed82-41b3-ad23-460dfe192be1.png");'
                ></div>
                <h2 class="text-[#151811] text-base font-bold leading-tight">Cat</h2>
              </div>
            </div>
            <h2 class="text-[#151811] text-[22px] font-bold leading-tight tracking-[-0.015em] px-4 pb-3 pt-5">PawnUnity</h2>
            <div class="grid grid-cols-[repeat(auto-fit,minmax(158px,1fr))] gap-3 p-4">
              <div class="flex flex-col gap-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-square bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/ae76f1c6-28d0-4bdb-9e7e-5fed5e0db1f1.png");'
                ></div>
              </div>
              <div class="flex flex-col gap-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-square bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/5d741bae-51e8-4f28-b7f7-ad0f52445ea3.png");'
                ></div>
              </div>
              <div class="flex flex-col gap-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-square bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/47a05a26-bb1c-4b21-87f1-7119a81f4884.png");'
                ></div>
              </div>
              <div class="flex flex-col gap-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-square bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/0b409078-8abd-44a7-8eb0-f63f89f004a1.png");'
                ></div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Login Page -->
      <div id="login" class="page">
        <div class="px-40 flex flex-1 justify-center py-5">
          <div class="layout-content-container flex flex-col w-[512px] max-w-[512px] py-5 max-w-[960px] flex-1">
            <div class="@container">
              <div class="@[480px]:px-4 @[480px]:py-3">
                <div
                  class="w-full bg-center bg-no-repeat bg-cover flex flex-col justify-end overflow-hidden bg-white @[480px]:rounded-xl min-h-80"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/4704eaca-e29b-43ce-9339-3e0ec4c4b067.png");'
                ></div>
              </div>
            </div>
            <h1 class="text-[#151811] text-[22px] font-bold leading-tight tracking-[-0.015em] px-4 text-center pb-3 pt-5">Welcome back!</h1>
            <div class="flex max-w-[480px] flex-wrap items-end gap-4 px-4 py-3">
              <label class="flex flex-col min-w-40 flex-1">
                <p class="text-[#151811] text-base font-medium leading-normal pb-2">Email</p>
                <input
                  class="form-input flex w-full min-w-0 flex-1 resize-none overflow-hidden rounded-xl text-[#151811] focus:outline-0 focus:ring-0 border border-[#e1e5dc] bg-white focus:border-[#e1e5dc] h-14 placeholder:text-[#778863] p-[15px] text-base font-normal leading-normal"
                  value=""
                />
              </label>
            </div>
            <div class="flex max-w-[480px] flex-wrap items-end gap-4 px-4 py-3">
              <label class="flex flex-col min-w-40 flex-1">
                <p class="text-[#151811] text-base font-medium leading-normal pb-2">Password</p>
                <input
                  class="form-input flex w-full min-w-0 flex-1 resize-none overflow-hidden rounded-xl text-[#151811] focus:outline-0 focus:ring-0 border border-[#e1e5dc] bg-white focus:border-[#e1e5dc] h-14 placeholder:text-[#778863] p-[15px] text-base font-normal leading-normal"
                  value=""
                />
              </label>
            </div>
            <div class="flex px-4 py-3">
              <button
                class="flex min-w-[84px] max-w-[480px] cursor-pointer items-center justify-center overflow-hidden rounded-xl h-12 px-5 flex-1 bg-[#86e31c] text-[#151811] text-base font-bold leading-normal tracking-[0.015em]"
              >
                <span class="truncate">Log in</span>
              </button>
            </div>
            <p class="text-[#778863] text-sm font-normal leading-normal pb-3 pt-1 px-4 text-center">or</p>
            <div class="flex px-4 py-3">
              <button
                class="flex min-w-[84px] max-w-[480px] cursor-pointer items-center justify-center overflow-hidden rounded-xl h-12 px-5 flex-1 bg-[#f2f4f0] text-[#151811] gap-2 pl-5 text-base font-bold leading-normal tracking-[0.015em]"
              >
                <div class="text-[#151811]" data-icon="GoogleLogo" data-size="24px" data-weight="regular">
                  <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" fill="currentColor" viewBox="0 0 256 256">
                    <path d="M224,128a96,96,0,1,1-21.95-61.09,8,8,0,1,1-12.33,10.18A80,80,0,1,0,207.6,136H128a8,8,0,0,1,0-16h88A8,8,0,0,1,224,128Z"></path>
                  </svg>
                </div>
                <span class="truncate">Continue with Google</span>
              </button>
            </div>
            <div class="flex px-4 py-3">
              <button
                class="flex min-w-[84px] max-w-[480px] cursor-pointer items-center justify-center overflow-hidden rounded-xl h-12 px-5 flex-1 bg-[#f2f4f0] text-[#151811] gap-2 pl-5 text-base font-bold leading-normal tracking-[0.015em]"
              >
                <div class="text-[#151811]" data-icon="FacebookLogo" data-size="24px" data-weight="regular">
                  <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" fill="currentColor" viewBox="0 0 256 256">
                    <path
                      d="M128,24A104,104,0,1,0,232,128,104.11,104.11,0,0,0,128,24Zm8,191.63V152h24a8,8,0,0,0,0-16H136V112a16,16,0,0,1,16-16h16a8,8,0,0,0,0-16H152a32,32,0,0,0-32,32v24H96a8,8,0,0,0,0,16h24v63.63a88,88,0,1,1,16,0Z"
                    ></path>
                  </svg>
                </div>
                <span class="truncate">Continue with Facebook</span>
              </button>
            </div>
            <div class="flex px-4 py-3">
              <button
                class="flex min-w-[84px] max-w-[480px] cursor-pointer items-center justify-center overflow-hidden rounded-xl h-12 px-5 flex-1 bg-[#f2f4f0] text-[#151811] gap-2 pl-5 text-base font-bold leading-normal tracking-[0.015em]"
              >
                <div class="text-[#151811]" data-icon="AppleLogo" data-size="24px" data-weight="regular">
                  <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" fill="currentColor" viewBox="0 0 256 256">
                    <path
                      d="M223.3,169.59a8.07,8.07,0,0,0-2.8-3.4C203.53,154.53,200,134.64,200,120c0-17.67,13.47-33.06,21.5-40.67a8,8,0,0,0,0-11.62C208.82,55.74,187.82,48,168,48a72.2,72.2,0,0,0-40,12.13,71.56,71.56,0,0,0-90.71,9.09A74.63,74.63,0,0,0,16,123.4a127.06,127.06,0,0,0,40.14,89.73A39.8,39.8,0,0,0,83.59,224h87.68a39.84,39.84,0,0,0,29.12-12.57,125,125,0,0,0,17.82-24.6C225.23,174,224.33,172,223.3,169.59Zm-34.63,30.94a23.76,23.76,0,0,1-17.4,7.47H83.59a23.82,23.82,0,0,1-16.44-6.51A111.14,111.14,0,0,1,32,123A58.5,58.5,0,0,1,48.65,80.47,54.81,54.81,0,0,1,88,64h.78A55.45,55.45,0,0,1,123,76.28a8,8,0,0,0,10,0A55.44,55.44,0,0,1,168,64a70.64,70.64,0,0,1,36,10.35c-13,14.52-20,30.47-20,45.65,0,23.77,7.64,42.73,22.18,55.3A105.82,105.82,0,0,1,188.67,200.53ZM128.23,30A40,40,0,0,1,167,0h1a8,8,0,0,1,0,16h-1a24,24,0,0,0-23.24,18,8,8,0,1,1-15.5-4Z"
                    ></path>
                  </svg>
                </div>
                <span class="truncate">Continue with Apple ID</span>
              </button>
            </div>
          </div>
        </div>
      </div>

      <!-- Pet Recommendation Page -->
      <div id="recommendation" class="page">
        <div class="px-40 flex flex-1 justify-center py-5">
          <div class="layout-content-container flex flex-col max-w-[960px] flex-1">
            <div class="@container">
              <div class="@[480px]:px-4 @[480px]:py-3">
                <div
                  class="bg-cover bg-center flex flex-col justify-end overflow-hidden bg-[#FFFFFF] @[480px]:rounded-xl min-h-80"
                  style='background-image: linear-gradient(0deg, rgba(0, 0, 0, 0.4) 0%, rgba(0, 0, 0, 0) 25%), url("https://cdn.usegalileo.ai/sdxl10/fb75b987-835f-472a-aacb-905d8d6e94b6.png");'
                >
                  <div class="flex p-4"><p class="text-white tracking-light text-[28px] font-bold leading-tight">Recommended For Your Cat</p></div>
                </div>
              </div>
            </div>
            <div class="px-4 py-3">
              <label class="flex flex-col min-w-40 h-12 w-full">
                <div class="flex w-full flex-1 items-stretch rounded-xl h-full">
                  <div
                    class="text-[#A18249] flex border-none bg-[#F4EFE6] items-center justify-center pl-4 rounded-l-xl border-r-0"
                    data-icon="MagnifyingGlass"
                    data-size="24px"
                    data-weight="regular"
                  >
                    <svg xmlns="http://www.w3.org/2000/svg" width="24px" height="24px" fill="currentColor" viewBox="0 0 256 256">
                      <path
                        d="M229.66,218.34l-50.07-50.06a88.11,88.11,0,1,0-11.31,11.31l50.06,50.07a8,8,0,0,0,11.32-11.32ZM40,112a72,72,0,1,1,72,72A72.08,72.08,0,0,1,40,112Z"
                      ></path>
                    </svg>
                  </div>
                  <input
                    placeholder="Search for products and services"
                    class="form-input flex w-full min-w-0 flex-1 resize-none overflow-hidden rounded-xl text-[#1C160C] focus:outline-0 focus:ring-0 border-none bg-[#F4EFE6] focus:border-none h-full placeholder:text-[#A18249] px-4 rounded-l-none border-l-0 pl-2 text-base font-normal leading-normal"
                    value=""
                  />
                </div>
              </label>
            </div>
            <div class="grid grid-cols-[repeat(auto-fit,minmax(158px,1fr))] gap-3 p-4">
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-[3/4] bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/61d5507d-1409-444f-8fa9-8c2f2f9038c4.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">Dry Cat Food - Whiskas 1kg</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Suitable for adult cats, helps maintain skin and fur health</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-[3/4] bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/1e6d5199-7124-4f48-8233-3cb4692aed75.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">Cat Litter - Tidy Cats 5kg</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Clumping litter, controls odors</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-[3/4] bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/5cfb4ab4-3007-4832-ae2f-7d37b8dcbd5e.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">Cat Toy - Kong Feather Teaser</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Feather teaser toy, suitable for all ages</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-[3/4] bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/9e493a87-d59c-40e3-b548-851fd1b5a0fe.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">Cat Collar - Blue Stripes</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Adjustable size, breakaway safety buckle</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Education Page -->
      <div id="education" class="page">
        <div class="px-40 flex flex-1 justify-center py-5">
          <div class="layout-content-container flex flex-col max-w-[960px] flex-1">
            <div class="flex flex-wrap justify-between gap-3 p-4">
              <p class="text-[#1C160C] text-4xl font-black leading-tight tracking-[-0.033em] min-w-72">Learn from experts</p>
            </div>
            <div class="pb-3">
              <div class="flex border-b border-[#E9DFCE] px-4 gap-8">
                <a class="flex flex-col items-center justify-center border-b-[3px] border-b-[#019863] text-[#1C160C] pb-[13px] pt-4" href="#">
                  <p class="text-[#1C160C] text-sm font-bold leading-normal tracking-[0.015em]">All Topics</p>
                </a>
                <a class="flex flex-col items-center justify-center border-b-[3px] border-b-transparent text-[#A18249] pb-[13px] pt-4" href="#">
                  <p class="text-[#A18249] text-sm font-bold leading-normal tracking-[0.015em]">Animal Health</p>
                </a>
                <a class="flex flex-col items-center justify-center border-b-[3px] border-b-transparent text-[#A18249] pb-[13px] pt-4" href="#">
                  <p class="text-[#A18249] text-sm font-bold leading-normal tracking-[0.015em]">Pet Care Tips</p>
                </a>
                <a class="flex flex-col items-center justify-center border-b-[3px] border-b-transparent text-[#A18249] pb-[13px] pt-4" href="#">
                  <p class="text-[#A18249] text-sm font-bold leading-normal tracking-[0.015em]">Training &amp; Behavior</p>
                </a>
                <a class="flex flex-col items-center justify-center border-b-[3px] border-b-transparent text-[#A18249] pb-[13px] pt-4" href="#">
                  <p class="text-[#A18249] text-sm font-bold leading-normal tracking-[0.015em]">Nutrition &amp; Food</p>
                </a>
              </div>
            </div>
            <div class="grid grid-cols-[repeat(auto-fit,minmax(158px,1fr))] gap-3 p-4">
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/b3e9dbff-05c3-4e77-bb48-e14864aa9add.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">How to Train a Puppy to Walk on a Leash</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Pet Training</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/fc3de76f-a47c-404d-a7e8-1fa95cc484e8.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">Why Does My Cat Sleep So Much?</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Cat Health</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/a09f9f5a-f9f7-4b35-b95b-a48988119f49.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">How to Keep Your Dog Safe During the Holidays</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Dog Safety</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/db4de9e5-dc39-4abb-abc4-e9ad0a57c3cc.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">How to Feed Your Fish: The Complete Guide</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Fish Care</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/2c50d885-d29a-4299-b8c1-408cf3c5768b.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">The Benefits of Grooming Your Pet Regularly</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Pet Grooming</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/e4ad7c23-db1c-4116-a6ee-af047545a5fb.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">How to Tell if Your Bird is Sick</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Bird Health</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/ccc9e1ab-fa13-40a9-8ff8-81acdc585190.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">What to Do if Your Reptile Stops Eating</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Reptile Care</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/4d43f418-9c56-4621-b52a-b66353410cd1.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">Caring for Small Animals: Tips for New Owners</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Small Animal Care</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/901fc3e6-e58e-46fe-a4db-5a1d8e006e89.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">How to Help Your Horse Recover from an Injury</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Horse Health</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/90c30505-7122-4aab-b7ff-1bf79fb11392.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">Understanding the Nutritional Needs of Rabbits</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Rabbit Nutrition</p>
                </div>
              </div>
            </div>
            <h2 class="text-[#1C160C] text-[22px] font-bold leading-tight tracking-[-0.015em] px-4 pb-3 pt-5">Most Popular</h2>
            <div class="grid grid-cols-[repeat(auto-fit,minmax(158px,1fr))] gap-3 p-4">
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/5045e05b-2b11-4159-b778-1fcb67375a99.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">How to Train a Puppy to Walk on a Leash</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Pet Training</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/3be1ece1-d5e2-4421-93fb-36870a969f09.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">Why Does My Cat Sleep So Much?</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Cat Health</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/31d2674c-25e0-47cd-924a-cee07444470a.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">How to Keep Your Dog Safe During the Holidays</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Dog Safety</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/c12f8c6f-8d7c-43ea-8fb0-b48b38a68783.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">How to Feed Your Fish: The Complete Guide</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Fish Care</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/37ddcfd7-f831-4baf-90aa-e2d8e4cd9c62.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">The Benefits of Grooming Your Pet Regularly</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Pet Grooming</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/8b99b791-07d3-4a9a-b7f4-486b5c88aa61.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">How to Tell if Your Bird is Sick</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Bird Health</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/62d37581-408e-424c-8774-2b5d70387d9f.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">What to Do if Your Reptile Stops Eating</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Reptile Care</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/0af8d2b7-4285-4a49-9d02-9b5421943724.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">Caring for Small Animals: Tips for New Owners</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Small Animal Care</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/60f42dca-042d-4434-87c3-7f22ef9fffde.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">How to Help Your Horse Recover from an Injury</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Horse Health</p>
                </div>
              </div>
              <div class="flex flex-col gap-3 pb-3">
                <div
                  class="w-full bg-center bg-no-repeat aspect-video bg-cover rounded-xl"
                  style='background-image: url("https://cdn.usegalileo.ai/sdxl10/8f7b2c17-87bd-42a5-a920-19330dce3fd8.png");'
                ></div>
                <div>
                  <p class="text-[#1C160C] text-base font-medium leading-normal">Understanding the Nutritional Needs of Rabbits</p>
                  <p class="text-[#A18249] text-sm font-normal leading-normal">Rabbit Nutrition</p>
                </div>
              </div>
            </div>
          </div>
          <div class="layout-content-container flex flex-col"></div>
        </div>
      </div>

      <!-- Community Page -->
      <div id="community" class="page">
        <div class="px-40 flex flex-1 justify-center py-5">
          <div class="layout-content-container flex flex-col max-w-[960px] flex-1">
            <div class="flex flex-wrap justify-between gap-3 p-4"><p class="text-[#1C160C] tracking-light text-[32px] font-bold leading-tight min-w-72">Ask a Question</p></div>
            <div class="flex max-w-[480px] flex-wrap items-end gap-4 px-4 py-3">
              <label class="flex flex-col min-w-40 flex-1">
                <input
                  placeholder="Ask your question here"
                  class="form-input flex w-full min-w-0 flex-1 resize-none overflow-hidden rounded-xl text-[#1C160C] focus:outline-0 focus:ring-0 border border-[#E9DFCE] bg-[#FFFFFF] focus:border-[#E9DFCE] h-14 placeholder:text-[#A18249] p-[15px] text-base font-normal leading-normal"
                  value=""
                />
              </label>
            </div>
            <h3 class="text-[#1C160C] tracking-light text-2xl font-bold leading-tight px-4 text-left pb-2 pt-5">Choose a Topic</h3>
            <div class="flex gap-3 p-3 flex-wrap pr-4">
              <div class="flex h-8 shrink-0 items-center justify-center gap-x-2 rounded-full bg-[#F4EFE6] pl-4 pr-4">
                <p class="text-[#1C160C] text-sm font-medium leading-normal">Health</p>
              </div>
              <div class="flex h-8 shrink-0 items-center justify-center gap-x-2 rounded-full bg-[#F4EFE6] pl-4 pr-4">
                <p class="text-[#1C160C] text-sm font-medium leading-normal">Training</p>
              </div>
              <div class="flex h-8 shrink-0 items-center justify-center gap-x-2 rounded-full bg-[#F4EFE6] pl-4 pr-4">
                <p class="text-[#1C160C] text-sm font-medium leading-normal">Behavior</p>
              </div>
              <div class="flex h-8 shrink-0 items-center justify-center gap-x-2 rounded-full bg-[#F4EFE6] pl-4 pr-4">
                <p class="text-[#1C160C] text-sm font-medium leading-normal">Food</p>
              </div>
              <div class="flex h-8 shrink-0 items-center justify-center gap-x-2 rounded-full bg-[#F4EFE6] pl-4 pr-4">
                <p class="text-[#1C160C] text-sm font-medium leading-normal">Loss &amp; Grief</p>
              </div>
            </div>
            <div class="flex px-4 py-3 justify-start">
              <button
                class="flex min-w-[84px] max-w-[480px] cursor-pointer items-center justify-center overflow-hidden rounded-full h-10 px-4 bg-[#019863] text-[#FFFFFF] text-sm font-bold leading-normal tracking-[0.015em]"
              >
                <span class="truncate">Post your question</span>
              </button>
            </div>
          </div>
          <div class="layout-content-container flex flex-col">
            <footer class="flex flex-col gap-6 px-5 py-10 text-center @container">
              <div class="flex flex-wrap items-center justify-center gap-6 @[480px]:flex-row @[480px]:justify-around">
                <a class="text-[#A18249] text-base font-normal leading-normal min-w-40" href="#">About</a>
                <a class="text-[#A18249] text-base font-normal leading-normal min-w-40" href="#">Blog</a>
                <a class="text-[#A18249] text-base font-normal leading-normal min-w-40" href="#">Community</a>
                <a class="text-[#A18249] text-base font-normal leading-normal min-w-40" href="#">Guidelines</a>
                <a class="text-[#A18249] text-base font-normal leading-normal min-w-40" href="#">Privacy</a>
                <a class="text-[#A18249] text-base font-normal leading-normal min-w-40" href="#">Terms</a>
                <a class="text-[#A18249] text-base font-normal leading-normal min-w-40" href="#">Feedback</a>
              </div>
              <p class="text-[#A18249] text-base font-normal leading-normal">@2023 PetPedia</p>
            </footer>
          </div>
        </div>
      </div>
    </div>

    <script>
      // Navigation functionality
      document.querySelectorAll('.nav-link').forEach(link => {
        link.addEventListener('click', function(e) {
          e.preventDefault();
          const pageId = this.getAttribute('data-page');
          
          // Hide all pages
          document.querySelectorAll('.page').forEach(page => {
            page.classList.remove('active-page');
          });
          
          // Show selected page
          document.getElementById(pageId).classList.add('active-page');
          
          // Update active link styling
          document.querySelectorAll('.nav-link').forEach(navLink => {
            navLink.classList.remove('text-[#019863]', 'font-bold');
          });
          this.classList.add('text-[#019863]', 'font-bold');
        });
      });
      
      // Set home as default active link
      document.querySelector('.nav-link[data-page="home"]').classList.add('text-[#019863]', 'font-bold');
    </script>
  </body>
</html>
