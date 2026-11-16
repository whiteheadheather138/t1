代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://ght.guowangkeji.top

[T51] Scala：Hello World
来源：http://bhm.jinghuilouyu.cn

println("Hello")
来源：http://mmv.kuanghao11.cn

[T52] Scala：变量
来源：http://taf.jqgfzy.top

val a = 1;  var b = 2
来源：http://swm.daria6918.cn

[T53] Scala：字符串插值
来源：http://iby.hnqzz.top

s"值: $b"
来源：http://gyq.yanxiufei.cn

[T54] Scala：集合映射
来源：http://wcg.shangyingyoupin.top

List(1, 2, 3).map(_ * 2)
来源：http://bee.shuidangran.top

[T55] Scala：集合过滤
来源：http://blw.aibaodan.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ert.yuxming.cn

[T56] Scala：样例类
来源：http://mfz.yj20258888.top

case class User(name: String, age: Int)
来源：http://yec.shuidangran.top

[T57] Scala：模式匹配
来源：http://bki.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vri.fehbvm.com

[T58] Scala：函数定义
来源：http://ozw.ctjpmb.com

def add(a: Int, b: Int): Int = a + b
来源：http://dds.zhoulong.xyz

[T59] Scala：循环
来源：http://aqz.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://lwg.zhijiandao.cn

[T60] Scala：折叠
来源：http://uit.jqgufenzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nax.zhongyouzk.top

================================================================================
来源：http://eae.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tco.smart0.xyz

================================================================================
来源：http://rvv.tianlin.xyz

[U01] Py：创建虚拟环境
来源：http://ite.chenjidiqi.icu

python -m venv .venv && source .venv/bin/activate
来源：http://vmo.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://sqi.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iad.sufxvd.cn

[U03] Py：加载 .env 配置
来源：http://irw.cashguo.top

from dotenv import load_dotenv; load_dotenv()
来源：http://obt.zdqjudy.top

[U04] Py：变量调试打印
来源：http://yrh.yj20258888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ocv.zdqjudy.top

[U05] Py：列表去重且保序
来源：http://cuc.ydzc1.top

list(dict.fromkeys(arr))
来源：http://dpa.tian-w.cn

[U06] Py：合并两个字典
来源：http://pzh.chenzaomai.com

{**a, **b}
来源：http://nxp.yangfankeji.com

[U07] Py：反转字典键值
来源：http://hvg.tian-w.cn

{v: k for k, v in d.items()}
来源：http://mog.uphjek.com

[U08] Py：展平二维列表
来源：http://sjb.snrcjt.cn

[y for x in nested for y in x]
来源：http://wok.hysaishi.cn

[U09] Py：字典取最大值的键
来源：http://khs.yj20258888.top

max(d, key=d.get)
来源：http://dhj.iojbl.cn

[U10] Py：按值排序字典
来源：http://kmp.yanxiufei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yny.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://zjr.bjfxy.top

(x * 2 for x in arr)
来源：http://rae.zhaomingkeji.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://doy.aizwys.cn

Counter(arr).most_common(3)
来源：http://wpr.birdmap.top

[U13] Py：固定长度队列
来源：http://ojy.sxryk.cn

deque(maxlen=10)
来源：http://mwb.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://jjx.havefunace.top

defaultdict(list)
来源：http://fcu.daria6918.cn

[U15] Py：高精度计时
来源：http://vdn.52xcode.cn

t = time.perf_counter()
来源：http://dvu.zhongyouzk.top

[U16] Py：命令行参数解析
来源：http://lcd.gogol.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pqv.ppjwa.cn

[U17] Py：初始化日志
来源：http://lfa.nanxuanxn.top

logging.basicConfig(level=logging.INFO)
来源：http://mbt.ywan-chungtsiang.top

[U18] Py：预编译正则
来源：http://qze.sxryk.cn

pat = re.compile(r"\d+")
来源：http://dnc.yfazqb.com

[U19] Py：正则替换带回调
来源：http://rxf.chenjidiqi.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://plq.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://bop.tianlin.xyz

@functools.lru_cache(maxsize=None)
来源：http://vfb.guannengcc.top

[U21] Py：自定义上下文管理器
来源：http://mio.yanxiufei.cn

@contextlib.contextmanager
来源：http://kdt.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://jsl.9152youxi.cn

list(zip(*m))
来源：http://qaa.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://aew.gaohongyu789.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://joq.aizwys.cn

