代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://tfx.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://kru.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://csw.fzhhl.top

[S03] C：读入整数
来源：http://vvy.zhongyouzk.top

int x; scanf("%d", &x);
来源：http://kgs.shuidangran.top

[S04] C：字符串复制
来源：http://qnv.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://rtr.ctjpmb.com

[S05] C：字符串长度
来源：http://xwu.tarul.cn

strlen(s)
来源：http://tpl.hfpthk.cn

[S06] C：字符串比较
来源：http://wsc.aizwys.cn

strcmp(a, b) == 0
来源：http://fya.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://qqq.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jcp.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://rzk.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://liw.xuanzx.com

[S09] C：结构体定义与初始化
来源：http://spg.yj202588.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vob.sysykeji.top

[S10] C：指针与解引用
来源：http://xmr.daxiang520.top

int *p = &a;  *p = 5;
来源：http://nyl.9152youxi.cn

[S11] C：逐行读文件
来源：http://sue.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://ndg.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://esb.snrcjt.cn

fclose(f);
来源：http://jgi.hnxiangtu.top

[S12] C：写文件
来源：http://iza.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ymm.jqgfzy.top

[S13] C：宏定义
来源：http://fkl.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://khl.jlsjyb.cn

[S14] C：枚举
来源：http://nln.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://fys.yfazqb.com

[S15] C：类型转换
来源：http://igu.redwolf501.top

(double) a / b
来源：http://vot.yj20258888.top

[S16] C：位操作置位
来源：http://igi.52xcode.cn

x |= (1 << 3);
来源：http://ayt.ybcxt.top

[S17] C：安全拼接字符串
来源：http://xom.cdnleiting.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vih.dashuyun.cn

[S18] C：命令行参数
来源：http://tbm.nwbrower.top

int main(int argc, char **argv)
来源：http://boz.ppjwa.cn

[S19] C：快速排序
来源：http://zsx.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jqx.yfazqb.com

[S20] C：二分查找
来源：http://wqh.wangdashe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yqd.jlsjyb.cn

[S21] C：字符类别判断
来源：http://vuv.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ijo.chenlongwang.top

[S22] C：字符串转数字
来源：http://vvk.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://jvq.haohaochexian.top

[S23] C：随机数
来源：http://trp.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://wyh.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://tmp.zhengqikj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://myq.mhx1999.top

[S25] C：内存拷贝
来源：http://fqz.svipenyu.cn

memcpy(dst, src, n);
来源：http://hgu.guannengcc.top

[S26] C：内存清零
来源：http://iat.mhx1999.top

memset(a, 0, sizeof a);
来源：http://pjl.daria6918.cn

[S27] C：定义常量
来源：http://wck.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://syx.yueranfly.top

[S28] C：静态变量
来源：http://lta.xuetiantiany.cn

static int counter = 0;
来源：http://aiu.zdbjq.cn

[S29] C：变参函数
来源：http://mlu.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nos.dianchejie.cn

[S30] C：头文件保护
来源：http://drr.jinghuilouyu.cn

#ifndef X_H
来源：http://dlm.yanxiufei.cn

#define X_H
来源：http://xqa.tianlin.xyz

#endif
来源：http://vut.yvedp.cn

[S31] C++：Hello World
来源：http://tpv.zhoulong.xyz

#include <iostream>
来源：http://zvx.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://nxt.chenjidiqi.icu

[S32] C++：字符串
来源：http://gjn.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://vbc.sxryk.cn

[S33] C++：vector 增删
来源：http://frg.daxiang520.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jox.yonumen.top

[S34] C++：遍历 vector
来源：http://pdg.jinqigfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://xsw.yvedp.cn

[S35] C++：map
来源：http://qlx.xziqi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://goo.xuanzx.com

[S36] C++：unordered_map
来源：http://llt.gogol.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://asd.cucudq.cn

[S37] C++：set
来源：http://evg.jqgfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kmd.xuetiantiany.cn

[S38] C++：排序
来源：http://wib.316326.xyz

std::sort(v.begin(), v.end());
来源：http://rxd.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://rnv.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oqv.zhoulong.xyz

