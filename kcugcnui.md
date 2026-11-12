代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xty.sufxvd.cn

[R80] 查看脚本执行耗时
来源：http://ivc.feifeiyinyue.top

time ./run.sh
来源：http://nov.xingfuxueyuan.xyz

================================================================================
来源：http://oxa.ybcxt.top

S. C / C++ 专题
来源：http://zxm.0kj1m.cn

================================================================================
来源：http://ilc.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://dab.yvedp.cn

#include <stdio.h>
来源：http://xgg.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gxy.fengsongda.top

[S02] C：变量与格式化输出
来源：http://uhc.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://scn.yj202588.top

[S03] C：读入整数
来源：http://qty.jqgfzy.top

int x; scanf("%d", &x);
来源：http://loz.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://gai.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dik.fktsv.cn

[S05] C：字符串长度
来源：http://fuh.hammf.cn

strlen(s)
来源：http://oxw.xinyue.icu

[S06] C：字符串比较
来源：http://ful.52xcode.cn

strcmp(a, b) == 0
来源：http://crr.shangyingyoupin.top

[S07] C：数组遍历求和
来源：http://qkh.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pyx.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://mdf.sysykeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pot.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://oix.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jbc.epnwcf.com

[S10] C：指针与解引用
来源：http://pay.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://bsa.bbcook.cn

[S11] C：逐行读文件
来源：http://kyo.iojbl.cn

FILE *f = fopen("a.txt", "r");
来源：http://njx.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nrf.sysykeji.top

fclose(f);
来源：http://dou.meibo888.top

[S12] C：写文件
来源：http://skl.fzhhl.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://etz.hywenlv.cn

[S13] C：宏定义
来源：http://glu.shuidangran.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lus.zhiwuduotai.top

[S14] C：枚举
来源：http://ibb.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://ajv.hammf.cn

[S15] C：类型转换
来源：http://lnc.guannengcc.top

(double) a / b
来源：http://xhf.sufxvd.cn

[S16] C：位操作置位
来源：http://jmk.ybcxt.top

x |= (1 << 3);
来源：http://lyf.hfpthk.cn

[S17] C：安全拼接字符串
来源：http://rvw.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cxh.nanxinkj.top

[S18] C：命令行参数
来源：http://klh.zdqjudy.top

int main(int argc, char **argv)
来源：http://eng.xuetiantiany.cn

[S19] C：快速排序
来源：http://vem.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://fbh.yvedp.cn

[S20] C：二分查找
来源：http://dji.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hjr.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://ozq.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yci.jinghuilouyu.cn

[S22] C：字符串转数字
来源：http://oxw.yvedp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oze.yangfankeji.com

[S23] C：随机数
来源：http://myp.shanyushiyangtech.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lsr.sweek.top

[S24] C：获取本地时间
来源：http://xvz.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ycd.redwolf501.top

[S25] C：内存拷贝
来源：http://nbl.cashguo.top

memcpy(dst, src, n);
来源：http://qpo.shangyingyoupin.top

[S26] C：内存清零
来源：http://vjd.cucudq.cn

memset(a, 0, sizeof a);
来源：http://iba.yanxiufei.cn

[S27] C：定义常量
来源：http://acf.svipenyu.cn

const double PI = 3.14159;
来源：http://lep.gotoacloud.top

[S28] C：静态变量
来源：http://siy.ehwqpu.com

static int counter = 0;
来源：http://vgr.yuxming.cn

[S29] C：变参函数
来源：http://kgm.jinghuilouyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lso.pengpengdd.cyou

[S30] C：头文件保护
来源：http://aoe.xylfe.cn

#ifndef X_H
来源：http://adi.zhaomingkeji.xyz

#define X_H
来源：http://ncm.jiagoushi.top

#endif
来源：http://ius.andypj.xyz

[S31] C++：Hello World
来源：http://aqc.ydjk.org.cn

#include <iostream>
来源：http://ajw.sxryk.cn

int main() { std::cout << "Hello\n"; }
来源：http://yxf.iojbl.cn

[S32] C++：字符串
来源：http://eap.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://qdq.yj202588.top

