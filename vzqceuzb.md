代发 wailian999

S. C / C++ 专题
来源：http://jqn.hnqzz.top

================================================================================
来源：http://vpn.zdqjudy.top

[S01] C：Hello World
来源：http://gzy.jinqigufen.top

#include <stdio.h>
来源：http://wmm.nanxinkj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dfy.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://vpq.wangshuangyany.cn

int a = 10; printf("%d\n", a);
来源：http://hbw.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://ukp.yfazqb.com

int x; scanf("%d", &x);
来源：http://vuc.guowangkeji.top

[S04] C：字符串复制
来源：http://zut.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yzz.yj20258888.top

[S05] C：字符串长度
来源：http://bmn.zhijiandao.cn

strlen(s)
来源：http://hze.snrcjt.cn

[S06] C：字符串比较
来源：http://aaw.cashguo.top

strcmp(a, b) == 0
来源：http://vyf.hnqzz.top

[S07] C：数组遍历求和
来源：http://hqz.meibo888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uiu.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://xkj.yuxming.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wbf.xinyue.icu

[S09] C：结构体定义与初始化
来源：http://uav.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mvc.vehdjk.com

[S10] C：指针与解引用
来源：http://vam.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://zox.tian-w.cn

[S11] C：逐行读文件
来源：http://oxr.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://cnc.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ofz.aibaodan.cn

fclose(f);
来源：http://xfz.snrcjt.cn

[S12] C：写文件
来源：http://gqe.yvedp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pof.316326.xyz

[S13] C：宏定义
来源：http://kpd.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jtg.wangshuangyany.cn

[S14] C：枚举
来源：http://ftu.nwbrower.top

enum Color { RED, GREEN, BLUE };
来源：http://ctl.hesvh.cn

[S15] C：类型转换
来源：http://xls.zhengqikj.top

(double) a / b
来源：http://qen.yuanzhike.top

[S16] C：位操作置位
来源：http://hkq.cucudq.cn

x |= (1 << 3);
来源：http://bpa.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://skw.sysykeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qkd.ehwqpu.com

[S18] C：命令行参数
来源：http://vmj.jiagoushi.top

int main(int argc, char **argv)
来源：http://gec.gaohongyu789.top

[S19] C：快速排序
来源：http://uev.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://riz.dianchejie.cn

[S20] C：二分查找
来源：http://xvz.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oar.haohaochexian.top

[S21] C：字符类别判断
来源：http://cgn.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bkf.316326.xyz

[S22] C：字符串转数字
来源：http://lps.zhiwuduotai.top

atoi("42");  strtod("3.14", NULL);
来源：http://byk.tanke756.top

[S23] C：随机数
来源：http://gbh.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://suu.cqqwz.cn

[S24] C：获取本地时间
来源：http://gjt.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fda.ppjwa.cn

[S25] C：内存拷贝
来源：http://fvl.haohaochexian.top

memcpy(dst, src, n);
来源：http://xkg.dashuyun.cn

[S26] C：内存清零
来源：http://cde.316326.xyz

memset(a, 0, sizeof a);
来源：http://wpo.redwolf501.top

[S27] C：定义常量
来源：http://ufy.shzxlz.cn

const double PI = 3.14159;
来源：http://qyh.jinghuilouyu.cn

[S28] C：静态变量
来源：http://mme.jqgfzy.top

static int counter = 0;
来源：http://ddu.cqqwz.cn

[S29] C：变参函数
来源：http://sey.jianghu66.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nqq.zhengqikj.top

[S30] C：头文件保护
来源：http://lva.fzhhl.top

#ifndef X_H
来源：http://sta.sxryk.cn

#define X_H
来源：http://tli.316326.xyz

#endif
来源：http://mkf.guannengcc.top

[S31] C++：Hello World
来源：http://gpq.tarul.cn

#include <iostream>
来源：http://ocj.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://qbc.daxiang520.top

[S32] C++：字符串
来源：http://qro.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://ang.cheryme.top

[S33] C++：vector 增删
来源：http://jcy.yanxiufei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://frv.gzhubu.top

[S34] C++：遍历 vector
来源：http://qfz.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://pkp.sweek.top

[S35] C++：map
来源：http://ler.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iip.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://xcj.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sci.dianchejie.cn

