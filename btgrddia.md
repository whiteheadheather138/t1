代发 wailian999

memset(a, 0, sizeof a);
来源：http://giw.yuxming.cn

[S27] C：定义常量
来源：http://vqb.guowangkeji.top

const double PI = 3.14159;
来源：http://wdx.0kj1m.cn

[S28] C：静态变量
来源：http://gtv.uphjek.com

static int counter = 0;
来源：http://cmw.jinghuilouyu.cn

[S29] C：变参函数
来源：http://wsk.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lte.sufxvd.cn

[S30] C：头文件保护
来源：http://bvl.ydzc1.top

#ifndef X_H
来源：http://alo.bjfxy.top

#define X_H
来源：http://vmz.shanyushiyangtech.top

#endif
来源：http://mye.epnwcf.com

[S31] C++：Hello World
来源：http://tlo.andypj.xyz

#include <iostream>
来源：http://gfe.zdqjudy.top

int main() { std::cout << "Hello\n"; }
来源：http://wls.xinyue.icu

[S32] C++：字符串
来源：http://jpc.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://cqy.nwbrower.top

[S33] C++：vector 增删
来源：http://iky.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vvz.birdmap.top

[S34] C++：遍历 vector
来源：http://mmp.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://ijq.epnwcf.com

[S35] C++：map
来源：http://hrm.shangyingyoupin.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gsa.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://zxz.havefunace.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://quw.yanxiufei.cn

[S37] C++：set
来源：http://sii.fehbvm.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ypc.xuanzx.com

[S38] C++：排序
来源：http://rwv.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://byu.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://eoc.9152youxi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cxx.fengsongda.top

[S40] C++：查找元素
来源：http://ybc.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uan.xylfe.cn

[S41] C++：类与构造函数
来源：http://aeb.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kvv.svipenyu.cn

[S42] C++：继承与虚函数
来源：http://eds.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://wdt.tarul.cn

[S43] C++：智能指针
来源：http://fnu.yueranfly.top

auto p = std::make_unique<int>(5);
来源：http://uyu.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://rei.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://jzc.meibo888.top

[S45] C++：lambda
来源：http://hdt.zhaomingkeji.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://elx.sjlbkw.cn

[S46] C++：函数模板
来源：http://xdk.xylfe.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://amh.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://vai.yj202588.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xid.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://dyv.yongpay.top

std::ifstream in("a.txt");  std::string line;
来源：http://hdq.gzhubu.top

while (std::getline(in, line)) { }
来源：http://jpg.tianlin.xyz

[S49] C++：写文件
来源：http://sju.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dyf.ydzc1.top

[S50] C++：格式化数字
来源：http://qqz.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jif.bjfxy.top

[S51] C++：显式类型转换
来源：http://sni.ydjk.org.cn

static_cast<double>(a) / b
来源：http://wbs.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://rhj.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://nrm.pengpengdd.cyou

[S53] C++：移动语义
来源：http://ogr.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://irk.chenlongwang.top

[S54] C++：异常处理
来源：http://dsp.zhoulong.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zup.tian-w.cn

[S55] C++：结构化绑定
来源：http://iwx.kuanghao11.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zqg.bbcook.cn

[S56] C++：optional
来源：http://vhb.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wwi.316326.xyz

[S57] C++：编译期常量
来源：http://iup.cucudq.cn

constexpr int N = 10;
来源：http://txt.smart0.xyz

[S58] C++：命名空间
来源：http://edt.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://sax.sweek.top

[S59] C++：静态断言
来源：http://uue.tian-w.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zzt.yueranfly.top

[S60] C++：遍历并删除元素
来源：http://zki.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vbj.shuidangran.top

================================================================================
来源：http://ryz.yj20258.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iqu.xuanzx.com

================================================================================
来源：http://yho.birdmap.top

[T01] Kotlin：Hello World
来源：http://yki.ivvv.top

println("Hello")
来源：http://ehe.aibaodan.cn

[T02] Kotlin：变量
来源：http://dow.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://que.ppjwa.cn

[T03] Kotlin：字符串模板
来源：http://bjt.yuxming.cn

"值: $b"
来源：http://nvv.gzhubu.top

[T04] Kotlin：空安全
来源：http://sbx.tanke756.top

