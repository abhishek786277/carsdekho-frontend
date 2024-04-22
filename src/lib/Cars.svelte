<script>
  let data = [
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/2/25/2015_Mazda_MX-5_ND_2.0_SKYACTIV-G_160_i-ELOOP_Rubinrot-Metallic_Vorderansicht.jpg/400px-2015_Mazda_MX-5_ND_2.0_SKYACTIV-G_160_i-ELOOP_Rubinrot-Metallic_Vorderansicht.jpg",
      title: "Mazda MX-5",
      start_production: 1989,
      class: "Sports car Roadster",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/VW_Kuebelwagen_1.jpg/400px-VW_Kuebelwagen_1.jpg",
      title: "Volkswagen Kübelwagen",
      class: "Military vehicle",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/e/e4/2014_Porsche_Cayenne_%2892A_MY14%29_GTS_wagon_%282015-08-07%29_01.jpg/400px-2014_Porsche_Cayenne_%2892A_MY14%29_GTS_wagon_%282015-08-07%29_01.jpg",
      title: "Porsche Cayenne",
      start_production: 2002,
      class: "Mid-size luxury crossover SUV",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/f/f0/Vintage_car_at_the_Wirral_Bus_%26_Tram_Show_-_DSC03336.JPG/400px-Vintage_car_at_the_Wirral_Bus_%26_Tram_Show_-_DSC03336.JPG",
      title: "Vauxhall Chevette",
      start_production: 1975,
      class: "Supermini",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/f/f0/Dynamixion_car_by_Buckminster_Fuller_1933_%28side_views%29.jpg/400px-Dynamixion_car_by_Buckminster_Fuller_1933_%28side_views%29.jpg",
      title: "Dymaxion car",
      start_production: 1933,
      class: "Concept car",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/f/f0/Ford_Crown_Victoria_LX.jpg/400px-Ford_Crown_Victoria_LX.jpg",
      title: "Ford Crown Victoria",
      start_production: 1955,
      class: "Full-size Ford",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/2/27/Plymouth_Superbird.jpg/400px-Plymouth_Superbird.jpg",
      title: "Plymouth Superbird",
      start_production: 1970,
      class: "Muscle car(today) and Race car(Past)",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/2/2a/2nd-Saab-9000-hatch.jpg/400px-2nd-Saab-9000-hatch.jpg",
      title: "Saab 9000",
      start_production: 1984,
      class: "Executive car",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/5/5e/2003-2005_Pontiac_Sunfire.jpg/400px-2003-2005_Pontiac_Sunfire.jpg",
      title: "Pontiac Sunfire",
      start_production: 1994,
      class: "Compact",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/5/55/1971_AMC_Javelin_SST_red_Kenosha_street.JPG/400px-1971_AMC_Javelin_SST_red_Kenosha_street.JPG",
      title: "AMC Javelin",
      start_production: 1967,
      class: "{{Unbulleted list| Pony car | Muscle car },},",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/c/cb/Jaguar_X-Type_Estate_front_20080731.jpg/400px-Jaguar_X-Type_Estate_front_20080731.jpg",
      title: "Jaguar X-Type",
      start_production: 2001,
      class: "Compact executive car",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/VW_Phaton_%282._Facelift%29_%E2%80%93_Frontansicht%2C_7._Mai_2011%2C_D%C3%BCsseldorf.jpg/400px-VW_Phaton_%282._Facelift%29_%E2%80%93_Frontansicht%2C_7._Mai_2011%2C_D%C3%BCsseldorf.jpg",
      title: "Volkswagen Phaeton",
      start_production: 2002,
      class: "Full-size luxury car",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/4/41/Pontiac_G6.jpg/400px-Pontiac_G6.jpg",
      title: "Pontiac G6",
      start_production: 2004,
      class: "Midsize",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/Ford500a.JPG/400px-Ford500a.JPG",
      title: "Ford Five Hundred",
      start_production: 2004,
      class: "Full-size",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/PontiacSolstice.jpg/400px-PontiacSolstice.jpg",
      title: "Pontiac Solstice",
      start_production: 2005,
      class: "Roadster, coupe",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/8/83/Fiat_tipo_f.jpg/400px-Fiat_tipo_f.jpg",
      title: "Fiat Tipo",
      start_production: 1988,
      class: "Small family car",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/1985-89_Plymouth_Reliant_K_LE.png/400px-1985-89_Plymouth_Reliant_K_LE.png",
      title: "Plymouth Reliant",
      start_production: 1981,
      class: "Mid-size",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/f/f6/1978_chevette.JPG/400px-1978_chevette.JPG",
      title: "Chevrolet Chevette",
      start_production: 1975,
      class: "Subcompact",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/c/c0/Seat_Leon_1.4_TSI_Start%26Stop_Style_%28III%29_%E2%80%93_Frontansicht%2C_10._August_2013%2C_Ratingen.jpg/400px-Seat_Leon_1.4_TSI_Start%26Stop_Style_%28III%29_%E2%80%93_Frontansicht%2C_10._August_2013%2C_Ratingen.jpg",
      title: "SEAT León",
      class: "Small family car",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/a/af/Chevrolet_Corsica_1994.jpg/400px-Chevrolet_Corsica_1994.jpg",
      title: "Chevrolet Corsica",
      start_production: 1987,
      class: "Compact car",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/2/28/1992_MX3_V6_24V.jpg/400px-1992_MX3_V6_24V.jpg",
      title: "Mazda MX-3",
      start_production: 1991,
      class: "Sport compact",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/f/fd/2000_TVR_Tuscan_4.0_Speed_Six_by_The_Car_Spy.jpg/400px-2000_TVR_Tuscan_4.0_Speed_Six_by_The_Car_Spy.jpg",
      title: "TVR Tuscan Speed Six",
      start_production: 1999,
      class: "Sports car",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/0/0c/Aston_Martin_DB9_coupe_02.jpg/400px-Aston_Martin_DB9_coupe_02.jpg",
      title: "Aston Martin DB9",
      start_production: 2004,
      class: "Grand tourer",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/4/4d/Pontiac_Catalina_front.jpg/400px-Pontiac_Catalina_front.jpg",
      title: "Pontiac Catalina",
      start_production: 1950,
      class: "Full-size",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/3/35/Oldsmobile_Toronado_0003.jpg/400px-Oldsmobile_Toronado_0003.jpg",
      title: "Oldsmobile Toronado",
      start_production: 1965,
      class: "Full-size personal luxury car",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/a/a3/Chrysler_Cirrus_--_01-27-2012.jpg/400px-Chrysler_Cirrus_--_01-27-2012.jpg",
      title: "Chrysler Cirrus",
      start_production: 1994,
      class: "Mid-size",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/2/2c/Mercedes_R_350_CDI_4MATIC_Lang_%28V251%29_Facelift_front_20101017.jpg/400px-Mercedes_R_350_CDI_4MATIC_Lang_%28V251%29_Facelift_front_20101017.jpg",
      title: "Mercedes-Benz R-Class",
      class: "Full-size CUV / Large MPV",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/8/85/Volvo_V50_1.6_D.jpg/400px-Volvo_V50_1.6_D.jpg",
      title: "Volvo V50",
      start_production: 2004,
      class: "Compact / Small family car",
    },
    {
      image:
        "https://upload.wikimedia.org/wikipedia/commons/thumb/f/f5/Audi_TT_Coup%C3%A9_2.0_TFSI_quattro_S-line_%288S%29_%E2%80%93_Frontansicht%2C_3._April_2015%2C_D%C3%BCsseldorf.jpg/400px-Audi_TT_Coup%C3%A9_2.0_TFSI_quattro_S-line_%288S%29_%E2%80%93_Frontansicht%2C_3._April_2015%2C_D%C3%BCsseldorf.jpg",
      title: "Audi TT",
      class: "Sport compact Sports car",
    },
  ];
</script>

<div class="grid grid-cols-3 gap-4 m-4">
  {#each data as car}
    <div
      class="w-full max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700 flex flex-col"
    >
      <div>
        <img class="p-8 rounded-t-lg" src={car.image} alt="product car" />
      </div>
      <div class="px-5 pb-5">
        <h5
          class="text-xl font-semibold tracking-tight text-gray-900 dark:text-white"
        >
          {car.title}
        </h5>

        <div class="flex items-center justify-between">
          <span class="text-xl font-bold text-gray-900 dark:text-white"
            >Rs 8.69 Lakh onwards</span
          >
          <a
            href="#"
            class="border hover:bg-gray-800 hover:text-white focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
            >Check On-Road Price</a
          >
        </div>
      </div>
    </div>
  {/each}
</div>
