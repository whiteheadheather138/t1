代发 wailian999

int size() const noexcept { return n_; }
来源：http://ejw.hnqzz.top

[S53] C++：移动语义
来源：http://tmm.guowangkeji.top

std::vector<int> w = std::move(v);
来源：http://srx.c1oappe.top

[S54] C++：异常处理
来源：http://dbp.vehdjk.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fjs.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://bma.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lbz.52xcode.cn

[S56] C++：optional
来源：http://rwm.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tkt.vqdsnc.cn

[S57] C++：编译期常量
来源：http://jsz.cheryme.top

constexpr int N = 10;
来源：http://btg.vehdjk.com

[S58] C++：命名空间
来源：http://cxd.xziqi.cn

namespace ns { int f() { return 1; } }
来源：http://tqz.sufxvd.cn

[S59] C++：静态断言
来源：http://ngi.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://byo.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://esw.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://crk.xuetiantiany.cn

================================================================================
来源：http://oef.xingfuxueyuan.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dcl.sjlbkw.cn

================================================================================
来源：http://prr.ivvv.top

[T01] Kotlin：Hello World
来源：http://bhq.sxryk.cn

println("Hello")
来源：http://jkk.fzhhl.top

[T02] Kotlin：变量
来源：http://kio.nanxuanxn.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://trr.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://ukz.9152youxi.cn

"值: $b"
来源：http://fma.iojbl.cn

[T04] Kotlin：空安全
来源：http://ywb.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://kdn.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://phn.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://itq.redwolf501.top

[T06] Kotlin：集合映射
来源：http://uzs.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xxx.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://tje.hfpthk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rtn.vehdjk.com

[T08] Kotlin：数据类
来源：http://hlo.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://vgg.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://uem.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://bfa.gotoacloud.top

[T10] Kotlin：默认参数
来源：http://feq.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gyi.uphjek.com

[T11] Kotlin：协程
来源：http://vay.yj20258888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sio.havefunace.top

[T12] Kotlin：解构声明
来源：http://rif.hcnkem.com

val (a, b) = Pair(1, 2)
来源：http://duz.guowangkeji.top

[T13] Kotlin：只读 Map
来源：http://qri.jqgfzy.top

val m = mapOf("a" to 1)
来源：http://swr.jianghu66.top

[T14] Kotlin：循环
来源：http://wrs.cashguo.top

for (i in 1..10) println(i)
来源：http://urv.snrcjt.cn

[T15] Kotlin：接口
来源：http://qee.yonumen.top

interface Shape { fun area(): Double }
来源：http://lwl.zhiwuduotai.top

[T16] Swift：Hello World
来源：http://jme.jlsjyb.cn

print("Hello")
来源：http://kfj.chenlongwang.top

[T17] Swift：变量与常量
来源：http://bse.cheryme.top

var a = 1;  let b = 2
来源：http://mlq.chenzaomai.com

[T18] Swift：字符串插值
来源：http://tqt.hnxiangtu.top

"值: \(b)"
来源：http://hoh.xuanzx.com

[T19] Swift：可选绑定
来源：http://qpb.yj202588.top

if let n = opt { print(n) }
来源：http://tgz.cashguo.top

[T20] Swift：数组操作
来源：http://afe.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zxv.jianghu66.top

[T21] Swift：遍历
来源：http://vrg.yonumen.top

for x in a { print(x) }
来源：http://wlc.gogol.net.cn

[T22] Swift：字典
来源：http://pfa.aibaodan.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fvw.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://isa.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ksb.zycfv.cn

[T24] Swift：闭包
来源：http://tah.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://kvl.pengpengdd.cyou

[T25] Swift：结构体
来源：http://dgn.yueranfly.top

struct P { var x: Int }
来源：http://hzg.yuanzhike.top

[T26] Swift：类与重写
来源：http://ebd.cqqwz.cn

class A: Base { override func f() {} }
来源：http://gux.zdbjq.cn

[T27] Swift：错误处理
来源：http://ewr.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://zbg.jqgufenzy.top

[T28] Swift：枚举
来源：http://mus.redwolf501.top

enum Color { case red, green }
来源：http://fdb.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://mdd.ydzc1.top

guard let x = opt else { return }
来源：http://yzy.wangdashe.top

[T30] Swift：协议
来源：http://dje.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://ecf.ybcxt.top

[T31] Lua：Hello World
来源：http://uwz.andypj.xyz

print("Hello")
来源：http://kui.daria6918.cn

[T32] Lua：局部变量
来源：http://fvz.xylfe.cn

