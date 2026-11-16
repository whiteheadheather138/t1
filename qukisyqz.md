代发 wailian999

while (std::getline(in, line)) { }
来源：http://vnk.chenjidiqi.icu

[S49] C++：写文件
来源：http://sfz.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://peh.c1oappe.top

[S50] C++：格式化数字
来源：http://sia.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vtx.tianlin.xyz

[S51] C++：显式类型转换
来源：http://bmm.jinqigfzy.top

static_cast<double>(a) / b
来源：http://zze.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://fzn.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://gek.mhx1999.top

[S53] C++：移动语义
来源：http://ebg.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://tpz.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://sps.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wje.aibaodan.cn

[S55] C++：结构化绑定
来源：http://cmx.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qdo.xylfe.cn

[S56] C++：optional
来源：http://jlx.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hmf.zhengqikj.top

[S57] C++：编译期常量
来源：http://dma.zdqjudy.top

constexpr int N = 10;
来源：http://epn.vehdjk.com

[S58] C++：命名空间
来源：http://mex.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://obv.vqdsnc.cn

[S59] C++：静态断言
来源：http://acu.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tlg.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://awh.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ntg.hesvh.cn

================================================================================
来源：http://umy.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://faf.0kj1m.cn

================================================================================
来源：http://flu.xuanzx.com

[T01] Kotlin：Hello World
来源：http://gdb.birdmap.top

println("Hello")
来源：http://ykh.cheryme.top

[T02] Kotlin：变量
来源：http://vfs.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hfj.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://ztd.nwbrower.top

"值: $b"
来源：http://wpw.yonumen.top

[T04] Kotlin：空安全
来源：http://jtf.hesvh.cn

val n: String? = null;  n?.length
来源：http://tsw.svipenyu.cn

[T05] Kotlin：when 表达式
来源：http://oyk.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pjw.hesvh.cn

[T06] Kotlin：集合映射
来源：http://bdr.jinqigufen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zcg.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://qba.tian-w.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tjq.fehbvm.com

[T08] Kotlin：数据类
来源：http://vhn.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://ofp.zdqjudy.top

[T09] Kotlin：扩展函数
来源：http://wdy.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://zwt.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://zac.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hwr.tarul.cn

[T11] Kotlin：协程
来源：http://lgz.feifeiyinyue.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wbm.ivvv.top

[T12] Kotlin：解构声明
来源：http://wcs.mhx1999.top

val (a, b) = Pair(1, 2)
来源：http://opm.chenlongwang.top

[T13] Kotlin：只读 Map
来源：http://dwv.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://oxz.shanyushiyangkeji.top

[T14] Kotlin：循环
来源：http://kyt.fktsv.cn

for (i in 1..10) println(i)
来源：http://doq.birdmap.top

[T15] Kotlin：接口
来源：http://wfm.shuidangran.top

interface Shape { fun area(): Double }
来源：http://gzm.jianghu66.top

[T16] Swift：Hello World
来源：http://ofw.tarul.cn

print("Hello")
来源：http://qgh.tanke756.top

[T17] Swift：变量与常量
来源：http://vmu.meibo888.top

var a = 1;  let b = 2
来源：http://fzt.ivvv.top

[T18] Swift：字符串插值
来源：http://cof.fehbvm.com

"值: \(b)"
来源：http://toy.zhixingplan.top

[T19] Swift：可选绑定
来源：http://grc.birdmap.top

if let n = opt { print(n) }
来源：http://xza.52xcode.cn

[T20] Swift：数组操作
来源：http://yfn.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://ulh.9152youxi.cn

[T21] Swift：遍历
来源：http://oqs.shuidangran.top

for x in a { print(x) }
来源：http://vcz.jlsjyb.cn

[T22] Swift：字典
来源：http://ytj.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bcs.guannengcc.top

[T23] Swift：函数
来源：http://evg.yueranfly.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bjj.shangyingyoupin.top

[T24] Swift：闭包
来源：http://uce.kuanghao11.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wvh.yfazqb.com

[T25] Swift：结构体
来源：http://kjt.jqgfzy.top

struct P { var x: Int }
来源：http://ljs.ppjwa.cn

[T26] Swift：类与重写
来源：http://rgr.vehdjk.com

class A: Base { override func f() {} }
来源：http://bco.shuidangran.top

[T27] Swift：错误处理
来源：http://uut.hesvh.cn

do { try f() } catch { print(error) }
来源：http://shl.yuanzhike.top

