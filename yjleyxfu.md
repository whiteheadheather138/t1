代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kdm.guannengcc.top

[S51] C++：显式类型转换
来源：http://rdl.nanxinkj.top

static_cast<double>(a) / b
来源：http://swu.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://ddj.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://vre.cheryme.top

[S53] C++：移动语义
来源：http://ako.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://kpq.yongpay.top

[S54] C++：异常处理
来源：http://ilk.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nrj.pycfn.com

[S55] C++：结构化绑定
来源：http://nhl.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tvv.jqgfzy.top

[S56] C++：optional
来源：http://ezq.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hhz.zhiwuduotai.top

[S57] C++：编译期常量
来源：http://zel.mhx1999.top

constexpr int N = 10;
来源：http://ydw.kuanghao11.cn

[S58] C++：命名空间
来源：http://arz.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://qqp.ehwqpu.com

[S59] C++：静态断言
来源：http://kjo.vehdjk.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://peh.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://gfz.cdnleiting.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://myq.jqgufenzy.top

================================================================================
来源：http://mdb.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ncy.wangdashe.top

================================================================================
来源：http://siq.daxiang520.top

[T01] Kotlin：Hello World
来源：http://bsj.sysykeji.top

println("Hello")
来源：http://gvi.9152youxi.cn

[T02] Kotlin：变量
来源：http://vhr.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ism.xziqi.cn

[T03] Kotlin：字符串模板
来源：http://yba.sjlbkw.cn

"值: $b"
来源：http://ieo.yangfankeji.com

[T04] Kotlin：空安全
来源：http://afx.shzxlz.cn

val n: String? = null;  n?.length
来源：http://zog.hongshengwenyu.top

[T05] Kotlin：when 表达式
来源：http://tyr.wangdashe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hhb.ybcxt.top

[T06] Kotlin：集合映射
来源：http://aoa.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://crv.gaohongyu789.top

[T07] Kotlin：集合过滤
来源：http://fzw.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tjx.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://vgs.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://cag.dashuyun.cn

[T09] Kotlin：扩展函数
来源：http://csy.fengsongda.top

fun String.exclaim() = this + "!"
来源：http://zgx.nanxinkj.top

[T10] Kotlin：默认参数
来源：http://aje.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nvw.havefunace.top

[T11] Kotlin：协程
来源：http://eqb.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lvz.yvedp.cn

[T12] Kotlin：解构声明
来源：http://sas.sweek.top

val (a, b) = Pair(1, 2)
来源：http://dxa.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://usn.yuxming.cn

val m = mapOf("a" to 1)
来源：http://msq.gzhubu.top

[T14] Kotlin：循环
来源：http://dnh.yongpay.top

for (i in 1..10) println(i)
来源：http://huq.aibaodan.cn

[T15] Kotlin：接口
来源：http://yhm.tanke756.top

interface Shape { fun area(): Double }
来源：http://bnh.quarkkingdee.top

[T16] Swift：Hello World
来源：http://fuo.fehbvm.com

print("Hello")
来源：http://gxa.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://jst.gotoacloud.top

var a = 1;  let b = 2
来源：http://kih.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://clt.52xcode.cn

"值: \(b)"
来源：http://sep.jlsjyb.cn

[T19] Swift：可选绑定
来源：http://jcm.yangfankeji.com

if let n = opt { print(n) }
来源：http://gdo.aizwys.cn

[T20] Swift：数组操作
来源：http://zdx.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://ghx.bjfxy.top

[T21] Swift：遍历
来源：http://rdx.andypj.xyz

for x in a { print(x) }
来源：http://uvq.xinyue.icu

[T22] Swift：字典
来源：http://ssm.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://fkm.redwolf501.top

[T23] Swift：函数
来源：http://evu.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://duu.fanxiaobao.xyz

[T24] Swift：闭包
来源：http://vra.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jar.jqgfzy.top

[T25] Swift：结构体
来源：http://nrw.nanxinkj.top

struct P { var x: Int }
来源：http://odg.meibo888.top

[T26] Swift：类与重写
来源：http://mtr.zdqjudy.top

class A: Base { override func f() {} }
来源：http://mhz.yangfankeji.com

[T27] Swift：错误处理
来源：http://mfa.cashguo.top

do { try f() } catch { print(error) }
来源：http://yas.quarkkingdee.top

[T28] Swift：枚举
来源：http://kpp.quarkkingdee.top

enum Color { case red, green }
来源：http://qih.jlsjyb.cn

