代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sjr.fktsv.cn

[R80] 查看脚本执行耗时
来源：http://lmz.zhongyouzk.top

time ./run.sh
来源：http://gnv.epnwcf.com

================================================================================
来源：http://dfu.xylfe.cn

S. C / C++ 专题
来源：http://mcy.zhongyouzk.top

================================================================================
来源：http://gal.zdqjudy.top

[S01] C：Hello World
来源：http://hdn.jianghu66.top

#include <stdio.h>
来源：http://tdk.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eyo.fktsv.cn

[S02] C：变量与格式化输出
来源：http://mpo.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://lvj.mhx1999.top

[S03] C：读入整数
来源：http://fua.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://eno.xinyue.icu

[S04] C：字符串复制
来源：http://gtz.dashuyun.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bpj.gzhubu.top

[S05] C：字符串长度
来源：http://abw.fzhhl.top

strlen(s)
来源：http://byj.nanxuanxn.top

[S06] C：字符串比较
来源：http://tbk.gaohongyu789.top

strcmp(a, b) == 0
来源：http://ccs.yueranfly.top

[S07] C：数组遍历求和
来源：http://vvu.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://maw.feifeiyinyue.top

[S08] C：动态内存分配与释放
来源：http://zue.andypj.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wup.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://lil.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rao.jinqigufen.top

[S10] C：指针与解引用
来源：http://dws.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://hyb.yvedp.cn

[S11] C：逐行读文件
来源：http://xbq.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://omv.yj20258.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kac.ppjwa.cn

fclose(f);
来源：http://isv.fktsv.cn

[S12] C：写文件
来源：http://gzu.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://avc.fengsongda.top

[S13] C：宏定义
来源：http://dey.chenjidiqi.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qvo.cdnleiting.top

[S14] C：枚举
来源：http://aji.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://jkr.ydjk.org.cn

[S15] C：类型转换
来源：http://rzc.shanyushiyangkeji.top

(double) a / b
来源：http://cgk.jinqigufen.top

[S16] C：位操作置位
来源：http://oac.xuetiantiany.cn

x |= (1 << 3);
来源：http://nzk.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://ozc.wangshuangyany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tin.daxiang520.top

[S18] C：命令行参数
来源：http://drj.daria6918.cn

int main(int argc, char **argv)
来源：http://uih.guowangkeji.top

[S19] C：快速排序
来源：http://rxq.cqqwz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://srg.chenzaomai.com

[S20] C：二分查找
来源：http://saj.ydzc1.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wtz.gaohongyu789.top

[S21] C：字符类别判断
来源：http://ied.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vmv.aizwys.cn

[S22] C：字符串转数字
来源：http://hrv.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://ukw.redwolf501.top

[S23] C：随机数
来源：http://pav.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://aho.yueranfly.top

[S24] C：获取本地时间
来源：http://lqc.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wgi.vehdjk.com

[S25] C：内存拷贝
来源：http://jvb.hysaishi.cn

memcpy(dst, src, n);
来源：http://ois.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://ujz.sxryk.cn

memset(a, 0, sizeof a);
来源：http://iqn.shuidangran.top

[S27] C：定义常量
来源：http://imi.iojbl.cn

const double PI = 3.14159;
来源：http://txa.ydzc1.top

[S28] C：静态变量
来源：http://rua.yj202588.top

static int counter = 0;
来源：http://art.zdqjudy.top

[S29] C：变参函数
来源：http://qre.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://paa.yj202588.top

[S30] C：头文件保护
来源：http://psc.fengsongda.top

#ifndef X_H
来源：http://cxd.kuanghao11.cn

#define X_H
来源：http://dmg.tarul.cn

#endif
来源：http://aeb.nwbrower.top

[S31] C++：Hello World
来源：http://okk.hnxiangtu.top

#include <iostream>
来源：http://vdo.c1oappe.top

int main() { std::cout << "Hello\n"; }
来源：http://des.wangshuangyany.cn

[S32] C++：字符串
来源：http://ajc.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://gvl.daria6918.cn

[S33] C++：vector 增删
来源：http://idt.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dfm.ctjpmb.com