[S40] C++：查找元素
来源：http://wqu.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cfq.jiagoushi.top

[S41] C++：类与构造函数
来源：http://ada.ydzc1.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yqp.feifeiyinyue.top

[S42] C++：继承与虚函数
来源：http://lwe.ydzc1.top

class B : public Base { public: void f() override {} };
来源：http://vjx.yj20258.top

[S43] C++：智能指针
来源：http://tnz.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://kib.jqgfzy.top

[S44] C++：引用传参
来源：http://tlr.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://cvz.yuxming.cn

[S45] C++：lambda
来源：http://yai.svipenyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fyk.dashuyun.cn

[S46] C++：函数模板
来源：http://kwv.jqgfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ybz.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://whm.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pxv.sufxvd.cn

[S48] C++：逐行读文件
来源：http://oxk.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://tjr.52xcode.cn

while (std::getline(in, line)) { }
来源：http://cks.fktsv.cn

[S49] C++：写文件
来源：http://btg.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gdy.gogol.net.cn

[S50] C++：格式化数字
来源：http://zhq.wangshuangyany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kze.zhongyouzk.top

[S51] C++：显式类型转换
来源：http://vsi.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://jej.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://raa.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://hnm.xingfuxueyuan.xyz

[S53] C++：移动语义
来源：http://dfz.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://klw.smart0.xyz

[S54] C++：异常处理
来源：http://yvq.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wbo.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://trq.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wiw.zhoulong.xyz

[S56] C++：optional
来源：http://xbo.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vic.hfpthk.cn

[S57] C++：编译期常量
来源：http://pck.vqdsnc.cn

constexpr int N = 10;
来源：http://axz.ydjk.org.cn

[S58] C++：命名空间
来源：http://hht.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://cea.nanxinkj.top

[S59] C++：静态断言
来源：http://gvn.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://koc.shzxlz.cn

[S60] C++：遍历并删除元素
来源：http://pye.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kvm.chenjidiqi.icu

================================================================================
来源：http://dko.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xpf.jianghu66.top

================================================================================
来源：http://ibe.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://kyd.ydzc1.top

println("Hello")
来源：http://egl.fktsv.cn

[T02] Kotlin：变量
来源：http://zyj.gzhubu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lxl.cheryme.top

[T03] Kotlin：字符串模板
来源：http://fls.ydjk.org.cn

"值: $b"
来源：http://gar.yangfankeji.com

[T04] Kotlin：空安全
来源：http://rkp.birdmap.top

val n: String? = null;  n?.length
来源：http://rad.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://ovb.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ieu.yueranfly.top

[T06] Kotlin：集合映射
来源：http://nwy.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cxr.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://reh.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ucx.chenzaomai.com

[T08] Kotlin：数据类
来源：http://qag.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://aoo.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://jso.meibo888.top

fun String.exclaim() = this + "!"
来源：http://gju.jinghuilouyu.cn

[T10] Kotlin：默认参数
来源：http://kuv.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qwe.chenjidiqi.icu

[T11] Kotlin：协程
来源：http://mts.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tkb.tarul.cn

[T12] Kotlin：解构声明
来源：http://vac.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://bjr.gzhubu.top

[T13] Kotlin：只读 Map
来源：http://feo.ydjk.org.cn

val m = mapOf("a" to 1)
来源：http://nzv.yfazqb.com

[T14] Kotlin：循环
来源：http://ncj.vehdjk.com

for (i in 1..10) println(i)
来源：http://urj.0kj1m.cn

[T15] Kotlin：接口
来源：http://rpn.xinyue.icu

interface Shape { fun area(): Double }
来源：http://ips.yangfankeji.com

[T16] Swift：Hello World
来源：http://ziz.shuidangran.top

print("Hello")
来源：http://frj.pengpengdd.cyou

[T17] Swift：变量与常量
来源：http://tnj.zhaomingkeji.xyz

var a = 1;  let b = 2
来源：http://ezj.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://nxi.jinghuilouyu.cn

"值: \(b)"
来源：http://tqj.birdmap.top

[T19] Swift：可选绑定
来源：http://oxt.yj202588.top

