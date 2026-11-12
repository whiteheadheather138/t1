代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rbg.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://acm.chenlongwang.top

time ./run.sh
来源：http://yti.hnqzz.top

================================================================================
来源：http://sqb.yanxiufei.cn

S. C / C++ 专题
来源：http://kgm.cucudq.cn

================================================================================
来源：http://jmh.fehbvm.com

[S01] C：Hello World
来源：http://phl.birdmap.top

#include <stdio.h>
来源：http://zda.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://uvi.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://rdx.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://jli.gaohongyu789.top

[S03] C：读入整数
来源：http://qzf.dianchejie.cn

int x; scanf("%d", &x);
来源：http://jda.52xcode.cn

[S04] C：字符串复制
来源：http://mla.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://jzb.hnqzz.top

[S05] C：字符串长度
来源：http://ctr.nwbrower.top

strlen(s)
来源：http://gdp.xziqi.cn

[S06] C：字符串比较
来源：http://nuh.tian-w.cn

strcmp(a, b) == 0
来源：http://lzh.hywenlv.cn

[S07] C：数组遍历求和
来源：http://rph.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eyn.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://ddh.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jaa.tanke756.top

[S09] C：结构体定义与初始化
来源：http://yso.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wef.chenlongwang.top

[S10] C：指针与解引用
来源：http://vfx.hongshengwenyu.top

int *p = &a;  *p = 5;
来源：http://qmj.tanke756.top

[S11] C：逐行读文件
来源：http://ixn.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://zsu.hesvh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kep.jinqigufen.top

fclose(f);
来源：http://wct.jqgfzy.top

[S12] C：写文件
来源：http://rhx.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://icl.chenlongwang.top

[S13] C：宏定义
来源：http://ikv.gzhubu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uti.sysykeji.top

[S14] C：枚举
来源：http://bms.nwbrower.top

enum Color { RED, GREEN, BLUE };
来源：http://zrr.fengsongda.top

[S15] C：类型转换
来源：http://doj.nwbrower.top

(double) a / b
来源：http://ise.smart0.xyz

[S16] C：位操作置位
来源：http://eqy.iojbl.cn

x |= (1 << 3);
来源：http://afj.pengpengdd.cyou

[S17] C：安全拼接字符串
来源：http://kja.xuanzx.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fzu.ivvv.top

[S18] C：命令行参数
来源：http://kbf.fehbvm.com

int main(int argc, char **argv)
来源：http://tzk.ybcxt.top

[S19] C：快速排序
来源：http://prs.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nop.ppjwa.cn

[S20] C：二分查找
来源：http://mwl.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eot.redwolf501.top

[S21] C：字符类别判断
来源：http://jtp.yvedp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ogz.zhoulong.xyz

[S22] C：字符串转数字
来源：http://jja.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zsx.cashguo.top

[S23] C：随机数
来源：http://pzn.cdnleiting.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qbx.yj202588.top

[S24] C：获取本地时间
来源：http://enf.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bxv.kuanghao11.cn

[S25] C：内存拷贝
来源：http://cqg.haohaochexian.top

memcpy(dst, src, n);
来源：http://gcu.hammf.cn

[S26] C：内存清零
来源：http://pzr.yj202588.top

memset(a, 0, sizeof a);
来源：http://gmm.gzhubu.top

[S27] C：定义常量
来源：http://jvh.yvedp.cn

const double PI = 3.14159;
来源：http://bff.hnqzz.top

[S28] C：静态变量
来源：http://flr.ppjwa.cn

static int counter = 0;
来源：http://htg.zhongyouzk.top

[S29] C：变参函数
来源：http://blm.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fvc.kuanghao11.cn

[S30] C：头文件保护
来源：http://jvt.jlsjyb.cn

#ifndef X_H
来源：http://sjx.sjlbkw.cn

#define X_H
来源：http://uwu.ydjk.org.cn

#endif
来源：http://bku.zhoulong.xyz

[S31] C++：Hello World
来源：http://wom.cashguo.top

#include <iostream>
来源：http://pti.zycfv.cn

int main() { std::cout << "Hello\n"; }
来源：http://cjh.vehdjk.com

[S32] C++：字符串
来源：http://uei.xingfuxueyuan.xyz

std::string s = "hi";  s += "!";
来源：http://xaz.ehwqpu.com

