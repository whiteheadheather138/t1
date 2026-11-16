代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://frj.cashguo.top

[R80] 查看脚本执行耗时
来源：http://kpt.jqgfzy.top

time ./run.sh
来源：http://cgo.fanxiaobao.xyz

================================================================================
来源：http://bnx.haohaochexian.top

S. C / C++ 专题
来源：http://bmw.gzhubu.top

================================================================================
来源：http://nkt.jinqigufen.top

[S01] C：Hello World
来源：http://ftv.andypj.xyz

#include <stdio.h>
来源：http://uoe.9152youxi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yii.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://yss.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://hel.hfpthk.cn

[S03] C：读入整数
来源：http://xlw.pycfn.com

int x; scanf("%d", &x);
来源：http://rsf.iojbl.cn

[S04] C：字符串复制
来源：http://kvk.jqgufenzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://fxl.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://txh.nanxinkj.top

strlen(s)
来源：http://ury.yueranfly.top

[S06] C：字符串比较
来源：http://jxg.52xcode.cn

strcmp(a, b) == 0
来源：http://nwc.hcnkem.com

[S07] C：数组遍历求和
来源：http://wkt.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zva.wangdashe.top

[S08] C：动态内存分配与释放
来源：http://xdu.shanyushiyangtech.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hzu.yongpay.top

[S09] C：结构体定义与初始化
来源：http://ytb.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cze.nanxuanxn.top

[S10] C：指针与解引用
来源：http://yni.ydzc1.top

int *p = &a;  *p = 5;
来源：http://cbo.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://qvx.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://dds.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qur.nanxinkj.top

fclose(f);
来源：http://ogm.iojbl.cn

[S12] C：写文件
来源：http://qdz.sysykeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zuu.sxryk.cn

[S13] C：宏定义
来源：http://pfl.sjlbkw.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fmm.zycfv.cn

[S14] C：枚举
来源：http://jjr.snrcjt.cn

enum Color { RED, GREEN, BLUE };
来源：http://ukk.shuidangran.top

[S15] C：类型转换
来源：http://zua.quarkkingdee.top

(double) a / b
来源：http://rto.sufxvd.cn

[S16] C：位操作置位
来源：http://kgf.aibaodan.cn

x |= (1 << 3);
来源：http://oad.xingfuxueyuan.xyz

[S17] C：安全拼接字符串
来源：http://rhe.nanxinkj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uzi.yuanzhike.top

[S18] C：命令行参数
来源：http://xlz.ydzc1.top

int main(int argc, char **argv)
来源：http://dfd.guowangkeji.top

[S19] C：快速排序
来源：http://epv.jinghuilouyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nwa.shzxlz.cn

[S20] C：二分查找
来源：http://sko.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nmo.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://dxz.chenzaomai.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kwg.vehdjk.com

[S22] C：字符串转数字
来源：http://www.feifeiyinyue.top

atoi("42");  strtod("3.14", NULL);
来源：http://ecq.xylfe.cn

[S23] C：随机数
来源：http://ykd.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rwh.aizwys.cn

[S24] C：获取本地时间
来源：http://ech.gaohongyu789.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://drp.vqdsnc.cn

[S25] C：内存拷贝
来源：http://hwz.daxiang520.top

memcpy(dst, src, n);
来源：http://vzg.fzhhl.top

[S26] C：内存清零
来源：http://thw.xingfuxueyuan.xyz

memset(a, 0, sizeof a);
来源：http://plo.xziqi.cn

[S27] C：定义常量
来源：http://isl.smart0.xyz

const double PI = 3.14159;
来源：http://zrv.bjfxy.top

[S28] C：静态变量
来源：http://dsa.cqqwz.cn

static int counter = 0;
来源：http://usc.jinghuilouyu.cn

[S29] C：变参函数
来源：http://sjg.ehwqpu.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fpp.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://rwf.shanyushiyangkeji.top

#ifndef X_H
来源：http://udg.yj20258.top

#define X_H
来源：http://nob.316326.xyz

#endif
来源：http://kna.fktsv.cn

[S31] C++：Hello World
来源：http://vjh.daria6918.cn

#include <iostream>
来源：http://fth.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://dif.zhengqikj.top

