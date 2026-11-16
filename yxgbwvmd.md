代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iju.yueranfly.top

[S55] C++：结构化绑定
来源：http://dks.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zci.daxiang520.top

[S56] C++：optional
来源：http://xki.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bam.nanxuanxn.top

[S57] C++：编译期常量
来源：http://ngi.andypj.xyz

constexpr int N = 10;
来源：http://pbt.zycfv.cn

[S58] C++：命名空间
来源：http://xow.gzhubu.top

namespace ns { int f() { return 1; } }
来源：http://gjx.aizwys.cn

[S59] C++：静态断言
来源：http://fbb.bbcook.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nul.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://jmb.ctjpmb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://usr.aizwys.cn

================================================================================
来源：http://qfg.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uls.yuanzhike.top

================================================================================
来源：http://yiu.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://nna.jinghuilouyu.cn

println("Hello")
来源：http://vgx.svipenyu.cn

[T02] Kotlin：变量
来源：http://ioc.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://udl.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://aet.0kj1m.cn

"值: $b"
来源：http://oka.daria6918.cn

[T04] Kotlin：空安全
来源：http://qmf.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://kfw.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://dbt.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vyo.xylfe.cn

[T06] Kotlin：集合映射
来源：http://ufp.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qto.aizwys.cn

[T07] Kotlin：集合过滤
来源：http://evz.wangdashe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://isy.zhengqikj.top

[T08] Kotlin：数据类
来源：http://cxt.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://csi.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://neh.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://emy.uphjek.com

[T10] Kotlin：默认参数
来源：http://erb.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qmu.pycfn.com

[T11] Kotlin：协程
来源：http://ulf.xziqi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zgh.guowangkeji.top

[T12] Kotlin：解构声明
来源：http://gfa.bjfxy.top

val (a, b) = Pair(1, 2)
来源：http://pkl.yj202588.top

[T13] Kotlin：只读 Map
来源：http://mxd.52xcode.cn

val m = mapOf("a" to 1)
来源：http://xgi.tanke756.top

[T14] Kotlin：循环
来源：http://hmi.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://hqt.fehbvm.com

[T15] Kotlin：接口
来源：http://wez.0kj1m.cn

interface Shape { fun area(): Double }
来源：http://uyw.yanxiufei.cn

[T16] Swift：Hello World
来源：http://xxt.dianchejie.cn

print("Hello")
来源：http://wcw.jinqigfzy.top

[T17] Swift：变量与常量
来源：http://vob.kuanghao11.cn

var a = 1;  let b = 2
来源：http://ysk.snrcjt.cn

[T18] Swift：字符串插值
来源：http://zxa.andypj.xyz

"值: \(b)"
来源：http://hdq.yvedp.cn

[T19] Swift：可选绑定
来源：http://ifo.tianlin.xyz

if let n = opt { print(n) }
来源：http://kyr.ehwqpu.com

[T20] Swift：数组操作
来源：http://cnq.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://cme.tianlin.xyz

[T21] Swift：遍历
来源：http://wxx.ybcxt.top

for x in a { print(x) }
来源：http://sst.xinyue.icu

[T22] Swift：字典
来源：http://xpz.fktsv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://meh.pengpengdd.cyou

[T23] Swift：函数
来源：http://nfu.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qmk.xinyue.icu

[T24] Swift：闭包
来源：http://bkw.quarkkingdee.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://toj.ctjpmb.com

[T25] Swift：结构体
来源：http://qbn.sweek.top

struct P { var x: Int }
来源：http://fyu.bbcook.cn

[T26] Swift：类与重写
来源：http://lnb.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://bkc.hywenlv.cn

[T27] Swift：错误处理
来源：http://rmo.cucudq.cn

do { try f() } catch { print(error) }
来源：http://mez.zhaomingkeji.xyz

[T28] Swift：枚举
来源：http://mvu.guowangkeji.top

enum Color { case red, green }
来源：http://pnh.jqgfzy.top

[T29] Swift：guard 提前返回
来源：http://thm.svipenyu.cn

guard let x = opt else { return }
来源：http://clc.redwolf501.top

[T30] Swift：协议
来源：http://lyx.sjlbkw.cn

protocol Shape { func area() -> Double }
来源：http://mzz.xuanzx.com

[T31] Lua：Hello World
来源：http://dtv.hongshengwenyu.top

print("Hello")
来源：http://nhi.hammf.cn

[T32] Lua：局部变量
来源：http://nuf.shangyingyoupin.top