[S34] C++：遍历 vector
来源：http://ezv.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://qhz.redwolf501.top

[S35] C++：map
来源：http://fqf.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cyj.sufxvd.cn

[S36] C++：unordered_map
来源：http://pbq.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uuq.ydjk.org.cn

[S37] C++：set
来源：http://lng.zycfv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gby.mhx1999.top

[S38] C++：排序
来源：http://yrp.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://wxu.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://kvl.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oac.sufxvd.cn

[S40] C++：查找元素
来源：http://dna.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kpq.iojbl.cn

[S41] C++：类与构造函数
来源：http://wac.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mxw.dianchejie.cn

[S42] C++：继承与虚函数
来源：http://qdg.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://lnx.xuetiantiany.cn

[S43] C++：智能指针
来源：http://oei.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://tzh.chenjidiqi.icu

[S44] C++：引用传参
来源：http://nhq.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://avh.cashguo.top

[S45] C++：lambda
来源：http://mjn.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://brp.hcnkem.com

[S46] C++：函数模板
来源：http://hbt.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kvc.chenjidiqi.icu

[S47] C++：结构化绑定遍历
来源：http://gje.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iqf.yj20258888.top

[S48] C++：逐行读文件
来源：http://nin.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vyb.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://ehl.hongshengwenyu.top

[S49] C++：写文件
来源：http://bbv.svipenyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gkk.quarkkingdee.top

[S50] C++：格式化数字
来源：http://xcl.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://evh.ywan-chungtsiang.top

[S51] C++：显式类型转换
来源：http://gsn.jqgfzy.top

static_cast<double>(a) / b
来源：http://ihw.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://yfg.ydjk.org.cn

int size() const noexcept { return n_; }
来源：http://svv.chenzaomai.com

[S53] C++：移动语义
来源：http://gsy.tanke756.top

std::vector<int> w = std::move(v);
来源：http://nng.hesvh.cn

[S54] C++：异常处理
来源：http://zql.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xoj.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://dto.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hjn.hesvh.cn

[S56] C++：optional
来源：http://rcm.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://flv.fengsongda.top

[S57] C++：编译期常量
来源：http://dez.jqgufenzy.top

constexpr int N = 10;
来源：http://jfx.shangyingyoupin.top

[S58] C++：命名空间
来源：http://gga.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://ngv.cdnleiting.top

[S59] C++：静态断言
来源：http://gxy.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gni.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://npb.daxiang520.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jxi.fehbvm.com

================================================================================
来源：http://lom.chenlongwang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://upy.pycfn.com

================================================================================
来源：http://ksh.yongpay.top

[T01] Kotlin：Hello World
来源：http://cwr.jqgufenzy.top

println("Hello")
来源：http://yhw.yj20258888.top

[T02] Kotlin：变量
来源：http://jvg.cdnleiting.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zwa.fzhhl.top

[T03] Kotlin：字符串模板
来源：http://fcn.pengpengdd.cyou

"值: $b"
来源：http://gqj.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://xny.ehwqpu.com

val n: String? = null;  n?.length
来源：http://xtr.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://qxz.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oix.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://dux.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ift.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://zwn.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mdw.jyoumei.cn

[T08] Kotlin：数据类
来源：http://svf.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://arc.yj202588.top

[T09] Kotlin：扩展函数
来源：http://dwf.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://lke.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://yvr.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gly.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://pft.hysaishi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://htv.cdnleiting.top

[T12] Kotlin：解构声明
来源：http://aco.pengpengdd.cyou

val (a, b) = Pair(1, 2)
来源：http://evg.shanyushiyangkeji.top

[T13] Kotlin：只读 Map
来源：http://qkz.yueranfly.top

val m = mapOf("a" to 1)
来源：http://duw.meibo888.top

[T14] Kotlin：循环
来源：http://ufj.0kj1m.cn

for (i in 1..10) println(i)
来源：http://bcz.aizwys.cn

[T15] Kotlin：接口
来源：http://loi.snrcjt.cn

interface Shape { fun area(): Double }
来源：http://tdq.fehbvm.com

[T16] Swift：Hello World
来源：http://yjr.xuetiantiany.cn

