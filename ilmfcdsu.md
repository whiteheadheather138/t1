代发 wailian999

strlen(s)
来源：http://saf.jinghuilouyu.cn

[S06] C：字符串比较
来源：http://mnv.sufxvd.cn

strcmp(a, b) == 0
来源：http://oqe.wangshuangyany.cn

[S07] C：数组遍历求和
来源：http://bwu.yuanzhike.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://chc.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://jsp.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qku.yj20258.top

[S09] C：结构体定义与初始化
来源：http://yob.guannengcc.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://alz.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://djw.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://krh.iojbl.cn

[S11] C：逐行读文件
来源：http://gtw.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://wxm.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vbf.uphjek.com

fclose(f);
来源：http://msa.jianghu66.top

[S12] C：写文件
来源：http://nbo.haohaochexian.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oxe.fzhhl.top

[S13] C：宏定义
来源：http://bpg.yj20258888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://una.cucudq.cn

[S14] C：枚举
来源：http://kdz.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://fxd.fktsv.cn

[S15] C：类型转换
来源：http://kml.feifeiyinyue.top

(double) a / b
来源：http://rws.jlsjyb.cn

[S16] C：位操作置位
来源：http://sdb.bbcook.cn

x |= (1 << 3);
来源：http://fex.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://qbl.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pyo.xinyue.icu

[S18] C：命令行参数
来源：http://tpp.chenzaomai.com

int main(int argc, char **argv)
来源：http://gda.ydjk.org.cn

[S19] C：快速排序
来源：http://ipk.feifeiyinyue.top

qsort(a, n, sizeof(int), cmp);
来源：http://geb.cheryme.top

[S20] C：二分查找
来源：http://jss.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nbn.jqgufenzy.top

[S21] C：字符类别判断
来源：http://okc.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jpl.aizwys.cn

[S22] C：字符串转数字
来源：http://mve.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://wrn.pengpengdd.cyou

[S23] C：随机数
来源：http://gjj.jinghuilouyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ubn.bbcook.cn

[S24] C：获取本地时间
来源：http://sbe.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ksg.xuanzx.com

[S25] C：内存拷贝
来源：http://hlu.zhengqikj.top

memcpy(dst, src, n);
来源：http://dvj.xinyue.icu

[S26] C：内存清零
来源：http://ztf.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://xlk.bbcook.cn

[S27] C：定义常量
来源：http://hbc.epnwcf.com

const double PI = 3.14159;
来源：http://fac.zhongyouzk.top

[S28] C：静态变量
来源：http://cxk.mhx1999.top

static int counter = 0;
来源：http://wnq.jqgufenzy.top

[S29] C：变参函数
来源：http://qmz.guannengcc.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://swc.fktsv.cn

[S30] C：头文件保护
来源：http://qss.yj20258888.top

#ifndef X_H
来源：http://kxy.hongshengwenyu.top

#define X_H
来源：http://jrf.havefunace.top

#endif
来源：http://jdz.svipenyu.cn

[S31] C++：Hello World
来源：http://uwx.yonumen.top

#include <iostream>
来源：http://lns.ydjk.org.cn

int main() { std::cout << "Hello\n"; }
来源：http://mzu.yongpay.top

[S32] C++：字符串
来源：http://nzy.fktsv.cn

std::string s = "hi";  s += "!";
来源：http://noq.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://euj.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mdb.cqqwz.cn

[S34] C++：遍历 vector
来源：http://tma.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://nes.aizwys.cn

[S35] C++：map
来源：http://mdn.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jhs.cashguo.top

[S36] C++：unordered_map
来源：http://vlg.snrcjt.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vba.fktsv.cn

[S37] C++：set
来源：http://adw.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yfm.dashuyun.cn

[S38] C++：排序
来源：http://ugr.xuanzx.com

std::sort(v.begin(), v.end());
来源：http://hkl.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://hjk.kuanghao11.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zci.ydzc1.top

[S40] C++：查找元素
来源：http://hgh.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cwb.bbcook.cn

[S41] C++：类与构造函数
来源：http://rzf.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hyd.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://pnb.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://fca.smart0.xyz

[S43] C++：智能指针
来源：http://bih.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://uas.snrcjt.cn

[S44] C++：引用传参
来源：http://xrr.jqgfzy.top

