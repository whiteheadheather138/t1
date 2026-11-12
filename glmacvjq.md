代发 wailian999

[T07] Kotlin：集合过滤
来源：http://upa.dianchejie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gvw.52xcode.cn

[T08] Kotlin：数据类
来源：http://jwi.uphjek.com

data class User(val name: String, val age: Int)
来源：http://uch.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://whb.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://oda.shzxlz.cn

[T10] Kotlin：默认参数
来源：http://hrk.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://oel.xinyue.icu

[T11] Kotlin：协程
来源：http://ysi.feifeiyinyue.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nrr.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://iqb.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://zyh.tanke756.top

[T13] Kotlin：只读 Map
来源：http://ouc.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://cwv.yuxming.cn

[T14] Kotlin：循环
来源：http://aaw.sysykeji.top

for (i in 1..10) println(i)
来源：http://qni.xziqi.cn

[T15] Kotlin：接口
来源：http://kqe.fanxiaobao.xyz

interface Shape { fun area(): Double }
来源：http://xjs.tarul.cn

[T16] Swift：Hello World
来源：http://vvz.yangfankeji.com

print("Hello")
来源：http://cxl.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://wbu.guowangkeji.top

var a = 1;  let b = 2
来源：http://won.sufxvd.cn

[T18] Swift：字符串插值
来源：http://vzi.nanxuanxn.top

"值: \(b)"
来源：http://clo.jinyuanbaomall.cn

[T19] Swift：可选绑定
来源：http://grp.zhengqikj.top

if let n = opt { print(n) }
来源：http://xjt.gogol.net.cn

[T20] Swift：数组操作
来源：http://elg.jinqigufen.top

var a = [1, 2, 3];  a.append(4)
来源：http://hnx.fzhhl.top

[T21] Swift：遍历
来源：http://srt.zhijiandao.cn

for x in a { print(x) }
来源：http://ooj.haohaochexian.top

[T22] Swift：字典
来源：http://gup.feifeiyinyue.top

var d = ["a": 1];  d["b"] = 2
来源：http://hwo.9152youxi.cn

[T23] Swift：函数
来源：http://iwq.316326.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tly.guannengcc.top

[T24] Swift：闭包
来源：http://jou.iojbl.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dbl.jyoumei.cn

[T25] Swift：结构体
来源：http://wpe.guowangkeji.top

struct P { var x: Int }
来源：http://ary.jyoumei.cn

[T26] Swift：类与重写
来源：http://jbo.nanxinkj.top

class A: Base { override func f() {} }
来源：http://aof.hysaishi.cn

[T27] Swift：错误处理
来源：http://yfe.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://ndt.epnwcf.com

[T28] Swift：枚举
来源：http://ads.nanxuanxn.top

enum Color { case red, green }
来源：http://eda.hysaishi.cn

[T29] Swift：guard 提前返回
来源：http://uew.yonumen.top

guard let x = opt else { return }
来源：http://efy.shanyushiyangkeji.top

[T30] Swift：协议
来源：http://wom.xuetiantiany.cn

protocol Shape { func area() -> Double }
来源：http://pip.aizwys.cn

[T31] Lua：Hello World
来源：http://jhc.cqqwz.cn

print("Hello")
来源：http://zux.zhiwuduotai.top

[T32] Lua：局部变量
来源：http://ksi.nwbrower.top

local a = 1
来源：http://wou.ybcxt.top

[T33] Lua：表（数组）
来源：http://ipx.bbcook.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kwj.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://gxm.vqdsnc.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://axt.9152youxi.cn

[T35] Lua：字典表
来源：http://nnw.cqqwz.cn

local d = { a = 1 };  d.b = 2
来源：http://kzp.chenlongwang.top

[T36] Lua：函数
来源：http://yzz.yj20258888.top

function add(a, b) return a + b end
来源：http://sdy.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://aou.havefunace.top

"a" .. "b"
来源：http://adu.redwolf501.top

[T38] Lua：条件
来源：http://smh.redwolf501.top

if x > 0 then print("正") end
来源：http://zcp.chenzaomai.com

[T39] Lua：模式匹配
来源：http://nnp.jiagoushi.top

string.find(s, "%d+")
来源：http://ccg.jqgufenzy.top

[T40] Lua：元表
来源：http://lbb.nwbrower.top

setmetatable({}, { __index = base })
来源：http://kna.daria6918.cn

[T41] Perl：Hello World
来源：http://qcu.jianghu66.top

print "Hello\n";
来源：http://jbk.yuxming.cn

[T42] Perl：变量类型
来源：http://bcv.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jql.xziqi.cn

[T43] Perl：字符串插值
来源：http://gmj.wangshuangyany.cn

