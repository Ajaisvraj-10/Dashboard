<template>
    <div class="user_main">
        <div class="wrap_div">
          <div class="header_cntct">
          <div class="txt_quick_strt"> Quick start</div>
          <div class="hedr_box1">
              <div>
                  <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M11 0C4.925 0 0 4.925 0 11s4.925 11 11 11 11-4.925 11-11A11 11 0 0 0 11 0z" fill="#E0F5F1"></path><path d="M14.29 8.33a.69.69 0 0 1 0 1l-4.34 4.34a.71.71 0 0 1-1 0l-2.24-2.26a.707.707 0 1 1 1-1l1.79 1.77 3.8-3.85a.71.71 0 0 1 .99 0z" fill="#009A79"></path></svg>
              </div>
              <div class="box1_txt">Understand the Team Inbox</div>
          </div>
          <!-- -->
          <div class="btw_line"></div>
          <!--  -->
          <div class="hedr_box1">
              <div class="contct_num2">2</div>
              <div class="box1_txt">Add support channels</div>
              <div class="cnct_btn_div"><button class="cnct_btn">Connect</button></div>
          </div>
          <!--  -->
          <div class="btw_line"></div>
          <!--  -->
          <div class="hedr_box1">
              <div class="contct_num2">3</div>
              <div class="box1_txt">Provide intelligent self service</div>
          </div>
      </div>
  </div>
      
      <!--  -->
      <!-- sidebar -->
      <div class="sidebar_container">
          <div class="chat_baloon">
              <img src="/dashboard/chat-balloon.png" alt="">
          </div>
          <div class="dashbrd">
              <img src="/dashboard/dashboard.png" alt="">
          </div>
          <div class="message">
              <img src="/dashboard/message.png" alt="">
          </div>
          
          <div class="user">
              <img src="/dashboard/social-network_round.png" alt="">
          </div>
          <router-link :to="{ name: 'home'}">
          <div class="people">
              <img src="/dashboard/user_rounded.png" alt="">
          </div>
        </router-link>
          <div class="open_book">
              <img src="/dashboard/open-book.png" alt="">
          </div>
          <div class="chat">
              <img src="/dashboard/chat.png" alt="">
          </div>
          <div class="mega_phone">
              <img src="/dashboard/megaphone.png" alt="">
          </div>
          <div class="stats">
              <img src="/dashboard/stats.png" alt="">
          </div>
          <div class="settings">
              <img src="/dashboard/settings.png" alt="">
          </div>
          <div class="colr_menu">
              <img src="https://accounts.freshworks.com/omnibar/assets/stable/switcher.svg?v=v2.1.2-1695193281" alt="" role="presentation">
          </div>
      </div>
      <!--  -->
      <!-- secnd_navbar -->

      <div class="wrap_div2">
        <div class="scnd_thrd_wrap">
            <div class="scndry_navbar">
          <div class="inptdiv">
              <svg  class="serch_img" width="16" height="16" viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path fill-opacity=".01" fill="#FFF" opacity=".01" d="M1 1h14v14H1z"></path><g stroke="#000"><path stroke-linecap="round" d="M9.733 9.733L14.5 14.5"></path><path d="M11.033 6.267a4.767 4.767 0 1 1-9.533 0 4.767 4.767 0 0 1 9.533 0z"></path></g></g></svg>
              <input v-model="searchQuery"  type="text" placeholder="Search your CRM..."> <button @click="performSearch">Search</button>
              <!-- <div class="popup" v-if="showSearchResults">
                <div class="popup-content">
      <h2 class="popup-title">Search Results</h2>
      <ul class="popup-list">
        <li v-for="(result, index) in searchResults" :key="index" class="popup-item">
          <a class="search_name" @click="showDetails(result)">{{ result.name }}</a>
        </li>
      </ul>
      <button @click="closePopup" class="popup-close-button">Close</button>
    </div>
    </div> -->
          </div>
          <div class="inner_navbar">
              <div class="inner_txt">Your trial ends in 14 days
                  <svg class="warn_img"  data-toggle="tooltip" data-placement="bottom" data-html="true" data-original-title="Your current plan is <b>Freshworks CS Suite Enterprise</b>" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><g data-name="Layer 1"><path d="M10 20a10 10 0 1 1 10-10 10 10 0 0 1-10 10zm0-18.6a8.6 8.6 0 1 0 8.6 8.6A8.61 8.61 0 0 0 10 1.4z"></path><path d="M11.29 13.33h-.59V9.45a.7.7 0 0 0-.7-.7H8.71a.7.7 0 1 0 0 1.4h.59v3.18h-.59a.7.7 0 1 0 0 1.4h2.58a.7.7 0 0 0 0-1.4zM10 5.27a1.05 1.05 0 1 1-1 1.05 1 1 0 0 1 1-1.05z"></path></g></svg>
              </div>
             <div class="explre_btn_div"> <button class="explre_btn">Explore plans</button></div>
             <div class="explre_btn_div"> <button class="explre_btn">Request Demo</button></div>
             <div class="explre_btn_div"> <button class="explre_btn">Recommended Features</button></div>
          </div>
          <!--  -->
          <div class="navbr_divider"></div>
          <div class="plus_btn"><img src="/dashboard/plus.png" alt=""></div>
          <div class="navbr_divider"></div>
          <div class="plus_btn"><img src="/dashboard/bell.png" alt=""></div>
          <div class="navbr_divider"></div>
          <div class="name_a">A</div>
      </div>
      <!--  -->
      <!-- thrd_bar -->
      <div class="thrd_bar">
          <div class="section_one">
            <div @click="setCurrentBtn('btn0')" :class="current_btn == 'btn0' ? 'active_btn' : ''" class="new_contct_sect">
            <div class="txt_mycontct">All Users</div>
            <div class="txt_four">4</div>
            <!-- <div class="close_icon"><img src="/dashboard/close.png" alt=""></div> -->
        </div>  
              <!--  new contacts-->
              <div @click="setCurrentBtn('btn1')" :class="current_btn == 'btn1' ? 'active_btn' : ''" class="new_contct_sect">
            <div class="txt_new_contct">Subscribed</div>
            </div>

              <!-- allcontact -->
              <div @click="setCurrentBtn('btn2')" :class="current_btn == 'btn2' ? 'active_btn' : ''" class="new_contct_sect">
                <div class="txt_new_contct">New</div>
            </div>
                        <!--  -->
              <div class="new_contct_sect">
                  <div class="txt_new_contct">+9 More...</div>
              </div>
              <!--  -->
              <div class="new_contct_sect">
                  <div class="txt_new_ctrl">Ctrl O</div>
              </div>
          </div>
          <!-- section two -->
          <div class="section_two">
              <button class="cutmiz_tble">
              <svg width="1em" height="1em" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon--container_WX8MsF4aQZ5i3RN1  svg-md undefined m-r-5"><path opacity="0.01" fill="#fff" fill-opacity="0.2" d="M0 0h14v14H0z"></path><path stroke="#333" stroke-linecap="round" stroke-linejoin="round" d="M2 7.5v6M2 .5v3"></path><circle cx="2" cy="5.5" r="1.5" stroke="#333" stroke-linecap="round" stroke-linejoin="round"></circle><path d="M7 11.5v2M7 .5v7" stroke="#333" stroke-linecap="round" stroke-linejoin="round"></path><circle cx="7" cy="9.5" r="1.5" stroke="#333" stroke-linecap="round" stroke-linejoin="round"></circle><path stroke="#333" stroke-linecap="round" stroke-linejoin="round" d="M12 7.5v6M12 .5v3"></path><circle cx="12" cy="5.5" r="1.5" stroke="#333" stroke-linecap="round" stroke-linejoin="round"></circle></svg>
              Customize table
          </button>
          <!-- <div class="imprt_btns_div">
              <button class="imprt_btn">
                  <svg width="1em" height="1em" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg" class="m-r-5"><path opacity="0.01" fill="#fff" fill-opacity="0.01" d="M0 0h14v14H0z"></path><path d="M7 .5a6.5 6.5 0 1 0 0 13 6.5 6.5 0 0 0 0-13Z" stroke="#384551" stroke-linecap="round" stroke-linejoin="round"></path><path d="M4.4 7 7 9.6 9.6 7M7 4.4v5.2" stroke="#384551" stroke-linecap="round" stroke-linejoin="round"></path></svg>
                  Import Contacts
              </button>
              <select name="View Import History" id="">
                  <option value=""></option>
              </select>
          </div>
          <div class="add_cntct_btn_div">
              <button class="add_cntct_btn">
                  <svg width="1em" height="1em" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg"><path opacity="0.01" fill="#fff" fill-opacity="0.01" d="M0 0h14v14H0z"></path><path d="M3.285 7h7.429M7 3.286v7.428" stroke="#fff" stroke-linecap="round"></path><rect x="0.5" y="0.5" width="13" height="13" rx="6.5" stroke="#fff" stroke-linecap="round" stroke-linejoin="round"></rect></svg>
                  Add Contact
              </button>
          </div> -->
          </div>
      </div>
        </div>
     
      <!-- 4bar -->

      <div class="forth_bar">
          <div class="forth_sect_one">
              <div class="tabl_btn_div">
                  <button class="tabl_btn">
                      <svg width="1em" height="1em" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon--container_WX8MsF4aQZ5i3RN1   vt__item-icon_MOzQfW1J23ifi3kW"><path fill-rule="evenodd" clip-rule="evenodd" d="M1.5 0A1.5 1.5 0 0 0 0 1.5v11A1.5 1.5 0 0 0 1.5 14h11a1.5 1.5 0 0 0 1.5-1.5v-11A1.5 1.5 0 0 0 12.5 0h-11ZM1 1.5a.5.5 0 0 1 .5-.5h2v2.5H1v-2Zm0 3v8a.5.5 0 0 0 .5.5h2V4.5H1ZM4.5 13h8a.5.5 0 0 0 .5-.5v-8H4.5V13ZM13 3.5v-2a.5.5 0 0 0-.5-.5h-8v2.5H13Z" fill="#000"></path></svg>
                      Table
                      <select name="" id=""></select>
                  </button>
              </div>
              <div>
                  <svg width="1em" height="1em" viewBox="0 0 15 14" fill="none" xmlns="http://www.w3.org/2000/svg" class="svg-md icon-style_myh0__iGZZd8UNMi"><path opacity="0.01" fill="#fff" fill-opacity="0.01" d="M1 0h14v14H1z"></path><path d="M7.95 1h6.503M7.95 5h6.503M7.95 9h6.503M7.95 13h6.503" stroke="#384551" stroke-linecap="round"></path><path d="M1.484 3.188 3.67 1 5.86 3.188M5.859 10.813 3.67 13l-2.187-2.188M3.671 12.989V1" stroke="#384551" stroke-linecap="round" stroke-linejoin="round"></path></svg>
              </div>

              <div class="tabl_btn_div">
                  <button class="tabl_btn2">
                      <svg width="1em" height="1em" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon--container_WX8MsF4aQZ5i3RN1  svg-md "><path d="M.5 10.25 7 13.5l6.5-3.25M.5 7 7 10.25 13.5 7M7 .5.5 3.75 7 7l6.5-3.25L7 .5Z" stroke="#384551" stroke-linecap="round" stroke-linejoin="round"></path></svg>
                      Bulk actions
                  </button>
              </div>

              <div class="tabl_btn_div">
                  <button class="tabl_btn2">
                      <svg width="1em" height="1em" viewBox="0 0 14 15" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon--container_WX8MsF4aQZ5i3RN1  svg-md "><path opacity="0.01" fill="#fff" fill-opacity="0.01" d="M0 .5h14v14H0z"></path><path stroke="#384551" stroke-linecap="round" d="M.5 3.5h13M2.5 7.5h9M5.5 11.5h3"></path></svg>
                      1 filter applied
                  </button>
              </div>
          </div>
      </div>
      <!--  -->
      <div class="table-responsive3">
          <table class="table3  table-hover table-bordered table-responsive">