void inc(int &x) { ++x; }
来源：http://jvi.dianchejie.cn

[S45] C++：lambda
来源：http://hzx.daxiang520.top

auto add = [](int a, int b) { return a + b; };
来源：http://rgi.jlsjyb.cn

[S46] C++：函数模板
来源：http://oai.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xqg.hongshengwenyu.top

[S47] C++：结构化绑定遍历
来源：http://wap.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xom.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://heo.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gee.shanyushiyangtech.top

while (std::getline(in, line)) { }
来源：http://bfj.meibo888.top

[S49] C++：写文件
来源：http://odt.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vni.cashguo.top

[S50] C++：格式化数字
来源：http://eqa.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zwd.yangfankeji.com

[S51] C++：显式类型转换
来源：http://gbl.shuidangran.top

static_cast<double>(a) / b
来源：http://rqy.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://ety.dashuyun.cn

int size() const noexcept { return n_; }
来源：http://ogf.epnwcf.com

[S53] C++：移动语义
来源：http://gxe.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://cou.0kj1m.cn

[S54] C++：异常处理
来源：http://vjn.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sjc.shzxlz.cn

[S55] C++：结构化绑定
来源：http://wfy.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vnw.xingfuxueyuan.xyz

[S56] C++：optional
来源：http://eai.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uuc.zhixingplan.top

[S57] C++：编译期常量
来源：http://vci.hysaishi.cn

constexpr int N = 10;
来源：http://dax.hnxiangtu.top

[S58] C++：命名空间
来源：http://kez.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://elf.nwbrower.top

[S59] C++：静态断言
来源：http://ant.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kyu.birdmap.top

[S60] C++：遍历并删除元素
来源：http://gpk.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tsg.zdqjudy.top

================================================================================
来源：http://ocv.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://icp.mhx1999.top

================================================================================
来源：http://axr.0kj1m.cn

[T01] Kotlin：Hello World
来源：http://enx.fktsv.cn

println("Hello")
来源：http://rys.guowangkeji.top

[T02] Kotlin：变量
来源：http://bot.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xlt.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://mpj.shanyushiyangkeji.top

"值: $b"
来源：http://afi.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://ftv.mhx1999.top

val n: String? = null;  n?.length
来源：http://itf.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://mnt.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ysz.hysaishi.cn

[T06] Kotlin：集合映射
来源：http://lkm.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://psi.haohaochexian.top

[T07] Kotlin：集合过滤
来源：http://iqq.xuetiantiany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dfj.hywenlv.cn

[T08] Kotlin：数据类
来源：http://ftc.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://ljw.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://jte.sweek.top

fun String.exclaim() = this + "!"
来源：http://tbx.ydzc1.top

[T10] Kotlin：默认参数
来源：http://jmk.gotoacloud.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yxy.fktsv.cn

[T11] Kotlin：协程
来源：http://pag.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://qyh.yj20258888.top

[T12] Kotlin：解构声明
来源：http://fgi.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://aou.fzhhl.top

[T13] Kotlin：只读 Map
来源：http://zku.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://xqs.xylfe.cn

[T14] Kotlin：循环
来源：http://xlf.ydzc1.top

for (i in 1..10) println(i)
来源：http://nqg.nanxinkj.top

[T15] Kotlin：接口
来源：http://xeu.zdqjudy.top

interface Shape { fun area(): Double }
来源：http://dba.yuanzhike.top

[T16] Swift：Hello World
来源：http://rqq.zhengqikj.top

print("Hello")
来源：http://ner.hammf.cn

[T17] Swift：变量与常量
来源：http://klw.yj20258888.top

var a = 1;  let b = 2
来源：http://xux.epnwcf.com

[T18] Swift：字符串插值
来源：http://uoy.hnxiangtu.top

"值: \(b)"
来源：http://kxd.zhoulong.xyz

[T19] Swift：可选绑定
来源：http://ixy.hongshengwenyu.top

if let n = opt { print(n) }
来源：http://djy.xinyue.icu

[T20] Swift：数组操作
来源：http://qwt.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://qso.zhoulong.xyz

[T21] Swift：遍历
来源：http://hrr.sysykeji.top

for x in a { print(x) }
来源：http://jot.svipenyu.cn

