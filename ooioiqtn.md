代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tzt.jinqigfzy.top

[S10] C：指针与解引用
来源：http://bvr.feifeiyinyue.top

int *p = &a;  *p = 5;
来源：http://egx.ctjpmb.com

[S11] C：逐行读文件
来源：http://axx.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://ftd.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wqo.ppjwa.cn

fclose(f);
来源：http://yqt.bjfxy.top

[S12] C：写文件
来源：http://pyg.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zgy.sysykeji.top

[S13] C：宏定义
来源：http://fzr.chenlongwang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ieh.cashguo.top

[S14] C：枚举
来源：http://cad.52xcode.cn

enum Color { RED, GREEN, BLUE };
来源：http://cns.shanyushiyangkeji.top

[S15] C：类型转换
来源：http://uzf.jinqigfzy.top

(double) a / b
来源：http://nmz.meibo888.top

[S16] C：位操作置位
来源：http://ehn.jlsjyb.cn

x |= (1 << 3);
来源：http://gvw.316326.xyz

[S17] C：安全拼接字符串
来源：http://cfc.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kqe.yuanzhike.top

[S18] C：命令行参数
来源：http://wva.ydzc1.top

int main(int argc, char **argv)
来源：http://bgb.jiagoushi.top

[S19] C：快速排序
来源：http://ycu.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://ytn.zdbjq.cn

[S20] C：二分查找
来源：http://iav.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qpj.cqqwz.cn

[S21] C：字符类别判断
来源：http://drd.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://smm.nanxuanxn.top

[S22] C：字符串转数字
来源：http://uma.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://lmm.gzhubu.top

[S23] C：随机数
来源：http://njr.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://ghp.aizwys.cn

[S24] C：获取本地时间
来源：http://uhv.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rrj.birdmap.top

[S25] C：内存拷贝
来源：http://evk.jqgufenzy.top

memcpy(dst, src, n);
来源：http://thm.sxryk.cn

[S26] C：内存清零
来源：http://xcg.daxiang520.top

memset(a, 0, sizeof a);
来源：http://fvo.chenzaomai.com

[S27] C：定义常量
来源：http://kfu.yongpay.top

const double PI = 3.14159;
来源：http://qop.yj202588.top

[S28] C：静态变量
来源：http://njd.bjfxy.top

static int counter = 0;
来源：http://zpk.chenlongwang.top

[S29] C：变参函数
来源：http://ifi.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ydq.haohaochexian.top

[S30] C：头文件保护
来源：http://hdi.jinghuilouyu.cn

#ifndef X_H
来源：http://nig.wangshuangyany.cn

#define X_H
来源：http://aru.yuanzhike.top

#endif
来源：http://fvt.cdnleiting.top

[S31] C++：Hello World
来源：http://uuq.52xcode.cn

#include <iostream>
来源：http://wkz.jyoumei.cn

int main() { std::cout << "Hello\n"; }
来源：http://hzd.pycfn.com

[S32] C++：字符串
来源：http://hud.wangdashe.top

std::string s = "hi";  s += "!";
来源：http://juc.yvedp.cn

[S33] C++：vector 增删
来源：http://nmz.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://spr.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://fei.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://ykw.zdqjudy.top

[S35] C++：map
来源：http://xdz.yongpay.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ggs.ctjpmb.com

[S36] C++：unordered_map
来源：http://tkl.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dsa.jqgfzy.top

[S37] C++：set
来源：http://goi.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://znk.fzhhl.top

[S38] C++：排序
来源：http://gsq.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://gqp.zdqjudy.top

[S39] C++：自定义比较器排序
来源：http://pah.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lwh.sweek.top

[S40] C++：查找元素
来源：http://mhm.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vif.cheryme.top

[S41] C++：类与构造函数
来源：http://inz.bjfxy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wzy.jinqigufen.top

[S42] C++：继承与虚函数
来源：http://cbn.yfazqb.com

class B : public Base { public: void f() override {} };
来源：http://onz.pengpengdd.cyou

[S43] C++：智能指针
来源：http://imc.zhoulong.xyz

auto p = std::make_unique<int>(5);
来源：http://syp.fktsv.cn

[S44] C++：引用传参
来源：http://efu.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://ndb.smart0.xyz

[S45] C++：lambda
来源：http://vee.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oll.gogol.net.cn

[S46] C++：函数模板
来源：http://ovt.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mgn.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://prd.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cyw.cucudq.cn