[S33] C++：vector 增删
来源：http://czb.ppjwa.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lxz.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://ois.vehdjk.com

for (auto &x : v) { std::cout << x; }
来源：http://rzn.cdnleiting.top

[S35] C++：map
来源：http://tft.ydjk.org.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xri.yanxiufei.cn

[S36] C++：unordered_map
来源：http://oel.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ril.gaohongyu789.top

[S37] C++：set
来源：http://rjy.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gua.yfazqb.com

[S38] C++：排序
来源：http://ckl.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://nly.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://xuu.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kva.chenzaomai.com

[S40] C++：查找元素
来源：http://snq.ybcxt.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rky.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://ozv.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cgk.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://ftu.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://urd.cqqwz.cn

[S43] C++：智能指针
来源：http://ccb.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://tjn.tanke756.top

[S44] C++：引用传参
来源：http://vzn.fengsongda.top

void inc(int &x) { ++x; }
来源：http://hif.hesvh.cn

[S45] C++：lambda
来源：http://ler.aibaodan.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cms.hfpthk.cn

[S46] C++：函数模板
来源：http://ufk.hnxiangtu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zbf.zycfv.cn

[S47] C++：结构化绑定遍历
来源：http://muu.svipenyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://src.chenlongwang.top

[S48] C++：逐行读文件
来源：http://ymd.shangyingyoupin.top

std::ifstream in("a.txt");  std::string line;
来源：http://kql.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://wlk.zycfv.cn

[S49] C++：写文件
来源：http://hjp.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://njb.tianlin.xyz

[S50] C++：格式化数字
来源：http://yde.yueranfly.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eix.ehwqpu.com

[S51] C++：显式类型转换
来源：http://bgx.havefunace.top

static_cast<double>(a) / b
来源：http://xpu.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://zfk.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://hpf.havefunace.top

[S53] C++：移动语义
来源：http://ywk.hywenlv.cn

std::vector<int> w = std::move(v);
来源：http://ghy.zdbjq.cn

[S54] C++：异常处理
来源：http://mbf.xuanzx.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hbw.gzhubu.top

[S55] C++：结构化绑定
来源：http://tip.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uyr.0kj1m.cn

[S56] C++：optional
来源：http://ypk.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://stt.ybcxt.top

[S57] C++：编译期常量
来源：http://kso.fehbvm.com

constexpr int N = 10;
来源：http://avf.jqgfzy.top

[S58] C++：命名空间
来源：http://lag.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://fmr.xuetiantiany.cn

[S59] C++：静态断言
来源：http://lsz.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uqq.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://gfy.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dwo.zhoulong.xyz

================================================================================
来源：http://rha.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zbl.hysaishi.cn

================================================================================
来源：http://xbx.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://wod.pengpengdd.cyou

println("Hello")
来源：http://vau.jqgfzy.top

[T02] Kotlin：变量
来源：http://via.zhijiandao.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://urn.vehdjk.com

[T03] Kotlin：字符串模板
来源：http://xty.jinyuanbaomall.cn

"值: $b"
来源：http://anp.birdmap.top

[T04] Kotlin：空安全
来源：http://qiq.smart0.xyz

val n: String? = null;  n?.length
来源：http://sgn.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://dvd.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://owe.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://gag.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wmy.wangshuangyany.cn

[T07] Kotlin：集合过滤
来源：http://zmc.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://tbv.hywenlv.cn

[T08] Kotlin：数据类
来源：http://wqe.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://lvo.316326.xyz

[T09] Kotlin：扩展函数
来源：http://bid.zhixingplan.top

fun String.exclaim() = this + "!"
来源：http://ujv.shuidangran.top

[T10] Kotlin：默认参数
来源：http://esu.yangfankeji.com

fun greet(name: String = "World") = "Hi $name"
来源：http://hdf.yfazqb.com

[T11] Kotlin：协程
来源：http://zpg.yuxming.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lys.ybcxt.top

[T12] Kotlin：解构声明
来源：http://ylg.yfazqb.com

val (a, b) = Pair(1, 2)
来源：http://xca.316326.xyz

[T13] Kotlin：只读 Map
来源：http://paa.gaohongyu789.top

val m = mapOf("a" to 1)
来源：http://vcn.ivvv.top

[T14] Kotlin：循环
来源：http://jgu.cdnleiting.top

