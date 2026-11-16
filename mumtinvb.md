代发 wailian999

x |= (1 << 3);
来源：http://rzu.pengpengdd.cyou

[S17] C：安全拼接字符串
来源：http://dxc.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ndr.bbcook.cn

[S18] C：命令行参数
来源：http://afu.c1oappe.top

int main(int argc, char **argv)
来源：http://vqn.ctjpmb.com

[S19] C：快速排序
来源：http://htw.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://cek.dashuyun.cn

[S20] C：二分查找
来源：http://dmx.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jir.smart0.xyz

[S21] C：字符类别判断
来源：http://bse.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jhb.iojbl.cn

[S22] C：字符串转数字
来源：http://mpo.zhengqikj.top

atoi("42");  strtod("3.14", NULL);
来源：http://rgn.hcnkem.com

[S23] C：随机数
来源：http://mbi.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zbt.xylfe.cn

[S24] C：获取本地时间
来源：http://okq.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vpu.gotoacloud.top

[S25] C：内存拷贝
来源：http://erb.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://jqq.0kj1m.cn

[S26] C：内存清零
来源：http://scf.hfpthk.cn

memset(a, 0, sizeof a);
来源：http://zfr.birdmap.top

[S27] C：定义常量
来源：http://tor.cashguo.top

const double PI = 3.14159;
来源：http://gro.fengsongda.top

[S28] C：静态变量
来源：http://vpm.jiagoushi.top

static int counter = 0;
来源：http://jjv.yueranfly.top

[S29] C：变参函数
来源：http://fyl.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://emb.hnxiangtu.top

[S30] C：头文件保护
来源：http://rfh.wangdashe.top

#ifndef X_H
来源：http://ryt.ehwqpu.com

#define X_H
来源：http://ibp.yvedp.cn

#endif
来源：http://qlv.havefunace.top

[S31] C++：Hello World
来源：http://lxn.xingfuxueyuan.xyz

#include <iostream>
来源：http://lsx.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://awz.ivvv.top

[S32] C++：字符串
来源：http://wxw.ctjpmb.com

std::string s = "hi";  s += "!";
来源：http://dax.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://dnw.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rfa.yonumen.top

[S34] C++：遍历 vector
来源：http://dfj.sjlbkw.cn

for (auto &x : v) { std::cout << x; }
来源：http://gnq.yj20258.top

[S35] C++：map
来源：http://pmd.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aqg.yuxming.cn

[S36] C++：unordered_map
来源：http://wjt.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://moc.yuxming.cn

[S37] C++：set
来源：http://fqu.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zdg.yangfankeji.com

[S38] C++：排序
来源：http://fmb.birdmap.top

std::sort(v.begin(), v.end());
来源：http://emq.nwbrower.top

[S39] C++：自定义比较器排序
来源：http://cgo.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gzh.yj20258.top

[S40] C++：查找元素
来源：http://bgl.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ske.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://fyx.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://msp.nanxuanxn.top

[S42] C++：继承与虚函数
来源：http://apr.hesvh.cn

class B : public Base { public: void f() override {} };
来源：http://dlm.meibo888.top

[S43] C++：智能指针
来源：http://bik.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://eey.zhongyouzk.top

[S44] C++：引用传参
来源：http://udk.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://jtu.yj202588.top

[S45] C++：lambda
来源：http://mcg.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://una.chenzaomai.com

[S46] C++：函数模板
来源：http://kwj.hywenlv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jfz.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://tvp.jinqigfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lgg.tianlin.xyz

[S48] C++：逐行读文件
来源：http://emn.chenlongwang.top

std::ifstream in("a.txt");  std::string line;
来源：http://yfp.fzhhl.top

while (std::getline(in, line)) { }
来源：http://jgk.cashguo.top

[S49] C++：写文件
来源：http://ezy.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ovo.jinqigfzy.top

[S50] C++：格式化数字
来源：http://mev.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uzf.yongpay.top

[S51] C++：显式类型转换
来源：http://mws.yonumen.top

static_cast<double>(a) / b
来源：http://adb.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://hab.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://eun.hywenlv.cn

[S53] C++：移动语义
来源：http://juv.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://pce.cdnleiting.top

[S54] C++：异常处理
来源：http://fbm.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ose.fehbvm.com

[S55] C++：结构化绑定
来源：http://dys.ydzc1.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ihv.xziqi.cn

[S56] C++：optional
来源：http://uze.zycfv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yuh.kuanghao11.cn

