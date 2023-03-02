<template>
  <div class="resume-profile">
    <var-row :gutter="20">
      <var-col justify="center" :span="12" :xs="24">
        <var-paper class="resume-profile-paper" :elevation="2" :radius="4">
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-cake class="resume-profile-icon" />
              <span>出生日期: 1996年08月22日</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-school class="resume-profile-icon" />
              <span>学校: 四川大学锦江学院（计算机应用技术）</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-calendar class="resume-profile-icon" />
              <span>工作年限: 7年</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-account-group class="resume-profile-icon" />
              <span>期望岗位: 前端开发工程师</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-cash class="resume-profile-icon" />
              <span>期望薪资: 面议</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0">
            <div class="resume-profile-cell">
              <icon-city class="resume-profile-icon" />
              <span>期望城市: 江苏无锡</span>
            </div>
          </var-cell>
        </var-paper>
      </var-col>

      <var-col :span="12" :xs="24">
        <var-paper class="resume-profile-paper" :elevation="2" :radius="4">
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-phone class="resume-profile-icon" />
              <span>手机: 18980433852</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-email class="resume-profile-icon" />
              <span>邮箱: 357229046@qq.com</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-tencent class="resume-profile-icon" />
              <span>QQ: 357229046</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-wechat class="resume-profile-icon" />
              <span>微信: qh357229046</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-post class="resume-profile-icon" />
              <span>
                掘金:
                <var-link type="primary" href="https://juejin.cn/user/1046390801697319" style="font-size: 12px">
                  https://juejin.cn/user/1046390801697319
                </var-link>
              </span>
            </div>
          </var-cell>
          <var-cell :border-offset="0">
            <div class="resume-profile-cell">
              <icon-github class="resume-profile-icon" />
              <span>
                Github:
                <var-link type="primary" href="https://github.com/haoziqaq" style="font-size: 12px">
                  https://github.com/haoziqaq
                </var-link>
              </span>
            </div>
          </var-cell>
        </var-paper>
      </var-col>
    </var-row>
  </div>
</template>

<style lang="less" scoped>
.resume-profile {
  width: 100%;

  &-paper {
    width: 100%;
    margin-top: 30px;
  }

  &-cell {
    display: flex;
    align-items: center;
  }

  &-icon {
    width: 22px;
    margin-right: 10px;
    fill: var(--color-primary);
  }
}
</style>
