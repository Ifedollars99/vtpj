<template>
<div class="bg-gray-100 max-w-full h-full md:h-screen grid grid-cols-1 
md:grid md:grid-cols-3 md:pl-28 place-items-center justify-items-center 
 " >
  <div class="bg-white shadow-lg w-[300px]
   mt-3 md:mt-0 h-[200px] md:w-[300px] md:h-[300px] 
   lg:w-[500px] rounded-xl p-6 md:-ml-24 ml-0 lg:ml-0 ">
    <div class="flex flex-row justify-between" >
      <h1 class="text-2xl font-bold" >Sales Overview</h1>
      <i class="bi bi-three-dots text-gray-300 text-3xl"></i>
    </div>
    <div class="chart-container">
    <canvas id="myChart"></canvas>
  </div>
  </div>

    <div class="relative md:w-[200px] md:h-[300px] bg-green-600 rounded-xl
     p-6 text-white shadow-lg max-w-xs overflow-hidden mt-11 md:mt-0 lg:ml-16 xl:ml-0 md:ml-0 ml-0 ">
  <!-- Background Circle Overlay -->
  <div class="absolute inset-20 bg-green-200 opacity-20 rounded-full w-3/4 h-3/4 top-10 right-10"></div>

  <!-- Card Content -->
  <div class="relative  space-y-28">
    <div class="flex flex-row justify-between" >
    <h2 class="text-lg font-semibold mt-1">Total Sales</h2>
    <i class="bi bi-three-dots text-4xl text-gray-300"></i>
  </div>
  <div class="flex flex-col " >
    <div class="flex flex-row gap-1" >
    <p class="text-4xl font-bold mt-2">$892</p> 
    <div class=" flex flex-row justify-center rounded-2xl bg-gray-300 h-10 w-28 gap-3 mt-3" >
      <i class="bi bi-arrow-bar-up w-0.5 h-0.5 text-green-600 pt-2"></i>
       <h1 class="text-sm  text-green-600 pt-2" >0.2%</h1>
      </div>
    </div>
    <div class="border-b-2 border-gray-300 w-32" ></div>
    <p class="text-sm opacity-75 mt-1">Vs last month: $869.3M</p>
  </div>
  </div>
