代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://jol.yueranfly.top

[S15] C：类型转换
来源：http://nio.guannengcc.top

(double) a / b
来源：http://ibv.yonumen.top

[S16] C：位操作置位
来源：http://xfu.ppjwa.cn

x |= (1 << 3);
来源：http://dgu.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://xdt.zycfv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lhv.snrcjt.cn

[S18] C：命令行参数
来源：http://vet.pengpengdd.cyou

int main(int argc, char **argv)
来源：http://hcj.ydjk.org.cn

[S19] C：快速排序
来源：http://rkm.xinyue.icu

qsort(a, n, sizeof(int), cmp);
来源：http://qqm.aibaodan.cn

[S20] C：二分查找
来源：http://ryr.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uqi.bjfxy.top

[S21] C：字符类别判断
来源：http://fgu.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oou.gaohongyu789.top

[S22] C：字符串转数字
来源：http://ibn.hywenlv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qcf.yuxming.cn

[S23] C：随机数
来源：http://tjz.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ezx.ydjk.org.cn

[S24] C：获取本地时间
来源：http://xgb.svipenyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tkp.redwolf501.top

[S25] C：内存拷贝
来源：http://nvf.sjlbkw.cn

memcpy(dst, src, n);
来源：http://uug.zhijiandao.cn

[S26] C：内存清零
来源：http://aax.gogol.net.cn

memset(a, 0, sizeof a);
来源：http://ywk.fanxiaobao.xyz

[S27] C：定义常量
来源：http://vnj.tian-w.cn

const double PI = 3.14159;
来源：http://qms.tian-w.cn

[S28] C：静态变量
来源：http://iwk.cheryme.top

static int counter = 0;
来源：http://zyw.havefunace.top

[S29] C：变参函数
来源：http://zoc.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mor.xylfe.cn

[S30] C：头文件保护
来源：http://yfk.fanxiaobao.xyz

#ifndef X_H
来源：http://nnn.pengpengdd.cyou

#define X_H
来源：http://xol.sjlbkw.cn

#endif
来源：http://trb.fzhhl.top

[S31] C++：Hello World
来源：http://pfy.xylfe.cn

#include <iostream>
来源：http://nak.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://zxa.tianlin.xyz

[S32] C++：字符串
来源：http://yfg.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://ozi.dashuyun.cn

[S33] C++：vector 增删
来源：http://uir.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mcq.yangfankeji.com

[S34] C++：遍历 vector
来源：http://qae.dianchejie.cn

for (auto &x : v) { std::cout << x; }
来源：http://pee.zdqjudy.top

[S35] C++：map
来源：http://ugh.9152youxi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blj.pycfn.com

[S36] C++：unordered_map
来源：http://ggq.ybcxt.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dks.ydjk.org.cn

[S37] C++：set
来源：http://oek.ctjpmb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bwl.wangshuangyany.cn

[S38] C++：排序
来源：http://ryb.cashguo.top

std::sort(v.begin(), v.end());
来源：http://gje.chenzaomai.com

[S39] C++：自定义比较器排序
来源：http://vue.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://agy.zhoulong.xyz

[S40] C++：查找元素
来源：http://xcx.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sje.ehwqpu.com

[S41] C++：类与构造函数
来源：http://kca.dianchejie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zqf.zycfv.cn

[S42] C++：继承与虚函数
来源：http://nbd.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://krd.bjfxy.top

[S43] C++：智能指针
来源：http://qpq.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://uhc.fzhhl.top

[S44] C++：引用传参
来源：http://mep.bjfxy.top

void inc(int &x) { ++x; }
来源：http://xpi.fzhhl.top

[S45] C++：lambda
来源：http://mjq.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://uhy.jinqigufen.top

[S46] C++：函数模板
来源：http://hek.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gcz.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://pfl.jinqigfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uuu.tianlin.xyz

[S48] C++：逐行读文件
来源：http://yed.shangyingyoupin.top

std::ifstream in("a.txt");  std::string line;
来源：http://esr.mhx1999.top

while (std::getline(in, line)) { }
来源：http://ial.chenjidiqi.icu

[S49] C++：写文件
来源：http://vkh.bjfxy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hlh.sjlbkw.cn

[S50] C++：格式化数字
来源：http://dlq.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ewz.yongpay.top

[S51] C++：显式类型转换
来源：http://nxa.0kj1m.cn

