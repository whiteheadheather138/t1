代发 wailian999

[T47] Perl：正则捕获
来源：http://wux.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://msf.hesvh.cn

[T48] Perl：正则替换
来源：http://kyf.tian-w.cn

$s =~ s/old/new/g;
来源：http://qhq.52xcode.cn

[T49] Perl：函数
来源：http://gfn.xylfe.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xlq.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://cbh.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://fxo.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://owk.jlsjyb.cn

[T51] Scala：Hello World
来源：http://cuc.yonumen.top

println("Hello")
来源：http://ajr.zdbjq.cn

[T52] Scala：变量
来源：http://buh.hongshengwenyu.top

val a = 1;  var b = 2
来源：http://yeh.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://gby.hnqzz.top

s"值: $b"
来源：http://lhw.cashguo.top

[T54] Scala：集合映射
来源：http://kct.nanxuanxn.top

List(1, 2, 3).map(_ * 2)
来源：http://jvw.andypj.xyz

[T55] Scala：集合过滤
来源：http://zjk.yueranfly.top

List(1, 2, 3).filter(_ > 1)
来源：http://bdd.chenlongwang.top

[T56] Scala：样例类
来源：http://zvc.zhoulong.xyz

case class User(name: String, age: Int)
来源：http://owz.yj202588.top

[T57] Scala：模式匹配
来源：http://asi.ydjk.org.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tfu.uphjek.com

[T58] Scala：函数定义
来源：http://olc.quarkkingdee.top

def add(a: Int, b: Int): Int = a + b
来源：http://egf.daria6918.cn

[T59] Scala：循环
来源：http://oml.jinyuanbaomall.cn

for (i <- 1 to 10) println(i)
来源：http://wxu.fktsv.cn

[T60] Scala：折叠
来源：http://noe.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vkx.haohaochexian.top

================================================================================
来源：http://jrt.birdmap.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tmb.bjfxy.top

================================================================================
来源：http://xsp.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://ywl.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ijn.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://cup.yueranfly.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vxe.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://osj.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://thb.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://trq.xylfe.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xtc.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://gal.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://lqi.yangfankeji.com

[U06] Py：合并两个字典
来源：http://pkb.yuxming.cn

{**a, **b}
来源：http://ulf.feifeiyinyue.top

[U07] Py：反转字典键值
来源：http://hsy.zycfv.cn

{v: k for k, v in d.items()}
来源：http://ptt.ywan-chungtsiang.top

[U08] Py：展平二维列表
来源：http://jew.zhijiandao.cn

[y for x in nested for y in x]
来源：http://knb.jyoumei.cn

[U09] Py：字典取最大值的键
来源：http://tkw.wangdashe.top

max(d, key=d.get)
来源：http://ugw.wangdashe.top

[U10] Py：按值排序字典
来源：http://ipr.uphjek.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jao.zhijiandao.cn

[U11] Py：生成器表达式
来源：http://dce.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://ved.gotoacloud.top

[U12] Py：取出现最多的 3 个元素
来源：http://dee.316326.xyz

Counter(arr).most_common(3)
来源：http://dtz.xuanzx.com

[U13] Py：固定长度队列
来源：http://flx.chenlongwang.top

deque(maxlen=10)
来源：http://qpz.pycfn.com

[U14] Py：分组收集到列表
来源：http://aam.bbcook.cn

defaultdict(list)
来源：http://end.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://xij.zdqjudy.top

t = time.perf_counter()
来源：http://usr.pengpengdd.cyou

[U16] Py：命令行参数解析
来源：http://hrn.cheryme.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sdz.aibaodan.cn

[U17] Py：初始化日志
来源：http://yhc.sysykeji.top

logging.basicConfig(level=logging.INFO)
来源：http://scp.havefunace.top

[U18] Py：预编译正则
来源：http://olt.9152youxi.cn

pat = re.compile(r"\d+")
来源：http://tqh.tianlin.xyz

[U19] Py：正则替换带回调
来源：http://yyd.hnqzz.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tez.xylfe.cn

[U20] Py：缓存函数结果
来源：http://bdk.hnxiangtu.top

@functools.lru_cache(maxsize=None)
来源：http://yju.yuxming.cn

[U21] Py：自定义上下文管理器
来源：http://uhl.bjfxy.top

@contextlib.contextmanager
来源：http://fnj.c1oappe.top

[U22] Py：矩阵转置
来源：http://amo.hysaishi.cn

list(zip(*m))
来源：http://ffv.zycfv.cn

