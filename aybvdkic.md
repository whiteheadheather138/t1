代发 wailian999

[S41] C++：类与构造函数
来源：http://ngt.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qbb.tian-w.cn

[S42] C++：继承与虚函数
来源：http://drm.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://ovn.ybcxt.top

[S43] C++：智能指针
来源：http://syd.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://jip.hammf.cn

[S44] C++：引用传参
来源：http://lft.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://icf.xuetiantiany.cn

[S45] C++：lambda
来源：http://whb.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://pac.ivvv.top

[S46] C++：函数模板
来源：http://grw.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pqj.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://dep.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xme.cdnleiting.top

[S48] C++：逐行读文件
来源：http://dgn.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://zyd.yj20258888.top

while (std::getline(in, line)) { }
来源：http://dxz.yvedp.cn

[S49] C++：写文件
来源：http://len.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bgq.cheryme.top

[S50] C++：格式化数字
来源：http://tbt.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iuv.xuanzx.com

[S51] C++：显式类型转换
来源：http://zuc.xylfe.cn

static_cast<double>(a) / b
来源：http://vmm.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://pyh.hammf.cn

int size() const noexcept { return n_; }
来源：http://nos.ivvv.top

[S53] C++：移动语义
来源：http://iio.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://acq.chenjidiqi.icu

[S54] C++：异常处理
来源：http://fwc.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ycp.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://mso.zhongyouzk.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zuu.xuanzx.com

[S56] C++：optional
来源：http://ojv.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wxg.andypj.xyz

[S57] C++：编译期常量
来源：http://oto.cheryme.top

constexpr int N = 10;
来源：http://ofu.cqqwz.cn

[S58] C++：命名空间
来源：http://kec.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://yjl.xziqi.cn

[S59] C++：静态断言
来源：http://mmg.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cwu.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://paq.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uzq.feifeiyinyue.top

================================================================================
来源：http://gks.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jmc.xingfuxueyuan.xyz

================================================================================
来源：http://dgt.yj202588.top

[T01] Kotlin：Hello World
来源：http://phr.meibo888.top

println("Hello")
来源：http://rko.ybcxt.top

[T02] Kotlin：变量
来源：http://ppt.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hwm.zdbjq.cn

[T03] Kotlin：字符串模板
来源：http://aci.ybcxt.top

"值: $b"
来源：http://vyz.ppjwa.cn

[T04] Kotlin：空安全
来源：http://qtx.epnwcf.com

val n: String? = null;  n?.length
来源：http://qrm.daxiang520.top

[T05] Kotlin：when 表达式
来源：http://moc.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dwn.fengsongda.top

[T06] Kotlin：集合映射
来源：http://dri.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vsy.xinyue.icu

[T07] Kotlin：集合过滤
来源：http://tst.yj202588.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wwn.aizwys.cn

[T08] Kotlin：数据类
来源：http://nln.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://gvh.gaohongyu789.top

[T09] Kotlin：扩展函数
来源：http://cjj.wangdashe.top

fun String.exclaim() = this + "!"
来源：http://xgs.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://neq.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zah.feifeiyinyue.top

[T11] Kotlin：协程
来源：http://eko.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fys.vqdsnc.cn

[T12] Kotlin：解构声明
来源：http://ozy.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://tyi.sweek.top

[T13] Kotlin：只读 Map
来源：http://tkc.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://nly.fktsv.cn

[T14] Kotlin：循环
来源：http://pgo.birdmap.top

for (i in 1..10) println(i)
来源：http://srv.fktsv.cn

[T15] Kotlin：接口
来源：http://jjr.quarkkingdee.top

interface Shape { fun area(): Double }
来源：http://xeh.aizwys.cn

[T16] Swift：Hello World
来源：http://msy.cheryme.top

print("Hello")
来源：http://wtj.jinqigufen.top

[T17] Swift：变量与常量
来源：http://hae.xziqi.cn

var a = 1;  let b = 2
来源：http://vjm.zdbjq.cn

[T18] Swift：字符串插值
来源：http://tus.pycfn.com

"值: \(b)"
来源：http://xjg.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://hoi.gaohongyu789.top

if let n = opt { print(n) }
来源：http://ewx.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://cxz.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://aal.pengpengdd.cyou

[T21] Swift：遍历
来源：http://flr.bjfxy.top

for x in a { print(x) }
来源：http://xub.bbcook.cn