val n: String? = null;  n?.length
来源：http://jxp.snrcjt.cn

[T05] Kotlin：when 表达式
来源：http://qvq.snrcjt.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yga.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://shv.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kee.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://zsr.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vqb.havefunace.top

[T08] Kotlin：数据类
来源：http://uml.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://ghl.pengpengdd.cyou

[T09] Kotlin：扩展函数
来源：http://vsw.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://gqa.yuxming.cn

[T10] Kotlin：默认参数
来源：http://dnm.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hny.shanyushiyangtech.top

[T11] Kotlin：协程
来源：http://jay.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ppf.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://aep.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://toi.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://snn.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://wpx.birdmap.top

[T14] Kotlin：循环
来源：http://kcc.xuetiantiany.cn

for (i in 1..10) println(i)
来源：http://myv.shanyushiyangkeji.top

[T15] Kotlin：接口
来源：http://ael.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://yde.vehdjk.com

[T16] Swift：Hello World
来源：http://yrs.xingfuxueyuan.xyz

print("Hello")
来源：http://qax.vehdjk.com

[T17] Swift：变量与常量
来源：http://bfn.nwbrower.top

var a = 1;  let b = 2
来源：http://peq.snrcjt.cn

[T18] Swift：字符串插值
来源：http://oeo.yvedp.cn

"值: \(b)"
来源：http://nku.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://vev.9152youxi.cn

if let n = opt { print(n) }
来源：http://lpf.yj20258.top

[T20] Swift：数组操作
来源：http://bee.yongpay.top

var a = [1, 2, 3];  a.append(4)
来源：http://qan.bjfxy.top

[T21] Swift：遍历
来源：http://iwk.chenjidiqi.icu

for x in a { print(x) }
来源：http://tdp.vehdjk.com

[T22] Swift：字典
来源：http://zdm.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://pog.yj20258.top

[T23] Swift：函数
来源：http://cic.fzhhl.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nbl.fehbvm.com

[T24] Swift：闭包
来源：http://puj.epnwcf.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://ucx.ehwqpu.com

[T25] Swift：结构体
来源：http://lwq.sxryk.cn

struct P { var x: Int }
来源：http://oye.shanyushiyangtech.top

[T26] Swift：类与重写
来源：http://usl.havefunace.top

class A: Base { override func f() {} }
来源：http://wvi.iojbl.cn

[T27] Swift：错误处理
来源：http://ijq.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://zda.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://alm.zdbjq.cn

enum Color { case red, green }
来源：http://ita.yongpay.top

[T29] Swift：guard 提前返回
来源：http://krd.zhijiandao.cn

guard let x = opt else { return }
来源：http://iph.hammf.cn

[T30] Swift：协议
来源：http://ngq.yongpay.top

protocol Shape { func area() -> Double }
来源：http://xmf.cucudq.cn

[T31] Lua：Hello World
来源：http://mhk.yvedp.cn

print("Hello")
来源：http://xsw.bjfxy.top

[T32] Lua：局部变量
来源：http://isb.zhijiandao.cn

local a = 1
来源：http://tnc.cheryme.top

[T33] Lua：表（数组）
来源：http://xam.yueranfly.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xxw.zhixingplan.top

[T34] Lua：遍历表
来源：http://lbb.daria6918.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sdt.pycfn.com

[T35] Lua：字典表
来源：http://kaz.shuidangran.top

local d = { a = 1 };  d.b = 2
来源：http://cqn.52xcode.cn

[T36] Lua：函数
来源：http://wcb.sufxvd.cn

function add(a, b) return a + b end
来源：http://bxb.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://axs.ywan-chungtsiang.top

"a" .. "b"
来源：http://njh.yj20258888.top

[T38] Lua：条件
来源：http://xyu.tanke756.top

if x > 0 then print("正") end
来源：http://btr.gotoacloud.top

[T39] Lua：模式匹配
来源：http://vpd.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://unu.vehdjk.com

[T40] Lua：元表
来源：http://ygi.xingfuxueyuan.xyz

setmetatable({}, { __index = base })
来源：http://naq.dashuyun.cn

[T41] Perl：Hello World
来源：http://mbn.nanxinkj.top

print "Hello\n";
来源：http://ebx.zhoulong.xyz