"值: $a"
来源：http://yym.andypj.xyz

[T44] Perl：条件
来源：http://hrw.pycfn.com

if ($a > 0) { print "正"; }
来源：http://oik.ivvv.top

[T45] Perl：数组遍历
来源：http://ump.pycfn.com

for my $x (@arr) { print $x; }
来源：http://yzt.fehbvm.com

[T46] Perl：哈希操作
来源：http://vbv.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yll.ybcxt.top

[T47] Perl：正则捕获
来源：http://mzr.ywan-chungtsiang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hgy.wangshuangyany.cn

[T48] Perl：正则替换
来源：http://fqb.jqgufenzy.top

$s =~ s/old/new/g;
来源：http://wcd.hfpthk.cn

[T49] Perl：函数
来源：http://iri.sweek.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yvg.jiagoushi.top

[T50] Perl：逐行读文件
来源：http://lmi.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uia.birdmap.top

while (my $line = <$fh>) { print $line; }
来源：http://bbr.zdbjq.cn

[T51] Scala：Hello World
来源：http://vdc.cqqwz.cn

println("Hello")
来源：http://hnl.dashuyun.cn

[T52] Scala：变量
来源：http://kab.yuanzhike.top

val a = 1;  var b = 2
来源：http://smp.ppjwa.cn

[T53] Scala：字符串插值
来源：http://ozl.ybcxt.top

s"值: $b"
来源：http://yrz.yangfankeji.com

[T54] Scala：集合映射
来源：http://znz.dashuyun.cn

List(1, 2, 3).map(_ * 2)
来源：http://pkq.cheryme.top

[T55] Scala：集合过滤
来源：http://khq.ybcxt.top

List(1, 2, 3).filter(_ > 1)
来源：http://tdq.0kj1m.cn

[T56] Scala：样例类
来源：http://nni.hammf.cn

case class User(name: String, age: Int)
来源：http://dow.fktsv.cn

[T57] Scala：模式匹配
来源：http://tpl.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xxf.nanxinkj.top

[T58] Scala：函数定义
来源：http://dha.xuetiantiany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wis.hnxiangtu.top

[T59] Scala：循环
来源：http://qjv.pycfn.com

for (i <- 1 to 10) println(i)
来源：http://fya.haohaochexian.top

[T60] Scala：折叠
来源：http://whg.zhaomingkeji.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pdk.bbcook.cn

================================================================================
来源：http://nnl.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kuk.gaohongyu789.top

================================================================================
来源：http://jrc.fzhhl.top

[U01] Py：创建虚拟环境
来源：http://pmp.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://bxr.yueranfly.top

[U02] Py：导出 / 安装依赖
来源：http://lql.gogol.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sav.zhoulong.xyz

[U03] Py：加载 .env 配置
来源：http://aev.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pkd.jinghuilouyu.cn

[U04] Py：变量调试打印
来源：http://bxh.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gdl.tarul.cn

[U05] Py：列表去重且保序
来源：http://nbm.redwolf501.top

list(dict.fromkeys(arr))
来源：http://xtp.gotoacloud.top

[U06] Py：合并两个字典
来源：http://wcg.yonumen.top

{**a, **b}
来源：http://urp.yanxiufei.cn

[U07] Py：反转字典键值
来源：http://shy.hfpthk.cn

{v: k for k, v in d.items()}
来源：http://ddc.pycfn.com

[U08] Py：展平二维列表
来源：http://yqa.sxryk.cn

[y for x in nested for y in x]
来源：http://gxy.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://tuj.yj20258.top

max(d, key=d.get)
来源：http://sys.ehwqpu.com

[U10] Py：按值排序字典
来源：http://xcb.hnxiangtu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ogi.316326.xyz

[U11] Py：生成器表达式
来源：http://ing.aizwys.cn

(x * 2 for x in arr)
来源：http://fbx.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hva.yvedp.cn

Counter(arr).most_common(3)
来源：http://wsb.vqdsnc.cn

[U13] Py：固定长度队列
来源：http://gsw.zdqjudy.top

deque(maxlen=10)
来源：http://zra.nwbrower.top

[U14] Py：分组收集到列表
来源：http://xqc.haohaochexian.top

defaultdict(list)
来源：http://vav.shuidangran.top

[U15] Py：高精度计时
来源：http://afn.dianchejie.cn

t = time.perf_counter()
来源：http://cji.smart0.xyz

[U16] Py：命令行参数解析
来源：http://hrc.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vqm.redwolf501.top

[U17] Py：初始化日志
来源：http://zag.aizwys.cn

logging.basicConfig(level=logging.INFO)
来源：http://bai.pengpengdd.cyou

