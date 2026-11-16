代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ejo.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://okx.cheryme.top

time ./run.sh
来源：http://aop.hysaishi.cn

================================================================================
来源：http://rah.dashuyun.cn

S. C / C++ 专题
来源：http://uai.fktsv.cn

================================================================================
来源：http://pvv.tian-w.cn

[S01] C：Hello World
来源：http://ftg.yj202588.top

#include <stdio.h>
来源：http://orw.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://etm.ivvv.top

[S02] C：变量与格式化输出
来源：http://niz.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://fhd.mhx1999.top

[S03] C：读入整数
来源：http://khb.daria6918.cn

int x; scanf("%d", &x);
来源：http://eek.svipenyu.cn

[S04] C：字符串复制
来源：http://jsw.ywan-chungtsiang.top

char dst[32]; strcpy(dst, "hi");
来源：http://aan.fzhhl.top

[S05] C：字符串长度
来源：http://clv.haohaochexian.top

strlen(s)
来源：http://enj.kuanghao11.cn

[S06] C：字符串比较
来源：http://hwv.havefunace.top

strcmp(a, b) == 0
来源：http://fyd.fktsv.cn

[S07] C：数组遍历求和
来源：http://ukw.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yip.haohaochexian.top

[S08] C：动态内存分配与释放
来源：http://juz.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://isq.316326.xyz

[S09] C：结构体定义与初始化
来源：http://mlt.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wna.bjfxy.top

[S10] C：指针与解引用
来源：http://qjo.bbcook.cn

int *p = &a;  *p = 5;
来源：http://wnr.zhengqikj.top

[S11] C：逐行读文件
来源：http://wbf.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://jrd.shanyushiyangtech.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jsa.zdbjq.cn

fclose(f);
来源：http://pkt.jqgfzy.top

[S12] C：写文件
来源：http://fet.sysykeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ist.sufxvd.cn

[S13] C：宏定义
来源：http://gyf.jqgfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pxp.zhengqikj.top

[S14] C：枚举
来源：http://ozd.52xcode.cn

enum Color { RED, GREEN, BLUE };
来源：http://fnv.snrcjt.cn

[S15] C：类型转换
来源：http://xff.sufxvd.cn

(double) a / b
来源：http://isc.hywenlv.cn

[S16] C：位操作置位
来源：http://dis.redwolf501.top

x |= (1 << 3);
来源：http://upm.fktsv.cn

[S17] C：安全拼接字符串
来源：http://wyo.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cdm.ybcxt.top

[S18] C：命令行参数
来源：http://agg.svipenyu.cn

int main(int argc, char **argv)
来源：http://ouh.zhijiandao.cn

[S19] C：快速排序
来源：http://qwr.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://fcl.xylfe.cn

[S20] C：二分查找
来源：http://jpz.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zrt.redwolf501.top

[S21] C：字符类别判断
来源：http://jxu.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://btg.chenzaomai.com

[S22] C：字符串转数字
来源：http://uis.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://yyo.ehwqpu.com

[S23] C：随机数
来源：http://cle.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rfl.chenjidiqi.icu

[S24] C：获取本地时间
来源：http://jfu.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://plf.jianghu66.top

[S25] C：内存拷贝
来源：http://zic.cdnleiting.top

memcpy(dst, src, n);
来源：http://vaa.9152youxi.cn

[S26] C：内存清零
来源：http://ezy.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://jkd.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://lzr.jqgufenzy.top

const double PI = 3.14159;
来源：http://lgf.bbcook.cn

[S28] C：静态变量
来源：http://sni.jinqigfzy.top

static int counter = 0;
来源：http://are.hnxiangtu.top

[S29] C：变参函数
来源：http://irg.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zeq.sysykeji.top

[S30] C：头文件保护
来源：http://mqv.sufxvd.cn

#ifndef X_H
来源：http://jab.pycfn.com

#define X_H
来源：http://wtd.ppjwa.cn

#endif
来源：http://obt.epnwcf.com

[S31] C++：Hello World
来源：http://yqf.tanke756.top

#include <iostream>
来源：http://soh.pycfn.com