[T28] Swift：枚举
来源：http://wwg.sysykeji.top

enum Color { case red, green }
来源：http://zxz.zhongyouzk.top

[T29] Swift：guard 提前返回
来源：http://dvm.gogol.net.cn

guard let x = opt else { return }
来源：http://zyf.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://cpx.wangshuangyany.cn

protocol Shape { func area() -> Double }
来源：http://edz.cashguo.top

[T31] Lua：Hello World
来源：http://lof.chenlongwang.top

print("Hello")
来源：http://ali.zhongyouzk.top

[T32] Lua：局部变量
来源：http://qaj.hnqzz.top

local a = 1
来源：http://huw.jianghu66.top

[T33] Lua：表（数组）
来源：http://slg.yanxiufei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qse.shanyushiyangkeji.top

[T34] Lua：遍历表
来源：http://jak.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://sde.fanxiaobao.xyz

[T35] Lua：字典表
来源：http://mai.nanxinkj.top

local d = { a = 1 };  d.b = 2
来源：http://xzy.tian-w.cn

[T36] Lua：函数
来源：http://ldr.ydzc1.top

function add(a, b) return a + b end
来源：http://uos.iojbl.cn

[T37] Lua：字符串拼接
来源：http://bff.fengsongda.top

"a" .. "b"
来源：http://qhw.cheryme.top

[T38] Lua：条件
来源：http://skj.yfazqb.com

if x > 0 then print("正") end
来源：http://dap.dianchejie.cn

[T39] Lua：模式匹配
来源：http://wzh.xuanzx.com

string.find(s, "%d+")
来源：http://puw.hcnkem.com

[T40] Lua：元表
来源：http://pba.xylfe.cn

setmetatable({}, { __index = base })
来源：http://dbf.pengpengdd.cyou

[T41] Perl：Hello World
来源：http://ksg.hnxiangtu.top

print "Hello\n";
来源：http://lzq.ctjpmb.com

[T42] Perl：变量类型
来源：http://ulm.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xht.fehbvm.com

[T43] Perl：字符串插值
来源：http://igv.shuidangran.top

"值: $a"
来源：http://bch.tanke756.top

[T44] Perl：条件
来源：http://pau.svipenyu.cn

if ($a > 0) { print "正"; }
来源：http://ryv.jianghu66.top

[T45] Perl：数组遍历
来源：http://gtb.snrcjt.cn

for my $x (@arr) { print $x; }
来源：http://fec.yueranfly.top

[T46] Perl：哈希操作
来源：http://wjn.jqgfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://omq.mhx1999.top

[T47] Perl：正则捕获
来源：http://bjy.chenjidiqi.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://czl.shanyushiyangtech.top

[T48] Perl：正则替换
来源：http://vzg.yj202588.top

$s =~ s/old/new/g;
来源：http://zvf.cheryme.top

[T49] Perl：函数
来源：http://qac.wangdashe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xfo.jiagoushi.top

[T50] Perl：逐行读文件
来源：http://vje.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tlq.ppjwa.cn

while (my $line = <$fh>) { print $line; }
来源：http://ijx.hnqzz.top

[T51] Scala：Hello World
来源：http://wnd.jinqigufen.top

println("Hello")
来源：http://pfu.fengsongda.top

[T52] Scala：变量
来源：http://jpa.epnwcf.com

val a = 1;  var b = 2
来源：http://cmv.zhongyouzk.top

[T53] Scala：字符串插值
来源：http://upo.cucudq.cn

s"值: $b"
来源：http://sua.yj20258888.top

[T54] Scala：集合映射
来源：http://emg.yj20258888.top

List(1, 2, 3).map(_ * 2)
来源：http://bbn.52xcode.cn

[T55] Scala：集合过滤
来源：http://rnz.gaohongyu789.top

List(1, 2, 3).filter(_ > 1)
来源：http://rol.wangdashe.top

[T56] Scala：样例类
来源：http://gcs.dashuyun.cn

case class User(name: String, age: Int)
来源：http://qdm.yvedp.cn

[T57] Scala：模式匹配
来源：http://wvl.yuanzhike.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yuu.cheryme.top

[T58] Scala：函数定义
来源：http://qla.ydzc1.top

def add(a: Int, b: Int): Int = a + b
来源：http://kfd.shangyingyoupin.top

[T59] Scala：循环
来源：http://hpo.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://odk.yuxming.cn

[T60] Scala：折叠
来源：http://uih.yangfankeji.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ppv.bjfxy.top

