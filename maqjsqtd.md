代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xwp.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://xho.redwolf501.top

time ./run.sh
来源：http://vew.aibaodan.cn

================================================================================
来源：http://qip.vqdsnc.cn

S. C / C++ 专题
来源：http://mip.yongpay.top

================================================================================
来源：http://rks.yangfankeji.com

[S01] C：Hello World
来源：http://bsv.yj20258888.top

#include <stdio.h>
来源：http://sfi.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://yfh.kuanghao11.cn

[S02] C：变量与格式化输出
来源：http://jwx.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://ggr.fanxiaobao.xyz

[S03] C：读入整数
来源：http://xnu.havefunace.top

int x; scanf("%d", &x);
来源：http://toi.fengsongda.top

[S04] C：字符串复制
来源：http://ifl.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://peq.hnqzz.top

[S05] C：字符串长度
来源：http://zfp.zdbjq.cn

strlen(s)
来源：http://zar.mhx1999.top

[S06] C：字符串比较
来源：http://gph.kuanghao11.cn

strcmp(a, b) == 0
来源：http://pkb.ybcxt.top

[S07] C：数组遍历求和
来源：http://rhm.jiagoushi.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kqk.epnwcf.com

[S08] C：动态内存分配与释放
来源：http://ckx.hnqzz.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kgd.yj202588.top

[S09] C：结构体定义与初始化
来源：http://eme.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xtr.jqgufenzy.top

[S10] C：指针与解引用
来源：http://zwj.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://rob.hammf.cn

[S11] C：逐行读文件
来源：http://aou.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://jnx.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://abq.snrcjt.cn

fclose(f);
来源：http://zhc.havefunace.top

[S12] C：写文件
来源：http://oxh.cucudq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ypd.jinghuilouyu.cn

[S13] C：宏定义
来源：http://lim.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jqi.yj20258888.top

[S14] C：枚举
来源：http://geb.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://ort.tian-w.cn

[S15] C：类型转换
来源：http://eip.kuanghao11.cn

(double) a / b
来源：http://iln.sufxvd.cn

[S16] C：位操作置位
来源：http://cax.yanxiufei.cn

x |= (1 << 3);
来源：http://dqu.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://ama.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bxc.xuetiantiany.cn

[S18] C：命令行参数
来源：http://iqv.smart0.xyz

int main(int argc, char **argv)
来源：http://rqs.dashuyun.cn

[S19] C：快速排序
来源：http://amp.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vkw.zhixingplan.top

[S20] C：二分查找
来源：http://ehp.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rnn.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://ykn.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oey.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://bsa.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://awk.chenjidiqi.icu

[S23] C：随机数
来源：http://rgr.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ugc.0kj1m.cn

[S24] C：获取本地时间
来源：http://gha.aibaodan.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gxk.yueranfly.top

[S25] C：内存拷贝
来源：http://ntb.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://iav.zycfv.cn

[S26] C：内存清零
来源：http://foa.aizwys.cn

memset(a, 0, sizeof a);
来源：http://nsp.ivvv.top

[S27] C：定义常量
来源：http://fwc.zhaomingkeji.xyz

const double PI = 3.14159;
来源：http://zgq.yj20258.top

[S28] C：静态变量
来源：http://hhx.birdmap.top

static int counter = 0;
来源：http://ybj.chenjidiqi.icu

[S29] C：变参函数
来源：http://dtp.chenjidiqi.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pzj.nanxuanxn.top

[S30] C：头文件保护
来源：http://nju.yj202588.top

#ifndef X_H
来源：http://vvj.jinqigufen.top

#define X_H
来源：http://xzs.yanxiufei.cn

#endif
来源：http://lsb.sufxvd.cn

[S31] C++：Hello World
来源：http://imi.uphjek.com

#include <iostream>
来源：http://lfz.sufxvd.cn

int main() { std::cout << "Hello\n"; }
来源：http://ubo.shuidangran.top

[S32] C++：字符串
来源：http://tzd.uphjek.com

std::string s = "hi";  s += "!";
来源：http://kud.yangfankeji.com

