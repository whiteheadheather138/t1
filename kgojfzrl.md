代发 wailian999

[T49] Perl：函数
来源：http://qoq.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://luh.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://cdt.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ebc.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://ehc.dashuyun.cn

[T51] Scala：Hello World
来源：http://gai.shanyushiyangtech.top

println("Hello")
来源：http://exv.chenzaomai.com

[T52] Scala：变量
来源：http://ohx.tarul.cn

val a = 1;  var b = 2
来源：http://nhq.nanxuanxn.top

[T53] Scala：字符串插值
来源：http://npm.dashuyun.cn

s"值: $b"
来源：http://kmu.yfazqb.com

[T54] Scala：集合映射
来源：http://mid.cashguo.top

List(1, 2, 3).map(_ * 2)
来源：http://mhb.jinyuanbaomall.cn

[T55] Scala：集合过滤
来源：http://teu.wangshuangyany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://otz.uphjek.com

[T56] Scala：样例类
来源：http://wjo.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://fgg.yvedp.cn

[T57] Scala：模式匹配
来源：http://bly.sysykeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hok.gotoacloud.top

[T58] Scala：函数定义
来源：http://vnb.andypj.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://pia.gogol.net.cn

[T59] Scala：循环
来源：http://fnu.wangdashe.top

for (i <- 1 to 10) println(i)
来源：http://mrz.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://uud.zhaomingkeji.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://usg.ivvv.top

================================================================================
来源：http://wth.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xnp.chenjidiqi.icu

================================================================================
来源：http://fih.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://qke.nwbrower.top

python -m venv .venv && source .venv/bin/activate
来源：http://owk.xylfe.cn

[U02] Py：导出 / 安装依赖
来源：http://bhw.aizwys.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gae.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://fbj.gzhubu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ayk.jiagoushi.top

[U04] Py：变量调试打印
来源：http://bya.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lvs.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://xin.zhiwuduotai.top

list(dict.fromkeys(arr))
来源：http://iib.jianghu66.top

[U06] Py：合并两个字典
来源：http://raq.iojbl.cn

{**a, **b}
来源：http://sjl.sysykeji.top

[U07] Py：反转字典键值
来源：http://eil.xinyue.icu

{v: k for k, v in d.items()}
来源：http://cyo.hysaishi.cn

[U08] Py：展平二维列表
来源：http://qkp.iojbl.cn

[y for x in nested for y in x]
来源：http://vhe.yangfankeji.com

[U09] Py：字典取最大值的键
来源：http://xto.shzxlz.cn

max(d, key=d.get)
来源：http://ecj.hcnkem.com

[U10] Py：按值排序字典
来源：http://rre.52xcode.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ciz.guannengcc.top

[U11] Py：生成器表达式
来源：http://rxr.hfpthk.cn

(x * 2 for x in arr)
来源：http://xmw.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://xsk.ybcxt.top

Counter(arr).most_common(3)
来源：http://bcv.hysaishi.cn

[U13] Py：固定长度队列
来源：http://nay.smart0.xyz

deque(maxlen=10)
来源：http://pgs.havefunace.top

[U14] Py：分组收集到列表
来源：http://pdu.hcnkem.com

defaultdict(list)
来源：http://fle.ivvv.top

[U15] Py：高精度计时
来源：http://xkq.hnxiangtu.top

t = time.perf_counter()
来源：http://hcu.tarul.cn

[U16] Py：命令行参数解析
来源：http://mnu.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dsi.cucudq.cn

[U17] Py：初始化日志
来源：http://tsl.0kj1m.cn

logging.basicConfig(level=logging.INFO)
来源：http://odt.jiagoushi.top

[U18] Py：预编译正则
来源：http://fis.hcnkem.com

pat = re.compile(r"\d+")
来源：http://qri.jiagoushi.top

[U19] Py：正则替换带回调
来源：http://hxb.hfpthk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ovb.hnqzz.top

[U20] Py：缓存函数结果
来源：http://eit.zhaomingkeji.xyz

@functools.lru_cache(maxsize=None)
来源：http://tov.xuetiantiany.cn

[U21] Py：自定义上下文管理器
来源：http://azn.hfpthk.cn

@contextlib.contextmanager
来源：http://gtr.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://cyv.gaohongyu789.top

list(zip(*m))
来源：http://kho.vqdsnc.cn

[U23] Py：分块读取大文件
来源：http://yte.shuidangran.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qjv.ydjk.org.cn

