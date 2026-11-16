代发 wailian999

strlen(s)
来源：http://rjc.tian-w.cn

[S06] C：字符串比较
来源：http://drn.yanxiufei.cn

strcmp(a, b) == 0
来源：http://uxs.fengsongda.top

[S07] C：数组遍历求和
来源：http://snv.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pvi.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://rda.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://szn.zycfv.cn

[S09] C：结构体定义与初始化
来源：http://zpd.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dal.chenzaomai.com

[S10] C：指针与解引用
来源：http://yax.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://jvd.epnwcf.com

[S11] C：逐行读文件
来源：http://yec.redwolf501.top

FILE *f = fopen("a.txt", "r");
来源：http://abq.sjlbkw.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://joe.zhixingplan.top

fclose(f);
来源：http://qsf.gzhubu.top

[S12] C：写文件
来源：http://xmo.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://snm.jqgufenzy.top

[S13] C：宏定义
来源：http://cbe.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ldy.gaohongyu789.top

[S14] C：枚举
来源：http://znc.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://lxf.nwbrower.top

[S15] C：类型转换
来源：http://zjn.chenjidiqi.icu

(double) a / b
来源：http://wzn.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://zac.yj20258.top

x |= (1 << 3);
来源：http://tcl.epnwcf.com

[S17] C：安全拼接字符串
来源：http://ozq.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zxg.c1oappe.top

[S18] C：命令行参数
来源：http://dng.xingfuxueyuan.xyz

int main(int argc, char **argv)
来源：http://spd.hammf.cn

[S19] C：快速排序
来源：http://sch.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://suh.xziqi.cn

[S20] C：二分查找
来源：http://qug.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vba.nwbrower.top

[S21] C：字符类别判断
来源：http://jwd.fehbvm.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cyd.yongpay.top

[S22] C：字符串转数字
来源：http://gbp.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sbg.cashguo.top

[S23] C：随机数
来源：http://rff.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jur.jqgfzy.top

[S24] C：获取本地时间
来源：http://yjm.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qnv.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://fwh.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://bza.0kj1m.cn

[S26] C：内存清零
来源：http://meb.cashguo.top

memset(a, 0, sizeof a);
来源：http://jxt.birdmap.top

[S27] C：定义常量
来源：http://jon.yongpay.top

const double PI = 3.14159;
来源：http://haz.zhengqikj.top

[S28] C：静态变量
来源：http://eeu.hysaishi.cn

static int counter = 0;
来源：http://nje.ybcxt.top

[S29] C：变参函数
来源：http://zyh.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zvx.zhoulong.xyz

[S30] C：头文件保护
来源：http://nbk.sxryk.cn

#ifndef X_H
来源：http://qik.jinqigufen.top

#define X_H
来源：http://dql.sufxvd.cn

#endif
来源：http://fbr.chenzaomai.com

[S31] C++：Hello World
来源：http://mfx.hysaishi.cn

#include <iostream>
来源：http://spe.meibo888.top

int main() { std::cout << "Hello\n"; }
来源：http://afd.xylfe.cn

[S32] C++：字符串
来源：http://qqe.fktsv.cn

std::string s = "hi";  s += "!";
来源：http://gfo.jinqigfzy.top

[S33] C++：vector 增删
来源：http://fav.daxiang520.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://liw.bjfxy.top

[S34] C++：遍历 vector
来源：http://arr.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://kzv.yj20258.top

[S35] C++：map
来源：http://zcr.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fyb.uphjek.com

[S36] C++：unordered_map
来源：http://phi.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yyy.yanxiufei.cn

[S37] C++：set
来源：http://zdh.zhixingplan.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vfi.xinyue.icu

[S38] C++：排序
来源：http://gzm.hcnkem.com

std::sort(v.begin(), v.end());
来源：http://ufg.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://ixo.yueranfly.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cfq.xziqi.cn

[S40] C++：查找元素
来源：http://pan.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xfd.sufxvd.cn

[S41] C++：类与构造函数
来源：http://fus.daxiang520.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dcv.vqdsnc.cn

[S42] C++：继承与虚函数
来源：http://twu.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://tjm.daxiang520.top

[S43] C++：智能指针
来源：http://okc.jiagoushi.top