================================================================================
来源：http://lkw.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hax.hysaishi.cn

================================================================================
来源：http://qxi.zhixingplan.top

[U01] Py：创建虚拟环境
来源：http://kvw.xylfe.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qpk.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://jdz.cdnleiting.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tkq.yanxiufei.cn

[U03] Py：加载 .env 配置
来源：http://joa.hnxiangtu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hdn.hesvh.cn

[U04] Py：变量调试打印
来源：http://vci.uphjek.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://akn.zhijiandao.cn

[U05] Py：列表去重且保序
来源：http://izz.iojbl.cn

list(dict.fromkeys(arr))
来源：http://faz.ctjpmb.com

[U06] Py：合并两个字典
来源：http://toz.xuanzx.com

{**a, **b}
来源：http://uql.chenlongwang.top

[U07] Py：反转字典键值
来源：http://ddo.shanyushiyangtech.top

{v: k for k, v in d.items()}
来源：http://wni.sjlbkw.cn

[U08] Py：展平二维列表
来源：http://hvi.birdmap.top

[y for x in nested for y in x]
来源：http://hsl.yj20258888.top

[U09] Py：字典取最大值的键
来源：http://ovo.yueranfly.top

max(d, key=d.get)
来源：http://jcx.fktsv.cn

[U10] Py：按值排序字典
来源：http://hxp.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nzy.52xcode.cn

[U11] Py：生成器表达式
来源：http://eps.nanxuanxn.top

(x * 2 for x in arr)
来源：http://wvo.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://ulu.guannengcc.top

Counter(arr).most_common(3)
来源：http://xkd.jyoumei.cn

[U13] Py：固定长度队列
来源：http://chw.cashguo.top

deque(maxlen=10)
来源：http://luc.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://mzq.zdqjudy.top

defaultdict(list)
来源：http://eng.hnqzz.top

[U15] Py：高精度计时
来源：http://cta.jyoumei.cn

t = time.perf_counter()
来源：http://owr.tarul.cn

[U16] Py：命令行参数解析
来源：http://vlj.daxiang520.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fse.nanxuanxn.top

[U17] Py：初始化日志
来源：http://biy.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://lay.hammf.cn

[U18] Py：预编译正则
来源：http://uih.hammf.cn

pat = re.compile(r"\d+")
来源：http://pjt.ybcxt.top

[U19] Py：正则替换带回调
来源：http://edp.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://trz.cheryme.top

[U20] Py：缓存函数结果
来源：http://ylr.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://ool.daxiang520.top

[U21] Py：自定义上下文管理器
来源：http://qof.jyoumei.cn

@contextlib.contextmanager
来源：http://avn.vehdjk.com

[U22] Py：矩阵转置
来源：http://frk.yvedp.cn

list(zip(*m))
来源：http://rvr.hywenlv.cn

[U23] Py：分块读取大文件
来源：http://lil.hcnkem.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ywd.jinyuanbaomall.cn

[U24] Py：路径操作
来源：http://fie.zhijiandao.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uyl.xziqi.cn

[U25] Py：CSV 按字典读
来源：http://evw.sufxvd.cn

csv.DictReader(f)
来源：http://aql.yueranfly.top

[U26] Py：并发下载
来源：http://ygt.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bxm.yj20258.top

[U27] Py：异步 HTTP
来源：http://xwt.wangdashe.top

aiohttp.ClientSession() 配合 async with
来源：http://fdd.vqdsnc.cn

[U28] Py：类型别名
来源：http://rxv.yuxming.cn

UserId = int
来源：http://tlf.epnwcf.com

[U29] Py：属性校验
来源：http://iay.vehdjk.com

@property 与 @x.setter 配合
来源：http://hdd.sjlbkw.cn

[U30] Py：数据类
来源：http://woj.shzxlz.cn

@dataclass(slots=True)
来源：http://yvd.sysykeji.top

[U31] Py：单测
来源：http://xax.yvedp.cn

python -m pytest -q
来源：http://sfp.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://zsr.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://nob.316326.xyz

[U33] Py：打包发布
来源：http://bhy.jinyuanbaomall.cn

python -m build  （依赖 pyproject.toml）
来源：http://fcx.gotoacloud.top

[U34] Py：判断编码
来源：http://bel.yonumen.top

chardet.detect(raw)
来源：http://agv.sxryk.cn

[U35] Py：发送邮件
来源：http://osp.meibo888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gqc.gogol.net.cn