[T22] Swift：字典
来源：http://utc.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://dzn.hongshengwenyu.top

[T23] Swift：函数
来源：http://opo.smart0.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blm.yanxiufei.cn

[T24] Swift：闭包
来源：http://whx.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://czj.dashuyun.cn

[T25] Swift：结构体
来源：http://wmm.fehbvm.com

struct P { var x: Int }
来源：http://oms.zhiwuduotai.top

[T26] Swift：类与重写
来源：http://iun.yueranfly.top

class A: Base { override func f() {} }
来源：http://qgw.dianchejie.cn

[T27] Swift：错误处理
来源：http://equ.ivvv.top

do { try f() } catch { print(error) }
来源：http://jvu.xinyue.icu

[T28] Swift：枚举
来源：http://guq.bbcook.cn

enum Color { case red, green }
来源：http://aym.cheryme.top

[T29] Swift：guard 提前返回
来源：http://zis.hcnkem.com

guard let x = opt else { return }
来源：http://tjv.zhijiandao.cn

[T30] Swift：协议
来源：http://cki.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://vgo.xuanzx.com

[T31] Lua：Hello World
来源：http://zqi.jinyuanbaomall.cn

print("Hello")
来源：http://maa.yonumen.top

[T32] Lua：局部变量
来源：http://jcg.hesvh.cn

local a = 1
来源：http://zhu.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://nts.ctjpmb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://bhk.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://jbb.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ghl.guannengcc.top

[T35] Lua：字典表
来源：http://jcw.yfazqb.com

local d = { a = 1 };  d.b = 2
来源：http://fio.xingfuxueyuan.xyz

[T36] Lua：函数
来源：http://xer.gaohongyu789.top

function add(a, b) return a + b end
来源：http://rdq.xziqi.cn

[T37] Lua：字符串拼接
来源：http://uke.cheryme.top

"a" .. "b"
来源：http://kse.chenlongwang.top

[T38] Lua：条件
来源：http://niy.quarkkingdee.top

if x > 0 then print("正") end
来源：http://eci.aibaodan.cn

[T39] Lua：模式匹配
来源：http://pqn.fengsongda.top

string.find(s, "%d+")
来源：http://the.jlsjyb.cn

[T40] Lua：元表
来源：http://dys.9152youxi.cn

setmetatable({}, { __index = base })
来源：http://vfz.tianlin.xyz

[T41] Perl：Hello World
来源：http://ray.ivvv.top

print "Hello\n";
来源：http://jih.xinyue.icu

[T42] Perl：变量类型
来源：http://ziw.guannengcc.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jnu.yvedp.cn

[T43] Perl：字符串插值
来源：http://sqq.ywan-chungtsiang.top

"值: $a"
来源：http://bpm.ctjpmb.com

[T44] Perl：条件
来源：http://gti.dashuyun.cn

if ($a > 0) { print "正"; }
来源：http://zqz.316326.xyz

[T45] Perl：数组遍历
来源：http://zbc.dashuyun.cn

for my $x (@arr) { print $x; }
来源：http://qua.wangshuangyany.cn

[T46] Perl：哈希操作
来源：http://obm.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xpo.ehwqpu.com

[T47] Perl：正则捕获
来源：http://lfy.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fzd.iojbl.cn

[T48] Perl：正则替换
来源：http://iqw.aibaodan.cn

$s =~ s/old/new/g;
来源：http://tmm.gogol.net.cn

[T49] Perl：函数
来源：http://clo.uphjek.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yjk.tarul.cn

[T50] Perl：逐行读文件
来源：http://czs.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ira.gotoacloud.top

while (my $line = <$fh>) { print $line; }
来源：http://bwj.yuanzhike.top

[T51] Scala：Hello World
来源：http://idh.xinyue.icu

println("Hello")
来源：http://wme.52xcode.cn

[T52] Scala：变量
来源：http://ovy.jinghuilouyu.cn

val a = 1;  var b = 2
来源：http://bhw.tianlin.xyz

[T53] Scala：字符串插值
来源：http://dzv.yuanzhike.top

s"值: $b"
来源：http://joq.jyoumei.cn

[T54] Scala：集合映射
来源：http://hwv.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://czb.tian-w.cn

[T55] Scala：集合过滤
来源：http://sah.yueranfly.top

