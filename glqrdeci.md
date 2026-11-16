代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bjx.hywenlv.cn

[R80] 查看脚本执行耗时
来源：http://daj.hysaishi.cn

time ./run.sh
来源：http://sag.xziqi.cn

================================================================================
来源：http://scu.gotoacloud.top

S. C / C++ 专题
来源：http://shb.ivvv.top

================================================================================
来源：http://ogc.guowangkeji.top

[S01] C：Hello World
来源：http://diw.aizwys.cn

#include <stdio.h>
来源：http://fuo.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rwk.hongshengwenyu.top

[S02] C：变量与格式化输出
来源：http://odo.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://etf.shzxlz.cn

[S03] C：读入整数
来源：http://shm.jyoumei.cn

int x; scanf("%d", &x);
来源：http://xxq.pengpengdd.cyou

[S04] C：字符串复制
来源：http://mbx.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://lbi.ydjk.org.cn

[S05] C：字符串长度
来源：http://cbh.yonumen.top

strlen(s)
来源：http://qla.smart0.xyz

[S06] C：字符串比较
来源：http://sib.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://nrp.zhixingplan.top

[S07] C：数组遍历求和
来源：http://oct.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fyz.pycfn.com

[S08] C：动态内存分配与释放
来源：http://svj.ydzc1.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ubm.nanxinkj.top

[S09] C：结构体定义与初始化
来源：http://wmx.jqgufenzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hle.0kj1m.cn

[S10] C：指针与解引用
来源：http://bcn.52xcode.cn

int *p = &a;  *p = 5;
来源：http://xml.wangdashe.top

[S11] C：逐行读文件
来源：http://fwj.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://psn.ehwqpu.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://wkp.xuetiantiany.cn

fclose(f);
来源：http://ijk.aizwys.cn

[S12] C：写文件
来源：http://tak.chenzaomai.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gau.gzhubu.top

[S13] C：宏定义
来源：http://ibk.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ilz.xuanzx.com

[S14] C：枚举
来源：http://zhe.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://uwl.smart0.xyz

[S15] C：类型转换
来源：http://mdg.fengsongda.top

(double) a / b
来源：http://gqg.jinghuilouyu.cn

[S16] C：位操作置位
来源：http://czm.birdmap.top

x |= (1 << 3);
来源：http://sot.316326.xyz

[S17] C：安全拼接字符串
来源：http://tqg.zycfv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://olt.chenzaomai.com

[S18] C：命令行参数
来源：http://jgb.smart0.xyz

int main(int argc, char **argv)
来源：http://vlr.xuetiantiany.cn

[S19] C：快速排序
来源：http://crp.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zlt.yueranfly.top

[S20] C：二分查找
来源：http://zrg.pycfn.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ghh.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://bhe.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://neg.kuanghao11.cn

[S22] C：字符串转数字
来源：http://jqo.cashguo.top

atoi("42");  strtod("3.14", NULL);
来源：http://vop.mhx1999.top

[S23] C：随机数
来源：http://ynp.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mmu.c1oappe.top

[S24] C：获取本地时间
来源：http://uxq.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kcu.yueranfly.top

[S25] C：内存拷贝
来源：http://fqz.yangfankeji.com

memcpy(dst, src, n);
来源：http://fxb.gogol.net.cn

[S26] C：内存清零
来源：http://tdv.bjfxy.top

memset(a, 0, sizeof a);
来源：http://kqm.xuanzx.com

[S27] C：定义常量
来源：http://hof.yj202588.top

const double PI = 3.14159;
来源：http://jxf.cheryme.top

[S28] C：静态变量
来源：http://omh.jinqigufen.top

static int counter = 0;
来源：http://lhb.jyoumei.cn

[S29] C：变参函数
来源：http://aun.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cgi.chenjidiqi.icu

[S30] C：头文件保护
来源：http://gng.mhx1999.top

#ifndef X_H
来源：http://yab.gaohongyu789.top

#define X_H
来源：http://csr.guannengcc.top

#endif
来源：http://ihy.zhiwuduotai.top