</div>

  <div class="flex flex-col gap-10 md:-ml-2 lg:-ml-36" >
  <div class="bg-white shadow-lg md:w-[200px] lg:w-[280px] md:h-[130px] rounded-lg px-6 md:mt-0 mt-11">
    <h1 class="text-2xl font-bold mt-3" >All Orders</h1>
    <div class="flex flex-row gap-4" >
    <h1 class="mt-3 text-5xl" >128.1k</h1>
    <div class="flex flex-row bg-green-200 gap-3 h-7 w-8 mt-4 md:-ml-5 lg:ml-0 ml-0" >
        <i class="bi bi-arrow-bar-up w-0.5 h-0.5 text-green-600"></i>
        <h1 class="text-sm  text-green-600" >56%</h1>
  </div>
  </div>
  </div>
  <div class="bg-white shadow-lg md:w-[200px] lg:w-[280px] md:h-[130px] rounded-lg px-6">
    <h1 class="text-2xl md:text-xl lg:text-2xl font-bold mt-3" >Order Created</h1>
    <div class="flex flex-row gap-4" >
    <h1 class="mt-3 text-5xl" >1,90M</h1>
    <div class="flex flex-row bg-red-200 md:-ml-5 lg:ml-0 ml-0 gap-3 h-7 w-12 mt-4" >
        <i class="bi bi-arrow-bar-up w-0.5 h-0.5 text-red-600"></i>
        <h1 class="text-sm  text-red-600" >2%</h1>
  </div>
  </div>
  </div>
   
  </div>
   <div class="md:grid md:grid-cols-2 md:gap-[400px] lg:gap-[550px] md:pl-16 lg:ml-16 
   md:px-4 lg:px-0 px-0 md:-mt-72 lg:-mt-96 xl:mt-60 "  >
  <div class="bg-white shadow-lg md:-mt-48 mt-16 md:my-2  md:w-[350px] md:h-[420px] lg:w-[500px] lg:h-[300px] rounded-lg">
    <div class="px-4 " > 
      <div class="flex flex-row justify-between" >
      <h1 class="text-xl font-bold" >Highest campaign</h1>
      <i class="bi bi-three-dots text-2xl text-gray-500"></i>
    </div>
    <div class="flex flex-row justify-around text-gray-500 mt-2" >
      <h1 class="text-sm -ml-7" >Influencer</h1>
      <h1 class="text-sm ml-2 md:ml-0 lg:ml-2">Spend</h1>
      <h1 class="text-sm -ml-20 md:ml-0 lg:-ml-20">Goal</h1>
      <h1 class="text-sm -ml-20 md:ml-0 lg:-ml-20" >Sales</h1>
    </div>
    <div class="flex flex-row justify-between mt-2" >
      <div class="flex flex-row gap-2" >
        <img src="https://cdn.dribbble.com/users/2030268/screenshots/6577285/human_planet_4x.jpg?resize=640x480&vertical=center"
        class="w-7 h-7 rounded-full" >
        <h1 class="text-lg font-mono" >Areif Poncol Muhammad</h1>
      </div>
      <h1 class="text-lg font-mono">$460</h1>
      <h1 class="text-lg font-mono">$880</h1>
      <h1 class="text-lg font-mono">$880</h1>
      <div class="flex flex-row bg-green-200 gap-3 h-7" >
        <i class="bi bi-arrow-bar-up w-0.5 h-0.5 text-green-600"></i>
        <h1 class="text-sm  text-green-600" >56%</h1>
      </div>
    </div>
    <div class="flex flex-row justify-between mt-2" >
      <div class="flex flex-row gap-2" >
        <img src="https://cdn.dribbble.com/users/2030268/screenshots/6577285/human_planet_4x.jpg?resize=640x480&vertical=center"
        class="w-7 h-7 rounded-full" >
        <h1 class="text-lg font-mono" >Li Congwei Montreal</h1>
      </div>
      <h1 class="text-lg font-mono">$200</h1>
      <h1 class="text-lg font-mono">$250</h1>
      <h1 class="text-lg font-mono">$490</h1>
      <div class="flex flex-row bg-green-200 gap-3 h-7" >
        <i class="bi bi-arrow-bar-up w-0.5 h-0.5 text-green-600"></i>
        <h1 class="text-sm  text-green-600" >12%</h1>
      </div>
    </div>
    <div class="flex flex-row justify-between mt-2" >
      <div class="flex flex-row gap-2" >
        <img src="https://cdn.dribbble.com/users/2030268/screenshots/6577285/human_planet_4x.jpg?resize=640x480&vertical=center"
        class="w-7 h-7 rounded-full" >
        <h1 class="text-lg font-mono" >Alex Farid Anggara</h1>
      </div>
      <h1 class="text-lg font-mono">$820</h1>
      <h1 class="text-lg font-mono">$550</h1>
      <h1 class="text-lg font-mono">$722</h1>
      <div class="flex flex-row bg-green-200 gap-3 h-7" >
        <i class="bi bi-arrow-bar-up w-0.5 h-0.5 text-green-600"></i>
        <h1 class="text-sm  text-green-600" >11,2%</h1>
      </div>
    </div>
    <div class="flex flex-row justify-between mt-2" >
      <div class="flex flex-row gap-2" >
        <img src="https://cdn.dribbble.com/users/2030268/screenshots/6577285/human_planet_4x.jpg?resize=640x480&vertical=center"
        class="w-7 h-7 rounded-full" >
        <h1 class="text-lg font-mono" >Angga Dwi Sasongro</h1>
      </div>
      <h1 class="text-lg font-mono">$460</h1>
      <h1 class="text-lg font-mono">$880</h1>
      <h1 class="text-lg font-mono">$880</h1>
      <div class="flex flex-row bg-red-200 gap-3 h-7" >
        <i class="bi bi-arrow-bar-up w-0.5 h-0.5 text-red-600"></i>
        <h1 class="text-sm  text-red-600" >0.1%</h1>
      </div>
    </div>
    </div>
  </div>
  <div class="bg-white shadow-lg md:w-[300px] md:h-[400px] lg:w-[550px] lg:h-[300px] rounded-lg md:-mt-48 mt-8">
    <div class="flex flex-row justify-between px-4 mt-2" >
      <h1 class="text-2xl font-bold" >Customer by time</h1>
      <i class="bi bi-three-dots text-gray-300 text-3xl"></i>
    </div>

    <div class="p-6">
    <div class="grid grid-cols-8 gap-2">
        <!-- Labels on the left side -->
        <div class="col-span-1 text-right mr-2">
          <div class="flex flex-row gap-2" >
          <i class="bi bi-record-circle-fill text-gray-200"></i> 
          <p class="text-gray-500">500></p>
        </div>
          <div class="flex flex-row gap-2" >
          <i class="bi bi-record-circle-fill text-gray-300"></i> 
          <p class="text-gray-500">600></p>
        </div>
          <div class="flex flex-row gap-2" >
          <i class="bi bi-record-circle-fill text-green-300"></i> 
          <p class="text-gray-500">700></p>
        </div>
          <div class="flex flex-row gap-2" >
          <i class="bi bi-record-circle-fill text-green-400"></i> 
          <p class="text-gray-500">800></p>
        </div>
           
        </div>
        
        <!-- Heatmap grid -->
        <div class="col-span-7">
            <div class="grid grid-cols-7 gap-2">
                <!-- Sunday to Saturday column labels -->
                <div class="h-8 bg-gray-100 rounded"></div>
                <div class="h-8 bg-gray-200 rounded"></div>
                <div class="h-8 bg-green-300 rounded"></div>
                <div class="h-8 bg-green-400 rounded"></div>
                <div class="h-8 bg-green-500 rounded"></div>
                <div class="h-8 bg-green-300 rounded"></div>
                <div class="h-8 bg-gray-100 rounded"></div>

                <div class="h-8 bg-gray-100 rounded"></div>
                <div class="h-8 bg-gray-200 rounded"></div>
                <div class="h-8 bg-green-300 rounded"></div>
                <div class="h-8 bg-green-400 rounded"></div>
                <div class="h-8 bg-green-500 rounded"></div>
                <div class="h-8 bg-green-300 rounded"></div>
                <div class="h-8 bg-gray-100 rounded"></div>
                
                <!-- Heatmap cells -->
                <!-- Adjust the background color for each cell to reflect different levels -->
                <div class="h-8 bg-gray-100 rounded"></div>
                <div class="h-8 bg-gray-200 rounded"></div>
                <div class="h-8 bg-green-300 rounded"></div>
                <div class="h-8 bg-green-400 rounded"></div>
                <div class="h-8 bg-green-500 rounded"></div>
                <div class="h-8 bg-green-300 rounded"></div>
                <div class="h-8 bg-gray-100 rounded"></div>
                
                <!-- Repeat the cells for each row with different colors -->
                <div class="h-8 bg-gray-100 rounded"></div>
                <div class="h-8 bg-gray-200 rounded"></div>
                <div class="h-8 bg-green-400 rounded"></div>
                <div class="h-8 bg-green-500 rounded"></div>
                <div class="h-8 bg-green-500 rounded"></div>
                <div class="h-8 bg-green-300 rounded"></div>
                <div class="h-8 bg-gray-100 rounded"></div>

                <span class="text-gray-500 text-center">Sun</span>
                <span class="text-gray-500 text-center">Mon</span>
                <span class="text-gray-500 text-center">Tue</span>
                <span class="text-gray-500 text-center">Wed</span>
                <span class="text-gray-500 text-center">Thu</span>
                <span class="text-gray-500 text-center">Fri</span>
                <span class="text-gray-500 text-center">Sat</span>
                <!-- Add more rows here to match the pattern -->
            </div>
        </div>
    </div>
