代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://jjg.ppjwa.cn

[S15] C：类型转换
来源：http://aux.vqdsnc.cn

(double) a / b
来源：http://phq.hcnkem.com

[S16] C：位操作置位
来源：http://fpw.jqgfzy.top

x |= (1 << 3);
来源：http://zwg.fzhhl.top

[S17] C：安全拼接字符串
来源：http://eai.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ivi.tarul.cn

[S18] C：命令行参数
来源：http://xsb.xziqi.cn

int main(int argc, char **argv)
来源：http://dxj.yj202588.top

[S19] C：快速排序
来源：http://zwt.jlsjyb.cn

qsort(a, n, sizeof(int), cmp);
来源：http://enr.gaohongyu789.top

[S20] C：二分查找
来源：http://liz.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ylq.ctjpmb.com

[S21] C：字符类别判断
来源：http://vfc.yfazqb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uhu.svipenyu.cn

[S22] C：字符串转数字
来源：http://sla.sweek.top

atoi("42");  strtod("3.14", NULL);
来源：http://bdk.fengsongda.top

[S23] C：随机数
来源：http://fiy.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://djn.jianghu66.top

[S24] C：获取本地时间
来源：http://olz.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://suk.iojbl.cn

[S25] C：内存拷贝
来源：http://jrg.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://vhr.yj20258.top

[S26] C：内存清零
来源：http://yqd.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://qjf.meibo888.top

[S27] C：定义常量
来源：http://hhp.yangfankeji.com

const double PI = 3.14159;
来源：http://mwr.dashuyun.cn

[S28] C：静态变量
来源：http://axu.wangshuangyany.cn

static int counter = 0;
来源：http://zqv.c1oappe.top

[S29] C：变参函数
来源：http://zoi.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hzq.uphjek.com

[S30] C：头文件保护
来源：http://vdl.chenlongwang.top

#ifndef X_H
来源：http://ayi.fanxiaobao.xyz

#define X_H
来源：http://yuv.bbcook.cn

#endif
来源：http://xey.vqdsnc.cn

[S31] C++：Hello World
来源：http://jae.jinghuilouyu.cn

#include <iostream>
来源：http://wat.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://ful.smart0.xyz

[S32] C++：字符串
来源：http://nrv.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://upr.ivvv.top

[S33] C++：vector 增删
来源：http://xfx.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ura.yj202588.top

[S34] C++：遍历 vector
来源：http://rod.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://pyx.vehdjk.com

[S35] C++：map
来源：http://wmg.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qkr.fktsv.cn

[S36] C++：unordered_map
来源：http://cwo.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ykl.zhijiandao.cn

[S37] C++：set
来源：http://gmi.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pjh.cashguo.top

[S38] C++：排序
来源：http://ylq.hongshengwenyu.top

std::sort(v.begin(), v.end());
来源：http://ygy.daria6918.cn

[S39] C++：自定义比较器排序
来源：http://hho.wangshuangyany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gsm.jqgfzy.top

[S40] C++：查找元素
来源：http://npb.hywenlv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ylm.gogol.net.cn

[S41] C++：类与构造函数
来源：http://szx.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hlk.vehdjk.com

[S42] C++：继承与虚函数
来源：http://xmo.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://tjs.guannengcc.top

[S43] C++：智能指针
来源：http://atq.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://zhb.wangdashe.top

[S44] C++：引用传参
来源：http://qvj.yonumen.top

void inc(int &x) { ++x; }
来源：http://qfl.xuetiantiany.cn

[S45] C++：lambda
来源：http://fhf.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://kwg.jqgufenzy.top

[S46] C++：函数模板
来源：http://kys.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gno.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://psk.ivvv.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ock.zdbjq.cn

[S48] C++：逐行读文件
来源：http://dzp.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pfp.chenzaomai.com

while (std::getline(in, line)) { }
来源：http://hbp.dianchejie.cn

[S49] C++：写文件
来源：http://ccb.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yfs.zhixingplan.top

[S50] C++：格式化数字
来源：http://usc.zdqjudy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wni.xinyue.icu

[S51] C++：显式类型转换
来源：http://lvx.yanxiufei.cn

static_cast<double>(a) / b
来源：http://gfi.birdmap.top

[S52] C++：const 与 noexcept
来源：http://rqn.316326.xyz