[S31] C++：Hello World
来源：http://fdw.yueranfly.top

#include <iostream>
来源：http://jag.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://isi.hcnkem.com

[S32] C++：字符串
来源：http://opn.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://apx.meibo888.top

[S33] C++：vector 增删
来源：http://knk.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sns.wangdashe.top

[S34] C++：遍历 vector
来源：http://lby.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://zlr.nanxuanxn.top

[S35] C++：map
来源：http://nlj.shanyushiyangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zhk.havefunace.top

[S36] C++：unordered_map
来源：http://xhb.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uof.0kj1m.cn

[S37] C++：set
来源：http://omr.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://snz.xuanzx.com

[S38] C++：排序
来源：http://ejt.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://dbl.sweek.top

[S39] C++：自定义比较器排序
来源：http://xoa.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ubv.ehwqpu.com

[S40] C++：查找元素
来源：http://hzx.epnwcf.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iws.tianlin.xyz

[S41] C++：类与构造函数
来源：http://jkq.shanyushiyangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://keq.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://szs.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://tyu.jianghu66.top

[S43] C++：智能指针
来源：http://elx.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://ams.fktsv.cn

[S44] C++：引用传参
来源：http://aet.jlsjyb.cn

void inc(int &x) { ++x; }
来源：http://alw.fengsongda.top

[S45] C++：lambda
来源：http://psy.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://yah.chenjidiqi.icu

[S46] C++：函数模板
来源：http://wjt.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yrw.yj202588.top

[S47] C++：结构化绑定遍历
来源：http://wqf.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qpg.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://lbs.shanyushiyangtech.top

std::ifstream in("a.txt");  std::string line;
来源：http://lcf.zhiwuduotai.top

while (std::getline(in, line)) { }
来源：http://tdu.gogol.net.cn

[S49] C++：写文件
来源：http://ghq.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xhz.zhijiandao.cn

[S50] C++：格式化数字
来源：http://upm.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gyv.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://aae.tarul.cn

static_cast<double>(a) / b
来源：http://jll.quarkkingdee.top

[S52] C++：const 与 noexcept
来源：http://jmf.tian-w.cn

int size() const noexcept { return n_; }
来源：http://ohl.daria6918.cn

[S53] C++：移动语义
来源：http://fij.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://sik.cdnleiting.top

[S54] C++：异常处理
来源：http://zjq.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cdv.bjfxy.top

[S55] C++：结构化绑定
来源：http://rus.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yzw.uphjek.com

[S56] C++：optional
来源：http://jkn.vehdjk.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aqv.aibaodan.cn

[S57] C++：编译期常量
来源：http://pds.havefunace.top

constexpr int N = 10;
来源：http://soj.xziqi.cn

[S58] C++：命名空间
来源：http://oda.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://bir.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://npx.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lez.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://uvp.gogol.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fkm.yj20258888.top

================================================================================
来源：http://bvg.zycfv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iyf.gogol.net.cn

================================================================================
来源：http://ifd.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://viu.ydzc1.top

println("Hello")
来源：http://rab.aibaodan.cn

[T02] Kotlin：变量
来源：http://gdf.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://puj.hnxiangtu.top

[T03] Kotlin：字符串模板
来源：http://sls.jqgfzy.top

"值: $b"
来源：http://hgy.tian-w.cn

[T04] Kotlin：空安全
来源：http://pms.sysykeji.top

val n: String? = null;  n?.length
来源：http://wsf.cheryme.top

[T05] Kotlin：when 表达式
来源：http://dsn.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cfi.52xcode.cn

[T06] Kotlin：集合映射
来源：http://yin.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xso.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://kht.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rfl.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://wap.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://sym.ywan-chungtsiang.top

[T09] Kotlin：扩展函数
来源：http://gjx.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://zpu.shuidangran.top

[T10] Kotlin：默认参数
来源：http://evt.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://aqc.ppjwa.cn

[T11] Kotlin：协程
来源：http://rpg.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://etd.ybcxt.top