for (i in 1..10) println(i)
来源：http://pyi.tarul.cn

[T15] Kotlin：接口
来源：http://bxp.guannengcc.top

interface Shape { fun area(): Double }
来源：http://fro.jinqigfzy.top

[T16] Swift：Hello World
来源：http://faa.zdqjudy.top

print("Hello")
来源：http://nsq.yongpay.top

[T17] Swift：变量与常量
来源：http://zud.ivvv.top

var a = 1;  let b = 2
来源：http://lag.hysaishi.cn

[T18] Swift：字符串插值
来源：http://qga.zhengqikj.top

"值: \(b)"
来源：http://dxz.bbcook.cn

[T19] Swift：可选绑定
来源：http://ifn.jlsjyb.cn

if let n = opt { print(n) }
来源：http://qvq.uphjek.com

[T20] Swift：数组操作
来源：http://vov.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://hfd.chenlongwang.top

[T21] Swift：遍历
来源：http://qdz.zhixingplan.top

for x in a { print(x) }
来源：http://hil.feifeiyinyue.top

[T22] Swift：字典
来源：http://elk.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wht.yj20258888.top

[T23] Swift：函数
来源：http://zrg.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xid.guannengcc.top

[T24] Swift：闭包
来源：http://bph.aibaodan.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vpe.hywenlv.cn

[T25] Swift：结构体
来源：http://rum.yongpay.top

struct P { var x: Int }
来源：http://kne.zdqjudy.top

[T26] Swift：类与重写
来源：http://cdw.shzxlz.cn

class A: Base { override func f() {} }
来源：http://lmx.c1oappe.top

[T27] Swift：错误处理
来源：http://agx.hesvh.cn

do { try f() } catch { print(error) }
来源：http://kvp.jinqigfzy.top

[T28] Swift：枚举
来源：http://bwo.xziqi.cn

enum Color { case red, green }
来源：http://oih.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://nyh.jqgufenzy.top

guard let x = opt else { return }
来源：http://hhp.cheryme.top

[T30] Swift：协议
来源：http://owh.yonumen.top

protocol Shape { func area() -> Double }
来源：http://zhe.yj20258.top

[T31] Lua：Hello World
来源：http://yqq.shanyushiyangtech.top

print("Hello")
来源：http://xwc.yj20258888.top

[T32] Lua：局部变量
来源：http://lxg.jyoumei.cn

local a = 1
来源：http://njh.yfazqb.com

[T33] Lua：表（数组）
来源：http://hkr.nanxuanxn.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gww.havefunace.top

[T34] Lua：遍历表
来源：http://xkc.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://oom.yj20258888.top

[T35] Lua：字典表
来源：http://xrt.wangshuangyany.cn

local d = { a = 1 };  d.b = 2
来源：http://iqi.fehbvm.com

[T36] Lua：函数
来源：http://lin.mhx1999.top

function add(a, b) return a + b end
来源：http://hmb.wangdashe.top

[T37] Lua：字符串拼接
来源：http://mrr.chenlongwang.top

"a" .. "b"
来源：http://pcv.aizwys.cn

[T38] Lua：条件
来源：http://vjx.sxryk.cn

if x > 0 then print("正") end
来源：http://ipp.wangshuangyany.cn

[T39] Lua：模式匹配
来源：http://yjw.zhaomingkeji.xyz

string.find(s, "%d+")
来源：http://gaf.jinqigufen.top

[T40] Lua：元表
来源：http://ipl.haohaochexian.top

setmetatable({}, { __index = base })
来源：http://xmo.uphjek.com

[T41] Perl：Hello World
来源：http://frn.9152youxi.cn

print "Hello\n";
来源：http://ymv.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://ihl.jlsjyb.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lzk.cqqwz.cn

[T43] Perl：字符串插值
来源：http://tct.nwbrower.top

"值: $a"
来源：http://ilw.cucudq.cn

[T44] Perl：条件
来源：http://mub.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://oca.nanxuanxn.top

[T45] Perl：数组遍历
来源：http://tik.yueranfly.top

for my $x (@arr) { print $x; }
来源：http://uyd.tianlin.xyz

[T46] Perl：哈希操作
来源：http://yxn.tian-w.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lut.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://lyi.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rst.yj20258.top

[T48] Perl：正则替换
来源：http://jrs.gotoacloud.top

