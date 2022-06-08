# UAS-AMBW-todo-list-app

Judul : to-do list 

-Michael Alexander = C14190058 : 
home page + detail

-Michael Kurniawan = C14190104 : 
add page todolist + addpage project
Database firebase

-Rensis Yehuda = C14190111 : missing page + report page

cara kerja : live share

---
*home page
-> memakai listview builder untuk menampilkan
project dan todo-list. Ada 2 button, yaitu
add project dan add todo-list. Ada icon untuk
menuju report page dan missing page. Icon missing page
memiliki badge dengan jumlah item yang telat.

*detail 
-> Detail ada 2 page, yaitu detail projek dan detail todolist.
Masing-masing ditampilkan dalam bentuk row untuk tiap atributnya.
Pada detail projek, akan ada listview untuk todolistnya, jika ditekan
akan mengarahkan ke detail todolist.

*add page (untuk to do list)-edit todolist page 
-> berisi textfield untuk tiap atribut, dan datepicker
untuk pemilihan waktunya.

*add page (untuk project list)-edit projectlist page 
-> berisi textfield untuk tiap atribut, dan datepicker
untuk pemilihan waktunya. Ada tombol untuk menambahkan
item-item todolist (ketika tombol tersebut ditekan,
akan mengarahkan ke add page untuk todolist).

*missing page (untuk item yang belum di checklist sampai waktu...)
-> memakai listview builder untuk menampilkan
project dan todo-list yang telat. 

*report page (untuk item yang sudah diselesaikan)
-> memakai listview builder untuk menampilkan
project dan todo-list yang sudah diselesaikan (bisa
di un-checked lagi jika tanpa sengaja user
menekan tombol selesai) 

---
NOTES :
- checklist berupa swipe gesture di item listviewnya.
- dataclass
*datclassProjek
	idProjek (int)
	namaprojek (String)
	
*datclassTodolist
	idtodolist (int)
	namatodolist (String)
	idProjek (int) ** 0=bukan termasuk projek, selain 0 termasuk bagian dari suatu projek
	tanggalselesai (datetime)
	tanggalreminder (datetime)
	status (String) **selesai/belum/telat
	
---
REFERENSI :
Datepicker
https://api.flutter.dev/flutter/material/showDatePicker.html

---