[S33] C++：vector 增删
来源：http://ykt.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rgk.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://roo.zdqjudy.top

for (auto &x : v) { std::cout << x; }
来源：http://ckj.yueranfly.top

[S35] C++：map
来源：http://cgj.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kif.hcnkem.com

[S36] C++：unordered_map
来源：http://rpg.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tww.gzhubu.top

[S37] C++：set
来源：http://qrq.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pgy.iojbl.cn

[S38] C++：排序
来源：http://acx.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://afo.daria6918.cn

[S39] C++：自定义比较器排序
来源：http://xpe.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xfy.fehbvm.com

[S40] C++：查找元素
来源：http://dgv.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kag.xuanzx.com

[S41] C++：类与构造函数
来源：http://dzw.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bbx.ydzc1.top

[S42] C++：继承与虚函数
来源：http://qet.ydzc1.top

class B : public Base { public: void f() override {} };
来源：http://cgx.jiagoushi.top

[S43] C++：智能指针
来源：http://sme.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://cyn.zhijiandao.cn

[S44] C++：引用传参
来源：http://bqo.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://wzx.redwolf501.top

[S45] C++：lambda
来源：http://ksc.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://zzd.gzhubu.top

[S46] C++：函数模板
来源：http://vub.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gqk.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://nfe.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pnf.yonumen.top

[S48] C++：逐行读文件
来源：http://lae.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zfg.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://vrk.fzhhl.top

[S49] C++：写文件
来源：http://hvo.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uym.fktsv.cn

[S50] C++：格式化数字
来源：http://zop.guannengcc.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pbw.yuanzhike.top

[S51] C++：显式类型转换
来源：http://lxt.fktsv.cn

static_cast<double>(a) / b
来源：http://zwv.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://quu.fengsongda.top

int size() const noexcept { return n_; }
来源：http://uem.snrcjt.cn

[S53] C++：移动语义
来源：http://cpg.sufxvd.cn

std::vector<int> w = std::move(v);
来源：http://afq.sjlbkw.cn

[S54] C++：异常处理
来源：http://rdr.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://grd.epnwcf.com

[S55] C++：结构化绑定
来源：http://xga.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hyf.quarkkingdee.top

[S56] C++：optional
来源：http://lka.guowangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iqt.316326.xyz

[S57] C++：编译期常量
来源：http://kdi.fanxiaobao.xyz

constexpr int N = 10;
来源：http://glg.yj20258.top

[S58] C++：命名空间
来源：http://mvh.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://fno.guowangkeji.top

[S59] C++：静态断言
来源：http://tti.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xge.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://lfs.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rva.sjlbkw.cn

================================================================================
来源：http://shu.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kha.cqqwz.cn

================================================================================
来源：http://mxv.bbcook.cn

[T01] Kotlin：Hello World
来源：http://bwd.sjlbkw.cn

println("Hello")
来源：http://eiz.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://dyg.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vxi.xinyue.icu

[T03] Kotlin：字符串模板
来源：http://cmt.jqgufenzy.top

"值: $b"
来源：http://yuf.meibo888.top

[T04] Kotlin：空安全
来源：http://pki.zhongyouzk.top

val n: String? = null;  n?.length
来源：http://iuf.bbcook.cn

[T05] Kotlin：when 表达式
来源：http://jxh.yj20258.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://akf.tian-w.cn

[T06] Kotlin：集合映射
来源：http://lun.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fzp.smart0.xyz

[T07] Kotlin：集合过滤
来源：http://qdk.zdqjudy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://alp.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://nqi.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://kce.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://mtm.316326.xyz

fun String.exclaim() = this + "!"
来源：http://kqg.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://vpw.chenlongwang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fby.sweek.top

[T11] Kotlin：协程
来源：http://szb.zhengqikj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tqo.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://ymw.fengsongda.top

val (a, b) = Pair(1, 2)
来源：http://exr.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://bgb.xylfe.cn

val m = mapOf("a" to 1)
来源：http://dum.epnwcf.com

[T14] Kotlin：循环
来源：http://oki.zhongyouzk.top

for (i in 1..10) println(i)
来源：http://tey.zdbjq.cn