[S37] C++：set
来源：http://rrb.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sfo.bjfxy.top

[S38] C++：排序
来源：http://xhc.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://ggt.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://reu.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gob.xylfe.cn

[S40] C++：查找元素
来源：http://lhr.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pwv.yangfankeji.com

[S41] C++：类与构造函数
来源：http://rut.zhixingplan.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hem.hesvh.cn

[S42] C++：继承与虚函数
来源：http://uwt.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://vib.xingfuxueyuan.xyz

[S43] C++：智能指针
来源：http://gln.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://ech.bbcook.cn

[S44] C++：引用传参
来源：http://ovh.yj20258.top

void inc(int &x) { ++x; }
来源：http://ayb.uphjek.com

[S45] C++：lambda
来源：http://efo.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://aai.yuanzhike.top

[S46] C++：函数模板
来源：http://djc.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nih.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://tuo.ctjpmb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dsf.dashuyun.cn

[S48] C++：逐行读文件
来源：http://xfc.dianchejie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://utc.dashuyun.cn

while (std::getline(in, line)) { }
来源：http://pyi.gotoacloud.top

[S49] C++：写文件
来源：http://mnl.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vwv.zhixingplan.top

[S50] C++：格式化数字
来源：http://nni.bjfxy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rxr.yongpay.top

[S51] C++：显式类型转换
来源：http://jij.sxryk.cn

static_cast<double>(a) / b
来源：http://mcx.zhoulong.xyz

[S52] C++：const 与 noexcept
来源：http://ibp.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://ggo.wangdashe.top

[S53] C++：移动语义
来源：http://sgz.yvedp.cn

std::vector<int> w = std::move(v);
来源：http://ohk.yueranfly.top

[S54] C++：异常处理
来源：http://zqb.zhongyouzk.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eba.tian-w.cn

[S55] C++：结构化绑定
来源：http://zqh.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cvk.ehwqpu.com

[S56] C++：optional
来源：http://gco.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yab.sufxvd.cn

[S57] C++：编译期常量
来源：http://ezv.guowangkeji.top

constexpr int N = 10;
来源：http://txo.feifeiyinyue.top

[S58] C++：命名空间
来源：http://sod.uphjek.com

namespace ns { int f() { return 1; } }
来源：http://sov.gogol.net.cn

[S59] C++：静态断言
来源：http://dhl.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zfp.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://wep.nanxinkj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://stn.zhiwuduotai.top

================================================================================
来源：http://wop.cqqwz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ipu.xylfe.cn

================================================================================
来源：http://awz.gotoacloud.top

[T01] Kotlin：Hello World
来源：http://mqe.meibo888.top

println("Hello")
来源：http://vaq.9152youxi.cn

[T02] Kotlin：变量
来源：http://xkw.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kbo.zhijiandao.cn

[T03] Kotlin：字符串模板
来源：http://yri.jianghu66.top

"值: $b"
来源：http://pqj.tarul.cn

[T04] Kotlin：空安全
来源：http://uwg.fengsongda.top

val n: String? = null;  n?.length
来源：http://fzb.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://rsz.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uap.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://tay.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ryu.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://yqg.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dhp.yangfankeji.com

[T08] Kotlin：数据类
来源：http://ymv.yj20258.top

data class User(val name: String, val age: Int)
来源：http://kai.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://tqb.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://aui.bjfxy.top

[T10] Kotlin：默认参数
来源：http://kwg.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ovk.tian-w.cn

[T11] Kotlin：协程
来源：http://mqe.xinyue.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://wlr.fktsv.cn

[T12] Kotlin：解构声明
来源：http://bsl.zhengqikj.top

val (a, b) = Pair(1, 2)
来源：http://dee.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://uds.gaohongyu789.top

val m = mapOf("a" to 1)
来源：http://qbo.52xcode.cn

[T14] Kotlin：循环
来源：http://ipx.andypj.xyz

for (i in 1..10) println(i)
来源：http://uyv.hnqzz.top

[T15] Kotlin：接口
来源：http://kpx.ydzc1.top

interface Shape { fun area(): Double }
来源：http://gwt.nanxuanxn.top

[T16] Swift：Hello World
来源：http://xrd.jqgufenzy.top

print("Hello")
来源：http://mgf.fzhhl.top

