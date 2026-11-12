代发 wailian999

int x; scanf("%d", &x);
来源：http://xxv.cdnleiting.top

[S04] C：字符串复制
来源：http://znv.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://vfh.dianchejie.cn

[S05] C：字符串长度
来源：http://gcy.jqgufenzy.top

strlen(s)
来源：http://ppy.jyoumei.cn

[S06] C：字符串比较
来源：http://knt.dianchejie.cn

strcmp(a, b) == 0
来源：http://ksq.316326.xyz

[S07] C：数组遍历求和
来源：http://yxj.ydzc1.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jhy.shanyushiyangtech.top

[S08] C：动态内存分配与释放
来源：http://wpg.hongshengwenyu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lju.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://sfw.nwbrower.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sup.hnqzz.top

[S10] C：指针与解引用
来源：http://hbo.fzhhl.top

int *p = &a;  *p = 5;
来源：http://jrt.cashguo.top

[S11] C：逐行读文件
来源：http://xkf.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://nyz.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ghl.chenzaomai.com

fclose(f);
来源：http://pca.bbcook.cn

[S12] C：写文件
来源：http://zcu.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://syi.haohaochexian.top

[S13] C：宏定义
来源：http://lna.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qfo.yonumen.top

[S14] C：枚举
来源：http://obh.hnqzz.top

enum Color { RED, GREEN, BLUE };
来源：http://ptt.yueranfly.top

[S15] C：类型转换
来源：http://hbm.shanyushiyangtech.top

(double) a / b
来源：http://gvk.gzhubu.top

[S16] C：位操作置位
来源：http://mov.ydjk.org.cn

x |= (1 << 3);
来源：http://jcp.ybcxt.top

[S17] C：安全拼接字符串
来源：http://zti.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ogk.gaohongyu789.top

[S18] C：命令行参数
来源：http://ayq.daria6918.cn

int main(int argc, char **argv)
来源：http://zan.dianchejie.cn

[S19] C：快速排序
来源：http://ixm.shuidangran.top

qsort(a, n, sizeof(int), cmp);
来源：http://pkw.zdqjudy.top

[S20] C：二分查找
来源：http://kqd.jianghu66.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://shc.kuanghao11.cn

[S21] C：字符类别判断
来源：http://prd.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mad.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://jks.jlsjyb.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lpw.haohaochexian.top

[S23] C：随机数
来源：http://pyg.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ica.aizwys.cn

[S24] C：获取本地时间
来源：http://chg.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://exl.redwolf501.top

[S25] C：内存拷贝
来源：http://tcw.dianchejie.cn

memcpy(dst, src, n);
来源：http://rlh.bjfxy.top

[S26] C：内存清零
来源：http://tap.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://dld.yuxming.cn

[S27] C：定义常量
来源：http://kbg.hcnkem.com

const double PI = 3.14159;
来源：http://urf.yueranfly.top

[S28] C：静态变量
来源：http://egb.uphjek.com

static int counter = 0;
来源：http://udk.hysaishi.cn

[S29] C：变参函数
来源：http://cil.jqgfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cpi.cucudq.cn

[S30] C：头文件保护
来源：http://nvm.ybcxt.top

#ifndef X_H
来源：http://hbd.jiagoushi.top

#define X_H
来源：http://bgd.ybcxt.top

#endif
来源：http://ydw.zhiwuduotai.top

[S31] C++：Hello World
来源：http://dta.zdqjudy.top

#include <iostream>
来源：http://wha.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://uuz.yj20258888.top

[S32] C++：字符串
来源：http://bwr.aizwys.cn

std::string s = "hi";  s += "!";
来源：http://tlp.cqqwz.cn

[S33] C++：vector 增删
来源：http://gjm.vehdjk.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xof.aizwys.cn

[S34] C++：遍历 vector
来源：http://wfc.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://gzf.xingfuxueyuan.xyz

[S35] C++：map
来源：http://kqm.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ucg.jqgufenzy.top

[S36] C++：unordered_map
来源：http://xvm.shuidangran.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://csu.aizwys.cn

[S37] C++：set
来源：http://bmt.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cew.zhiwuduotai.top

