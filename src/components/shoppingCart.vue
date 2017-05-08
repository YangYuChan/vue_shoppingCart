<template>
	<div id="shopping-cart">
		 <svg style="position: absolute; width: 0; height: 0; overflow: hidden;" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
      <defs>
        <symbol id="icon-add" viewBox="0 0 32 32">
          <title>add2</title>
          <path class="path1" d="M15 17h-13.664c-0.554 0-1.002-0.446-1.002-1 0-0.552 0.452-1 1.002-1h13.664v-13.664c0-0.554 0.446-1.002 1-1.002 0.552 0 1 0.452 1 1.002v13.664h13.664c0.554 0 1.002 0.446 1.002 1 0 0.552-0.452 1-1.002 1h-13.664v13.664c0 0.554-0.446 1.002-1 1.002-0.552 0-1-0.452-1-1.002v-13.664z"></path>
        </symbol>
        <symbol id="icon-ok" viewBox="0 0 39 32">
          <title>ok</title>
          <path class="path1" d="M14.084 20.656l-7.845-9.282c-1.288-1.482-3.534-1.639-5.016-0.351s-1.639 3.534-0.351 5.016l10.697 12.306c1.451 1.669 4.057 1.623 5.448-0.096l18.168-22.456c1.235-1.527 0.999-3.765-0.528-5.001s-3.765-0.999-5.001 0.528l-15.573 19.337z"></path>
        </symbol>
        <symbol id="icon-edit" viewBox="0 0 32 32">
          <title>edit</title>
          <path class="path1" d="M25.599 11.292l-4.892-4.892 3.825-3.825 4.892 4.892-3.825 3.825zM4.732 23.308l3.959 3.959-5.939 1.98 1.98-5.939zM10.666 26.225l-4.892-4.892 13.425-13.425 4.892 4.892-13.425 13.425zM31.687 6.713l-6.4-6.4c-0.417-0.417-1.091-0.417-1.508 0l-20.267 20.267c-0.114 0.115-0.191 0.25-0.242 0.393-0.003 0.009-0.012 0.015-0.015 0.025l-3.2 9.6c-0.128 0.383-0.029 0.806 0.257 1.091 0.203 0.204 0.476 0.313 0.754 0.313 0.112 0 0.227-0.017 0.337-0.054l9.6-3.2c0.011-0.003 0.017-0.013 0.027-0.016 0.142-0.052 0.276-0.128 0.39-0.242l20.267-20.267c0.417-0.416 0.417-1.091 0-1.508v0z"></path>
        </symbol>
        <symbol id="icon-del" viewBox="0 0 26 32">
          <title>delete</title>
          <path class="path1" d="M17.723 28c0.543 0 0.984-0.448 0.984-1v-12c0-0.552-0.441-1-0.984-1s-0.985 0.448-0.985 1v12c0 0.552 0.441 1 0.985 1v0zM7.877 28c0.543 0 0.984-0.448 0.984-1v-12c0-0.552-0.441-1-0.984-1s-0.985 0.448-0.985 1v12c0 0.552 0.441 1 0.985 1v0zM12.8 28c0.543 0 0.985-0.448 0.985-1v-12c0-0.552-0.441-1-0.985-1s-0.984 0.448-0.984 1v12c0 0.552 0.441 1 0.984 1v0zM23.631 4h-5.908v-2c0-1.104-0.882-2-1.969-2h-5.908c-1.087 0-1.969 0.896-1.969 2v2h-5.908c-1.087 0-1.969 0.896-1.969 2v2c0 1.104 0.882 2 1.969 2v18c0 2.208 1.765 4 3.939 4h13.784c2.174 0 3.938-1.792 3.938-4v-18c1.087 0 1.969-0.896 1.969-2v-2c0-1.104-0.882-2-1.969-2v0zM9.846 3c0-0.552 0.441-1 0.984-1h3.938c0.544 0 0.985 0.448 0.985 1v1h-5.908v-1zM21.662 28c0 1.104-0.882 2-1.969 2h-13.784c-1.087 0-1.97-0.896-1.97-2v-18h17.723v18zM22.646 8h-19.692c-0.543 0-0.985-0.448-0.985-1s0.441-1 0.985-1h19.692c0.543 0 0.984 0.448 0.984 1s-0.441 1-0.984 1v0z"></path>
        </symbol>
        <symbol id="icon-clock" viewBox="0 0 32 32">
          <title>clock</title>
          <path class="path1" d="M29.333 16c0-7.364-5.97-13.333-13.333-13.333s-13.333 5.97-13.333 13.333c0 7.364 5.97 13.333 13.333 13.333s13.333-5.97 13.333-13.333v0 0 0 0 0 0zM0 16c0-8.837 7.163-16 16-16s16 7.163 16 16c0 8.837-7.163 16-16 16s-16-7.163-16-16zM14.667 14.667v1.333h2.667v-10.667h-2.667v9.333zM24 18.667h1.333v-2.667h-10.667v2.667h9.333z"></path>
        </symbol>
      </defs>
    </svg>
		<div class="container">
      <div class="cart">
        <div class="checkout-title">
          <span>购物车</span>
        </div>
        <!-- table -->
        <div class="item-list-wrap">
          <div class="cart-item">
            <div class="cart-item-head">
              <ul>
                <li>商品信息</li>
                <li>商品金额</li>
                <li>商品数量</li>
                <li>总金额</li>
                <li>编辑</li>
              </ul>
            </div>
            <ul class="cart-item-list">
              <li v-for="(item,index) in productList">
                <div class="cart-tab-1">
                  <div class="cart-item-check">
                    <a href="javascript:;" class="item-check-btn" v-bind:class="{'check':item.checked}" @click="selectedProduct(item)">
                      <svg class="icon icon-ok"><use xlink:href="#icon-ok"></use></svg>
                    </a>
                  </div>
                  <div class="cart-item-pic">
                    <img v-bind:src="item.productImage">
                  </div>
                  <div class="cart-item-title">
                    <div class="item-name">{{index+". "+item.productName}}</div>
                  </div>
                  <div class="item-include">
                    <dl>
                      <dt>赠送:</dt>
                      <dd v-for="part in item.parts">
                        <div class="partContent">
                          <div class="left">
                            <img v-bind:src="part.imgSrc" style="width: 50px;"/>
                          </div>
                          <div class="right">
                            <span>{{part.partsName}}</span>
                          </div>
                        </div>
                      </dd>
                    </dl>
                  </div>
                </div>
                <div class="cart-tab-2">
                  <div class="item-price">{{item.productPrice | formatMoney('') }}</div>
                </div>
                <div class="cart-tab-3">
                  <div class="item-quantity">
                    <div class="select-self select-self-open">
                      <div class="quantity">
                        <a href="javascript:;" v-on:click="changeQuantity(item,-1)">-</a>
                        <input type="text" value="0" v-model="item.productQuantity">
                        <a href="javascript:;" @click="changeQuantity(item,1)">+</a>
                      </div>
                    </div>
                    <div class="item-stock">有货</div>
                  </div>
                </div>
                <div class="cart-tab-4">
                  <div class="item-price-total">{{item.productPrice * item.productQuantity | formatMoney('元')}}</div>
                </div>
                <div class="cart-tab-5">
                  <div class="cart-item-operation">
                    <a href="javascript:;" class="item-edit-btn" @click="deleteConfirm(item)">
                      <svg class="icon icon-del"><use xlink:href="#icon-del" ></use></svg>
                    </a>
                  </div>
                </div>
              </li>
            </ul>
          </div>
        </div>
        <!-- footer -->
        <div class="cart-foot-wrap">
          <div class="cart-foot-l">
            <div class="item-all-check">
              <a href="javascript:void 0">
								<span class="item-check-btn" :class="{'check':isCheckAll}" @click="checkAll(true)">
									<svg class="icon icon-ok"><use xlink:href="#icon-ok"></use></svg>
								</span>
                <span v-show="!isCheckAll">全选</span>
              </a>
            </div>
            <div class="item-all-del">
              <a href="javascript:;" class="item-del-btn" @click="checkAll(false)">
                <span v-show="isCheckAll">取消全选</span>
              </a>
            </div>
          </div>
          <div class="cart-foot-r">
            <div class="item-total">
              Item total: <span class="total-price">{{totalMoney | formatMoney('元')}}</span>
            </div>
            <div class="next-btn-wrap">
              <router-link to="/address" class="btn btn--red" style="width: 200px">结账</router-link>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="md-modal modal-msg md-modal-transition" id="showModal" :class="{'md-show':isDelete}">
      <div class="md-modal-inner">
        <div class="md-top">
          <button class="md-close" @click="isDelete=false">关闭</button>
        </div>
        <div class="md-content">
          <div class="confirm-tips">
            <p id="cusLanInfo">你确认删除此订单信息吗?</p>
          </div>
          <div class="btn-wrap col-2">
            <button class="btn btn--m" id="btnModalConfirm" @click="deleteProduct">Yes</button>
            <button class="btn btn--m btn--red" id="btnModalCancel" @click="isDelete=false">No</button>
          </div>
        </div>
      </div>
    </div>
    <div class="md-overlay" id="showOverLay" v-if="isDelete"></div>
 
	</div>