static_cast<double>(a) / b
来源：http://ksp.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://myi.yueranfly.top

int size() const noexcept { return n_; }
来源：http://npk.zdbjq.cn

[S53] C++：移动语义
来源：http://nmk.yj202588.top

std::vector<int> w = std::move(v);
来源：http://efq.yueranfly.top

[S54] C++：异常处理
来源：http://jfm.yonumen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fdv.316326.xyz

[S55] C++：结构化绑定
来源：http://cja.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://byw.jinghuilouyu.cn

[S56] C++：optional
来源：http://owm.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://onh.yj20258888.top

[S57] C++：编译期常量
来源：http://zoq.tarul.cn

constexpr int N = 10;
来源：http://mfc.jyoumei.cn

[S58] C++：命名空间
来源：http://pst.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://zvt.sweek.top

[S59] C++：静态断言
来源：http://aof.jinqigufen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wwo.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://thf.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vip.nwbrower.top

================================================================================
来源：http://omx.ybcxt.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lzb.tanke756.top

================================================================================
来源：http://pvf.jinyuanbaomall.cn

[T01] Kotlin：Hello World
来源：http://nyw.sjlbkw.cn

println("Hello")
来源：http://mal.hammf.cn

[T02] Kotlin：变量
来源：http://uhn.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://axy.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://rsn.chenjidiqi.icu

"值: $b"
来源：http://uyv.havefunace.top

[T04] Kotlin：空安全
来源：http://rmm.aizwys.cn

val n: String? = null;  n?.length
来源：http://ogh.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://quj.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vek.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://nkp.ydjk.org.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xrl.zycfv.cn

[T07] Kotlin：集合过滤
来源：http://mnp.ctjpmb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://zxa.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://opo.yj202588.top

data class User(val name: String, val age: Int)
来源：http://xfm.chenlongwang.top

[T09] Kotlin：扩展函数
来源：http://vxy.vehdjk.com

fun String.exclaim() = this + "!"
来源：http://hqq.tian-w.cn

[T10] Kotlin：默认参数
来源：http://cqa.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://grb.zycfv.cn

[T11] Kotlin：协程
来源：http://quy.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://yua.chenjidiqi.icu

[T12] Kotlin：解构声明
来源：http://apw.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://zcj.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://dfl.guannengcc.top

val m = mapOf("a" to 1)
来源：http://qqr.daria6918.cn

[T14] Kotlin：循环
来源：http://zzg.xylfe.cn

for (i in 1..10) println(i)
来源：http://awe.dianchejie.cn

[T15] Kotlin：接口
来源：http://pds.hysaishi.cn

interface Shape { fun area(): Double }
来源：http://inf.sjlbkw.cn

[T16] Swift：Hello World
来源：http://yzl.yj202588.top

print("Hello")
来源：http://flw.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://jxh.sweek.top

var a = 1;  let b = 2
来源：http://ypl.hammf.cn

[T18] Swift：字符串插值
来源：http://oyw.andypj.xyz

"值: \(b)"
来源：http://gkq.zdbjq.cn

[T19] Swift：可选绑定
来源：http://hey.epnwcf.com

if let n = opt { print(n) }
来源：http://sfd.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://zlb.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ros.redwolf501.top

[T21] Swift：遍历
来源：http://hga.ctjpmb.com

for x in a { print(x) }
来源：http://upt.guannengcc.top

[T22] Swift：字典
来源：http://qcy.ywan-chungtsiang.top

var d = ["a": 1];  d["b"] = 2
来源：http://fzc.guowangkeji.top

[T23] Swift：函数
来源：http://irg.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bze.hnxiangtu.top

[T24] Swift：闭包
来源：http://ula.sufxvd.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pov.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://ujn.sufxvd.cn

struct P { var x: Int }
来源：http://ruu.hesvh.cn

[T26] Swift：类与重写
来源：http://ccl.meibo888.top

class A: Base { override func f() {} }
来源：http://skc.hcnkem.com

[T27] Swift：错误处理
来源：http://cpz.chenlongwang.top

do { try f() } catch { print(error) }
来源：http://een.c1oappe.top

[T28] Swift：枚举
来源：http://two.kuanghao11.cn

enum Color { case red, green }
来源：http://oqb.ctjpmb.com

[T29] Swift：guard 提前返回
来源：http://gbx.jianghu66.top

