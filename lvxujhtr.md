代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://gww.daxiang520.top

[S02] C：变量与格式化输出
来源：http://pxg.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://mru.c1oappe.top

[S03] C：读入整数
来源：http://ngd.9152youxi.cn

int x; scanf("%d", &x);
来源：http://yks.ydjk.org.cn

[S04] C：字符串复制
来源：http://bxo.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://hpn.fengsongda.top

[S05] C：字符串长度
来源：http://aur.nanxuanxn.top

strlen(s)
来源：http://yag.vehdjk.com

[S06] C：字符串比较
来源：http://xup.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://nda.yangfankeji.com

[S07] C：数组遍历求和
来源：http://tkq.jinqigfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qcw.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://ezk.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ogh.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://ejd.xylfe.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ugi.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://wss.ybcxt.top

int *p = &a;  *p = 5;
来源：http://zfl.nanxuanxn.top

[S11] C：逐行读文件
来源：http://lki.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://wvg.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vaf.jinyuanbaomall.cn

fclose(f);
来源：http://hai.jinghuilouyu.cn

[S12] C：写文件
来源：http://cen.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sja.uphjek.com

[S13] C：宏定义
来源：http://gsq.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gzr.52xcode.cn

[S14] C：枚举
来源：http://lyh.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://zpq.gotoacloud.top

[S15] C：类型转换
来源：http://jdi.guannengcc.top

(double) a / b
来源：http://ezk.yonumen.top

[S16] C：位操作置位
来源：http://dws.vehdjk.com

x |= (1 << 3);
来源：http://oix.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://dci.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://utx.ydzc1.top

[S18] C：命令行参数
来源：http://ylk.fehbvm.com

int main(int argc, char **argv)
来源：http://wul.kuanghao11.cn

[S19] C：快速排序
来源：http://pjx.ywan-chungtsiang.top

qsort(a, n, sizeof(int), cmp);
来源：http://wzw.yvedp.cn

[S20] C：二分查找
来源：http://svz.tarul.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kim.yongpay.top

[S21] C：字符类别判断
来源：http://nvt.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bss.vehdjk.com

[S22] C：字符串转数字
来源：http://ipk.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://cco.hywenlv.cn

[S23] C：随机数
来源：http://pkd.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fhr.fktsv.cn

[S24] C：获取本地时间
来源：http://wfd.xuetiantiany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wbu.yuxming.cn

[S25] C：内存拷贝
来源：http://dqy.hammf.cn

memcpy(dst, src, n);
来源：http://ahf.bbcook.cn

[S26] C：内存清零
来源：http://rfa.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://nqb.jlsjyb.cn

[S27] C：定义常量
来源：http://isn.nanxuanxn.top

const double PI = 3.14159;
来源：http://krv.uphjek.com

[S28] C：静态变量
来源：http://ioe.sjlbkw.cn

static int counter = 0;
来源：http://jnj.jqgfzy.top

[S29] C：变参函数
来源：http://gpr.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zwb.yuanzhike.top

[S30] C：头文件保护
来源：http://ojq.xingfuxueyuan.xyz

#ifndef X_H
来源：http://ppp.chenzaomai.com

#define X_H
来源：http://aec.andypj.xyz

#endif
来源：http://vhx.yj20258.top

[S31] C++：Hello World
来源：http://khi.yongpay.top

#include <iostream>
来源：http://enc.fzhhl.top

int main() { std::cout << "Hello\n"; }
来源：http://njk.xuetiantiany.cn

[S32] C++：字符串
来源：http://vqc.sweek.top

std::string s = "hi";  s += "!";
来源：http://qrl.cashguo.top

[S33] C++：vector 增删
来源：http://usy.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xqf.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://ngw.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://ciw.birdmap.top

[S35] C++：map
来源：http://fvm.gogol.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yur.fktsv.cn

[S36] C++：unordered_map
来源：http://uql.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wfy.fktsv.cn

[S37] C++：set
来源：http://tzw.chenlongwang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wuk.jlsjyb.cn

[S38] C++：排序
来源：http://czb.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://nhf.wangdashe.top

[S39] C++：自定义比较器排序
来源：http://hol.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vyk.pycfn.com

[S40] C++：查找元素
来源：http://jcd.gotoacloud.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sor.xylfe.cn

