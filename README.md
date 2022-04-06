# DEPRECATED! Tài liệu này đã không còn được cập nhật
## VMS_Developer_API_doc
Tài liệu này đang được xây dựng dựa trên mã nguồn VMS build ngày 10/03/2022 (commit [3e5570649a16360e1b2cd9c18196f8faf183392b](https://github.com/lesongvi/ViMinerShop/commit/3e5570649a16360e1b2cd9c18196f8faf183392b)), quickjump [BitGeeks/ProjectAERT1_Javascript](https://github.com/BitGeeks/ProjectAERT1_Javascript), [BitGeeks/ProjectAERT2_PHP](https://github.com/BitGeeks/ProjectAERT2_PHP), [BitGeeks/ProjectAERT3_Java](https://github.com/BitGeeks/ProjectAERT3_Java)

| ID | Method | Endpoint | Request | Response | Add. | Description
| --- | --- | --- | --- | --- | --- | --- |
| 1 | POST | ```/api/users/register``` | [account.service.ts#L22](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L22) | [UsersController.cs#L166](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L166) | None | Đăng ký |
| 2 | POST | ```/api/users/authenticate``` | [account.service.ts#L33](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L33) | [UsersController.cs#L40](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L40) | None | Đăng nhập |
| 3 | POST | ```/api/users/:id``` | [account.service.ts#L49](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L49) | [UsersController.cs#L40](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L40) | Authorize | Nhận thông tin người dùng |
| 4 | PUT | ```/api/users/update``` | [account.service.ts#L69](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L69) | [UsersController.cs#L128](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L128) | Authorize | Cập nhật thông tin người dùng |
| 5 | PUT | ```/api/users/subscription``` | [account.service.ts#L73](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L73) | [UsersController.cs#L149](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L149) | Authorize | Toggle Subscription |
| 6 | DELETE | ```/api/users/delete/:id``` | None | [UsersController.cs#L182](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L182) | Authorize, Option | Xóa tài khoản người dùng |
| 7 | GET | ```/api/users/records/all``` | [account.service.ts#L57](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L57) | [UsersController.cs#L190](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L190) | Authorize | Lấy bản ghi |
| 8 | GET | ```/api/users/records/count``` | [account.service.ts#L207](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L207) | [UsersController.cs#L199](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L199) | Authorize | Đếm bản ghi |
| 9 | POST | ```/api/users/register/validate``` | [account.service.ts#L77](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L77) | [UsersController.cs#L208](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L208) | Authorize | Xác thực email |
| 10 | POST | ```/api/users/referrals/create``` | [account.service.ts#L187](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L187) | [UsersController.cs#L217](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L217) | Authorize | Tạo referral |
| 11 | GET | ```/api/users/referrals/all``` | [account.service.ts#L190](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L190) | [UsersController.cs#L234](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L234) | Authorize | Lấy danh sách referral của người dùng |
| 12 | POST | ```/api/users/referrals/resend``` | [account.service.ts#L53](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L53) | [UsersController.cs#L250](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L250) | Authorize | Gửi lại mã xác minh đăng ký |
| 13 | GET | ```/api/users/stats/point``` | [account.service.ts#L194](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L194) | [UsersController.cs#L265](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L265) | Authorize | Lấy điểm của người dùng |
| 14 | POST | ```/api/users/soldoutnotify``` | [account.service.ts#L198](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L198) | [UsersController.cs#L281](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UsersController.cs#L281) | Authorize | Lưu đăng ký đặt máy đào đã được bán hết |
| 15 | GET | ```/api/useraddresses``` | None | [UserAddressesController.cs#L27](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UserAddressesController.cs#L27) | Authorize, Option | Lấy dữ liệu địa chỉ của người dùng |
| 16 | GET | ```/api/useraddresses/:id``` | None | [UserAddressesController.cs#L34](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UserAddressesController.cs#L34) | Authorize, Option | Tìm dữ liệu theo mã định danh |
| 17 | PUT | ```/api/useraddresses/update``` | [account.service.ts#L147](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L147) | [UserAddressesController.cs#L81](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UserAddressesController.cs#L81) | Authorize | Cập nhật dữ liệu địa chỉ của người dùng |
| 18 | POST | ```/api/useraddresses/add``` | [account.service.ts#L131](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L131) | [UserAddressesController.cs#L114](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UserAddressesController.cs#114) | Authorize | Thêm dữ liệu địa chỉ của người dùng |
| 19 | POST | ```/api/useraddresses/setdefault``` | [account.service.ts#L172](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L172) | [UserAddressesController.cs#L154](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UserAddressesController.cs#154) | Authorize | Thêm dữ liệu địa chỉ của người dùng |
| 20 | DELETE | ```/api/useraddresses/remove/:id``` | [account.service.ts#L168](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L168) | [UserAddressesController.cs#L183](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/UserAddressesController.cs#183) | Authorize | Xoá dữ liệu địa chỉ của người dùng |
| 21 | GET | ```/api/slideimages``` | [notice.service.ts#L20](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/notice.service.ts#L20) | [SlideImagesController.cs#L24](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/SlideImagesController.cs#L24) | None | Lấy thông tin slide |
| 22 | GET | ```/api/shippingmethods/all``` | [account.service.ts#L178](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L178) | [ShippingMethodsController.cs#L24](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/ShippingMethodsController.cs#L24) | Authorize | Lấy thông tin phương thức vận chuyển |
| 23 | GET | ```/api/shippingmethods/flag/:flag``` | [account.service.ts#L182](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/account.service.ts#L182) | [ShippingMethodsController.cs#L31](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/ShippingMethodsController.cs#L31) | Authorize | Lấy thông tin phương thức vận chuyển theo flag |
| 24 | GET | ```/api/repairs/all``` | [repair.service.ts#L18](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopApp/src/app/services/repair.service.ts#L18) | [RepairsController.cs#L34](https://github.com/lesongvi/ViMinerShop/blob/main/ViMinerShopAPI/ViMinerShopAPI/Controllers/RepairsController.cs#34) | Authorize | Lấy danh sách tất cả phiếu sửa chữa máy đào |