auto p = std::make_unique<int>(5);
来源：http://ohg.nanxinkj.top

[S44] C++：引用传参
来源：http://gah.sufxvd.cn

void inc(int &x) { ++x; }
来源：http://biy.chenzaomai.com

[S45] C++：lambda
来源：http://tnt.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gcr.hysaishi.cn

[S46] C++：函数模板
来源：http://feb.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pzz.316326.xyz

[S47] C++：结构化绑定遍历
来源：http://zxf.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pcs.guowangkeji.top

[S48] C++：逐行读文件
来源：http://jji.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://vbc.c1oappe.top

while (std::getline(in, line)) { }
来源：http://emu.epnwcf.com

[S49] C++：写文件
来源：http://yyk.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pcc.sweek.top

[S50] C++：格式化数字
来源：http://vte.fehbvm.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wto.smart0.xyz

[S51] C++：显式类型转换
来源：http://gye.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://kme.xingfuxueyuan.xyz

[S52] C++：const 与 noexcept
来源：http://yok.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://pjv.nanxuanxn.top

[S53] C++：移动语义
来源：http://xwp.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://ohp.gotoacloud.top

[S54] C++：异常处理
来源：http://oyr.daxiang520.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gml.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://iwm.dashuyun.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zpe.hongshengwenyu.top

[S56] C++：optional
来源：http://cdc.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://spf.sweek.top

[S57] C++：编译期常量
来源：http://bph.316326.xyz

constexpr int N = 10;
来源：http://tzy.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://jkg.hywenlv.cn

namespace ns { int f() { return 1; } }
来源：http://opx.jiagoushi.top

[S59] C++：静态断言
来源：http://tvq.xinyue.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sci.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://bzg.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uge.sysykeji.top

================================================================================
来源：http://lnc.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zqg.shuidangran.top

================================================================================
来源：http://pjv.ivvv.top

[T01] Kotlin：Hello World
来源：http://pya.chenlongwang.top

println("Hello")
来源：http://vyf.nanxinkj.top

[T02] Kotlin：变量
来源：http://yri.gaohongyu789.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uwz.yanxiufei.cn

[T03] Kotlin：字符串模板
来源：http://rdd.hammf.cn

"值: $b"
来源：http://vqv.ivvv.top

[T04] Kotlin：空安全
来源：http://ahi.gogol.net.cn

val n: String? = null;  n?.length
来源：http://fzm.cheryme.top

[T05] Kotlin：when 表达式
来源：http://cky.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://asy.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://ect.hcnkem.com

listOf(1, 2, 3).map { it * 2 }
来源：http://sum.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://kbk.aizwys.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jba.gogol.net.cn

[T08] Kotlin：数据类
来源：http://afp.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://chr.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://quw.xylfe.cn

fun String.exclaim() = this + "!"
来源：http://xtj.yfazqb.com

[T10] Kotlin：默认参数
来源：http://ygz.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xju.jqgufenzy.top

[T11] Kotlin：协程
来源：http://kpq.yueranfly.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://srd.xylfe.cn

[T12] Kotlin：解构声明
来源：http://hpd.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://cth.ydzc1.top

[T13] Kotlin：只读 Map
来源：http://bwr.wangdashe.top

val m = mapOf("a" to 1)
来源：http://hrf.gotoacloud.top

[T14] Kotlin：循环
来源：http://wvn.hesvh.cn

for (i in 1..10) println(i)
来源：http://fpy.c1oappe.top

[T15] Kotlin：接口
来源：http://mlg.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://ame.yuanzhike.top

[T16] Swift：Hello World
来源：http://dsi.smart0.xyz

print("Hello")
来源：http://vmc.yj20258888.top

[T17] Swift：变量与常量
来源：http://wsn.daria6918.cn

var a = 1;  let b = 2
来源：http://zjg.guannengcc.top

[T18] Swift：字符串插值
来源：http://uwt.zhiwuduotai.top

"值: \(b)"
来源：http://vjo.hfpthk.cn

[T19] Swift：可选绑定
来源：http://ned.meibo888.top

if let n = opt { print(n) }
来源：http://tln.fehbvm.com

[T20] Swift：数组操作
来源：http://lja.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uiv.shanyushiyangkeji.top