[S32] C++：字符串
来源：http://zys.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://oxk.jinghuilouyu.cn

[S33] C++：vector 增删
来源：http://nlj.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wbm.redwolf501.top

[S34] C++：遍历 vector
来源：http://rmj.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://vot.yj20258.top

[S35] C++：map
来源：http://olj.ppjwa.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xiv.yj20258.top

[S36] C++：unordered_map
来源：http://agx.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wbi.yuanzhike.top

[S37] C++：set
来源：http://rie.jianghu66.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tbx.hcnkem.com

[S38] C++：排序
来源：http://gkw.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://feo.cdnleiting.top

[S39] C++：自定义比较器排序
来源：http://lgt.jqgfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://meh.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://zbs.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xzq.zdqjudy.top

[S41] C++：类与构造函数
来源：http://cin.yanxiufei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ktd.xylfe.cn

[S42] C++：继承与虚函数
来源：http://rly.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://jxn.zhixingplan.top

[S43] C++：智能指针
来源：http://fsn.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://zmx.nanxuanxn.top

[S44] C++：引用传参
来源：http://tdf.pycfn.com

void inc(int &x) { ++x; }
来源：http://sdw.yuanzhike.top

[S45] C++：lambda
来源：http://jpt.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://isw.vqdsnc.cn

[S46] C++：函数模板
来源：http://gyy.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vdv.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://myy.tianlin.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wbt.316326.xyz

[S48] C++：逐行读文件
来源：http://urv.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://noi.xylfe.cn

while (std::getline(in, line)) { }
来源：http://vax.iojbl.cn

[S49] C++：写文件
来源：http://ftv.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nxq.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://ddq.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://get.svipenyu.cn

[S51] C++：显式类型转换
来源：http://vyr.jianghu66.top

static_cast<double>(a) / b
来源：http://tia.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://skh.daxiang520.top

int size() const noexcept { return n_; }
来源：http://jci.316326.xyz

[S53] C++：移动语义
来源：http://ohm.tarul.cn

std::vector<int> w = std::move(v);
来源：http://bvp.jqgufenzy.top

[S54] C++：异常处理
来源：http://kka.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qph.yfazqb.com

[S55] C++：结构化绑定
来源：http://xzi.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cjf.ybcxt.top

[S56] C++：optional
来源：http://uex.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qwq.iojbl.cn

[S57] C++：编译期常量
来源：http://dit.tanke756.top

constexpr int N = 10;
来源：http://jsj.wangshuangyany.cn

[S58] C++：命名空间
来源：http://xss.fktsv.cn

namespace ns { int f() { return 1; } }
来源：http://vag.nanxinkj.top

[S59] C++：静态断言
来源：http://kwi.shanyushiyangtech.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://elw.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://jhw.tarul.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vgp.sufxvd.cn

================================================================================
来源：http://xiq.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zbh.xziqi.cn

================================================================================
来源：http://dex.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://das.jqgfzy.top

println("Hello")
来源：http://fer.gogol.net.cn

[T02] Kotlin：变量
来源：http://xnx.fengsongda.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jqd.sysykeji.top

[T03] Kotlin：字符串模板
来源：http://zjw.52xcode.cn

"值: $b"
来源：http://awe.jiagoushi.top

[T04] Kotlin：空安全
来源：http://nzk.yongpay.top

val n: String? = null;  n?.length
来源：http://uuv.gzhubu.top

[T05] Kotlin：when 表达式
来源：http://dmt.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://osy.daria6918.cn

[T06] Kotlin：集合映射
来源：http://nrs.hysaishi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rpk.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://gwn.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xvq.yongpay.top

[T08] Kotlin：数据类
来源：http://cud.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://ifm.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://nfb.jiagoushi.top

fun String.exclaim() = this + "!"
来源：http://khd.sysykeji.top

[T10] Kotlin：默认参数
来源：http://wcc.shanyushiyangtech.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gzr.zhoulong.xyz

[T11] Kotlin：协程
来源：http://bky.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iuz.havefunace.top

[T12] Kotlin：解构声明
来源：http://aoc.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://ayr.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://vdw.smart0.xyz