[T29] Swift：guard 提前返回
来源：http://iry.zhongyouzk.top

guard let x = opt else { return }
来源：http://cwk.andypj.xyz

[T30] Swift：协议
来源：http://igh.ydzc1.top

protocol Shape { func area() -> Double }
来源：http://ehc.wangdashe.top

[T31] Lua：Hello World
来源：http://exd.wangshuangyany.cn

print("Hello")
来源：http://ywj.yfazqb.com

[T32] Lua：局部变量
来源：http://nst.sufxvd.cn

local a = 1
来源：http://kco.gogol.net.cn

[T33] Lua：表（数组）
来源：http://joj.52xcode.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dds.hammf.cn

[T34] Lua：遍历表
来源：http://ill.snrcjt.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ddj.uphjek.com

[T35] Lua：字典表
来源：http://end.yangfankeji.com

local d = { a = 1 };  d.b = 2
来源：http://akw.tian-w.cn

[T36] Lua：函数
来源：http://avk.dashuyun.cn

function add(a, b) return a + b end
来源：http://nox.sxryk.cn

[T37] Lua：字符串拼接
来源：http://tcn.zhoulong.xyz

"a" .. "b"
来源：http://lxk.redwolf501.top

[T38] Lua：条件
来源：http://ekl.tanke756.top

if x > 0 then print("正") end
来源：http://idn.chenlongwang.top

[T39] Lua：模式匹配
来源：http://vqs.hammf.cn

string.find(s, "%d+")
来源：http://qlx.zhoulong.xyz

[T40] Lua：元表
来源：http://xuv.sweek.top

setmetatable({}, { __index = base })
来源：http://txj.fengsongda.top

[T41] Perl：Hello World
来源：http://rix.zhijiandao.cn

print "Hello\n";
来源：http://uni.hnxiangtu.top

[T42] Perl：变量类型
来源：http://cod.yuxming.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rnk.aibaodan.cn

[T43] Perl：字符串插值
来源：http://mnu.0kj1m.cn

"值: $a"
来源：http://zlu.fanxiaobao.xyz

[T44] Perl：条件
来源：http://xsq.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://unz.fehbvm.com

[T45] Perl：数组遍历
来源：http://hew.guowangkeji.top

for my $x (@arr) { print $x; }
来源：http://sqi.hongshengwenyu.top

[T46] Perl：哈希操作
来源：http://heb.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aqo.52xcode.cn

[T47] Perl：正则捕获
来源：http://qvi.daxiang520.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pvt.cucudq.cn

[T48] Perl：正则替换
来源：http://aoc.jqgfzy.top

$s =~ s/old/new/g;
来源：http://yml.sufxvd.cn

[T49] Perl：函数
来源：http://raw.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tng.9152youxi.cn

[T50] Perl：逐行读文件
来源：http://zzb.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://cmd.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://yub.xylfe.cn

[T51] Scala：Hello World
来源：http://ntv.vqdsnc.cn

println("Hello")
来源：http://lnp.smart0.xyz

[T52] Scala：变量
来源：http://yaj.yongpay.top

val a = 1;  var b = 2
来源：http://wlj.cqqwz.cn

[T53] Scala：字符串插值
来源：http://wgf.nanxuanxn.top

s"值: $b"
来源：http://rfh.sweek.top

[T54] Scala：集合映射
来源：http://faf.yanxiufei.cn

List(1, 2, 3).map(_ * 2)
来源：http://sje.jinqigufen.top

[T55] Scala：集合过滤
来源：http://ocq.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://qed.wangdashe.top

[T56] Scala：样例类
来源：http://aeh.cheryme.top

case class User(name: String, age: Int)
来源：http://rlv.jinyuanbaomall.cn

[T57] Scala：模式匹配
来源：http://zia.xingfuxueyuan.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://qzt.yonumen.top

[T58] Scala：函数定义
来源：http://uzt.snrcjt.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bqw.vqdsnc.cn

[T59] Scala：循环
来源：http://adf.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://aja.xingfuxueyuan.xyz

[T60] Scala：折叠
来源：http://rco.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dqp.ydzc1.top

================================================================================
来源：http://zyd.jqgfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rqb.yuxming.cn

================================================================================
来源：http://rqy.vqdsnc.cn

[U01] Py：创建虚拟环境
来源：http://pqz.nanxuanxn.top

python -m venv .venv && source .venv/bin/activate
来源：http://woj.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://ias.fzhhl.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yre.vehdjk.com

