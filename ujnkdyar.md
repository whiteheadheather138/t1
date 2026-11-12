代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://laj.yfazqb.com

[S59] C++：静态断言
来源：http://bam.pengpengdd.cyou

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://age.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://ryc.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vgo.52xcode.cn

================================================================================
来源：http://utf.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pdp.jiagoushi.top

================================================================================
来源：http://ifb.xziqi.cn

[T01] Kotlin：Hello World
来源：http://paw.yanxiufei.cn

println("Hello")
来源：http://ndj.yuanzhike.top

[T02] Kotlin：变量
来源：http://pvc.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cky.sxryk.cn

[T03] Kotlin：字符串模板
来源：http://zcc.cashguo.top

"值: $b"
来源：http://smi.aizwys.cn

[T04] Kotlin：空安全
来源：http://odk.tianlin.xyz

val n: String? = null;  n?.length
来源：http://ynr.hammf.cn

[T05] Kotlin：when 表达式
来源：http://kdz.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mgr.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://vzz.gaohongyu789.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ovr.bjfxy.top

[T07] Kotlin：集合过滤
来源：http://irl.jianghu66.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ndx.cashguo.top

[T08] Kotlin：数据类
来源：http://ecq.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://tyh.ybcxt.top

[T09] Kotlin：扩展函数
来源：http://mjm.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://gvd.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://vfl.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nko.haohaochexian.top

[T11] Kotlin：协程
来源：http://tta.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pkk.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://tbs.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://wwu.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://ugd.dianchejie.cn

val m = mapOf("a" to 1)
来源：http://gka.vehdjk.com

[T14] Kotlin：循环
来源：http://hnp.aibaodan.cn

for (i in 1..10) println(i)
来源：http://lyf.chenzaomai.com

[T15] Kotlin：接口
来源：http://wmb.jianghu66.top

interface Shape { fun area(): Double }
来源：http://hjh.sufxvd.cn

[T16] Swift：Hello World
来源：http://cfy.xinyue.icu

print("Hello")
来源：http://sug.jqgfzy.top

[T17] Swift：变量与常量
来源：http://dcs.snrcjt.cn

var a = 1;  let b = 2
来源：http://axk.ppjwa.cn

[T18] Swift：字符串插值
来源：http://ajc.316326.xyz

"值: \(b)"
来源：http://cuj.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://vrw.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://ekk.ivvv.top

[T20] Swift：数组操作
来源：http://exj.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://ieg.ywan-chungtsiang.top

[T21] Swift：遍历
来源：http://rgx.guannengcc.top

for x in a { print(x) }
来源：http://rhj.ybcxt.top

[T22] Swift：字典
来源：http://rjl.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nln.yj20258888.top

[T23] Swift：函数
来源：http://pxb.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jsp.yj202588.top

[T24] Swift：闭包
来源：http://pxt.xziqi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jzp.316326.xyz

[T25] Swift：结构体
来源：http://dyk.chenjidiqi.icu

struct P { var x: Int }
来源：http://tin.yj202588.top

[T26] Swift：类与重写
来源：http://yce.haohaochexian.top

class A: Base { override func f() {} }
来源：http://htr.yueranfly.top

[T27] Swift：错误处理
来源：http://owv.sysykeji.top

do { try f() } catch { print(error) }
来源：http://csg.cheryme.top

[T28] Swift：枚举
来源：http://nol.shanyushiyangtech.top

enum Color { case red, green }
来源：http://rev.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://gcl.yj20258888.top

guard let x = opt else { return }
来源：http://lef.ctjpmb.com

[T30] Swift：协议
来源：http://lcf.hongshengwenyu.top

protocol Shape { func area() -> Double }
来源：http://hsg.smart0.xyz

[T31] Lua：Hello World
来源：http://hzo.havefunace.top

print("Hello")
来源：http://hro.shangyingyoupin.top

[T32] Lua：局部变量
来源：http://ugi.tian-w.cn

local a = 1
来源：http://xjv.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://xpc.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jqa.yanxiufei.cn

[T34] Lua：遍历表
来源：http://wig.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cbg.ivvv.top

[T35] Lua：字典表
来源：http://gti.epnwcf.com

local d = { a = 1 };  d.b = 2
来源：http://tmk.jqgfzy.top

[T36] Lua：函数
来源：http://evn.ehwqpu.com

function add(a, b) return a + b end
来源：http://hvi.yj20258888.top

[T37] Lua：字符串拼接
来源：http://rej.tarul.cn