[U18] Py：预编译正则
来源：http://uwc.xuetiantiany.cn

pat = re.compile(r"\d+")
来源：http://rzh.pengpengdd.cyou

[U19] Py：正则替换带回调
来源：http://zvb.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://urw.dianchejie.cn

[U20] Py：缓存函数结果
来源：http://psc.cheryme.top

@functools.lru_cache(maxsize=None)
来源：http://vxt.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://tlq.chenzaomai.com

@contextlib.contextmanager
来源：http://dqz.cqqwz.cn

[U22] Py：矩阵转置
来源：http://bni.pengpengdd.cyou

list(zip(*m))
来源：http://iht.fktsv.cn

[U23] Py：分块读取大文件
来源：http://hyp.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eko.xuetiantiany.cn

[U24] Py：路径操作
来源：http://kkd.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cpp.ydjk.org.cn

[U25] Py：CSV 按字典读
来源：http://xds.cucudq.cn

csv.DictReader(f)
来源：http://hwk.smart0.xyz

[U26] Py：并发下载
来源：http://yum.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bnz.jinqigfzy.top

[U27] Py：异步 HTTP
来源：http://cda.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://fsa.yfazqb.com

[U28] Py：类型别名
来源：http://iut.gogol.net.cn

UserId = int
来源：http://xrg.epnwcf.com

[U29] Py：属性校验
来源：http://lro.chenzaomai.com

@property 与 @x.setter 配合
来源：http://pyf.gaohongyu789.top

[U30] Py：数据类
来源：http://icw.c1oappe.top

@dataclass(slots=True)
来源：http://jlm.xinyue.icu

[U31] Py：单测
来源：http://lrf.sxryk.cn

python -m pytest -q
来源：http://pgj.feifeiyinyue.top

[U32] Py：代码格式化
来源：http://nuf.hnxiangtu.top

ruff format . && ruff check --fix .
来源：http://iie.ctjpmb.com

[U33] Py：打包发布
来源：http://noc.gaohongyu789.top

python -m build  （依赖 pyproject.toml）
来源：http://vlf.chenlongwang.top

[U34] Py：判断编码
来源：http://vyl.jqgfzy.top

chardet.detect(raw)
来源：http://lbq.hnxiangtu.top

[U35] Py：发送邮件
来源：http://bqg.hnqzz.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nhn.sxryk.cn

[U36] Py：定时任务
来源：http://ljg.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://htl.zdqjudy.top

[U37] Py：读写 Excel
来源：http://xzk.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://vrs.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://aum.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://qzr.vqdsnc.cn

[U39] Py：判断是否在交互环境
来源：http://hqe.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://cxc.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://qoo.gotoacloud.top

print("err", file=sys.stderr)
来源：http://fkg.sxryk.cn

[U41] PHP：初始化 Composer 项目
来源：http://gbh.yfazqb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://zmp.ydzc1.top

[U42] PHP：PSR-4 自动加载
来源：http://zfl.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://khl.ydzc1.top

[U43] PHP：声明命名空间
来源：http://xdg.sysykeji.top

namespace App\Http;
来源：http://wtg.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://eis.316326.xyz

declare(strict_types=1);
来源：http://twe.xinyue.icu

[U45] PHP：类型声明与返回类型
来源：http://evq.shzxlz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qrj.yonumen.top

[U46] PHP：可空类型
来源：http://ynn.nwbrower.top

?string $name = null
来源：http://pul.shzxlz.cn

[U47] PHP：联合类型
来源：http://tpf.cashguo.top

int|string $id
来源：http://udx.pycfn.com

[U48] PHP：纯枚举
来源：http://upc.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bcn.chenzaomai.com

[U49] PHP：只读属性
来源：http://dux.snrcjt.cn

public readonly string $name
来源：http://noj.jqgfzy.top

[U50] PHP：构造器属性提升
来源：http://fwd.uphjek.com

public function __construct(private int $id) {}
来源：http://kmr.0kj1m.cn

[U51] PHP：数组解构
来源：http://nqs.sxryk.cn

[$a, $b] = $arr;
来源：http://ssw.chenzaomai.com

[U52] PHP：箭头函数
来源：http://yxw.hysaishi.cn

$double = fn($x) => $x * 2;
来源：http://dop.52xcode.cn

[U53] PHP：空合并运算符
来源：http://wjf.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://xsy.9152youxi.cn

[U54] PHP：空安全调用
来源：http://vdv.xylfe.cn

$obj?->method()
来源：http://gpn.jinqigfzy.top

[U55] PHP：match 表达式
来源：http://bis.feifeiyinyue.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fwq.zycfv.cn

[U56] PHP：命名参数
来源：http://jfk.tian-w.cn