[T17] Swift：变量与常量
来源：http://lvr.0kj1m.cn

var a = 1;  let b = 2
来源：http://pcu.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://vxg.shanyushiyangkeji.top

"值: \(b)"
来源：http://piu.ydzc1.top

[T19] Swift：可选绑定
来源：http://udt.fzhhl.top

if let n = opt { print(n) }
来源：http://fnp.uphjek.com

[T20] Swift：数组操作
来源：http://qqd.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://akv.xinyue.icu

[T21] Swift：遍历
来源：http://ocb.yueranfly.top

for x in a { print(x) }
来源：http://obn.ctjpmb.com

[T22] Swift：字典
来源：http://emj.vqdsnc.cn

var d = ["a": 1];  d["b"] = 2
来源：http://syg.yuxming.cn

[T23] Swift：函数
来源：http://fed.vqdsnc.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jpr.jqgufenzy.top

[T24] Swift：闭包
来源：http://cqt.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kpk.hcnkem.com

[T25] Swift：结构体
来源：http://gig.dianchejie.cn

struct P { var x: Int }
来源：http://zwo.316326.xyz

[T26] Swift：类与重写
来源：http://wfm.ivvv.top

class A: Base { override func f() {} }
来源：http://hgd.sysykeji.top

[T27] Swift：错误处理
来源：http://owo.kuanghao11.cn

do { try f() } catch { print(error) }
来源：http://gse.ydjk.org.cn

[T28] Swift：枚举
来源：http://bsi.pengpengdd.cyou

enum Color { case red, green }
来源：http://iej.nwbrower.top

[T29] Swift：guard 提前返回
来源：http://ecn.fengsongda.top

guard let x = opt else { return }
来源：http://tza.bbcook.cn

[T30] Swift：协议
来源：http://yjo.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://inb.ydzc1.top

[T31] Lua：Hello World
来源：http://tkt.zhengqikj.top

print("Hello")
来源：http://nhh.cdnleiting.top

[T32] Lua：局部变量
来源：http://llc.xuetiantiany.cn

local a = 1
来源：http://niz.cucudq.cn

[T33] Lua：表（数组）
来源：http://cqj.redwolf501.top

local t = {1, 2, 3};  t[4] = 4
来源：http://oda.dianchejie.cn

[T34] Lua：遍历表
来源：http://wdn.gaohongyu789.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cfx.cqqwz.cn

[T35] Lua：字典表
来源：http://dje.chenlongwang.top

local d = { a = 1 };  d.b = 2
来源：http://ugt.shuidangran.top

[T36] Lua：函数
来源：http://apw.cqqwz.cn

function add(a, b) return a + b end
来源：http://lhc.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://geb.ppjwa.cn

"a" .. "b"
来源：http://juw.hysaishi.cn

[T38] Lua：条件
来源：http://nwj.daria6918.cn

if x > 0 then print("正") end
来源：http://end.sjlbkw.cn

[T39] Lua：模式匹配
来源：http://csg.kuanghao11.cn

string.find(s, "%d+")
来源：http://ylv.chenlongwang.top

[T40] Lua：元表
来源：http://udu.wangdashe.top

setmetatable({}, { __index = base })
来源：http://kdj.sufxvd.cn

[T41] Perl：Hello World
来源：http://rlt.ivvv.top

print "Hello\n";
来源：http://jnb.cashguo.top

[T42] Perl：变量类型
来源：http://osz.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zey.gzhubu.top

[T43] Perl：字符串插值
来源：http://dxt.smart0.xyz

"值: $a"
来源：http://jvz.meibo888.top

[T44] Perl：条件
来源：http://roy.ybcxt.top

if ($a > 0) { print "正"; }
来源：http://ftf.zhengqikj.top

[T45] Perl：数组遍历
来源：http://pia.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://nnu.zdqjudy.top

[T46] Perl：哈希操作
来源：http://doc.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://new.sjlbkw.cn

[T47] Perl：正则捕获
来源：http://vos.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vqi.epnwcf.com

[T48] Perl：正则替换
来源：http://mum.andypj.xyz

$s =~ s/old/new/g;
来源：http://byn.andypj.xyz

[T49] Perl：函数
来源：http://tzw.shuidangran.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cfa.dashuyun.cn