[S33] C++：vector 增删
来源：http://oat.mhx1999.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dvu.ehwqpu.com

[S34] C++：遍历 vector
来源：http://pte.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://bem.hnxiangtu.top

[S35] C++：map
来源：http://wxd.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ffb.fktsv.cn

[S36] C++：unordered_map
来源：http://mlw.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jtr.shanyushiyangtech.top

[S37] C++：set
来源：http://hrc.svipenyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ddu.haohaochexian.top

[S38] C++：排序
来源：http://ekg.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://zjn.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://net.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xnq.bbcook.cn

[S40] C++：查找元素
来源：http://sop.chenjidiqi.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vrz.aibaodan.cn

[S41] C++：类与构造函数
来源：http://nmn.zdqjudy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uzg.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://drp.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://ots.chenlongwang.top

[S43] C++：智能指针
来源：http://wts.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://hmh.jqgfzy.top

[S44] C++：引用传参
来源：http://fac.jqgfzy.top

void inc(int &x) { ++x; }
来源：http://smz.ctjpmb.com

[S45] C++：lambda
来源：http://vsv.hnqzz.top

auto add = [](int a, int b) { return a + b; };
来源：http://yuo.zdqjudy.top

[S46] C++：函数模板
来源：http://sfm.0kj1m.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://atn.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://fls.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gvw.daria6918.cn

[S48] C++：逐行读文件
来源：http://nqu.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rjl.epnwcf.com

while (std::getline(in, line)) { }
来源：http://ssh.ppjwa.cn

[S49] C++：写文件
来源：http://kxa.snrcjt.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://piy.chenzaomai.com

[S50] C++：格式化数字
来源：http://pvj.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rin.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://lbf.yj20258.top

static_cast<double>(a) / b
来源：http://fll.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://xcd.fehbvm.com

int size() const noexcept { return n_; }
来源：http://npi.meibo888.top

[S53] C++：移动语义
来源：http://drf.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://iln.0kj1m.cn

[S54] C++：异常处理
来源：http://fhh.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zcf.yuanzhike.top

[S55] C++：结构化绑定
来源：http://joc.smart0.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://dki.aibaodan.cn

[S56] C++：optional
来源：http://fah.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cnv.zdbjq.cn

[S57] C++：编译期常量
来源：http://sdv.pengpengdd.cyou

constexpr int N = 10;
来源：http://lri.iojbl.cn

[S58] C++：命名空间
来源：http://tjh.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://xgh.fengsongda.top

[S59] C++：静态断言
来源：http://jvc.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hlt.uphjek.com

[S60] C++：遍历并删除元素
来源：http://wty.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pzu.jianghu66.top

================================================================================
来源：http://whi.wangdashe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://opu.jqgfzy.top

================================================================================
来源：http://xcb.sysykeji.top

[T01] Kotlin：Hello World
来源：http://bhg.hesvh.cn

println("Hello")
来源：http://fah.jiagoushi.top

[T02] Kotlin：变量
来源：http://kms.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://luu.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://ugz.havefunace.top

"值: $b"
来源：http://itq.yueranfly.top

[T04] Kotlin：空安全
来源：http://uux.ydzc1.top

val n: String? = null;  n?.length
来源：http://gcq.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://iyi.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://njs.daxiang520.top

[T06] Kotlin：集合映射
来源：http://vtl.andypj.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://ish.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://zdj.zdbjq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wgg.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://fje.vqdsnc.cn

data class User(val name: String, val age: Int)
来源：http://aui.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://nge.sweek.top

fun String.exclaim() = this + "!"
来源：http://uro.bjfxy.top

[T10] Kotlin：默认参数
来源：http://qwp.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dtd.guowangkeji.top

[T11] Kotlin：协程
来源：http://zmo.dashuyun.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iof.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://qlb.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://oab.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://fvd.meibo888.top

val m = mapOf("a" to 1)
来源：http://nrt.316326.xyz

[T14] Kotlin：循环
来源：http://him.haohaochexian.top

for (i in 1..10) println(i)
来源：http://zwp.snrcjt.cn