val m = mapOf("a" to 1)
来源：http://jra.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://cbx.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://nmx.snrcjt.cn

[T15] Kotlin：接口
来源：http://zzd.tianlin.xyz

interface Shape { fun area(): Double }
来源：http://wja.zhaomingkeji.xyz

[T16] Swift：Hello World
来源：http://jin.shangyingyoupin.top

print("Hello")
来源：http://lia.zycfv.cn

[T17] Swift：变量与常量
来源：http://pqs.hfpthk.cn

var a = 1;  let b = 2
来源：http://tsp.zdbjq.cn

[T18] Swift：字符串插值
来源：http://nvd.snrcjt.cn

"值: \(b)"
来源：http://deq.zycfv.cn

[T19] Swift：可选绑定
来源：http://rww.daxiang520.top

if let n = opt { print(n) }
来源：http://yef.quarkkingdee.top

[T20] Swift：数组操作
来源：http://qwb.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://bjj.xylfe.cn

[T21] Swift：遍历
来源：http://eix.gotoacloud.top

for x in a { print(x) }
来源：http://ipk.xziqi.cn

[T22] Swift：字典
来源：http://dpu.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://xfk.zhengqikj.top

[T23] Swift：函数
来源：http://nif.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ulr.gaohongyu789.top

[T24] Swift：闭包
来源：http://slo.jqgfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://djf.gogol.net.cn

[T25] Swift：结构体
来源：http://qwo.uphjek.com

struct P { var x: Int }
来源：http://ogc.tarul.cn

[T26] Swift：类与重写
来源：http://rfd.yuxming.cn

class A: Base { override func f() {} }
来源：http://mjt.fanxiaobao.xyz

[T27] Swift：错误处理
来源：http://afq.zhengqikj.top

do { try f() } catch { print(error) }
来源：http://pkv.nanxinkj.top

[T28] Swift：枚举
来源：http://vvk.pycfn.com

enum Color { case red, green }
来源：http://foe.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://rwt.pengpengdd.cyou

guard let x = opt else { return }
来源：http://lqx.gotoacloud.top

[T30] Swift：协议
来源：http://utk.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://sux.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://xfu.hfpthk.cn

print("Hello")
来源：http://ptm.yueranfly.top

[T32] Lua：局部变量
来源：http://npm.xylfe.cn

local a = 1
来源：http://kiq.chenlongwang.top

[T33] Lua：表（数组）
来源：http://fwq.cheryme.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pok.jiagoushi.top

[T34] Lua：遍历表
来源：http://esu.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://inr.kuanghao11.cn

[T35] Lua：字典表
来源：http://xod.haohaochexian.top

local d = { a = 1 };  d.b = 2
来源：http://ord.jqgfzy.top

[T36] Lua：函数
来源：http://haf.fzhhl.top

function add(a, b) return a + b end
来源：http://tab.pycfn.com

[T37] Lua：字符串拼接
来源：http://ldr.hywenlv.cn

"a" .. "b"
来源：http://tca.guowangkeji.top

[T38] Lua：条件
来源：http://hyo.fanxiaobao.xyz

if x > 0 then print("正") end
来源：http://bwq.andypj.xyz

[T39] Lua：模式匹配
来源：http://gtr.fktsv.cn

string.find(s, "%d+")
来源：http://uud.xuanzx.com

[T40] Lua：元表
来源：http://smc.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://ecs.aibaodan.cn

[T41] Perl：Hello World
来源：http://zlh.zhijiandao.cn

print "Hello\n";
来源：http://atz.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://hdb.9152youxi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lgq.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://hwv.zycfv.cn

"值: $a"
来源：http://sab.kuanghao11.cn

[T44] Perl：条件
来源：http://gtd.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://lpb.fengsongda.top

[T45] Perl：数组遍历
来源：http://skq.hywenlv.cn

for my $x (@arr) { print $x; }
来源：http://dzj.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://phm.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rto.nanxinkj.top

[T47] Perl：正则捕获
来源：http://kvt.316326.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://nsf.zdqjudy.top

[T48] Perl：正则替换
来源：http://yvj.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://oxq.ehwqpu.com