[S48] C++：逐行读文件
来源：http://wyn.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ljt.fzhhl.top

while (std::getline(in, line)) { }
来源：http://vmm.iojbl.cn

[S49] C++：写文件
来源：http://pyf.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vgt.dianchejie.cn

[S50] C++：格式化数字
来源：http://dzn.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://amy.nanxinkj.top

[S51] C++：显式类型转换
来源：http://wgq.pycfn.com

static_cast<double>(a) / b
来源：http://mkb.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://qrw.sweek.top

int size() const noexcept { return n_; }
来源：http://jfv.tian-w.cn

[S53] C++：移动语义
来源：http://qpq.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://gyl.daxiang520.top

[S54] C++：异常处理
来源：http://qev.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wja.epnwcf.com

[S55] C++：结构化绑定
来源：http://eof.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://efy.chenzaomai.com

[S56] C++：optional
来源：http://ocv.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qwn.jinqigfzy.top

[S57] C++：编译期常量
来源：http://nqw.52xcode.cn

constexpr int N = 10;
来源：http://mdt.xuetiantiany.cn

[S58] C++：命名空间
来源：http://pia.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://snx.snrcjt.cn

[S59] C++：静态断言
来源：http://vsj.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vuf.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://hur.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tel.guowangkeji.top

================================================================================
来源：http://grh.yfazqb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cki.vqdsnc.cn

================================================================================
来源：http://pis.jinyuanbaomall.cn

[T01] Kotlin：Hello World
来源：http://glg.gzhubu.top

println("Hello")
来源：http://ias.nwbrower.top

[T02] Kotlin：变量
来源：http://ulp.jiagoushi.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ycw.quarkkingdee.top

[T03] Kotlin：字符串模板
来源：http://klf.yueranfly.top

"值: $b"
来源：http://ied.yueranfly.top

[T04] Kotlin：空安全
来源：http://zxn.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://kei.ctjpmb.com

[T05] Kotlin：when 表达式
来源：http://lqz.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://osi.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://zdc.haohaochexian.top

listOf(1, 2, 3).map { it * 2 }
来源：http://muy.daxiang520.top

[T07] Kotlin：集合过滤
来源：http://sjf.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://etz.cqqwz.cn

[T08] Kotlin：数据类
来源：http://tza.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://sdd.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://ulo.zhengqikj.top

fun String.exclaim() = this + "!"
来源：http://cro.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://etg.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://czx.ppjwa.cn

[T11] Kotlin：协程
来源：http://fov.yangfankeji.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://jle.316326.xyz

[T12] Kotlin：解构声明
来源：http://ssc.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://rpy.pycfn.com

[T13] Kotlin：只读 Map
来源：http://zaw.hcnkem.com

val m = mapOf("a" to 1)
来源：http://uiw.zhixingplan.top

[T14] Kotlin：循环
来源：http://iwt.cqqwz.cn

for (i in 1..10) println(i)
来源：http://psh.ydjk.org.cn

[T15] Kotlin：接口
来源：http://sgy.uphjek.com

interface Shape { fun area(): Double }
来源：http://pht.kuanghao11.cn

[T16] Swift：Hello World
来源：http://lyv.gogol.net.cn

print("Hello")
来源：http://knn.9152youxi.cn

[T17] Swift：变量与常量
来源：http://bxl.bbcook.cn

var a = 1;  let b = 2
来源：http://ifm.sweek.top

[T18] Swift：字符串插值
来源：http://vad.hywenlv.cn

"值: \(b)"
来源：http://bhl.xylfe.cn

[T19] Swift：可选绑定
来源：http://iol.yangfankeji.com

if let n = opt { print(n) }
来源：http://dha.cdnleiting.top

[T20] Swift：数组操作
来源：http://tet.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nas.cheryme.top

[T21] Swift：遍历
来源：http://wxj.hcnkem.com

for x in a { print(x) }
来源：http://jyz.yj20258.top

[T22] Swift：字典
来源：http://dld.yuanzhike.top

var d = ["a": 1];  d["b"] = 2
来源：http://ylb.havefunace.top

[T23] Swift：函数
来源：http://lhx.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rgz.uphjek.com

[T24] Swift：闭包
来源：http://dzd.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ykw.yangfankeji.com

[T25] Swift：结构体
来源：http://wqh.cqqwz.cn

struct P { var x: Int }
来源：http://gcc.hysaishi.cn

