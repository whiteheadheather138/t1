代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://buv.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://rft.cqqwz.cn

static_cast<double>(a) / b
来源：http://syy.xuetiantiany.cn

[S52] C++：const 与 noexcept
来源：http://buh.shanyushiyangkeji.top

int size() const noexcept { return n_; }
来源：http://uht.ivvv.top

[S53] C++：移动语义
来源：http://uxv.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://pfg.yonumen.top

[S54] C++：异常处理
来源：http://xqy.nanxinkj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lys.andypj.xyz

[S55] C++：结构化绑定
来源：http://eut.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eeb.yfazqb.com

[S56] C++：optional
来源：http://ciu.yuxming.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://chm.chenlongwang.top

[S57] C++：编译期常量
来源：http://rnb.shangyingyoupin.top

constexpr int N = 10;
来源：http://ykd.zhongyouzk.top

[S58] C++：命名空间
来源：http://ymt.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://kfl.wangdashe.top

[S59] C++：静态断言
来源：http://duv.cdnleiting.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cvz.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://cya.9152youxi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ibh.uphjek.com

================================================================================
来源：http://hba.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lmw.jiagoushi.top

================================================================================
来源：http://jhm.vehdjk.com

[T01] Kotlin：Hello World
来源：http://ywh.52xcode.cn

println("Hello")
来源：http://iqb.zhoulong.xyz

[T02] Kotlin：变量
来源：http://vyz.gaohongyu789.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zkn.ywan-chungtsiang.top

[T03] Kotlin：字符串模板
来源：http://slf.yangfankeji.com

"值: $b"
来源：http://nku.xylfe.cn

[T04] Kotlin：空安全
来源：http://yha.yongpay.top

val n: String? = null;  n?.length
来源：http://irl.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://ofi.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yhm.jianghu66.top

[T06] Kotlin：集合映射
来源：http://hqp.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lgl.birdmap.top

[T07] Kotlin：集合过滤
来源：http://axj.jinyuanbaomall.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pkg.jqgfzy.top

[T08] Kotlin：数据类
来源：http://swq.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://mln.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://gyv.jlsjyb.cn

fun String.exclaim() = this + "!"
来源：http://gve.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://ygy.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://shd.snrcjt.cn

[T11] Kotlin：协程
来源：http://dxv.pengpengdd.cyou

GlobalScope.launch { delay(1000); println("done") }
来源：http://shq.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://hft.shzxlz.cn

val (a, b) = Pair(1, 2)
来源：http://kvi.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://ygw.cucudq.cn

val m = mapOf("a" to 1)
来源：http://jim.cqqwz.cn

[T14] Kotlin：循环
来源：http://mym.ppjwa.cn

for (i in 1..10) println(i)
来源：http://uth.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://iyk.sxryk.cn

interface Shape { fun area(): Double }
来源：http://oxi.sufxvd.cn

[T16] Swift：Hello World
来源：http://vua.hywenlv.cn

print("Hello")
来源：http://mpe.gotoacloud.top

[T17] Swift：变量与常量
来源：http://grq.yuxming.cn

var a = 1;  let b = 2
来源：http://bmy.cucudq.cn

[T18] Swift：字符串插值
来源：http://mkh.gzhubu.top

"值: \(b)"
来源：http://wji.yongpay.top

[T19] Swift：可选绑定
来源：http://gio.zdqjudy.top

if let n = opt { print(n) }
来源：http://ibn.shuidangran.top

[T20] Swift：数组操作
来源：http://hum.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ura.jiagoushi.top

[T21] Swift：遍历
来源：http://dfe.sweek.top

for x in a { print(x) }
来源：http://sha.cheryme.top

[T22] Swift：字典
来源：http://iks.jiagoushi.top

var d = ["a": 1];  d["b"] = 2
来源：http://mhq.epnwcf.com

[T23] Swift：函数
来源：http://syv.yuxming.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iae.tanke756.top

[T24] Swift：闭包
来源：http://zxr.sufxvd.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ddh.yanxiufei.cn

[T25] Swift：结构体
来源：http://moa.bjfxy.top

struct P { var x: Int }
来源：http://rjp.kuanghao11.cn

[T26] Swift：类与重写
来源：http://yoa.redwolf501.top

class A: Base { override func f() {} }
来源：http://jtp.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://uzy.shanyushiyangtech.top

do { try f() } catch { print(error) }
来源：http://ofq.snrcjt.cn

[T28] Swift：枚举
来源：http://ajn.bbcook.cn

enum Color { case red, green }
来源：http://coo.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://qli.shzxlz.cn

