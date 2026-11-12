代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://ada.hammf.cn

[T51] Scala：Hello World
来源：http://ymq.quarkkingdee.top

println("Hello")
来源：http://vip.hywenlv.cn

[T52] Scala：变量
来源：http://xuo.ydzc1.top

val a = 1;  var b = 2
来源：http://vsh.fzhhl.top

[T53] Scala：字符串插值
来源：http://pht.hysaishi.cn

s"值: $b"
来源：http://xwo.jinqigufen.top

[T54] Scala：集合映射
来源：http://ovh.ppjwa.cn

List(1, 2, 3).map(_ * 2)
来源：http://wkh.fzhhl.top

[T55] Scala：集合过滤
来源：http://nhy.xuanzx.com

List(1, 2, 3).filter(_ > 1)
来源：http://bmk.tanke756.top

[T56] Scala：样例类
来源：http://hcy.ydzc1.top

case class User(name: String, age: Int)
来源：http://nkm.aizwys.cn

[T57] Scala：模式匹配
来源：http://buw.ydjk.org.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wlo.pycfn.com

[T58] Scala：函数定义
来源：http://twb.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://npe.gogol.net.cn

[T59] Scala：循环
来源：http://urq.smart0.xyz

for (i <- 1 to 10) println(i)
来源：http://eqf.yj202588.top

[T60] Scala：折叠
来源：http://jes.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aas.aibaodan.cn

================================================================================
来源：http://flm.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qpe.yangfankeji.com

================================================================================
来源：http://bnk.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://asb.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://mhn.ybcxt.top

[U02] Py：导出 / 安装依赖
来源：http://vjs.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://keh.cucudq.cn

[U03] Py：加载 .env 配置
来源：http://wxl.yonumen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lvl.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://neu.jinqigufen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ciy.hcnkem.com

[U05] Py：列表去重且保序
来源：http://dxo.chenjidiqi.icu

list(dict.fromkeys(arr))
来源：http://yez.yangfankeji.com

[U06] Py：合并两个字典
来源：http://lko.fengsongda.top

{**a, **b}
来源：http://utt.pycfn.com

[U07] Py：反转字典键值
来源：http://ltv.zhixingplan.top

{v: k for k, v in d.items()}
来源：http://xru.bbcook.cn

[U08] Py：展平二维列表
来源：http://vku.aizwys.cn

[y for x in nested for y in x]
来源：http://ptl.yueranfly.top

[U09] Py：字典取最大值的键
来源：http://iif.haohaochexian.top

max(d, key=d.get)
来源：http://lup.yj20258888.top

[U10] Py：按值排序字典
来源：http://jfu.cdnleiting.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jhj.fanxiaobao.xyz

[U11] Py：生成器表达式
来源：http://axs.c1oappe.top

(x * 2 for x in arr)
来源：http://iui.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gcd.jianghu66.top

Counter(arr).most_common(3)
来源：http://lmy.aizwys.cn

[U13] Py：固定长度队列
来源：http://shq.sxryk.cn

deque(maxlen=10)
来源：http://xxf.yangfankeji.com

[U14] Py：分组收集到列表
来源：http://yew.yangfankeji.com

defaultdict(list)
来源：http://scq.chenlongwang.top

[U15] Py：高精度计时
来源：http://bel.yonumen.top

t = time.perf_counter()
来源：http://srm.jianghu66.top

[U16] Py：命令行参数解析
来源：http://pwc.ydjk.org.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cwo.cheryme.top

[U17] Py：初始化日志
来源：http://blf.hysaishi.cn

logging.basicConfig(level=logging.INFO)
来源：http://jwp.gaohongyu789.top

[U18] Py：预编译正则
来源：http://dkw.cqqwz.cn

pat = re.compile(r"\d+")
来源：http://hqd.xuanzx.com

[U19] Py：正则替换带回调
来源：http://rrx.c1oappe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://prj.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://djz.dianchejie.cn

@functools.lru_cache(maxsize=None)
来源：http://hcd.yj20258.top

[U21] Py：自定义上下文管理器
来源：http://msx.bbcook.cn

@contextlib.contextmanager
来源：http://jvj.haohaochexian.top

[U22] Py：矩阵转置
来源：http://egv.haohaochexian.top

list(zip(*m))
来源：http://wgf.birdmap.top

[U23] Py：分块读取大文件
来源：http://zsp.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hol.chenjidiqi.icu

[U24] Py：路径操作
来源：http://jlc.cucudq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rja.redwolf501.top

[U25] Py：CSV 按字典读
来源：http://fil.zhixingplan.top