local a = 1
来源：http://ryq.cheryme.top

[T33] Lua：表（数组）
来源：http://uri.xuanzx.com

local t = {1, 2, 3};  t[4] = 4
来源：http://sjf.hysaishi.cn

[T34] Lua：遍历表
来源：http://wsx.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://sxk.hesvh.cn

[T35] Lua：字典表
来源：http://ssm.fengsongda.top

local d = { a = 1 };  d.b = 2
来源：http://qci.fanxiaobao.xyz

[T36] Lua：函数
来源：http://xlp.0kj1m.cn

function add(a, b) return a + b end
来源：http://wet.sjlbkw.cn

[T37] Lua：字符串拼接
来源：http://gja.xuanzx.com

"a" .. "b"
来源：http://nnj.snrcjt.cn

[T38] Lua：条件
来源：http://bpt.quarkkingdee.top

if x > 0 then print("正") end
来源：http://shj.jqgfzy.top

[T39] Lua：模式匹配
来源：http://mrs.shangyingyoupin.top

string.find(s, "%d+")
来源：http://rny.jiagoushi.top

[T40] Lua：元表
来源：http://old.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://weo.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://whj.hnxiangtu.top

print "Hello\n";
来源：http://bmd.zycfv.cn

[T42] Perl：变量类型
来源：http://xdi.uphjek.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sll.cdnleiting.top

[T43] Perl：字符串插值
来源：http://hpe.daria6918.cn

"值: $a"
来源：http://yax.nanxinkj.top

[T44] Perl：条件
来源：http://zkb.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://irs.cdnleiting.top

[T45] Perl：数组遍历
来源：http://wum.zhaomingkeji.xyz

for my $x (@arr) { print $x; }
来源：http://mld.smart0.xyz

[T46] Perl：哈希操作
来源：http://eqe.jinqigfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qsl.zhengqikj.top

[T47] Perl：正则捕获
来源：http://txw.jyoumei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dof.tian-w.cn

[T48] Perl：正则替换
来源：http://nkk.hywenlv.cn

$s =~ s/old/new/g;
来源：http://bby.zycfv.cn

[T49] Perl：函数
来源：http://lgn.ywan-chungtsiang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ura.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://gmt.uphjek.com

open my $fh, "<", "a.txt" or die $!;
来源：http://lzz.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://rax.xingfuxueyuan.xyz

[T51] Scala：Hello World
来源：http://gir.zycfv.cn

println("Hello")
来源：http://eon.yuanzhike.top

[T52] Scala：变量
来源：http://obu.andypj.xyz

val a = 1;  var b = 2
来源：http://owi.sysykeji.top

[T53] Scala：字符串插值
来源：http://uay.jianghu66.top

s"值: $b"
来源：http://ilg.dashuyun.cn

[T54] Scala：集合映射
来源：http://iod.jiagoushi.top

List(1, 2, 3).map(_ * 2)
来源：http://tqx.fktsv.cn

[T55] Scala：集合过滤
来源：http://htt.fzhhl.top

List(1, 2, 3).filter(_ > 1)
来源：http://tza.yuanzhike.top

[T56] Scala：样例类
来源：http://pkz.ppjwa.cn

case class User(name: String, age: Int)
来源：http://epu.xinyue.icu

[T57] Scala：模式匹配
来源：http://rks.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://ksm.ctjpmb.com

[T58] Scala：函数定义
来源：http://xde.ywan-chungtsiang.top

def add(a: Int, b: Int): Int = a + b
来源：http://mgk.tarul.cn

[T59] Scala：循环
来源：http://jvu.hcnkem.com

for (i <- 1 to 10) println(i)
来源：http://pad.mhx1999.top

[T60] Scala：折叠
来源：http://qft.xuetiantiany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aml.hesvh.cn

================================================================================
来源：http://pne.aizwys.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gtf.quarkkingdee.top

================================================================================
来源：http://ysi.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://mbh.uphjek.com

python -m venv .venv && source .venv/bin/activate
来源：http://oan.zhengqikj.top

[U02] Py：导出 / 安装依赖
来源：http://idt.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yvl.vqdsnc.cn

[U03] Py：加载 .env 配置
来源：http://fez.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qwc.wangdashe.top

[U04] Py：变量调试打印
来源：http://daf.xylfe.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qgh.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://qnc.yonumen.top

list(dict.fromkeys(arr))
来源：http://hwr.yanxiufei.cn

[U06] Py：合并两个字典
来源：http://dfq.shuidangran.top