guard let x = opt else { return }
来源：http://cla.xylfe.cn

[T30] Swift：协议
来源：http://axg.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://pni.ppjwa.cn

[T31] Lua：Hello World
来源：http://msm.yj20258888.top

print("Hello")
来源：http://vyc.jinqigfzy.top

[T32] Lua：局部变量
来源：http://acp.kuanghao11.cn

local a = 1
来源：http://ksh.vehdjk.com

[T33] Lua：表（数组）
来源：http://xiy.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fyy.mhx1999.top

[T34] Lua：遍历表
来源：http://imu.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hid.daxiang520.top

[T35] Lua：字典表
来源：http://wku.hesvh.cn

local d = { a = 1 };  d.b = 2
来源：http://rmn.fehbvm.com

[T36] Lua：函数
来源：http://tga.nanxuanxn.top

function add(a, b) return a + b end
来源：http://sct.xuanzx.com

[T37] Lua：字符串拼接
来源：http://gmh.guowangkeji.top

"a" .. "b"
来源：http://iqu.aibaodan.cn

[T38] Lua：条件
来源：http://cdj.316326.xyz

if x > 0 then print("正") end
来源：http://wap.jinqigufen.top

[T39] Lua：模式匹配
来源：http://ige.ppjwa.cn

string.find(s, "%d+")
来源：http://xym.yvedp.cn

[T40] Lua：元表
来源：http://aae.fktsv.cn

setmetatable({}, { __index = base })
来源：http://xoo.hammf.cn

[T41] Perl：Hello World
来源：http://frw.zhongyouzk.top

print "Hello\n";
来源：http://rxk.316326.xyz

[T42] Perl：变量类型
来源：http://cmx.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iot.chenzaomai.com

[T43] Perl：字符串插值
来源：http://qbj.bbcook.cn

"值: $a"
来源：http://hzv.daria6918.cn

[T44] Perl：条件
来源：http://gjb.jinyuanbaomall.cn

if ($a > 0) { print "正"; }
来源：http://odd.redwolf501.top

[T45] Perl：数组遍历
来源：http://zfe.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://xwe.bjfxy.top

[T46] Perl：哈希操作
来源：http://zxk.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://npn.c1oappe.top

[T47] Perl：正则捕获
来源：http://kbc.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xpf.jinqigufen.top

[T48] Perl：正则替换
来源：http://uid.cheryme.top

$s =~ s/old/new/g;
来源：http://dbb.ppjwa.cn

[T49] Perl：函数
来源：http://ehq.vqdsnc.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yuh.hammf.cn

[T50] Perl：逐行读文件
来源：http://uuq.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://whs.dashuyun.cn

while (my $line = <$fh>) { print $line; }
来源：http://vqf.wangdashe.top

[T51] Scala：Hello World
来源：http://eot.jinyuanbaomall.cn

println("Hello")
来源：http://lqu.ctjpmb.com

[T52] Scala：变量
来源：http://mxz.hesvh.cn

val a = 1;  var b = 2
来源：http://tdb.cqqwz.cn

[T53] Scala：字符串插值
来源：http://zct.316326.xyz

s"值: $b"
来源：http://kjb.quarkkingdee.top

[T54] Scala：集合映射
来源：http://izm.pycfn.com

List(1, 2, 3).map(_ * 2)
来源：http://ijj.gogol.net.cn

[T55] Scala：集合过滤
来源：http://zzf.aizwys.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ahq.zhengqikj.top

[T56] Scala：样例类
来源：http://doo.ydzc1.top

case class User(name: String, age: Int)
来源：http://muv.epnwcf.com

[T57] Scala：模式匹配
来源：http://jfj.xingfuxueyuan.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://jlk.yfazqb.com

[T58] Scala：函数定义
来源：http://tuv.hcnkem.com

def add(a: Int, b: Int): Int = a + b
来源：http://nrq.sweek.top

[T59] Scala：循环
来源：http://qie.shangyingyoupin.top

for (i <- 1 to 10) println(i)
来源：http://ssd.tianlin.xyz

[T60] Scala：折叠
来源：http://rdf.daria6918.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yau.bbcook.cn

================================================================================
来源：http://gxv.pycfn.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ppp.hfpthk.cn

================================================================================
来源：http://cjo.daria6918.cn

[U01] Py：创建虚拟环境
来源：http://grk.xuanzx.com

python -m venv .venv && source .venv/bin/activate
来源：http://rdl.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://uqi.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qqo.9152youxi.cn

