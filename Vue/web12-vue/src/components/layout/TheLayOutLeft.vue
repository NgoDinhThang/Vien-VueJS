<template>
    <div class="layout-left">
            <div class="layout-left-logo">
                <button class="layout-left-logo-button"></button>
                <div class="layout-left-logo-image"><img src="" alt="" height="32px" style="margin-right: 5px;"> KẾ TOÁN
                </div>
            </div>
            <div class="layout-left-menu">

                <div class="layout-left-menu-item"><button>Tổng quan</button></div>
                <div class="layout-left-menu-item"><button>Tiền mặt</button></div>
                <div class="layout-left-menu-item"><button>Tiền gửi</button></div>
                <div class="layout-left-menu-item"><button>Mua hàng</button></div>
                <div class="layout-left-menu-item"><button>Bán hàng</button></div>
                <div class="layout-left-menu-item"><button>Quản lý hoá đơn</button></div>
                <div class="layout-left-menu-item"><button>Kho</button></div>
                <div class="layout-left-menu-item"><button>Công cụ dụng cụ</button></div>
                <div class="layout-left-menu-item"><button>Tài sản cố định</button></div>
                <div class="layout-left-menu-item"><button>Thuế</button></div>
                <div class="layout-left-menu-item"><button>Giá thành</button></div>
                <div class="layout-left-menu-item"><button>Tổng hợp</button></div>
                <div class="layout-left-menu-item"><button>Ngân sách</button></div>
                <div class="layout-left-menu-item"><button>Báo cáo</button></div>
                <div class="layout-left-menu-item"><button>Phân tích tài chính</button></div>
            </div>
            
        </div>
        
</template>
<style scoped>
    
        
        .layout-left {
            width: 178px;
            height: auto;
            background-color: #38393D;
            font-family: inherit;
            color: white;
            font-size: 13px;
        }
        
        .layout-left-logo {
            height: 48px;
            display: flex;
            text-align: center;
            align-items: center;
            padding-left: 24px;
        }
        
        .layout-left-logo-image {
            width: 96px;
            height: 32px;
            width: 32px;
            text-align: center;
            text-decoration-line: none;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            outline: none;
            text-transform: none;
            text-decoration: none;
            align-items: center;
            display: flex;
            text-decoration-color: rgb(0, 0, 238);
        }
        
        .layout-left-logo-button {
            background-image: url(../../assets/Resource/toggle.png);
            background-size: 24px;
            background-color: unset;
            width: 24px;
            height: 24px;
            border: none;
            right: 10px;

        }
        
        .layout-left-menu {
            display: grid;
        }
        
        .layout-left-menu button {
            background-color: unset;
            border: none;
            font-size: 13px;
            text-align: left;
            color: white;
            height: 42px;
            width: 170px;
            margin-left: 8px;
            margin-right: 0px;
        }
        
        .layout-left-menu-item {
            height: 42px;
            /* display: flex; */
            /* text-align: center; */
        }
        .layout-left-menu-item:hover {
            cursor: pointer;
            /* display: flex; */
            /* text-align: center; */
            background-color: rgba(235, 237, 240, 0.2);
        }
        
        
        g .nc-loop_dots-06-32 {
            width: 20px;
        }  

</style>
