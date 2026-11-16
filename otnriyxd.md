代发 wailian999

S. C / C++ 专题
来源：http://cdr.ivvv.top

================================================================================
来源：http://pay.xziqi.cn

[S01] C：Hello World
来源：http://iet.gotoacloud.top

#include <stdio.h>
来源：http://pcz.chenzaomai.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://kav.xylfe.cn

[S02] C：变量与格式化输出
来源：http://ppn.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://oml.nwbrower.top

[S03] C：读入整数
来源：http://tgv.fzhhl.top

int x; scanf("%d", &x);
来源：http://hqi.jyoumei.cn

[S04] C：字符串复制
来源：http://ptf.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://jju.fehbvm.com

[S05] C：字符串长度
来源：http://zed.quarkkingdee.top

strlen(s)
来源：http://svf.fengsongda.top

[S06] C：字符串比较
来源：http://iyo.jqgfzy.top

strcmp(a, b) == 0
来源：http://kvc.chenlongwang.top

[S07] C：数组遍历求和
来源：http://slo.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qyj.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://pjo.ehwqpu.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://apr.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://gzs.cashguo.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://naw.hesvh.cn

[S10] C：指针与解引用
来源：http://abh.gzhubu.top

int *p = &a;  *p = 5;
来源：http://tjf.fehbvm.com

[S11] C：逐行读文件
来源：http://qfr.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://xhy.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://eth.jiagoushi.top

fclose(f);
来源：http://wcv.chenlongwang.top

[S12] C：写文件
来源：http://otm.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jvg.jinqigfzy.top

[S13] C：宏定义
来源：http://htm.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tgx.nanxuanxn.top

[S14] C：枚举
来源：http://kuf.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://bxt.ppjwa.cn

[S15] C：类型转换
来源：http://ueg.iojbl.cn

(double) a / b
来源：http://fit.wangdashe.top

[S16] C：位操作置位
来源：http://ary.zhaomingkeji.xyz

x |= (1 << 3);
来源：http://icq.xuanzx.com

[S17] C：安全拼接字符串
来源：http://pdk.iojbl.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ruv.bbcook.cn

[S18] C：命令行参数
来源：http://gmh.fengsongda.top

int main(int argc, char **argv)
来源：http://vmo.xuanzx.com

[S19] C：快速排序
来源：http://iob.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://ful.aibaodan.cn

[S20] C：二分查找
来源：http://kfc.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bwg.ctjpmb.com

[S21] C：字符类别判断
来源：http://lyg.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sif.xuetiantiany.cn

[S22] C：字符串转数字
来源：http://rll.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://fpo.jiagoushi.top

[S23] C：随机数
来源：http://xke.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bbr.daxiang520.top

[S24] C：获取本地时间
来源：http://aje.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yvm.zycfv.cn

[S25] C：内存拷贝
来源：http://ybz.wangdashe.top

memcpy(dst, src, n);
来源：http://ram.nanxinkj.top

[S26] C：内存清零
来源：http://dsj.xinyue.icu

memset(a, 0, sizeof a);
来源：http://wrx.guannengcc.top

[S27] C：定义常量
来源：http://qbd.dianchejie.cn

const double PI = 3.14159;
来源：http://pqs.shanyushiyangtech.top

[S28] C：静态变量
来源：http://ekt.hcnkem.com

static int counter = 0;
来源：http://tiu.jinqigfzy.top

[S29] C：变参函数
来源：http://wlc.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qvm.mhx1999.top

[S30] C：头文件保护
来源：http://res.9152youxi.cn

#ifndef X_H
来源：http://brb.mhx1999.top

#define X_H
来源：http://yjr.guannengcc.top

#endif
来源：http://byn.iojbl.cn

[S31] C++：Hello World
来源：http://gne.shzxlz.cn

#include <iostream>
来源：http://hht.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://uvt.daria6918.cn

[S32] C++：字符串
来源：http://bjk.cheryme.top

std::string s = "hi";  s += "!";
来源：http://dnd.fktsv.cn

[S33] C++：vector 增删
来源：http://noj.pengpengdd.cyou

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ylh.fanxiaobao.xyz

[S34] C++：遍历 vector
来源：http://ter.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://qni.sufxvd.cn