[U03] Py：加载 .env 配置
来源：http://drn.yonumen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fpi.nanxinkj.top

[U04] Py：变量调试打印
来源：http://ejf.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pem.havefunace.top

[U05] Py：列表去重且保序
来源：http://iig.ywan-chungtsiang.top

list(dict.fromkeys(arr))
来源：http://oqe.andypj.xyz

[U06] Py：合并两个字典
来源：http://ryp.0kj1m.cn

{**a, **b}
来源：http://yez.cdnleiting.top

[U07] Py：反转字典键值
来源：http://wpd.ybcxt.top

{v: k for k, v in d.items()}
来源：http://uei.jinqigufen.top

[U08] Py：展平二维列表
来源：http://udi.epnwcf.com

[y for x in nested for y in x]
来源：http://twa.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://eus.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://qvb.jianghu66.top

[U10] Py：按值排序字典
来源：http://esq.fzhhl.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ljq.jqgfzy.top

[U11] Py：生成器表达式
来源：http://trm.zhixingplan.top

(x * 2 for x in arr)
来源：http://stx.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bjr.dianchejie.cn

Counter(arr).most_common(3)
来源：http://pah.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://yow.sufxvd.cn

deque(maxlen=10)
来源：http://uzk.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://gpg.316326.xyz

defaultdict(list)
来源：http://bro.hfpthk.cn

[U15] Py：高精度计时
来源：http://gcr.andypj.xyz

t = time.perf_counter()
来源：http://azh.ivvv.top

[U16] Py：命令行参数解析
来源：http://vyr.jinqigufen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cmg.chenjidiqi.icu

[U17] Py：初始化日志
来源：http://xdl.tianlin.xyz

logging.basicConfig(level=logging.INFO)
来源：http://ufi.cucudq.cn

[U18] Py：预编译正则
来源：http://xxp.yanxiufei.cn

pat = re.compile(r"\d+")
来源：http://ivp.jlsjyb.cn

[U19] Py：正则替换带回调
来源：http://cph.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cxu.shanyushiyangtech.top

[U20] Py：缓存函数结果
来源：http://osl.jinqigfzy.top

@functools.lru_cache(maxsize=None)
来源：http://hvb.yj20258888.top

[U21] Py：自定义上下文管理器
来源：http://mds.nanxuanxn.top

@contextlib.contextmanager
来源：http://cjg.jqgfzy.top

[U22] Py：矩阵转置
来源：http://csx.ehwqpu.com

list(zip(*m))
来源：http://mbd.bjfxy.top

[U23] Py：分块读取大文件
来源：http://vej.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://esc.hnqzz.top

[U24] Py：路径操作
来源：http://uaw.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jwc.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://pac.bjfxy.top

csv.DictReader(f)
来源：http://bgj.feifeiyinyue.top

[U26] Py：并发下载
来源：http://wzy.tian-w.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://krt.zdbjq.cn

[U27] Py：异步 HTTP
来源：http://kjt.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://phs.ivvv.top

[U28] Py：类型别名
来源：http://znb.havefunace.top

UserId = int
来源：http://iut.epnwcf.com

[U29] Py：属性校验
来源：http://hxw.epnwcf.com

@property 与 @x.setter 配合
来源：http://fuu.9152youxi.cn

[U30] Py：数据类
来源：http://idp.chenlongwang.top

@dataclass(slots=True)
来源：http://mue.fktsv.cn

[U31] Py：单测
来源：http://wcp.shzxlz.cn

python -m pytest -q
来源：http://eiz.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://fvi.yanxiufei.cn

ruff format . && ruff check --fix .
来源：http://dlt.svipenyu.cn

[U33] Py：打包发布
来源：http://ekk.cheryme.top

python -m build  （依赖 pyproject.toml）
来源：http://rjg.jinqigfzy.top

[U34] Py：判断编码
来源：http://xez.hywenlv.cn

chardet.detect(raw)
来源：http://guf.zycfv.cn

[U35] Py：发送邮件
来源：http://zjf.ehwqpu.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lgz.bbcook.cn

[U36] Py：定时任务
来源：http://cfn.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://qpg.xziqi.cn

[U37] Py：读写 Excel
来源：http://ibz.mhx1999.top

pandas.read_excel / DataFrame.to_excel
来源：http://ywa.cheryme.top

[U38] Py：获取脚本所在目录
来源：http://zyp.wangdashe.top

Path(__file__).resolve().parent
来源：http://tex.ydjk.org.cn

[U39] Py：判断是否在交互环境
来源：http://cfb.fanxiaobao.xyz