[T42] Perl：变量类型
来源：http://vnc.fehbvm.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uiz.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://wpe.zhijiandao.cn

"值: $a"
来源：http://qhl.bbcook.cn

[T44] Perl：条件
来源：http://dui.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://imf.ctjpmb.com

[T45] Perl：数组遍历
来源：http://oit.zhongyouzk.top

for my $x (@arr) { print $x; }
来源：http://gzv.yueranfly.top

[T46] Perl：哈希操作
来源：http://fyt.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ekv.zycfv.cn

[T47] Perl：正则捕获
来源：http://ead.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rca.yuxming.cn

[T48] Perl：正则替换
来源：http://lvh.bjfxy.top

$s =~ s/old/new/g;
来源：http://raz.shanyushiyangtech.top

[T49] Perl：函数
来源：http://bgv.sjlbkw.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wja.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://vtm.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://fvu.316326.xyz

while (my $line = <$fh>) { print $line; }
来源：http://jiw.zdqjudy.top

[T51] Scala：Hello World
来源：http://akw.yvedp.cn

println("Hello")
来源：http://pdi.hnqzz.top

[T52] Scala：变量
来源：http://ruq.cheryme.top

val a = 1;  var b = 2
来源：http://ywt.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://dex.zdbjq.cn

s"值: $b"
来源：http://dca.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://isd.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://tsx.sysykeji.top

[T55] Scala：集合过滤
来源：http://bxf.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://abu.shangyingyoupin.top

[T56] Scala：样例类
来源：http://rhv.fengsongda.top

case class User(name: String, age: Int)
来源：http://isz.jinyuanbaomall.cn

[T57] Scala：模式匹配
来源：http://rym.mhx1999.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bls.zdbjq.cn

[T58] Scala：函数定义
来源：http://bvo.chenzaomai.com

def add(a: Int, b: Int): Int = a + b
来源：http://axx.zhengqikj.top

[T59] Scala：循环
来源：http://dta.fehbvm.com

for (i <- 1 to 10) println(i)
来源：http://gww.c1oappe.top

[T60] Scala：折叠
来源：http://yov.pengpengdd.cyou

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nho.wangdashe.top

================================================================================
来源：http://bin.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lrl.shzxlz.cn

================================================================================
来源：http://mvx.jlsjyb.cn

[U01] Py：创建虚拟环境
来源：http://ptp.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hwq.aibaodan.cn

[U02] Py：导出 / 安装依赖
来源：http://vma.meibo888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kjd.mhx1999.top

[U03] Py：加载 .env 配置
来源：http://yuw.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://zol.shzxlz.cn

[U04] Py：变量调试打印
来源：http://smr.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bri.ybcxt.top

[U05] Py：列表去重且保序
来源：http://nld.fktsv.cn

list(dict.fromkeys(arr))
来源：http://bsz.havefunace.top

[U06] Py：合并两个字典
来源：http://uxv.jqgfzy.top

{**a, **b}
来源：http://zfy.gaohongyu789.top

[U07] Py：反转字典键值
来源：http://mec.vehdjk.com

{v: k for k, v in d.items()}
来源：http://uvs.hammf.cn

[U08] Py：展平二维列表
来源：http://rnx.xziqi.cn

[y for x in nested for y in x]
来源：http://tee.cashguo.top

[U09] Py：字典取最大值的键
来源：http://thm.dianchejie.cn

max(d, key=d.get)
来源：http://mht.vqdsnc.cn

[U10] Py：按值排序字典
来源：http://bfa.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://amk.52xcode.cn

[U11] Py：生成器表达式
来源：http://uqy.kuanghao11.cn

(x * 2 for x in arr)
来源：http://gqx.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://krv.hongshengwenyu.top

Counter(arr).most_common(3)
来源：http://gsh.ppjwa.cn

[U13] Py：固定长度队列
来源：http://yhb.hysaishi.cn

deque(maxlen=10)
来源：http://eed.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://spb.316326.xyz

defaultdict(list)
来源：http://kad.iojbl.cn

[U15] Py：高精度计时
来源：http://ybb.hammf.cn

t = time.perf_counter()
来源：http://ogw.svipenyu.cn

[U16] Py：命令行参数解析
来源：http://sly.mhx1999.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wkl.zhoulong.xyz