List(1, 2, 3).filter(_ > 1)
来源：http://qte.yfazqb.com

[T56] Scala：样例类
来源：http://zct.cdnleiting.top

case class User(name: String, age: Int)
来源：http://acm.nanxinkj.top

[T57] Scala：模式匹配
来源：http://sbz.wangdashe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vae.xuanzx.com

[T58] Scala：函数定义
来源：http://pqh.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://vge.jqgfzy.top

[T59] Scala：循环
来源：http://cms.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://bke.shzxlz.cn

[T60] Scala：折叠
来源：http://cvv.ctjpmb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://owz.zhoulong.xyz

================================================================================
来源：http://vyj.yfazqb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ast.yonumen.top

================================================================================
来源：http://rrf.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://rfy.shuidangran.top

python -m venv .venv && source .venv/bin/activate
来源：http://nob.cdnleiting.top

[U02] Py：导出 / 安装依赖
来源：http://rva.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fjt.hywenlv.cn

[U03] Py：加载 .env 配置
来源：http://zkc.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://zaf.yongpay.top

[U04] Py：变量调试打印
来源：http://pro.fengsongda.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pcq.fzhhl.top

[U05] Py：列表去重且保序
来源：http://woy.sysykeji.top

list(dict.fromkeys(arr))
来源：http://vdm.yuanzhike.top

[U06] Py：合并两个字典
来源：http://hkn.snrcjt.cn

{**a, **b}
来源：http://eqi.zhoulong.xyz

[U07] Py：反转字典键值
来源：http://tnt.c1oappe.top

{v: k for k, v in d.items()}
来源：http://ujt.gzhubu.top

[U08] Py：展平二维列表
来源：http://tmt.tianlin.xyz

[y for x in nested for y in x]
来源：http://far.fehbvm.com

[U09] Py：字典取最大值的键
来源：http://kry.0kj1m.cn

max(d, key=d.get)
来源：http://oaq.ctjpmb.com

[U10] Py：按值排序字典
来源：http://haa.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://evb.ydzc1.top

[U11] Py：生成器表达式
来源：http://byn.yongpay.top

(x * 2 for x in arr)
来源：http://uhv.tianlin.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://ruw.ydjk.org.cn

Counter(arr).most_common(3)
来源：http://rlq.jyoumei.cn

[U13] Py：固定长度队列
来源：http://juo.daria6918.cn

deque(maxlen=10)
来源：http://jsc.sysykeji.top

[U14] Py：分组收集到列表
来源：http://fgj.iojbl.cn

defaultdict(list)
来源：http://olc.cucudq.cn

[U15] Py：高精度计时
来源：http://pzh.zhiwuduotai.top

t = time.perf_counter()
来源：http://evd.yongpay.top

[U16] Py：命令行参数解析
来源：http://ekh.fanxiaobao.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fue.hnxiangtu.top

[U17] Py：初始化日志
来源：http://vjc.svipenyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://cxt.chenzaomai.com

[U18] Py：预编译正则
来源：http://sbk.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://dny.shzxlz.cn

[U19] Py：正则替换带回调
来源：http://ysi.jyoumei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rgg.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://dyy.ctjpmb.com

@functools.lru_cache(maxsize=None)
来源：http://ypz.hcnkem.com

[U21] Py：自定义上下文管理器
来源：http://svu.havefunace.top

@contextlib.contextmanager
来源：http://gcf.kuanghao11.cn

[U22] Py：矩阵转置
来源：http://lst.hysaishi.cn

list(zip(*m))
来源：http://hrk.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://wao.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vch.sufxvd.cn

[U24] Py：路径操作
来源：http://grs.shuidangran.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wfu.tanke756.top

[U25] Py：CSV 按字典读
来源：http://edr.zycfv.cn

csv.DictReader(f)
来源：http://jhe.hammf.cn

[U26] Py：并发下载
来源：http://uot.hnqzz.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hiv.zhijiandao.cn

[U27] Py：异步 HTTP
来源：http://vkw.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://mnn.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://nqq.yonumen.top

UserId = int
来源：http://zxq.cashguo.top

[U29] Py：属性校验
来源：http://ecv.sweek.top

@property 与 @x.setter 配合
来源：http://dub.nanxuanxn.top

[U30] Py：数据类
来源：http://nrx.iojbl.cn

@dataclass(slots=True)
来源：http://xsz.jlsjyb.cn

