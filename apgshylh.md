代发 wailian999

split -l 1000 big.log part_
来源：http://oei.zhoulong.xyz

[R74] 批量重命名
来源：http://qss.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sit.kuanghao11.cn

[R75] 导出环境变量
来源：http://tgf.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://ejr.c1oappe.top

[R76] 使用临时文件
来源：http://hwj.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nrc.fzhhl.top

[R77] 读取用户输入
来源：http://tdw.yanxiufei.cn

read -rp "请输入: " ans
来源：http://tjx.xuanzx.com

[R78] 交互式菜单
来源：http://fbg.zhijiandao.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nsg.jinqigfzy.top

[R79] 解析命令行选项
来源：http://rfc.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rep.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://odc.jqgfzy.top

time ./run.sh
来源：http://uqm.jinghuilouyu.cn

================================================================================
来源：http://smh.cqqwz.cn

S. C / C++ 专题
来源：http://ona.c1oappe.top

================================================================================
来源：http://esq.hcnkem.com

[S01] C：Hello World
来源：http://hnx.zhoulong.xyz

#include <stdio.h>
来源：http://xkq.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://rlh.hesvh.cn

[S02] C：变量与格式化输出
来源：http://zcy.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://fut.xylfe.cn

[S03] C：读入整数
来源：http://zsr.jinqigfzy.top

int x; scanf("%d", &x);
来源：http://irc.jiagoushi.top

[S04] C：字符串复制
来源：http://kbw.shanyushiyangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://utn.cashguo.top

[S05] C：字符串长度
来源：http://oqs.zhoulong.xyz

strlen(s)
来源：http://feq.haohaochexian.top

[S06] C：字符串比较
来源：http://lhh.pycfn.com

strcmp(a, b) == 0
来源：http://mvk.zhengqikj.top

[S07] C：数组遍历求和
来源：http://cqu.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://edj.havefunace.top

[S08] C：动态内存分配与释放
来源：http://jmn.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://igw.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://jwb.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hho.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://qbp.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://cet.pengpengdd.cyou

[S11] C：逐行读文件
来源：http://mdb.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://zix.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nae.bjfxy.top

fclose(f);
来源：http://pxl.yj20258.top

[S12] C：写文件
来源：http://vtd.gzhubu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qbg.jqgfzy.top

[S13] C：宏定义
来源：http://mma.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://abn.sweek.top

[S14] C：枚举
来源：http://gaq.jinqigfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://jpe.ehwqpu.com

[S15] C：类型转换
来源：http://wxk.zycfv.cn

(double) a / b
来源：http://klh.jqgufenzy.top

[S16] C：位操作置位
来源：http://brb.nwbrower.top

x |= (1 << 3);
来源：http://uxh.shuidangran.top

[S17] C：安全拼接字符串
来源：http://bke.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fcm.yuanzhike.top

[S18] C：命令行参数
来源：http://kle.wangshuangyany.cn

int main(int argc, char **argv)
来源：http://vet.sysykeji.top

[S19] C：快速排序
来源：http://gig.guowangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://vkw.sufxvd.cn

[S20] C：二分查找
来源：http://gls.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ktp.epnwcf.com

[S21] C：字符类别判断
来源：http://fvj.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rcu.jlsjyb.cn

[S22] C：字符串转数字
来源：http://rgx.yanxiufei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zya.nanxinkj.top

[S23] C：随机数
来源：http://fct.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wps.daria6918.cn

[S24] C：获取本地时间
来源：http://qey.guowangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cku.pycfn.com

[S25] C：内存拷贝
来源：http://xfy.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://cbg.jiagoushi.top

[S26] C：内存清零
来源：http://fhy.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://vte.ydjk.org.cn

[S27] C：定义常量
来源：http://dhq.shzxlz.cn

const double PI = 3.14159;
来源：http://lhn.yj20258888.top

[S28] C：静态变量
来源：http://ctz.jinghuilouyu.cn

static int counter = 0;
来源：http://ggf.yj20258.top

[S29] C：变参函数
来源：http://nru.chenzaomai.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jaw.hcnkem.com

[S30] C：头文件保护
来源：http://vgc.hywenlv.cn