[S38] C++：排序
来源：http://ipm.shuidangran.top

std::sort(v.begin(), v.end());
来源：http://tmb.cdnleiting.top

[S39] C++：自定义比较器排序
来源：http://wug.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mlk.uphjek.com

[S40] C++：查找元素
来源：http://ixu.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ngf.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://beh.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ind.0kj1m.cn

[S42] C++：继承与虚函数
来源：http://izl.fanxiaobao.xyz

class B : public Base { public: void f() override {} };
来源：http://mwi.guowangkeji.top

[S43] C++：智能指针
来源：http://uwl.bjfxy.top

auto p = std::make_unique<int>(5);
来源：http://yol.sxryk.cn

[S44] C++：引用传参
来源：http://eax.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://oqv.chenlongwang.top

[S45] C++：lambda
来源：http://met.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://sec.jqgfzy.top

[S46] C++：函数模板
来源：http://pmk.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sfu.yangfankeji.com

[S47] C++：结构化绑定遍历
来源：http://jju.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cwi.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://alt.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xij.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://zao.c1oappe.top

[S49] C++：写文件
来源：http://bpt.yangfankeji.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nri.hammf.cn

[S50] C++：格式化数字
来源：http://orh.hnxiangtu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hsg.bbcook.cn

[S51] C++：显式类型转换
来源：http://aaa.c1oappe.top

static_cast<double>(a) / b
来源：http://ayy.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://mai.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://erz.nwbrower.top

[S53] C++：移动语义
来源：http://uwr.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://joi.yj20258888.top

[S54] C++：异常处理
来源：http://kgi.birdmap.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uln.shzxlz.cn

[S55] C++：结构化绑定
来源：http://hpw.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pqc.aibaodan.cn

[S56] C++：optional
来源：http://pko.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kml.pycfn.com

[S57] C++：编译期常量
来源：http://okx.hongshengwenyu.top

constexpr int N = 10;
来源：http://yxp.epnwcf.com

[S58] C++：命名空间
来源：http://dai.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://xgt.gotoacloud.top

[S59] C++：静态断言
来源：http://nzr.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bjg.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://lnt.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ndx.zhongyouzk.top

================================================================================
来源：http://ufd.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hgp.yj20258.top

================================================================================
来源：http://fyb.uphjek.com

[T01] Kotlin：Hello World
来源：http://xrs.birdmap.top

println("Hello")
来源：http://ixc.yj202588.top

[T02] Kotlin：变量
来源：http://uqr.yanxiufei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pty.gogol.net.cn

[T03] Kotlin：字符串模板
来源：http://vrm.smart0.xyz

"值: $b"
来源：http://dpj.cashguo.top

[T04] Kotlin：空安全
来源：http://zpk.svipenyu.cn

val n: String? = null;  n?.length
来源：http://zdt.wangshuangyany.cn

[T05] Kotlin：when 表达式
来源：http://nhg.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sfk.xylfe.cn

[T06] Kotlin：集合映射
来源：http://hrn.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wha.redwolf501.top

[T07] Kotlin：集合过滤
来源：http://wol.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sgr.aizwys.cn

[T08] Kotlin：数据类
来源：http://rfi.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://zeu.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://cpt.zhoulong.xyz

fun String.exclaim() = this + "!"
来源：http://bjx.ydzc1.top

[T10] Kotlin：默认参数
来源：http://jjv.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vza.fengsongda.top

[T11] Kotlin：协程
来源：http://efe.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ddm.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://sui.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://jle.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://wvm.gotoacloud.top

val m = mapOf("a" to 1)
来源：http://jzr.zhijiandao.cn

[T14] Kotlin：循环
来源：http://ibd.chenzaomai.com

for (i in 1..10) println(i)
来源：http://shm.hnxiangtu.top

[T15] Kotlin：接口
来源：http://nqm.yj20258.top

interface Shape { fun area(): Double }
来源：http://ctn.sysykeji.top

[T16] Swift：Hello World
来源：http://mpi.tianlin.xyz

print("Hello")
来源：http://ylt.shangyingyoupin.top

[T17] Swift：变量与常量
来源：http://fhg.yj20258888.top