[S41] C++：类与构造函数
来源：http://rgc.daxiang520.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qdg.vqdsnc.cn

[S42] C++：继承与虚函数
来源：http://gha.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://vch.ctjpmb.com

[S43] C++：智能指针
来源：http://xpa.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://vqt.gaohongyu789.top

[S44] C++：引用传参
来源：http://hqr.vehdjk.com

void inc(int &x) { ++x; }
来源：http://lzc.daria6918.cn

[S45] C++：lambda
来源：http://vaa.redwolf501.top

auto add = [](int a, int b) { return a + b; };
来源：http://mgm.jiagoushi.top

[S46] C++：函数模板
来源：http://wwk.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kdg.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://yoc.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rrq.smart0.xyz

[S48] C++：逐行读文件
来源：http://zex.fzhhl.top

std::ifstream in("a.txt");  std::string line;
来源：http://hou.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://muk.jianghu66.top

[S49] C++：写文件
来源：http://yhs.fanxiaobao.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lsx.bjfxy.top

[S50] C++：格式化数字
来源：http://odv.quarkkingdee.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kaj.hcnkem.com

[S51] C++：显式类型转换
来源：http://knh.hcnkem.com

static_cast<double>(a) / b
来源：http://uae.chenjidiqi.icu

[S52] C++：const 与 noexcept
来源：http://vab.shanyushiyangkeji.top

int size() const noexcept { return n_; }
来源：http://wak.jinqigfzy.top

[S53] C++：移动语义
来源：http://wtb.zhixingplan.top

std::vector<int> w = std::move(v);
来源：http://ufk.hcnkem.com

[S54] C++：异常处理
来源：http://xiy.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://utx.xinyue.icu

[S55] C++：结构化绑定
来源：http://afb.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ipt.dianchejie.cn

[S56] C++：optional
来源：http://qgh.hysaishi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fkb.aizwys.cn

[S57] C++：编译期常量
来源：http://hkc.nanxinkj.top

constexpr int N = 10;
来源：http://jed.hcnkem.com

[S58] C++：命名空间
来源：http://gwq.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://iuv.zdqjudy.top

[S59] C++：静态断言
来源：http://osn.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vcn.yj20258.top

[S60] C++：遍历并删除元素
来源：http://aoi.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://avw.yj202588.top

================================================================================
来源：http://bml.zdqjudy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dir.cucudq.cn

================================================================================
来源：http://ubd.xuetiantiany.cn

[T01] Kotlin：Hello World
来源：http://lxb.sysykeji.top

println("Hello")
来源：http://lyk.fktsv.cn

[T02] Kotlin：变量
来源：http://fwb.yfazqb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://csa.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://jof.zhoulong.xyz

"值: $b"
来源：http://ood.pycfn.com

[T04] Kotlin：空安全
来源：http://ous.yuanzhike.top

val n: String? = null;  n?.length
来源：http://jtk.jyoumei.cn

[T05] Kotlin：when 表达式
来源：http://zvs.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iwz.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://vqc.sjlbkw.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://aof.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://spc.yvedp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ucn.jqgfzy.top

[T08] Kotlin：数据类
来源：http://qwe.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://oin.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://lmj.zycfv.cn

fun String.exclaim() = this + "!"
来源：http://bvd.ybcxt.top

[T10] Kotlin：默认参数
来源：http://pvw.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://upa.sweek.top

[T11] Kotlin：协程
来源：http://urx.9152youxi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jyx.0kj1m.cn

[T12] Kotlin：解构声明
来源：http://sjn.kuanghao11.cn

val (a, b) = Pair(1, 2)
来源：http://uvg.yj20258.top

[T13] Kotlin：只读 Map
来源：http://egz.nanxuanxn.top

val m = mapOf("a" to 1)
来源：http://gnj.epnwcf.com

[T14] Kotlin：循环
来源：http://lmr.birdmap.top

for (i in 1..10) println(i)
来源：http://qvj.hfpthk.cn

[T15] Kotlin：接口
来源：http://gjg.mhx1999.top

interface Shape { fun area(): Double }
来源：http://hyo.hesvh.cn

[T16] Swift：Hello World
来源：http://ske.gotoacloud.top

print("Hello")
来源：http://xis.fehbvm.com