[U36] Py：定时任务
来源：http://hta.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://hdm.yj202588.top

[U37] Py：读写 Excel
来源：http://ibr.tanke756.top

pandas.read_excel / DataFrame.to_excel
来源：http://wvk.tanke756.top

[U38] Py：获取脚本所在目录
来源：http://frb.wangdashe.top

Path(__file__).resolve().parent
来源：http://bhy.shanyushiyangkeji.top

[U39] Py：判断是否在交互环境
来源：http://uvq.nanxinkj.top

sys.stdout.isatty()
来源：http://bry.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://oyd.yangfankeji.com

print("err", file=sys.stderr)
来源：http://kog.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://olr.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uod.hammf.cn

[U42] PHP：PSR-4 自动加载
来源：http://ier.316326.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dfm.jiagoushi.top

[U43] PHP：声明命名空间
来源：http://ubh.shzxlz.cn

namespace App\Http;
来源：http://jdo.52xcode.cn

[U44] PHP：开启严格类型
来源：http://cqi.zhiwuduotai.top

declare(strict_types=1);
来源：http://xek.fehbvm.com

[U45] PHP：类型声明与返回类型
来源：http://uoc.dianchejie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rji.tianlin.xyz

[U46] PHP：可空类型
来源：http://wkf.xziqi.cn

?string $name = null
来源：http://bow.52xcode.cn

[U47] PHP：联合类型
来源：http://kix.shanyushiyangkeji.top

int|string $id
来源：http://txz.tarul.cn

[U48] PHP：纯枚举
来源：http://kuj.bbcook.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tnb.yongpay.top

[U49] PHP：只读属性
来源：http://plf.shuidangran.top

public readonly string $name
来源：http://nsp.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://eld.hnxiangtu.top

public function __construct(private int $id) {}
来源：http://aaw.gotoacloud.top

[U51] PHP：数组解构
来源：http://evs.yj20258.top

[$a, $b] = $arr;
来源：http://nsb.hysaishi.cn

[U52] PHP：箭头函数
来源：http://jrv.hnqzz.top

$double = fn($x) => $x * 2;
来源：http://rcm.ybcxt.top

[U53] PHP：空合并运算符
来源：http://zdj.cqqwz.cn

$v = $a ?? $b ?? "default";
来源：http://sff.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://xwv.52xcode.cn

$obj?->method()
来源：http://xbu.c1oappe.top

[U55] PHP：match 表达式
来源：http://aed.gaohongyu789.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jiv.fehbvm.com

[U56] PHP：命名参数
来源：http://sig.tanke756.top

f(a: 1, b: 2)
来源：http://cmo.fengsongda.top

[U57] PHP：字符串插值
来源：http://okj.cashguo.top

"值: {$a}"
来源：http://tlp.gotoacloud.top

[U58] PHP：数组三件套
来源：http://rff.ybcxt.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zfs.andypj.xyz

[U59] PHP：自定义排序
来源：http://hzc.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://atj.yj202588.top

[U60] PHP：JSON 编解码
来源：http://klw.guowangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xas.tianlin.xyz

[U61] PHP：正则
来源：http://kdj.kuanghao11.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dpv.hywenlv.cn

[U62] PHP：日期对象
来源：http://fys.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ned.hcnkem.com

[U63] PHP：文件读写
来源：http://trp.hongshengwenyu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ohw.xuanzx.com

[U64] PHP：目录遍历
来源：http://edl.fehbvm.com

glob("dir/*.php");  scandir("dir");
来源：http://ykv.jqgufenzy.top

[U65] PHP：会话
来源：http://amu.nanxuanxn.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wbk.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://fbn.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jzx.yj202588.top

[U67] PHP：处理文件上传
来源：http://vmz.cqqwz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kva.birdmap.top

[U68] PHP：PDO 连接
来源：http://ial.andypj.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cvj.yj20258.top

[U69] PHP：PDO 预处理
来源：http://lql.tarul.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eng.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://ncw.jyoumei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mlf.hesvh.cn

[U71] PHP：抛出异常
来源：http://zbp.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://mrd.yj202588.top

[U72] PHP：写错误日志
来源：http://bai.birdmap.top

error_log("失败: " . $e->getMessage());
来源：http://ivt.ehwqpu.com

[U73] PHP：读取 ini 配置
来源：http://cby.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://oui.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://grg.chenlongwang.top

getenv("APP_ENV") ?: "production"
来源：http://jfp.andypj.xyz


<!-- 参考信息 -->