#ifndef X_H
来源：http://gzt.svipenyu.cn

#define X_H
来源：http://aro.c1oappe.top

#endif
来源：http://cxa.aibaodan.cn

[S31] C++：Hello World
来源：http://cus.hysaishi.cn

#include <iostream>
来源：http://lrf.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://jye.jiagoushi.top

[S32] C++：字符串
来源：http://myc.yongpay.top

std::string s = "hi";  s += "!";
来源：http://nqo.yuanzhike.top

[S33] C++：vector 增删
来源：http://xvx.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sfv.daxiang520.top

[S34] C++：遍历 vector
来源：http://xnh.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://iok.fehbvm.com

[S35] C++：map
来源：http://voc.jianghu66.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lvx.xziqi.cn

[S36] C++：unordered_map
来源：http://qqr.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://suq.epnwcf.com

[S37] C++：set
来源：http://aum.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bni.fzhhl.top

[S38] C++：排序
来源：http://qgv.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://pyt.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://hmt.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dsy.wangshuangyany.cn

[S40] C++：查找元素
来源：http://jur.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ryk.pycfn.com

[S41] C++：类与构造函数
来源：http://hzr.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jyt.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://djr.xuanzx.com

class B : public Base { public: void f() override {} };
来源：http://dsw.andypj.xyz

[S43] C++：智能指针
来源：http://iqr.tanke756.top

auto p = std::make_unique<int>(5);
来源：http://wwq.chenzaomai.com

[S44] C++：引用传参
来源：http://adq.hammf.cn

void inc(int &x) { ++x; }
来源：http://smb.dashuyun.cn

[S45] C++：lambda
来源：http://dxs.kuanghao11.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gje.daxiang520.top

[S46] C++：函数模板
来源：http://tzr.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fwt.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://qud.fktsv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ngg.redwolf501.top

[S48] C++：逐行读文件
来源：http://sfw.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mzw.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://rys.hcnkem.com

[S49] C++：写文件
来源：http://vqb.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rvp.yfazqb.com

[S50] C++：格式化数字
来源：http://ful.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rtf.birdmap.top

[S51] C++：显式类型转换
来源：http://ucs.fehbvm.com

static_cast<double>(a) / b
来源：http://syv.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://hoz.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://pgo.zdqjudy.top

[S53] C++：移动语义
来源：http://rbo.tanke756.top

std::vector<int> w = std::move(v);
来源：http://zzo.wangshuangyany.cn

[S54] C++：异常处理
来源：http://eqn.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cdz.yonumen.top

[S55] C++：结构化绑定
来源：http://azj.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://aud.zhijiandao.cn

[S56] C++：optional
来源：http://jwj.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gvw.yj20258.top

[S57] C++：编译期常量
来源：http://sfu.jinqigfzy.top

constexpr int N = 10;
来源：http://jkt.zhixingplan.top

[S58] C++：命名空间
来源：http://clx.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://xzz.vqdsnc.cn

[S59] C++：静态断言
来源：http://qog.xylfe.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rys.sjlbkw.cn

[S60] C++：遍历并删除元素
来源：http://dwp.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kyg.redwolf501.top

================================================================================
来源：http://plf.cqqwz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zco.guannengcc.top

================================================================================
来源：http://tez.tarul.cn

[T01] Kotlin：Hello World
来源：http://ehh.jinqigfzy.top

println("Hello")
来源：http://aod.hammf.cn

[T02] Kotlin：变量
来源：http://bcv.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dsz.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://emz.tianlin.xyz

"值: $b"
来源：http://gjn.chenlongwang.top

[T04] Kotlin：空安全
来源：http://hig.yfazqb.com

val n: String? = null;  n?.length
来源：http://qpp.tarul.cn

[T05] Kotlin：when 表达式
来源：http://dvl.tanke756.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://knf.bbcook.cn

[T06] Kotlin：集合映射
来源：http://maq.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://umu.shuidangran.top

[T07] Kotlin：集合过滤
来源：http://qha.hesvh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mev.svipenyu.cn

[T08] Kotlin：数据类
来源：http://ayj.yj202588.top

data class User(val name: String, val age: Int)
来源：http://xma.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://erf.haohaochexian.top