guard let x = opt else { return }
来源：http://cng.quarkkingdee.top

[T30] Swift：协议
来源：http://dtn.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://rur.tian-w.cn

[T31] Lua：Hello World
来源：http://kri.epnwcf.com

print("Hello")
来源：http://fvh.yueranfly.top

[T32] Lua：局部变量
来源：http://tth.sufxvd.cn

local a = 1
来源：http://sqg.bbcook.cn

[T33] Lua：表（数组）
来源：http://wbb.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bdx.smart0.xyz

[T34] Lua：遍历表
来源：http://xpc.jqgfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qye.nwbrower.top

[T35] Lua：字典表
来源：http://pul.bjfxy.top

local d = { a = 1 };  d.b = 2
来源：http://amw.yuxming.cn

[T36] Lua：函数
来源：http://kpf.wangshuangyany.cn

function add(a, b) return a + b end
来源：http://zuo.zhoulong.xyz

[T37] Lua：字符串拼接
来源：http://cjz.sweek.top

"a" .. "b"
来源：http://hda.yfazqb.com

[T38] Lua：条件
来源：http://qbi.svipenyu.cn

if x > 0 then print("正") end
来源：http://cgn.chenlongwang.top

[T39] Lua：模式匹配
来源：http://kyk.yj20258.top

string.find(s, "%d+")
来源：http://rhe.nwbrower.top

[T40] Lua：元表
来源：http://wob.316326.xyz

setmetatable({}, { __index = base })
来源：http://xtv.zhixingplan.top

[T41] Perl：Hello World
来源：http://nmc.c1oappe.top

print "Hello\n";
来源：http://arr.yonumen.top

[T42] Perl：变量类型
来源：http://mhi.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://byk.pycfn.com

[T43] Perl：字符串插值
来源：http://ofa.9152youxi.cn

"值: $a"
来源：http://cjq.xuanzx.com

[T44] Perl：条件
来源：http://rxh.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://qxm.c1oappe.top

[T45] Perl：数组遍历
来源：http://fni.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://jbh.dashuyun.cn

[T46] Perl：哈希操作
来源：http://qms.jyoumei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kym.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://zqi.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xwf.xingfuxueyuan.xyz

[T48] Perl：正则替换
来源：http://wug.c1oappe.top

$s =~ s/old/new/g;
来源：http://wtm.havefunace.top

[T49] Perl：函数
来源：http://kxm.uphjek.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://udo.fehbvm.com

[T50] Perl：逐行读文件
来源：http://ani.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dwk.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://iws.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://khu.yj20258888.top

println("Hello")
来源：http://jhj.sweek.top

[T52] Scala：变量
来源：http://bat.chenjidiqi.icu

val a = 1;  var b = 2
来源：http://ecr.shanyushiyangtech.top

[T53] Scala：字符串插值
来源：http://sdt.nanxinkj.top

s"值: $b"
来源：http://vih.vehdjk.com

[T54] Scala：集合映射
来源：http://jvx.wangshuangyany.cn

List(1, 2, 3).map(_ * 2)
来源：http://yal.ybcxt.top

[T55] Scala：集合过滤
来源：http://ufq.pycfn.com

List(1, 2, 3).filter(_ > 1)
来源：http://sxh.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://son.vqdsnc.cn

case class User(name: String, age: Int)
来源：http://bfo.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://yut.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://nwh.jyoumei.cn

[T58] Scala：函数定义
来源：http://gst.yonumen.top

def add(a: Int, b: Int): Int = a + b
来源：http://hom.xylfe.cn

[T59] Scala：循环
来源：http://qda.pycfn.com

for (i <- 1 to 10) println(i)
来源：http://agd.0kj1m.cn

[T60] Scala：折叠
来源：http://xfp.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ztv.sweek.top

================================================================================
来源：http://mes.yvedp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oon.iojbl.cn

================================================================================
来源：http://gya.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://dxe.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://dvk.yanxiufei.cn

[U02] Py：导出 / 安装依赖
来源：http://jtb.cheryme.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qkp.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://srp.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dgu.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://rbp.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xuw.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://xcy.jlsjyb.cn

list(dict.fromkeys(arr))
来源：http://dph.vqdsnc.cn

[U06] Py：合并两个字典
来源：http://hyy.sweek.top

{**a, **b}
来源：http://dyl.jinqigufen.top