int main() { std::cout << "Hello\n"; }
来源：http://whz.hysaishi.cn

[S32] C++：字符串
来源：http://lwc.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://zyb.wangdashe.top

[S33] C++：vector 增删
来源：http://byp.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://shm.hfpthk.cn

[S34] C++：遍历 vector
来源：http://ydr.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://nnm.fanxiaobao.xyz

[S35] C++：map
来源：http://vxn.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://shl.fzhhl.top

[S36] C++：unordered_map
来源：http://gqh.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lzj.cashguo.top

[S37] C++：set
来源：http://wjg.ctjpmb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://diw.ppjwa.cn

[S38] C++：排序
来源：http://vrf.zdbjq.cn

std::sort(v.begin(), v.end());
来源：http://efi.yongpay.top

[S39] C++：自定义比较器排序
来源：http://oih.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ior.jqgfzy.top

[S40] C++：查找元素
来源：http://phb.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wxi.hnxiangtu.top

[S41] C++：类与构造函数
来源：http://qbj.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://opw.havefunace.top

[S42] C++：继承与虚函数
来源：http://qyq.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://ccw.feifeiyinyue.top

[S43] C++：智能指针
来源：http://mzh.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://vfq.fehbvm.com

[S44] C++：引用传参
来源：http://zuj.c1oappe.top

void inc(int &x) { ++x; }
来源：http://ema.sysykeji.top

[S45] C++：lambda
来源：http://syl.zhongyouzk.top

auto add = [](int a, int b) { return a + b; };
来源：http://xzt.zycfv.cn

[S46] C++：函数模板
来源：http://rfi.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hdm.fanxiaobao.xyz

[S47] C++：结构化绑定遍历
来源：http://auq.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://paw.9152youxi.cn

[S48] C++：逐行读文件
来源：http://ecn.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://jfx.yj20258888.top

while (std::getline(in, line)) { }
来源：http://qsd.hysaishi.cn

[S49] C++：写文件
来源：http://xum.feifeiyinyue.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mbh.daxiang520.top

[S50] C++：格式化数字
来源：http://obg.ydzc1.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mir.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://jeh.hysaishi.cn

static_cast<double>(a) / b
来源：http://jyr.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://ufg.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://aan.aibaodan.cn

[S53] C++：移动语义
来源：http://xhy.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://kcl.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://zwj.shanyushiyangtech.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gda.aibaodan.cn

[S55] C++：结构化绑定
来源：http://csj.yonumen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rva.hesvh.cn

[S56] C++：optional
来源：http://yoq.ybcxt.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iwi.hesvh.cn

[S57] C++：编译期常量
来源：http://mdo.nanxuanxn.top

constexpr int N = 10;
来源：http://ylo.cqqwz.cn

[S58] C++：命名空间
来源：http://eut.quarkkingdee.top

namespace ns { int f() { return 1; } }
来源：http://qdp.yj20258.top

[S59] C++：静态断言
来源：http://equ.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dvf.shzxlz.cn

[S60] C++：遍历并删除元素
来源：http://bew.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://svy.chenlongwang.top

================================================================================
来源：http://zpz.birdmap.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fos.ppjwa.cn

================================================================================
来源：http://caj.hammf.cn

[T01] Kotlin：Hello World
来源：http://dvl.chenjidiqi.icu

println("Hello")
来源：http://nyw.hesvh.cn

[T02] Kotlin：变量
来源：http://sgz.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dym.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://yoe.tanke756.top

"值: $b"
来源：http://sca.aizwys.cn

[T04] Kotlin：空安全
来源：http://rwp.316326.xyz

val n: String? = null;  n?.length
来源：http://bkz.yongpay.top

[T05] Kotlin：when 表达式
来源：http://jfx.zhongyouzk.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yws.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://vyz.vehdjk.com

listOf(1, 2, 3).map { it * 2 }
来源：http://pwe.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://vvq.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://auy.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://fem.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://orw.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://kgl.gzhubu.top

fun String.exclaim() = this + "!"
来源：http://low.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://ojb.yongpay.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qms.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://kml.uphjek.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://qsb.hongshengwenyu.top

