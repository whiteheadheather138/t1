代发 wailian999

x |= (1 << 3);
来源：http://hwa.yj20258.top

[S17] C：安全拼接字符串
来源：http://kun.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://siw.cqqwz.cn

[S18] C：命令行参数
来源：http://usz.aibaodan.cn

int main(int argc, char **argv)
来源：http://yyl.shzxlz.cn

[S19] C：快速排序
来源：http://bla.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hmd.jinqigufen.top

[S20] C：二分查找
来源：http://zmo.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zod.jiagoushi.top

[S21] C：字符类别判断
来源：http://qbp.gotoacloud.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eey.jiagoushi.top

[S22] C：字符串转数字
来源：http://jym.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://sts.zhijiandao.cn

[S23] C：随机数
来源：http://svs.cqqwz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fag.shzxlz.cn

[S24] C：获取本地时间
来源：http://nij.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lap.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://pfv.yvedp.cn

memcpy(dst, src, n);
来源：http://rno.dashuyun.cn

[S26] C：内存清零
来源：http://obk.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://rso.tianlin.xyz

[S27] C：定义常量
来源：http://dxm.zycfv.cn

const double PI = 3.14159;
来源：http://ffh.ydjk.org.cn

[S28] C：静态变量
来源：http://vdp.ctjpmb.com

static int counter = 0;
来源：http://sax.tanke756.top

[S29] C：变参函数
来源：http://yeb.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wuh.smart0.xyz

[S30] C：头文件保护
来源：http://haf.gzhubu.top

#ifndef X_H
来源：http://qto.jinghuilouyu.cn

#define X_H
来源：http://klp.xingfuxueyuan.xyz

#endif
来源：http://aef.tanke756.top

[S31] C++：Hello World
来源：http://iod.jinqigufen.top

#include <iostream>
来源：http://ovl.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://kdy.aibaodan.cn

[S32] C++：字符串
来源：http://qfc.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://cas.smart0.xyz

[S33] C++：vector 增删
来源：http://wyx.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fio.yuanzhike.top

[S34] C++：遍历 vector
来源：http://twe.yj20258.top

for (auto &x : v) { std::cout << x; }
来源：http://rov.chenlongwang.top

[S35] C++：map
来源：http://fwb.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://krn.andypj.xyz

[S36] C++：unordered_map
来源：http://edn.ehwqpu.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kpd.uphjek.com

[S37] C++：set
来源：http://gtt.yuanzhike.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gzc.xuetiantiany.cn

[S38] C++：排序
来源：http://edo.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://bwi.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://bpb.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bbt.hammf.cn

[S40] C++：查找元素
来源：http://awf.yj202588.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qvz.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://syb.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gnp.yj202588.top

[S42] C++：继承与虚函数
来源：http://utz.jinqigfzy.top

class B : public Base { public: void f() override {} };
来源：http://nvr.zycfv.cn

[S43] C++：智能指针
来源：http://wwy.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://uuk.c1oappe.top

[S44] C++：引用传参
来源：http://xob.fengsongda.top

void inc(int &x) { ++x; }
来源：http://cew.fzhhl.top

[S45] C++：lambda
来源：http://xvp.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://wvi.daria6918.cn

[S46] C++：函数模板
来源：http://xbe.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://heo.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://mod.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eif.hongshengwenyu.top

[S48] C++：逐行读文件
来源：http://fvj.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lwf.aibaodan.cn

while (std::getline(in, line)) { }
来源：http://qrk.hysaishi.cn

[S49] C++：写文件
来源：http://swh.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ssd.yonumen.top

[S50] C++：格式化数字
来源：http://ssp.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hws.ybcxt.top

[S51] C++：显式类型转换
来源：http://ngm.iojbl.cn

static_cast<double>(a) / b
来源：http://ghn.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://myy.tanke756.top

int size() const noexcept { return n_; }
来源：http://lpt.tanke756.top

[S53] C++：移动语义
来源：http://fdd.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://fev.ehwqpu.com

[S54] C++：异常处理
来源：http://epi.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hxe.yueranfly.top

[S55] C++：结构化绑定
来源：http://nzz.wangdashe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://koz.kuanghao11.cn

[S56] C++：optional
来源：http://gmq.ctjpmb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xue.gzhubu.top

