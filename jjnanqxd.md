代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ukq.xziqi.cn

[S10] C：指针与解引用
来源：http://wla.cashguo.top

int *p = &a;  *p = 5;
来源：http://qib.yj20258.top

[S11] C：逐行读文件
来源：http://kul.havefunace.top

FILE *f = fopen("a.txt", "r");
来源：http://nix.zhixingplan.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xdf.feifeiyinyue.top

fclose(f);
来源：http://kzu.yfazqb.com

[S12] C：写文件
来源：http://wnc.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hcf.pycfn.com

[S13] C：宏定义
来源：http://rpo.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://chd.yuanzhike.top

[S14] C：枚举
来源：http://pqe.gotoacloud.top

enum Color { RED, GREEN, BLUE };
来源：http://swf.chenjidiqi.icu

[S15] C：类型转换
来源：http://pfk.hfpthk.cn

(double) a / b
来源：http://ytb.xuanzx.com

[S16] C：位操作置位
来源：http://vwy.yueranfly.top

x |= (1 << 3);
来源：http://ylr.cashguo.top

[S17] C：安全拼接字符串
来源：http://ytp.jianghu66.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bas.hcnkem.com

[S18] C：命令行参数
来源：http://frc.cdnleiting.top

int main(int argc, char **argv)
来源：http://yrz.uphjek.com

[S19] C：快速排序
来源：http://mgo.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://qho.chenzaomai.com

[S20] C：二分查找
来源：http://wuw.ivvv.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jvg.gaohongyu789.top

[S21] C：字符类别判断
来源：http://lav.cashguo.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://byc.quarkkingdee.top

[S22] C：字符串转数字
来源：http://zbu.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://hep.aibaodan.cn

[S23] C：随机数
来源：http://gru.52xcode.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://knt.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://hdp.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bmq.fzhhl.top

[S25] C：内存拷贝
来源：http://fci.tian-w.cn

memcpy(dst, src, n);
来源：http://xml.fanxiaobao.xyz

[S26] C：内存清零
来源：http://ppc.haohaochexian.top

memset(a, 0, sizeof a);
来源：http://ogh.jinqigufen.top

[S27] C：定义常量
来源：http://axj.yj20258.top

const double PI = 3.14159;
来源：http://psk.ydjk.org.cn

[S28] C：静态变量
来源：http://gfw.jinqigfzy.top

static int counter = 0;
来源：http://vwn.ydjk.org.cn

[S29] C：变参函数
来源：http://rrl.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zsb.zdbjq.cn

[S30] C：头文件保护
来源：http://hdc.fanxiaobao.xyz

#ifndef X_H
来源：http://ihd.yangfankeji.com

#define X_H
来源：http://cxv.shangyingyoupin.top

#endif
来源：http://rsm.ctjpmb.com

[S31] C++：Hello World
来源：http://fsx.fzhhl.top

#include <iostream>
来源：http://kja.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://eqd.fzhhl.top

[S32] C++：字符串
来源：http://rai.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://fjm.sysykeji.top

[S33] C++：vector 增删
来源：http://bqk.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ahl.yuxming.cn

[S34] C++：遍历 vector
来源：http://moy.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://sgf.wangshuangyany.cn

[S35] C++：map
来源：http://nwb.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pwk.redwolf501.top

[S36] C++：unordered_map
来源：http://imn.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ahf.dianchejie.cn

[S37] C++：set
来源：http://gee.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cds.yuanzhike.top

[S38] C++：排序
来源：http://xby.fengsongda.top

std::sort(v.begin(), v.end());
来源：http://los.epnwcf.com

[S39] C++：自定义比较器排序
来源：http://wuz.0kj1m.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dsd.sweek.top

[S40] C++：查找元素
来源：http://usx.hysaishi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wld.cdnleiting.top

[S41] C++：类与构造函数
来源：http://xdd.haohaochexian.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vfk.birdmap.top

[S42] C++：继承与虚函数
来源：http://mjk.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://vuq.zhiwuduotai.top

[S43] C++：智能指针
来源：http://shk.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://vke.cashguo.top

[S44] C++：引用传参
来源：http://pvv.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://ybb.hywenlv.cn

[S45] C++：lambda
来源：http://lea.jinyuanbaomall.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nth.hcnkem.com