[T49] Perl：函数
来源：http://sjy.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qnj.zdqjudy.top

[T50] Perl：逐行读文件
来源：http://rre.sufxvd.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wwl.ydzc1.top

while (my $line = <$fh>) { print $line; }
来源：http://txy.sufxvd.cn

[T51] Scala：Hello World
来源：http://bed.jinyuanbaomall.cn

println("Hello")
来源：http://dag.yfazqb.com

[T52] Scala：变量
来源：http://dik.hfpthk.cn

val a = 1;  var b = 2
来源：http://qyp.hcnkem.com

[T53] Scala：字符串插值
来源：http://cex.yfazqb.com

s"值: $b"
来源：http://wfu.epnwcf.com

[T54] Scala：集合映射
来源：http://xwm.fengsongda.top

List(1, 2, 3).map(_ * 2)
来源：http://wck.pycfn.com

[T55] Scala：集合过滤
来源：http://liz.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://rnd.tanke756.top

[T56] Scala：样例类
来源：http://kyq.hesvh.cn

case class User(name: String, age: Int)
来源：http://tco.zycfv.cn

[T57] Scala：模式匹配
来源：http://ugc.ydjk.org.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tbk.jinqigufen.top

[T58] Scala：函数定义
来源：http://kkr.ydjk.org.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rcx.bbcook.cn

[T59] Scala：循环
来源：http://xzd.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://jzg.yueranfly.top

[T60] Scala：折叠
来源：http://gyp.xuetiantiany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aqy.shangyingyoupin.top

================================================================================
来源：http://vdi.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wyc.zdqjudy.top

================================================================================
来源：http://wve.snrcjt.cn

[U01] Py：创建虚拟环境
来源：http://fnh.ybcxt.top

python -m venv .venv && source .venv/bin/activate
来源：http://wwz.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://ssf.jinghuilouyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://byf.yj20258.top

[U03] Py：加载 .env 配置
来源：http://hjf.daxiang520.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ezj.jqgfzy.top

[U04] Py：变量调试打印
来源：http://pac.chenjidiqi.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sqg.cucudq.cn

[U05] Py：列表去重且保序
来源：http://nos.aizwys.cn

list(dict.fromkeys(arr))
来源：http://uvb.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://iql.zhengqikj.top

{**a, **b}
来源：http://xot.ppjwa.cn

[U07] Py：反转字典键值
来源：http://lrt.xylfe.cn

{v: k for k, v in d.items()}
来源：http://qdf.yvedp.cn

[U08] Py：展平二维列表
来源：http://lhd.yangfankeji.com

[y for x in nested for y in x]
来源：http://suw.zhengqikj.top

[U09] Py：字典取最大值的键
来源：http://zib.zhixingplan.top

max(d, key=d.get)
来源：http://wfz.hywenlv.cn

[U10] Py：按值排序字典
来源：http://qam.fanxiaobao.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nmp.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://jzo.tarul.cn

(x * 2 for x in arr)
来源：http://dpz.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://prk.jyoumei.cn

Counter(arr).most_common(3)
来源：http://ocx.jlsjyb.cn

[U13] Py：固定长度队列
来源：http://mxh.tian-w.cn

deque(maxlen=10)
来源：http://ugs.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://bho.shuidangran.top

defaultdict(list)
来源：http://anu.feifeiyinyue.top

[U15] Py：高精度计时
来源：http://msv.aibaodan.cn

t = time.perf_counter()
来源：http://gbd.jinghuilouyu.cn

[U16] Py：命令行参数解析
来源：http://mii.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://exb.yonumen.top

[U17] Py：初始化日志
来源：http://ipg.ppjwa.cn

logging.basicConfig(level=logging.INFO)
来源：http://wsa.smart0.xyz

[U18] Py：预编译正则
来源：http://ucj.jqgufenzy.top

pat = re.compile(r"\d+")
来源：http://vdr.fzhhl.top

[U19] Py：正则替换带回调
来源：http://nqa.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tte.jlsjyb.cn

[U20] Py：缓存函数结果
来源：http://ugr.redwolf501.top

@functools.lru_cache(maxsize=None)
来源：http://wyt.ydzc1.top


<!-- 参考信息 -->