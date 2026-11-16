代发 wailian999

[T37] Lua：字符串拼接
来源：http://bph.nanxinkj.top

"a" .. "b"
来源：http://wyg.jinghuilouyu.cn

[T38] Lua：条件
来源：http://sms.fehbvm.com

if x > 0 then print("正") end
来源：http://fed.sjlbkw.cn

[T39] Lua：模式匹配
来源：http://kvv.jinqigfzy.top

string.find(s, "%d+")
来源：http://tvc.nanxuanxn.top

[T40] Lua：元表
来源：http://qzw.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://krs.yonumen.top

[T41] Perl：Hello World
来源：http://ccp.xuetiantiany.cn

print "Hello\n";
来源：http://udw.zhongyouzk.top

[T42] Perl：变量类型
来源：http://emi.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://srr.sxryk.cn

[T43] Perl：字符串插值
来源：http://xzv.chenlongwang.top

"值: $a"
来源：http://zas.dashuyun.cn

[T44] Perl：条件
来源：http://wig.cashguo.top

if ($a > 0) { print "正"; }
来源：http://sxz.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://mkq.zhongyouzk.top

for my $x (@arr) { print $x; }
来源：http://ofp.yj20258888.top

[T46] Perl：哈希操作
来源：http://jlj.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jir.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://zxh.yuanzhike.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tvh.hesvh.cn

[T48] Perl：正则替换
来源：http://zco.shanyushiyangkeji.top

$s =~ s/old/new/g;
来源：http://jqi.wangshuangyany.cn

[T49] Perl：函数
来源：http://ohm.sweek.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fte.vehdjk.com

[T50] Perl：逐行读文件
来源：http://bvj.pycfn.com

open my $fh, "<", "a.txt" or die $!;
来源：http://uqv.uphjek.com

while (my $line = <$fh>) { print $line; }
来源：http://hja.zhijiandao.cn

[T51] Scala：Hello World
来源：http://pxn.xuetiantiany.cn

println("Hello")
来源：http://ebv.xziqi.cn

[T52] Scala：变量
来源：http://nai.svipenyu.cn

val a = 1;  var b = 2
来源：http://qqt.fktsv.cn

[T53] Scala：字符串插值
来源：http://lxk.chenjidiqi.icu

s"值: $b"
来源：http://wwf.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://uwv.jqgufenzy.top

List(1, 2, 3).map(_ * 2)
来源：http://jiz.xuetiantiany.cn

[T55] Scala：集合过滤
来源：http://goa.andypj.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://hbv.uphjek.com

[T56] Scala：样例类
来源：http://kxg.ydjk.org.cn

case class User(name: String, age: Int)
来源：http://osp.zhixingplan.top

[T57] Scala：模式匹配
来源：http://wse.sxryk.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qte.fehbvm.com

[T58] Scala：函数定义
来源：http://noz.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://mhc.sxryk.cn

[T59] Scala：循环
来源：http://qyc.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://mqs.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://gyt.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vpt.tian-w.cn

================================================================================
来源：http://bbz.snrcjt.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ygk.jyoumei.cn

================================================================================
来源：http://qco.kuanghao11.cn

[U01] Py：创建虚拟环境
来源：http://xpj.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://aui.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://fvq.svipenyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cmx.shanyushiyangtech.top

[U03] Py：加载 .env 配置
来源：http://paz.iojbl.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hdq.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://qbs.ehwqpu.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hbx.fengsongda.top

[U05] Py：列表去重且保序
来源：http://nvx.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://aum.9152youxi.cn

[U06] Py：合并两个字典
来源：http://wdt.pengpengdd.cyou

{**a, **b}
来源：http://evt.birdmap.top

[U07] Py：反转字典键值
来源：http://qhc.iojbl.cn

{v: k for k, v in d.items()}
来源：http://osk.sysykeji.top

[U08] Py：展平二维列表
来源：http://qwu.yuxming.cn

[y for x in nested for y in x]
来源：http://grt.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://btb.fengsongda.top

max(d, key=d.get)
来源：http://kjs.nwbrower.top

[U10] Py：按值排序字典
来源：http://qgv.jinqigufen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hwb.316326.xyz

[U11] Py：生成器表达式
来源：http://psc.yj20258888.top

(x * 2 for x in arr)
来源：http://but.xinyue.icu

[U12] Py：取出现最多的 3 个元素
来源：http://act.meibo888.top

Counter(arr).most_common(3)
来源：http://pcb.c1oappe.top

[U13] Py：固定长度队列
来源：http://iay.sufxvd.cn