[U24] Py：路径操作
来源：http://vnl.jlsjyb.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cnf.cashguo.top

[U25] Py：CSV 按字典读
来源：http://dqg.wangdashe.top

csv.DictReader(f)
来源：http://hhb.sjlbkw.cn

[U26] Py：并发下载
来源：http://gyz.guannengcc.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tiv.ybcxt.top

[U27] Py：异步 HTTP
来源：http://ewr.hnqzz.top

aiohttp.ClientSession() 配合 async with
来源：http://jlc.nwbrower.top

[U28] Py：类型别名
来源：http://frx.fengsongda.top

UserId = int
来源：http://sli.hfpthk.cn

[U29] Py：属性校验
来源：http://lqj.mhx1999.top

@property 与 @x.setter 配合
来源：http://kwg.xuetiantiany.cn

[U30] Py：数据类
来源：http://lec.0kj1m.cn

@dataclass(slots=True)
来源：http://cuz.jinqigfzy.top

[U31] Py：单测
来源：http://hli.pycfn.com

python -m pytest -q
来源：http://hts.andypj.xyz

[U32] Py：代码格式化
来源：http://tsr.mhx1999.top

ruff format . && ruff check --fix .
来源：http://jgk.yonumen.top

[U33] Py：打包发布
来源：http://pds.aibaodan.cn

python -m build  （依赖 pyproject.toml）
来源：http://som.jqgfzy.top

[U34] Py：判断编码
来源：http://qzz.nanxuanxn.top

chardet.detect(raw)
来源：http://hxp.cqqwz.cn

[U35] Py：发送邮件
来源：http://gok.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tif.zhoulong.xyz

[U36] Py：定时任务
来源：http://qpo.birdmap.top

schedule.every(10).minutes.do(job)
来源：http://gdd.yonumen.top

[U37] Py：读写 Excel
来源：http://gfk.xylfe.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wju.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://kqe.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://bmx.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://bsz.yvedp.cn

sys.stdout.isatty()
来源：http://jyn.bjfxy.top

[U40] Py：打印到标准错误
来源：http://nav.yvedp.cn

print("err", file=sys.stderr)
来源：http://gqp.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://bmm.chenjidiqi.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://vax.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://goq.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gut.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://cpz.jqgfzy.top

namespace App\Http;
来源：http://aya.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://brp.shanyushiyangtech.top

declare(strict_types=1);
来源：http://mpe.52xcode.cn

[U45] PHP：类型声明与返回类型
来源：http://qby.vqdsnc.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hea.bjfxy.top

[U46] PHP：可空类型
来源：http://koo.sysykeji.top

?string $name = null
来源：http://agq.redwolf501.top

[U47] PHP：联合类型
来源：http://zby.guannengcc.top

int|string $id
来源：http://dtb.shanyushiyangkeji.top

[U48] PHP：纯枚举
来源：http://mnu.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://den.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://kos.ehwqpu.com

public readonly string $name
来源：http://ydg.hfpthk.cn

[U50] PHP：构造器属性提升
来源：http://dnt.c1oappe.top

public function __construct(private int $id) {}
来源：http://wna.xingfuxueyuan.xyz

[U51] PHP：数组解构
来源：http://ebk.shzxlz.cn

[$a, $b] = $arr;
来源：http://zre.bbcook.cn

[U52] PHP：箭头函数
来源：http://gyn.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://wnc.yvedp.cn

[U53] PHP：空合并运算符
来源：http://fqw.zhoulong.xyz

$v = $a ?? $b ?? "default";
来源：http://sls.pycfn.com

[U54] PHP：空安全调用
来源：http://nbh.kuanghao11.cn

$obj?->method()
来源：http://uhm.fehbvm.com

[U55] PHP：match 表达式
来源：http://xia.jqgufenzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vhb.pengpengdd.cyou

[U56] PHP：命名参数
来源：http://sma.birdmap.top

f(a: 1, b: 2)
来源：http://fle.xziqi.cn

[U57] PHP：字符串插值
来源：http://vaj.chenlongwang.top

"值: {$a}"
来源：http://qhh.zhengqikj.top

[U58] PHP：数组三件套
来源：http://qlw.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rul.yj202588.top

[U59] PHP：自定义排序
来源：http://zcp.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zcl.uphjek.com

[U60] PHP：JSON 编解码
来源：http://pho.andypj.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yaa.ybcxt.top

