<template>
    <div style="display:block">
        <div class="stats shadow" style=" margin-left:10% ;margin-bottom:20px;margin-top:20px">

            <div class="stat" style="">
                <div class="stat-figure text-primary">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                        class="inline-block w-8 h-8 stroke-current">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z">
                        </path>
                    </svg>
                </div>
                <div class="stat-title">关注</div>
                <div class="stat-value text-primary">25.6K</div>
                <div class="stat-desc"> 本月新增123位</div>
            </div>

            <div class="stat">
                <div class="stat-figure text-secondary">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
                        class="inline-block w-8 h-8 stroke-current">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M13 10V3L4 14h7v7l9-11h-7z"></path>
                    </svg>
                </div>
                <div class="stat-title">讨论</div>
                <div class="stat-value text-secondary">2.6M</div>
                <div class="stat-desc">比上月多21%</div>
            </div>

            <div class="stat">
                <div class="stat-figure text-secondary">
                    <div class="avatar online">
                        <div class="w-16 rounded-full">
                            <img src="https://daisyui.com/images/stock/photo-1534528741775-53994a69daeb.jpg" />
                        </div>
                    </div>
                </div>
                <div class="stat-value">30</div>
                <div class="stat-title">学时</div>
                <div class="stat-desc text-secondary">已学习56小时</div>
            </div>

        </div>
        
        <div  style="margin-left:20%     ;display:block ;width:200px; " class="stats bg-primary text-primary-content">

            <div class="stat">
                <div class="stat-title"></div>
                <div class="stat-value">
                    <button class="btn btn-bg btn-success">社区商城</button>
                </div>
                <div class="stat-actions">
                    <button class="btn btn-sm btn-success">购物车</button>
                </div>
            </div>

            <div class="stat">
                <div class="stat-title">余额</div>
                <div class="stat-value">89,400</div>
                <div class="stat-actions">
                    <button class="btn btn-sm">提现</button>
                    <button class="btn btn-sm">充值</button>
                </div>
            </div>

        </div>
        <ul class="menu bg-base-200 w-56 rounded-box" style="margin-left:20%;margin-bottom: 10px;margin-top:10px">
            <li><a>设置</a></li>
            <li><a>退出登陆</a></li>
            <li><a>注销</a></li>
        </ul>
    </div>
</template>
<style>
.stat{
}
</style>