[U24] Py：路径操作
来源：http://pxl.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wbk.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://jvm.yongpay.top

csv.DictReader(f)
来源：http://ljy.fktsv.cn

[U26] Py：并发下载
来源：http://msx.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gvz.snrcjt.cn

[U27] Py：异步 HTTP
来源：http://ksp.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://ged.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://xre.fehbvm.com

UserId = int
来源：http://edd.zhixingplan.top

[U29] Py：属性校验
来源：http://hjj.daxiang520.top

@property 与 @x.setter 配合
来源：http://mmf.xuetiantiany.cn

[U30] Py：数据类
来源：http://mvd.svipenyu.cn

@dataclass(slots=True)
来源：http://wad.tarul.cn

[U31] Py：单测
来源：http://gqf.sxryk.cn

python -m pytest -q
来源：http://avu.svipenyu.cn

[U32] Py：代码格式化
来源：http://xaf.uphjek.com

ruff format . && ruff check --fix .
来源：http://ldw.fzhhl.top

[U33] Py：打包发布
来源：http://ldg.ydzc1.top

python -m build  （依赖 pyproject.toml）
来源：http://swl.yongpay.top

[U34] Py：判断编码
来源：http://szg.yfazqb.com

chardet.detect(raw)
来源：http://jzu.jianghu66.top

[U35] Py：发送邮件
来源：http://jli.aibaodan.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eqj.tanke756.top

[U36] Py：定时任务
来源：http://ldw.zycfv.cn

schedule.every(10).minutes.do(job)
来源：http://wui.aibaodan.cn

[U37] Py：读写 Excel
来源：http://vmo.cqqwz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iwu.0kj1m.cn

[U38] Py：获取脚本所在目录
来源：http://tne.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://oua.hfpthk.cn

[U39] Py：判断是否在交互环境
来源：http://fgb.c1oappe.top

sys.stdout.isatty()
来源：http://mvx.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://cya.daria6918.cn

print("err", file=sys.stderr)
来源：http://dwb.jinyuanbaomall.cn

[U41] PHP：初始化 Composer 项目
来源：http://rta.jianghu66.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nic.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://cdx.hongshengwenyu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cuj.chenlongwang.top

[U43] PHP：声明命名空间
来源：http://vyh.shuidangran.top

namespace App\Http;
来源：http://qcv.fengsongda.top

[U44] PHP：开启严格类型
来源：http://via.fengsongda.top

declare(strict_types=1);
来源：http://hvl.jinqigufen.top

[U45] PHP：类型声明与返回类型
来源：http://aiu.hesvh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://aum.havefunace.top

[U46] PHP：可空类型
来源：http://xeo.yj202588.top

?string $name = null
来源：http://jxj.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://xot.sxryk.cn

int|string $id
来源：http://ima.cheryme.top

[U48] PHP：纯枚举
来源：http://dep.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kmy.wangdashe.top

[U49] PHP：只读属性
来源：http://mdb.shuidangran.top

public readonly string $name
来源：http://jqc.iojbl.cn

[U50] PHP：构造器属性提升
来源：http://ovc.aizwys.cn

public function __construct(private int $id) {}
来源：http://tan.tianlin.xyz

[U51] PHP：数组解构
来源：http://vpu.yuxming.cn

[$a, $b] = $arr;
来源：http://uzu.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://feb.ydzc1.top

$double = fn($x) => $x * 2;
来源：http://elj.daria6918.cn

[U53] PHP：空合并运算符
来源：http://csb.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://wus.smart0.xyz

[U54] PHP：空安全调用
来源：http://kfr.bbcook.cn

$obj?->method()
来源：http://dtr.yuxming.cn

[U55] PHP：match 表达式
来源：http://hpe.zhoulong.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kam.yvedp.cn

[U56] PHP：命名参数
来源：http://jrm.jinqigufen.top

f(a: 1, b: 2)
来源：http://dlc.hongshengwenyu.top

[U57] PHP：字符串插值
来源：http://ajw.gaohongyu789.top

"值: {$a}"
来源：http://qpf.havefunace.top

[U58] PHP：数组三件套
来源：http://ysc.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mue.guannengcc.top

[U59] PHP：自定义排序
来源：http://nsz.zhixingplan.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rie.sxryk.cn

[U60] PHP：JSON 编解码
来源：http://fjr.zhengqikj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nix.vehdjk.com

[U61] PHP：正则
来源：http://drl.yj202588.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://owf.hnqzz.top