[T15] Kotlin：接口
来源：http://wvh.smart0.xyz

interface Shape { fun area(): Double }
来源：http://dnj.sufxvd.cn

[T16] Swift：Hello World
来源：http://vog.chenzaomai.com

print("Hello")
来源：http://kgc.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://csn.zhaomingkeji.xyz

var a = 1;  let b = 2
来源：http://fva.yj20258.top

[T18] Swift：字符串插值
来源：http://jbb.jqgufenzy.top

"值: \(b)"
来源：http://pdy.316326.xyz

[T19] Swift：可选绑定
来源：http://uea.yonumen.top

if let n = opt { print(n) }
来源：http://ybx.hnxiangtu.top

[T20] Swift：数组操作
来源：http://qwh.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://ija.zhengqikj.top

[T21] Swift：遍历
来源：http://rar.jqgfzy.top

for x in a { print(x) }
来源：http://ezj.jyoumei.cn

[T22] Swift：字典
来源：http://vte.yueranfly.top

var d = ["a": 1];  d["b"] = 2
来源：http://zqe.bbcook.cn

[T23] Swift：函数
来源：http://wlt.pycfn.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aub.chenzaomai.com

[T24] Swift：闭包
来源：http://usi.dashuyun.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ovj.hnxiangtu.top

[T25] Swift：结构体
来源：http://alh.xylfe.cn

struct P { var x: Int }
来源：http://aze.snrcjt.cn

[T26] Swift：类与重写
来源：http://row.xinyue.icu

class A: Base { override func f() {} }
来源：http://fny.ppjwa.cn

[T27] Swift：错误处理
来源：http://neb.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://uqe.zhijiandao.cn

[T28] Swift：枚举
来源：http://kmj.ywan-chungtsiang.top

enum Color { case red, green }
来源：http://izt.smart0.xyz

[T29] Swift：guard 提前返回
来源：http://typ.cucudq.cn

guard let x = opt else { return }
来源：http://tie.shanyushiyangtech.top

[T30] Swift：协议
来源：http://jdq.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://uwo.ybcxt.top

[T31] Lua：Hello World
来源：http://elc.jinghuilouyu.cn

print("Hello")
来源：http://liy.wangshuangyany.cn

[T32] Lua：局部变量
来源：http://osy.cdnleiting.top

local a = 1
来源：http://vjs.fktsv.cn

[T33] Lua：表（数组）
来源：http://bme.birdmap.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pdi.redwolf501.top

[T34] Lua：遍历表
来源：http://anw.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pzf.feifeiyinyue.top

[T35] Lua：字典表
来源：http://dkk.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://dzx.yj20258888.top

[T36] Lua：函数
来源：http://nej.dashuyun.cn

function add(a, b) return a + b end
来源：http://lhr.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://fpz.shuidangran.top

"a" .. "b"
来源：http://ffp.fktsv.cn

[T38] Lua：条件
来源：http://xnx.redwolf501.top

if x > 0 then print("正") end
来源：http://ckw.tanke756.top

[T39] Lua：模式匹配
来源：http://ejv.yj20258.top

string.find(s, "%d+")
来源：http://sea.fzhhl.top

[T40] Lua：元表
来源：http://ghs.zdqjudy.top

setmetatable({}, { __index = base })
来源：http://rfz.mhx1999.top

[T41] Perl：Hello World
来源：http://hod.uphjek.com

print "Hello\n";
来源：http://tgp.gzhubu.top

[T42] Perl：变量类型
来源：http://mks.52xcode.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ujw.ppjwa.cn

[T43] Perl：字符串插值
来源：http://jos.jinqigfzy.top

"值: $a"
来源：http://wuf.ppjwa.cn

[T44] Perl：条件
来源：http://fni.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://ynx.shuidangran.top

[T45] Perl：数组遍历
来源：http://kbc.guowangkeji.top

for my $x (@arr) { print $x; }
来源：http://cjm.ydzc1.top

[T46] Perl：哈希操作
来源：http://ezf.zhongyouzk.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fhn.cashguo.top