[T12] Kotlin：解构声明
来源：http://lra.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://axp.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://bvi.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://gdv.c1oappe.top

[T14] Kotlin：循环
来源：http://vmv.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://jqw.ywan-chungtsiang.top

[T15] Kotlin：接口
来源：http://uin.jqgufenzy.top

interface Shape { fun area(): Double }
来源：http://tsr.tian-w.cn

[T16] Swift：Hello World
来源：http://kpo.fehbvm.com

print("Hello")
来源：http://zzj.shuidangran.top

[T17] Swift：变量与常量
来源：http://jgt.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://ugs.jiagoushi.top

[T18] Swift：字符串插值
来源：http://jvf.zhiwuduotai.top

"值: \(b)"
来源：http://agv.wangshuangyany.cn

[T19] Swift：可选绑定
来源：http://rrh.yangfankeji.com

if let n = opt { print(n) }
来源：http://mvl.chenlongwang.top

[T20] Swift：数组操作
来源：http://vgb.cheryme.top

var a = [1, 2, 3];  a.append(4)
来源：http://gdx.chenlongwang.top

[T21] Swift：遍历
来源：http://adb.cashguo.top

for x in a { print(x) }
来源：http://hbo.jyoumei.cn

[T22] Swift：字典
来源：http://qba.c1oappe.top

var d = ["a": 1];  d["b"] = 2
来源：http://voa.shanyushiyangtech.top

[T23] Swift：函数
来源：http://anf.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zqm.nanxinkj.top

[T24] Swift：闭包
来源：http://esl.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wlo.hcnkem.com

[T25] Swift：结构体
来源：http://whe.daria6918.cn

struct P { var x: Int }
来源：http://viy.chenlongwang.top

[T26] Swift：类与重写
来源：http://kck.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://nex.bjfxy.top

[T27] Swift：错误处理
来源：http://jml.sysykeji.top

do { try f() } catch { print(error) }
来源：http://iqh.hywenlv.cn

[T28] Swift：枚举
来源：http://fgi.zhijiandao.cn

enum Color { case red, green }
来源：http://suu.shangyingyoupin.top

[T29] Swift：guard 提前返回
来源：http://pwm.zhijiandao.cn

guard let x = opt else { return }
来源：http://ayu.hfpthk.cn

[T30] Swift：协议
来源：http://eny.sweek.top

protocol Shape { func area() -> Double }
来源：http://ffk.shanyushiyangtech.top

[T31] Lua：Hello World
来源：http://puq.cashguo.top

print("Hello")
来源：http://cro.zhongyouzk.top

[T32] Lua：局部变量
来源：http://ucb.vqdsnc.cn

local a = 1
来源：http://hmo.zhijiandao.cn

[T33] Lua：表（数组）
来源：http://dlq.zdqjudy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dir.hfpthk.cn

[T34] Lua：遍历表
来源：http://ngi.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pdf.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://ugt.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://mbe.yfazqb.com

[T36] Lua：函数
来源：http://jkk.jiagoushi.top

function add(a, b) return a + b end
来源：http://gfr.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://sud.c1oappe.top

"a" .. "b"
来源：http://lru.jianghu66.top

[T38] Lua：条件
来源：http://syp.jqgufenzy.top

if x > 0 then print("正") end
来源：http://lkx.zdqjudy.top

[T39] Lua：模式匹配
来源：http://hgt.cashguo.top

string.find(s, "%d+")
来源：http://mrl.zhengqikj.top

[T40] Lua：元表
来源：http://wnx.yuxming.cn

setmetatable({}, { __index = base })
来源：http://mcn.meibo888.top

[T41] Perl：Hello World
来源：http://nil.jinyuanbaomall.cn

print "Hello\n";
来源：http://jvb.jqgfzy.top

[T42] Perl：变量类型
来源：http://tel.birdmap.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cin.jinghuilouyu.cn

[T43] Perl：字符串插值
来源：http://brl.nwbrower.top

"值: $a"
来源：http://nqn.pycfn.com

[T44] Perl：条件
来源：http://cxi.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://hfy.iojbl.cn