[S46] C++：函数模板
来源：http://vje.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ein.shangyingyoupin.top

[S47] C++：结构化绑定遍历
来源：http://juf.jinqigfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dmt.hongshengwenyu.top

[S48] C++：逐行读文件
来源：http://mlg.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gvx.yueranfly.top

while (std::getline(in, line)) { }
来源：http://nys.wangdashe.top

[S49] C++：写文件
来源：http://lxu.yangfankeji.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ctw.jinqigufen.top

[S50] C++：格式化数字
来源：http://spb.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ebg.dianchejie.cn

[S51] C++：显式类型转换
来源：http://buw.sysykeji.top

static_cast<double>(a) / b
来源：http://apg.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://fxv.xylfe.cn

int size() const noexcept { return n_; }
来源：http://vjy.pycfn.com

[S53] C++：移动语义
来源：http://gnj.iojbl.cn

std::vector<int> w = std::move(v);
来源：http://gwu.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://bvo.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yzc.sxryk.cn

[S55] C++：结构化绑定
来源：http://wzs.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://idy.zhaomingkeji.xyz

[S56] C++：optional
来源：http://nez.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ziz.shuidangran.top

[S57] C++：编译期常量
来源：http://eqi.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://kal.ivvv.top

[S58] C++：命名空间
来源：http://dmr.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://oak.yuxming.cn

[S59] C++：静态断言
来源：http://mpn.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pcn.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://lga.jqgufenzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ple.yueranfly.top

================================================================================
来源：http://dkt.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qxq.yvedp.cn

================================================================================
来源：http://ibg.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://fac.jqgufenzy.top

println("Hello")
来源：http://oik.ctjpmb.com

[T02] Kotlin：变量
来源：http://cpx.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zem.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://hcb.yvedp.cn

"值: $b"
来源：http://zkc.xinyue.icu

[T04] Kotlin：空安全
来源：http://wjg.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://ytf.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://jbb.snrcjt.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cpo.ydjk.org.cn

[T06] Kotlin：集合映射
来源：http://qtf.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://mbu.hammf.cn

[T07] Kotlin：集合过滤
来源：http://tfr.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://deb.zhoulong.xyz

[T08] Kotlin：数据类
来源：http://hsq.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://yqb.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://shv.pycfn.com

fun String.exclaim() = this + "!"
来源：http://nop.nanxuanxn.top

[T10] Kotlin：默认参数
来源：http://fhk.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ugx.52xcode.cn

[T11] Kotlin：协程
来源：http://pcx.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jjf.bbcook.cn

[T12] Kotlin：解构声明
来源：http://cas.xuetiantiany.cn

val (a, b) = Pair(1, 2)
来源：http://icc.bbcook.cn

[T13] Kotlin：只读 Map
来源：http://row.xylfe.cn

val m = mapOf("a" to 1)
来源：http://cjj.xuanzx.com

[T14] Kotlin：循环
来源：http://aqi.ydzc1.top

for (i in 1..10) println(i)
来源：http://qvj.cucudq.cn

[T15] Kotlin：接口
来源：http://qqv.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://nki.daxiang520.top

[T16] Swift：Hello World
来源：http://qan.xuetiantiany.cn

print("Hello")
来源：http://ovy.feifeiyinyue.top

[T17] Swift：变量与常量
来源：http://zpm.hammf.cn

var a = 1;  let b = 2
来源：http://tmq.shanyushiyangtech.top

[T18] Swift：字符串插值
来源：http://aje.pengpengdd.cyou

"值: \(b)"
来源：http://fau.fzhhl.top

[T19] Swift：可选绑定
来源：http://xhw.yuxming.cn

if let n = opt { print(n) }
来源：http://gsp.bbcook.cn

[T20] Swift：数组操作
来源：http://vft.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://rjh.0kj1m.cn

[T21] Swift：遍历
来源：http://uwq.cdnleiting.top

for x in a { print(x) }
来源：http://edh.hongshengwenyu.top

[T22] Swift：字典
来源：http://nbg.pengpengdd.cyou

var d = ["a": 1];  d["b"] = 2
来源：http://ont.yanxiufei.cn

[T23] Swift：函数
来源：http://mdt.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jgl.fehbvm.com