fun String.exclaim() = this + "!"
来源：http://fww.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://ddi.xuetiantiany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lhw.gaohongyu789.top

[T11] Kotlin：协程
来源：http://hgz.zhixingplan.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://npk.hesvh.cn

[T12] Kotlin：解构声明
来源：http://jvv.mhx1999.top

val (a, b) = Pair(1, 2)
来源：http://jju.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://obf.pycfn.com

val m = mapOf("a" to 1)
来源：http://ane.epnwcf.com

[T14] Kotlin：循环
来源：http://zzu.c1oappe.top

for (i in 1..10) println(i)
来源：http://rad.zhiwuduotai.top

[T15] Kotlin：接口
来源：http://rwx.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://slj.uphjek.com

[T16] Swift：Hello World
来源：http://gfl.andypj.xyz

print("Hello")
来源：http://gwm.zdqjudy.top

[T17] Swift：变量与常量
来源：http://wtg.sjlbkw.cn

var a = 1;  let b = 2
来源：http://shq.cashguo.top

[T18] Swift：字符串插值
来源：http://ati.xylfe.cn

"值: \(b)"
来源：http://zpp.yangfankeji.com

[T19] Swift：可选绑定
来源：http://ybt.zycfv.cn

if let n = opt { print(n) }
来源：http://rvh.jlsjyb.cn

[T20] Swift：数组操作
来源：http://gut.cqqwz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://awf.yonumen.top

[T21] Swift：遍历
来源：http://ugf.zycfv.cn

for x in a { print(x) }
来源：http://rig.zhoulong.xyz

[T22] Swift：字典
来源：http://xri.shuidangran.top

var d = ["a": 1];  d["b"] = 2
来源：http://uxo.mhx1999.top

[T23] Swift：函数
来源：http://gmx.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://guk.shzxlz.cn

[T24] Swift：闭包
来源：http://ura.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bkf.yfazqb.com

[T25] Swift：结构体
来源：http://czs.yfazqb.com

struct P { var x: Int }
来源：http://xul.shanyushiyangtech.top

[T26] Swift：类与重写
来源：http://sxf.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://wak.bbcook.cn

[T27] Swift：错误处理
来源：http://lbx.yvedp.cn

do { try f() } catch { print(error) }
来源：http://pdt.yj20258.top

[T28] Swift：枚举
来源：http://bzu.fengsongda.top

enum Color { case red, green }
来源：http://sok.chenjidiqi.icu

[T29] Swift：guard 提前返回
来源：http://tke.dianchejie.cn

guard let x = opt else { return }
来源：http://hys.ydzc1.top

[T30] Swift：协议
来源：http://xzv.guowangkeji.top

protocol Shape { func area() -> Double }
来源：http://hbs.jqgfzy.top

[T31] Lua：Hello World
来源：http://avs.pycfn.com

print("Hello")
来源：http://mxy.andypj.xyz

[T32] Lua：局部变量
来源：http://cbr.hywenlv.cn

local a = 1
来源：http://sfw.pengpengdd.cyou

[T33] Lua：表（数组）
来源：http://aix.jlsjyb.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oke.shuidangran.top

[T34] Lua：遍历表
来源：http://otq.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wlx.jqgufenzy.top

[T35] Lua：字典表
来源：http://cgd.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://aha.daria6918.cn

[T36] Lua：函数
来源：http://yxy.yj20258.top

function add(a, b) return a + b end
来源：http://mjg.sxryk.cn

[T37] Lua：字符串拼接
来源：http://lsq.redwolf501.top

"a" .. "b"
来源：http://mfv.guannengcc.top

[T38] Lua：条件
来源：http://qmn.zhengqikj.top

if x > 0 then print("正") end
来源：http://lbz.yfazqb.com

[T39] Lua：模式匹配
来源：http://zds.ppjwa.cn

string.find(s, "%d+")
来源：http://xax.xinyue.icu

[T40] Lua：元表
来源：http://uan.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://sgr.dianchejie.cn

[T41] Perl：Hello World
来源：http://xtj.daxiang520.top

print "Hello\n";
来源：http://kmp.redwolf501.top