<thead>
  <tr>
    <th class="tble_name_sect3" scope="col"> <input class="inptchck_main" type="checkbox"> Name <select name="" id="table_slct3"></select></th>
    <th class="tble_txt3" scope="col">Emails <select name="" id="table_slct3"></select></th>
    <th class="tble_name_sect3" scope="col">Phone <select name="" id="table_slct3"></select></th>
    <th class="tble_txt3" scope="col">Plan <select name="" id="table_slct3"></select></th>
    <th class="tble_txt3" scope="col">Date <select name="" id="table_slct3"></select></th>
  </tr>
</thead>
<tbody>
  <tr v-for="(item, index) in filteredData" :key="index" @click="showDetails(item)">
  <th class="name_sect2" scope="row">
    <input class="inptchck_user" type="checkbox">
    <img class="tble_img" :src="item.image || '/dashboard/prof_pic_dashbrd.png'" alt="">
    <p class="text-primary">{{ item.name }}</p>
  </th>
  <td class="tble_txt2">{{ item.email }}</td>
  <td class="tble_txt2">{{ item.phone }}</td>
  <td class="tble_txt2">{{ item.plans[0].name }}</td>
  <td class="tble_txt2">{{ formatDateTime(item.date_joined) }}</td>
</tr>


</tbody>