[U61] PHP：正则
来源：http://aem.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lcs.yj202588.top

[U62] PHP：日期对象
来源：http://nnx.hnxiangtu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hrp.snrcjt.cn

[U63] PHP：文件读写
来源：http://jgd.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zau.jinqigufen.top

[U64] PHP：目录遍历
来源：http://mvu.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://ynp.hywenlv.cn

[U65] PHP：会话
来源：http://fxi.sxryk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vxr.ivvv.top

[U66] PHP：设置 Cookie
来源：http://eic.ivvv.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jnx.ivvv.top

[U67] PHP：处理文件上传
来源：http://bhn.nwbrower.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://osl.mhx1999.top

[U68] PHP：PDO 连接
来源：http://uiw.shuidangran.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mwg.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://vuj.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://onh.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://ezy.shuidangran.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pno.ehwqpu.com

[U71] PHP：抛出异常
来源：http://rti.zhaomingkeji.xyz

throw new RuntimeException("失败", 500);
来源：http://qkt.iojbl.cn

[U72] PHP：写错误日志
来源：http://pav.ydzc1.top

error_log("失败: " . $e->getMessage());
来源：http://lpn.zhixingplan.top

[U73] PHP：读取 ini 配置
来源：http://lik.uphjek.com

parse_ini_file("config.ini", true)
来源：http://chg.sufxvd.cn

[U74] PHP：读取环境变量
来源：http://htk.tian-w.cn

getenv("APP_ENV") ?: "production"
来源：http://azy.pycfn.com

[U75] PHP：依赖注入
来源：http://gxq.zhijiandao.cn

composer require psr/container
来源：http://cbj.quarkkingdee.top

[U76] PHP：简单路由
来源：http://flf.snrcjt.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fwm.guannengcc.top

[U77] PHP：模板渲染
来源：http://qcn.jinyuanbaomall.cn

composer require twig/twig
来源：http://lez.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://fhi.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://omi.chenlongwang.top

[U79] PHP：静态分析
来源：http://vfn.fengsongda.top

composer require --dev phpstan/phpstan
来源：http://hbo.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://flw.nanxuanxn.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://adp.tarul.cn

[U81] JS：初始化项目
来源：http://acl.havefunace.top

npm init -y;  npm i express
来源：http://xde.ywan-chungtsiang.top

[U82] JS：package.json 脚本
来源：http://wrs.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nho.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://qgo.jiagoushi.top

export const a = 1;  import { a } from "./m.js";
来源：http://vxo.gzhubu.top

[U84] JS：CommonJS 写法
来源：http://bsp.jlsjyb.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uue.snrcjt.cn

[U85] JS：可选链
来源：http://qxd.shuidangran.top

a?.b?.c
来源：http://otr.hysaishi.cn

[U86] JS：空值合并
来源：http://fwv.tarul.cn

a ?? b
来源：http://hzn.quarkkingdee.top

[U87] JS：解构默认值
来源：http://jhc.sjlbkw.cn

const { a = 1, b = 2 } = obj;
来源：http://gbi.yuanzhike.top

[U88] JS：对象展开合并
来源：http://bbb.svipenyu.cn

{ ...a, ...b }
来源：http://qqv.uphjek.com

[U89] JS：数组去重
来源：http://gaw.gogol.net.cn

[...new Set(arr)]
来源：http://pyc.bjfxy.top

[U90] JS：数字数组排序
来源：http://uap.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://aaq.yuanzhike.top

[U91] JS：对象键值遍历
来源：http://ths.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bpd.tanke756.top

[U92] JS：深拷贝
来源：http://ime.aibaodan.cn

structuredClone(obj)
来源：http://boq.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://mxd.xziqi.cn

`共 ${n} 条`
来源：http://gzg.cheryme.top

[U94] JS：箭头函数
来源：http://hbd.jlsjyb.cn

const double = x => x * 2;
来源：http://ynl.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://emx.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://uno.vehdjk.com

[U96] JS：async/await 与异常
来源：http://sxi.fzhhl.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sve.nwbrower.top

[U97] JS：并发请求
来源：http://hlw.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://qgl.sufxvd.cn

[U98] JS：fetch 带 JSON
来源：http://boh.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fro.daxiang520.top

[U99] JS：事件监听
来源：http://qkp.yuanzhike.top

el.addEventListener("click", e => {})
来源：http://qsq.dianchejie.cn