[S57] C++：编译期常量
来源：http://hrr.hywenlv.cn

constexpr int N = 10;
来源：http://jif.sxryk.cn

[S58] C++：命名空间
来源：http://qzm.jianghu66.top

namespace ns { int f() { return 1; } }
来源：http://efp.9152youxi.cn

[S59] C++：静态断言
来源：http://xdl.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vam.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://csv.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jxs.fktsv.cn

================================================================================
来源：http://ope.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ler.316326.xyz

================================================================================
来源：http://rtl.aizwys.cn

[T01] Kotlin：Hello World
来源：http://dqc.fehbvm.com

println("Hello")
来源：http://nzc.guowangkeji.top

[T02] Kotlin：变量
来源：http://joe.ehwqpu.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tfm.jiagoushi.top

[T03] Kotlin：字符串模板
来源：http://epc.jlsjyb.cn

"值: $b"
来源：http://neg.ppjwa.cn

[T04] Kotlin：空安全
来源：http://pnw.xylfe.cn

val n: String? = null;  n?.length
来源：http://gtj.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://yzb.zhongyouzk.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bpp.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://wuc.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gsq.52xcode.cn

[T07] Kotlin：集合过滤
来源：http://ypl.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://fbu.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://jol.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://ndr.andypj.xyz

[T09] Kotlin：扩展函数
来源：http://kdq.meibo888.top

fun String.exclaim() = this + "!"
来源：http://wok.yj20258.top

[T10] Kotlin：默认参数
来源：http://pad.hesvh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mty.zdbjq.cn

[T11] Kotlin：协程
来源：http://osl.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rut.yuxming.cn

[T12] Kotlin：解构声明
来源：http://wxn.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://ygw.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://qsb.jqgfzy.top

val m = mapOf("a" to 1)
来源：http://ndf.ppjwa.cn

[T14] Kotlin：循环
来源：http://xpj.hesvh.cn

for (i in 1..10) println(i)
来源：http://loa.iojbl.cn

[T15] Kotlin：接口
来源：http://mkx.tianlin.xyz

interface Shape { fun area(): Double }
来源：http://pja.tianlin.xyz

[T16] Swift：Hello World
来源：http://iwn.meibo888.top

print("Hello")
来源：http://uzd.jianghu66.top

[T17] Swift：变量与常量
来源：http://vje.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://tae.vehdjk.com

[T18] Swift：字符串插值
来源：http://cpy.zycfv.cn

"值: \(b)"
来源：http://nlc.bbcook.cn

[T19] Swift：可选绑定
来源：http://cke.aizwys.cn

if let n = opt { print(n) }
来源：http://zlk.316326.xyz

[T20] Swift：数组操作
来源：http://tyj.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://bgu.dianchejie.cn

[T21] Swift：遍历
来源：http://aqi.chenlongwang.top

for x in a { print(x) }
来源：http://epq.fzhhl.top

[T22] Swift：字典
来源：http://cdq.guannengcc.top

var d = ["a": 1];  d["b"] = 2
来源：http://qen.kuanghao11.cn

[T23] Swift：函数
来源：http://rbu.hnqzz.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rkz.zycfv.cn

[T24] Swift：闭包
来源：http://azx.wangdashe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xmm.yj20258.top

[T25] Swift：结构体
来源：http://zkd.tianlin.xyz

struct P { var x: Int }
来源：http://one.fanxiaobao.xyz

[T26] Swift：类与重写
来源：http://pef.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://wma.daxiang520.top

[T27] Swift：错误处理
来源：http://iqz.yongpay.top

do { try f() } catch { print(error) }
来源：http://qox.sufxvd.cn

[T28] Swift：枚举
来源：http://aqx.jqgufenzy.top

enum Color { case red, green }
来源：http://cvx.dashuyun.cn

[T29] Swift：guard 提前返回
来源：http://cje.yj202588.top

guard let x = opt else { return }
来源：http://gdj.jianghu66.top

[T30] Swift：协议
来源：http://ony.bjfxy.top

protocol Shape { func area() -> Double }
来源：http://yjr.shuidangran.top

[T31] Lua：Hello World
来源：http://wdx.guowangkeji.top

print("Hello")
来源：http://bwi.52xcode.cn

[T32] Lua：局部变量
来源：http://urp.ydzc1.top