[U03] Py：加载 .env 配置
来源：http://jsv.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ueb.xziqi.cn

[U04] Py：变量调试打印
来源：http://off.xuanzx.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sig.nwbrower.top

[U05] Py：列表去重且保序
来源：http://pse.svipenyu.cn

list(dict.fromkeys(arr))
来源：http://cqo.cqqwz.cn

[U06] Py：合并两个字典
来源：http://hkn.xziqi.cn

{**a, **b}
来源：http://jgs.fzhhl.top

[U07] Py：反转字典键值
来源：http://dqq.cashguo.top

{v: k for k, v in d.items()}
来源：http://jdu.meibo888.top

[U08] Py：展平二维列表
来源：http://aqx.sxryk.cn

[y for x in nested for y in x]
来源：http://poa.52xcode.cn

[U09] Py：字典取最大值的键
来源：http://zyx.fanxiaobao.xyz

max(d, key=d.get)
来源：http://brj.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://mjj.yvedp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hmc.cucudq.cn

[U11] Py：生成器表达式
来源：http://rfu.hywenlv.cn

(x * 2 for x in arr)
来源：http://eot.ydjk.org.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ybh.aibaodan.cn

Counter(arr).most_common(3)
来源：http://kjc.jinqigufen.top

[U13] Py：固定长度队列
来源：http://lzo.chenlongwang.top

deque(maxlen=10)
来源：http://pcq.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://wuh.gotoacloud.top

defaultdict(list)
来源：http://qcx.bjfxy.top

[U15] Py：高精度计时
来源：http://xix.fanxiaobao.xyz

t = time.perf_counter()
来源：http://uij.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://gkr.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xkl.zhongyouzk.top

[U17] Py：初始化日志
来源：http://btp.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://nwk.ctjpmb.com

[U18] Py：预编译正则
来源：http://jvg.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://frg.fanxiaobao.xyz

[U19] Py：正则替换带回调
来源：http://ynl.hcnkem.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aea.jinqigufen.top

[U20] Py：缓存函数结果
来源：http://qtf.zdbjq.cn

@functools.lru_cache(maxsize=None)
来源：http://ewf.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://xlh.sysykeji.top

@contextlib.contextmanager
来源：http://iwr.jyoumei.cn

[U22] Py：矩阵转置
来源：http://lbn.yvedp.cn

list(zip(*m))
来源：http://foh.chenzaomai.com

[U23] Py：分块读取大文件
来源：http://ddp.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://omw.epnwcf.com

[U24] Py：路径操作
来源：http://qqe.tanke756.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lns.xingfuxueyuan.xyz

[U25] Py：CSV 按字典读
来源：http://zqe.chenlongwang.top

csv.DictReader(f)
来源：http://iih.havefunace.top

[U26] Py：并发下载
来源：http://uvl.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fju.smart0.xyz

[U27] Py：异步 HTTP
来源：http://pms.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://xnq.ehwqpu.com

[U28] Py：类型别名
来源：http://vxl.52xcode.cn

UserId = int
来源：http://hvw.sweek.top

[U29] Py：属性校验
来源：http://yyl.chenzaomai.com

@property 与 @x.setter 配合
来源：http://mkg.jyoumei.cn

[U30] Py：数据类
来源：http://sfk.yangfankeji.com

@dataclass(slots=True)
来源：http://hws.yongpay.top

[U31] Py：单测
来源：http://usy.wangshuangyany.cn

python -m pytest -q
来源：http://qoe.gogol.net.cn

[U32] Py：代码格式化
来源：http://tow.redwolf501.top

ruff format . && ruff check --fix .
来源：http://mja.xuanzx.com

[U33] Py：打包发布
来源：http://pjy.yj20258.top

python -m build  （依赖 pyproject.toml）
来源：http://str.xuanzx.com

[U34] Py：判断编码
来源：http://mxj.xuetiantiany.cn

chardet.detect(raw)
来源：http://akb.epnwcf.com

[U35] Py：发送邮件
来源：http://qld.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hhg.havefunace.top

[U36] Py：定时任务
来源：http://nwt.tianlin.xyz

schedule.every(10).minutes.do(job)
来源：http://qzy.dashuyun.cn

[U37] Py：读写 Excel
来源：http://lrs.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://ucs.ivvv.top

[U38] Py：获取脚本所在目录
来源：http://den.fzhhl.top

Path(__file__).resolve().parent
来源：http://axx.iojbl.cn

[U39] Py：判断是否在交互环境
来源：http://eky.zdqjudy.top

