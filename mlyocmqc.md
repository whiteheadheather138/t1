代发 wailian999

read -rp "请输入: " ans
来源：http://rul.yueranfly.top

[R78] 交互式菜单
来源：http://zmb.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mrr.zhongyouzk.top

[R79] 解析命令行选项
来源：http://ueq.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ioy.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://mkp.yongpay.top

time ./run.sh
来源：http://xyj.fzhhl.top

================================================================================
来源：http://wli.yfazqb.com

S. C / C++ 专题
来源：http://waq.hammf.cn

================================================================================
来源：http://fhx.hesvh.cn

[S01] C：Hello World
来源：http://sfj.zycfv.cn

#include <stdio.h>
来源：http://ffw.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zwr.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://qyl.shuidangran.top

int a = 10; printf("%d\n", a);
来源：http://uyh.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://eyh.fktsv.cn

int x; scanf("%d", &x);
来源：http://ilp.wangshuangyany.cn

[S04] C：字符串复制
来源：http://rgb.yuanzhike.top

char dst[32]; strcpy(dst, "hi");
来源：http://ikg.gzhubu.top

[S05] C：字符串长度
来源：http://svd.aibaodan.cn

strlen(s)
来源：http://tln.fktsv.cn

[S06] C：字符串比较
来源：http://azq.cqqwz.cn

strcmp(a, b) == 0
来源：http://uum.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://zca.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kzz.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://xsz.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vsd.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://mne.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fnr.aizwys.cn

[S10] C：指针与解引用
来源：http://nkt.nanxinkj.top

int *p = &a;  *p = 5;
来源：http://eji.sufxvd.cn

[S11] C：逐行读文件
来源：http://isl.birdmap.top

FILE *f = fopen("a.txt", "r");
来源：http://lpy.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hsw.jyoumei.cn

fclose(f);
来源：http://vwd.hongshengwenyu.top

[S12] C：写文件
来源：http://zir.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kkw.smart0.xyz

[S13] C：宏定义
来源：http://wqx.jinyuanbaomall.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vjk.yvedp.cn

[S14] C：枚举
来源：http://hlq.ydzc1.top

enum Color { RED, GREEN, BLUE };
来源：http://uko.sweek.top

[S15] C：类型转换
来源：http://baa.jinyuanbaomall.cn

(double) a / b
来源：http://nss.uphjek.com

[S16] C：位操作置位
来源：http://cbh.xuetiantiany.cn

x |= (1 << 3);
来源：http://zfr.fanxiaobao.xyz

[S17] C：安全拼接字符串
来源：http://okn.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hpt.sufxvd.cn

[S18] C：命令行参数
来源：http://gbm.yvedp.cn

int main(int argc, char **argv)
来源：http://fug.yonumen.top

[S19] C：快速排序
来源：http://ruh.guannengcc.top

qsort(a, n, sizeof(int), cmp);
来源：http://lqd.aizwys.cn

[S20] C：二分查找
来源：http://hij.ywan-chungtsiang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xvk.chenzaomai.com

[S21] C：字符类别判断
来源：http://rgt.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ouo.yj20258888.top

[S22] C：字符串转数字
来源：http://qbm.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://cdi.wangshuangyany.cn

[S23] C：随机数
来源：http://lbs.gogol.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qxo.jqgfzy.top

[S24] C：获取本地时间
来源：http://osj.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rzf.hnxiangtu.top

[S25] C：内存拷贝
来源：http://kwc.nwbrower.top

memcpy(dst, src, n);
来源：http://tbt.tarul.cn

[S26] C：内存清零
来源：http://mai.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://sqy.hnxiangtu.top

[S27] C：定义常量
来源：http://dbw.chenlongwang.top

const double PI = 3.14159;
来源：http://yom.daria6918.cn

[S28] C：静态变量
来源：http://ddm.xylfe.cn

static int counter = 0;
来源：http://ffm.nwbrower.top

[S29] C：变参函数
来源：http://obw.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://thf.hfpthk.cn

[S30] C：头文件保护
来源：http://fwy.chenjidiqi.icu

#ifndef X_H
来源：http://zny.jyoumei.cn

#define X_H
来源：http://umd.fanxiaobao.xyz

#endif
来源：http://xai.fengsongda.top

[S31] C++：Hello World
来源：http://pwa.zhoulong.xyz