</table>
<div class="custom-pagination">
      <button class="pagination-button" @click="goToFirstPage" :disabled="currentPage === 1">First</button>
      <button class="pagination-button" @click="setPage(currentPage - 1)" :disabled="currentPage === 1">&laquo; Previous</button>
      <button v-for="page in calculatedPages" :key="page" @click="setPage(page)" :class="{ active: currentPage === page }" class="pagination-button">{{ page }}</button>
      <button class="pagination-button" @click="setPage(currentPage + 1)" :disabled="currentPage === totalPages">Next &raquo;</button>
      <button class="pagination-button" @click="goToLastPage" :disabled="currentPage === totalPages">Last</button>
    </div>
</div>
     
      <b-sidebar v-model="sidebarVisible"   id="sidebar-1" right shadow>
   <div class="px-3 py-2"  v-if="selectedItem">
    <div class="profl_sect">
      <img class="modal_img" :src="selectedItem.image || '/dashboard/prof_pic_dashbrd.png'" alt="">
        <h2 style="font-weight: 800px; font-size: 18px; color: black;">{{selectedItem.name}}<br>
            <h6>{{selectedItem.email}}</h6> 
        </h2>
        <div class="dtl_btn_top">
            <button class="tabl_btn"><svg class="svg-md mg-r-5 custom-button-svg" width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M14 0H0v14h14V0z" fill="#fff" fill-opacity=".01"></path><path d="M7.696 6.304l2.803-2.803M6.567 10.5H3.5V7.433M7.433 3.5H10.5v3.067M10.5 3.5l-7 7" stroke="#333" stroke-linecap="round" stroke-linejoin="round"></path><rect x=".5" y=".5" width="13" height="13" rx="2" stroke="#333" stroke-linecap="round" stroke-linejoin="round"></rect></svg>
                See all Details</button>
        </div>
        <div class="dtl_btn_top2">
                <button class="tabl_btn"><svg class=" custom-button-svg" width="8" height="14" viewBox="0 0 8 14" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path fill-opacity=".01" fill="#FFF" fill-rule="nonzero" opacity=".01" d="M-3 0h14v14H-3z"></path><path d="M7.5.5L1 7l6.5 6.5" opacity=".6" stroke="#000" stroke-linecap="round" stroke-linejoin="round"></path></g></svg></button> 
                <button class="tabl_btn"><svg class=" custom-button-svg" width="8" height="14" viewBox="0 0 8 14" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path fill-opacity=".01" fill="#FFF" fill-rule="nonzero" opacity=".01" d="M11 0H-3v14h14z"></path><path d="M.5.5L7 7 .5 13.5" opacity=".6" stroke="#000" stroke-linecap="round" stroke-linejoin="round"></path></g></svg></button>
            </div>
    </div>
    <div class="btn_div">
        <div class="top_btns">   
            <div class="popup_btns_div">
                <button class="tabl_btn"><svg class="svg-md valign-middle mg-r-5 custom-button-svg" width="18" height="18" viewBox="0 0 18 18" xmlns="http://www.w3.org/2000/svg"><g stroke="#000" fill="none" fill-rule="evenodd"><path d="M10.921.52H4.113c-.94 0-1.702.761-1.702 1.701v13.616c0 .94.762 1.702 1.702 1.702h10.212c.94 0 1.702-.762 1.702-1.702V5.625L10.921.52z"></path><path d="M10.921.52v4.105a1 1 0 0 0 1 1h4.106"></path><path d="M12.623 9.88H5.815M12.623 13.284H5.815M7.517 6.476H5.815" stroke-linecap="round" stroke-linejoin="round"></path></g></svg>
                <div>Note</div>
            </button>
            </div>     
           
        </div>
    <button class="tabl_btn"><svg class="svg-md valign-middle mg-r-5 custom-button-svg" width="18" height="18" viewBox="0 0 18 18" xmlns="http://www.w3.org/2000/svg"><g stroke="#000" fill="none" fill-rule="evenodd"><path d="M10.703 1.75H4.141c-.906 0-1.641.705-1.641 1.575v12.6c0 .87.735 1.575 1.64 1.575h9.844c.906 0 1.641-.705 1.641-1.575V3.75a2 2 0 0 0-2-2h-2.922z"></path><g stroke-linecap="round"><path d="M5.716.525v2.154M12.826.525v2.154M9.271.525v2.154"></path></g><path d="M5.563 10.48l2.456 2.398c.083.08.215.08.298 0L13 8.306" stroke-linecap="round"></path></g></svg>
    <div>Task</div>
    </button>
    <button class="tabl_btn"><svg class="svg-md valign-middle mg-r-5 custom-button-svg" width="18" height="18" viewBox="0 0 18 18" xmlns="http://www.w3.org/2000/svg"><g transform="translate(1)" stroke="#000" fill="none" fill-rule="evenodd" stroke-linecap="round" stroke-linejoin="round"><rect y="1.778" width="16" height="15.8" rx="2"></rect><path d="M11.556.5v3M4.444.5v3M0 8.111h16"></path></g></svg>
    <div>Meeting</div>
    </button>
    <button class="tabl_btn"><svg width="20" height="20" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg" class="svg-md valign-middle mg-r-5"><path fill-rule="evenodd" clip-rule="evenodd" d="M10.7.7A.7.7 0 0 0 10 0H.7a.7.7 0 0 0-.7.7v18.6a.7.7 0 0 0 .7.7h18.6a.7.7 0 0 0 .7-.7V6.9a.7.7 0 0 0-.7-.7h-8.6V.7zM4 12.4a.92.92 0 0 0-.92.92v5.28H1.4V1.4h7.9v17.2H7.54v-5.28a.92.92 0 0 0-.92-.92H4zm13.36 2.9a.7.7 0 0 0-.7-.7h-4a.7.7 0 1 0 0 1.4h4a.7.7 0 0 0 .7-.7zm0-4a.7.7 0 0 0-.7-.7h-4a.7.7 0 1 0 0 1.4h4a.7.7 0 0 0 .7-.7zm-9.3-2.19a.7.7 0 0 0-.7-.7h-4a.7.7 0 1 0 0 1.4h4a.7.7 0 0 0 .7-.7zm0-3.98a.7.7 0 0 0-.7-.7h-4a.7.7 0 0 0 0 1.4h4a.7.7 0 0 0 .7-.7zM4.48 13.8h1.66v4.8H4.48v-4.8zm6.22-6.2h7.9v11h-7.9v-11z"></path></svg>
    <div>Add account</div>
    </button>
    <button class="tabl_btn"><svg class="svg-md" width="4" height="14" viewBox="0 0 4 14" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path fill-opacity=".01" fill="#FFF" opacity=".01" d="M-5 0H9v14H-5z"></path><g transform="translate(.833 .583)" fill="#000"><circle cx="1.3" cy="1.3" r="1.3"></circle><circle cx="1.3" cy="6.5" r="1.3"></circle><circle cx="1.3" cy="11.7" r="1.3"></circle></g></g></svg></button>
    </div>
    <hr>
    <br>
    <div class="txt_lyf_cycle">
        <h3 class="overview_txt">Plan Details</h3>
        <button class="tabl_btn"><svg class="svg-md custom-button-svg" width="18" height="18" viewBox="0 0 18 18" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path fill-opacity=".01" fill="#FFF" opacity=".01" d="M0 0h18v18H0z"></path><g stroke="#000" stroke-linecap="round" stroke-linejoin="round"><path d="M14.718 11.318c-.21.477-.11 1.034.255 1.407l.047.046a1.545 1.545 0 1 1-2.187 2.187l-.047-.047a1.275 1.275 0 0 0-1.406-.255c-.467.2-.77.659-.773 1.167v.132a1.545 1.545 0 0 1-3.09 0v-.07a1.275 1.275 0 0 0-.835-1.167 1.275 1.275 0 0 0-1.407.255l-.046.047a1.545 1.545 0 1 1-2.187-2.187l.047-.047c.364-.372.465-.93.255-1.406-.2-.467-.659-.77-1.167-.773h-.132a1.545 1.545 0 1 1 0-3.09h.07a1.275 1.275 0 0 0 1.167-.835c.21-.477.11-1.034-.255-1.407L2.98 5.23a1.545 1.545 0 1 1 2.187-2.187l.047.047c.372.364.93.465 1.406.255h.062c.467-.2.77-.659.773-1.167v-.132a1.545 1.545 0 1 1 3.09 0v.07c.002.508.306.967.773 1.167.477.21 1.034.11 1.407-.255l.046-.047a1.545 1.545 0 1 1 2.187 2.187l-.047.047c-.364.372-.465.93-.255 1.406v.062c.2.467.659.77 1.167.773h.132a1.545 1.545 0 0 1 0 3.09h-.07a1.275 1.275 0 0 0-1.167.773z"></path><circle cx="9" cy="9" r="2"></circle></g></g></svg>
        <div>Customize Plan</div>
        </button>
    </div>
    <br>
  <div class="table-responsive_plan">
    <table class="table">
      <thead>
        <tr>
          <th class="text-info">Plan</th>
          <th class="text-info">Price</th>
          <th class="text-info">Exp-Date</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(plan, index) in planHistory" :key="index">
      <td class="text-info">{{ plan.plan_details.plan }}</td>
      <td class="text-info">{{ plan.plan_details.amount }}</td>
      <td class="text-info">{{ formatDateTime(plan.plan_details.created_on) }}</td>
    </tr>