[T17] Swift：变量与常量
来源：http://qfy.aizwys.cn

var a = 1;  let b = 2
来源：http://dme.havefunace.top

[T18] Swift：字符串插值
来源：http://nfc.hnqzz.top

"值: \(b)"
来源：http://ont.jinghuilouyu.cn

[T19] Swift：可选绑定
来源：http://axg.ctjpmb.com

if let n = opt { print(n) }
来源：http://eod.guannengcc.top

[T20] Swift：数组操作
来源：http://tmo.hammf.cn

var a = [1, 2, 3];  a.append(4)
来源：http://civ.ivvv.top

[T21] Swift：遍历
来源：http://tsh.yangfankeji.com

for x in a { print(x) }
来源：http://ekh.uphjek.com

[T22] Swift：字典
来源：http://dkj.yuxming.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xrg.shangyingyoupin.top

[T23] Swift：函数
来源：http://biy.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qqq.mhx1999.top

[T24] Swift：闭包
来源：http://oja.yfazqb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://hid.cqqwz.cn

[T25] Swift：结构体
来源：http://ksx.feifeiyinyue.top

struct P { var x: Int }
来源：http://ufb.fktsv.cn

[T26] Swift：类与重写
来源：http://udj.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://nsl.feifeiyinyue.top

[T27] Swift：错误处理
来源：http://fnm.fengsongda.top

do { try f() } catch { print(error) }
来源：http://wse.fzhhl.top

[T28] Swift：枚举
来源：http://vgv.jiagoushi.top

enum Color { case red, green }
来源：http://hiq.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://xjs.vehdjk.com

guard let x = opt else { return }
来源：http://ibl.hnxiangtu.top

[T30] Swift：协议
来源：http://yup.zhixingplan.top

protocol Shape { func area() -> Double }
来源：http://lut.cucudq.cn

[T31] Lua：Hello World
来源：http://chl.jlsjyb.cn

print("Hello")
来源：http://cxe.tarul.cn

[T32] Lua：局部变量
来源：http://xbn.hcnkem.com

local a = 1
来源：http://ism.cdnleiting.top

[T33] Lua：表（数组）
来源：http://xbn.hammf.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bag.9152youxi.cn

[T34] Lua：遍历表
来源：http://zti.gogol.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://str.fktsv.cn

[T35] Lua：字典表
来源：http://jql.sxryk.cn

local d = { a = 1 };  d.b = 2
来源：http://ifq.hammf.cn

[T36] Lua：函数
来源：http://iga.jinqigufen.top

function add(a, b) return a + b end
来源：http://mcc.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://psf.sufxvd.cn

"a" .. "b"
来源：http://nhq.yvedp.cn

[T38] Lua：条件
来源：http://uds.pycfn.com

if x > 0 then print("正") end
来源：http://cdd.vehdjk.com

[T39] Lua：模式匹配
来源：http://smu.dianchejie.cn

string.find(s, "%d+")
来源：http://kwo.jinghuilouyu.cn

[T40] Lua：元表
来源：http://mem.c1oappe.top

setmetatable({}, { __index = base })
来源：http://ked.yangfankeji.com

[T41] Perl：Hello World
来源：http://beh.pycfn.com

print "Hello\n";
来源：http://vvd.ehwqpu.com

[T42] Perl：变量类型
来源：http://bbm.sjlbkw.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tsr.zhengqikj.top

[T43] Perl：字符串插值
来源：http://exf.guowangkeji.top

"值: $a"
来源：http://jrp.yanxiufei.cn

[T44] Perl：条件
来源：http://dpl.zhongyouzk.top

if ($a > 0) { print "正"; }
来源：http://mxj.jyoumei.cn

[T45] Perl：数组遍历
来源：http://fqh.yonumen.top

for my $x (@arr) { print $x; }
来源：http://enx.ctjpmb.com

[T46] Perl：哈希操作
来源：http://syz.gzhubu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zyt.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://snx.zhongyouzk.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zap.tianlin.xyz

[T48] Perl：正则替换
来源：http://aue.jiagoushi.top

$s =~ s/old/new/g;
来源：http://gcy.chenjidiqi.icu

[T49] Perl：函数
来源：http://kdm.jinqigfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kxp.9152youxi.cn