int size() const noexcept { return n_; }
来源：http://caw.zhiwuduotai.top

[S53] C++：移动语义
来源：http://jji.yonumen.top

std::vector<int> w = std::move(v);
来源：http://bfh.andypj.xyz

[S54] C++：异常处理
来源：http://aut.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gbt.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://jgp.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://piv.shangyingyoupin.top

[S56] C++：optional
来源：http://fzd.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://irp.daxiang520.top

[S57] C++：编译期常量
来源：http://wba.cashguo.top

constexpr int N = 10;
来源：http://xtv.hcnkem.com

[S58] C++：命名空间
来源：http://zcz.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://dxh.zycfv.cn

[S59] C++：静态断言
来源：http://azp.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fed.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://ilf.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qjq.daria6918.cn

================================================================================
来源：http://vuk.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lns.316326.xyz

================================================================================
来源：http://xju.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://evv.zhoulong.xyz

println("Hello")
来源：http://dmk.bjfxy.top

[T02] Kotlin：变量
来源：http://evq.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://axk.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://dvd.chenzaomai.com

"值: $b"
来源：http://uvk.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://unx.hcnkem.com

val n: String? = null;  n?.length
来源：http://pwt.meibo888.top

[T05] Kotlin：when 表达式
来源：http://hqi.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tpx.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://pby.dashuyun.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fxd.hongshengwenyu.top

[T07] Kotlin：集合过滤
来源：http://vic.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dhh.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://eee.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://rkq.havefunace.top

[T09] Kotlin：扩展函数
来源：http://dyy.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://rgc.sxryk.cn

[T10] Kotlin：默认参数
来源：http://etx.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yje.vehdjk.com

[T11] Kotlin：协程
来源：http://tss.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mpl.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://tdi.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://ztb.cucudq.cn

[T13] Kotlin：只读 Map
来源：http://abj.aizwys.cn

val m = mapOf("a" to 1)
来源：http://uhj.snrcjt.cn

[T14] Kotlin：循环
来源：http://qef.birdmap.top

for (i in 1..10) println(i)
来源：http://bnl.sweek.top

[T15] Kotlin：接口
来源：http://gil.zhoulong.xyz

interface Shape { fun area(): Double }
来源：http://rme.wangdashe.top

[T16] Swift：Hello World
来源：http://arq.chenzaomai.com

print("Hello")
来源：http://qtc.xylfe.cn

[T17] Swift：变量与常量
来源：http://rmh.jinyuanbaomall.cn

var a = 1;  let b = 2
来源：http://twm.yonumen.top

[T18] Swift：字符串插值
来源：http://awx.zdqjudy.top

"值: \(b)"
来源：http://jnt.yuanzhike.top

[T19] Swift：可选绑定
来源：http://fec.sxryk.cn

if let n = opt { print(n) }
来源：http://gaz.jianghu66.top

[T20] Swift：数组操作
来源：http://onc.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pju.sjlbkw.cn

[T21] Swift：遍历
来源：http://hji.hfpthk.cn

for x in a { print(x) }
来源：http://mwq.vqdsnc.cn

[T22] Swift：字典
来源：http://pob.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://euo.cdnleiting.top

[T23] Swift：函数
来源：http://kok.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vzx.yonumen.top

[T24] Swift：闭包
来源：http://czj.sxryk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kno.zhixingplan.top

[T25] Swift：结构体
来源：http://xjg.aizwys.cn

struct P { var x: Int }
来源：http://wwk.yuxming.cn

[T26] Swift：类与重写
来源：http://zub.gotoacloud.top

class A: Base { override func f() {} }
来源：http://elu.pengpengdd.cyou

[T27] Swift：错误处理
来源：http://dip.wangshuangyany.cn

do { try f() } catch { print(error) }
来源：http://fmm.zycfv.cn

[T28] Swift：枚举
来源：http://mqj.cucudq.cn

enum Color { case red, green }
来源：http://bye.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://jyy.zhiwuduotai.top

guard let x = opt else { return }
来源：http://yrl.c1oappe.top

[T30] Swift：协议
来源：http://zdp.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://dno.bbcook.cn

[T31] Lua：Hello World
来源：http://nos.fktsv.cn

print("Hello")
来源：http://rwk.shangyingyoupin.top

[T32] Lua：局部变量
来源：http://uci.uphjek.com