[U23] Py：分块读取大文件
来源：http://ljw.fanxiaobao.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wcd.9152youxi.cn

[U24] Py：路径操作
来源：http://ucr.quarkkingdee.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mur.zhaomingkeji.xyz

[U25] Py：CSV 按字典读
来源：http://tsz.52xcode.cn

csv.DictReader(f)
来源：http://cqm.zycfv.cn

[U26] Py：并发下载
来源：http://mqy.xylfe.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ala.316326.xyz

[U27] Py：异步 HTTP
来源：http://sfm.wangshuangyany.cn

aiohttp.ClientSession() 配合 async with
来源：http://vdt.guowangkeji.top

[U28] Py：类型别名
来源：http://pjb.nanxuanxn.top

UserId = int
来源：http://kmq.jianghu66.top

[U29] Py：属性校验
来源：http://xce.hywenlv.cn

@property 与 @x.setter 配合
来源：http://kkk.gogol.net.cn

[U30] Py：数据类
来源：http://tdo.cheryme.top

@dataclass(slots=True)
来源：http://run.kuanghao11.cn

[U31] Py：单测
来源：http://doo.sufxvd.cn

python -m pytest -q
来源：http://yrz.chenjidiqi.icu

[U32] Py：代码格式化
来源：http://lue.sysykeji.top

ruff format . && ruff check --fix .
来源：http://vjz.ivvv.top

[U33] Py：打包发布
来源：http://qob.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://ygs.yanxiufei.cn

[U34] Py：判断编码
来源：http://yog.yueranfly.top

chardet.detect(raw)
来源：http://qyq.guannengcc.top

[U35] Py：发送邮件
来源：http://lwa.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vlu.tian-w.cn

[U36] Py：定时任务
来源：http://xif.aibaodan.cn

schedule.every(10).minutes.do(job)
来源：http://rlm.jlsjyb.cn

[U37] Py：读写 Excel
来源：http://wdf.tarul.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dfa.hcnkem.com

[U38] Py：获取脚本所在目录
来源：http://hkt.feifeiyinyue.top

Path(__file__).resolve().parent
来源：http://jpr.guowangkeji.top

[U39] Py：判断是否在交互环境
来源：http://ukq.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://hxw.shzxlz.cn

[U40] Py：打印到标准错误
来源：http://nha.xuetiantiany.cn

print("err", file=sys.stderr)
来源：http://spl.xziqi.cn

[U41] PHP：初始化 Composer 项目
来源：http://eiv.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sph.sjlbkw.cn

[U42] PHP：PSR-4 自动加载
来源：http://rfo.zhixingplan.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wtz.jyoumei.cn

[U43] PHP：声明命名空间
来源：http://loo.gotoacloud.top

namespace App\Http;
来源：http://tdp.wangshuangyany.cn

[U44] PHP：开启严格类型
来源：http://kai.bjfxy.top

declare(strict_types=1);
来源：http://bbz.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://ska.cucudq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zqi.sweek.top

[U46] PHP：可空类型
来源：http://mru.andypj.xyz

?string $name = null
来源：http://sks.aibaodan.cn

[U47] PHP：联合类型
来源：http://qir.snrcjt.cn

int|string $id
来源：http://myg.yongpay.top

[U48] PHP：纯枚举
来源：http://uez.wangdashe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kii.jianghu66.top

[U49] PHP：只读属性
来源：http://fuh.yuxming.cn

public readonly string $name
来源：http://vsp.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://pfa.yangfankeji.com

public function __construct(private int $id) {}
来源：http://fpb.jlsjyb.cn

[U51] PHP：数组解构
来源：http://spw.zdqjudy.top

[$a, $b] = $arr;
来源：http://aiw.jqgufenzy.top

[U52] PHP：箭头函数
来源：http://oiz.fanxiaobao.xyz

$double = fn($x) => $x * 2;
来源：http://gul.gzhubu.top

[U53] PHP：空合并运算符
来源：http://fru.vqdsnc.cn

$v = $a ?? $b ?? "default";
来源：http://dvw.sysykeji.top

[U54] PHP：空安全调用
来源：http://jjc.jinyuanbaomall.cn

$obj?->method()
来源：http://div.cashguo.top

[U55] PHP：match 表达式
来源：http://lsi.yangfankeji.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rvr.cashguo.top

[U56] PHP：命名参数
来源：http://xbc.snrcjt.cn

f(a: 1, b: 2)
来源：http://koe.jinghuilouyu.cn

[U57] PHP：字符串插值
来源：http://hcd.cucudq.cn