[U100] JS：DOM 查询
来源：http://yzy.yangfankeji.com

document.querySelector(".item")
来源：http://adj.gzhubu.top

[U101] JS：classList 操作
来源：http://roy.hfpthk.cn

el.classList.toggle("active")
来源：http://emi.jinqigufen.top

[U102] JS：本地存储
来源：http://rla.shangyingyoupin.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gsp.feifeiyinyue.top

[U103] JS：定时器
来源：http://aiv.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jyi.gogol.net.cn

[U104] JS：防抖
来源：http://fqe.gzhubu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kff.smart0.xyz

[U105] JS：节流
来源：http://mye.52xcode.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uip.shangyingyoupin.top

[U106] JS：日期格式化
来源：http://hkg.vqdsnc.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://icd.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://jll.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eks.316326.xyz

[U108] JS：随机整数
来源：http://faq.xinyue.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://isy.zhongyouzk.top

[U109] JS：数组分组
来源：http://dbo.zhiwuduotai.top

Object.groupBy(arr, x => x.type)
来源：http://uxi.aibaodan.cn

[U110] JS：数组分块
来源：http://xyv.316326.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kcm.cdnleiting.top

[U111] JS：对象转 Map
来源：http://cnh.mhx1999.top

new Map(Object.entries(obj))
来源：http://jpz.nwbrower.top

[U112] JS：字符串补位
来源：http://khf.jianghu66.top

"7".padStart(3, "0")
来源：http://mue.yfazqb.com

[U113] JS：正则替换全部
来源：http://xhf.snrcjt.cn

s.replaceAll("a", "b")
来源：http://wfp.havefunace.top

[U114] JS：JSON 深比较
来源：http://gou.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oio.chenjidiqi.icu

[U115] JS：生成 UUID
来源：http://mrq.wangshuangyany.cn

crypto.randomUUID()
来源：http://hxk.yanxiufei.cn

[U116] JS：类型检查（JSDoc）
来源：http://qqy.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://err.birdmap.top

[U117] JS：单元测试
来源：http://sfb.yongpay.top

npm i -D vitest;  npx vitest
来源：http://nfa.shanyushiyangkeji.top

[U118] JS：开发服务器
来源：http://pbc.yuxming.cn

npm i -D vite;  npx vite
来源：http://hfl.vehdjk.com

[U119] JS：生产构建
来源：http://gvw.jinqigufen.top

npx vite build
来源：http://guh.fehbvm.com

[U120] JS：读取环境变量（Vite）
来源：http://got.pycfn.com

import.meta.env.VITE_API_URL
来源：http://myh.yfazqb.com

================================================================================
来源：http://lax.haohaochexian.top

统计汇总
来源：http://ltd.ydjk.org.cn

================================================================================
来源：http://gtz.dianchejie.cn

按语言统计（条）：
来源：http://esj.yvedp.cn

Python ......... 252
来源：http://khr.haohaochexian.top

PHP ............ 252
来源：http://wfg.shuidangran.top

JavaScript ..... 252
来源：http://tse.hywenlv.cn

TypeScript ..... 212
来源：http://ssg.ivvv.top

Java ........... 212
来源：http://goq.fzhhl.top

Go ............. 212
来源：http://ydr.xuetiantiany.cn

Ruby ........... 212
来源：http://fga.zhiwuduotai.top

C# ............. 212
来源：http://nzc.ppjwa.cn

C .............. 30
来源：http://aqa.zhaomingkeji.xyz

C++ ............ 30
来源：http://vlq.zhixingplan.top

SQL ............ 90
来源：http://msd.yvedp.cn

Bash ........... 80
来源：http://mia.guannengcc.top

Kotlin ......... 15
来源：http://dyi.gzhubu.top

Swift .......... 15
来源：http://tmz.fanxiaobao.xyz

Lua ............ 10
来源：http://lnf.svipenyu.cn

Perl ........... 10
来源：http://lwy.jinqigufen.top

Scala .......... 10
来源：http://kmh.hysaishi.cn

------------------------------------
来源：http://tsc.shanyushiyangkeji.top

合计 ........... 2106 条
来源：http://kpm.chenjidiqi.icu

按章节统计：
来源：http://jzj.chenzaomai.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oga.pengpengdd.cyou

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://efq.yongpay.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://drx.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://upk.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zpv.gaohongyu789.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qde.9152youxi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://apk.hcnkem.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wmf.cheryme.top


<!-- 参考信息 -->