</div>

  </div>
  </div>
</div>

  
</template>

<script>
import Chart from 'chart.js/auto';


const verticalLinePlugin = {
  id: 'verticalLinePlugin',
  afterDraw: (chart) => {
    const ctx = chart.ctx;
    const xValue = chart.scales.x.getPixelForValue('Mar 23'); // Change the date to match your x-axis label

    ctx.save();
    ctx.strokeStyle = 'green'; // Color of the vertical line
    ctx.lineWidth = 0.5;

    ctx.beginPath();
    ctx.moveTo(xValue, chart.chartArea.top);
    ctx.lineTo(xValue, chart.chartArea.bottom);
    ctx.stroke();
    ctx.restore();
  }
};


const aprilContainerPlugin = {
  id: 'aprilContainerPlugin',
  afterDraw: (chart) => {
    const ctx = chart.ctx;
    const xValue = chart.scales.x.getPixelForValue('Apr 23'); // April position
    const yValue = chart.scales.y.getPixelForValue(600); // Adjust the y-value as needed

    ctx.save();
    ctx.fillStyle = 'white'; // Background color for the container
    ctx.strokeStyle = 'black'; // Outline color
    ctx.lineWidth = 0.09;

    // Draw the rounded rectangle
    const boxWidth = 120; // Width of the container
    const boxHeight = 60; // Height of the container
    const radius = 10; // Corner radius

    // Calculate the rectangle's top-left corner
    const rectX = xValue - boxWidth / 2;
    const rectY = yValue - boxHeight / 2;

    // Begin path for rounded rectangle
    ctx.beginPath();
    ctx.moveTo(rectX + radius, rectY);
    ctx.lineTo(rectX + boxWidth - radius, rectY);
    ctx.quadraticCurveTo(rectX + boxWidth, rectY, rectX + boxWidth, rectY + radius);
    ctx.lineTo(rectX + boxWidth, rectY + boxHeight - radius);
    ctx.quadraticCurveTo(rectX + boxWidth, rectY + boxHeight, rectX + boxWidth - radius, rectY + boxHeight);
    ctx.lineTo(rectX + radius, rectY + boxHeight);
    ctx.quadraticCurveTo(rectX, rectY + boxHeight, rectX, rectY + boxHeight - radius);
    ctx.lineTo(rectX, rectY + radius);
    ctx.quadraticCurveTo(rectX, rectY, rectX + radius, rectY);
    ctx.closePath();

    ctx.fill(); // Fill the rectangle
    ctx.stroke(); // Outline the rectangle

    // Add text inside the container
    ctx.fillStyle = 'black'; // Text color
    ctx.font = '14px Arial'; // Font style
    ctx.textAlign = 'center'; // Center text alignment
    ctx.textBaseline = 'middle'; // Vertical alignment
    ctx.fillText('MARKET 2024 ', xValue, yValue); // Draw text centered in the box

    ctx.restore();
  }
};