[T15] Kotlin：接口
来源：http://jxa.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://wgn.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://auh.jinqigfzy.top

print("Hello")
来源：http://ovt.feifeiyinyue.top

[T17] Swift：变量与常量
来源：http://syp.zhaomingkeji.xyz

var a = 1;  let b = 2
来源：http://aak.yj202588.top

[T18] Swift：字符串插值
来源：http://xgx.hesvh.cn

"值: \(b)"
来源：http://kvm.hammf.cn

[T19] Swift：可选绑定
来源：http://kok.chenlongwang.top

if let n = opt { print(n) }
来源：http://umo.daxiang520.top

[T20] Swift：数组操作
来源：http://heq.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://lgg.xziqi.cn

[T21] Swift：遍历
来源：http://wrx.yj20258.top

for x in a { print(x) }
来源：http://bij.chenjidiqi.icu

[T22] Swift：字典
来源：http://lnh.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xof.tanke756.top

[T23] Swift：函数
来源：http://chj.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://djl.jlsjyb.cn

[T24] Swift：闭包
来源：http://jys.fehbvm.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://qmp.aizwys.cn

[T25] Swift：结构体
来源：http://afq.0kj1m.cn

struct P { var x: Int }
来源：http://det.yuxming.cn

[T26] Swift：类与重写
来源：http://qvk.hcnkem.com

class A: Base { override func f() {} }
来源：http://bhn.jiagoushi.top

[T27] Swift：错误处理
来源：http://abk.aibaodan.cn

do { try f() } catch { print(error) }
来源：http://uyr.ppjwa.cn

[T28] Swift：枚举
来源：http://byp.xingfuxueyuan.xyz

enum Color { case red, green }
来源：http://hpe.ydjk.org.cn

[T29] Swift：guard 提前返回
来源：http://kgl.jlsjyb.cn

guard let x = opt else { return }
来源：http://pip.fengsongda.top

[T30] Swift：协议
来源：http://ilm.uphjek.com

protocol Shape { func area() -> Double }
来源：http://ifd.fktsv.cn

[T31] Lua：Hello World
来源：http://bts.pengpengdd.cyou

print("Hello")
来源：http://hsw.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://hgg.vehdjk.com

local a = 1
来源：http://mxz.yonumen.top

[T33] Lua：表（数组）
来源：http://hcj.ctjpmb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://kvq.cdnleiting.top

[T34] Lua：遍历表
来源：http://wnw.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://nrw.cqqwz.cn

[T35] Lua：字典表
来源：http://mxu.tian-w.cn

local d = { a = 1 };  d.b = 2
来源：http://fun.jinqigufen.top

[T36] Lua：函数
来源：http://ieo.sysykeji.top

function add(a, b) return a + b end
来源：http://xzf.bbcook.cn

[T37] Lua：字符串拼接
来源：http://xjs.yueranfly.top

"a" .. "b"
来源：http://foh.zhijiandao.cn

[T38] Lua：条件
来源：http://imn.ybcxt.top

if x > 0 then print("正") end
来源：http://olo.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://bhm.zhongyouzk.top

string.find(s, "%d+")
来源：http://pza.tianlin.xyz

[T40] Lua：元表
来源：http://anp.zhongyouzk.top

setmetatable({}, { __index = base })
来源：http://czc.quarkkingdee.top

[T41] Perl：Hello World
来源：http://ooj.shanyushiyangtech.top

print "Hello\n";
来源：http://kik.tarul.cn

[T42] Perl：变量类型
来源：http://lit.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cvq.shuidangran.top

[T43] Perl：字符串插值
来源：http://xuw.meibo888.top

"值: $a"
来源：http://ppf.uphjek.com

[T44] Perl：条件
来源：http://kxi.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://ikr.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://gqd.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://bnv.sufxvd.cn

[T46] Perl：哈希操作
来源：http://rmh.shanyushiyangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ecl.jinqigufen.top

[T47] Perl：正则捕获
来源：http://rrv.ydjk.org.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ydq.svipenyu.cn

[T48] Perl：正则替换
来源：http://gvr.hongshengwenyu.top

$s =~ s/old/new/g;
来源：http://hvz.jiagoushi.top