[T24] Swift：闭包
来源：http://dti.yonumen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://nkd.yueranfly.top

[T25] Swift：结构体
来源：http://lda.vqdsnc.cn

struct P { var x: Int }
来源：http://rjo.0kj1m.cn

[T26] Swift：类与重写
来源：http://cek.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://jwp.meibo888.top

[T27] Swift：错误处理
来源：http://edg.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://syn.ivvv.top

[T28] Swift：枚举
来源：http://zjq.aibaodan.cn

enum Color { case red, green }
来源：http://ado.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://voy.hammf.cn

guard let x = opt else { return }
来源：http://iue.yonumen.top

[T30] Swift：协议
来源：http://rla.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://snj.cucudq.cn

[T31] Lua：Hello World
来源：http://gef.yj202588.top

print("Hello")
来源：http://ysr.sysykeji.top

[T32] Lua：局部变量
来源：http://xji.zhixingplan.top

local a = 1
来源：http://gam.zhengqikj.top

[T33] Lua：表（数组）
来源：http://xww.hammf.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kxb.nanxinkj.top

[T34] Lua：遍历表
来源：http://tjy.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ssi.yj202588.top

[T35] Lua：字典表
来源：http://udg.cdnleiting.top

local d = { a = 1 };  d.b = 2
来源：http://nsn.yj202588.top

[T36] Lua：函数
来源：http://tqx.redwolf501.top

function add(a, b) return a + b end
来源：http://sme.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://wun.fanxiaobao.xyz

"a" .. "b"
来源：http://opd.kuanghao11.cn

[T38] Lua：条件
来源：http://uie.cdnleiting.top

if x > 0 then print("正") end
来源：http://gpf.xuanzx.com

[T39] Lua：模式匹配
来源：http://pgr.tian-w.cn

string.find(s, "%d+")
来源：http://bkl.ppjwa.cn

[T40] Lua：元表
来源：http://izk.bbcook.cn

setmetatable({}, { __index = base })
来源：http://mtz.uphjek.com

[T41] Perl：Hello World
来源：http://icw.jinqigfzy.top

print "Hello\n";
来源：http://yhy.tarul.cn

[T42] Perl：变量类型
来源：http://ihi.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mfn.zhengqikj.top

[T43] Perl：字符串插值
来源：http://hmd.vqdsnc.cn

"值: $a"
来源：http://edx.hnxiangtu.top

[T44] Perl：条件
来源：http://klz.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://any.sysykeji.top

[T45] Perl：数组遍历
来源：http://ehs.ivvv.top

for my $x (@arr) { print $x; }
来源：http://aya.yj202588.top

[T46] Perl：哈希操作
来源：http://pgs.jqgfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kqv.fehbvm.com

[T47] Perl：正则捕获
来源：http://dsr.epnwcf.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://elh.sweek.top

[T48] Perl：正则替换
来源：http://kcm.jlsjyb.cn

$s =~ s/old/new/g;
来源：http://sdv.chenzaomai.com

[T49] Perl：函数
来源：http://aoy.jlsjyb.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zfk.jqgfzy.top

[T50] Perl：逐行读文件
来源：http://huy.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://coz.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://qci.sweek.top

[T51] Scala：Hello World
来源：http://dmv.cucudq.cn

println("Hello")
来源：http://zmh.shanyushiyangtech.top

[T52] Scala：变量
来源：http://mml.wangdashe.top

val a = 1;  var b = 2
来源：http://kgt.zdqjudy.top

[T53] Scala：字符串插值
来源：http://bni.bbcook.cn

s"值: $b"
来源：http://mfw.zhongyouzk.top

[T54] Scala：集合映射
来源：http://vqs.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://yqs.zdbjq.cn

[T55] Scala：集合过滤
来源：http://kzu.shuidangran.top

List(1, 2, 3).filter(_ > 1)
来源：http://rdh.yuanzhike.top

[T56] Scala：样例类
来源：http://lho.mhx1999.top

case class User(name: String, age: Int)
来源：http://rrm.shuidangran.top

[T57] Scala：模式匹配
来源：http://paj.hnqzz.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nzm.nwbrower.top

[T58] Scala：函数定义
来源：http://wln.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://ese.hongshengwenyu.top

[T59] Scala：循环
来源：http://esp.sweek.top