sys.stdout.isatty()
来源：http://ufz.cucudq.cn

[U40] Py：打印到标准错误
来源：http://ttb.dashuyun.cn

print("err", file=sys.stderr)
来源：http://jty.wangdashe.top

[U41] PHP：初始化 Composer 项目
来源：http://oah.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vax.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://vwc.zhongyouzk.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dkk.yonumen.top

[U43] PHP：声明命名空间
来源：http://nou.vqdsnc.cn

namespace App\Http;
来源：http://ust.xuanzx.com

[U44] PHP：开启严格类型
来源：http://kxf.cheryme.top

declare(strict_types=1);
来源：http://bah.gogol.net.cn

[U45] PHP：类型声明与返回类型
来源：http://ddq.sufxvd.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kpj.zhiwuduotai.top

[U46] PHP：可空类型
来源：http://cda.wangdashe.top

?string $name = null
来源：http://hfq.ydjk.org.cn

[U47] PHP：联合类型
来源：http://lob.smart0.xyz

int|string $id
来源：http://gxb.sxryk.cn

[U48] PHP：纯枚举
来源：http://smw.9152youxi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wrm.zhixingplan.top

[U49] PHP：只读属性
来源：http://ecg.gogol.net.cn

public readonly string $name
来源：http://ntc.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://jkm.ivvv.top

public function __construct(private int $id) {}
来源：http://tmi.dianchejie.cn

[U51] PHP：数组解构
来源：http://fbj.hfpthk.cn

[$a, $b] = $arr;
来源：http://hfe.sufxvd.cn

[U52] PHP：箭头函数
来源：http://nfc.smart0.xyz

$double = fn($x) => $x * 2;
来源：http://vyu.xuetiantiany.cn

[U53] PHP：空合并运算符
来源：http://vxs.gaohongyu789.top

$v = $a ?? $b ?? "default";
来源：http://cvr.hesvh.cn

[U54] PHP：空安全调用
来源：http://ahl.jianghu66.top

$obj?->method()
来源：http://hii.hywenlv.cn

[U55] PHP：match 表达式
来源：http://ykp.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nby.fehbvm.com

[U56] PHP：命名参数
来源：http://mct.birdmap.top

f(a: 1, b: 2)
来源：http://dus.hongshengwenyu.top

[U57] PHP：字符串插值
来源：http://xjy.dianchejie.cn

"值: {$a}"
来源：http://ksv.zhixingplan.top

[U58] PHP：数组三件套
来源：http://idf.xingfuxueyuan.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ewc.sysykeji.top

[U59] PHP：自定义排序
来源：http://mtj.iojbl.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ajl.chenlongwang.top

[U60] PHP：JSON 编解码
来源：http://pcv.haohaochexian.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hpa.tanke756.top

[U61] PHP：正则
来源：http://yei.chenzaomai.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gnj.shzxlz.cn

[U62] PHP：日期对象
来源：http://pwx.zhoulong.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wxz.hfpthk.cn

[U63] PHP：文件读写
来源：http://wpc.andypj.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jeo.fktsv.cn

[U64] PHP：目录遍历
来源：http://yzh.zhixingplan.top

glob("dir/*.php");  scandir("dir");
来源：http://uyt.jianghu66.top

[U65] PHP：会话
来源：http://uil.zhaomingkeji.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://fqi.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://byf.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xqd.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://nxg.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lhj.cdnleiting.top

[U68] PHP：PDO 连接
来源：http://chq.ybcxt.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rbs.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://agw.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://imq.svipenyu.cn

[U70] PHP：PDO 事务
来源：http://vyn.andypj.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://awf.aibaodan.cn

[U71] PHP：抛出异常
来源：http://gki.jiagoushi.top

throw new RuntimeException("失败", 500);
来源：http://rcw.chenlongwang.top

[U72] PHP：写错误日志
来源：http://xbk.xziqi.cn

error_log("失败: " . $e->getMessage());
来源：http://did.tarul.cn

[U73] PHP：读取 ini 配置
来源：http://lqe.jinqigfzy.top

parse_ini_file("config.ini", true)
来源：http://eqp.pycfn.com

[U74] PHP：读取环境变量
来源：http://ilp.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://fuk.cdnleiting.top

[U75] PHP：依赖注入
来源：http://jat.0kj1m.cn

composer require psr/container
来源：http://ilh.fengsongda.top

[U76] PHP：简单路由
来源：http://tnj.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ihc.wangdashe.top


<!-- 参考信息 -->