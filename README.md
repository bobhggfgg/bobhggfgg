# 本配置文件仅适用于 [萌通加速]1.2.1 以上版本，如有不懂请联系开发者 tg:@gogocloudd
# 注意：修改内容请严格遵守 yaml 格式，特别是缩进和空格，否则 app 可能会报错
# 开发者：TG：@gogocloudd
# 授权密钥（月付版必填）
license: "eteswjfbdskfhsdklfhksj"

# app与v2b面板的通信地址，一般是面板前端域名
# 月付版注意：这里的域名一定要和授权域名一致，若更换域名请联系开发者重新获取授权密钥
apiUrl: "https://zhlt.site"

# Crisp在线客服，不填写则入口隐藏
crispId: ""

# 邀请链接，APP里点复制链接，邀请码会拼接在最后
inviteUrl: "https://zhlt.site/#/login?code="

# 节点延迟的展示相关
nodeDelayShow:
  type: 1 # 展示方式：0=延迟数值，1=信号图标
  colorBest: 1500 # 延迟数值/图标颜色：延迟小于此值为绿色
  colorGood: 2500 # 延迟数值/图标颜色：延迟小于此值并大于{colorBest}为黄色，大于此值为红色

# 是否显示流量明细入口 true=显示，false=隐藏
trafficLogShow: true

# 用户协议及隐私政策
agreements:
  # 是否显示（总开关：[第一次进入app、登录、注册、其他设置-关于]的显示）
  show: false
  # 第一次进入 app 的弹窗标题
  title: "个人信息保护提示"
  # 第一次进入 app 的弹窗内容，支持文字a标签跳转
  content: "感谢您使用gogocloud！我们将依据<a href='https://moetor.one/user-agreement.html'>《用户服务协议》</a>和<a href='https://moetor.one/privacy-policy.html'>《隐私政策》</a>来帮助您了解我们在收集、使用、存储和共享您个人信息的情况以及您享有的相关权利。<br><br>1、您可以通过查看《用户服务协议》和《隐私政策》来了解我们可能收集、使用的您的个人信息情况；<br><br>2、基于您的明示授权，我们可能调用您的重要设备权限。我们将在首次调用时逐项询问您是否允许使用该权限，您有权拒绝或取消授权；<br><br>3、我们会采取业界先进的安全措施保护您的信息安全；<br><br>4、您可以查询、更正、删除、撤回授权您的个人信息，我们也提供账户注销的渠道。<br><br>"
  # 服务协议url
  serviceLink: ""
  # 隐私政策url
  privacyLink: ""

# 版本更新时是否强制，最新版本信息请在面板-系统配置-APP-Android进行配置，下载地址需要apk文件直链url
versionUpdateForce: false

# 每次进入app时的弹窗，支持多弹窗队列弹出
noticeList:
  - show: true  # 开关
    title: "邀请返利15%"
    content: "每邀请一名朋友并成为我们的会员，您将获得邀请佣金奖励(佣金比例30%)，若朋友在gogocloud消费100元，您则可获得返利15元。此返利可用于购买套餐或提现！【快来和我们一起赚钱吧！】"
    negative: ""  # 左边按钮文字，不填则隐藏
    position: ""  # 右边按钮文字，不填则隐藏
    positionLink: ""  # 右边按钮跳转地址，不填则不进行跳转

    # 示例
  - show: false
    title: "这是第二个弹窗"
    content: "这里是弹窗内容"
    negative: ""
    position: ""
    positionLink: ""

# 购买套餐下单时的弹窗
buyTip:
  show: false
  title: "购买须知"
  content: "是否确认购买？"


# 首页网站推荐
homeNav:
  show: false # 是否显示
  title: "gogocloud"  # 标题
  list: #以下列表数量不限可以无限添加，但请注意格式
    - text: "gogocloud"
      icon: "https://cdn-fusion.imgimg.cc/i/2024/bd877a1512fffaec.jpg"
      link: "https://zhlt.site"
      needConnected: false # 是否在连接状态下才能跳转
   