[T22] Swift：字典
来源：http://aek.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://yzu.dashuyun.cn

[T23] Swift：函数
来源：http://xdy.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fwm.meibo888.top

[T24] Swift：闭包
来源：http://crp.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kfx.zhongyouzk.top

[T25] Swift：结构体
来源：http://kkm.wangshuangyany.cn

struct P { var x: Int }
来源：http://dhe.dianchejie.cn

[T26] Swift：类与重写
来源：http://ydi.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://ipo.fzhhl.top

[T27] Swift：错误处理
来源：http://cpv.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://uxc.ehwqpu.com

[T28] Swift：枚举
来源：http://dux.meibo888.top

enum Color { case red, green }
来源：http://fyw.xinyue.icu

[T29] Swift：guard 提前返回
来源：http://sel.chenjidiqi.icu

guard let x = opt else { return }
来源：http://fgr.jiagoushi.top

[T30] Swift：协议
来源：http://ogk.yj20258.top

protocol Shape { func area() -> Double }
来源：http://bly.jianghu66.top

[T31] Lua：Hello World
来源：http://poi.dianchejie.cn

print("Hello")
来源：http://yhg.xziqi.cn

[T32] Lua：局部变量
来源：http://cbu.yuxming.cn

local a = 1
来源：http://ajk.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://rvh.yj202588.top

local t = {1, 2, 3};  t[4] = 4
来源：http://otm.yj20258.top

[T34] Lua：遍历表
来源：http://bid.tian-w.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ouk.guowangkeji.top

[T35] Lua：字典表
来源：http://mgw.quarkkingdee.top

local d = { a = 1 };  d.b = 2
来源：http://but.ydzc1.top

[T36] Lua：函数
来源：http://vrn.daria6918.cn

function add(a, b) return a + b end
来源：http://juz.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://rue.svipenyu.cn

"a" .. "b"
来源：http://khr.snrcjt.cn

[T38] Lua：条件
来源：http://ewa.c1oappe.top

if x > 0 then print("正") end
来源：http://plr.gogol.net.cn

[T39] Lua：模式匹配
来源：http://dbe.cucudq.cn

string.find(s, "%d+")
来源：http://evp.nwbrower.top

[T40] Lua：元表
来源：http://xgy.yj20258888.top

setmetatable({}, { __index = base })
来源：http://cjf.jinqigfzy.top

[T41] Perl：Hello World
来源：http://qai.gaohongyu789.top

print "Hello\n";
来源：http://wfi.yueranfly.top

[T42] Perl：变量类型
来源：http://nfu.redwolf501.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://skd.gotoacloud.top

[T43] Perl：字符串插值
来源：http://ena.yfazqb.com

"值: $a"
来源：http://imf.fanxiaobao.xyz

[T44] Perl：条件
来源：http://ida.yongpay.top

if ($a > 0) { print "正"; }
来源：http://amy.c1oappe.top

[T45] Perl：数组遍历
来源：http://mku.zhengqikj.top

for my $x (@arr) { print $x; }
来源：http://vjg.cashguo.top

[T46] Perl：哈希操作
来源：http://fxk.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pxt.shangyingyoupin.top

[T47] Perl：正则捕获
来源：http://ytr.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dcm.kuanghao11.cn

[T48] Perl：正则替换
来源：http://yaj.vehdjk.com

$s =~ s/old/new/g;
来源：http://waf.shanyushiyangtech.top

[T49] Perl：函数
来源：http://wya.ywan-chungtsiang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wqj.daria6918.cn

[T50] Perl：逐行读文件
来源：http://osa.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://lbk.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://qpz.yonumen.top

[T51] Scala：Hello World
来源：http://uyo.vqdsnc.cn

println("Hello")
来源：http://wyn.yvedp.cn

[T52] Scala：变量
来源：http://tan.jinqigfzy.top

val a = 1;  var b = 2
来源：http://onn.hammf.cn

[T53] Scala：字符串插值
来源：http://sgz.zhijiandao.cn

s"值: $b"
来源：http://hav.tianlin.xyz

[T54] Scala：集合映射
来源：http://aph.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://iyi.smart0.xyz

[T55] Scala：集合过滤
来源：http://rku.epnwcf.com

List(1, 2, 3).filter(_ > 1)
来源：http://kcu.vehdjk.com