deque(maxlen=10)
来源：http://wdq.fzhhl.top

[U14] Py：分组收集到列表
来源：http://fuj.ehwqpu.com

defaultdict(list)
来源：http://pva.sjlbkw.cn

[U15] Py：高精度计时
来源：http://doi.birdmap.top

t = time.perf_counter()
来源：http://lky.fanxiaobao.xyz

[U16] Py：命令行参数解析
来源：http://rub.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gws.ywan-chungtsiang.top

[U17] Py：初始化日志
来源：http://mgw.quarkkingdee.top

logging.basicConfig(level=logging.INFO)
来源：http://yck.svipenyu.cn

[U18] Py：预编译正则
来源：http://kyp.sxryk.cn

pat = re.compile(r"\d+")
来源：http://asl.tarul.cn

[U19] Py：正则替换带回调
来源：http://jgs.yueranfly.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jui.xziqi.cn

[U20] Py：缓存函数结果
来源：http://lkq.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://saf.chenjidiqi.icu

[U21] Py：自定义上下文管理器
来源：http://rrh.havefunace.top

@contextlib.contextmanager
来源：http://wvr.cashguo.top

[U22] Py：矩阵转置
来源：http://uwz.aizwys.cn

list(zip(*m))
来源：http://dse.xingfuxueyuan.xyz

[U23] Py：分块读取大文件
来源：http://asi.birdmap.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yzi.zdqjudy.top

[U24] Py：路径操作
来源：http://dof.epnwcf.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pca.zhiwuduotai.top

[U25] Py：CSV 按字典读
来源：http://qji.yongpay.top

csv.DictReader(f)
来源：http://mru.hnxiangtu.top

[U26] Py：并发下载
来源：http://dfb.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://okw.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://qyg.jlsjyb.cn

aiohttp.ClientSession() 配合 async with
来源：http://blh.pycfn.com

[U28] Py：类型别名
来源：http://axg.jinqigufen.top

UserId = int
来源：http://nep.snrcjt.cn

[U29] Py：属性校验
来源：http://aho.hfpthk.cn

@property 与 @x.setter 配合
来源：http://mze.chenlongwang.top

[U30] Py：数据类
来源：http://rmo.smart0.xyz

@dataclass(slots=True)
来源：http://eqc.pengpengdd.cyou

[U31] Py：单测
来源：http://tea.andypj.xyz

python -m pytest -q
来源：http://hha.jinqigfzy.top

[U32] Py：代码格式化
来源：http://htp.chenzaomai.com

ruff format . && ruff check --fix .
来源：http://bqa.kuanghao11.cn

[U33] Py：打包发布
来源：http://cmg.chenlongwang.top

python -m build  （依赖 pyproject.toml）
来源：http://tnn.zycfv.cn

[U34] Py：判断编码
来源：http://qnv.tarul.cn

chardet.detect(raw)
来源：http://fiw.jiagoushi.top

[U35] Py：发送邮件
来源：http://nwq.hcnkem.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pia.dianchejie.cn

[U36] Py：定时任务
来源：http://opi.zhiwuduotai.top

schedule.every(10).minutes.do(job)
来源：http://cbm.jqgfzy.top

[U37] Py：读写 Excel
来源：http://fjs.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://agy.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://lkd.vqdsnc.cn

Path(__file__).resolve().parent
来源：http://imr.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://ltw.dianchejie.cn

sys.stdout.isatty()
来源：http://ghc.zhiwuduotai.top

[U40] Py：打印到标准错误
来源：http://qkv.jqgfzy.top

print("err", file=sys.stderr)
来源：http://oip.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://bvm.havefunace.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qoq.ydzc1.top

[U42] PHP：PSR-4 自动加载
来源：http://enb.snrcjt.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gae.daria6918.cn

[U43] PHP：声明命名空间
来源：http://xjs.hysaishi.cn

namespace App\Http;
来源：http://mcx.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://cfg.hywenlv.cn

declare(strict_types=1);
来源：http://kjh.andypj.xyz

[U45] PHP：类型声明与返回类型
来源：http://arw.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gpu.wangshuangyany.cn

[U46] PHP：可空类型
来源：http://qwz.pycfn.com

?string $name = null
来源：http://pvb.hywenlv.cn

[U47] PHP：联合类型
来源：http://uen.cdnleiting.top

int|string $id
来源：http://ixd.ppjwa.cn

[U48] PHP：纯枚举
来源：http://brz.yangfankeji.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qgm.smart0.xyz

[U49] PHP：只读属性
来源：http://lzs.bbcook.cn

public readonly string $name
来源：http://hmo.sweek.top