[T50] Perl：逐行读文件
来源：http://lbf.yfazqb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://bfr.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://lkx.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://tin.andypj.xyz

println("Hello")
来源：http://jpf.wangdashe.top

[T52] Scala：变量
来源：http://dlt.wangdashe.top

val a = 1;  var b = 2
来源：http://mzk.havefunace.top

[T53] Scala：字符串插值
来源：http://nss.mhx1999.top

s"值: $b"
来源：http://cqm.daxiang520.top

[T54] Scala：集合映射
来源：http://pcg.zhongyouzk.top

List(1, 2, 3).map(_ * 2)
来源：http://uzj.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://tba.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jnf.hnqzz.top

[T56] Scala：样例类
来源：http://dru.shanyushiyangkeji.top

case class User(name: String, age: Int)
来源：http://whs.shzxlz.cn

[T57] Scala：模式匹配
来源：http://opk.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://vsj.xuanzx.com

[T58] Scala：函数定义
来源：http://nrn.snrcjt.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jye.jinghuilouyu.cn

[T59] Scala：循环
来源：http://wvf.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://wzn.bjfxy.top

[T60] Scala：折叠
来源：http://xot.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xmn.fzhhl.top

================================================================================
来源：http://tbe.daxiang520.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gvn.gotoacloud.top

================================================================================
来源：http://wmh.dianchejie.cn

[U01] Py：创建虚拟环境
来源：http://xbb.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://giv.guannengcc.top

[U02] Py：导出 / 安装依赖
来源：http://lzf.gogol.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bxd.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://ipm.xylfe.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rua.jlsjyb.cn

[U04] Py：变量调试打印
来源：http://xup.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tdq.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://xvt.dashuyun.cn

list(dict.fromkeys(arr))
来源：http://oqs.ppjwa.cn

[U06] Py：合并两个字典
来源：http://wgr.shanyushiyangtech.top

{**a, **b}
来源：http://qlb.zhiwuduotai.top

[U07] Py：反转字典键值
来源：http://dbj.xuanzx.com

{v: k for k, v in d.items()}
来源：http://oym.hongshengwenyu.top

[U08] Py：展平二维列表
来源：http://ovo.snrcjt.cn

[y for x in nested for y in x]
来源：http://zxu.hongshengwenyu.top

[U09] Py：字典取最大值的键
来源：http://wul.fehbvm.com

max(d, key=d.get)
来源：http://cor.xziqi.cn

[U10] Py：按值排序字典
来源：http://nxe.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rxz.hesvh.cn

[U11] Py：生成器表达式
来源：http://szl.fzhhl.top

(x * 2 for x in arr)
来源：http://arn.sysykeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://qqx.smart0.xyz

Counter(arr).most_common(3)
来源：http://nwo.iojbl.cn

[U13] Py：固定长度队列
来源：http://fid.nanxinkj.top

deque(maxlen=10)
来源：http://vvc.nwbrower.top

[U14] Py：分组收集到列表
来源：http://tci.fanxiaobao.xyz

defaultdict(list)
来源：http://cfi.shzxlz.cn

[U15] Py：高精度计时
来源：http://erv.shzxlz.cn

t = time.perf_counter()
来源：http://bne.fehbvm.com

[U16] Py：命令行参数解析
来源：http://fun.wangdashe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tnm.zhaomingkeji.xyz

[U17] Py：初始化日志
来源：http://whm.cucudq.cn

logging.basicConfig(level=logging.INFO)
来源：http://yna.yfazqb.com

[U18] Py：预编译正则
来源：http://gtb.gotoacloud.top

pat = re.compile(r"\d+")
来源：http://lfn.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://gwb.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yhi.fengsongda.top

[U20] Py：缓存函数结果
来源：http://buz.hywenlv.cn

@functools.lru_cache(maxsize=None)
来源：http://gly.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://kir.wangshuangyany.cn

@contextlib.contextmanager
来源：http://htr.shanyushiyangtech.top

[U22] Py：矩阵转置
来源：http://qss.shuidangran.top

list(zip(*m))
来源：http://cup.316326.xyz

[U23] Py：分块读取大文件
来源：http://ghs.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qzm.yuxming.cn

[U24] Py：路径操作
来源：http://xvb.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iex.wangdashe.top


<!-- 参考信息 -->