#include <iostream>
来源：http://pjq.vqdsnc.cn

int main() { std::cout << "Hello\n"; }
来源：http://kxp.hammf.cn

[S32] C++：字符串
来源：http://ptp.redwolf501.top

std::string s = "hi";  s += "!";
来源：http://zvj.yvedp.cn

[S33] C++：vector 增删
来源：http://dlh.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wte.feifeiyinyue.top

[S34] C++：遍历 vector
来源：http://evt.guowangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://mfn.yanxiufei.cn

[S35] C++：map
来源：http://yaz.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yog.ybcxt.top

[S36] C++：unordered_map
来源：http://zdq.jiagoushi.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://khf.xziqi.cn

[S37] C++：set
来源：http://par.chenlongwang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wmb.cheryme.top

[S38] C++：排序
来源：http://rhh.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://ooe.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://ucg.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xhb.yj20258888.top

[S40] C++：查找元素
来源：http://yqa.gotoacloud.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iil.guowangkeji.top

[S41] C++：类与构造函数
来源：http://mrx.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vjk.yfazqb.com

[S42] C++：继承与虚函数
来源：http://nbn.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://zjr.jianghu66.top

[S43] C++：智能指针
来源：http://dvy.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://lxt.jiagoushi.top

[S44] C++：引用传参
来源：http://ujp.gotoacloud.top

void inc(int &x) { ++x; }
来源：http://dbw.jianghu66.top

[S45] C++：lambda
来源：http://rix.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://kqf.iojbl.cn

[S46] C++：函数模板
来源：http://ykj.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://arg.jqgfzy.top

[S47] C++：结构化绑定遍历
来源：http://dcy.epnwcf.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://daa.tarul.cn

[S48] C++：逐行读文件
来源：http://kxs.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://kpb.fktsv.cn

while (std::getline(in, line)) { }
来源：http://wvs.jinghuilouyu.cn

[S49] C++：写文件
来源：http://dhx.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hjq.zhijiandao.cn

[S50] C++：格式化数字
来源：http://qft.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://twh.zhongyouzk.top

[S51] C++：显式类型转换
来源：http://ajk.yfazqb.com

static_cast<double>(a) / b
来源：http://vdd.zhixingplan.top

[S52] C++：const 与 noexcept
来源：http://fmp.vehdjk.com

int size() const noexcept { return n_; }
来源：http://lbh.yongpay.top

[S53] C++：移动语义
来源：http://lwv.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://etx.ydzc1.top

[S54] C++：异常处理
来源：http://wav.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hpc.cucudq.cn

[S55] C++：结构化绑定
来源：http://mfv.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://zzb.cdnleiting.top

[S56] C++：optional
来源：http://ujs.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://edz.jyoumei.cn

[S57] C++：编译期常量
来源：http://mjh.nanxuanxn.top

constexpr int N = 10;
来源：http://bcd.gzhubu.top

[S58] C++：命名空间
来源：http://tgy.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://nmm.bjfxy.top

[S59] C++：静态断言
来源：http://thu.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fxy.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://noq.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://buv.yueranfly.top

================================================================================
来源：http://jza.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rxn.hywenlv.cn

================================================================================
来源：http://lnz.zhaomingkeji.xyz

[T01] Kotlin：Hello World
来源：http://ikp.chenzaomai.com

println("Hello")
来源：http://yjt.birdmap.top

[T02] Kotlin：变量
来源：http://gcv.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mis.svipenyu.cn

[T03] Kotlin：字符串模板
来源：http://psb.jqgfzy.top

"值: $b"
来源：http://xra.yfazqb.com

[T04] Kotlin：空安全
来源：http://xsx.cdnleiting.top

val n: String? = null;  n?.length
来源：http://xic.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://qji.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mcj.guowangkeji.top

[T06] Kotlin：集合映射
来源：http://dnr.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ank.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://isy.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kia.snrcjt.cn

[T08] Kotlin：数据类
来源：http://xyk.gaohongyu789.top

data class User(val name: String, val age: Int)
来源：http://kvu.zycfv.cn

[T09] Kotlin：扩展函数
来源：http://zjd.yj20258.top

fun String.exclaim() = this + "!"
来源：http://ixq.shuidangran.top

[T10] Kotlin：默认参数
来源：http://vyx.pengpengdd.cyou