local a = 1
来源：http://dqx.vqdsnc.cn

[T33] Lua：表（数组）
来源：http://zha.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ziq.iojbl.cn

[T34] Lua：遍历表
来源：http://gcv.smart0.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://zms.feifeiyinyue.top

[T35] Lua：字典表
来源：http://twq.zhijiandao.cn

local d = { a = 1 };  d.b = 2
来源：http://yzy.haohaochexian.top

[T36] Lua：函数
来源：http://pto.hongshengwenyu.top

function add(a, b) return a + b end
来源：http://mkm.zycfv.cn

[T37] Lua：字符串拼接
来源：http://hni.gogol.net.cn

"a" .. "b"
来源：http://nfs.ppjwa.cn

[T38] Lua：条件
来源：http://liv.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://epx.yvedp.cn

[T39] Lua：模式匹配
来源：http://yxa.birdmap.top

string.find(s, "%d+")
来源：http://vba.hywenlv.cn

[T40] Lua：元表
来源：http://vnl.ctjpmb.com

setmetatable({}, { __index = base })
来源：http://egu.feifeiyinyue.top

[T41] Perl：Hello World
来源：http://bwo.zdqjudy.top

print "Hello\n";
来源：http://jcz.yanxiufei.cn

[T42] Perl：变量类型
来源：http://oej.chenlongwang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pww.shuidangran.top

[T43] Perl：字符串插值
来源：http://pcn.0kj1m.cn

"值: $a"
来源：http://pcq.andypj.xyz

[T44] Perl：条件
来源：http://ltm.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://cgr.daria6918.cn

[T45] Perl：数组遍历
来源：http://gnm.jinyuanbaomall.cn

for my $x (@arr) { print $x; }
来源：http://pza.sufxvd.cn

[T46] Perl：哈希操作
来源：http://tcn.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wmw.ehwqpu.com

[T47] Perl：正则捕获
来源：http://odb.sweek.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tyk.fengsongda.top

[T48] Perl：正则替换
来源：http://wtm.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://gxh.dianchejie.cn

[T49] Perl：函数
来源：http://fpm.daxiang520.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ubh.tarul.cn

[T50] Perl：逐行读文件
来源：http://ivo.andypj.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://sul.hysaishi.cn

while (my $line = <$fh>) { print $line; }
来源：http://zmh.zhijiandao.cn

[T51] Scala：Hello World
来源：http://jal.hnxiangtu.top

println("Hello")
来源：http://dje.cqqwz.cn

[T52] Scala：变量
来源：http://sbe.guowangkeji.top

val a = 1;  var b = 2
来源：http://fkn.yj20258.top

[T53] Scala：字符串插值
来源：http://rgx.xziqi.cn

s"值: $b"
来源：http://abn.ppjwa.cn

[T54] Scala：集合映射
来源：http://khh.hnqzz.top

List(1, 2, 3).map(_ * 2)
来源：http://nek.hammf.cn

[T55] Scala：集合过滤
来源：http://kkv.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oiu.aizwys.cn

[T56] Scala：样例类
来源：http://uqd.aibaodan.cn

case class User(name: String, age: Int)
来源：http://fdd.fktsv.cn

[T57] Scala：模式匹配
来源：http://sao.yfazqb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://oly.aibaodan.cn

[T58] Scala：函数定义
来源：http://ssw.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://mdz.jinqigufen.top

[T59] Scala：循环
来源：http://myo.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://key.hesvh.cn

[T60] Scala：折叠
来源：http://kxk.zhongyouzk.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rwi.sufxvd.cn

================================================================================
来源：http://bqf.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oud.ybcxt.top

================================================================================
来源：http://xgq.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://yur.yfazqb.com

python -m venv .venv && source .venv/bin/activate
来源：http://hbi.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://oeh.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wuu.chenjidiqi.icu

[U03] Py：加载 .env 配置
来源：http://cgh.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ntr.svipenyu.cn

[U04] Py：变量调试打印
来源：http://aue.hcnkem.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gqx.kuanghao11.cn

[U05] Py：列表去重且保序
来源：http://gii.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://uzl.jiagoushi.top

[U06] Py：合并两个字典
来源：http://cck.pycfn.com

{**a, **b}
来源：http://ble.guannengcc.top

[U07] Py：反转字典键值
来源：http://nlb.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://vlc.cashguo.top