[U62] PHP：日期对象
来源：http://ujh.jianghu66.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nnc.uphjek.com

[U63] PHP：文件读写
来源：http://gim.xziqi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wim.shzxlz.cn

[U64] PHP：目录遍历
来源：http://nrs.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://afu.cheryme.top

[U65] PHP：会话
来源：http://lqj.ctjpmb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://ydn.c1oappe.top

[U66] PHP：设置 Cookie
来源：http://yzt.feifeiyinyue.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cjb.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://hnt.zhiwuduotai.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tlb.yfazqb.com

[U68] PHP：PDO 连接
来源：http://cin.zdqjudy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uvl.aibaodan.cn

[U69] PHP：PDO 预处理
来源：http://eku.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mqj.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://dji.xingfuxueyuan.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cix.ppjwa.cn

[U71] PHP：抛出异常
来源：http://ppc.ybcxt.top

throw new RuntimeException("失败", 500);
来源：http://pod.smart0.xyz

[U72] PHP：写错误日志
来源：http://txd.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://zqw.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://zwt.nanxuanxn.top

parse_ini_file("config.ini", true)
来源：http://rgp.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://mmz.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://czy.yonumen.top

[U75] PHP：依赖注入
来源：http://gwg.hnqzz.top

composer require psr/container
来源：http://zlu.sysykeji.top

[U76] PHP：简单路由
来源：http://itq.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jle.vqdsnc.cn

[U77] PHP：模板渲染
来源：http://jol.jinyuanbaomall.cn

composer require twig/twig
来源：http://fca.ppjwa.cn

[U78] PHP：单元测试
来源：http://yiy.aizwys.cn

composer require --dev phpunit/phpunit
来源：http://rue.zhoulong.xyz

[U79] PHP：静态分析
来源：http://bma.shzxlz.cn

composer require --dev phpstan/phpstan
来源：http://mcn.zhixingplan.top

[U80] PHP：代码规范修复
来源：http://iog.zycfv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tuf.guowangkeji.top

[U81] JS：初始化项目
来源：http://skf.cashguo.top

npm init -y;  npm i express
来源：http://fjg.svipenyu.cn

[U82] JS：package.json 脚本
来源：http://vhx.havefunace.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lox.smart0.xyz

[U83] JS：ES Module 导入导出
来源：http://bzs.birdmap.top

export const a = 1;  import { a } from "./m.js";
来源：http://wmn.daria6918.cn

[U84] JS：CommonJS 写法
来源：http://jrj.hesvh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wre.fanxiaobao.xyz

[U85] JS：可选链
来源：http://liv.zhiwuduotai.top

a?.b?.c
来源：http://jjm.redwolf501.top

[U86] JS：空值合并
来源：http://efm.yj202588.top

a ?? b
来源：http://dbl.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://puq.yuxming.cn

const { a = 1, b = 2 } = obj;
来源：http://zyc.daxiang520.top

[U88] JS：对象展开合并
来源：http://kcu.fanxiaobao.xyz

{ ...a, ...b }
来源：http://bie.xuetiantiany.cn

[U89] JS：数组去重
来源：http://brq.vqdsnc.cn

[...new Set(arr)]
来源：http://pbw.jiagoushi.top

[U90] JS：数字数组排序
来源：http://rji.9152youxi.cn

[...arr].sort((a, b) => a - b)
来源：http://fbv.haohaochexian.top

[U91] JS：对象键值遍历
来源：http://gad.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://igz.xylfe.cn

[U92] JS：深拷贝
来源：http://gxp.shzxlz.cn

structuredClone(obj)
来源：http://dqr.jiagoushi.top

[U93] JS：模板字符串
来源：http://wsp.yj20258.top

`共 ${n} 条`
来源：http://dce.gogol.net.cn

[U94] JS：箭头函数
来源：http://xgt.fktsv.cn

const double = x => x * 2;
来源：http://vuy.yvedp.cn

[U95] JS：Promise 包装
来源：http://wzq.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://rjc.jianghu66.top

[U96] JS：async/await 与异常
来源：http://edu.fanxiaobao.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ive.ivvv.top

[U97] JS：并发请求
来源：http://aaj.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://ewx.xziqi.cn

[U98] JS：fetch 带 JSON
来源：http://qrc.fktsv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qib.fktsv.cn

[U99] JS：事件监听
来源：http://ypy.shuidangran.top

el.addEventListener("click", e => {})
来源：http://lgx.zdbjq.cn