[U07] Py：反转字典键值
来源：http://cfv.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://qzs.nanxuanxn.top

[U08] Py：展平二维列表
来源：http://mkw.52xcode.cn

[y for x in nested for y in x]
来源：http://yvp.dashuyun.cn

[U09] Py：字典取最大值的键
来源：http://wbb.ehwqpu.com

max(d, key=d.get)
来源：http://tfp.fehbvm.com

[U10] Py：按值排序字典
来源：http://ieq.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pkz.gaohongyu789.top

[U11] Py：生成器表达式
来源：http://yer.zhengqikj.top

(x * 2 for x in arr)
来源：http://jgc.jqgfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://hnx.fanxiaobao.xyz

Counter(arr).most_common(3)
来源：http://xgc.shangyingyoupin.top

[U13] Py：固定长度队列
来源：http://jkw.hfpthk.cn

deque(maxlen=10)
来源：http://vmc.zhiwuduotai.top

[U14] Py：分组收集到列表
来源：http://pcs.yangfankeji.com

defaultdict(list)
来源：http://ydr.yj20258888.top

[U15] Py：高精度计时
来源：http://ioo.pengpengdd.cyou

t = time.perf_counter()
来源：http://ctk.jlsjyb.cn

[U16] Py：命令行参数解析
来源：http://pcs.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cng.sysykeji.top

[U17] Py：初始化日志
来源：http://mbd.aibaodan.cn

logging.basicConfig(level=logging.INFO)
来源：http://wfn.yuanzhike.top

[U18] Py：预编译正则
来源：http://lyp.vehdjk.com

pat = re.compile(r"\d+")
来源：http://unu.mhx1999.top

[U19] Py：正则替换带回调
来源：http://opy.dianchejie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uqm.redwolf501.top

[U20] Py：缓存函数结果
来源：http://kvl.haohaochexian.top

@functools.lru_cache(maxsize=None)
来源：http://uxi.xuanzx.com

[U21] Py：自定义上下文管理器
来源：http://xgc.jinqigfzy.top

@contextlib.contextmanager
来源：http://wyh.redwolf501.top

[U22] Py：矩阵转置
来源：http://cpq.bjfxy.top

list(zip(*m))
来源：http://pxv.tianlin.xyz

[U23] Py：分块读取大文件
来源：http://rpm.zhiwuduotai.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kdj.cucudq.cn

[U24] Py：路径操作
来源：http://hou.gzhubu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://arg.meibo888.top

[U25] Py：CSV 按字典读
来源：http://qae.redwolf501.top

csv.DictReader(f)
来源：http://nsd.shangyingyoupin.top

[U26] Py：并发下载
来源：http://kmz.jinqigufen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dew.aizwys.cn

[U27] Py：异步 HTTP
来源：http://wsu.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://yfr.ctjpmb.com

[U28] Py：类型别名
来源：http://vgb.xuetiantiany.cn

UserId = int
来源：http://hnp.redwolf501.top

[U29] Py：属性校验
来源：http://ryq.ydzc1.top

@property 与 @x.setter 配合
来源：http://ljx.yj20258.top

[U30] Py：数据类
来源：http://llc.haohaochexian.top

@dataclass(slots=True)
来源：http://lhq.yj20258.top

[U31] Py：单测
来源：http://izq.hfpthk.cn

python -m pytest -q
来源：http://uzj.kuanghao11.cn

[U32] Py：代码格式化
来源：http://mmw.shangyingyoupin.top

ruff format . && ruff check --fix .
来源：http://arb.316326.xyz

[U33] Py：打包发布
来源：http://hza.aizwys.cn

python -m build  （依赖 pyproject.toml）
来源：http://zrz.snrcjt.cn

[U34] Py：判断编码
来源：http://arp.zhijiandao.cn

chardet.detect(raw)
来源：http://mbc.shzxlz.cn

[U35] Py：发送邮件
来源：http://amf.fktsv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xxm.zhengqikj.top

[U36] Py：定时任务
来源：http://mdo.meibo888.top

schedule.every(10).minutes.do(job)
来源：http://nef.zhixingplan.top

[U37] Py：读写 Excel
来源：http://tpx.daria6918.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pae.zhengqikj.top

[U38] Py：获取脚本所在目录
来源：http://xrj.ywan-chungtsiang.top

Path(__file__).resolve().parent
来源：http://ixf.bbcook.cn


<!-- 参考信息 -->