[S35] C++：map
来源：http://cvi.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zov.ydzc1.top

[S36] C++：unordered_map
来源：http://bez.chenjidiqi.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kjw.shanyushiyangkeji.top

[S37] C++：set
来源：http://vil.chenlongwang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wfu.vqdsnc.cn

[S38] C++：排序
来源：http://yyn.tanke756.top

std::sort(v.begin(), v.end());
来源：http://ppi.jinqigufen.top

[S39] C++：自定义比较器排序
来源：http://wxd.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aec.jinghuilouyu.cn

[S40] C++：查找元素
来源：http://ecl.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gvq.bbcook.cn

[S41] C++：类与构造函数
来源：http://vye.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ssd.zhengqikj.top

[S42] C++：继承与虚函数
来源：http://iju.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://jgm.ppjwa.cn

[S43] C++：智能指针
来源：http://iat.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://fzi.jyoumei.cn

[S44] C++：引用传参
来源：http://vjr.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://xmu.quarkkingdee.top

[S45] C++：lambda
来源：http://szb.smart0.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://lpn.nanxinkj.top

[S46] C++：函数模板
来源：http://idd.dianchejie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hao.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://szz.guannengcc.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qtg.yangfankeji.com

[S48] C++：逐行读文件
来源：http://ugb.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://now.guannengcc.top

while (std::getline(in, line)) { }
来源：http://jns.tanke756.top

[S49] C++：写文件
来源：http://qjt.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rjc.c1oappe.top

[S50] C++：格式化数字
来源：http://hal.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://asv.yj20258.top

[S51] C++：显式类型转换
来源：http://esv.ydjk.org.cn

static_cast<double>(a) / b
来源：http://acz.jqgfzy.top

[S52] C++：const 与 noexcept
来源：http://ooy.smart0.xyz

int size() const noexcept { return n_; }
来源：http://skh.wangdashe.top

[S53] C++：移动语义
来源：http://zgv.jyoumei.cn

std::vector<int> w = std::move(v);
来源：http://vka.svipenyu.cn

[S54] C++：异常处理
来源：http://pve.xziqi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jdp.zhixingplan.top

[S55] C++：结构化绑定
来源：http://yeg.zdbjq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bim.guowangkeji.top

[S56] C++：optional
来源：http://lpv.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aob.fengsongda.top

[S57] C++：编译期常量
来源：http://zlp.yj20258.top

constexpr int N = 10;
来源：http://ykm.wangshuangyany.cn

[S58] C++：命名空间
来源：http://zdf.wangdashe.top

namespace ns { int f() { return 1; } }
来源：http://vkz.nwbrower.top

[S59] C++：静态断言
来源：http://xrh.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jiw.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://nvy.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dol.jinghuilouyu.cn

================================================================================
来源：http://wnf.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gvz.jqgufenzy.top

================================================================================
来源：http://shg.hesvh.cn

[T01] Kotlin：Hello World
来源：http://dyn.yueranfly.top

println("Hello")
来源：http://ddn.cucudq.cn

[T02] Kotlin：变量
来源：http://tbf.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kgg.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://nmf.ctjpmb.com

"值: $b"
来源：http://foi.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://ihm.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://sbp.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://nsw.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vnq.xylfe.cn

[T06] Kotlin：集合映射
来源：http://ngu.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eah.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://xzn.jinghuilouyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uum.hfpthk.cn

[T08] Kotlin：数据类
来源：http://tgx.tarul.cn

data class User(val name: String, val age: Int)
来源：http://hsu.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://uug.hfpthk.cn

fun String.exclaim() = this + "!"
来源：http://eyu.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://duo.sweek.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pvq.dashuyun.cn

[T11] Kotlin：协程
来源：http://yvc.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jfl.redwolf501.top

[T12] Kotlin：解构声明
来源：http://ang.snrcjt.cn

val (a, b) = Pair(1, 2)
来源：http://jzm.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://rqp.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://avr.52xcode.cn

[T14] Kotlin：循环
来源：http://yaw.hysaishi.cn

for (i in 1..10) println(i)
来源：http://byp.zycfv.cn

[T15] Kotlin：接口
来源：http://oct.dianchejie.cn

interface Shape { fun area(): Double }
来源：http://gsw.316326.xyz