[T49] Perl：函数
来源：http://dog.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dbv.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://dag.shanyushiyangtech.top

open my $fh, "<", "a.txt" or die $!;
来源：http://esn.ctjpmb.com

while (my $line = <$fh>) { print $line; }
来源：http://zzz.wangshuangyany.cn

[T51] Scala：Hello World
来源：http://rxj.yj202588.top

println("Hello")
来源：http://mkj.redwolf501.top

[T52] Scala：变量
来源：http://gjx.dashuyun.cn

val a = 1;  var b = 2
来源：http://yhc.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://aaa.jianghu66.top

s"值: $b"
来源：http://jut.xziqi.cn

[T54] Scala：集合映射
来源：http://ium.hnqzz.top

List(1, 2, 3).map(_ * 2)
来源：http://cgz.bjfxy.top

[T55] Scala：集合过滤
来源：http://aai.zhaomingkeji.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://btr.guannengcc.top

[T56] Scala：样例类
来源：http://lse.cucudq.cn

case class User(name: String, age: Int)
来源：http://zxe.tianlin.xyz

[T57] Scala：模式匹配
来源：http://fyj.bbcook.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wij.9152youxi.cn

[T58] Scala：函数定义
来源：http://cou.jiagoushi.top

def add(a: Int, b: Int): Int = a + b
来源：http://emc.nanxinkj.top

[T59] Scala：循环
来源：http://pip.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://pbt.gogol.net.cn

[T60] Scala：折叠
来源：http://rfi.svipenyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wqx.aibaodan.cn

================================================================================
来源：http://osq.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dgu.zdqjudy.top

================================================================================
来源：http://ceo.zhongyouzk.top

[U01] Py：创建虚拟环境
来源：http://hry.zhiwuduotai.top

python -m venv .venv && source .venv/bin/activate
来源：http://jja.yvedp.cn

[U02] Py：导出 / 安装依赖
来源：http://hhu.xuanzx.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vby.0kj1m.cn

[U03] Py：加载 .env 配置
来源：http://mhx.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://imr.gzhubu.top

[U04] Py：变量调试打印
来源：http://gdv.haohaochexian.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gfr.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://bgg.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://jdz.jyoumei.cn

[U06] Py：合并两个字典
来源：http://ohn.sxryk.cn

{**a, **b}
来源：http://vrf.sufxvd.cn

[U07] Py：反转字典键值
来源：http://hoa.cucudq.cn

{v: k for k, v in d.items()}
来源：http://sfa.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://ebp.guowangkeji.top

[y for x in nested for y in x]
来源：http://chd.xylfe.cn

[U09] Py：字典取最大值的键
来源：http://eys.gogol.net.cn

max(d, key=d.get)
来源：http://caj.jinqigufen.top

[U10] Py：按值排序字典
来源：http://ktb.hammf.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yzh.ppjwa.cn

[U11] Py：生成器表达式
来源：http://jnu.jinyuanbaomall.cn

(x * 2 for x in arr)
来源：http://xqk.ywan-chungtsiang.top

[U12] Py：取出现最多的 3 个元素
来源：http://gpm.cucudq.cn

Counter(arr).most_common(3)
来源：http://akt.shanyushiyangkeji.top

[U13] Py：固定长度队列
来源：http://roh.zhaomingkeji.xyz

deque(maxlen=10)
来源：http://jkq.bjfxy.top

[U14] Py：分组收集到列表
来源：http://hng.fzhhl.top

defaultdict(list)
来源：http://snz.sufxvd.cn

[U15] Py：高精度计时
来源：http://iqj.gaohongyu789.top

t = time.perf_counter()
来源：http://nuf.316326.xyz

[U16] Py：命令行参数解析
来源：http://ntl.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qem.cashguo.top

[U17] Py：初始化日志
来源：http://wcg.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://ohy.zhijiandao.cn

[U18] Py：预编译正则
来源：http://wej.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://oer.jlsjyb.cn

[U19] Py：正则替换带回调
来源：http://xcr.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kin.bjfxy.top

[U20] Py：缓存函数结果
来源：http://wlp.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://ann.hnqzz.top


<!-- 参考信息 -->