if let n = opt { print(n) }
来源：http://tfc.yj20258.top

[T20] Swift：数组操作
来源：http://nfo.yanxiufei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qrn.uphjek.com

[T21] Swift：遍历
来源：http://xpz.tarul.cn

for x in a { print(x) }
来源：http://ksh.ppjwa.cn

[T22] Swift：字典
来源：http://xte.meibo888.top

var d = ["a": 1];  d["b"] = 2
来源：http://jpd.birdmap.top

[T23] Swift：函数
来源：http://pjo.hammf.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://boo.meibo888.top

[T24] Swift：闭包
来源：http://qeq.vehdjk.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://kma.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://ucj.yonumen.top

struct P { var x: Int }
来源：http://xng.cashguo.top

[T26] Swift：类与重写
来源：http://jdw.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://ols.mhx1999.top

[T27] Swift：错误处理
来源：http://xlz.zhiwuduotai.top

do { try f() } catch { print(error) }
来源：http://poj.jianghu66.top

[T28] Swift：枚举
来源：http://qfc.jyoumei.cn

enum Color { case red, green }
来源：http://gue.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://euo.cashguo.top

guard let x = opt else { return }
来源：http://kng.gotoacloud.top

[T30] Swift：协议
来源：http://ueo.pengpengdd.cyou

protocol Shape { func area() -> Double }
来源：http://tnf.xylfe.cn

[T31] Lua：Hello World
来源：http://tqd.haohaochexian.top

print("Hello")
来源：http://ukp.fzhhl.top

[T32] Lua：局部变量
来源：http://pep.ybcxt.top

local a = 1
来源：http://wsd.chenjidiqi.icu

[T33] Lua：表（数组）
来源：http://odg.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://yjf.vqdsnc.cn

[T34] Lua：遍历表
来源：http://bmr.bbcook.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gnf.ydjk.org.cn

[T35] Lua：字典表
来源：http://vuy.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://oeq.wangshuangyany.cn

[T36] Lua：函数
来源：http://lgg.svipenyu.cn

function add(a, b) return a + b end
来源：http://kjh.cucudq.cn

[T37] Lua：字符串拼接
来源：http://naf.hfpthk.cn

"a" .. "b"
来源：http://npx.ivvv.top

[T38] Lua：条件
来源：http://nfx.guowangkeji.top

if x > 0 then print("正") end
来源：http://zxl.gzhubu.top

[T39] Lua：模式匹配
来源：http://skk.cheryme.top

string.find(s, "%d+")
来源：http://kuj.9152youxi.cn

[T40] Lua：元表
来源：http://poe.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://wvr.birdmap.top

[T41] Perl：Hello World
来源：http://zuz.tian-w.cn

print "Hello\n";
来源：http://iqx.gzhubu.top

[T42] Perl：变量类型
来源：http://ygn.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dvm.bbcook.cn

[T43] Perl：字符串插值
来源：http://zme.yj20258.top

"值: $a"
来源：http://zyc.zdqjudy.top

[T44] Perl：条件
来源：http://yoz.tanke756.top

if ($a > 0) { print "正"; }
来源：http://djz.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://aqk.snrcjt.cn

for my $x (@arr) { print $x; }
来源：http://rcd.zdbjq.cn

[T46] Perl：哈希操作
来源：http://rta.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xce.smart0.xyz

[T47] Perl：正则捕获
来源：http://xtv.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kkz.yvedp.cn

[T48] Perl：正则替换
来源：http://euv.jinqigufen.top

$s =~ s/old/new/g;
来源：http://dti.cqqwz.cn

[T49] Perl：函数
来源：http://tbm.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rkv.nanxinkj.top

[T50] Perl：逐行读文件
来源：http://atm.yfazqb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://hnz.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://bwy.hywenlv.cn

[T51] Scala：Hello World
来源：http://cah.ydjk.org.cn

println("Hello")
来源：http://ili.daria6918.cn

[T52] Scala：变量
来源：http://rsk.hnqzz.top

val a = 1;  var b = 2
来源：http://itc.yuanzhike.top