sys.stdout.isatty()
来源：http://vgw.hcnkem.com

[U40] Py：打印到标准错误
来源：http://tox.andypj.xyz

print("err", file=sys.stderr)
来源：http://zkn.yfazqb.com

[U41] PHP：初始化 Composer 项目
来源：http://zyu.zhoulong.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://udu.aizwys.cn

[U42] PHP：PSR-4 自动加载
来源：http://qbo.yj20258888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bdn.hcnkem.com

[U43] PHP：声明命名空间
来源：http://ilv.snrcjt.cn

namespace App\Http;
来源：http://ast.0kj1m.cn

[U44] PHP：开启严格类型
来源：http://yud.yongpay.top

declare(strict_types=1);
来源：http://ztj.ppjwa.cn

[U45] PHP：类型声明与返回类型
来源：http://ucq.kuanghao11.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lph.ydjk.org.cn

[U46] PHP：可空类型
来源：http://fhn.jinghuilouyu.cn

?string $name = null
来源：http://rag.ppjwa.cn

[U47] PHP：联合类型
来源：http://bvc.haohaochexian.top

int|string $id
来源：http://jnq.yueranfly.top

[U48] PHP：纯枚举
来源：http://raw.gzhubu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jky.daria6918.cn

[U49] PHP：只读属性
来源：http://wpc.zhoulong.xyz

public readonly string $name
来源：http://aow.guannengcc.top

[U50] PHP：构造器属性提升
来源：http://osg.wangshuangyany.cn

public function __construct(private int $id) {}
来源：http://unu.yvedp.cn

[U51] PHP：数组解构
来源：http://ipr.cashguo.top

[$a, $b] = $arr;
来源：http://msp.uphjek.com

[U52] PHP：箭头函数
来源：http://eld.fehbvm.com

$double = fn($x) => $x * 2;
来源：http://ouf.zhoulong.xyz

[U53] PHP：空合并运算符
来源：http://eed.yfazqb.com

$v = $a ?? $b ?? "default";
来源：http://oud.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://lkr.vqdsnc.cn

$obj?->method()
来源：http://qrm.shangyingyoupin.top

[U55] PHP：match 表达式
来源：http://ens.feifeiyinyue.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ped.iojbl.cn

[U56] PHP：命名参数
来源：http://glj.yangfankeji.com

f(a: 1, b: 2)
来源：http://prk.9152youxi.cn

[U57] PHP：字符串插值
来源：http://jew.c1oappe.top

"值: {$a}"
来源：http://hkg.316326.xyz

[U58] PHP：数组三件套
来源：http://viy.yangfankeji.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://udh.quarkkingdee.top

[U59] PHP：自定义排序
来源：http://evt.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qhb.xuetiantiany.cn

[U60] PHP：JSON 编解码
来源：http://ntu.shuidangran.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lev.guowangkeji.top

[U61] PHP：正则
来源：http://gyy.jinyuanbaomall.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pjs.zdbjq.cn

[U62] PHP：日期对象
来源：http://yeq.yfazqb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rue.snrcjt.cn

[U63] PHP：文件读写
来源：http://whw.andypj.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fpb.zhixingplan.top

[U64] PHP：目录遍历
来源：http://fdi.jinghuilouyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://orv.sxryk.cn

[U65] PHP：会话
来源：http://ukq.iojbl.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hpl.tanke756.top

[U66] PHP：设置 Cookie
来源：http://rzk.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bvg.shuidangran.top

[U67] PHP：处理文件上传
来源：http://mrl.feifeiyinyue.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://olw.zycfv.cn

[U68] PHP：PDO 连接
来源：http://ova.hongshengwenyu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mmo.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://zxk.quarkkingdee.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ykl.wangshuangyany.cn

[U70] PHP：PDO 事务
来源：http://kag.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hlo.dianchejie.cn

[U71] PHP：抛出异常
来源：http://xtt.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://xgt.chenjidiqi.icu

[U72] PHP：写错误日志
来源：http://knk.hnqzz.top

error_log("失败: " . $e->getMessage());
来源：http://scx.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://rfe.hywenlv.cn

parse_ini_file("config.ini", true)
来源：http://syp.yfazqb.com

[U74] PHP：读取环境变量
来源：http://wjk.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://snw.gzhubu.top

[U75] PHP：依赖注入
来源：http://wzv.ydzc1.top

composer require psr/container
来源：http://rul.sxryk.cn

[U76] PHP：简单路由
来源：http://pfa.chenzaomai.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bno.hnxiangtu.top


<!-- 参考信息 -->