[S57] C++：编译期常量
来源：http://jan.yongpay.top

constexpr int N = 10;
来源：http://yrs.ivvv.top

[S58] C++：命名空间
来源：http://twq.uphjek.com

namespace ns { int f() { return 1; } }
来源：http://fsx.zhongyouzk.top

[S59] C++：静态断言
来源：http://ket.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://alk.shanyushiyangtech.top

[S60] C++：遍历并删除元素
来源：http://vcx.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fik.yvedp.cn

================================================================================
来源：http://zsa.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ekr.sysykeji.top

================================================================================
来源：http://yag.yj202588.top

[T01] Kotlin：Hello World
来源：http://dze.tian-w.cn

println("Hello")
来源：http://sjj.fktsv.cn

[T02] Kotlin：变量
来源：http://jvu.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yig.wangshuangyany.cn

[T03] Kotlin：字符串模板
来源：http://fts.sweek.top

"值: $b"
来源：http://kvm.zhengqikj.top

[T04] Kotlin：空安全
来源：http://lim.ctjpmb.com

val n: String? = null;  n?.length
来源：http://tle.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://dlz.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nzm.hywenlv.cn

[T06] Kotlin：集合映射
来源：http://tty.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mfi.haohaochexian.top

[T07] Kotlin：集合过滤
来源：http://tmt.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jqv.dianchejie.cn

[T08] Kotlin：数据类
来源：http://cib.ydzc1.top

data class User(val name: String, val age: Int)
来源：http://xbb.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://gnq.pycfn.com

fun String.exclaim() = this + "!"
来源：http://hhp.yueranfly.top

[T10] Kotlin：默认参数
来源：http://lrc.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wpv.ydzc1.top

[T11] Kotlin：协程
来源：http://uti.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://niq.pycfn.com

[T12] Kotlin：解构声明
来源：http://ytl.yueranfly.top

val (a, b) = Pair(1, 2)
来源：http://izl.ppjwa.cn

[T13] Kotlin：只读 Map
来源：http://wka.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://hax.epnwcf.com

[T14] Kotlin：循环
来源：http://dhq.birdmap.top

for (i in 1..10) println(i)
来源：http://xee.guannengcc.top

[T15] Kotlin：接口
来源：http://nwi.52xcode.cn

interface Shape { fun area(): Double }
来源：http://cjc.iojbl.cn

[T16] Swift：Hello World
来源：http://evf.aibaodan.cn

print("Hello")
来源：http://enp.ivvv.top

[T17] Swift：变量与常量
来源：http://eja.zhiwuduotai.top

var a = 1;  let b = 2
来源：http://ebj.bjfxy.top

[T18] Swift：字符串插值
来源：http://yqw.cdnleiting.top

"值: \(b)"
来源：http://obh.zycfv.cn

[T19] Swift：可选绑定
来源：http://cei.bjfxy.top

if let n = opt { print(n) }
来源：http://aez.jlsjyb.cn

[T20] Swift：数组操作
来源：http://sbt.wangdashe.top

var a = [1, 2, 3];  a.append(4)
来源：http://dfc.guannengcc.top

[T21] Swift：遍历
来源：http://hod.shuidangran.top

for x in a { print(x) }
来源：http://ktp.9152youxi.cn

[T22] Swift：字典
来源：http://vsm.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vvl.zhixingplan.top

[T23] Swift：函数
来源：http://gvh.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mrt.52xcode.cn

[T24] Swift：闭包
来源：http://tfl.sufxvd.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qia.nanxinkj.top

[T25] Swift：结构体
来源：http://bcu.cqqwz.cn

struct P { var x: Int }
来源：http://ajn.epnwcf.com

[T26] Swift：类与重写
来源：http://shu.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://riv.zhixingplan.top

[T27] Swift：错误处理
来源：http://wpn.xinyue.icu

do { try f() } catch { print(error) }
来源：http://els.sxryk.cn

[T28] Swift：枚举
来源：http://uwd.quarkkingdee.top

enum Color { case red, green }
来源：http://onk.havefunace.top

[T29] Swift：guard 提前返回
来源：http://dqz.hammf.cn

guard let x = opt else { return }
来源：http://eto.cdnleiting.top

[T30] Swift：协议
来源：http://yro.hongshengwenyu.top

protocol Shape { func area() -> Double }
来源：http://phg.tanke756.top

[T31] Lua：Hello World
来源：http://vrx.aizwys.cn

print("Hello")
来源：http://pjn.uphjek.com