csv.DictReader(f)
来源：http://pfj.xylfe.cn

[U26] Py：并发下载
来源：http://xkk.jinqigufen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ulu.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://pcr.hfpthk.cn

aiohttp.ClientSession() 配合 async with
来源：http://eda.sysykeji.top

[U28] Py：类型别名
来源：http://qkr.jianghu66.top

UserId = int
来源：http://znh.tian-w.cn

[U29] Py：属性校验
来源：http://khd.haohaochexian.top

@property 与 @x.setter 配合
来源：http://svn.chenjidiqi.icu

[U30] Py：数据类
来源：http://bhd.yanxiufei.cn

@dataclass(slots=True)
来源：http://wye.haohaochexian.top

[U31] Py：单测
来源：http://npk.zhijiandao.cn

python -m pytest -q
来源：http://yak.wangshuangyany.cn

[U32] Py：代码格式化
来源：http://ots.havefunace.top

ruff format . && ruff check --fix .
来源：http://wya.zdbjq.cn

[U33] Py：打包发布
来源：http://kmo.shanyushiyangtech.top

python -m build  （依赖 pyproject.toml）
来源：http://psd.jqgufenzy.top

[U34] Py：判断编码
来源：http://irg.0kj1m.cn

chardet.detect(raw)
来源：http://toe.zhijiandao.cn

[U35] Py：发送邮件
来源：http://vdg.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ltd.tianlin.xyz

[U36] Py：定时任务
来源：http://djt.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://gdm.xylfe.cn

[U37] Py：读写 Excel
来源：http://kae.bjfxy.top

pandas.read_excel / DataFrame.to_excel
来源：http://uhz.zhixingplan.top

[U38] Py：获取脚本所在目录
来源：http://axc.cqqwz.cn

Path(__file__).resolve().parent
来源：http://byl.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://wko.hcnkem.com

sys.stdout.isatty()
来源：http://qxk.hesvh.cn

[U40] Py：打印到标准错误
来源：http://tqs.meibo888.top

print("err", file=sys.stderr)
来源：http://skt.vehdjk.com

[U41] PHP：初始化 Composer 项目
来源：http://pvy.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sii.quarkkingdee.top

[U42] PHP：PSR-4 自动加载
来源：http://igx.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xzw.bbcook.cn

[U43] PHP：声明命名空间
来源：http://fjw.feifeiyinyue.top

namespace App\Http;
来源：http://wac.fehbvm.com

[U44] PHP：开启严格类型
来源：http://ypq.zhiwuduotai.top

declare(strict_types=1);
来源：http://cng.xuanzx.com

[U45] PHP：类型声明与返回类型
来源：http://mvx.hammf.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uyo.zycfv.cn

[U46] PHP：可空类型
来源：http://kfy.gzhubu.top

?string $name = null
来源：http://ylc.daria6918.cn

[U47] PHP：联合类型
来源：http://bjy.xziqi.cn

int|string $id
来源：http://loe.guannengcc.top

[U48] PHP：纯枚举
来源：http://zbj.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zgs.zhongyouzk.top

[U49] PHP：只读属性
来源：http://bch.fzhhl.top

public readonly string $name
来源：http://cki.fanxiaobao.xyz

[U50] PHP：构造器属性提升
来源：http://nkr.yueranfly.top

public function __construct(private int $id) {}
来源：http://jbz.ywan-chungtsiang.top

[U51] PHP：数组解构
来源：http://erz.yongpay.top

[$a, $b] = $arr;
来源：http://cgl.sxryk.cn

[U52] PHP：箭头函数
来源：http://zyz.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://mlw.yongpay.top

[U53] PHP：空合并运算符
来源：http://ejm.jyoumei.cn

$v = $a ?? $b ?? "default";
来源：http://ybw.c1oappe.top

[U54] PHP：空安全调用
来源：http://yfp.shanyushiyangtech.top

$obj?->method()
来源：http://bhi.tian-w.cn

[U55] PHP：match 表达式
来源：http://eug.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://diw.daxiang520.top

[U56] PHP：命名参数
来源：http://rni.pengpengdd.cyou

f(a: 1, b: 2)
来源：http://fiz.jianghu66.top

[U57] PHP：字符串插值
来源：http://mxu.zdbjq.cn

"值: {$a}"
来源：http://gks.hnqzz.top

[U58] PHP：数组三件套
来源：http://xqm.zhongyouzk.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fsv.ppjwa.cn

[U59] PHP：自定义排序
来源：http://lhr.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bmg.hammf.cn

[U60] PHP：JSON 编解码
来源：http://urj.nwbrower.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jyi.ppjwa.cn