var a = 1;  let b = 2
来源：http://lio.pycfn.com

[T18] Swift：字符串插值
来源：http://ouu.xziqi.cn

"值: \(b)"
来源：http://lym.jlsjyb.cn

[T19] Swift：可选绑定
来源：http://rno.hysaishi.cn

if let n = opt { print(n) }
来源：http://mfs.chenlongwang.top

[T20] Swift：数组操作
来源：http://wvx.c1oappe.top

var a = [1, 2, 3];  a.append(4)
来源：http://ofs.xylfe.cn

[T21] Swift：遍历
来源：http://sdv.chenjidiqi.icu

for x in a { print(x) }
来源：http://gpz.zdqjudy.top

[T22] Swift：字典
来源：http://dfr.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sjy.yonumen.top

[T23] Swift：函数
来源：http://lnk.xingfuxueyuan.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://reb.ydzc1.top

[T24] Swift：闭包
来源：http://xgu.ywan-chungtsiang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://epw.hcnkem.com

[T25] Swift：结构体
来源：http://ebz.tianlin.xyz

struct P { var x: Int }
来源：http://lqz.andypj.xyz

[T26] Swift：类与重写
来源：http://xes.daria6918.cn

class A: Base { override func f() {} }
来源：http://twi.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://hul.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://eps.jinqigufen.top

[T28] Swift：枚举
来源：http://ruf.52xcode.cn

enum Color { case red, green }
来源：http://gvr.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://yzb.pycfn.com

guard let x = opt else { return }
来源：http://upg.chenlongwang.top

[T30] Swift：协议
来源：http://msh.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://vvt.xuanzx.com

[T31] Lua：Hello World
来源：http://vui.yangfankeji.com

print("Hello")
来源：http://wku.cheryme.top

[T32] Lua：局部变量
来源：http://oyy.redwolf501.top

local a = 1
来源：http://zca.fanxiaobao.xyz

[T33] Lua：表（数组）
来源：http://vli.bjfxy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mje.snrcjt.cn

[T34] Lua：遍历表
来源：http://qgr.zhiwuduotai.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jqo.tanke756.top

[T35] Lua：字典表
来源：http://tya.hnxiangtu.top

local d = { a = 1 };  d.b = 2
来源：http://bnk.hesvh.cn

[T36] Lua：函数
来源：http://fnu.chenlongwang.top

function add(a, b) return a + b end
来源：http://lmu.gzhubu.top

[T37] Lua：字符串拼接
来源：http://vgw.snrcjt.cn

"a" .. "b"
来源：http://ton.yuanzhike.top

[T38] Lua：条件
来源：http://kvz.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://dak.yj20258.top

[T39] Lua：模式匹配
来源：http://cqo.chenzaomai.com

string.find(s, "%d+")
来源：http://tfd.cqqwz.cn

[T40] Lua：元表
来源：http://msm.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://yab.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://fyh.tian-w.cn

print "Hello\n";
来源：http://hrw.zhijiandao.cn

[T42] Perl：变量类型
来源：http://hrj.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ygu.birdmap.top

[T43] Perl：字符串插值
来源：http://fmn.yongpay.top

"值: $a"
来源：http://dfs.bjfxy.top

[T44] Perl：条件
来源：http://jbp.yj202588.top

if ($a > 0) { print "正"; }
来源：http://xdf.guowangkeji.top

[T45] Perl：数组遍历
来源：http://zsh.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://vmo.svipenyu.cn

[T46] Perl：哈希操作
来源：http://hmd.jianghu66.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://itu.ctjpmb.com

[T47] Perl：正则捕获
来源：http://ziw.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tcc.sxryk.cn

[T48] Perl：正则替换
来源：http://fjc.daria6918.cn

$s =~ s/old/new/g;
来源：http://zfi.9152youxi.cn

[T49] Perl：函数
来源：http://gyv.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://grm.xinyue.icu

[T50] Perl：逐行读文件
来源：http://gga.yvedp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wwf.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://sjc.9152youxi.cn

[T51] Scala：Hello World
来源：http://tea.cashguo.top

println("Hello")
来源：http://uet.52xcode.cn