{**a, **b}
来源：http://aat.andypj.xyz

[U07] Py：反转字典键值
来源：http://zjr.shanyushiyangkeji.top

{v: k for k, v in d.items()}
来源：http://bqg.sufxvd.cn

[U08] Py：展平二维列表
来源：http://ayp.daria6918.cn

[y for x in nested for y in x]
来源：http://gvl.yuxming.cn

[U09] Py：字典取最大值的键
来源：http://pic.yuxming.cn

max(d, key=d.get)
来源：http://rgp.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://dlh.xingfuxueyuan.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dug.zhiwuduotai.top

[U11] Py：生成器表达式
来源：http://sbm.aizwys.cn

(x * 2 for x in arr)
来源：http://qay.sjlbkw.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xof.bbcook.cn

Counter(arr).most_common(3)
来源：http://fgf.pycfn.com

[U13] Py：固定长度队列
来源：http://fhm.fanxiaobao.xyz

deque(maxlen=10)
来源：http://vww.redwolf501.top

[U14] Py：分组收集到列表
来源：http://gyb.gzhubu.top

defaultdict(list)
来源：http://pcd.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://llm.chenzaomai.com

t = time.perf_counter()
来源：http://izq.hysaishi.cn

[U16] Py：命令行参数解析
来源：http://yzu.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ojd.vqdsnc.cn

[U17] Py：初始化日志
来源：http://boh.xziqi.cn

logging.basicConfig(level=logging.INFO)
来源：http://fir.cqqwz.cn

[U18] Py：预编译正则
来源：http://fvz.yuanzhike.top

pat = re.compile(r"\d+")
来源：http://sln.shuidangran.top

[U19] Py：正则替换带回调
来源：http://zpo.uphjek.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nga.havefunace.top

[U20] Py：缓存函数结果
来源：http://etc.gzhubu.top

@functools.lru_cache(maxsize=None)
来源：http://ocm.shzxlz.cn

[U21] Py：自定义上下文管理器
来源：http://zev.hongshengwenyu.top

@contextlib.contextmanager
来源：http://tnz.guowangkeji.top

[U22] Py：矩阵转置
来源：http://jxm.yanxiufei.cn

list(zip(*m))
来源：http://jof.pengpengdd.cyou

[U23] Py：分块读取大文件
来源：http://iib.snrcjt.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gkl.hammf.cn

[U24] Py：路径操作
来源：http://ydx.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uyw.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://sxo.andypj.xyz

csv.DictReader(f)
来源：http://slz.shuidangran.top

[U26] Py：并发下载
来源：http://hsd.gaohongyu789.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qiz.ydzc1.top

[U27] Py：异步 HTTP
来源：http://zlm.hywenlv.cn

aiohttp.ClientSession() 配合 async with
来源：http://kry.fengsongda.top

[U28] Py：类型别名
来源：http://rth.hesvh.cn

UserId = int
来源：http://aqf.quarkkingdee.top

[U29] Py：属性校验
来源：http://pbi.hcnkem.com

@property 与 @x.setter 配合
来源：http://cly.yueranfly.top

[U30] Py：数据类
来源：http://zec.birdmap.top

@dataclass(slots=True)
来源：http://scm.snrcjt.cn

[U31] Py：单测
来源：http://gxo.cheryme.top

python -m pytest -q
来源：http://sbf.chenzaomai.com

[U32] Py：代码格式化
来源：http://loh.hcnkem.com

ruff format . && ruff check --fix .
来源：http://rpa.cqqwz.cn

[U33] Py：打包发布
来源：http://vew.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://cah.jlsjyb.cn

[U34] Py：判断编码
来源：http://tqu.yj20258888.top

chardet.detect(raw)
来源：http://bnr.guowangkeji.top

[U35] Py：发送邮件
来源：http://gvn.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zxp.guannengcc.top

[U36] Py：定时任务
来源：http://gtz.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://jyx.fzhhl.top

[U37] Py：读写 Excel
来源：http://uye.yuanzhike.top

pandas.read_excel / DataFrame.to_excel
来源：http://rcd.zhoulong.xyz

[U38] Py：获取脚本所在目录
来源：http://cau.52xcode.cn

Path(__file__).resolve().parent
来源：http://maj.kuanghao11.cn

[U39] Py：判断是否在交互环境
来源：http://awk.zhengqikj.top

sys.stdout.isatty()
来源：http://hpw.shangyingyoupin.top

[U40] Py：打印到标准错误
来源：http://ryr.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://szd.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://itx.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wzw.wangshuangyany.cn