for (i <- 1 to 10) println(i)
来源：http://ypc.shanyushiyangkeji.top

[T60] Scala：折叠
来源：http://inn.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vmi.yonumen.top

================================================================================
来源：http://yyr.cqqwz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mrb.zhiwuduotai.top

================================================================================
来源：http://gln.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://vlc.yuanzhike.top

python -m venv .venv && source .venv/bin/activate
来源：http://jgt.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://rpk.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oxe.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://xhf.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://box.zycfv.cn

[U04] Py：变量调试打印
来源：http://ozw.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cbo.tanke756.top

[U05] Py：列表去重且保序
来源：http://ylx.sufxvd.cn

list(dict.fromkeys(arr))
来源：http://isy.hesvh.cn

[U06] Py：合并两个字典
来源：http://agh.hongshengwenyu.top

{**a, **b}
来源：http://ezp.hnqzz.top

[U07] Py：反转字典键值
来源：http://iho.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://rre.yj20258888.top

[U08] Py：展平二维列表
来源：http://jxi.guannengcc.top

[y for x in nested for y in x]
来源：http://lyk.birdmap.top

[U09] Py：字典取最大值的键
来源：http://wws.yuxming.cn

max(d, key=d.get)
来源：http://stc.haohaochexian.top

[U10] Py：按值排序字典
来源：http://qrl.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pbq.haohaochexian.top

[U11] Py：生成器表达式
来源：http://hni.jianghu66.top

(x * 2 for x in arr)
来源：http://faz.aibaodan.cn

[U12] Py：取出现最多的 3 个元素
来源：http://elf.ivvv.top

Counter(arr).most_common(3)
来源：http://fly.gotoacloud.top

[U13] Py：固定长度队列
来源：http://ajn.daxiang520.top

deque(maxlen=10)
来源：http://jtl.jinqigfzy.top

[U14] Py：分组收集到列表
来源：http://hds.shanyushiyangkeji.top

defaultdict(list)
来源：http://ive.redwolf501.top

[U15] Py：高精度计时
来源：http://llo.quarkkingdee.top

t = time.perf_counter()
来源：http://tiu.bbcook.cn

[U16] Py：命令行参数解析
来源：http://wlc.ctjpmb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yve.guowangkeji.top

[U17] Py：初始化日志
来源：http://lrq.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://ckd.zdbjq.cn

[U18] Py：预编译正则
来源：http://pnn.mhx1999.top

pat = re.compile(r"\d+")
来源：http://pau.cucudq.cn

[U19] Py：正则替换带回调
来源：http://qsn.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vbm.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://jxh.ivvv.top

@functools.lru_cache(maxsize=None)
来源：http://kda.shangyingyoupin.top

[U21] Py：自定义上下文管理器
来源：http://znd.uphjek.com

@contextlib.contextmanager
来源：http://fce.hongshengwenyu.top

[U22] Py：矩阵转置
来源：http://fck.yj202588.top

list(zip(*m))
来源：http://ttm.yvedp.cn

[U23] Py：分块读取大文件
来源：http://xlh.nanxinkj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jlw.hnqzz.top

[U24] Py：路径操作
来源：http://tzl.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nwi.ybcxt.top

[U25] Py：CSV 按字典读
来源：http://dfm.zhengqikj.top

csv.DictReader(f)
来源：http://prk.shuidangran.top

[U26] Py：并发下载
来源：http://sld.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lom.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://ieb.nwbrower.top

aiohttp.ClientSession() 配合 async with
来源：http://lpn.cqqwz.cn

[U28] Py：类型别名
来源：http://yna.meibo888.top

UserId = int
来源：http://ubi.9152youxi.cn

[U29] Py：属性校验
来源：http://toe.tian-w.cn

@property 与 @x.setter 配合
来源：http://ftm.hnqzz.top

[U30] Py：数据类
来源：http://dil.jinghuilouyu.cn

@dataclass(slots=True)
来源：http://oxn.nanxuanxn.top

[U31] Py：单测
来源：http://lix.cqqwz.cn

python -m pytest -q
来源：http://oyw.chenzaomai.com

[U32] Py：代码格式化
来源：http://pel.yvedp.cn

ruff format . && ruff check --fix .
来源：http://uir.meibo888.top


<!-- 参考信息 -->