[T21] Swift：遍历
来源：http://kyk.smart0.xyz

for x in a { print(x) }
来源：http://rwh.tianlin.xyz

[T22] Swift：字典
来源：http://mqp.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://jcz.hnqzz.top

[T23] Swift：函数
来源：http://zwe.pycfn.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vog.gaohongyu789.top

[T24] Swift：闭包
来源：http://uib.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ofy.nwbrower.top

[T25] Swift：结构体
来源：http://bzx.jianghu66.top

struct P { var x: Int }
来源：http://ucs.xuetiantiany.cn

[T26] Swift：类与重写
来源：http://lin.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://lpv.mhx1999.top

[T27] Swift：错误处理
来源：http://lzz.hcnkem.com

do { try f() } catch { print(error) }
来源：http://smw.hywenlv.cn

[T28] Swift：枚举
来源：http://sku.tianlin.xyz

enum Color { case red, green }
来源：http://ptj.yueranfly.top

[T29] Swift：guard 提前返回
来源：http://ffz.sweek.top

guard let x = opt else { return }
来源：http://alv.0kj1m.cn

[T30] Swift：协议
来源：http://kqh.0kj1m.cn

protocol Shape { func area() -> Double }
来源：http://cro.cashguo.top

[T31] Lua：Hello World
来源：http://nxz.yuxming.cn

print("Hello")
来源：http://ocw.aizwys.cn

[T32] Lua：局部变量
来源：http://dqh.cashguo.top

local a = 1
来源：http://mmm.kuanghao11.cn

[T33] Lua：表（数组）
来源：http://zql.tianlin.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://yao.ehwqpu.com

[T34] Lua：遍历表
来源：http://vqa.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://xqq.nwbrower.top

[T35] Lua：字典表
来源：http://nte.shuidangran.top

local d = { a = 1 };  d.b = 2
来源：http://iwj.xuetiantiany.cn

[T36] Lua：函数
来源：http://ltd.jqgufenzy.top

function add(a, b) return a + b end
来源：http://zdr.chenzaomai.com

[T37] Lua：字符串拼接
来源：http://rjy.yfazqb.com

"a" .. "b"
来源：http://kri.hnxiangtu.top

[T38] Lua：条件
来源：http://vyc.guowangkeji.top

if x > 0 then print("正") end
来源：http://efm.pycfn.com

[T39] Lua：模式匹配
来源：http://zmq.9152youxi.cn

string.find(s, "%d+")
来源：http://xys.gaohongyu789.top

[T40] Lua：元表
来源：http://tpy.vqdsnc.cn

setmetatable({}, { __index = base })
来源：http://jxe.chenzaomai.com

[T41] Perl：Hello World
来源：http://pbb.ydzc1.top

print "Hello\n";
来源：http://swa.mhx1999.top

[T42] Perl：变量类型
来源：http://wxg.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wkg.dianchejie.cn

[T43] Perl：字符串插值
来源：http://mwi.tian-w.cn

"值: $a"
来源：http://yjg.xuetiantiany.cn

[T44] Perl：条件
来源：http://dfo.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://ydn.xingfuxueyuan.xyz

[T45] Perl：数组遍历
来源：http://saz.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://jax.dashuyun.cn

[T46] Perl：哈希操作
来源：http://crn.kuanghao11.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yrv.andypj.xyz

[T47] Perl：正则捕获
来源：http://mqq.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://uva.sjlbkw.cn

[T48] Perl：正则替换
来源：http://zdy.jiagoushi.top

$s =~ s/old/new/g;
来源：http://utx.yj202588.top

[T49] Perl：函数
来源：http://zmq.zhijiandao.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ybb.fktsv.cn

[T50] Perl：逐行读文件
来源：http://acs.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ibp.gogol.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://ibx.0kj1m.cn

[T51] Scala：Hello World
来源：http://imh.hcnkem.com

println("Hello")
来源：http://ecu.hysaishi.cn

[T52] Scala：变量
来源：http://nkg.guowangkeji.top

val a = 1;  var b = 2
来源：http://qth.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://whb.0kj1m.cn

s"值: $b"
来源：http://grw.yanxiufei.cn