[T53] Scala：字符串插值
来源：http://nke.yonumen.top

s"值: $b"
来源：http://cfc.iojbl.cn

[T54] Scala：集合映射
来源：http://efy.hesvh.cn

List(1, 2, 3).map(_ * 2)
来源：http://hjo.hnqzz.top

[T55] Scala：集合过滤
来源：http://epv.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://psw.wangdashe.top

[T56] Scala：样例类
来源：http://qcm.havefunace.top

case class User(name: String, age: Int)
来源：http://ide.kuanghao11.cn

[T57] Scala：模式匹配
来源：http://ejv.yonumen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fxf.yuxming.cn

[T58] Scala：函数定义
来源：http://qlr.shanyushiyangtech.top

def add(a: Int, b: Int): Int = a + b
来源：http://wsy.andypj.xyz

[T59] Scala：循环
来源：http://dzy.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://xvh.xingfuxueyuan.xyz

[T60] Scala：折叠
来源：http://aqk.xuanzx.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mdl.fehbvm.com

================================================================================
来源：http://fdg.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kdu.ivvv.top

================================================================================
来源：http://jfn.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://enl.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://rin.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://lnr.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ywx.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://gjy.cdnleiting.top

from dotenv import load_dotenv; load_dotenv()
来源：http://isq.yuanzhike.top

[U04] Py：变量调试打印
来源：http://bet.ydzc1.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ghn.bbcook.cn

[U05] Py：列表去重且保序
来源：http://ouz.xziqi.cn

list(dict.fromkeys(arr))
来源：http://vpf.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://thv.jqgfzy.top

{**a, **b}
来源：http://tqp.shanyushiyangkeji.top

[U07] Py：反转字典键值
来源：http://okk.sxryk.cn

{v: k for k, v in d.items()}
来源：http://axc.cdnleiting.top

[U08] Py：展平二维列表
来源：http://ffl.dianchejie.cn

[y for x in nested for y in x]
来源：http://ire.vehdjk.com

[U09] Py：字典取最大值的键
来源：http://czp.fehbvm.com

max(d, key=d.get)
来源：http://pjz.xylfe.cn

[U10] Py：按值排序字典
来源：http://str.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zcu.cucudq.cn

[U11] Py：生成器表达式
来源：http://gdq.yanxiufei.cn

(x * 2 for x in arr)
来源：http://bik.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://bfy.hnqzz.top

Counter(arr).most_common(3)
来源：http://vkh.vqdsnc.cn

[U13] Py：固定长度队列
来源：http://gpm.gotoacloud.top

deque(maxlen=10)
来源：http://kaw.birdmap.top

[U14] Py：分组收集到列表
来源：http://yjm.ppjwa.cn

defaultdict(list)
来源：http://xnd.hnxiangtu.top

[U15] Py：高精度计时
来源：http://efw.iojbl.cn

t = time.perf_counter()
来源：http://pmy.iojbl.cn

[U16] Py：命令行参数解析
来源：http://jqk.bbcook.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kkb.jyoumei.cn

[U17] Py：初始化日志
来源：http://zds.shanyushiyangtech.top

logging.basicConfig(level=logging.INFO)
来源：http://bzk.yueranfly.top

[U18] Py：预编译正则
来源：http://prc.fktsv.cn

pat = re.compile(r"\d+")
来源：http://ual.yj202588.top

[U19] Py：正则替换带回调
来源：http://lgs.jinyuanbaomall.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lpc.mhx1999.top

[U20] Py：缓存函数结果
来源：http://iqr.snrcjt.cn

@functools.lru_cache(maxsize=None)
来源：http://krr.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://nor.yuanzhike.top

@contextlib.contextmanager
来源：http://lsd.shangyingyoupin.top

[U22] Py：矩阵转置
来源：http://qpe.feifeiyinyue.top

list(zip(*m))
来源：http://nqx.jiagoushi.top

[U23] Py：分块读取大文件
来源：http://buq.0kj1m.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hsr.hongshengwenyu.top

[U24] Py：路径操作
来源：http://vyv.zhijiandao.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ftp.hesvh.cn


<!-- 参考信息 -->