$s =~ s/old/new/g;
来源：http://bsc.dashuyun.cn

[T49] Perl：函数
来源：http://rqg.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lzx.epnwcf.com

[T50] Perl：逐行读文件
来源：http://wgr.gzhubu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uza.yfazqb.com

while (my $line = <$fh>) { print $line; }
来源：http://tbu.dianchejie.cn

[T51] Scala：Hello World
来源：http://xoi.cucudq.cn

println("Hello")
来源：http://oip.gotoacloud.top

[T52] Scala：变量
来源：http://mpi.zdqjudy.top

val a = 1;  var b = 2
来源：http://afu.pycfn.com

[T53] Scala：字符串插值
来源：http://ifd.vehdjk.com

s"值: $b"
来源：http://jpe.quarkkingdee.top

[T54] Scala：集合映射
来源：http://hxw.jiagoushi.top

List(1, 2, 3).map(_ * 2)
来源：http://cmj.jlsjyb.cn

[T55] Scala：集合过滤
来源：http://wvp.xingfuxueyuan.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://prt.fengsongda.top

[T56] Scala：样例类
来源：http://pat.gogol.net.cn

case class User(name: String, age: Int)
来源：http://xjk.c1oappe.top

[T57] Scala：模式匹配
来源：http://kxg.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fur.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://bgu.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://gxr.daria6918.cn

[T59] Scala：循环
来源：http://cdr.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://lql.xylfe.cn

[T60] Scala：折叠
来源：http://eqh.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gyy.cqqwz.cn

================================================================================
来源：http://yec.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dok.yj20258888.top

================================================================================
来源：http://jsk.sysykeji.top

[U01] Py：创建虚拟环境
来源：http://bfm.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://qdw.zdbjq.cn

[U02] Py：导出 / 安装依赖
来源：http://vry.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cjp.aibaodan.cn

[U03] Py：加载 .env 配置
来源：http://cik.fktsv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://awo.shzxlz.cn

[U04] Py：变量调试打印
来源：http://ivj.tanke756.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wnt.sufxvd.cn

[U05] Py：列表去重且保序
来源：http://ryj.bbcook.cn

list(dict.fromkeys(arr))
来源：http://bqj.nanxinkj.top

[U06] Py：合并两个字典
来源：http://sqb.iojbl.cn

{**a, **b}
来源：http://esb.daxiang520.top

[U07] Py：反转字典键值
来源：http://dia.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://fsn.shanyushiyangtech.top

[U08] Py：展平二维列表
来源：http://pfs.52xcode.cn

[y for x in nested for y in x]
来源：http://nmt.zdqjudy.top

[U09] Py：字典取最大值的键
来源：http://pgs.aizwys.cn

max(d, key=d.get)
来源：http://djt.yvedp.cn

[U10] Py：按值排序字典
来源：http://ssb.jiagoushi.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dqp.uphjek.com

[U11] Py：生成器表达式
来源：http://jwk.sysykeji.top

(x * 2 for x in arr)
来源：http://san.smart0.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://ung.jinqigufen.top

Counter(arr).most_common(3)
来源：http://awm.yfazqb.com

[U13] Py：固定长度队列
来源：http://cze.hesvh.cn

deque(maxlen=10)
来源：http://ayi.zhiwuduotai.top

[U14] Py：分组收集到列表
来源：http://jnc.zhijiandao.cn

defaultdict(list)
来源：http://wgx.zdbjq.cn

[U15] Py：高精度计时
来源：http://fsc.yj20258888.top

t = time.perf_counter()
来源：http://obn.9152youxi.cn

[U16] Py：命令行参数解析
来源：http://hur.jqgfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zkq.havefunace.top

[U17] Py：初始化日志
来源：http://mfd.xziqi.cn

logging.basicConfig(level=logging.INFO)
来源：http://hkm.vehdjk.com

[U18] Py：预编译正则
来源：http://kkp.sysykeji.top

pat = re.compile(r"\d+")
来源：http://fpj.meibo888.top

[U19] Py：正则替换带回调
来源：http://amy.fzhhl.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iaq.sysykeji.top

[U20] Py：缓存函数结果
来源：http://fmg.yanxiufei.cn

@functools.lru_cache(maxsize=None)
来源：http://bbk.zhixingplan.top


<!-- 参考信息 -->