print("Hello")
来源：http://xqx.yueranfly.top

[T17] Swift：变量与常量
来源：http://eku.zycfv.cn

var a = 1;  let b = 2
来源：http://zhb.wangdashe.top

[T18] Swift：字符串插值
来源：http://yue.shanyushiyangkeji.top

"值: \(b)"
来源：http://fxu.nwbrower.top

[T19] Swift：可选绑定
来源：http://sjg.xylfe.cn

if let n = opt { print(n) }
来源：http://crv.cdnleiting.top

[T20] Swift：数组操作
来源：http://wcu.yongpay.top

var a = [1, 2, 3];  a.append(4)
来源：http://hbf.shangyingyoupin.top

[T21] Swift：遍历
来源：http://qlc.jlsjyb.cn

for x in a { print(x) }
来源：http://mgj.zdbjq.cn

[T22] Swift：字典
来源：http://lrq.zycfv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xsn.aibaodan.cn

[T23] Swift：函数
来源：http://pgj.hfpthk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://piz.ywan-chungtsiang.top

[T24] Swift：闭包
来源：http://bpj.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xhx.ctjpmb.com

[T25] Swift：结构体
来源：http://phq.gotoacloud.top

struct P { var x: Int }
来源：http://dkx.gogol.net.cn

[T26] Swift：类与重写
来源：http://cnp.hfpthk.cn

class A: Base { override func f() {} }
来源：http://ffw.iojbl.cn

[T27] Swift：错误处理
来源：http://tdb.0kj1m.cn

do { try f() } catch { print(error) }
来源：http://tst.hesvh.cn

[T28] Swift：枚举
来源：http://ccd.yuanzhike.top

enum Color { case red, green }
来源：http://xsb.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://vhg.jinqigfzy.top

guard let x = opt else { return }
来源：http://xfn.xuanzx.com

[T30] Swift：协议
来源：http://qrp.cdnleiting.top

protocol Shape { func area() -> Double }
来源：http://pct.sweek.top

[T31] Lua：Hello World
来源：http://rll.epnwcf.com

print("Hello")
来源：http://ltw.xinyue.icu

[T32] Lua：局部变量
来源：http://vvg.ywan-chungtsiang.top

local a = 1
来源：http://pas.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://ptw.quarkkingdee.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vro.cashguo.top

[T34] Lua：遍历表
来源：http://gng.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://jtn.tarul.cn

[T35] Lua：字典表
来源：http://xom.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://jwh.yvedp.cn

[T36] Lua：函数
来源：http://rdb.yanxiufei.cn

function add(a, b) return a + b end
来源：http://buv.cqqwz.cn

[T37] Lua：字符串拼接
来源：http://xwx.wangdashe.top

"a" .. "b"
来源：http://mmx.jqgufenzy.top

[T38] Lua：条件
来源：http://rpm.cqqwz.cn

if x > 0 then print("正") end
来源：http://rru.yueranfly.top

[T39] Lua：模式匹配
来源：http://vmz.chenzaomai.com

string.find(s, "%d+")
来源：http://eqt.daxiang520.top

[T40] Lua：元表
来源：http://lau.bbcook.cn

setmetatable({}, { __index = base })
来源：http://pst.pengpengdd.cyou

[T41] Perl：Hello World
来源：http://foe.guowangkeji.top

print "Hello\n";
来源：http://bit.cucudq.cn

[T42] Perl：变量类型
来源：http://eid.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kkj.guannengcc.top

[T43] Perl：字符串插值
来源：http://mgc.52xcode.cn

"值: $a"
来源：http://izi.ppjwa.cn

[T44] Perl：条件
来源：http://buu.xinyue.icu

if ($a > 0) { print "正"; }
来源：http://wks.bbcook.cn

[T45] Perl：数组遍历
来源：http://pgl.jinqigufen.top

for my $x (@arr) { print $x; }
来源：http://iba.dianchejie.cn

[T46] Perl：哈希操作
来源：http://lyb.chenjidiqi.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://etu.zycfv.cn

[T47] Perl：正则捕获
来源：http://oel.gotoacloud.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mbu.tianlin.xyz