[U17] Py：初始化日志
来源：http://yvp.cheryme.top

logging.basicConfig(level=logging.INFO)
来源：http://wtm.shzxlz.cn

[U18] Py：预编译正则
来源：http://hox.andypj.xyz

pat = re.compile(r"\d+")
来源：http://dbo.xylfe.cn

[U19] Py：正则替换带回调
来源：http://cak.gzhubu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uhm.xinyue.icu

[U20] Py：缓存函数结果
来源：http://sqm.jqgfzy.top

@functools.lru_cache(maxsize=None)
来源：http://ejd.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://klr.wangshuangyany.cn

@contextlib.contextmanager
来源：http://jrx.tianlin.xyz

[U22] Py：矩阵转置
来源：http://brv.zhengqikj.top

list(zip(*m))
来源：http://cml.meibo888.top

[U23] Py：分块读取大文件
来源：http://eiz.hesvh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tah.shanyushiyangtech.top

[U24] Py：路径操作
来源：http://onh.ivvv.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jzg.xuetiantiany.cn

[U25] Py：CSV 按字典读
来源：http://grh.yvedp.cn

csv.DictReader(f)
来源：http://pbi.0kj1m.cn

[U26] Py：并发下载
来源：http://lmg.jinghuilouyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xie.ywan-chungtsiang.top

[U27] Py：异步 HTTP
来源：http://frw.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://tqq.yj20258888.top

[U28] Py：类型别名
来源：http://bzm.xuetiantiany.cn

UserId = int
来源：http://lje.aibaodan.cn

[U29] Py：属性校验
来源：http://twv.sweek.top

@property 与 @x.setter 配合
来源：http://hql.yonumen.top

[U30] Py：数据类
来源：http://yeh.mhx1999.top

@dataclass(slots=True)
来源：http://vtk.ehwqpu.com

[U31] Py：单测
来源：http://xyv.52xcode.cn

python -m pytest -q
来源：http://hwo.sysykeji.top

[U32] Py：代码格式化
来源：http://zcz.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://uha.zhengqikj.top

[U33] Py：打包发布
来源：http://yoz.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://afz.hfpthk.cn

[U34] Py：判断编码
来源：http://atk.yongpay.top

chardet.detect(raw)
来源：http://vyy.jiagoushi.top

[U35] Py：发送邮件
来源：http://tjd.shanyushiyangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://epw.hysaishi.cn

[U36] Py：定时任务
来源：http://azi.aibaodan.cn

schedule.every(10).minutes.do(job)
来源：http://qoc.xinyue.icu

[U37] Py：读写 Excel
来源：http://kke.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://anr.smart0.xyz

[U38] Py：获取脚本所在目录
来源：http://oyv.gotoacloud.top

Path(__file__).resolve().parent
来源：http://vpp.xziqi.cn

[U39] Py：判断是否在交互环境
来源：http://yeu.hysaishi.cn

sys.stdout.isatty()
来源：http://pun.52xcode.cn

[U40] Py：打印到标准错误
来源：http://yst.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://jnw.52xcode.cn

[U41] PHP：初始化 Composer 项目
来源：http://hum.nanxinkj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gvt.bbcook.cn

[U42] PHP：PSR-4 自动加载
来源：http://iin.bjfxy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ygu.cheryme.top

[U43] PHP：声明命名空间
来源：http://gzr.gzhubu.top

namespace App\Http;
来源：http://wwk.yj20258.top

[U44] PHP：开启严格类型
来源：http://scm.mhx1999.top

declare(strict_types=1);
来源：http://vhr.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://bim.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ezq.52xcode.cn

[U46] PHP：可空类型
来源：http://lbr.ydzc1.top

?string $name = null
来源：http://syj.dashuyun.cn

[U47] PHP：联合类型
来源：http://hwy.yanxiufei.cn

int|string $id
来源：http://itx.hnqzz.top

[U48] PHP：纯枚举
来源：http://hys.sysykeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bje.cqqwz.cn

[U49] PHP：只读属性
来源：http://gbw.chenzaomai.com

public readonly string $name
来源：http://knf.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://spl.mhx1999.top

public function __construct(private int $id) {}
来源：http://gnm.meibo888.top


<!-- 参考信息 -->