</tbody>

</table >
  </div > 
    <hr >
    <div>
        <div class="txt_main_one">
            <h5>Lead History (Download)</h5>
        </div>
        <div class="table-responsive2">
    <table class="table2 table-hover table-bordered table-responsive">
      <thead>
        <tr>
          <th class="tble_name_sect2" scope="col">Name</th>
          <th class="tble_txt3" scope="col">Location</th>
          <th class="tble_name_sect2" scope="col">Radius</th>
          <th class="tble_txt3" scope="col">Estimation</th>
          <th class="tble_txt3" scope="col">Leads</th>
          <th class="tble_txt3" scope="col">Is Stopped</th>
          <th class="tble_txt3_dt" scope="col">Date & Time</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(downloadLead, index) in userSpecificData.download_leads" :key="index">
          <th class="name_sect" scope="row">
            <p class="text-primary">{{ downloadLead.business }}</p>
          </th>
          <td class="tble_txt2">{{ parseData(downloadLead.data).location || 'N/A' }}</td>
          <td class="tble_txt2">{{ (parseData(downloadLead.data).radius / 1000) || 'N/A' }} Km</td>
          <td class="tble_txt2">{{ parseData(downloadLead.data).estimate || 'N/A' }}</td>
          <td class="tble_txt2">{{ downloadLead.leads !== undefined ? downloadLead.leads : 'N/A' }}</td>
          <td class="tble_txt2">
          <button v-if="parseData(downloadLead.data).is_stop === 1" type="button" class="btn_won">Yes</button>
          <span v-else>---</span>
          </td>
          <td class="tble_txt2">{{ formatDateTime(downloadLead.created_on) || 'N/A' }}</td>
        </tr>
   </tbody>
    </table>
  </div>
    </div>
    <div>
        <div class="txt_main_one">
            <h5>Lead History (Tap)</h5>
        </div>
        <div class="table-responsive2">
    <table class="table2 table-hover table-bordered table-responsive">
      <thead>
        <tr>
          <th class="tble_name_sect2" scope="col">Name</th>
          <th class="tble_txt3" scope="col">Location</th>
          <th class="tble_name_sect2" scope="col">Radius</th>
          <th class="tble_txt3" scope="col">Estimation</th>
          <th class="tble_txt3" scope="col">Leads</th>
          <th class="tble_txt3" scope="col">Is Stopped</th>
          <th class="tble_txt3_dt" scope="col">Date & Time</th>
        </tr>
      </thead>
      <tbody>
        <tr v-if="userSpecificData">
  <th class="name_sect" scope="row">
    <!-- <p class="text-primary">{{ userSpecificData.user.name }}</p> -->
  </th>
