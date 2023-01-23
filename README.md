# Start-Up-Match-Making
// Start Up Match Making

// Objectives
// Mampu memecahkan masalah yang diberikan. Mampu menggabungkan konsep looping / iteration dan conditional. Mampu membuat array dari string tertentu dan memanipulasi array. Mengerti keterhubungan satu function dengan function lainnya. Mengerti cara melemparkan data yang dikembalikan dari satu function kemudian digunakan sebagai parameter function lain.
// Restriction
// Tidak boleh menggunakan built-in function
// Hints
// Nama function haruslah splitJobCharacters, reverseJobCharacters, decryptJobCharacters, makingDreamTeam,
// dan startUpMatchMaking dan tidak boleh diganti dengan nama function lainnya. Untuk detail fungsi akan mengacu kepada Directions yang disebutkan di bawah.
// Directions
// Start-Up Match Making

// Di challenge kali ini kalian diberikan sebuah function startUpMatchMaking yang menerima satu parameter bertipe data string. Function ini menerima sebuah parameter bertipe data string, dan parameter ini berisikan nama dan job characters dari para pejuang start-up. dan value job characters disini di sajikan dalam bentuk disandikan/terenkripsi sehingga satu sama lain pada awalnya belum mengetahui apa job characters mereka masing-masing. Disini kalian di minta untuk membuat sebuah tim Start-Up dan mendekripsikan/decode job characters yang telah disandikan/terenkripsi, dan yang mana tim ini nanti akan di ikut sertakan ke dalam lomba Start-Up International. Berikut adalah proses atau cara kerja untuk function startUpMatchMaking:

// Pisahkan nama dan job characters menjadi array. Gunakan function splitJobCharacters.
// Putar balikkan value job characters yg telah disandikan. Gunakan function reverseJobCharacters.
// Decryptlah value job characters yg telah disandikan. Gunakan function decryptJobCharacters.
// Bentuklah sebuah tim dengan format array 2 dimensi yang tiap elementnya berisi nama dan job characters. Gunakan function makingDreamTeam.
// Berikut adalah kriteria function startUpMatchMaking:
// Harus memanfaatkan function splitJobCharacters, reverseJobCharacters, decryptJobCharacters, dan makingDreamTeam dan dipanggil di dalam function startUpMatchMaking secara berurutan. Function akan mengembalikan string berdasarkan hasil pengecekkan data start-up tim di function startUpMatchMaking. Function akan mengembalikan string Minimum 3 members in the team jika data start-upnya yang sudah diolah kurang dari 3 orang.
// Perhatikan contoh berikut:

// function splitJobCharacters(str) {
//   // Your code here
// }

// function reverseJobCharacters(arr) {
//   // Your code here
// }

// function decryptJobCharacters(arr) {
//   // Your code here
// }

// function makingDreamTeam(arr) {
//   // Your code here
// }


// function startUpMatchMaking(str) {
//   // Your code here
// }

// console.log(startUpMatchMaking('idaz-sfmutvi,anggara-sfutqji,fika-sfldbi'))
// // Match your Dream Start-Up Team
// console.log(startUpMatchMaking('eko-sfldbi,fajrin-sfmutvi,abdullah-sfutqji,anggara-sfutqji'))
// // Match your Dream Start-Up Team
// console.log(startUpMatchMaking('abdullah-sfldbi,fajrin-sfmutvi,samir-sfldbi,eko-sfmutvi,basil-sfmutvi'))
// // The job composition in the team is not suitable
// console.log(startUpMatchMaking('samir-sfmutvi,basil-sfutqji,eko-sfmutvi'))
// // The job composition in the team is not suitable
// console.log(startUpMatchMaking('samir-sfmutvi,basil-sfutqji'))
// // Minimum 3 members in the team
// SplitJobCharacters
// Diberikan sebuah function splitJobCharacters yang menerima satu parameter string. Dimana function ini akan memisahakan/splitting input str menjadi array dengan urutan nama dan job characters. Output dari function ini bertipe data array. Perhatikan contoh berikut:

// function splitJobCharacters(str) {
//   // Your code here

// }

// console.log(splitJobCharacters('idaz-sfmutvi,anggara-sfutqji,dear-sfldbi'));
// // [ 'idaz', 'sfmutvi', 'anggara', 'sfutqji', 'dear', 'sfldbi' ]
// console.log(splitJobCharacters('kurnia-sfutqji,adi-sfldbi,anggara-sfmutvi'));
// // [ 'kurnia', 'sfutqji', 'adi', 'sfldbi', 'anggara', 'sfmutvi' ]
// ReverseJobCharacters
// Diberikan sebuah function reverseJobCharacters yang menerima satu parameter array. Dimana function ini akan membalik value job characters bertipe data string di dalam data array . Output dari function ini bertipe data array dan value job characters bertipe data string hasil reversing. Perhatikan contoh berikut:

// function reverseJobCharacters(arr) {
//   // Your code here
// }

// console.log(reverseJobCharacters([ 'idaz', 'sfmutvi', 'anggara', 'sfutqji', 'dear', 'sfldbi' ]));
// // [ 'idaz', 'ivtumfs', 'anggara', 'ijqtufs', 'dear', 'ibdlfs' ]
// console.log(reverseJobCharacters([ 'kurnia', 'sfutqji', 'adi', 'sfldbi', 'anggara', 'sfmutvi' ]));
// // [ 'kurnia', 'ijqtufs', 'adi', 'ibdlfs', 'anggara', 'ivtumfs' ]
// DecryptJobCharacters
// Diberikan sebuah function decryptJobCharacters yang menerima satu parameter bertipe data array. Dimana function ini akan mendekripsikan/decode value job characters bertipe data string di dalam data array, dan cara kerjanya dari function ini ada menggeser setiap huruf menjadi huruf sebelumnya (ex:I menjadi H). Output dari function ini bertipe data array dan value job characters bertipe data string hasil decryption. Perhatikan contoh berikut:

// function decryptJobCharacters(arr) {
//   // (ex: I -> H, A -> Z, D -> C, O -> N, S -> R, T -> S, Z -> Y)
//   // Your code here
// }

// console.log(decryptJobCharacters([ 'idaz', 'ivtumfs', 'anggara', 'ijqtufs', 'dear', 'ibdlfs' ]));
// // [ 'idaz', 'hustler', 'anggara', 'hipster', 'dear', 'hacker' ]
// console.log(decryptJobCharacters([ 'kurnia', 'ijqtufs', 'adi', 'ibdlfs', 'anggara', 'ivtumfs' ]));
// // [ 'kurnia', 'hipster', 'adi', 'hacker', 'anggara', 'hustler' ]
// MakingTheDreamTeam
// Diberikan sebuah function makingDreamTeam yang menerima satu parameter bertipe data array. Dimana function ini akan mengelompokan data sebuah tim start-up dengan format array 2 dimensi yang tiap elementnya berisi nama dan job characters. Output dari function ini bertipe data array 2 dimensi. Perhatikan contoh berikut:

// function makingDreamTeam(arr) {
//   // Your code here
// }

// console.log(makingDreamTeam([ 'idaz', 'hustler', 'anggara', 'hipster', 'dear', 'hacker' ]));
// // [
// //   [ 'idaz', 'hustler' ],
// //   [ 'anggara', 'hipster' ],
// //   [ 'dear', 'hacker' ]
// // ]
// console.log(makingDreamTeam([ 'kurnia', 'hipster', 'adi', 'hacker', 'anggara', 'hustler' ]));
// // [
// //   [ 'kurnia', 'hipster' ],
// //   [ 'adi', 'hacker' ],
// //   [ 'anggara', 'hustler' ]
// // ]
// startUpMatchMaking
// Diberikan sebuah function startUpMatchMaking yang merupakan main function yang akan menggabungkan seluruh function yang sudah kita buat sebelumnya dengan aturan:

// Jika team startup memiliki character kurang dari 3 maka tampilkan Minimum 3 members in the team
// Jika di dalam team startup memiliki character dengan job hustler, hipster dan hacker maka tampilkan Match your dream Start-up team.
// Jika tidak maka tampilkan The job composition in the team is not suitable.
// console.log(startUpMatchMaking('idaz-sfmutvi,anggara-sfutqji,fika-sfldbi'))
// // Match your Dream Start-Up Team
// console.log(startUpMatchMaking('eko-sfldbi,fajrin-sfmutvi,abdullah-sfutqji,anggara-sfutqji'))
// // Match your Dream Start-Up Team
// console.log(startUpMatchMaking('abdullah-sfldbi,fajrin-sfmutvi,samir-sfldbi,eko-sfmutvi,basil-sfmutvi'))
// // The job composition in the team is not suitable
// console.log(startUpMatchMaking('samir-sfmutvi,basil-sfutqji,eko-sfmutvi'))
// // The job composition in the team is not suitable
// console.log(startUpMatchMaking('samir-sfmutvi,basil-sfutqji'))
// // Minimum 3 members in the team