</template>
<script>
	import AXIOS from '../axios/axios'
	const Axios = new AXIOS();
	export default {
		name: 'address',
		data () {
			return{
				productList: [],  //商品列表
				totalMoney: 0,    //商品总价
				isCheckAll: false,//是否全选 
				isDelete: false,  //是否删除
				curProduct: ''    //当前商品
			}
		},
		//局部过滤器
		filters: {
			formatMoney(value,param){
				return "￥" + value.toFixed(2) + param; // param '元'
				//货币不应该前端格式化，应该由后端格式化 ，因为前端格式化数据四舍五入不准确 特别是一些金额的计算  保留小数点后两位
			}
		},
		//vue2.0的生命周期类似ready 实例化完成以后需要调用那些方法
		mounted () {
			this.$nextTick(() => {
				//保证this.$el已经插入文档
				this.getCartList();
			})
		},
		methods: {
			getCartList: function(){
				let params = {
					api:'static/axios/cartData.json',
					param: {}
				};
				//Axios类似于jquery里面的ajax
				Axios.get(params)
					// .then(function(response){})
					.then(response => {
						this.productList = response.data.result.list;
					})
					.catch(error => {
						console.log(error);
					})
			},
			changeQuantity (product,type) {
				if(type > 0){
					product.productQuantity++;
				}else{
					product.productQuantity--;
					if(product.productQuantity < 1){
						product.productQuantity = 1;
					}
				}
				this.calcTotalPrice();
			},
			selectedProduct (item) {
				//判断一个变量里面的对象是否存在
				if(typeof item.checked == 'undefined'){
					//如果不存在  多看官网
					//往item变量里面注册一个checked属性，设置值为true
					//Vue.set全局
					//this.$set局部 如果用this 必须用$set
					this.$set(item,"checked",true);
				}else{
					item.checked = !item.checked;
				}
				this.calcTotalPrice();
			},
			checkAll (flag) {
				this.isCheckAll = flag;
					this.productList.forEach((product,index) => {
						if(typeof product.checked == 'undefined'){
							this.$set(product,"checked",this.isCheckAll);
						}else{
							product.checked = this.isCheckAll;
						}
					})
				this.calcTotalPrice();
			},
			calcTotalPrice () {
				var _this = this;
				this.totalMoney = 0;//默认每次操作前都先把总金额设置为0 ，防止累加
				this.productList.forEach((item,index) =>{
					if(item.checked){
						_this.totalMoney += item.productPrice * item.productQuantity;
					}
				})
			},
			deleteConfirm (item) {
				//显示提示层
				this.isDelete = true;
				this.curProduct = item;
			},
			deleteProduct () {
				//获取当前元素的索引
				let index = this.productList.indexOf(this.curProduct);
				//splice()从当前索引开始，删除一个元素
				//vue2.0提倡能用元素js实现的方法就用原生Js去实现
				this.productList.splice(index,1); //删除正常情况下需要调用后台接口 前端只是模拟一下
				//隐藏提示层
				this.isDelete = false;
				this.calcTotalPrice();
			}
		}
	}
	//全局过滤器
//	Vue.filter('formatMoney',function(value,param){
//		return "￥" + value.toFixed(2) + param;);
//	});
</script>

<style>
  .quantity input{
    width: 40px;
    padding: 5px 10px;
    text-align: center;
  }
  .partContent{
    width:130px;
    height: 50px;
  }
  .partContent .left{
    float:left;
    width:50px;
    height:50px;
    display: table-cell;
    vertical-align: middle;
    text-align: left;
  }
  .partContent .right{
    float:right;
    width:65px;
    height: 50px;
    margin-left: 10px;
    cursor:pointer;
  }
</style>