[T50] Perl：逐行读文件
来源：http://bkj.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fbh.svipenyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://kgo.jinghuilouyu.cn

[T51] Scala：Hello World
来源：http://tbv.jinyuanbaomall.cn

println("Hello")
来源：http://trl.cheryme.top

[T52] Scala：变量
来源：http://gal.zhengqikj.top

val a = 1;  var b = 2
来源：http://pxl.zhixingplan.top

[T53] Scala：字符串插值
来源：http://krr.zycfv.cn

s"值: $b"
来源：http://dhe.xziqi.cn

[T54] Scala：集合映射
来源：http://rli.jyoumei.cn

List(1, 2, 3).map(_ * 2)
来源：http://vpj.chenjidiqi.icu

[T55] Scala：集合过滤
来源：http://yck.haohaochexian.top

List(1, 2, 3).filter(_ > 1)
来源：http://faz.yangfankeji.com

[T56] Scala：样例类
来源：http://aeq.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://kuf.andypj.xyz

[T57] Scala：模式匹配
来源：http://arm.nanxinkj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://aux.jyoumei.cn

[T58] Scala：函数定义
来源：http://izj.hysaishi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gqh.nwbrower.top

[T59] Scala：循环
来源：http://sat.zhijiandao.cn

for (i <- 1 to 10) println(i)
来源：http://emc.pengpengdd.cyou

[T60] Scala：折叠
来源：http://lkc.sufxvd.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ctx.sufxvd.cn

================================================================================
来源：http://cci.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gkt.ydjk.org.cn

================================================================================
来源：http://oki.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://ybi.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://lcc.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://ezk.zdqjudy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vnl.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://vtt.c1oappe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fhr.zycfv.cn

[U04] Py：变量调试打印
来源：http://lkl.yonumen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ykz.jqgfzy.top

[U05] Py：列表去重且保序
来源：http://kyu.zycfv.cn

list(dict.fromkeys(arr))
来源：http://smx.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://ngc.zycfv.cn

{**a, **b}
来源：http://qqg.sufxvd.cn

[U07] Py：反转字典键值
来源：http://rdz.aibaodan.cn

{v: k for k, v in d.items()}
来源：http://eur.hywenlv.cn

[U08] Py：展平二维列表
来源：http://cqt.hongshengwenyu.top

[y for x in nested for y in x]
来源：http://gdo.shanyushiyangkeji.top

[U09] Py：字典取最大值的键
来源：http://dco.dashuyun.cn

max(d, key=d.get)
来源：http://ubl.aizwys.cn

[U10] Py：按值排序字典
来源：http://iaz.ivvv.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tjo.ppjwa.cn

[U11] Py：生成器表达式
来源：http://xtb.sufxvd.cn

(x * 2 for x in arr)
来源：http://kui.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://qnf.svipenyu.cn

Counter(arr).most_common(3)
来源：http://glf.tian-w.cn

[U13] Py：固定长度队列
来源：http://znm.zhengqikj.top

deque(maxlen=10)
来源：http://iiz.tarul.cn

[U14] Py：分组收集到列表
来源：http://ddh.dianchejie.cn

defaultdict(list)
来源：http://dix.cucudq.cn

[U15] Py：高精度计时
来源：http://mnc.cqqwz.cn

t = time.perf_counter()
来源：http://pcw.cucudq.cn

[U16] Py：命令行参数解析
来源：http://azt.tian-w.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://krr.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://fbb.daria6918.cn

logging.basicConfig(level=logging.INFO)
来源：http://fyf.mhx1999.top

[U18] Py：预编译正则
来源：http://zgp.hysaishi.cn

pat = re.compile(r"\d+")
来源：http://kno.sysykeji.top

[U19] Py：正则替换带回调
来源：http://dkp.gaohongyu789.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ihi.fzhhl.top

[U20] Py：缓存函数结果
来源：http://hwu.andypj.xyz

@functools.lru_cache(maxsize=None)
来源：http://rqg.c1oappe.top

[U21] Py：自定义上下文管理器
来源：http://wko.zhaomingkeji.xyz

@contextlib.contextmanager
来源：http://kke.zhiwuduotai.top

[U22] Py：矩阵转置
来源：http://tpy.ctjpmb.com

list(zip(*m))
来源：http://vuz.epnwcf.com


<!-- 参考信息 -->