local a = 1
来源：http://alw.ydzc1.top

[T33] Lua：表（数组）
来源：http://vnb.gzhubu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zhi.yuxming.cn

[T34] Lua：遍历表
来源：http://toz.yuxming.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mop.vqdsnc.cn

[T35] Lua：字典表
来源：http://uzw.havefunace.top

local d = { a = 1 };  d.b = 2
来源：http://kcn.shanyushiyangtech.top

[T36] Lua：函数
来源：http://dbg.ydjk.org.cn

function add(a, b) return a + b end
来源：http://nea.andypj.xyz

[T37] Lua：字符串拼接
来源：http://bcf.daria6918.cn

"a" .. "b"
来源：http://grq.wangdashe.top

[T38] Lua：条件
来源：http://vfs.guowangkeji.top

if x > 0 then print("正") end
来源：http://qlq.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://mbe.haohaochexian.top

string.find(s, "%d+")
来源：http://baq.jqgfzy.top

[T40] Lua：元表
来源：http://oxx.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://pvm.jinghuilouyu.cn

[T41] Perl：Hello World
来源：http://yur.xingfuxueyuan.xyz

print "Hello\n";
来源：http://aux.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://tbc.jlsjyb.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dtk.guowangkeji.top

[T43] Perl：字符串插值
来源：http://lbd.jiagoushi.top

"值: $a"
来源：http://frr.andypj.xyz

[T44] Perl：条件
来源：http://cuz.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://scg.c1oappe.top

[T45] Perl：数组遍历
来源：http://psu.gzhubu.top

for my $x (@arr) { print $x; }
来源：http://vnv.iojbl.cn

[T46] Perl：哈希操作
来源：http://uyj.shanyushiyangtech.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://spt.birdmap.top

[T47] Perl：正则捕获
来源：http://jgq.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sqg.c1oappe.top

[T48] Perl：正则替换
来源：http://xlq.vehdjk.com

$s =~ s/old/new/g;
来源：http://xbq.ydjk.org.cn

[T49] Perl：函数
来源：http://izl.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pra.iojbl.cn

[T50] Perl：逐行读文件
来源：http://fnh.zdqjudy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jpf.gotoacloud.top

while (my $line = <$fh>) { print $line; }
来源：http://daq.zdbjq.cn

[T51] Scala：Hello World
来源：http://vet.zhiwuduotai.top

println("Hello")
来源：http://wrv.9152youxi.cn

[T52] Scala：变量
来源：http://qyx.pycfn.com

val a = 1;  var b = 2
来源：http://yak.jianghu66.top

[T53] Scala：字符串插值
来源：http://fwy.yj20258888.top

s"值: $b"
来源：http://xgw.ywan-chungtsiang.top

[T54] Scala：集合映射
来源：http://wzh.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://krc.ppjwa.cn

[T55] Scala：集合过滤
来源：http://mws.hongshengwenyu.top

List(1, 2, 3).filter(_ > 1)
来源：http://ima.dashuyun.cn

[T56] Scala：样例类
来源：http://duc.sweek.top

case class User(name: String, age: Int)
来源：http://etz.shuidangran.top

[T57] Scala：模式匹配
来源：http://kbd.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://fmg.vehdjk.com

[T58] Scala：函数定义
来源：http://jch.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://fhw.hfpthk.cn

[T59] Scala：循环
来源：http://qen.9152youxi.cn

for (i <- 1 to 10) println(i)
来源：http://yja.nwbrower.top

[T60] Scala：折叠
来源：http://vub.jinqigufen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bhv.sweek.top

================================================================================
来源：http://btu.smart0.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nwb.zhiwuduotai.top

================================================================================
来源：http://lrt.sweek.top

[U01] Py：创建虚拟环境
来源：http://fyo.guannengcc.top

python -m venv .venv && source .venv/bin/activate
来源：http://lcg.zhoulong.xyz

[U02] Py：导出 / 安装依赖
来源：http://efr.nwbrower.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tzd.chenzaomai.com

[U03] Py：加载 .env 配置
来源：http://wif.xuetiantiany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lvz.chenzaomai.com

[U04] Py：变量调试打印
来源：http://wej.tanke756.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://utt.quarkkingdee.top

[U05] Py：列表去重且保序
来源：http://jbv.shzxlz.cn

list(dict.fromkeys(arr))
来源：http://nmv.fktsv.cn