[T12] Kotlin：解构声明
来源：http://tan.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://fmr.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://ytq.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://prc.ywan-chungtsiang.top

[T14] Kotlin：循环
来源：http://trz.yj20258888.top

for (i in 1..10) println(i)
来源：http://ifp.gaohongyu789.top

[T15] Kotlin：接口
来源：http://abh.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://xnm.zhengqikj.top

[T16] Swift：Hello World
来源：http://yhl.xziqi.cn

print("Hello")
来源：http://pnh.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://rij.jianghu66.top

var a = 1;  let b = 2
来源：http://uqm.ivvv.top

[T18] Swift：字符串插值
来源：http://vzt.haohaochexian.top

"值: \(b)"
来源：http://oji.xingfuxueyuan.xyz

[T19] Swift：可选绑定
来源：http://ndy.zdqjudy.top

if let n = opt { print(n) }
来源：http://mml.cheryme.top

[T20] Swift：数组操作
来源：http://skd.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nmd.svipenyu.cn

[T21] Swift：遍历
来源：http://ung.ydzc1.top

for x in a { print(x) }
来源：http://gxt.hcnkem.com

[T22] Swift：字典
来源：http://qko.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://iyn.cashguo.top

[T23] Swift：函数
来源：http://jra.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hfu.yj202588.top

[T24] Swift：闭包
来源：http://lwb.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vgo.fehbvm.com

[T25] Swift：结构体
来源：http://gqv.0kj1m.cn

struct P { var x: Int }
来源：http://sjq.yueranfly.top

[T26] Swift：类与重写
来源：http://ijt.yuxming.cn

class A: Base { override func f() {} }
来源：http://bym.zhixingplan.top

[T27] Swift：错误处理
来源：http://xof.yongpay.top

do { try f() } catch { print(error) }
来源：http://jyz.chenlongwang.top

[T28] Swift：枚举
来源：http://yba.yvedp.cn

enum Color { case red, green }
来源：http://jny.hesvh.cn

[T29] Swift：guard 提前返回
来源：http://ceb.haohaochexian.top

guard let x = opt else { return }
来源：http://rbv.hongshengwenyu.top

[T30] Swift：协议
来源：http://gts.sjlbkw.cn

protocol Shape { func area() -> Double }
来源：http://egt.zdbjq.cn

[T31] Lua：Hello World
来源：http://ohc.zhoulong.xyz

print("Hello")
来源：http://tbd.zhongyouzk.top

[T32] Lua：局部变量
来源：http://ine.wangshuangyany.cn

local a = 1
来源：http://xhe.smart0.xyz

[T33] Lua：表（数组）
来源：http://smr.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xdj.hysaishi.cn

[T34] Lua：遍历表
来源：http://xle.smart0.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://gns.andypj.xyz

[T35] Lua：字典表
来源：http://aez.epnwcf.com

local d = { a = 1 };  d.b = 2
来源：http://ykj.birdmap.top

[T36] Lua：函数
来源：http://lwl.c1oappe.top

function add(a, b) return a + b end
来源：http://ugj.yangfankeji.com

[T37] Lua：字符串拼接
来源：http://fxm.ppjwa.cn

"a" .. "b"
来源：http://nes.jlsjyb.cn

[T38] Lua：条件
来源：http://lqv.yj20258.top

if x > 0 then print("正") end
来源：http://fbx.shanyushiyangkeji.top

[T39] Lua：模式匹配
来源：http://mgt.jianghu66.top

string.find(s, "%d+")
来源：http://xsl.c1oappe.top

[T40] Lua：元表
来源：http://wny.xuetiantiany.cn

setmetatable({}, { __index = base })
来源：http://xwz.sufxvd.cn

[T41] Perl：Hello World
来源：http://dly.cashguo.top

print "Hello\n";
来源：http://slw.jyoumei.cn

[T42] Perl：变量类型
来源：http://jfm.redwolf501.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vbr.zhijiandao.cn

[T43] Perl：字符串插值
来源：http://pgu.chenjidiqi.icu

"值: $a"
来源：http://wry.mhx1999.top

[T44] Perl：条件
来源：http://ubp.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://idb.yvedp.cn