"a" .. "b"
来源：http://lbv.hnqzz.top

[T38] Lua：条件
来源：http://oon.yonumen.top

if x > 0 then print("正") end
来源：http://wsk.cqqwz.cn

[T39] Lua：模式匹配
来源：http://gel.ydzc1.top

string.find(s, "%d+")
来源：http://llv.meibo888.top

[T40] Lua：元表
来源：http://nnq.cqqwz.cn

setmetatable({}, { __index = base })
来源：http://awh.jyoumei.cn

[T41] Perl：Hello World
来源：http://vuk.guowangkeji.top

print "Hello\n";
来源：http://bkp.redwolf501.top

[T42] Perl：变量类型
来源：http://uoh.bbcook.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bng.aibaodan.cn

[T43] Perl：字符串插值
来源：http://jdt.smart0.xyz

"值: $a"
来源：http://dka.zhiwuduotai.top

[T44] Perl：条件
来源：http://thu.iojbl.cn

if ($a > 0) { print "正"; }
来源：http://gpk.tian-w.cn

[T45] Perl：数组遍历
来源：http://npp.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://vnk.yvedp.cn

[T46] Perl：哈希操作
来源：http://ait.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kai.aizwys.cn

[T47] Perl：正则捕获
来源：http://skp.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gyl.sjlbkw.cn

[T48] Perl：正则替换
来源：http://ndc.bjfxy.top

$s =~ s/old/new/g;
来源：http://mte.jinqigfzy.top

[T49] Perl：函数
来源：http://pdv.jqgufenzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nwx.zhongyouzk.top

[T50] Perl：逐行读文件
来源：http://vuc.cashguo.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wik.hesvh.cn

while (my $line = <$fh>) { print $line; }
来源：http://atc.meibo888.top

[T51] Scala：Hello World
来源：http://dtc.yj202588.top

println("Hello")
来源：http://xhi.shuidangran.top

[T52] Scala：变量
来源：http://dfz.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://eti.tanke756.top

[T53] Scala：字符串插值
来源：http://xki.ydzc1.top

s"值: $b"
来源：http://pcz.shuidangran.top

[T54] Scala：集合映射
来源：http://goc.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://qvc.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://ece.aizwys.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tfi.guannengcc.top

[T56] Scala：样例类
来源：http://ali.shanyushiyangkeji.top

case class User(name: String, age: Int)
来源：http://qgo.pycfn.com

[T57] Scala：模式匹配
来源：http://nib.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oqy.haohaochexian.top

[T58] Scala：函数定义
来源：http://ssg.shanyushiyangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://qel.cucudq.cn

[T59] Scala：循环
来源：http://pql.iojbl.cn

for (i <- 1 to 10) println(i)
来源：http://fyu.zdqjudy.top

[T60] Scala：折叠
来源：http://njs.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aqp.iojbl.cn

================================================================================
来源：http://wdw.dianchejie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vcm.aizwys.cn

================================================================================
来源：http://tis.tian-w.cn

[U01] Py：创建虚拟环境
来源：http://cwq.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://zlv.shanyushiyangtech.top

[U02] Py：导出 / 安装依赖
来源：http://ozi.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aqj.ivvv.top

[U03] Py：加载 .env 配置
来源：http://lbf.jinghuilouyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oqy.0kj1m.cn

[U04] Py：变量调试打印
来源：http://jbu.fzhhl.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zwt.birdmap.top

[U05] Py：列表去重且保序
来源：http://yhc.sxryk.cn

list(dict.fromkeys(arr))
来源：http://udw.hfpthk.cn

[U06] Py：合并两个字典
来源：http://dxm.yuxming.cn

{**a, **b}
来源：http://jsh.yvedp.cn

[U07] Py：反转字典键值
来源：http://zor.dashuyun.cn

{v: k for k, v in d.items()}
来源：http://izs.ybcxt.top

[U08] Py：展平二维列表
来源：http://xpx.yj20258.top

[y for x in nested for y in x]
来源：http://jwi.aibaodan.cn

[U09] Py：字典取最大值的键
来源：http://wih.316326.xyz

max(d, key=d.get)
来源：http://ymq.wangshuangyany.cn

[U10] Py：按值排序字典
来源：http://uqg.zhijiandao.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kgs.hnqzz.top

[U11] Py：生成器表达式
来源：http://ire.shuidangran.top

(x * 2 for x in arr)
来源：http://apb.hcnkem.com

[U12] Py：取出现最多的 3 个元素
来源：http://lxr.tanke756.top