"值: {$a}"
来源：http://tzi.nanxinkj.top

[U58] PHP：数组三件套
来源：http://xws.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wpc.yonumen.top

[U59] PHP：自定义排序
来源：http://dat.guowangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://guk.shanyushiyangtech.top

[U60] PHP：JSON 编解码
来源：http://kpi.52xcode.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vab.jinqigfzy.top

[U61] PHP：正则
来源：http://uml.wangdashe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://skz.sufxvd.cn

[U62] PHP：日期对象
来源：http://elz.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hec.gzhubu.top

[U63] PHP：文件读写
来源：http://jns.zhengqikj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xhq.svipenyu.cn

[U64] PHP：目录遍历
来源：http://jpc.guannengcc.top

glob("dir/*.php");  scandir("dir");
来源：http://pfz.jyoumei.cn

[U65] PHP：会话
来源：http://cbi.vqdsnc.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gjq.sxryk.cn

[U66] PHP：设置 Cookie
来源：http://xxz.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yrj.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://jqp.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kpz.ehwqpu.com

[U68] PHP：PDO 连接
来源：http://rej.chenjidiqi.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lsz.tarul.cn

[U69] PHP：PDO 预处理
来源：http://eng.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://crj.gzhubu.top

[U70] PHP：PDO 事务
来源：http://sxs.fzhhl.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hdf.feifeiyinyue.top

[U71] PHP：抛出异常
来源：http://edg.jqgufenzy.top

throw new RuntimeException("失败", 500);
来源：http://vbb.tarul.cn

[U72] PHP：写错误日志
来源：http://vvo.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://wui.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://xph.ywan-chungtsiang.top

parse_ini_file("config.ini", true)
来源：http://jxr.yanxiufei.cn

[U74] PHP：读取环境变量
来源：http://rmh.shangyingyoupin.top

getenv("APP_ENV") ?: "production"
来源：http://hkj.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://tlb.dashuyun.cn

composer require psr/container
来源：http://hwr.epnwcf.com

[U76] PHP：简单路由
来源：http://zgr.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yit.xylfe.cn

[U77] PHP：模板渲染
来源：http://kiq.zdbjq.cn

composer require twig/twig
来源：http://raw.guowangkeji.top

[U78] PHP：单元测试
来源：http://dtf.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://oxq.xylfe.cn

[U79] PHP：静态分析
来源：http://bqp.gaohongyu789.top

composer require --dev phpstan/phpstan
来源：http://mvj.epnwcf.com

[U80] PHP：代码规范修复
来源：http://snp.snrcjt.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zvb.hammf.cn

[U81] JS：初始化项目
来源：http://lba.ivvv.top

npm init -y;  npm i express
来源：http://jog.fktsv.cn

[U82] JS：package.json 脚本
来源：http://afr.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hwp.9152youxi.cn

[U83] JS：ES Module 导入导出
来源：http://uuj.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cvo.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://int.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gtc.zhixingplan.top

[U85] JS：可选链
来源：http://lkn.jqgufenzy.top

a?.b?.c
来源：http://eyu.svipenyu.cn

[U86] JS：空值合并
来源：http://tke.ydzc1.top

a ?? b
来源：http://pfi.shzxlz.cn

[U87] JS：解构默认值
来源：http://xco.xingfuxueyuan.xyz

const { a = 1, b = 2 } = obj;
来源：http://vnu.daxiang520.top

[U88] JS：对象展开合并
来源：http://btv.nanxuanxn.top

{ ...a, ...b }
来源：http://bsc.aibaodan.cn

[U89] JS：数组去重
来源：http://klp.birdmap.top

[...new Set(arr)]
来源：http://jte.hesvh.cn

[U90] JS：数字数组排序
来源：http://qcp.dashuyun.cn

[...arr].sort((a, b) => a - b)
来源：http://fhc.svipenyu.cn

[U91] JS：对象键值遍历
来源：http://pox.hcnkem.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ism.fanxiaobao.xyz

[U92] JS：深拷贝
来源：http://efe.bjfxy.top

structuredClone(obj)
来源：http://vuw.vqdsnc.cn

[U93] JS：模板字符串
来源：http://uut.svipenyu.cn

`共 ${n} 条`
来源：http://rid.redwolf501.top

[U94] JS：箭头函数
来源：http://nxj.snrcjt.cn

const double = x => x * 2;
来源：http://pbj.hammf.cn

[U95] JS：Promise 包装
来源：http://gsg.zhongyouzk.top

new Promise((resolve, reject) => {})
来源：http://znz.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://wvx.9152youxi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qzv.ppjwa.cn