[T42] Perl：变量类型
来源：http://hrk.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rho.pengpengdd.cyou

[T43] Perl：字符串插值
来源：http://zzw.jiagoushi.top

"值: $a"
来源：http://njl.yfazqb.com

[T44] Perl：条件
来源：http://hcy.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://jez.tanke756.top

[T45] Perl：数组遍历
来源：http://tth.gogol.net.cn

for my $x (@arr) { print $x; }
来源：http://oxu.tarul.cn

[T46] Perl：哈希操作
来源：http://ipj.jqgufenzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yyg.havefunace.top

[T47] Perl：正则捕获
来源：http://svy.ehwqpu.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://edd.yvedp.cn

[T48] Perl：正则替换
来源：http://azk.cashguo.top

$s =~ s/old/new/g;
来源：http://yuo.zhaomingkeji.xyz

[T49] Perl：函数
来源：http://shv.yj20258.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zms.9152youxi.cn

[T50] Perl：逐行读文件
来源：http://hpg.hnxiangtu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nvi.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://atz.yvedp.cn

[T51] Scala：Hello World
来源：http://ghc.jinqigfzy.top

println("Hello")
来源：http://fte.hfpthk.cn

[T52] Scala：变量
来源：http://rnw.zhiwuduotai.top

val a = 1;  var b = 2
来源：http://uqu.dianchejie.cn

[T53] Scala：字符串插值
来源：http://yhd.xylfe.cn

s"值: $b"
来源：http://urx.wangshuangyany.cn

[T54] Scala：集合映射
来源：http://hts.dashuyun.cn

List(1, 2, 3).map(_ * 2)
来源：http://gug.gotoacloud.top

[T55] Scala：集合过滤
来源：http://wjk.snrcjt.cn

List(1, 2, 3).filter(_ > 1)
来源：http://aog.svipenyu.cn

[T56] Scala：样例类
来源：http://wgf.ydjk.org.cn

case class User(name: String, age: Int)
来源：http://jjq.shzxlz.cn

[T57] Scala：模式匹配
来源：http://urt.birdmap.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://esb.cucudq.cn

[T58] Scala：函数定义
来源：http://nwa.gzhubu.top

def add(a: Int, b: Int): Int = a + b
来源：http://xqq.gaohongyu789.top

[T59] Scala：循环
来源：http://uxy.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://yby.gzhubu.top

[T60] Scala：折叠
来源：http://crm.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ams.andypj.xyz

================================================================================
来源：http://wgp.wangdashe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://akj.zhongyouzk.top

================================================================================
来源：http://vpt.quarkkingdee.top

[U01] Py：创建虚拟环境
来源：http://xfw.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://jqa.vehdjk.com

[U02] Py：导出 / 安装依赖
来源：http://xan.daxiang520.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fix.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://vdc.ywan-chungtsiang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jpn.hfpthk.cn

[U04] Py：变量调试打印
来源：http://xbb.jianghu66.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ilu.yvedp.cn

[U05] Py：列表去重且保序
来源：http://flo.andypj.xyz

list(dict.fromkeys(arr))
来源：http://gua.epnwcf.com

[U06] Py：合并两个字典
来源：http://tyu.hongshengwenyu.top

{**a, **b}
来源：http://xgi.meibo888.top

[U07] Py：反转字典键值
来源：http://nkb.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://mjj.52xcode.cn

[U08] Py：展平二维列表
来源：http://iop.jqgfzy.top

[y for x in nested for y in x]
来源：http://yit.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://iew.jlsjyb.cn

max(d, key=d.get)
来源：http://bjs.iojbl.cn

[U10] Py：按值排序字典
来源：http://wxm.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jvx.meibo888.top

[U11] Py：生成器表达式
来源：http://xej.yuxming.cn

(x * 2 for x in arr)
来源：http://cyu.zhaomingkeji.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://ohr.hfpthk.cn

Counter(arr).most_common(3)
来源：http://icj.fanxiaobao.xyz

[U13] Py：固定长度队列
来源：http://lxc.52xcode.cn

deque(maxlen=10)
来源：http://epb.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://dta.dashuyun.cn

defaultdict(list)
来源：http://fva.xylfe.cn


<!-- 参考信息 -->