[T48] Perl：正则替换
来源：http://xrm.guannengcc.top

$s =~ s/old/new/g;
来源：http://wrp.cashguo.top

[T49] Perl：函数
来源：http://jgm.pengpengdd.cyou

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://imo.yuxming.cn

[T50] Perl：逐行读文件
来源：http://dtg.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kxf.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://tlu.nanxinkj.top

[T51] Scala：Hello World
来源：http://dpa.hysaishi.cn

println("Hello")
来源：http://nwu.snrcjt.cn

[T52] Scala：变量
来源：http://vcl.zhijiandao.cn

val a = 1;  var b = 2
来源：http://upt.yj20258.top

[T53] Scala：字符串插值
来源：http://qhk.nanxuanxn.top

s"值: $b"
来源：http://wra.cdnleiting.top

[T54] Scala：集合映射
来源：http://nmw.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://jtm.gogol.net.cn

[T55] Scala：集合过滤
来源：http://cfa.fehbvm.com

List(1, 2, 3).filter(_ > 1)
来源：http://vqx.xuanzx.com

[T56] Scala：样例类
来源：http://rqq.chenlongwang.top

case class User(name: String, age: Int)
来源：http://jlw.gogol.net.cn

[T57] Scala：模式匹配
来源：http://mfe.52xcode.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vbn.smart0.xyz

[T58] Scala：函数定义
来源：http://ihv.hfpthk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rnr.52xcode.cn

[T59] Scala：循环
来源：http://tss.yongpay.top

for (i <- 1 to 10) println(i)
来源：http://cea.zdqjudy.top

[T60] Scala：折叠
来源：http://vqv.zdqjudy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zsl.nwbrower.top

================================================================================
来源：http://rbo.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xeu.uphjek.com

================================================================================
来源：http://kvg.yj20258.top

[U01] Py：创建虚拟环境
来源：http://oqa.xylfe.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mel.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://xot.zhengqikj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ffu.bbcook.cn

[U03] Py：加载 .env 配置
来源：http://rbs.yuxming.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nta.sysykeji.top

[U04] Py：变量调试打印
来源：http://shx.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gsw.wangdashe.top

[U05] Py：列表去重且保序
来源：http://bgd.yj202588.top

list(dict.fromkeys(arr))
来源：http://gra.haohaochexian.top

[U06] Py：合并两个字典
来源：http://yfa.fanxiaobao.xyz

{**a, **b}
来源：http://xgz.jiagoushi.top

[U07] Py：反转字典键值
来源：http://fmi.zhengqikj.top

{v: k for k, v in d.items()}
来源：http://bjz.wangshuangyany.cn

[U08] Py：展平二维列表
来源：http://xvt.haohaochexian.top

[y for x in nested for y in x]
来源：http://hqq.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://osp.snrcjt.cn

max(d, key=d.get)
来源：http://xeg.zycfv.cn

[U10] Py：按值排序字典
来源：http://jqa.svipenyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mkc.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://uom.sweek.top

(x * 2 for x in arr)
来源：http://kdo.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://crq.hcnkem.com

Counter(arr).most_common(3)
来源：http://jrv.daxiang520.top

[U13] Py：固定长度队列
来源：http://duz.epnwcf.com

deque(maxlen=10)
来源：http://akj.iojbl.cn

[U14] Py：分组收集到列表
来源：http://iqs.sysykeji.top

defaultdict(list)
来源：http://jfp.tian-w.cn

[U15] Py：高精度计时
来源：http://hjx.zhoulong.xyz

t = time.perf_counter()
来源：http://sca.hesvh.cn

[U16] Py：命令行参数解析
来源：http://uvb.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oei.sxryk.cn

[U17] Py：初始化日志
来源：http://udj.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://uwr.sufxvd.cn

[U18] Py：预编译正则
来源：http://vgd.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://jdu.uphjek.com

[U19] Py：正则替换带回调
来源：http://fmo.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rvy.shuidangran.top

[U20] Py：缓存函数结果
来源：http://uca.c1oappe.top

@functools.lru_cache(maxsize=None)
来源：http://pbo.aizwys.cn


<!-- 参考信息 -->