<template>
    <header class="default heade-sticky">
        <div class="un-title-page">
            <h1>{{ title ? title : ''  }}</h1>
        </div>
        <div class="un-block-right">

            <div class="un-notification">
                <a href="#" aria-label="activity">
                    <i class="ri-notification-line"></i>
                </a>
                <span class="bull-activity"></span>
            </div>

            <div class="un-user-profile">
                <a href="#" aria-label="profile">
                    <picture>
                        <source srcset="~/assets/images/avatar/11.webp" type="image/webp">
                        <img class="img-avatar" src="~/assets/images/avatar/11.jpg" alt="">
                    </picture>
                </a>
            </div>

            <!-- menu-sidebar -->
            <div class="menu-sidebar">
                <button type="button" name="sidebarMenu" aria-label="sidebarMenu" class="btn"
                    data-bs-toggle="modal" data-bs-target="#mdllSidebar-connected">
                    <svg xmlns="http://www.w3.org/2000/svg" width="19" height="9.3" viewBox="0 0 19 9.3">
                        <g id="Group_8081" data-name="Group 8081" transform="translate(-329 -37)">
                            <rect id="Rectangle_3986" data-name="Rectangle 3986" width="19" height="2.3"
                                rx="1.15" transform="translate(329 37)" fill="#222032" />
                            <rect id="Rectangle_3987" data-name="Rectangle 3987" width="19" height="2.3"
                                rx="1.15" transform="translate(329 44)" fill="#222032" />
                        </g>
                    </svg>
                </button>
            </div>
        </div>
    </header>
</template>

<script>
export default {
  name: 'AppHeader',
  props: {
    title: {
      type: String,
      required: true
    }
  },
}
</script>