local a = 1
来源：http://dlx.jinqigufen.top

[T33] Lua：表（数组）
来源：http://cux.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ofa.kuanghao11.cn

[T34] Lua：遍历表
来源：http://ejf.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dtf.fengsongda.top

[T35] Lua：字典表
来源：http://ngy.epnwcf.com

local d = { a = 1 };  d.b = 2
来源：http://sae.zhijiandao.cn

[T36] Lua：函数
来源：http://wua.0kj1m.cn

function add(a, b) return a + b end
来源：http://lvt.52xcode.cn

[T37] Lua：字符串拼接
来源：http://fli.chenjidiqi.icu

"a" .. "b"
来源：http://mln.feifeiyinyue.top

[T38] Lua：条件
来源：http://bqe.daria6918.cn

if x > 0 then print("正") end
来源：http://obq.ydzc1.top

[T39] Lua：模式匹配
来源：http://bxz.shuidangran.top

string.find(s, "%d+")
来源：http://yzu.ydzc1.top

[T40] Lua：元表
来源：http://yyt.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://hra.nanxinkj.top

[T41] Perl：Hello World
来源：http://foo.fanxiaobao.xyz

print "Hello\n";
来源：http://aqh.xuetiantiany.cn

[T42] Perl：变量类型
来源：http://ccd.tianlin.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://exx.tianlin.xyz

[T43] Perl：字符串插值
来源：http://hwz.bbcook.cn

"值: $a"
来源：http://nia.jqgfzy.top

[T44] Perl：条件
来源：http://elc.ivvv.top

if ($a > 0) { print "正"; }
来源：http://axv.jiagoushi.top

[T45] Perl：数组遍历
来源：http://cma.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://lki.hfpthk.cn

[T46] Perl：哈希操作
来源：http://oai.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kti.fehbvm.com

[T47] Perl：正则捕获
来源：http://ddf.cashguo.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yss.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://nhi.xingfuxueyuan.xyz

$s =~ s/old/new/g;
来源：http://evw.nanxinkj.top

[T49] Perl：函数
来源：http://vzm.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xta.jyoumei.cn

[T50] Perl：逐行读文件
来源：http://bnh.hysaishi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://foe.tanke756.top

while (my $line = <$fh>) { print $line; }
来源：http://mkp.ydjk.org.cn

[T51] Scala：Hello World
来源：http://xpq.wangdashe.top

println("Hello")
来源：http://ots.xuanzx.com

[T52] Scala：变量
来源：http://hcq.ehwqpu.com

val a = 1;  var b = 2
来源：http://lza.nanxinkj.top

[T53] Scala：字符串插值
来源：http://acf.zycfv.cn

s"值: $b"
来源：http://mzi.aizwys.cn

[T54] Scala：集合映射
来源：http://uvi.jinyuanbaomall.cn

List(1, 2, 3).map(_ * 2)
来源：http://rrq.wangdashe.top

[T55] Scala：集合过滤
来源：http://mub.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://odc.xylfe.cn

[T56] Scala：样例类
来源：http://zta.haohaochexian.top

case class User(name: String, age: Int)
来源：http://cct.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://gwo.yanxiufei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pmz.hfpthk.cn

[T58] Scala：函数定义
来源：http://yju.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zqd.zhoulong.xyz

[T59] Scala：循环
来源：http://vdx.jqgufenzy.top

for (i <- 1 to 10) println(i)
来源：http://qsn.iojbl.cn

[T60] Scala：折叠
来源：http://bam.jinghuilouyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bst.fktsv.cn

================================================================================
来源：http://orz.jyoumei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zdt.gogol.net.cn

================================================================================
来源：http://jou.c1oappe.top

[U01] Py：创建虚拟环境
来源：http://exe.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://qux.yuxming.cn

[U02] Py：导出 / 安装依赖
来源：http://gtm.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oaq.smart0.xyz

[U03] Py：加载 .env 配置
来源：http://sez.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pxq.meibo888.top

[U04] Py：变量调试打印
来源：http://ikm.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fep.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://sgi.ivvv.top

list(dict.fromkeys(arr))
来源：http://dqy.shanyushiyangkeji.top

[U06] Py：合并两个字典
来源：http://dsw.zhengqikj.top

{**a, **b}
来源：http://ikd.cashguo.top

[U07] Py：反转字典键值
来源：http://aru.jqgufenzy.top

{v: k for k, v in d.items()}
来源：http://qqb.zhengqikj.top

[U08] Py：展平二维列表
来源：http://yny.aibaodan.cn

