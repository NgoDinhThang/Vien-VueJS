<template>
    <div class="layout-right">
            <div class="header">
                <div class="header-combobox">
                    <div class="text-combobox">Nhà hàng biển đông</div>
                    <button class="btn-header"></button>
                </div>
                <div class="header-user">
                    <img src="../../assets/img/default-avatar.jpg" alt="" class="user-img">
                    <div class="text-combobox user-text">Nguyễn Văn Mạnh</div>
                    <button class="btn-user"></button>

                </div>
            </div>
            <div class="grid">

                <div class="table-header">
                    <div class="title">
                        <h2>Danh sách nhân viên</h2>
                        <div class="Ontap">
                            <button class="m-button" id="btn-addNV">Thêm nhân viên</button>


                        </div>
                    </div>
                    <div class="search">
                        <div class="m-field-input">
                            <input type="text" class="m-ip" placeholder="tìm theo mã,tên hoặc số điện thoại ">
                            <div class="m-ip-img">
                                <img src="../../assets/icon/search.png" alt="">

                            </div>
                        </div>
                        <div class="m-field-input m-cbb" id="btnComboboxLeft">
                            <input type="text" placeholder="tất cả phòng ban" class="m-ip m-ip-right">
                            <button class="cbb-button" id="btnLeft">

                            </button>
                            <div class="cbb-data m-left">
                                <div class="cbb-data-item data-left">Trạng thái 1</div>
                                <div class="cbb-data-item data-left">Trạng thái 2</div>
                                <div class="cbb-data-item data-left">Trạng thái 3</div>
                            </div>
                        </div>
                        <div class="m-field-input m-cbb" id="btnComboboxRight">
                            <input type="text" placeholder="tất cả vị trí" class="m-ip m-ip-right">
                            <button class="cbb-button" id="btnRight">
                            </button>
                            <div class="cbb-data m-right">
                                <div class="cbb-data-item data-right">Trạng thái 1</div>
                                <div class="cbb-data-item data-right">Trạng thái 2</div>
                                <div class="cbb-data-item data-right">Trạng thái 3</div>
                            </div>
                        </div>
                        <button class="refresh" id="refresh"></button>
                        <button class="delete" id="delete"></button>
                    </div>

                </div>

                <table border="0px" class="m-table" id="table-nhanvien">
                    <thead class="head-table">
                        <th style="padding-left: 12px;" propertyName="CustomerCode">Mã nhân viên</th>
                        <th propertyName="FullName">Họ tên</th>
                        <th propertyName="Gender">Giới tính</th>
                        <th style="text-align: center;" propertyName="DateOfBirth">Ngày sinh</th>
                        <th propertyName="PhoneNumber">Điện thoại</th>
                        <th propertyName="Email">Email</th>
                        <th propertyName="CompanyName">Công ty</th>
                        <th propertyName="DebitAmount">Số tiền nợ</th>

                    </thead>
                    <tbody>

                    </tbody>
                </table>
            </div>
            <div class="footer">
                <div class="hienthi">Hiển thị 1-10/1000 nhân viên</div>
                <div class="Trang">
                    <button class="first icon"><i class="fas fa-angle-double-left"></i></button>
                    <button class="pre icon"><i class="fas fa-angle-left"></i></button>
                    <button class="page" style="background-color: #2FBE8E; color: white;">1</button>
                    <button class="page">2</button>
                    <button class="page">3</button>
                    <button class="page">4</button>
                    <button class="next icon"><i class="fas fa-chevron-right"></i></button>
                    <button class="last icon"><i class="fas fa-angle-double-right"></i></button>
                </div>
                <div class="soluong">10 nhân viên/trang</div>

            </div>
            <div class="toast-message-box">
                <div class="msg-box message-info" id="toast-info">
                    <div class="msg-icon"><i class="fas fa-info-circle"></i></div>
                    <div class="msg-text-info">Thêm mới thành công</div>
                    <div class="msg-cancel"><i class="fas fa-times"></i></div>
                </div>
                <div class=" msg-box message-error">
                    <div class="msg-icon error"><i class="fas fa-exclamation-triangle"></i></div>
                    <div class="msg-text-error">Lỗi</div>
                    <div class="msg-cancel error"><i class="fas fa-times"></i></div>
                </div>
            </div>
        </div>
</template>
<style lang="scss" scoped>
@import url('../base/button.css');
@import url('../base/combobox.css');
@import url('../base/input.css');
@import url('../base/table.css');
@import url('../base/footer.css');
@import url('../base/toastMessage.css');
@import url('../base/dialog.css');
.layout-right {
    width: calc(100% - 200px);
    position: relative;
}

.header {
    height: 48px;
    display: flex;
    border-bottom: 1px solid #ccc;
}

.header-combobox {
    /* position: relative; */
    /* display: flex; */
    width: 200px;
    margin-left: 0px;
    height: 48px;
}

.btn-header {
    position: absolute;
    width: 12px;
    height: 12px;
    background-image: url('../../assets/img/SeekPng.com_chevron-logo-png_1350793.png');
    background-size: 12px 12px;
    border: none;
    margin-top: 20px;
    margin-left: 175px;
    background-color: unset;
    cursor: pointer;
}

.btn-header:hover {
    background-color: #E9EBEE;
}

.text-combobox {
    position: absolute;
    text-align: center;
    width: auto;
    padding-left: 40px;
    line-height: 48px;
    font-size: 13px;
}

.user-img {
    width: 35px;
    border-radius: 50%;
    margin-top: 8px;
}

.btn-user {
    background-image: url('../../assets/icon/option.png');
    background-repeat: no-repeat;
    background-size: 30px 30px;
    border: none;
    background-position: center center;
    background-color: unset;
    width: 40px;
    height: 40px;
}

.btn-user:hover {
    cursor: pointer;
}

.header-user {
    position: absolute;
    width: 200px;
    right: 20px;
    display: flex;
    justify-content: space-between;
}

.text-combobox.user-text {
    margin-left: 8px;
}

.m-table {
    right: 20px;
}

.grid {
    width: calc(100% - 20px);
    padding-left: 10px;
}

.title {
    display: flex;
    height: 65px;
}

.search {
    display: flex;
}

.m-cbb:hover {
    outline-color: #019160;
}

.refresh {
    width: 40px;
    height: 35px;
    right: 40px;
    position: absolute;
    background-image: url('../../assets/icon/refresh.png');
    background-position: center center;
    background-repeat: no-repeat;
    border: 1px solid #ccc;
    background-color: unset;
    border-radius: 4px;
}

.delete {
    width: 40px;
    height: 35px;
    right: 80px;
    position: absolute;
    background-image: url('../../assets/icon/delete.png');
    background-size: 16px;
    background-position: center center;
    background-repeat: no-repeat;
    border: 1px solid #ccc;
    background-color: unset;
    border-radius: 4px;
}

.refresh:hover {
    cursor: pointer;
    background-color: whitesmoke;
}

.delete:hover {
    cursor: pointer;
    background-color: whitesmoke;
}

</style>
<script>
export default {
    
}
</script>