[T32] Lua：局部变量
来源：http://ytv.smart0.xyz

local a = 1
来源：http://qmj.dashuyun.cn

[T33] Lua：表（数组）
来源：http://qck.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uqi.aibaodan.cn

[T34] Lua：遍历表
来源：http://vpa.yongpay.top

for i, v in ipairs(t) do print(i, v) end
来源：http://sol.fanxiaobao.xyz

[T35] Lua：字典表
来源：http://jdr.c1oappe.top

local d = { a = 1 };  d.b = 2
来源：http://zwh.0kj1m.cn

[T36] Lua：函数
来源：http://aul.hongshengwenyu.top

function add(a, b) return a + b end
来源：http://lyr.hesvh.cn

[T37] Lua：字符串拼接
来源：http://vrw.yangfankeji.com

"a" .. "b"
来源：http://yib.gaohongyu789.top

[T38] Lua：条件
来源：http://qsr.hesvh.cn

if x > 0 then print("正") end
来源：http://iuw.zycfv.cn

[T39] Lua：模式匹配
来源：http://jhp.52xcode.cn

string.find(s, "%d+")
来源：http://zqk.jqgfzy.top

[T40] Lua：元表
来源：http://edz.tanke756.top

setmetatable({}, { __index = base })
来源：http://bxu.chenlongwang.top

[T41] Perl：Hello World
来源：http://tbv.bjfxy.top

print "Hello\n";
来源：http://yey.sufxvd.cn

[T42] Perl：变量类型
来源：http://gtf.gogol.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tck.jyoumei.cn

[T43] Perl：字符串插值
来源：http://fnp.pengpengdd.cyou

"值: $a"
来源：http://eum.zhongyouzk.top

[T44] Perl：条件
来源：http://bnh.sysykeji.top

if ($a > 0) { print "正"; }
来源：http://mau.aizwys.cn

[T45] Perl：数组遍历
来源：http://nhv.fktsv.cn

for my $x (@arr) { print $x; }
来源：http://czs.meibo888.top

[T46] Perl：哈希操作
来源：http://wpo.yj20258.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://snv.daxiang520.top

[T47] Perl：正则捕获
来源：http://gpu.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://lfm.sufxvd.cn

[T48] Perl：正则替换
来源：http://ojq.xingfuxueyuan.xyz

$s =~ s/old/new/g;
来源：http://hvg.hesvh.cn

[T49] Perl：函数
来源：http://usj.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://evi.yongpay.top

[T50] Perl：逐行读文件
来源：http://gfo.daria6918.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://otg.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://bgl.ivvv.top

[T51] Scala：Hello World
来源：http://poy.tianlin.xyz

println("Hello")
来源：http://szr.sweek.top

[T52] Scala：变量
来源：http://mzf.hammf.cn

val a = 1;  var b = 2
来源：http://une.andypj.xyz

[T53] Scala：字符串插值
来源：http://isy.nanxuanxn.top

s"值: $b"
来源：http://hjk.quarkkingdee.top

[T54] Scala：集合映射
来源：http://zzb.zhiwuduotai.top

List(1, 2, 3).map(_ * 2)
来源：http://myu.hammf.cn

[T55] Scala：集合过滤
来源：http://wfq.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://prq.shangyingyoupin.top

[T56] Scala：样例类
来源：http://rbd.yj20258888.top

case class User(name: String, age: Int)
来源：http://nul.guowangkeji.top

[T57] Scala：模式匹配
来源：http://aqc.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://xsa.sufxvd.cn

[T58] Scala：函数定义
来源：http://gaa.nwbrower.top

def add(a: Int, b: Int): Int = a + b
来源：http://nhd.yanxiufei.cn

[T59] Scala：循环
来源：http://ibz.sweek.top

for (i <- 1 to 10) println(i)
来源：http://xsw.gogol.net.cn

[T60] Scala：折叠
来源：http://pxf.fktsv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://meo.yvedp.cn

================================================================================
来源：http://fnl.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vmq.dashuyun.cn

================================================================================
来源：http://xip.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://emz.bjfxy.top

python -m venv .venv && source .venv/bin/activate
来源：http://ogs.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://xvk.ivvv.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iah.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://qbs.ywan-chungtsiang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wub.gzhubu.top

[U04] Py：变量调试打印
来源：http://zvc.havefunace.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vti.aizwys.cn

[U05] Py：列表去重且保序
来源：http://glg.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://bch.hfpthk.cn

[U06] Py：合并两个字典
来源：http://isf.fktsv.cn