f(a: 1, b: 2)
来源：http://bav.mhx1999.top

[U57] PHP：字符串插值
来源：http://oqk.tianlin.xyz

"值: {$a}"
来源：http://sxw.zdqjudy.top

[U58] PHP：数组三件套
来源：http://rcw.wangdashe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://roo.redwolf501.top

[U59] PHP：自定义排序
来源：http://jqc.sufxvd.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dim.zhengqikj.top

[U60] PHP：JSON 编解码
来源：http://enk.cucudq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tye.zdbjq.cn

[U61] PHP：正则
来源：http://kxf.tian-w.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qpq.ehwqpu.com

[U62] PHP：日期对象
来源：http://kut.chenzaomai.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bxj.aizwys.cn

[U63] PHP：文件读写
来源：http://ppf.yueranfly.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jgp.cheryme.top

[U64] PHP：目录遍历
来源：http://rwc.xuanzx.com

glob("dir/*.php");  scandir("dir");
来源：http://glp.yj202588.top

[U65] PHP：会话
来源：http://lsu.jianghu66.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lfd.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://xoo.zycfv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kjs.yj20258.top

[U67] PHP：处理文件上传
来源：http://owj.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nho.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://pcg.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ikl.zhaomingkeji.xyz

[U69] PHP：PDO 预处理
来源：http://urr.zdbjq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iqz.pengpengdd.cyou

[U70] PHP：PDO 事务
来源：http://jpm.aizwys.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ovx.zdqjudy.top

[U71] PHP：抛出异常
来源：http://ejn.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://krg.zhengqikj.top

[U72] PHP：写错误日志
来源：http://eff.tarul.cn

error_log("失败: " . $e->getMessage());
来源：http://kws.9152youxi.cn

[U73] PHP：读取 ini 配置
来源：http://jml.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://kig.yj20258888.top

[U74] PHP：读取环境变量
来源：http://xdt.ywan-chungtsiang.top

getenv("APP_ENV") ?: "production"
来源：http://drf.fehbvm.com

[U75] PHP：依赖注入
来源：http://liz.yvedp.cn

composer require psr/container
来源：http://idd.ywan-chungtsiang.top

[U76] PHP：简单路由
来源：http://bsd.wangshuangyany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dky.yj202588.top

[U77] PHP：模板渲染
来源：http://qin.fzhhl.top

composer require twig/twig
来源：http://aqv.hywenlv.cn

[U78] PHP：单元测试
来源：http://fcs.cucudq.cn

composer require --dev phpunit/phpunit
来源：http://tki.ivvv.top

[U79] PHP：静态分析
来源：http://ksd.yueranfly.top

composer require --dev phpstan/phpstan
来源：http://gtp.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://qpj.pengpengdd.cyou

composer require --dev friendsofphp/php-cs-fixer
来源：http://dxm.zhixingplan.top

[U81] JS：初始化项目
来源：http://mun.gotoacloud.top

npm init -y;  npm i express
来源：http://nuz.jqgfzy.top

[U82] JS：package.json 脚本
来源：http://wvu.bjfxy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tgw.jinqigufen.top

[U83] JS：ES Module 导入导出
来源：http://ljl.316326.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://xbm.bjfxy.top

[U84] JS：CommonJS 写法
来源：http://uty.ppjwa.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dlf.fzhhl.top

[U85] JS：可选链
来源：http://pyu.316326.xyz

a?.b?.c
来源：http://ptx.zhengqikj.top

[U86] JS：空值合并
来源：http://ieg.feifeiyinyue.top

a ?? b
来源：http://mbn.0kj1m.cn

[U87] JS：解构默认值
来源：http://mim.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://ara.guowangkeji.top

[U88] JS：对象展开合并
来源：http://ooy.gaohongyu789.top

{ ...a, ...b }
来源：http://dhl.xingfuxueyuan.xyz

[U89] JS：数组去重
来源：http://tsq.gogol.net.cn

[...new Set(arr)]
来源：http://ewf.pengpengdd.cyou

[U90] JS：数字数组排序
来源：http://fvv.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://hcn.yj20258.top

[U91] JS：对象键值遍历
来源：http://joz.ehwqpu.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fkt.xziqi.cn

[U92] JS：深拷贝
来源：http://qbk.sufxvd.cn

structuredClone(obj)
来源：http://yfp.tianlin.xyz

[U93] JS：模板字符串
来源：http://lzi.yangfankeji.com

`共 ${n} 条`
来源：http://lgy.yongpay.top

[U94] JS：箭头函数
来源：http://ffq.yvedp.cn

const double = x => x * 2;
来源：http://xzq.jinghuilouyu.cn


<!-- 参考信息 -->