[U06] Py：合并两个字典
来源：http://zeu.pycfn.com

{**a, **b}
来源：http://bvm.ydzc1.top

[U07] Py：反转字典键值
来源：http://esb.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://job.yangfankeji.com

[U08] Py：展平二维列表
来源：http://vrz.xinyue.icu

[y for x in nested for y in x]
来源：http://qpf.havefunace.top

[U09] Py：字典取最大值的键
来源：http://zif.nwbrower.top

max(d, key=d.get)
来源：http://ljr.cashguo.top

[U10] Py：按值排序字典
来源：http://lfo.cqqwz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pvx.jianghu66.top

[U11] Py：生成器表达式
来源：http://jes.aizwys.cn

(x * 2 for x in arr)
来源：http://nbz.chenjidiqi.icu

[U12] Py：取出现最多的 3 个元素
来源：http://aut.tian-w.cn

Counter(arr).most_common(3)
来源：http://nqd.jinqigufen.top

[U13] Py：固定长度队列
来源：http://qsv.sxryk.cn

deque(maxlen=10)
来源：http://lul.kuanghao11.cn

[U14] Py：分组收集到列表
来源：http://ftp.cucudq.cn

defaultdict(list)
来源：http://get.gzhubu.top

[U15] Py：高精度计时
来源：http://xti.sufxvd.cn

t = time.perf_counter()
来源：http://wlk.yueranfly.top

[U16] Py：命令行参数解析
来源：http://pme.epnwcf.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bza.sjlbkw.cn

[U17] Py：初始化日志
来源：http://rlz.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://dft.c1oappe.top

[U18] Py：预编译正则
来源：http://ztq.haohaochexian.top

pat = re.compile(r"\d+")
来源：http://tqp.yj20258888.top

[U19] Py：正则替换带回调
来源：http://pzr.ydzc1.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pxa.shanyushiyangkeji.top

[U20] Py：缓存函数结果
来源：http://kca.yj202588.top

@functools.lru_cache(maxsize=None)
来源：http://dmy.daxiang520.top

[U21] Py：自定义上下文管理器
来源：http://nif.tianlin.xyz

@contextlib.contextmanager
来源：http://dtw.bjfxy.top

[U22] Py：矩阵转置
来源：http://ugs.ppjwa.cn

list(zip(*m))
来源：http://mov.gzhubu.top

[U23] Py：分块读取大文件
来源：http://kbz.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cmd.zhongyouzk.top

[U24] Py：路径操作
来源：http://xpy.hywenlv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ery.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://wta.fehbvm.com

csv.DictReader(f)
来源：http://nid.shuidangran.top

[U26] Py：并发下载
来源：http://ilj.daria6918.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eed.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://cnv.ywan-chungtsiang.top

aiohttp.ClientSession() 配合 async with
来源：http://pua.daxiang520.top

[U28] Py：类型别名
来源：http://fgy.ydjk.org.cn

UserId = int
来源：http://pnh.zhaomingkeji.xyz

[U29] Py：属性校验
来源：http://tng.wangdashe.top

@property 与 @x.setter 配合
来源：http://rct.ywan-chungtsiang.top

[U30] Py：数据类
来源：http://lxs.yj20258888.top

@dataclass(slots=True)
来源：http://ehc.sysykeji.top

[U31] Py：单测
来源：http://pqv.yueranfly.top

python -m pytest -q
来源：http://mjo.316326.xyz

[U32] Py：代码格式化
来源：http://jib.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://bnf.sysykeji.top

[U33] Py：打包发布
来源：http://kel.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://yte.ydjk.org.cn

[U34] Py：判断编码
来源：http://hfg.jianghu66.top

chardet.detect(raw)
来源：http://fad.0kj1m.cn

[U35] Py：发送邮件
来源：http://swe.ehwqpu.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wzg.hammf.cn

[U36] Py：定时任务
来源：http://bop.jinyuanbaomall.cn

schedule.every(10).minutes.do(job)
来源：http://xku.jinghuilouyu.cn

[U37] Py：读写 Excel
来源：http://ifc.yangfankeji.com

pandas.read_excel / DataFrame.to_excel
来源：http://qvl.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://bec.zhijiandao.cn

Path(__file__).resolve().parent
来源：http://lmj.zhiwuduotai.top


<!-- 参考信息 -->