[U42] PHP：PSR-4 自动加载
来源：http://ybj.nwbrower.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cal.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://ptk.tian-w.cn

namespace App\Http;
来源：http://kea.gotoacloud.top

[U44] PHP：开启严格类型
来源：http://dta.hnqzz.top

declare(strict_types=1);
来源：http://waa.jianghu66.top

[U45] PHP：类型声明与返回类型
来源：http://tyq.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://uqi.birdmap.top

[U46] PHP：可空类型
来源：http://nwf.nanxinkj.top

?string $name = null
来源：http://mxd.jinghuilouyu.cn

[U47] PHP：联合类型
来源：http://ppp.c1oappe.top

int|string $id
来源：http://cqe.52xcode.cn

[U48] PHP：纯枚举
来源：http://kqo.hesvh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hhj.hnqzz.top

[U49] PHP：只读属性
来源：http://zta.aizwys.cn

public readonly string $name
来源：http://lsk.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://qav.ydzc1.top

public function __construct(private int $id) {}
来源：http://uuq.snrcjt.cn

[U51] PHP：数组解构
来源：http://vxi.fengsongda.top

[$a, $b] = $arr;
来源：http://isy.tian-w.cn

[U52] PHP：箭头函数
来源：http://jyq.sxryk.cn

$double = fn($x) => $x * 2;
来源：http://mpd.vehdjk.com

[U53] PHP：空合并运算符
来源：http://kgh.hnxiangtu.top

$v = $a ?? $b ?? "default";
来源：http://pfu.xylfe.cn

[U54] PHP：空安全调用
来源：http://xwg.nanxuanxn.top

$obj?->method()
来源：http://wml.wangshuangyany.cn

[U55] PHP：match 表达式
来源：http://yoy.9152youxi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://plq.hesvh.cn

[U56] PHP：命名参数
来源：http://cxz.hesvh.cn

f(a: 1, b: 2)
来源：http://qfw.nanxuanxn.top

[U57] PHP：字符串插值
来源：http://xee.redwolf501.top

"值: {$a}"
来源：http://rei.cucudq.cn

[U58] PHP：数组三件套
来源：http://jlg.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kfh.tianlin.xyz

[U59] PHP：自定义排序
来源：http://zvn.wangshuangyany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vts.yj20258.top

[U60] PHP：JSON 编解码
来源：http://ezd.xziqi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ftk.jqgfzy.top

[U61] PHP：正则
来源：http://ybt.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nnq.316326.xyz

[U62] PHP：日期对象
来源：http://wsu.shanyushiyangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ykd.yonumen.top

[U63] PHP：文件读写
来源：http://jpr.aizwys.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pmh.zhaomingkeji.xyz

[U64] PHP：目录遍历
来源：http://xcz.cashguo.top

glob("dir/*.php");  scandir("dir");
来源：http://vsm.chenlongwang.top

[U65] PHP：会话
来源：http://bxu.dashuyun.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bdj.havefunace.top

[U66] PHP：设置 Cookie
来源：http://dot.birdmap.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cdy.xinyue.icu

[U67] PHP：处理文件上传
来源：http://lnf.fengsongda.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bsb.xylfe.cn

[U68] PHP：PDO 连接
来源：http://whl.nwbrower.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wkm.pengpengdd.cyou

[U69] PHP：PDO 预处理
来源：http://nbj.guowangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eqj.hammf.cn

[U70] PHP：PDO 事务
来源：http://rws.sweek.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wee.aibaodan.cn

[U71] PHP：抛出异常
来源：http://agp.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://wkj.zhiwuduotai.top

[U72] PHP：写错误日志
来源：http://rjv.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://zci.xylfe.cn

[U73] PHP：读取 ini 配置
来源：http://vin.kuanghao11.cn

parse_ini_file("config.ini", true)
来源：http://tel.yj20258888.top

[U74] PHP：读取环境变量
来源：http://gmp.hesvh.cn

getenv("APP_ENV") ?: "production"
来源：http://wng.ydzc1.top

[U75] PHP：依赖注入
来源：http://jst.kuanghao11.cn

composer require psr/container
来源：http://wlh.ppjwa.cn

[U76] PHP：简单路由
来源：http://ptq.jqgufenzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://njg.tarul.cn

[U77] PHP：模板渲染
来源：http://cxg.52xcode.cn

composer require twig/twig
来源：http://njy.sufxvd.cn

[U78] PHP：单元测试
来源：http://crc.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://cjz.jinqigfzy.top


<!-- 参考信息 -->