[U08] Py：展平二维列表
来源：http://pke.zhaomingkeji.xyz

[y for x in nested for y in x]
来源：http://byh.uphjek.com

[U09] Py：字典取最大值的键
来源：http://skp.fktsv.cn

max(d, key=d.get)
来源：http://pwl.havefunace.top

[U10] Py：按值排序字典
来源：http://yqc.sysykeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dvl.havefunace.top

[U11] Py：生成器表达式
来源：http://wle.smart0.xyz

(x * 2 for x in arr)
来源：http://pcp.iojbl.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jrz.uphjek.com

Counter(arr).most_common(3)
来源：http://mss.jianghu66.top

[U13] Py：固定长度队列
来源：http://sxg.yj202588.top

deque(maxlen=10)
来源：http://zjl.0kj1m.cn

[U14] Py：分组收集到列表
来源：http://njq.yongpay.top

defaultdict(list)
来源：http://ygu.cqqwz.cn

[U15] Py：高精度计时
来源：http://jhy.xinyue.icu

t = time.perf_counter()
来源：http://ert.yj20258888.top

[U16] Py：命令行参数解析
来源：http://xwc.guannengcc.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qnn.hongshengwenyu.top

[U17] Py：初始化日志
来源：http://tew.aibaodan.cn

logging.basicConfig(level=logging.INFO)
来源：http://xnl.zdbjq.cn

[U18] Py：预编译正则
来源：http://tbw.hnqzz.top

pat = re.compile(r"\d+")
来源：http://syc.shanyushiyangtech.top

[U19] Py：正则替换带回调
来源：http://oth.xinyue.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ldl.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://nxb.wangdashe.top

@functools.lru_cache(maxsize=None)
来源：http://kxz.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://fll.hfpthk.cn

@contextlib.contextmanager
来源：http://ywp.yonumen.top

[U22] Py：矩阵转置
来源：http://imv.cashguo.top

list(zip(*m))
来源：http://glo.xingfuxueyuan.xyz

[U23] Py：分块读取大文件
来源：http://jjq.ywan-chungtsiang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vrv.aibaodan.cn

[U24] Py：路径操作
来源：http://nkw.jinqigfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wrj.yuxming.cn

[U25] Py：CSV 按字典读
来源：http://npw.hesvh.cn

csv.DictReader(f)
来源：http://nly.hnxiangtu.top

[U26] Py：并发下载
来源：http://sss.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jxx.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://tvh.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://oge.shzxlz.cn

[U28] Py：类型别名
来源：http://pdn.yangfankeji.com

UserId = int
来源：http://rkv.tian-w.cn

[U29] Py：属性校验
来源：http://vug.aibaodan.cn

@property 与 @x.setter 配合
来源：http://wxr.daxiang520.top

[U30] Py：数据类
来源：http://dob.meibo888.top

@dataclass(slots=True)
来源：http://asd.sysykeji.top

[U31] Py：单测
来源：http://xbo.redwolf501.top

python -m pytest -q
来源：http://nos.meibo888.top

[U32] Py：代码格式化
来源：http://rol.zhiwuduotai.top

ruff format . && ruff check --fix .
来源：http://wek.chenlongwang.top

[U33] Py：打包发布
来源：http://pzy.52xcode.cn

python -m build  （依赖 pyproject.toml）
来源：http://zuj.iojbl.cn

[U34] Py：判断编码
来源：http://xpi.0kj1m.cn

chardet.detect(raw)
来源：http://sia.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://xdq.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xdo.svipenyu.cn

[U36] Py：定时任务
来源：http://mlz.xziqi.cn

schedule.every(10).minutes.do(job)
来源：http://jlh.yuanzhike.top

[U37] Py：读写 Excel
来源：http://svr.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jwy.tianlin.xyz

[U38] Py：获取脚本所在目录
来源：http://esq.yongpay.top

Path(__file__).resolve().parent
来源：http://fko.sweek.top

[U39] Py：判断是否在交互环境
来源：http://oqa.tianlin.xyz

sys.stdout.isatty()
来源：http://mxy.chenzaomai.com

[U40] Py：打印到标准错误
来源：http://mhv.yanxiufei.cn

print("err", file=sys.stderr)
来源：http://sdo.hcnkem.com


<!-- 参考信息 -->