</tr>
<tr v-for="(lead, index) in userSpecificData.lead_history" :key="index">
  <th class="name_sect" scope="row">
    <p class="text-primary">{{ lead.business }}</p>
  </th>
  <td class="tble_txt2">{{ lead.location || '---' }}</td>
  <td class="tble_txt2">{{ (lead.radius / 1000) || '---' }} Km</td>
  <td class="tble_txt2">{{ lead.estimate || '---' }}</td>
  <td class="tble_txt2">{{ lead.results !== undefined ? lead.results   : 'N/A' }}</td>
  <td class="tble_txt2">
  <button v-if="lead.is_stop" type="button" class="btn_won">Yes</button>
  <span v-else>---</span>
  </td>
  <td class="tble_txt2">{{ formatDateTime(lead.created_on) || '---' }}</td>
</tr>

</tbody>
</table>
</div>

<!--  -->
    </div>
    <hr>
    <!-- <div class="more_dtls_div">
        <div>
        <h5>Location</h5>
        <h6 class="text-info">Toronto, Ontario, Canada</h6>
        </div>
        <div>
            <h5>Accounts</h5>
        <h6 class="text-info">Acme Inc (sample)</h6>
        </div>
        <div>
            <h5>Emails</h5>
        <h6 class="text-dark">lauranordasample@gmail.com</h6>
        </div>

        <div>
        <h5>Mobile</h5>
        <h6 class="text-dark">19266343001</h6>
        </div>
        <div>
            <h5>Sales owner</h5>
        <h6 class="text-dark">ajais vraj</h6>
        </div>
        <div>
            <h5>Created at</h5>
        <h6 class="text-dark">a month ago</h6>
        </div>
    </div>
    Show all <select name="" id=""></select>
    <hr> -->
    <!-- <div class="text_area"> 
        <input class="inpt_area" type="text" placeholder="Add a note...">
        <hr>
        <p class="inpt_text">Laura wants to buy one more license and will decide by the end of the month.</p>
        <br>
        <p class="inpt_text">ajais vraj . 13 days ago</p>
    </div> -->
    <!--  -->
    <div class="bottom_icons">
        <div class="icon_cover">
            <svg viewBox="0 0 14 14" xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" class="icon--container_WX8MsF4aQZ5i3RN1  card-icon_d2zbHgAjG6G91rwP "><g fill="none" fill-rule="evenodd"><path fill-opacity="0.2" fill="#FFF" opacity="0.01" d="M0 0h14v14H0z"></path><g stroke="#eb8344"><path d="m8.717 2.398 4.255 7.347a2 2 0 0 1-1.73 3.002h-8.51A2 2 0 0 1 1 9.745l4.255-7.347a2 2 0 0 1 3.461 0ZM7 9.603v1.121M7 3.615v4.807"></path></g></g></svg>
        </div>
        <div>Couldn’t load this card. Try refreshing the page.</div>
    </div>
    <!--  -->
    <div class="bottom_icons2">
        <div class="icon_cover2">
            <svg width="1em" height="1em" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg" class="icon--container_WX8MsF4aQZ5i3RN1  card-icon_d2zbHgAjG6G91rwP "><path opacity="0.01" fill="#fff" fill-opacity="0.2" d="M1 1h20v20H1z"></path><path opacity="0.01" fill="#A9A9EB" d="M1 1h20v20H1z"></path><rect x="1.313" y="3.465" width="19.375" height="17.222" rx="2" fill="#fff" stroke="#6E49B8" stroke-linecap="round" stroke-linejoin="round"></rect><path d="M1.313 5.465a2 2 0 0 1 2-2h15.374a2 2 0 0 1 2 2v2.844H1.313V5.465Z" fill="#B4A3D6" stroke="#6E49B8" stroke-linecap="round" stroke-linejoin="round"></path><path d="M15.306 1.313v4.305M6.694 1.313v4.305" stroke="#6E49B8" stroke-linecap="round" stroke-linejoin="round"></path></svg>        </div>
        <div>No upcoming meetings with {{selectedItem.name}} <br>
            <b class="text-info">Add meeting</b>
        </div>
    </div>
    <!--  -->
    <div class="bottom_icons2">
        <div class="icon_cover">
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 22 15" fill="none" class="icon--container_WX8MsF4aQZ5i3RN1  card-icon_d2zbHgAjG6G91rwP "><path fill-rule="evenodd" clip-rule="evenodd" d="M1.313 2.75a2 2 0 0 1 2-2h15.374a2 2 0 0 1 2 2v8.799a2 2 0 0 1-2 2H3.313a2 2 0 0 1-2-2V2.75Z" fill="#FDDBB5" stroke="#E86F25" stroke-linecap="round" stroke-linejoin="round"></path><path fill-rule="evenodd" clip-rule="evenodd" d="M1.313 2.54a.9.9 0 0 1 1.478-.69L11 8.749l8.209-6.897a.9.9 0 0 1 1.479.689v8.867a2 2 0 0 1-2 2H3.313a2 2 0 0 1-2-2V2.54Z" fill="#fff" stroke="#E86F25" stroke-linecap="round" stroke-linejoin="round"></path></svg>        </div>
        <b class="text-dark">{{selectedItem.name}} sent an email
            <p>5 Days ago</p>
        </b>
    </div>
    <!--  -->
    <div class="bottom_icons2">
        <div class="icon_cover3">
            <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 21 21" fill="none" class="icon--container_WX8MsF4aQZ5i3RN1  card-icon_d2zbHgAjG6G91rwP "><circle cx="10.236" cy="10.764" r="9.236" fill="#fff" stroke="#2895A4" stroke-linecap="round" stroke-linejoin="round"></circle><circle cx="10.236" cy="10.764" fill="#ABECF5" stroke="#2895A4" stroke-linecap="round" stroke-linejoin="round" r="5.278"></circle><circle cx="10.236" cy="10.764" fill="#fff" r="1.319"></circle><path d="M10.236 10.764 18.1 2.9M18.1 1v1.9H20" stroke="#2895A4" stroke-linecap="round" stroke-linejoin="round"></path></svg>        </div>
        <p class="text-dark">{{selectedItem.name}} is not part of any sales sequence.</p>
    </div>
   </div>