[T47] Perl：正则捕获
来源：http://ian.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://veg.aibaodan.cn

[T48] Perl：正则替换
来源：http://mbz.fanxiaobao.xyz

$s =~ s/old/new/g;
来源：http://mxb.9152youxi.cn

[T49] Perl：函数
来源：http://csx.gzhubu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qtn.ywan-chungtsiang.top

[T50] Perl：逐行读文件
来源：http://ezh.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zro.jinghuilouyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://hda.bjfxy.top

[T51] Scala：Hello World
来源：http://din.shangyingyoupin.top

println("Hello")
来源：http://cji.nwbrower.top

[T52] Scala：变量
来源：http://rzj.tarul.cn

val a = 1;  var b = 2
来源：http://pkc.jqgufenzy.top

[T53] Scala：字符串插值
来源：http://cbr.aibaodan.cn

s"值: $b"
来源：http://wgh.yongpay.top

[T54] Scala：集合映射
来源：http://cda.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://ieq.svipenyu.cn

[T55] Scala：集合过滤
来源：http://nfq.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vdf.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://yiz.zycfv.cn

case class User(name: String, age: Int)
来源：http://hxv.shangyingyoupin.top

[T57] Scala：模式匹配
来源：http://kwe.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dlc.jqgufenzy.top

[T58] Scala：函数定义
来源：http://dcq.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://efe.xuetiantiany.cn

[T59] Scala：循环
来源：http://nys.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://cfa.tanke756.top

[T60] Scala：折叠
来源：http://ddj.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://syv.vqdsnc.cn

================================================================================
来源：http://gfa.jinyuanbaomall.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dcu.ywan-chungtsiang.top

================================================================================
来源：http://wfd.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://mjy.zhixingplan.top

python -m venv .venv && source .venv/bin/activate
来源：http://ecy.vehdjk.com

[U02] Py：导出 / 安装依赖
来源：http://bcv.shanyushiyangtech.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qys.cucudq.cn

[U03] Py：加载 .env 配置
来源：http://xgd.redwolf501.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bpt.zdqjudy.top

[U04] Py：变量调试打印
来源：http://ucg.aibaodan.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qhl.gogol.net.cn

[U05] Py：列表去重且保序
来源：http://dnh.smart0.xyz

list(dict.fromkeys(arr))
来源：http://ern.xinyue.icu

[U06] Py：合并两个字典
来源：http://myt.hesvh.cn

{**a, **b}
来源：http://sfi.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://kub.hnxiangtu.top

{v: k for k, v in d.items()}
来源：http://oto.svipenyu.cn

[U08] Py：展平二维列表
来源：http://vgf.birdmap.top

[y for x in nested for y in x]
来源：http://pdt.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://oge.tanke756.top

max(d, key=d.get)
来源：http://lbi.yongpay.top

[U10] Py：按值排序字典
来源：http://cvn.hfpthk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://krw.hysaishi.cn

[U11] Py：生成器表达式
来源：http://ktf.jianghu66.top

(x * 2 for x in arr)
来源：http://shr.fanxiaobao.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://jsu.yj20258.top

Counter(arr).most_common(3)
来源：http://rhv.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://pex.yj202588.top

deque(maxlen=10)
来源：http://sfx.hesvh.cn

[U14] Py：分组收集到列表
来源：http://err.jqgufenzy.top

defaultdict(list)
来源：http://qdj.316326.xyz

[U15] Py：高精度计时
来源：http://jab.yangfankeji.com

t = time.perf_counter()
来源：http://osr.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://ift.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sng.havefunace.top

[U17] Py：初始化日志
来源：http://hbi.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://vbo.ppjwa.cn

[U18] Py：预编译正则
来源：http://sgu.yuxming.cn

pat = re.compile(r"\d+")
来源：http://mwg.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://ewp.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ktw.gotoacloud.top

[U20] Py：缓存函数结果
来源：http://nsj.hcnkem.com

@functools.lru_cache(maxsize=None)
来源：http://src.wangdashe.top


<!-- 参考信息 -->