{**a, **b}
来源：http://vlh.dashuyun.cn

[U07] Py：反转字典键值
来源：http://gib.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://gch.yuxming.cn

[U08] Py：展平二维列表
来源：http://cdk.wangshuangyany.cn

[y for x in nested for y in x]
来源：http://ppl.hcnkem.com

[U09] Py：字典取最大值的键
来源：http://olw.bbcook.cn

max(d, key=d.get)
来源：http://abl.gzhubu.top

[U10] Py：按值排序字典
来源：http://zov.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lpn.haohaochexian.top

[U11] Py：生成器表达式
来源：http://cqz.yonumen.top

(x * 2 for x in arr)
来源：http://zem.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pxk.nanxuanxn.top

Counter(arr).most_common(3)
来源：http://ykg.zhaomingkeji.xyz

[U13] Py：固定长度队列
来源：http://xai.ydjk.org.cn

deque(maxlen=10)
来源：http://yim.jqgufenzy.top

[U14] Py：分组收集到列表
来源：http://olm.c1oappe.top

defaultdict(list)
来源：http://jtq.jqgfzy.top

[U15] Py：高精度计时
来源：http://gsq.aizwys.cn

t = time.perf_counter()
来源：http://xfl.fanxiaobao.xyz

[U16] Py：命令行参数解析
来源：http://tzg.jyoumei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://duf.birdmap.top

[U17] Py：初始化日志
来源：http://mur.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://itb.gzhubu.top

[U18] Py：预编译正则
来源：http://ewq.sysykeji.top

pat = re.compile(r"\d+")
来源：http://vuh.jinqigfzy.top

[U19] Py：正则替换带回调
来源：http://sux.sufxvd.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tgw.gzhubu.top

[U20] Py：缓存函数结果
来源：http://znb.yj20258.top

@functools.lru_cache(maxsize=None)
来源：http://zjl.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://ycw.shzxlz.cn

@contextlib.contextmanager
来源：http://hvr.redwolf501.top

[U22] Py：矩阵转置
来源：http://std.xingfuxueyuan.xyz

list(zip(*m))
来源：http://daw.zhiwuduotai.top

[U23] Py：分块读取大文件
来源：http://hlt.shanyushiyangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mee.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://llf.cqqwz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dok.ctjpmb.com

[U25] Py：CSV 按字典读
来源：http://svf.hesvh.cn

csv.DictReader(f)
来源：http://sco.jqgfzy.top

[U26] Py：并发下载
来源：http://hka.zycfv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xki.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://rcg.ywan-chungtsiang.top

aiohttp.ClientSession() 配合 async with
来源：http://uge.quarkkingdee.top

[U28] Py：类型别名
来源：http://pkp.xziqi.cn

UserId = int
来源：http://mff.sjlbkw.cn

[U29] Py：属性校验
来源：http://imy.yfazqb.com

@property 与 @x.setter 配合
来源：http://kxt.snrcjt.cn

[U30] Py：数据类
来源：http://ywe.iojbl.cn

@dataclass(slots=True)
来源：http://ygp.hesvh.cn

[U31] Py：单测
来源：http://dmn.cashguo.top

python -m pytest -q
来源：http://odz.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://tlc.52xcode.cn

ruff format . && ruff check --fix .
来源：http://ysa.yfazqb.com

[U33] Py：打包发布
来源：http://quy.yangfankeji.com

python -m build  （依赖 pyproject.toml）
来源：http://uuq.ydjk.org.cn

[U34] Py：判断编码
来源：http://xap.haohaochexian.top

chardet.detect(raw)
来源：http://waz.ivvv.top

[U35] Py：发送邮件
来源：http://kcu.yanxiufei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hgt.vqdsnc.cn

[U36] Py：定时任务
来源：http://lsh.zhengqikj.top

schedule.every(10).minutes.do(job)
来源：http://dhu.hesvh.cn

[U37] Py：读写 Excel
来源：http://nxd.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://hxp.zhongyouzk.top

[U38] Py：获取脚本所在目录
来源：http://edj.epnwcf.com

Path(__file__).resolve().parent
来源：http://dfr.aibaodan.cn

[U39] Py：判断是否在交互环境
来源：http://kng.jinyuanbaomall.cn

sys.stdout.isatty()
来源：http://vhr.kuanghao11.cn

[U40] Py：打印到标准错误
来源：http://cft.svipenyu.cn

print("err", file=sys.stderr)
来源：http://bgz.0kj1m.cn


<!-- 参考信息 -->