[U61] PHP：正则
来源：http://dkp.ybcxt.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pkl.aibaodan.cn

[U62] PHP：日期对象
来源：http://hzb.fzhhl.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lla.zhaomingkeji.xyz

[U63] PHP：文件读写
来源：http://aqn.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rmt.xingfuxueyuan.xyz

[U64] PHP：目录遍历
来源：http://txt.xingfuxueyuan.xyz

glob("dir/*.php");  scandir("dir");
来源：http://jwl.jianghu66.top

[U65] PHP：会话
来源：http://wdg.pengpengdd.cyou

session_start();  $_SESSION["uid"] = 1;
来源：http://jlb.andypj.xyz

[U66] PHP：设置 Cookie
来源：http://wcr.vqdsnc.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fnk.xuetiantiany.cn

[U67] PHP：处理文件上传
来源：http://mqk.andypj.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hqx.ivvv.top

[U68] PHP：PDO 连接
来源：http://hkf.hywenlv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iup.fehbvm.com

[U69] PHP：PDO 预处理
来源：http://itu.zhongyouzk.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mxj.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://vid.yonumen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cxo.iojbl.cn

[U71] PHP：抛出异常
来源：http://ipx.ydjk.org.cn

throw new RuntimeException("失败", 500);
来源：http://xjm.shzxlz.cn

[U72] PHP：写错误日志
来源：http://uhz.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://phe.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://hyz.sxryk.cn

parse_ini_file("config.ini", true)
来源：http://bag.ydzc1.top

[U74] PHP：读取环境变量
来源：http://mya.tian-w.cn

getenv("APP_ENV") ?: "production"
来源：http://lud.ctjpmb.com

[U75] PHP：依赖注入
来源：http://eed.hongshengwenyu.top

composer require psr/container
来源：http://wna.yueranfly.top

[U76] PHP：简单路由
来源：http://ouw.xingfuxueyuan.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dvf.chenlongwang.top

[U77] PHP：模板渲染
来源：http://gqv.yj202588.top

composer require twig/twig
来源：http://zxq.mhx1999.top

[U78] PHP：单元测试
来源：http://yju.redwolf501.top

composer require --dev phpunit/phpunit
来源：http://mme.hesvh.cn

[U79] PHP：静态分析
来源：http://lwr.jinqigufen.top

composer require --dev phpstan/phpstan
来源：http://vqf.sxryk.cn

[U80] PHP：代码规范修复
来源：http://ebm.gotoacloud.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://can.jinqigfzy.top

[U81] JS：初始化项目
来源：http://omv.hywenlv.cn

npm init -y;  npm i express
来源：http://bvt.jiagoushi.top

[U82] JS：package.json 脚本
来源：http://wed.sysykeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qbi.shanyushiyangtech.top

[U83] JS：ES Module 导入导出
来源：http://wqp.yj20258.top

export const a = 1;  import { a } from "./m.js";
来源：http://hla.yonumen.top

[U84] JS：CommonJS 写法
来源：http://vvg.jinqigfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://evv.chenjidiqi.icu

[U85] JS：可选链
来源：http://ktv.ydzc1.top

a?.b?.c
来源：http://dkk.sjlbkw.cn

[U86] JS：空值合并
来源：http://hfu.cdnleiting.top

a ?? b
来源：http://txt.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://pca.dashuyun.cn

const { a = 1, b = 2 } = obj;
来源：http://njk.52xcode.cn

[U88] JS：对象展开合并
来源：http://ecw.hcnkem.com

{ ...a, ...b }
来源：http://kdt.cashguo.top

[U89] JS：数组去重
来源：http://wxl.dianchejie.cn

[...new Set(arr)]
来源：http://sia.yj20258888.top

[U90] JS：数字数组排序
来源：http://kec.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://elg.hesvh.cn

[U91] JS：对象键值遍历
来源：http://vce.jinyuanbaomall.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vtz.yj20258888.top

[U92] JS：深拷贝
来源：http://iyv.aibaodan.cn

structuredClone(obj)
来源：http://njw.vqdsnc.cn

[U93] JS：模板字符串
来源：http://gjr.shzxlz.cn

`共 ${n} 条`
来源：http://xwe.shanyushiyangkeji.top

[U94] JS：箭头函数
来源：http://kxt.ppjwa.cn

const double = x => x * 2;
来源：http://ejp.zhixingplan.top

[U95] JS：Promise 包装
来源：http://dxu.ctjpmb.com

new Promise((resolve, reject) => {})
来源：http://zwb.yj20258888.top

[U96] JS：async/await 与异常
来源：http://vgw.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qvj.hnxiangtu.top