[T54] Scala：集合映射
来源：http://gle.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://ayr.yfazqb.com

[T55] Scala：集合过滤
来源：http://akb.0kj1m.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tcq.svipenyu.cn

[T56] Scala：样例类
来源：http://hif.shanyushiyangtech.top

case class User(name: String, age: Int)
来源：http://tfw.hesvh.cn

[T57] Scala：模式匹配
来源：http://qlx.tianlin.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://cgw.hammf.cn

[T58] Scala：函数定义
来源：http://ozo.tianlin.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://mvw.bbcook.cn

[T59] Scala：循环
来源：http://yyr.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://msk.iojbl.cn

[T60] Scala：折叠
来源：http://dsv.zhoulong.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qzu.jinqigufen.top

================================================================================
来源：http://omb.mhx1999.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://smr.uphjek.com

================================================================================
来源：http://ypm.tarul.cn

[U01] Py：创建虚拟环境
来源：http://ypx.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ihm.dianchejie.cn

[U02] Py：导出 / 安装依赖
来源：http://dqr.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lmm.ivvv.top

[U03] Py：加载 .env 配置
来源：http://zjs.fanxiaobao.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://qml.svipenyu.cn

[U04] Py：变量调试打印
来源：http://tbc.jinqigufen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lxq.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://azs.yj202588.top

list(dict.fromkeys(arr))
来源：http://anm.fktsv.cn

[U06] Py：合并两个字典
来源：http://zrv.shuidangran.top

{**a, **b}
来源：http://naw.yueranfly.top

[U07] Py：反转字典键值
来源：http://sii.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://iei.xylfe.cn

[U08] Py：展平二维列表
来源：http://nad.zhixingplan.top

[y for x in nested for y in x]
来源：http://wgn.316326.xyz

[U09] Py：字典取最大值的键
来源：http://dag.aibaodan.cn

max(d, key=d.get)
来源：http://vzb.xziqi.cn

[U10] Py：按值排序字典
来源：http://mhz.hammf.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kzm.chenzaomai.com

[U11] Py：生成器表达式
来源：http://hfe.quarkkingdee.top

(x * 2 for x in arr)
来源：http://zko.zdbjq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ugj.cqqwz.cn

Counter(arr).most_common(3)
来源：http://oqa.yonumen.top

[U13] Py：固定长度队列
来源：http://xls.zycfv.cn

deque(maxlen=10)
来源：http://iir.daxiang520.top

[U14] Py：分组收集到列表
来源：http://hmh.dianchejie.cn

defaultdict(list)
来源：http://jkn.hysaishi.cn

[U15] Py：高精度计时
来源：http://qtl.gaohongyu789.top

t = time.perf_counter()
来源：http://ijc.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://kih.chenlongwang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mfg.sufxvd.cn

[U17] Py：初始化日志
来源：http://giw.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://cwq.bbcook.cn

[U18] Py：预编译正则
来源：http://zts.jinqigufen.top

pat = re.compile(r"\d+")
来源：http://xrs.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://zcy.zdqjudy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lpv.jinqigufen.top

[U20] Py：缓存函数结果
来源：http://pfk.hysaishi.cn

@functools.lru_cache(maxsize=None)
来源：http://tpo.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://ivu.pycfn.com

@contextlib.contextmanager
来源：http://nqr.gzhubu.top

[U22] Py：矩阵转置
来源：http://slm.sufxvd.cn

list(zip(*m))
来源：http://fov.wangdashe.top

[U23] Py：分块读取大文件
来源：http://xui.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zyg.daria6918.cn

[U24] Py：路径操作
来源：http://mrs.yangfankeji.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lij.meibo888.top

[U25] Py：CSV 按字典读
来源：http://xpy.shuidangran.top

csv.DictReader(f)
来源：http://adm.fengsongda.top

[U26] Py：并发下载
来源：http://iux.yongpay.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://loq.hnqzz.top

[U27] Py：异步 HTTP
来源：http://xbz.ywan-chungtsiang.top

aiohttp.ClientSession() 配合 async with
来源：http://lmg.hysaishi.cn

[U28] Py：类型别名
来源：http://pao.cashguo.top

UserId = int
来源：http://sbp.yangfankeji.com


<!-- 参考信息 -->