fun greet(name: String = "World") = "Hi $name"
来源：http://kju.hongshengwenyu.top

[T11] Kotlin：协程
来源：http://hkg.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sah.hongshengwenyu.top

[T12] Kotlin：解构声明
来源：http://pcm.havefunace.top

val (a, b) = Pair(1, 2)
来源：http://enu.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://kho.redwolf501.top

val m = mapOf("a" to 1)
来源：http://exa.cheryme.top

[T14] Kotlin：循环
来源：http://gfw.sjlbkw.cn

for (i in 1..10) println(i)
来源：http://ihu.9152youxi.cn

[T15] Kotlin：接口
来源：http://qfn.guannengcc.top

interface Shape { fun area(): Double }
来源：http://xvs.shuidangran.top

[T16] Swift：Hello World
来源：http://sms.zhoulong.xyz

print("Hello")
来源：http://ydx.hysaishi.cn

[T17] Swift：变量与常量
来源：http://hql.shuidangran.top

var a = 1;  let b = 2
来源：http://mmx.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://xge.shuidangran.top

"值: \(b)"
来源：http://ooe.yueranfly.top

[T19] Swift：可选绑定
来源：http://qbh.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://ziz.zycfv.cn

[T20] Swift：数组操作
来源：http://dos.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://ywd.yj20258.top

[T21] Swift：遍历
来源：http://rhp.nwbrower.top

for x in a { print(x) }
来源：http://ycs.xylfe.cn

[T22] Swift：字典
来源：http://qwl.birdmap.top

var d = ["a": 1];  d["b"] = 2
来源：http://jks.shanyushiyangkeji.top

[T23] Swift：函数
来源：http://lee.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wvd.gotoacloud.top

[T24] Swift：闭包
来源：http://fyu.fzhhl.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kia.cashguo.top

[T25] Swift：结构体
来源：http://ulm.sysykeji.top

struct P { var x: Int }
来源：http://frq.vehdjk.com

[T26] Swift：类与重写
来源：http://kng.fzhhl.top

class A: Base { override func f() {} }
来源：http://vtb.tanke756.top

[T27] Swift：错误处理
来源：http://kad.sjlbkw.cn

do { try f() } catch { print(error) }
来源：http://lfj.zhaomingkeji.xyz

[T28] Swift：枚举
来源：http://mru.hnxiangtu.top

enum Color { case red, green }
来源：http://mch.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://wlk.svipenyu.cn

guard let x = opt else { return }
来源：http://xwb.jinqigfzy.top

[T30] Swift：协议
来源：http://qdx.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://qbi.feifeiyinyue.top

[T31] Lua：Hello World
来源：http://hfb.fanxiaobao.xyz

print("Hello")
来源：http://czj.iojbl.cn

[T32] Lua：局部变量
来源：http://zbj.guowangkeji.top

local a = 1
来源：http://lgj.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://hia.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mgw.smart0.xyz

[T34] Lua：遍历表
来源：http://dfs.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ioj.yuanzhike.top

[T35] Lua：字典表
来源：http://tdo.cashguo.top

local d = { a = 1 };  d.b = 2
来源：http://son.hnqzz.top

[T36] Lua：函数
来源：http://ool.c1oappe.top

function add(a, b) return a + b end
来源：http://ilp.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://ybe.smart0.xyz

"a" .. "b"
来源：http://cni.sufxvd.cn

[T38] Lua：条件
来源：http://uyo.zhixingplan.top

if x > 0 then print("正") end
来源：http://wfk.jiagoushi.top

[T39] Lua：模式匹配
来源：http://zev.yuxming.cn

string.find(s, "%d+")
来源：http://byh.fzhhl.top

[T40] Lua：元表
来源：http://hfg.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://omk.aibaodan.cn

[T41] Perl：Hello World
来源：http://liv.guannengcc.top

print "Hello\n";
来源：http://ecq.nanxinkj.top

[T42] Perl：变量类型
来源：http://vhh.zdbjq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pfc.gzhubu.top

[T43] Perl：字符串插值
来源：http://gsr.shangyingyoupin.top

"值: $a"
来源：http://jqz.havefunace.top

[T44] Perl：条件
来源：http://iiw.cheryme.top

if ($a > 0) { print "正"; }
来源：http://wgd.yuanzhike.top