[U97] JS：并发请求
来源：http://iiu.andypj.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://kxd.bjfxy.top

[U98] JS：fetch 带 JSON
来源：http://erq.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vgm.shangyingyoupin.top

[U99] JS：事件监听
来源：http://vko.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://tjd.jinghuilouyu.cn

[U100] JS：DOM 查询
来源：http://ywq.fehbvm.com

document.querySelector(".item")
来源：http://bxe.yfazqb.com

[U101] JS：classList 操作
来源：http://ugr.cheryme.top

el.classList.toggle("active")
来源：http://psn.yj20258.top

[U102] JS：本地存储
来源：http://teg.yvedp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hof.sweek.top

[U103] JS：定时器
来源：http://wfm.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ibo.ybcxt.top

[U104] JS：防抖
来源：http://drb.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://irg.hnqzz.top

[U105] JS：节流
来源：http://ipo.cdnleiting.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mjp.yj20258.top

[U106] JS：日期格式化
来源：http://tie.zhaomingkeji.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zpe.vqdsnc.cn

[U107] JS：数字千分位
来源：http://rlg.meibo888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zzz.zhixingplan.top

[U108] JS：随机整数
来源：http://epf.xziqi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wei.yonumen.top

[U109] JS：数组分组
来源：http://rgy.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://loo.fanxiaobao.xyz

[U110] JS：数组分块
来源：http://ywj.aizwys.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zyz.316326.xyz

[U111] JS：对象转 Map
来源：http://dkr.316326.xyz

new Map(Object.entries(obj))
来源：http://xfg.mhx1999.top

[U112] JS：字符串补位
来源：http://amm.hammf.cn

"7".padStart(3, "0")
来源：http://yzi.mhx1999.top

[U113] JS：正则替换全部
来源：http://fpi.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://fit.yueranfly.top

[U114] JS：JSON 深比较
来源：http://zjn.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ihj.wangshuangyany.cn

[U115] JS：生成 UUID
来源：http://tcu.vqdsnc.cn

crypto.randomUUID()
来源：http://shh.hcnkem.com

[U116] JS：类型检查（JSDoc）
来源：http://fdd.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://ekc.aizwys.cn

[U117] JS：单元测试
来源：http://yfk.nanxinkj.top

npm i -D vitest;  npx vitest
来源：http://ahv.chenzaomai.com

[U118] JS：开发服务器
来源：http://ges.xuetiantiany.cn

npm i -D vite;  npx vite
来源：http://yjr.jyoumei.cn

[U119] JS：生产构建
来源：http://pzr.zhixingplan.top

npx vite build
来源：http://ngk.yuanzhike.top

[U120] JS：读取环境变量（Vite）
来源：http://qch.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://rmj.yongpay.top

================================================================================
来源：http://fxa.hfpthk.cn

统计汇总
来源：http://evq.zhengqikj.top

================================================================================
来源：http://nxt.ehwqpu.com

按语言统计（条）：
来源：http://iqt.hnqzz.top

Python ......... 252
来源：http://hpr.dashuyun.cn

PHP ............ 252
来源：http://etz.cqqwz.cn

JavaScript ..... 252
来源：http://tux.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://fxc.shuidangran.top

Java ........... 212
来源：http://mia.nwbrower.top

Go ............. 212
来源：http://yyq.tarul.cn

Ruby ........... 212
来源：http://chf.sxryk.cn

C# ............. 212
来源：http://zng.c1oappe.top

C .............. 30
来源：http://vav.yj20258888.top

C++ ............ 30
来源：http://dwu.bjfxy.top

SQL ............ 90
来源：http://ypn.hnqzz.top

Bash ........... 80
来源：http://ihe.birdmap.top

Kotlin ......... 15
来源：http://xln.hysaishi.cn

Swift .......... 15
来源：http://jqa.shzxlz.cn

Lua ............ 10
来源：http://ysp.nanxinkj.top

Perl ........... 10
来源：http://aqr.cdnleiting.top

Scala .......... 10
来源：http://dip.ywan-chungtsiang.top

------------------------------------
来源：http://cxf.tian-w.cn

合计 ........... 2106 条
来源：http://eta.yongpay.top

按章节统计：
来源：http://wrw.chenzaomai.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://umx.guannengcc.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kao.ywan-chungtsiang.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rxd.mhx1999.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gml.smart0.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sra.yongpay.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ntz.kuanghao11.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jyh.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dhu.sufxvd.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rkk.nanxinkj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vuc.shanyushiyangtech.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gjy.yj20258.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hpr.fanxiaobao.xyz


<!-- 参考信息 -->