export default {
  name: 'SalesGoalsChart',
  mounted() {
    const ctx = document.getElementById('myChart').getContext('2d');

    const data = {
      labels: ['Jan 23', 'Feb 23', 'Mar 23', 'Apr 23', 'May 23'],
      datasets: [
        {
          label: '',
      data: [200, 400, 750, 820, 400, 830  ], // Alternating values for a zig-zag effect
      borderColor: 'green', // Green line color (adjust as needed)
      borderWidth: 2,
      pointBackgroundColor: 'white',
      pointBorderColor: 'green',
      pointBorderWidth: 2,
      tension: 0, // Straight line for sharp zig-zag effect
    },
    {
      label: '',
      data: [400, 100, 420, 400, 800], // Example data for Goals line
      borderColor: '#ff6347',
      borderWidth: 2,
      pointBackgroundColor: 'white',
      pointBorderColor: '#ff6347',
      pointBorderWidth: 2,
      borderDash: [10, 5],
      tension: 0, // Slight curve for the Goals line, if desired
    },

      ],
    };

    const config = {
      type: 'line',
      data: data,
      options: {
        responsive: true,
        scales: {
          y: {
        beginAtZero: true,
        ticks: {
          callback: function(value) {
            // Customize specific values to display with custom labels
            if (value === 0) return '$0';
            if (value === 400) return '$400M';
            if (value === 800) return '$800M';
            if (value === 1200) return '$1.2B';
            return ''; // Hide other values
          },
          font: {
            size: 10,
            weight: 'bold',
          },
          color: '#333',
        },
        min: 0,  // Minimum y-axis value
        max: 1200, // Maximum y-axis value
      },
        },
        plugins: {
          tooltip: {
            callbacks: {
              title: function (tooltipItems) {
                return `Date: ${tooltipItems[0].label}`;
              },
              label: function (tooltipItem) {
                return `${tooltipItem.dataset.label}: $${tooltipItem.raw}M`;
              },
            },
            backgroundColor: 'rgba(255, 255, 255, 0.9)',
            titleColor: '#333',
            bodyColor: '#333',
            borderColor: '#ddd',
            borderWidth: 1,
            titleFont: {
          size: 16, // Increase this value for larger title text
          weight: 'bold',
        },
          },
        },
      },
      plugins: [verticalLinePlugin, aprilContainerPlugin],
    };

    new Chart(ctx, config);
  },
};
</script>

<style scoped>
.chart-container {
  max-width: 600px;
  margin: auto;
}
</style> 

 