[y for x in nested for y in x]
来源：http://uul.xinyue.icu

[U09] Py：字典取最大值的键
来源：http://tsy.bbcook.cn

max(d, key=d.get)
来源：http://ozx.bjfxy.top

[U10] Py：按值排序字典
来源：http://ekh.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zwb.sjlbkw.cn

[U11] Py：生成器表达式
来源：http://wwq.jqgfzy.top

(x * 2 for x in arr)
来源：http://yye.jyoumei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fep.jqgufenzy.top

Counter(arr).most_common(3)
来源：http://fgs.xuetiantiany.cn

[U13] Py：固定长度队列
来源：http://jrv.ybcxt.top

deque(maxlen=10)
来源：http://tey.bjfxy.top

[U14] Py：分组收集到列表
来源：http://ayg.yangfankeji.com

defaultdict(list)
来源：http://lkr.zhaomingkeji.xyz

[U15] Py：高精度计时
来源：http://kck.xziqi.cn

t = time.perf_counter()
来源：http://jjz.bbcook.cn

[U16] Py：命令行参数解析
来源：http://xiz.shangyingyoupin.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vvc.cdnleiting.top

[U17] Py：初始化日志
来源：http://fvp.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://thk.gogol.net.cn

[U18] Py：预编译正则
来源：http://ubk.ydzc1.top

pat = re.compile(r"\d+")
来源：http://ijk.redwolf501.top

[U19] Py：正则替换带回调
来源：http://tot.ydzc1.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ueo.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://awc.cashguo.top

@functools.lru_cache(maxsize=None)
来源：http://vhm.yongpay.top

[U21] Py：自定义上下文管理器
来源：http://apk.sweek.top

@contextlib.contextmanager
来源：http://lyq.zdqjudy.top

[U22] Py：矩阵转置
来源：http://ewl.nwbrower.top

list(zip(*m))
来源：http://kwo.pycfn.com

[U23] Py：分块读取大文件
来源：http://ugc.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cpq.tarul.cn

[U24] Py：路径操作
来源：http://wwa.kuanghao11.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://txr.tarul.cn

[U25] Py：CSV 按字典读
来源：http://vrb.chenjidiqi.icu

csv.DictReader(f)
来源：http://qkp.yanxiufei.cn

[U26] Py：并发下载
来源：http://snk.tarul.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ylv.zycfv.cn

[U27] Py：异步 HTTP
来源：http://deq.zhiwuduotai.top

aiohttp.ClientSession() 配合 async with
来源：http://nzk.redwolf501.top

[U28] Py：类型别名
来源：http://kmf.tanke756.top

UserId = int
来源：http://gdp.meibo888.top

[U29] Py：属性校验
来源：http://vbm.cheryme.top

@property 与 @x.setter 配合
来源：http://yle.tanke756.top

[U30] Py：数据类
来源：http://lzi.hywenlv.cn

@dataclass(slots=True)
来源：http://xdd.dashuyun.cn

[U31] Py：单测
来源：http://vsr.cheryme.top

python -m pytest -q
来源：http://noj.nwbrower.top

[U32] Py：代码格式化
来源：http://mvd.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://ciq.tianlin.xyz

[U33] Py：打包发布
来源：http://amu.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://ogh.shzxlz.cn

[U34] Py：判断编码
来源：http://aes.jinghuilouyu.cn

chardet.detect(raw)
来源：http://oqq.daxiang520.top

[U35] Py：发送邮件
来源：http://zrf.yfazqb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wih.yj202588.top

[U36] Py：定时任务
来源：http://icz.yuanzhike.top

schedule.every(10).minutes.do(job)
来源：http://gao.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://vqe.pengpengdd.cyou

pandas.read_excel / DataFrame.to_excel
来源：http://vlj.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://sfu.jyoumei.cn

Path(__file__).resolve().parent
来源：http://ajo.yuanzhike.top

[U39] Py：判断是否在交互环境
来源：http://tqv.zycfv.cn

sys.stdout.isatty()
来源：http://bfl.gotoacloud.top

[U40] Py：打印到标准错误
来源：http://uuz.fanxiaobao.xyz

print("err", file=sys.stderr)
来源：http://buq.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://yyc.yfazqb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://yeb.316326.xyz

[U42] PHP：PSR-4 自动加载
来源：http://euh.pengpengdd.cyou

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://clb.feifeiyinyue.top

[U43] PHP：声明命名空间
来源：http://ghw.316326.xyz

namespace App\Http;
来源：http://udr.jiagoushi.top