</b-sidebar>
      </div>
    </div>
</template>

<script>
import axios from 'axios';
export default {
data() {
  return {
    current_btn: 'btn0',
    currentPage: 1,
    itemsperPage: 20,
    displayedItems: [],
    sidebarVisible: false,
    selectedItem: null,
    TableData: [],
    selectedUserId: null,
    userSpecificData: {},
    parsedDownloadLeadsData: null,
    planNames: [],
    totalPages:418,
    allData: [],
    planHistory: [],
    searchQuery: '',
    filteredData: [],
    searchResults: [],
    showSearchResults: false,
    pageNumber: 1,
  };
},

computed: {
  planName() {
    if (this.allData.length > 0 && this.allData[0].plans.length > 0) {
      return this.allData[0].plans[0].name;
    }
    return 'N/A';
  },
  planAmount() {
    if (this.allData.length > 0 && this.allData[0].plans.length > 0) {
      return this.allData[0].plans[0].amount;
    }
    return 'N/A';
  },
  planCreatedDate() {
    if (this.allData.length > 0 && this.allData[0].plans.length > 0) {
      return this.allData[0].plans[0].date;
    }
    return 'N/A';
  },
  calculatedPages() {
  const maxButtons = 7;
  const totalPages = this.totalPages;

  let start = Math.max(1, this.currentPage - Math.floor(maxButtons / 2));
  let end = Math.min(start + maxButtons - 1, totalPages);

  if (end - start < maxButtons - 1) {
    start = Math.max(1, start - (maxButtons - 1 - (end - start)));
  }

  return Array.from({ length: end - start + 1 }, (_, index) => start + index);
},



totalNumberOfPages() {
    return Math.ceil(this.totalResultsCount / this.itemsPerPage);
  },
},

methods: {
  async fetchDataFromApi(pageNumber) {
  try {
    const url = `https://api.leadfinder.live/users/users/?page=${pageNumber}${this.searchQuery ? `&search=${this.searchQuery}` : ''}`;
    const response = await axios.get(url);
    const responseData = response.data.results;
    this.allData = responseData;
    this.filteredData = responseData;
    this.itemsperPage = responseData.length; 
    this.totalResultsCount = response.data.count;
  } catch (error) {
    console.error('Error fetching data:', error);
  }
},


async performSearch() {
  try {
    const url = `https://api.leadfinder.live/users/users/?page=${this.pageNumber}&search=${this.searchQuery}`;
    const response = await axios.get(url);
    const responseData = response.data.results;
    this.filteredData = responseData;
    this.totalResultsCount = response.data.count;
    this.totalPages = Math.ceil(this.totalResultsCount / this.itemsperPage);
    console.log('Filtered Data:', this.filteredData);
  } catch (error) {
    console.error('Error fetching data:', error);
  }
},


  async search() {
  try {
    const query = this.searchQuery.trim().toLowerCase();
    if (query === '') {
      this.filteredData = this.allData;
    } else {
      const allData = await this.fetchAndFilterData(query);
      this.filteredData = allData;
      this.totalResultsCount = allData.length;
    }
    this.currentPage = 1;
    this.totalPages = Math.ceil(this.totalResultsCount / this.itemsperPage);
  } catch (error) {
    console.error('Error searching:', error);
  }
},



async fetchUserSpecificData() {
try {
if (this.selectedUserId) {
  const url = `https://api.leadfinder.live/employee/user_info/${this.selectedUserId}/`;
  const response = await axios.get(url);
  this.userSpecificData = response.data;
  this.planHistory = response.data.plan_history;

  if (this.userSpecificData.download_leads && this.userSpecificData.download_leads.length > 0) {
    const downloadLeadData = this.userSpecificData.download_leads[0].result_table;
    this.parsedDownloadLeadsData = this.parseResultTable(downloadLeadData);
    console.log('downloadLead:', this.userSpecificData.download_leads[0]);
  }
  if (this.userSpecificData.lead_history) {
    this.parseLeadHistoryData(this.userSpecificData.lead_history);
  }
}
} catch (error) {
console.error('Error fetching user-specific data:', error);
}
},

async parseResultTable(resultTableHTML) {
  const parser = new DOMParser();
  const doc = parser.parseFromString(resultTableHTML, 'text/html');
  const tableRows = doc.querySelectorAll('tbody tr');
  const parsedData = [];

  tableRows.forEach((row) => {
    const columns = row.querySelectorAll('td');
    const rowDataEntry = {
      No: columns[0].textContent,
      Name: columns[1].textContent,
      Phone: columns[2].textContent,
      Email: columns[3].textContent,
      Rating: columns[4].textContent,
      Website: columns[5].textContent,
      Address: columns[6].textContent,
      ZipCode: columns[7].textContent,
    };
    parsedData.push(rowDataEntry);
  });

  return parsedData;
},


async parseDownloadLeadsData() {
  if (this.userSpecificData.download_leads && this.userSpecificData.download_leads.length > 0) {
    const rawData = this.userSpecificData.download_leads[0].data;
    try {
      this.parsedDownloadLeadsData = JSON.parse(rawData);
      if (Array.isArray(this.parsedDownloadLeadsData)) {
        const firstItem = this.parsedDownloadLeadsData[0];
        this.TableData = [firstItem];
      }
    } catch (error) {
      console.error('Error parsing download leads data:', error);
      this.parsedDownloadLeadsData = null;
    }
  }
},


parseData(data) {
  if (typeof data === 'string') {
    try {
      const parsedData = JSON.parse(data);
      if (Array.isArray(parsedData) && parsedData.length > 0) {
        return parsedData[0];
      }
    } catch (error) {
      console.error('Error parsing data:', error);
    }
  }
  return {};
},


formatDateTime(dateTime) {
  if (!dateTime) return '---'; 

  const date = new Date(dateTime);
  const year = date.getFullYear();
  const month = (date.getMonth() + 1).toString().padStart(2, '0'); 
  const day = date.getDate().toString().padStart(2, '0');
  const hours = date.getHours();
  const minutes = date.getMinutes();
  const ampm = hours >= 12 ? 'PM' : 'AM';
  const formattedHours = hours % 12 || 12; 
  const formattedMinutes = minutes < 10 ? `0${minutes}` : minutes;
  const formattedDateTime = `${year}-${month}-${day} ${formattedHours}:${formattedMinutes} ${ampm}`;
  return formattedDateTime;
},


parseLeadHistoryData(leadHistory) {
},


toggleSidebar() {
  this.$refs.mySidebar.toggle();
},


setCurrentBtn(btn) {
  this.current_btn = btn;
},


onPageChange(newPage) {
  if (newPage >= 1 && newPage <= this.totalPages) {
    this.currentPage = newPage;
    this.fetchDataFromApi(newPage);
  }
},


showDetails(item) {
  this.selectedItem = item;
  this.sidebarVisible = true;
  this.selectedUserId = item.id;
  this.$nextTick(async () => {
    await this.fetchUserSpecificData();
  });
},

setPage(page) {
if (page >= 1 && page <= this.totalPages) {
  if (page === this.totalPages) {
    this.currentPage = this.totalPages;
  } else {
    this.currentPage = page;
    this.fetchDataFromApi(page); 
  }
}
},
goToLastPage() {
    this.currentPage = this.totalPages;
    this.fetchDataFromApi(this.currentPage);
  },
  goToFirstPage() {
    this.currentPage = 1;
    this.fetchDataFromApi(this.currentPage);
  },
},

created() {
  this.fetchDataFromApi(this.currentPage);
  this.fetchPlanHistoryData
  // this.search();
},

watch: {
  sidebarVisible(newVal) {
    if (newVal) {
      // this.fetchUserSpecificData();
      if (this.userSpecificData && this.userSpecificData.download_leads) {
        this.parseDownloadLeadsData();
      }
    }
  },
  searchQuery(newValue) {
    if (!newValue) {
      this.filteredData = this.allData; 
      this.currentPage = 1; 
    } else {
      this.performSearch(); 
    }
  },
  
  
},
};    
</script>



<style>
@import './style/usersstyle.css';
</style>