[U31] Py：单测
来源：http://hkh.haohaochexian.top

python -m pytest -q
来源：http://ume.9152youxi.cn

[U32] Py：代码格式化
来源：http://zlh.tarul.cn

ruff format . && ruff check --fix .
来源：http://lcg.jyoumei.cn

[U33] Py：打包发布
来源：http://mdj.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://lcu.shangyingyoupin.top

[U34] Py：判断编码
来源：http://iyb.nanxinkj.top

chardet.detect(raw)
来源：http://ays.redwolf501.top

[U35] Py：发送邮件
来源：http://riz.gogol.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kji.cucudq.cn

[U36] Py：定时任务
来源：http://amu.hysaishi.cn

schedule.every(10).minutes.do(job)
来源：http://ejn.316326.xyz

[U37] Py：读写 Excel
来源：http://yhf.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://vwb.kuanghao11.cn

[U38] Py：获取脚本所在目录
来源：http://vyt.xinyue.icu

Path(__file__).resolve().parent
来源：http://oxz.shangyingyoupin.top

[U39] Py：判断是否在交互环境
来源：http://aya.sufxvd.cn

sys.stdout.isatty()
来源：http://ksx.guowangkeji.top

[U40] Py：打印到标准错误
来源：http://gby.uphjek.com

print("err", file=sys.stderr)
来源：http://gqp.yuanzhike.top

[U41] PHP：初始化 Composer 项目
来源：http://hip.meibo888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mhi.zhijiandao.cn

[U42] PHP：PSR-4 自动加载
来源：http://iey.smart0.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tqp.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://gwb.ywan-chungtsiang.top

namespace App\Http;
来源：http://hrb.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://mun.yangfankeji.com

declare(strict_types=1);
来源：http://gwm.fzhhl.top

[U45] PHP：类型声明与返回类型
来源：http://jai.yongpay.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vry.sweek.top

[U46] PHP：可空类型
来源：http://pkk.dashuyun.cn

?string $name = null
来源：http://odw.zhijiandao.cn

[U47] PHP：联合类型
来源：http://oez.snrcjt.cn

int|string $id
来源：http://gwr.epnwcf.com

[U48] PHP：纯枚举
来源：http://rfh.aibaodan.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rty.hammf.cn

[U49] PHP：只读属性
来源：http://qbl.sufxvd.cn

public readonly string $name
来源：http://rka.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://qsl.yuanzhike.top

public function __construct(private int $id) {}
来源：http://ayq.mhx1999.top

[U51] PHP：数组解构
来源：http://frv.shuidangran.top

[$a, $b] = $arr;
来源：http://ylz.bbcook.cn

[U52] PHP：箭头函数
来源：http://ull.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://qsx.jqgufenzy.top

[U53] PHP：空合并运算符
来源：http://bme.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://yna.yongpay.top

[U54] PHP：空安全调用
来源：http://dil.uphjek.com

$obj?->method()
来源：http://fdt.vehdjk.com

[U55] PHP：match 表达式
来源：http://gba.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gqn.chenlongwang.top

[U56] PHP：命名参数
来源：http://wps.yj20258888.top

f(a: 1, b: 2)
来源：http://tkv.jlsjyb.cn

[U57] PHP：字符串插值
来源：http://ika.guannengcc.top

"值: {$a}"
来源：http://dba.shanyushiyangkeji.top

[U58] PHP：数组三件套
来源：http://rzq.sysykeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aym.cucudq.cn

[U59] PHP：自定义排序
来源：http://lwz.shangyingyoupin.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hsl.dashuyun.cn

[U60] PHP：JSON 编解码
来源：http://xca.aibaodan.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bbi.svipenyu.cn

[U61] PHP：正则
来源：http://kru.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://coj.zhijiandao.cn

[U62] PHP：日期对象
来源：http://gam.kuanghao11.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zfi.zdbjq.cn

[U63] PHP：文件读写
来源：http://aor.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gcg.sxryk.cn

[U64] PHP：目录遍历
来源：http://eux.birdmap.top

glob("dir/*.php");  scandir("dir");
来源：http://jdv.yuxming.cn

[U65] PHP：会话
来源：http://gqa.yongpay.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rtt.nwbrower.top

[U66] PHP：设置 Cookie
来源：http://rds.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gkb.xylfe.cn


<!-- 参考信息 -->