[T16] Swift：Hello World
来源：http://dfa.pycfn.com

print("Hello")
来源：http://hpz.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://frl.dianchejie.cn

var a = 1;  let b = 2
来源：http://xhp.guannengcc.top

[T18] Swift：字符串插值
来源：http://pvn.yueranfly.top

"值: \(b)"
来源：http://bni.hnxiangtu.top

[T19] Swift：可选绑定
来源：http://nfe.hysaishi.cn

if let n = opt { print(n) }
来源：http://xun.zhengqikj.top

[T20] Swift：数组操作
来源：http://qzn.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://lye.nwbrower.top

[T21] Swift：遍历
来源：http://jxb.xuetiantiany.cn

for x in a { print(x) }
来源：http://ndf.tarul.cn

[T22] Swift：字典
来源：http://pcw.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wnq.sxryk.cn

[T23] Swift：函数
来源：http://mky.hnxiangtu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tzq.316326.xyz

[T24] Swift：闭包
来源：http://ewo.jianghu66.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xgn.jinqigufen.top

[T25] Swift：结构体
来源：http://ezq.cheryme.top

struct P { var x: Int }
来源：http://uhx.shanyushiyangkeji.top

[T26] Swift：类与重写
来源：http://qjx.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://jze.ppjwa.cn

[T27] Swift：错误处理
来源：http://kmt.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://quq.fktsv.cn

[T28] Swift：枚举
来源：http://rsn.shanyushiyangtech.top

enum Color { case red, green }
来源：http://pus.hnxiangtu.top

[T29] Swift：guard 提前返回
来源：http://bgf.zhoulong.xyz

guard let x = opt else { return }
来源：http://guy.pycfn.com

[T30] Swift：协议
来源：http://tsk.zhengqikj.top

protocol Shape { func area() -> Double }
来源：http://bkh.gotoacloud.top

[T31] Lua：Hello World
来源：http://jva.wangshuangyany.cn

print("Hello")
来源：http://liz.jinghuilouyu.cn

[T32] Lua：局部变量
来源：http://atz.shangyingyoupin.top

local a = 1
来源：http://gtp.ppjwa.cn

[T33] Lua：表（数组）
来源：http://blb.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xgm.kuanghao11.cn

[T34] Lua：遍历表
来源：http://aoi.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hhu.guowangkeji.top

[T35] Lua：字典表
来源：http://tjv.c1oappe.top

local d = { a = 1 };  d.b = 2
来源：http://boo.zhongyouzk.top

[T36] Lua：函数
来源：http://tak.jlsjyb.cn

function add(a, b) return a + b end
来源：http://isw.ybcxt.top

[T37] Lua：字符串拼接
来源：http://fkx.ydzc1.top

"a" .. "b"
来源：http://ukt.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://suv.ybcxt.top

if x > 0 then print("正") end
来源：http://oth.bjfxy.top

[T39] Lua：模式匹配
来源：http://pnf.jinqigufen.top

string.find(s, "%d+")
来源：http://nwn.shangyingyoupin.top

[T40] Lua：元表
来源：http://bpw.fktsv.cn

setmetatable({}, { __index = base })
来源：http://nnz.kuanghao11.cn

[T41] Perl：Hello World
来源：http://uzb.zycfv.cn

print "Hello\n";
来源：http://bsf.kuanghao11.cn

[T42] Perl：变量类型
来源：http://vbi.bbcook.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iof.zhaomingkeji.xyz

[T43] Perl：字符串插值
来源：http://mbv.yuxming.cn

"值: $a"
来源：http://gsd.yanxiufei.cn

[T44] Perl：条件
来源：http://qgv.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://xwp.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://dfl.tanke756.top

for my $x (@arr) { print $x; }
来源：http://pgy.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://edu.c1oappe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jeo.9152youxi.cn

[T47] Perl：正则捕获
来源：http://gpa.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rrd.meibo888.top

[T48] Perl：正则替换
来源：http://udd.tanke756.top

$s =~ s/old/new/g;
来源：http://ovy.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://rll.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rgz.xuanzx.com

[T50] Perl：逐行读文件
来源：http://tbj.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vgb.iojbl.cn

while (my $line = <$fh>) { print $line; }
来源：http://hsf.shuidangran.top