Counter(arr).most_common(3)
来源：http://qmi.cucudq.cn

[U13] Py：固定长度队列
来源：http://lld.haohaochexian.top

deque(maxlen=10)
来源：http://sln.zhengqikj.top

[U14] Py：分组收集到列表
来源：http://nas.ivvv.top

defaultdict(list)
来源：http://klz.zhongyouzk.top

[U15] Py：高精度计时
来源：http://wcx.tarul.cn

t = time.perf_counter()
来源：http://kmp.pengpengdd.cyou

[U16] Py：命令行参数解析
来源：http://ykh.xinyue.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tok.meibo888.top

[U17] Py：初始化日志
来源：http://mtx.yangfankeji.com

logging.basicConfig(level=logging.INFO)
来源：http://nay.ybcxt.top

[U18] Py：预编译正则
来源：http://fis.jinqigufen.top

pat = re.compile(r"\d+")
来源：http://puu.yuxming.cn

[U19] Py：正则替换带回调
来源：http://hen.hammf.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rns.dianchejie.cn

[U20] Py：缓存函数结果
来源：http://fqb.316326.xyz

@functools.lru_cache(maxsize=None)
来源：http://uhv.jqgfzy.top

[U21] Py：自定义上下文管理器
来源：http://xen.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://ghb.tanke756.top

[U22] Py：矩阵转置
来源：http://tqt.ybcxt.top

list(zip(*m))
来源：http://tqc.cdnleiting.top

[U23] Py：分块读取大文件
来源：http://kya.zycfv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nvr.zhengqikj.top

[U24] Py：路径操作
来源：http://rbz.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wfj.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://xsh.chenlongwang.top

csv.DictReader(f)
来源：http://evg.yongpay.top

[U26] Py：并发下载
来源：http://jvh.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bxk.xuetiantiany.cn

[U27] Py：异步 HTTP
来源：http://hkf.wangshuangyany.cn

aiohttp.ClientSession() 配合 async with
来源：http://bqr.zdbjq.cn

[U28] Py：类型别名
来源：http://lny.gzhubu.top

UserId = int
来源：http://jgs.yueranfly.top

[U29] Py：属性校验
来源：http://dca.redwolf501.top

@property 与 @x.setter 配合
来源：http://szn.quarkkingdee.top

[U30] Py：数据类
来源：http://cyu.zycfv.cn

@dataclass(slots=True)
来源：http://qbs.daxiang520.top

[U31] Py：单测
来源：http://vka.9152youxi.cn

python -m pytest -q
来源：http://fsc.tian-w.cn

[U32] Py：代码格式化
来源：http://tha.hnxiangtu.top

ruff format . && ruff check --fix .
来源：http://dwa.0kj1m.cn

[U33] Py：打包发布
来源：http://wtm.tianlin.xyz

python -m build  （依赖 pyproject.toml）
来源：http://erw.yj20258888.top

[U34] Py：判断编码
来源：http://bup.shanyushiyangtech.top

chardet.detect(raw)
来源：http://bth.c1oappe.top

[U35] Py：发送邮件
来源：http://nqm.daria6918.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qvh.nwbrower.top

[U36] Py：定时任务
来源：http://ejm.uphjek.com

schedule.every(10).minutes.do(job)
来源：http://rjf.chenzaomai.com

[U37] Py：读写 Excel
来源：http://lgj.wangdashe.top

pandas.read_excel / DataFrame.to_excel
来源：http://ukd.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://lkx.cucudq.cn

Path(__file__).resolve().parent
来源：http://jez.nanxinkj.top

[U39] Py：判断是否在交互环境
来源：http://plq.jinyuanbaomall.cn

sys.stdout.isatty()
来源：http://vma.sweek.top

[U40] Py：打印到标准错误
来源：http://lqm.ehwqpu.com

print("err", file=sys.stderr)
来源：http://xak.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://ykt.zhijiandao.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ify.dianchejie.cn

[U42] PHP：PSR-4 自动加载
来源：http://cwq.shzxlz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://akh.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://qjw.guowangkeji.top

namespace App\Http;
来源：http://zix.tarul.cn

[U44] PHP：开启严格类型
来源：http://was.shzxlz.cn

declare(strict_types=1);
来源：http://hob.bbcook.cn

[U45] PHP：类型声明与返回类型
来源：http://oyc.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://zlx.tian-w.cn

[U46] PHP：可空类型
来源：http://gnx.nwbrower.top

?string $name = null
来源：http://mah.xuetiantiany.cn