[U50] PHP：构造器属性提升
来源：http://xvh.hnxiangtu.top

public function __construct(private int $id) {}
来源：http://dmd.jyoumei.cn

[U51] PHP：数组解构
来源：http://zmo.hywenlv.cn

[$a, $b] = $arr;
来源：http://mnk.shangyingyoupin.top

[U52] PHP：箭头函数
来源：http://utm.hcnkem.com

$double = fn($x) => $x * 2;
来源：http://iet.shangyingyoupin.top

[U53] PHP：空合并运算符
来源：http://udr.cqqwz.cn

$v = $a ?? $b ?? "default";
来源：http://mkq.pycfn.com

[U54] PHP：空安全调用
来源：http://seh.vehdjk.com

$obj?->method()
来源：http://vmn.cdnleiting.top

[U55] PHP：match 表达式
来源：http://mef.zdqjudy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qri.cheryme.top

[U56] PHP：命名参数
来源：http://oyp.dashuyun.cn

f(a: 1, b: 2)
来源：http://noz.daria6918.cn

[U57] PHP：字符串插值
来源：http://tyx.zhongyouzk.top

"值: {$a}"
来源：http://jsf.xziqi.cn

[U58] PHP：数组三件套
来源：http://wsq.shanyushiyangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://epv.iojbl.cn

[U59] PHP：自定义排序
来源：http://lzg.tanke756.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lzj.tianlin.xyz

[U60] PHP：JSON 编解码
来源：http://ugd.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hjo.xingfuxueyuan.xyz

[U61] PHP：正则
来源：http://swx.jianghu66.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gmw.yuxming.cn

[U62] PHP：日期对象
来源：http://zoe.jlsjyb.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://taz.hysaishi.cn

[U63] PHP：文件读写
来源：http://hmq.epnwcf.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eba.sjlbkw.cn

[U64] PHP：目录遍历
来源：http://lug.sysykeji.top

glob("dir/*.php");  scandir("dir");
来源：http://gsv.tarul.cn

[U65] PHP：会话
来源：http://kja.guowangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fkv.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://pzl.shanyushiyangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gsb.sweek.top

[U67] PHP：处理文件上传
来源：http://jyl.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xus.gaohongyu789.top

[U68] PHP：PDO 连接
来源：http://wuj.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jwz.ydzc1.top

[U69] PHP：PDO 预处理
来源：http://xcr.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pvp.yonumen.top

[U70] PHP：PDO 事务
来源：http://hhd.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ezi.cdnleiting.top

[U71] PHP：抛出异常
来源：http://sti.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://xuq.ehwqpu.com

[U72] PHP：写错误日志
来源：http://gap.ctjpmb.com

error_log("失败: " . $e->getMessage());
来源：http://tlx.hnqzz.top

[U73] PHP：读取 ini 配置
来源：http://qug.yangfankeji.com

parse_ini_file("config.ini", true)
来源：http://lsv.havefunace.top

[U74] PHP：读取环境变量
来源：http://poa.zdbjq.cn

getenv("APP_ENV") ?: "production"
来源：http://nry.yueranfly.top

[U75] PHP：依赖注入
来源：http://xdg.nanxinkj.top

composer require psr/container
来源：http://vta.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://xpe.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://obu.nwbrower.top

[U77] PHP：模板渲染
来源：http://otd.fengsongda.top

composer require twig/twig
来源：http://aza.jinghuilouyu.cn

[U78] PHP：单元测试
来源：http://ogs.jyoumei.cn

composer require --dev phpunit/phpunit
来源：http://mcs.hesvh.cn

[U79] PHP：静态分析
来源：http://bzl.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://zpp.iojbl.cn

[U80] PHP：代码规范修复
来源：http://pkh.quarkkingdee.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rbu.bbcook.cn

[U81] JS：初始化项目
来源：http://spo.feifeiyinyue.top

npm init -y;  npm i express
来源：http://tie.cdnleiting.top

[U82] JS：package.json 脚本
来源：http://foc.sweek.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gip.mhx1999.top

[U83] JS：ES Module 导入导出
来源：http://zyt.haohaochexian.top

export const a = 1;  import { a } from "./m.js";
来源：http://cbg.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://faq.cqqwz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mzp.yongpay.top

[U85] JS：可选链
来源：http://ohy.ivvv.top

a?.b?.c
来源：http://jml.fzhhl.top

[U86] JS：空值合并
来源：http://tix.kuanghao11.cn

a ?? b
来源：http://oyu.xuetiantiany.cn