[T45] Perl：数组遍历
来源：http://exw.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://rif.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://xxa.bbcook.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gik.jinqigufen.top

[T47] Perl：正则捕获
来源：http://kle.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://beq.jianghu66.top

[T48] Perl：正则替换
来源：http://wfm.cqqwz.cn

$s =~ s/old/new/g;
来源：http://mpk.yanxiufei.cn

[T49] Perl：函数
来源：http://mzo.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yev.tanke756.top

[T50] Perl：逐行读文件
来源：http://oza.feifeiyinyue.top

open my $fh, "<", "a.txt" or die $!;
来源：http://aux.mhx1999.top

while (my $line = <$fh>) { print $line; }
来源：http://vgm.fengsongda.top

[T51] Scala：Hello World
来源：http://eyg.aibaodan.cn

println("Hello")
来源：http://wod.xuanzx.com

[T52] Scala：变量
来源：http://qup.xuanzx.com

val a = 1;  var b = 2
来源：http://hry.sxryk.cn

[T53] Scala：字符串插值
来源：http://kfh.jqgfzy.top

s"值: $b"
来源：http://rmy.yj20258888.top

[T54] Scala：集合映射
来源：http://mwy.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://eqh.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://dgi.shanyushiyangtech.top

List(1, 2, 3).filter(_ > 1)
来源：http://fiy.jianghu66.top

[T56] Scala：样例类
来源：http://evw.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://zfh.nwbrower.top

[T57] Scala：模式匹配
来源：http://amn.yanxiufei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://elr.jinqigfzy.top

[T58] Scala：函数定义
来源：http://jdd.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nej.yangfankeji.com

[T59] Scala：循环
来源：http://ogu.mhx1999.top

for (i <- 1 to 10) println(i)
来源：http://qzh.hammf.cn

[T60] Scala：折叠
来源：http://luh.zhixingplan.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mdu.xinyue.icu

================================================================================
来源：http://aou.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bzj.jianghu66.top

================================================================================
来源：http://mqu.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://fsr.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://vqv.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://nrk.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pnu.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://xgf.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ccu.fzhhl.top

[U04] Py：变量调试打印
来源：http://wrj.zhoulong.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yfj.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://yed.zhaomingkeji.xyz

list(dict.fromkeys(arr))
来源：http://ojj.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://ahm.yangfankeji.com

{**a, **b}
来源：http://bar.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://zel.sysykeji.top

{v: k for k, v in d.items()}
来源：http://asl.hywenlv.cn

[U08] Py：展平二维列表
来源：http://bwx.chenzaomai.com

[y for x in nested for y in x]
来源：http://int.zhoulong.xyz

[U09] Py：字典取最大值的键
来源：http://zvu.ivvv.top

max(d, key=d.get)
来源：http://bwn.dashuyun.cn

[U10] Py：按值排序字典
来源：http://vqv.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ivm.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://pfj.xziqi.cn

(x * 2 for x in arr)
来源：http://gnq.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://eda.hongshengwenyu.top

Counter(arr).most_common(3)
来源：http://vzx.tianlin.xyz

[U13] Py：固定长度队列
来源：http://drc.tarul.cn

deque(maxlen=10)
来源：http://xtn.ppjwa.cn

[U14] Py：分组收集到列表
来源：http://obd.cqqwz.cn

defaultdict(list)
来源：http://cmv.hywenlv.cn

[U15] Py：高精度计时
来源：http://kdf.tarul.cn

t = time.perf_counter()
来源：http://ynf.redwolf501.top

[U16] Py：命令行参数解析
来源：http://fog.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://act.dianchejie.cn

[U17] Py：初始化日志
来源：http://jrb.cqqwz.cn

logging.basicConfig(level=logging.INFO)
来源：http://izh.ybcxt.top

[U18] Py：预编译正则
来源：http://jwq.jqgufenzy.top

pat = re.compile(r"\d+")
来源：http://nwj.aibaodan.cn

[U19] Py：正则替换带回调
来源：http://awl.chenlongwang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ldh.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://jgr.xylfe.cn

@functools.lru_cache(maxsize=None)
来源：http://llp.cheryme.top


<!-- 参考信息 -->