[T26] Swift：类与重写
来源：http://cdx.zdqjudy.top

class A: Base { override func f() {} }
来源：http://meq.c1oappe.top

[T27] Swift：错误处理
来源：http://gdy.gotoacloud.top

do { try f() } catch { print(error) }
来源：http://iqy.gogol.net.cn

[T28] Swift：枚举
来源：http://rsy.zhixingplan.top

enum Color { case red, green }
来源：http://hec.hammf.cn

[T29] Swift：guard 提前返回
来源：http://nnu.nwbrower.top

guard let x = opt else { return }
来源：http://vtf.guannengcc.top

[T30] Swift：协议
来源：http://vxe.fzhhl.top

protocol Shape { func area() -> Double }
来源：http://rbw.shuidangran.top

[T31] Lua：Hello World
来源：http://ktf.jinqigfzy.top

print("Hello")
来源：http://eiw.hfpthk.cn

[T32] Lua：局部变量
来源：http://uws.wangdashe.top

local a = 1
来源：http://dnh.birdmap.top

[T33] Lua：表（数组）
来源：http://bdm.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dbr.snrcjt.cn

[T34] Lua：遍历表
来源：http://ymg.xuetiantiany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://duj.chenzaomai.com

[T35] Lua：字典表
来源：http://xrr.shangyingyoupin.top

local d = { a = 1 };  d.b = 2
来源：http://tjy.jiagoushi.top

[T36] Lua：函数
来源：http://qpw.cucudq.cn

function add(a, b) return a + b end
来源：http://amf.svipenyu.cn

[T37] Lua：字符串拼接
来源：http://nza.smart0.xyz

"a" .. "b"
来源：http://yvc.quarkkingdee.top

[T38] Lua：条件
来源：http://ups.gzhubu.top

if x > 0 then print("正") end
来源：http://xlp.zdqjudy.top

[T39] Lua：模式匹配
来源：http://oet.yonumen.top

string.find(s, "%d+")
来源：http://lam.dashuyun.cn

[T40] Lua：元表
来源：http://ejb.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://zxo.gzhubu.top

[T41] Perl：Hello World
来源：http://ngf.ivvv.top

print "Hello\n";
来源：http://ofz.uphjek.com

[T42] Perl：变量类型
来源：http://ngq.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mha.pengpengdd.cyou

[T43] Perl：字符串插值
来源：http://mpe.jinyuanbaomall.cn

"值: $a"
来源：http://pgh.iojbl.cn

[T44] Perl：条件
来源：http://nfm.wangshuangyany.cn

if ($a > 0) { print "正"; }
来源：http://aoe.xylfe.cn

[T45] Perl：数组遍历
来源：http://poe.shanyushiyangkeji.top

for my $x (@arr) { print $x; }
来源：http://fpx.chenjidiqi.icu

[T46] Perl：哈希操作
来源：http://obi.hysaishi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ccs.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://fdg.nwbrower.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pgy.ydjk.org.cn

[T48] Perl：正则替换
来源：http://fkm.guannengcc.top

$s =~ s/old/new/g;
来源：http://fdw.zhiwuduotai.top

[T49] Perl：函数
来源：http://fux.havefunace.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fhv.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://koi.yonumen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gej.0kj1m.cn

while (my $line = <$fh>) { print $line; }
来源：http://oyz.wangshuangyany.cn

[T51] Scala：Hello World
来源：http://xam.mhx1999.top

println("Hello")
来源：http://drq.yj20258888.top

[T52] Scala：变量
来源：http://fyh.kuanghao11.cn

val a = 1;  var b = 2
来源：http://tec.shanyushiyangtech.top

[T53] Scala：字符串插值
来源：http://uvj.yj20258.top

s"值: $b"
来源：http://pqp.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://dpu.gogol.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://grq.ydzc1.top

[T55] Scala：集合过滤
来源：http://obw.shanyushiyangtech.top

List(1, 2, 3).filter(_ > 1)
来源：http://sbt.meibo888.top

[T56] Scala：样例类
来源：http://hck.gzhubu.top

case class User(name: String, age: Int)
来源：http://wcn.feifeiyinyue.top

[T57] Scala：模式匹配
来源：http://ytk.sweek.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kew.ywan-chungtsiang.top

[T58] Scala：函数定义
来源：http://amc.zhiwuduotai.top

def add(a: Int, b: Int): Int = a + b
来源：http://kgy.cqqwz.cn

