nama : Bagas Ikhsan


Tugas javascript


Definisi + Contohnya


1. toString => digunakan untuk menggabung semua elemen array dan menjadikannya satu string, dipisahkan dengan koma.

contoh : 	let arr = ['bagas','ikhsan', 7];
		arr.toString();
	hasilnya :
		arr = ['bagas,ikhsan,7']
			

2. join => digunakan untuk menggabung semua elemen dari array menjadi  satu string dan pemisahnya bisa sesuai keinginan.

contoh : 	let arr = ['bagas','ikhsan', 7];
		arr.join('-'); --> 'bagas-ikhsan-7'
		arr.join(); --> 'bagas,ikhsan,7'
		arr.join('') --> 'bagasikhsan7'
			

3. push => digunakan untuk menambahkan elemen/item pada akhir array.

contoh : 	let arr = ['bagas','ikhsan', 7];
		arr.push('programmer');
	hasilnya :
		arr = ['bagas','ikhsan', 7, 'programmer']

4. pop => digunakan untuk menghapus elemen/ite pada akhir array.

contoh : 	let arr = ['bagas','ikhsan', 7];
		arr.pop();
	hasilnya :
		arr = ['bagas','ikhsan']

5. unshift => digunakan untuk menghapus elemen/item pada awal array.

contoh : 	let arr = ['bagas','ikhsan', 7];
		arr.unshift();
	hasilnya :
		arr = ['ikhsan', 7]

6. shift => digunakan untuk menambahakan elemen/item pada awal array.

contoh : 	let arr = ['bagas','ikhsan', 7];
		arr.shift('Aku');
	hasilnya :
		arr = ['Aku','bagas','ikhsan', 7]

7. splice => method yang bisa digunakan untuk menambahkan, menghapus, dan mengganti elemen/item.

	susunannya seperti ini :

		arr.splice(index , deleteCount, elemN) // maksudnya adalah index menunjukkan akan dimulai dari index keberapa , deleteCount menunjukkan akan menghapus berapa elemen, elemN menunjukkan elemen yg akan ditambahkan.

contoh : 	let arr = ['bagas','ikhsan', 7];
	a. untuk menghapus :

		arr.splice(1, 1); // maksudnya adalah ... dimulai dari index ke 1 dan menghapus 1 elemen yaitu 'ikhsan'.
	hasilnya :
		arr = ['bagas', 7]

	b. untuk menambah : // untuk menambah tanpa menghapus, kita hanya perlu menulis 0 pada deleteCount.

		arr.splice(1, 0, 'ikhsan') // ini akan menambahkan 'ikhsan' ditengah-tengah array.
	hasilnya :
		arr = ['bagas','ikhsan', 7];

	c. untuk mengganti:

		arr.splice(2, 1, 'programmer')
	hasilnya :
		arr = ['bagas','ikhsan','programmer']

8. concat => method yang digunakan untuk menggabung array dengan array yg lain.

contoh :	let depan = ['a','b','c'];
		let blakang = ['d','e','f'];
		depan.concat(blakang);

	hasilnya :
		['a','b','c','d','e','f']

9. slice => method yang digunakan untuk membuat salinan array ke array baru dengan item yg dipilih, dari awal sampai akhir (tetapi yg terakhir tidak termasuk). Array yang asli tidak dimodifikasi.

	susunannya seperti ini :

		arr.slice(start, end);


contoh :	let arr = ['bagas','ikhsan', 7, 10]
	

		arr.slice(2) --> [7, 10] // jika didalam slice() kita isi hanya satu angka saja, maka yang di copy mulai index tsb dalam contoh ini dari index ke 2 yaitu 7 sampai akhir dari array

		arr.slice(1,3) --> ['ikhsan', 7] // ingat yg terakhir tidak termasuk, jadi jika di akhir kita tulis 3, maka hanya akan mengambil index 1 sampai 2 saja.

10. map => method yang digunakan untuk menbuat array baru dan memanggil fungsi pada tiap elemen array serta menampilkan hasil dari fungsi tsb.

contoh : 	let arr = [5, 6, 7];

		let arrKaliDua = arr.map(kaliDua);

		function kaliDua(arr){
			return arr * 2;
		}

	hasilnya :
		arrKaliDua = [10, 12, 14]