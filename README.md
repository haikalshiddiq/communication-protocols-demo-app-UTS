# communication-protocols-demo-app-UTS

Silakan di download karena ada enhancement dibagian ini :

Changed:

Tambah CRUD lengkap GET/POST/PUT/PATCH/DELETE untuk:
/api/products
/api/users
/api/profiles
/api/orders
/api/transactions
Tambah shortcut classroom:
/api/user/profile
/api/order/transaction
Tambah endpoint daftar case UTS:
/api/uts/cases
Update P2 REST builder di UI supaya bisa pilih resource, bukan cuma products.
Update P8 UTS Evidence supaya menampilkan users, profiles, orders, transactions.
Update Postman collection dengan folder baru UTS REST Case Resources - Users Profiles Orders Transactions.
Tambah seed data baru untuk users, profiles, orders, transactions.
Update README endpoint list.

Kemudian update kedua :
Changed:

Tambah Quick UTS Method Matrix di P2 dan P8 untuk:
users
profiles
orders
transactions
masing-masing tombol GET, POST, PUT, PATCH, DELETE
Tombol DELETE sekarang repeatable: UI create temporary record dulu, lalu delete record itu, jadi tidak gagal kalau demo diulang.
Perbaiki gRPC web demo:
Tambah Quick Invoke untuk Predict, BatchPredict, HealthCheck
BatchPredict otomatis isi sample items[], jadi output tidak kosong.
HealthCheck HTTP/2 sekarang return status: SERVING, tidak stuck.
Real HTTP/2 punya timeout lebih pendek dan fallback fallbackConceptResponse kalau gRPC server/port 50051 bermasalah.
Update Postman collection: folder UTS REST case sekarang ada reset di awal.
Update README guidance.