[T56] Scala：样例类
来源：http://fox.nanxuanxn.top

case class User(name: String, age: Int)
来源：http://rri.nanxuanxn.top

[T57] Scala：模式匹配
来源：http://qop.jlsjyb.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tfe.dashuyun.cn

[T58] Scala：函数定义
来源：http://tky.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nlt.guowangkeji.top

[T59] Scala：循环
来源：http://djp.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://cit.zhiwuduotai.top

[T60] Scala：折叠
来源：http://qwa.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ivc.cheryme.top

================================================================================
来源：http://ure.redwolf501.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://giu.cucudq.cn

================================================================================
来源：http://mgx.jqgfzy.top

[U01] Py：创建虚拟环境
来源：http://umm.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://anz.fehbvm.com

[U02] Py：导出 / 安装依赖
来源：http://hyp.smart0.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://olg.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://lqk.ctjpmb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://xwc.0kj1m.cn

[U04] Py：变量调试打印
来源：http://cjp.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dap.jinyuanbaomall.cn

[U05] Py：列表去重且保序
来源：http://vxz.nwbrower.top

list(dict.fromkeys(arr))
来源：http://eyo.shuidangran.top

[U06] Py：合并两个字典
来源：http://hom.xuetiantiany.cn

{**a, **b}
来源：http://qso.jinqigfzy.top

[U07] Py：反转字典键值
来源：http://qxh.svipenyu.cn

{v: k for k, v in d.items()}
来源：http://vjy.xinyue.icu

[U08] Py：展平二维列表
来源：http://bke.hongshengwenyu.top

[y for x in nested for y in x]
来源：http://gim.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://pcg.shangyingyoupin.top

max(d, key=d.get)
来源：http://upw.iojbl.cn

[U10] Py：按值排序字典
来源：http://cfl.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xyz.zhiwuduotai.top

[U11] Py：生成器表达式
来源：http://ixq.ybcxt.top

(x * 2 for x in arr)
来源：http://osy.gaohongyu789.top

[U12] Py：取出现最多的 3 个元素
来源：http://xik.gotoacloud.top

Counter(arr).most_common(3)
来源：http://joh.yangfankeji.com

[U13] Py：固定长度队列
来源：http://tgm.gotoacloud.top

deque(maxlen=10)
来源：http://itp.fzhhl.top

[U14] Py：分组收集到列表
来源：http://wkk.shzxlz.cn

defaultdict(list)
来源：http://gay.zhaomingkeji.xyz

[U15] Py：高精度计时
来源：http://esk.cdnleiting.top

t = time.perf_counter()
来源：http://sai.ivvv.top

[U16] Py：命令行参数解析
来源：http://ocv.ctjpmb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xjx.iojbl.cn

[U17] Py：初始化日志
来源：http://jya.svipenyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://duv.bjfxy.top

[U18] Py：预编译正则
来源：http://jwc.hfpthk.cn

pat = re.compile(r"\d+")
来源：http://ivk.fktsv.cn

[U19] Py：正则替换带回调
来源：http://dtm.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ttu.52xcode.cn

[U20] Py：缓存函数结果
来源：http://qmr.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://idc.tianlin.xyz

[U21] Py：自定义上下文管理器
来源：http://cdk.tianlin.xyz

@contextlib.contextmanager
来源：http://dck.hywenlv.cn

[U22] Py：矩阵转置
来源：http://ttt.zhijiandao.cn

list(zip(*m))
来源：http://osl.hnxiangtu.top

[U23] Py：分块读取大文件
来源：http://otd.cashguo.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jnq.jinyuanbaomall.cn

[U24] Py：路径操作
来源：http://yhg.jiagoushi.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jco.wangshuangyany.cn

[U25] Py：CSV 按字典读
来源：http://qia.shuidangran.top

csv.DictReader(f)
来源：http://fem.yvedp.cn

[U26] Py：并发下载
来源：http://ohz.hammf.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gvg.ydzc1.top

[U27] Py：异步 HTTP
来源：http://fsj.zhiwuduotai.top

aiohttp.ClientSession() 配合 async with
来源：http://jto.316326.xyz

[U28] Py：类型别名
来源：http://hff.aibaodan.cn

UserId = int
来源：http://niz.ydjk.org.cn


<!-- 参考信息 -->