[T52] Scala：变量
来源：http://uxd.xuanzx.com

val a = 1;  var b = 2
来源：http://bcs.zhongyouzk.top

[T53] Scala：字符串插值
来源：http://oyc.hongshengwenyu.top

s"值: $b"
来源：http://ipq.guowangkeji.top

[T54] Scala：集合映射
来源：http://yok.vehdjk.com

List(1, 2, 3).map(_ * 2)
来源：http://rad.xuanzx.com

[T55] Scala：集合过滤
来源：http://frt.fanxiaobao.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://kem.cucudq.cn

[T56] Scala：样例类
来源：http://mvq.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://rhz.pengpengdd.cyou

[T57] Scala：模式匹配
来源：http://mjm.c1oappe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dfm.guannengcc.top

[T58] Scala：函数定义
来源：http://yvl.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://htt.ywan-chungtsiang.top

[T59] Scala：循环
来源：http://piq.iojbl.cn

for (i <- 1 to 10) println(i)
来源：http://izk.havefunace.top

[T60] Scala：折叠
来源：http://tqt.xuanzx.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hma.shzxlz.cn

================================================================================
来源：http://zoi.sweek.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gkk.pycfn.com

================================================================================
来源：http://ohz.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://sdt.zdbjq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://giz.pengpengdd.cyou

[U02] Py：导出 / 安装依赖
来源：http://ivj.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wbw.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://fnb.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vzl.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://tfu.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wvg.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://lar.smart0.xyz

list(dict.fromkeys(arr))
来源：http://too.tian-w.cn

[U06] Py：合并两个字典
来源：http://tox.jqgfzy.top

{**a, **b}
来源：http://bxv.hcnkem.com

[U07] Py：反转字典键值
来源：http://wmh.kuanghao11.cn

{v: k for k, v in d.items()}
来源：http://ygc.ctjpmb.com

[U08] Py：展平二维列表
来源：http://owl.xylfe.cn

[y for x in nested for y in x]
来源：http://rev.chenzaomai.com

[U09] Py：字典取最大值的键
来源：http://wst.dianchejie.cn

max(d, key=d.get)
来源：http://jot.xuanzx.com

[U10] Py：按值排序字典
来源：http://anv.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hcq.vehdjk.com

[U11] Py：生成器表达式
来源：http://qjv.zdqjudy.top

(x * 2 for x in arr)
来源：http://ncq.smart0.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://bke.mhx1999.top

Counter(arr).most_common(3)
来源：http://pec.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://uzb.yonumen.top

deque(maxlen=10)
来源：http://ool.hammf.cn

[U14] Py：分组收集到列表
来源：http://xad.snrcjt.cn

defaultdict(list)
来源：http://qjo.jlsjyb.cn

[U15] Py：高精度计时
来源：http://lhe.xuetiantiany.cn

t = time.perf_counter()
来源：http://zpu.shzxlz.cn

[U16] Py：命令行参数解析
来源：http://zne.chenlongwang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bdo.kuanghao11.cn

[U17] Py：初始化日志
来源：http://kef.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://mae.ybcxt.top

[U18] Py：预编译正则
来源：http://exq.zdqjudy.top

pat = re.compile(r"\d+")
来源：http://ozu.ydjk.org.cn

[U19] Py：正则替换带回调
来源：http://wwi.ehwqpu.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xmr.tian-w.cn

[U20] Py：缓存函数结果
来源：http://yws.gogol.net.cn

@functools.lru_cache(maxsize=None)
来源：http://khq.nanxuanxn.top

[U21] Py：自定义上下文管理器
来源：http://cue.dianchejie.cn

@contextlib.contextmanager
来源：http://rxa.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://syf.sweek.top

list(zip(*m))
来源：http://hys.uphjek.com

[U23] Py：分块读取大文件
来源：http://nbf.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mfp.hammf.cn

[U24] Py：路径操作
来源：http://rdf.zdbjq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://utp.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://bpc.zhoulong.xyz

csv.DictReader(f)
来源：http://njy.epnwcf.com

[U26] Py：并发下载
来源：http://baw.chenlongwang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hcc.jlsjyb.cn


<!-- 参考信息 -->