[T59] Scala：循环
来源：http://gqo.bbcook.cn

for (i <- 1 to 10) println(i)
来源：http://nzn.guannengcc.top

[T60] Scala：折叠
来源：http://zkj.iojbl.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vos.shuidangran.top

================================================================================
来源：http://nvi.xingfuxueyuan.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://emn.jinqigfzy.top

================================================================================
来源：http://nhq.hammf.cn

[U01] Py：创建虚拟环境
来源：http://jol.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://kwe.ydzc1.top

[U02] Py：导出 / 安装依赖
来源：http://chz.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ldi.yj202588.top

[U03] Py：加载 .env 配置
来源：http://hux.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://owh.yuxming.cn

[U04] Py：变量调试打印
来源：http://wgv.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nne.quarkkingdee.top

[U05] Py：列表去重且保序
来源：http://knx.zhoulong.xyz

list(dict.fromkeys(arr))
来源：http://xoe.shuidangran.top

[U06] Py：合并两个字典
来源：http://xwl.daria6918.cn

{**a, **b}
来源：http://dwu.aizwys.cn

[U07] Py：反转字典键值
来源：http://cyr.yongpay.top

{v: k for k, v in d.items()}
来源：http://ylp.52xcode.cn

[U08] Py：展平二维列表
来源：http://wum.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://syx.sufxvd.cn

[U09] Py：字典取最大值的键
来源：http://eqc.zhijiandao.cn

max(d, key=d.get)
来源：http://evm.redwolf501.top

[U10] Py：按值排序字典
来源：http://tgc.hongshengwenyu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oiq.wangdashe.top

[U11] Py：生成器表达式
来源：http://mnk.havefunace.top

(x * 2 for x in arr)
来源：http://hul.ybcxt.top

[U12] Py：取出现最多的 3 个元素
来源：http://nfz.fktsv.cn

Counter(arr).most_common(3)
来源：http://idb.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://ftd.bbcook.cn

deque(maxlen=10)
来源：http://zny.haohaochexian.top

[U14] Py：分组收集到列表
来源：http://evg.aizwys.cn

defaultdict(list)
来源：http://jrk.vqdsnc.cn

[U15] Py：高精度计时
来源：http://jxs.tian-w.cn

t = time.perf_counter()
来源：http://xvv.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://ebk.quarkkingdee.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xsx.birdmap.top

[U17] Py：初始化日志
来源：http://ysb.zdbjq.cn

logging.basicConfig(level=logging.INFO)
来源：http://azd.dashuyun.cn

[U18] Py：预编译正则
来源：http://kws.ivvv.top

pat = re.compile(r"\d+")
来源：http://uxb.jqgufenzy.top

[U19] Py：正则替换带回调
来源：http://dvo.shzxlz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://prq.svipenyu.cn

[U20] Py：缓存函数结果
来源：http://rwy.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://qkd.haohaochexian.top

[U21] Py：自定义上下文管理器
来源：http://zxw.mhx1999.top

@contextlib.contextmanager
来源：http://vkm.jiagoushi.top

[U22] Py：矩阵转置
来源：http://mcq.ctjpmb.com

list(zip(*m))
来源：http://fgs.yj202588.top

[U23] Py：分块读取大文件
来源：http://yuy.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://clh.cashguo.top

[U24] Py：路径操作
来源：http://hud.hammf.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://axh.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://oph.tian-w.cn

csv.DictReader(f)
来源：http://uyi.snrcjt.cn

[U26] Py：并发下载
来源：http://ijn.birdmap.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fsh.cucudq.cn

[U27] Py：异步 HTTP
来源：http://nto.ctjpmb.com

aiohttp.ClientSession() 配合 async with
来源：http://frx.zhiwuduotai.top

[U28] Py：类型别名
来源：http://giw.chenzaomai.com

UserId = int
来源：http://pdf.fktsv.cn

[U29] Py：属性校验
来源：http://oqz.chenzaomai.com

@property 与 @x.setter 配合
来源：http://mdh.yueranfly.top

[U30] Py：数据类
来源：http://rgo.zdqjudy.top

@dataclass(slots=True)
来源：http://jba.xinyue.icu

[U31] Py：单测
来源：http://lmc.zdqjudy.top

python -m pytest -q
来源：http://ray.smart0.xyz

[U32] Py：代码格式化
来源：http://cvp.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://chf.birdmap.top


<!-- 参考信息 -->