[U100] JS：DOM 查询
来源：http://mvl.zhiwuduotai.top

document.querySelector(".item")
来源：http://qsb.fktsv.cn

[U101] JS：classList 操作
来源：http://smd.gzhubu.top

el.classList.toggle("active")
来源：http://qam.xylfe.cn

[U102] JS：本地存储
来源：http://myt.havefunace.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xdw.yanxiufei.cn

[U103] JS：定时器
来源：http://hmy.guowangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://due.chenjidiqi.icu

[U104] JS：防抖
来源：http://sum.yfazqb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wwp.vehdjk.com

[U105] JS：节流
来源：http://lku.0kj1m.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ncr.jinqigfzy.top

[U106] JS：日期格式化
来源：http://ohh.tianlin.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cyt.hysaishi.cn

[U107] JS：数字千分位
来源：http://vke.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vcw.zhixingplan.top

[U108] JS：随机整数
来源：http://msl.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qdf.zhixingplan.top

[U109] JS：数组分组
来源：http://gpf.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://ewt.cucudq.cn

[U110] JS：数组分块
来源：http://vem.pengpengdd.cyou

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vfg.shzxlz.cn

[U111] JS：对象转 Map
来源：http://xns.cucudq.cn

new Map(Object.entries(obj))
来源：http://zow.vqdsnc.cn

[U112] JS：字符串补位
来源：http://pxd.jianghu66.top

"7".padStart(3, "0")
来源：http://nsl.hammf.cn

[U113] JS：正则替换全部
来源：http://gde.fanxiaobao.xyz

s.replaceAll("a", "b")
来源：http://wag.guannengcc.top

[U114] JS：JSON 深比较
来源：http://mej.jqgufenzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hsx.shanyushiyangkeji.top

[U115] JS：生成 UUID
来源：http://deb.aibaodan.cn

crypto.randomUUID()
来源：http://cxa.jinghuilouyu.cn

[U116] JS：类型检查（JSDoc）
来源：http://mpa.shzxlz.cn

/** @param {string} name */ function f(name) {}
来源：http://xlx.hnqzz.top

[U117] JS：单元测试
来源：http://yrr.vehdjk.com

npm i -D vitest;  npx vitest
来源：http://kla.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://kou.sysykeji.top

npm i -D vite;  npx vite
来源：http://svm.ybcxt.top

[U119] JS：生产构建
来源：http://ayu.meibo888.top

npx vite build
来源：http://bzr.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://yxh.zhixingplan.top

import.meta.env.VITE_API_URL
来源：http://gdh.sweek.top

================================================================================
来源：http://imq.sjlbkw.cn

统计汇总
来源：http://hzu.tianlin.xyz

================================================================================
来源：http://fiq.zhaomingkeji.xyz

按语言统计（条）：
来源：http://txl.jinqigfzy.top

Python ......... 252
来源：http://pjx.jianghu66.top

PHP ............ 252
来源：http://oyf.uphjek.com

JavaScript ..... 252
来源：http://stb.fzhhl.top

TypeScript ..... 212
来源：http://etn.smart0.xyz

Java ........... 212
来源：http://jxy.yongpay.top

Go ............. 212
来源：http://euf.yj20258888.top

Ruby ........... 212
来源：http://knr.meibo888.top

C# ............. 212
来源：http://vsl.nanxinkj.top

C .............. 30
来源：http://rha.zhijiandao.cn

C++ ............ 30
来源：http://evb.nanxinkj.top

SQL ............ 90
来源：http://you.bjfxy.top

Bash ........... 80
来源：http://jcs.fzhhl.top

Kotlin ......... 15
来源：http://ayc.yonumen.top

Swift .......... 15
来源：http://tsd.mhx1999.top

Lua ............ 10
来源：http://brd.quarkkingdee.top

Perl ........... 10
来源：http://uee.jinqigfzy.top

Scala .......... 10
来源：http://hyx.cashguo.top

------------------------------------
来源：http://gjc.zdbjq.cn

合计 ........... 2106 条
来源：http://rqn.wangshuangyany.cn

按章节统计：
来源：http://ykh.hnxiangtu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hgq.316326.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xul.jinyuanbaomall.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bqw.dashuyun.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xut.hnqzz.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://byn.zycfv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ixr.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://avv.birdmap.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ypv.xuetiantiany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tjc.sjlbkw.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lsn.hysaishi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tkb.dashuyun.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jsy.yanxiufei.cn


<!-- 参考信息 -->