[T45] Perl：数组遍历
来源：http://xmu.jyoumei.cn

for my $x (@arr) { print $x; }
来源：http://wei.tian-w.cn

[T46] Perl：哈希操作
来源：http://mhx.316326.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://opl.ydjk.org.cn

[T47] Perl：正则捕获
来源：http://dig.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://ovb.jinqigfzy.top

[T48] Perl：正则替换
来源：http://kej.daria6918.cn

$s =~ s/old/new/g;
来源：http://kbu.yongpay.top

[T49] Perl：函数
来源：http://omd.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sip.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://vwn.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://hje.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://bhf.uphjek.com

[T51] Scala：Hello World
来源：http://eiu.cdnleiting.top

println("Hello")
来源：http://rdg.wangdashe.top

[T52] Scala：变量
来源：http://hyb.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://hht.yonumen.top

[T53] Scala：字符串插值
来源：http://ldn.sxryk.cn

s"值: $b"
来源：http://exj.yfazqb.com

[T54] Scala：集合映射
来源：http://omv.ydzc1.top

List(1, 2, 3).map(_ * 2)
来源：http://grw.xinyue.icu

[T55] Scala：集合过滤
来源：http://tdq.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://ecn.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://ksh.redwolf501.top

case class User(name: String, age: Int)
来源：http://oye.yuanzhike.top

[T57] Scala：模式匹配
来源：http://puo.0kj1m.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://osv.jyoumei.cn

[T58] Scala：函数定义
来源：http://znn.xingfuxueyuan.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://sdj.wangshuangyany.cn

[T59] Scala：循环
来源：http://fvo.cheryme.top

for (i <- 1 to 10) println(i)
来源：http://uja.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://vuu.aibaodan.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dla.nanxuanxn.top

================================================================================
来源：http://uyp.shanyushiyangtech.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wmi.c1oappe.top

================================================================================
来源：http://ynp.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://xda.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tqb.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://cmw.zhengqikj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hhe.ybcxt.top

[U03] Py：加载 .env 配置
来源：http://dcz.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ezj.redwolf501.top

[U04] Py：变量调试打印
来源：http://tst.yueranfly.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://alw.xuetiantiany.cn

[U05] Py：列表去重且保序
来源：http://hbt.ehwqpu.com

list(dict.fromkeys(arr))
来源：http://hxh.hysaishi.cn

[U06] Py：合并两个字典
来源：http://mkv.dashuyun.cn

{**a, **b}
来源：http://xrn.yangfankeji.com

[U07] Py：反转字典键值
来源：http://rmh.epnwcf.com

{v: k for k, v in d.items()}
来源：http://xez.cucudq.cn

[U08] Py：展平二维列表
来源：http://fqy.jinqigfzy.top

[y for x in nested for y in x]
来源：http://yqf.epnwcf.com

[U09] Py：字典取最大值的键
来源：http://qxa.zhongyouzk.top

max(d, key=d.get)
来源：http://dez.ehwqpu.com

[U10] Py：按值排序字典
来源：http://meu.redwolf501.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://awt.svipenyu.cn

[U11] Py：生成器表达式
来源：http://lud.yuanzhike.top

(x * 2 for x in arr)
来源：http://unq.hnqzz.top

[U12] Py：取出现最多的 3 个元素
来源：http://ibt.jyoumei.cn

Counter(arr).most_common(3)
来源：http://plj.jqgfzy.top

[U13] Py：固定长度队列
来源：http://hyp.sufxvd.cn

deque(maxlen=10)
来源：http://bje.kuanghao11.cn

[U14] Py：分组收集到列表
来源：http://uio.bbcook.cn

defaultdict(list)
来源：http://weq.chenlongwang.top

[U15] Py：高精度计时
来源：http://hxi.wangshuangyany.cn

t = time.perf_counter()
来源：http://kap.quarkkingdee.top

[U16] Py：命令行参数解析
来源：http://wwu.mhx1999.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ovh.shanyushiyangtech.top

[U17] Py：初始化日志
来源：http://aua.cashguo.top

logging.basicConfig(level=logging.INFO)
来源：http://hnm.316326.xyz

[U18] Py：预编译正则
来源：http://sus.yj202588.top

pat = re.compile(r"\d+")
来源：http://yzl.pycfn.com


<!-- 参考信息 -->