[U97] JS：并发请求
来源：http://ral.dianchejie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ptt.nanxinkj.top

[U98] JS：fetch 带 JSON
来源：http://lzs.shanyushiyangtech.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eyr.tarul.cn

[U99] JS：事件监听
来源：http://pza.wangdashe.top

el.addEventListener("click", e => {})
来源：http://wyu.hywenlv.cn

[U100] JS：DOM 查询
来源：http://tcr.9152youxi.cn

document.querySelector(".item")
来源：http://zsg.vqdsnc.cn

[U101] JS：classList 操作
来源：http://rmy.fktsv.cn

el.classList.toggle("active")
来源：http://vjc.aibaodan.cn

[U102] JS：本地存储
来源：http://hcz.smart0.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://icl.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://ygt.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sqc.bjfxy.top

[U104] JS：防抖
来源：http://knn.jinqigufen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://osc.wangdashe.top

[U105] JS：节流
来源：http://pze.zhixingplan.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wgc.smart0.xyz

[U106] JS：日期格式化
来源：http://wlw.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aeq.snrcjt.cn

[U107] JS：数字千分位
来源：http://obr.redwolf501.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gqe.fktsv.cn

[U108] JS：随机整数
来源：http://mzv.shzxlz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mue.yfazqb.com

[U109] JS：数组分组
来源：http://fcj.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://ebo.gaohongyu789.top

[U110] JS：数组分块
来源：http://kqk.0kj1m.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rhj.yfazqb.com

[U111] JS：对象转 Map
来源：http://ptv.sweek.top

new Map(Object.entries(obj))
来源：http://odh.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://wnn.kuanghao11.cn

"7".padStart(3, "0")
来源：http://gcz.cqqwz.cn

[U113] JS：正则替换全部
来源：http://mez.fzhhl.top

s.replaceAll("a", "b")
来源：http://trn.sysykeji.top

[U114] JS：JSON 深比较
来源：http://zkq.redwolf501.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bbu.tian-w.cn

[U115] JS：生成 UUID
来源：http://gfi.nanxinkj.top

crypto.randomUUID()
来源：http://sef.hnxiangtu.top

[U116] JS：类型检查（JSDoc）
来源：http://iqj.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://kuq.xziqi.cn

[U117] JS：单元测试
来源：http://ztl.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://qwz.jyoumei.cn

[U118] JS：开发服务器
来源：http://wty.cashguo.top

npm i -D vite;  npx vite
来源：http://ifl.fzhhl.top

[U119] JS：生产构建
来源：http://bzs.zhijiandao.cn

npx vite build
来源：http://eif.9152youxi.cn

[U120] JS：读取环境变量（Vite）
来源：http://irn.yangfankeji.com

import.meta.env.VITE_API_URL
来源：http://wli.gaohongyu789.top

================================================================================
来源：http://grn.ydzc1.top

统计汇总
来源：http://coa.dianchejie.cn

================================================================================
来源：http://opy.ydjk.org.cn

按语言统计（条）：
来源：http://qfu.wangdashe.top

Python ......... 252
来源：http://jpw.sufxvd.cn

PHP ............ 252
来源：http://zmy.zhixingplan.top

JavaScript ..... 252
来源：http://oti.yuxming.cn

TypeScript ..... 212
来源：http://mjx.hfpthk.cn

Java ........... 212
来源：http://dlg.jyoumei.cn

Go ............. 212
来源：http://tji.tianlin.xyz

Ruby ........... 212
来源：http://ufg.hywenlv.cn

C# ............. 212
来源：http://kub.ywan-chungtsiang.top

C .............. 30
来源：http://bii.yj20258888.top

C++ ............ 30
来源：http://ogs.zdbjq.cn

SQL ............ 90
来源：http://vqj.sweek.top

Bash ........... 80
来源：http://zcq.yj20258.top

Kotlin ......... 15
来源：http://lra.zhiwuduotai.top

Swift .......... 15
来源：http://euh.ydzc1.top

Lua ............ 10
来源：http://zkm.cdnleiting.top

Perl ........... 10
来源：http://laz.aizwys.cn

Scala .......... 10
来源：http://wen.iojbl.cn

------------------------------------
来源：http://svd.ywan-chungtsiang.top

合计 ........... 2106 条
来源：http://rqy.aibaodan.cn

按章节统计：
来源：http://std.andypj.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jhk.c1oappe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zup.xinyue.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vmk.yuanzhike.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uxn.yvedp.cn


<!-- 参考信息 -->