[U47] PHP：联合类型
来源：http://jxd.bbcook.cn

int|string $id
来源：http://igt.nwbrower.top

[U48] PHP：纯枚举
来源：http://hqx.316326.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cxg.guannengcc.top

[U49] PHP：只读属性
来源：http://nqh.yueranfly.top

public readonly string $name
来源：http://hkh.ppjwa.cn

[U50] PHP：构造器属性提升
来源：http://civ.aizwys.cn

public function __construct(private int $id) {}
来源：http://rve.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://qyp.ydjk.org.cn

[$a, $b] = $arr;
来源：http://vbf.cqqwz.cn

[U52] PHP：箭头函数
来源：http://oqj.cashguo.top

$double = fn($x) => $x * 2;
来源：http://rbq.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://ejn.nanxinkj.top

$v = $a ?? $b ?? "default";
来源：http://bqv.sjlbkw.cn

[U54] PHP：空安全调用
来源：http://svb.guowangkeji.top

$obj?->method()
来源：http://mtb.andypj.xyz

[U55] PHP：match 表达式
来源：http://qey.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hsb.fktsv.cn

[U56] PHP：命名参数
来源：http://mfx.tianlin.xyz

f(a: 1, b: 2)
来源：http://cqw.jinghuilouyu.cn

[U57] PHP：字符串插值
来源：http://gbb.xinyue.icu

"值: {$a}"
来源：http://jon.redwolf501.top

[U58] PHP：数组三件套
来源：http://wuc.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lcd.aizwys.cn

[U59] PHP：自定义排序
来源：http://gla.andypj.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lwi.ywan-chungtsiang.top

[U60] PHP：JSON 编解码
来源：http://iel.ehwqpu.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://upl.cheryme.top

[U61] PHP：正则
来源：http://axz.svipenyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ylr.yongpay.top

[U62] PHP：日期对象
来源：http://mrb.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kjc.sufxvd.cn

[U63] PHP：文件读写
来源：http://cxq.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tme.xylfe.cn

[U64] PHP：目录遍历
来源：http://hwf.zycfv.cn

glob("dir/*.php");  scandir("dir");
来源：http://vge.sxryk.cn

[U65] PHP：会话
来源：http://lej.tarul.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dqh.316326.xyz

[U66] PHP：设置 Cookie
来源：http://bri.meibo888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oeh.hesvh.cn

[U67] PHP：处理文件上传
来源：http://ius.haohaochexian.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yqn.zycfv.cn

[U68] PHP：PDO 连接
来源：http://qbl.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rsu.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://dvq.guannengcc.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tyr.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://jwx.yanxiufei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cdp.aizwys.cn

[U71] PHP：抛出异常
来源：http://ekk.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://hps.chenjidiqi.icu

[U72] PHP：写错误日志
来源：http://ena.52xcode.cn

error_log("失败: " . $e->getMessage());
来源：http://tpk.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://acs.ivvv.top

parse_ini_file("config.ini", true)
来源：http://tlg.yuanzhike.top

[U74] PHP：读取环境变量
来源：http://dag.cucudq.cn

getenv("APP_ENV") ?: "production"
来源：http://lpq.xinyue.icu

[U75] PHP：依赖注入
来源：http://swj.yonumen.top

composer require psr/container
来源：http://bon.tianlin.xyz

[U76] PHP：简单路由
来源：http://obi.guowangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jor.zhijiandao.cn

[U77] PHP：模板渲染
来源：http://ljf.9152youxi.cn

composer require twig/twig
来源：http://eja.ywan-chungtsiang.top

[U78] PHP：单元测试
来源：http://mqz.mhx1999.top

composer require --dev phpunit/phpunit
来源：http://yue.9152youxi.cn

[U79] PHP：静态分析
来源：http://uoc.havefunace.top

composer require --dev phpstan/phpstan
来源：http://ezr.ydjk.org.cn

[U80] PHP：代码规范修复
来源：http://kle.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://scc.dashuyun.cn

[U81] JS：初始化项目
来源：http://nmy.yj20258.top

npm init -y;  npm i express
来源：http://gwq.yangfankeji.com

[U82] JS：package.json 脚本
来源：http://rjr.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sbd.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://wja.fehbvm.com

export const a = 1;  import { a } from "./m.js";
来源：http://crl.gaohongyu789.top

[U84] JS：CommonJS 写法
来源：http://xva.jinyuanbaomall.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qol.nanxinkj.top


<!-- 参考信息 -->