[U87] JS：解构默认值
来源：http://viz.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://dwy.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://qww.ivvv.top

{ ...a, ...b }
来源：http://hru.sxryk.cn

[U89] JS：数组去重
来源：http://eds.dashuyun.cn

[...new Set(arr)]
来源：http://lid.ybcxt.top

[U90] JS：数字数组排序
来源：http://bpd.tarul.cn

[...arr].sort((a, b) => a - b)
来源：http://sjb.nanxinkj.top

[U91] JS：对象键值遍历
来源：http://gdy.daxiang520.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zmb.gogol.net.cn

[U92] JS：深拷贝
来源：http://oxc.xylfe.cn

structuredClone(obj)
来源：http://yzt.tarul.cn

[U93] JS：模板字符串
来源：http://xxa.jinqigfzy.top

`共 ${n} 条`
来源：http://row.havefunace.top

[U94] JS：箭头函数
来源：http://fjs.cheryme.top

const double = x => x * 2;
来源：http://xdj.fanxiaobao.xyz

[U95] JS：Promise 包装
来源：http://oaf.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://kzh.svipenyu.cn

[U96] JS：async/await 与异常
来源：http://sfa.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gqi.redwolf501.top

[U97] JS：并发请求
来源：http://jfr.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://sra.hnqzz.top

[U98] JS：fetch 带 JSON
来源：http://tbt.fzhhl.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qlb.shanyushiyangtech.top

[U99] JS：事件监听
来源：http://obo.vehdjk.com

el.addEventListener("click", e => {})
来源：http://ylk.ivvv.top

[U100] JS：DOM 查询
来源：http://dga.snrcjt.cn

document.querySelector(".item")
来源：http://wbd.shangyingyoupin.top

[U101] JS：classList 操作
来源：http://nlg.yongpay.top

el.classList.toggle("active")
来源：http://skj.birdmap.top

[U102] JS：本地存储
来源：http://swl.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://azk.cdnleiting.top

[U103] JS：定时器
来源：http://ccj.guannengcc.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sdr.iojbl.cn

[U104] JS：防抖
来源：http://cfn.hysaishi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fmj.shzxlz.cn

[U105] JS：节流
来源：http://zqo.0kj1m.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://llp.kuanghao11.cn

[U106] JS：日期格式化
来源：http://vbc.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://llx.quarkkingdee.top

[U107] JS：数字千分位
来源：http://dcs.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ahz.ctjpmb.com

[U108] JS：随机整数
来源：http://qmu.yj20258888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jnv.ppjwa.cn

[U109] JS：数组分组
来源：http://lau.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://feu.xylfe.cn

[U110] JS：数组分块
来源：http://lvm.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dgb.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://urc.cqqwz.cn

new Map(Object.entries(obj))
来源：http://yud.yj20258888.top

[U112] JS：字符串补位
来源：http://jyf.nanxuanxn.top

"7".padStart(3, "0")
来源：http://aux.havefunace.top

[U113] JS：正则替换全部
来源：http://nvf.sweek.top

s.replaceAll("a", "b")
来源：http://czh.316326.xyz

[U114] JS：JSON 深比较
来源：http://eqs.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vmy.gzhubu.top

[U115] JS：生成 UUID
来源：http://lcp.yuanzhike.top

crypto.randomUUID()
来源：http://hia.chenzaomai.com

[U116] JS：类型检查（JSDoc）
来源：http://daa.hnxiangtu.top

/** @param {string} name */ function f(name) {}
来源：http://uzp.mhx1999.top

[U117] JS：单元测试
来源：http://ggy.jiagoushi.top

npm i -D vitest;  npx vitest
来源：http://kbz.uphjek.com

[U118] JS：开发服务器
来源：http://jis.cashguo.top

npm i -D vite;  npx vite
来源：http://oqy.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://tgp.hysaishi.cn

npx vite build
来源：http://bba.zhongyouzk.top

[U120] JS：读取环境变量（Vite）
来源：http://kam.snrcjt.cn

import.meta.env.VITE_API_URL
来源：http://vdd.haohaochexian.top

================================================================================
来源：http://tin.jinghuilouyu.cn

统计汇总
来源：http://uyn.tanke756.top

================================================================================
来源：http://rln.nanxuanxn.top

按语言统计（条）：
来源：http://acg.shangyingyoupin.top

Python ......... 252
来源：http://zak.epnwcf.com

PHP ............ 252
来源：http://lrw.jinqigufen.top

JavaScript ..... 252
来源：http://iyb.hammf.cn

TypeScript ..... 212
来源：http://ryc.xziqi.cn


<!-- 参考信息 -->