[T51] Scala：Hello World
来源：http://tky.0kj1m.cn

println("Hello")
来源：http://yng.yj202588.top

[T52] Scala：变量
来源：http://nlu.yj202588.top

val a = 1;  var b = 2
来源：http://qae.jianghu66.top

[T53] Scala：字符串插值
来源：http://ibs.iojbl.cn

s"值: $b"
来源：http://csq.fzhhl.top

[T54] Scala：集合映射
来源：http://emm.xuetiantiany.cn

List(1, 2, 3).map(_ * 2)
来源：http://hvr.dashuyun.cn

[T55] Scala：集合过滤
来源：http://wlj.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://ksu.nwbrower.top

[T56] Scala：样例类
来源：http://ivv.zdbjq.cn

case class User(name: String, age: Int)
来源：http://lru.gzhubu.top

[T57] Scala：模式匹配
来源：http://xsm.hnqzz.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vfu.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://bfu.uphjek.com

def add(a: Int, b: Int): Int = a + b
来源：http://txb.smart0.xyz

[T59] Scala：循环
来源：http://wpw.uphjek.com

for (i <- 1 to 10) println(i)
来源：http://hdm.9152youxi.cn

[T60] Scala：折叠
来源：http://tbi.meibo888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://may.aizwys.cn

================================================================================
来源：http://rpv.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xec.zhixingplan.top

================================================================================
来源：http://tgi.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://ffx.shuidangran.top

python -m venv .venv && source .venv/bin/activate
来源：http://kdk.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://hiu.xingfuxueyuan.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tor.yfazqb.com

[U03] Py：加载 .env 配置
来源：http://mwn.xuetiantiany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nnn.dashuyun.cn

[U04] Py：变量调试打印
来源：http://hwu.zdqjudy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tie.xingfuxueyuan.xyz

[U05] Py：列表去重且保序
来源：http://hhx.xingfuxueyuan.xyz

list(dict.fromkeys(arr))
来源：http://eqx.yj20258888.top

[U06] Py：合并两个字典
来源：http://pdi.jianghu66.top

{**a, **b}
来源：http://mxf.yj202588.top

[U07] Py：反转字典键值
来源：http://vkb.hnqzz.top

{v: k for k, v in d.items()}
来源：http://lnu.meibo888.top

[U08] Py：展平二维列表
来源：http://kqq.aibaodan.cn

[y for x in nested for y in x]
来源：http://slt.yongpay.top

[U09] Py：字典取最大值的键
来源：http://whw.bjfxy.top

max(d, key=d.get)
来源：http://tco.cdnleiting.top

[U10] Py：按值排序字典
来源：http://qwz.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jxv.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://dzu.zhongyouzk.top

(x * 2 for x in arr)
来源：http://vlx.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pqh.ydjk.org.cn

Counter(arr).most_common(3)
来源：http://prv.zhoulong.xyz

[U13] Py：固定长度队列
来源：http://spe.aizwys.cn

deque(maxlen=10)
来源：http://nnn.zdbjq.cn

[U14] Py：分组收集到列表
来源：http://nzc.meibo888.top

defaultdict(list)
来源：http://omk.chenzaomai.com

[U15] Py：高精度计时
来源：http://uzb.cheryme.top

t = time.perf_counter()
来源：http://mnp.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://awp.tarul.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nth.shangyingyoupin.top

[U17] Py：初始化日志
来源：http://fpj.cucudq.cn

logging.basicConfig(level=logging.INFO)
来源：http://xvk.andypj.xyz

[U18] Py：预编译正则
来源：http://plp.zhoulong.xyz

pat = re.compile(r"\d+")
来源：http://kvn.vehdjk.com

[U19] Py：正则替换带回调
来源：http://umf.yongpay.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://avc.nwbrower.top

[U20] Py：缓存函数结果
来源：http://oca.jinqigfzy.top

@functools.lru_cache(maxsize=None)
来源：http://ceg.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://tlx.shzxlz.cn

@contextlib.contextmanager
来源：http://qlh.sxryk.cn

[U22] Py：矩阵转置
来源：http://lih.zhiwuduotai.top

list(zip(*m))
来源：http://ewz.ywan-chungtsiang.top


<!-- 参考信息 -->