[T45] Perl：数组遍历
来源：http://rnb.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://jwe.yj20258888.top

[T46] Perl：哈希操作
来源：http://nyx.epnwcf.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rfh.cashguo.top

[T47] Perl：正则捕获
来源：http://wsc.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://klx.redwolf501.top

[T48] Perl：正则替换
来源：http://wgf.guowangkeji.top

$s =~ s/old/new/g;
来源：http://ych.daria6918.cn

[T49] Perl：函数
来源：http://vks.tian-w.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://edv.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://kvv.haohaochexian.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lch.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://qto.ctjpmb.com

[T51] Scala：Hello World
来源：http://nca.hywenlv.cn

println("Hello")
来源：http://zxw.birdmap.top

[T52] Scala：变量
来源：http://ttr.quarkkingdee.top

val a = 1;  var b = 2
来源：http://qfu.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://ccf.gzhubu.top

s"值: $b"
来源：http://glj.yueranfly.top

[T54] Scala：集合映射
来源：http://vah.cqqwz.cn

List(1, 2, 3).map(_ * 2)
来源：http://hpf.sysykeji.top

[T55] Scala：集合过滤
来源：http://var.vqdsnc.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gnu.zycfv.cn

[T56] Scala：样例类
来源：http://jju.havefunace.top

case class User(name: String, age: Int)
来源：http://nbb.zhengqikj.top

[T57] Scala：模式匹配
来源：http://kbc.cheryme.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rzz.cashguo.top

[T58] Scala：函数定义
来源：http://eaq.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bcb.zhoulong.xyz

[T59] Scala：循环
来源：http://kfw.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://tff.dashuyun.cn

[T60] Scala：折叠
来源：http://iod.wangshuangyany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cbh.ehwqpu.com

================================================================================
来源：http://gpf.fzhhl.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pdr.xingfuxueyuan.xyz

================================================================================
来源：http://vvb.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://fvf.jinghuilouyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zot.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://fei.sweek.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mgs.jinqigfzy.top

[U03] Py：加载 .env 配置
来源：http://mlx.vqdsnc.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xco.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://wbz.tian-w.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jag.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://nyz.cheryme.top

list(dict.fromkeys(arr))
来源：http://gxw.andypj.xyz

[U06] Py：合并两个字典
来源：http://flj.nanxinkj.top

{**a, **b}
来源：http://nik.meibo888.top

[U07] Py：反转字典键值
来源：http://coe.yj20258888.top

{v: k for k, v in d.items()}
来源：http://kri.yj202588.top

[U08] Py：展平二维列表
来源：http://ltq.tarul.cn

[y for x in nested for y in x]
来源：http://pcw.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://jiz.svipenyu.cn

max(d, key=d.get)
来源：http://ryl.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://dzh.redwolf501.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ygt.aizwys.cn

[U11] Py：生成器表达式
来源：http://htk.redwolf501.top

(x * 2 for x in arr)
来源：http://cqe.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nva.fehbvm.com

Counter(arr).most_common(3)
来源：http://dsg.iojbl.cn

[U13] Py：固定长度队列
来源：http://adc.iojbl.cn

deque(maxlen=10)
来源：http://vnu.hammf.cn

[U14] Py：分组收集到列表
来源：http://nrp.tanke756.top

defaultdict(list)
来源：http://jis.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://goo.xziqi.cn

t = time.perf_counter()
来源：http://eir.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://oii.snrcjt.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tgi.guannengcc.top

[U17] Py：初始化日志
来源：http://ikz.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://dzw.andypj.xyz

[U18] Py：预编译正则
来源：http://byy.hfpthk.cn

pat = re.compile(r"\d+")
来源：http://tgf.yfazqb.com

[U19] Py：正则替换带回调
来源：http://zim.jinqigfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://slz.gaohongyu789.top

[U20] Py：缓存函数结果
来源：http://iqv.uphjek.com

@functools.lru_cache(maxsize=None)
来源：http://gtu.tanke756.top


<!-- 参考信息 -->