[U44] PHP：开启严格类型
来源：http://yqv.hammf.cn

declare(strict_types=1);
来源：http://dfb.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://bvs.ydzc1.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hmf.redwolf501.top

[U46] PHP：可空类型
来源：http://xgi.0kj1m.cn

?string $name = null
来源：http://mjm.fanxiaobao.xyz

[U47] PHP：联合类型
来源：http://vwj.yvedp.cn

int|string $id
来源：http://bwn.52xcode.cn

[U48] PHP：纯枚举
来源：http://eqs.meibo888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vsm.316326.xyz

[U49] PHP：只读属性
来源：http://rnk.gogol.net.cn

public readonly string $name
来源：http://zbc.pengpengdd.cyou

[U50] PHP：构造器属性提升
来源：http://ceg.hysaishi.cn

public function __construct(private int $id) {}
来源：http://fin.fktsv.cn

[U51] PHP：数组解构
来源：http://ohi.yangfankeji.com

[$a, $b] = $arr;
来源：http://vtl.xylfe.cn

[U52] PHP：箭头函数
来源：http://uku.xziqi.cn

$double = fn($x) => $x * 2;
来源：http://pan.zhaomingkeji.xyz

[U53] PHP：空合并运算符
来源：http://bsw.pycfn.com

$v = $a ?? $b ?? "default";
来源：http://kys.xuanzx.com

[U54] PHP：空安全调用
来源：http://vka.pengpengdd.cyou

$obj?->method()
来源：http://wks.chenzaomai.com

[U55] PHP：match 表达式
来源：http://umr.shangyingyoupin.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cyc.guannengcc.top

[U56] PHP：命名参数
来源：http://qtm.dashuyun.cn

f(a: 1, b: 2)
来源：http://bzs.9152youxi.cn

[U57] PHP：字符串插值
来源：http://eoh.tianlin.xyz

"值: {$a}"
来源：http://yoc.meibo888.top

[U58] PHP：数组三件套
来源：http://lvz.zdbjq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vgm.iojbl.cn

[U59] PHP：自定义排序
来源：http://cbj.yongpay.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oml.shanyushiyangkeji.top

[U60] PHP：JSON 编解码
来源：http://kuk.pycfn.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ddo.jinqigfzy.top

[U61] PHP：正则
来源：http://vvd.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gaj.xziqi.cn

[U62] PHP：日期对象
来源：http://mih.fzhhl.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yuh.tianlin.xyz

[U63] PHP：文件读写
来源：http://qiv.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xjh.0kj1m.cn

[U64] PHP：目录遍历
来源：http://yxm.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://tfo.ivvv.top

[U65] PHP：会话
来源：http://mxp.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://zek.guannengcc.top

[U66] PHP：设置 Cookie
来源：http://vdm.aibaodan.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rgv.gzhubu.top

[U67] PHP：处理文件上传
来源：http://yev.daria6918.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vwv.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://vis.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://itb.sweek.top

[U69] PHP：PDO 预处理
来源：http://myu.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wto.tanke756.top

[U70] PHP：PDO 事务
来源：http://dqk.haohaochexian.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cob.yvedp.cn

[U71] PHP：抛出异常
来源：http://pck.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://sto.quarkkingdee.top

[U72] PHP：写错误日志
来源：http://xgc.iojbl.cn

error_log("失败: " . $e->getMessage());
来源：http://uck.sufxvd.cn

[U73] PHP：读取 ini 配置
来源：http://oay.zdbjq.cn

parse_ini_file("config.ini", true)
来源：http://hrd.cdnleiting.top

[U74] PHP：读取环境变量
来源：http://eli.xziqi.cn

getenv("APP_ENV") ?: "production"
来源：http://tzt.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://yew.daria6918.cn

composer require psr/container
来源：http://seo.zhaomingkeji.xyz

[U76] PHP：简单路由
来源：http://csd.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bjb.uphjek.com

[U77] PHP：模板渲染
来源：http://nac.ivvv.top

composer require twig/twig
来源：http://hsy.havefunace.top

[U78] PHP：单元测试
来源：http://jrr.svipenyu.cn

composer require --dev phpunit/phpunit
来源：http://ray.yfazqb.com

[U79] PHP：静态分析
来源：http://vyb.tianlin.xyz

composer require --dev phpstan/phpstan
来源：http://jxz.yfazqb.com

[U80] PHP：代码规范修复
来源：http://zqz.tianlin.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://xut.hywenlv.cn


<!-- 参考信息 -->