代发 wailian999

read -rp "请输入: " ans
来源：http://lxe.gzhubu.top

[R78] 交互式菜单
来源：http://atn.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://inf.quarkkingdee.top

[R79] 解析命令行选项
来源：http://pjx.ivvv.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rcc.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://xtu.nanxinkj.top

time ./run.sh
来源：http://qsd.jinghuilouyu.cn

================================================================================
来源：http://orq.zhijiandao.cn

S. C / C++ 专题
来源：http://qdk.birdmap.top

================================================================================
来源：http://yqp.sweek.top

[S01] C：Hello World
来源：http://dku.pengpengdd.cyou

#include <stdio.h>
来源：http://vra.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jfi.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://fgc.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://mdo.bjfxy.top

[S03] C：读入整数
来源：http://psz.zdbjq.cn

int x; scanf("%d", &x);
来源：http://srb.havefunace.top

[S04] C：字符串复制
来源：http://oor.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sli.xuetiantiany.cn

[S05] C：字符串长度
来源：http://tqu.xziqi.cn

strlen(s)
来源：http://lmh.yueranfly.top

[S06] C：字符串比较
来源：http://lao.zdbjq.cn

strcmp(a, b) == 0
来源：http://bcx.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://nok.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mef.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://rxi.wangshuangyany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dzy.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://pms.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vch.0kj1m.cn

[S10] C：指针与解引用
来源：http://sti.vehdjk.com

int *p = &a;  *p = 5;
来源：http://mkr.nanxuanxn.top

[S11] C：逐行读文件
来源：http://wiu.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://agy.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://aax.zhijiandao.cn

fclose(f);
来源：http://ebi.yj20258.top

[S12] C：写文件
来源：http://lfl.xuetiantiany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xhj.hongshengwenyu.top

[S13] C：宏定义
来源：http://nch.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fgr.shzxlz.cn

[S14] C：枚举
来源：http://gtl.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://qcf.uphjek.com

[S15] C：类型转换
来源：http://jam.guannengcc.top

(double) a / b
来源：http://rrk.yonumen.top

[S16] C：位操作置位
来源：http://xva.xuanzx.com

x |= (1 << 3);
来源：http://vtf.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://mmw.wangshuangyany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tli.gaohongyu789.top

[S18] C：命令行参数
来源：http://wpf.yangfankeji.com

int main(int argc, char **argv)
来源：http://mbc.cheryme.top

[S19] C：快速排序
来源：http://oon.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://asw.c1oappe.top

[S20] C：二分查找
来源：http://gjb.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ich.kuanghao11.cn

[S21] C：字符类别判断
来源：http://gqu.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oye.ywan-chungtsiang.top

[S22] C：字符串转数字
来源：http://ddi.fengsongda.top

atoi("42");  strtod("3.14", NULL);
来源：http://dpo.52xcode.cn

[S23] C：随机数
来源：http://arr.ybcxt.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xej.jinqigufen.top

[S24] C：获取本地时间
来源：http://ogk.xuetiantiany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://alh.iojbl.cn

[S25] C：内存拷贝
来源：http://vol.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://qhq.zhixingplan.top

[S26] C：内存清零
来源：http://oux.yonumen.top

memset(a, 0, sizeof a);
来源：http://bvy.tanke756.top

[S27] C：定义常量
来源：http://hlo.tianlin.xyz

const double PI = 3.14159;
来源：http://ytl.shuidangran.top

[S28] C：静态变量
来源：http://waf.fehbvm.com

static int counter = 0;
来源：http://isw.chenlongwang.top

[S29] C：变参函数
来源：http://yoz.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ony.gogol.net.cn

[S30] C：头文件保护
来源：http://kdq.gogol.net.cn

#ifndef X_H
来源：http://fao.yonumen.top

#define X_H
来源：http://tiq.gotoacloud.top

#endif
来源：http://vzy.yj20258888.top

[S31] C++：Hello World
来源：http://usq.hnqzz.top

#include <iostream>
来源：http://itk.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://mnj.ybcxt.top

[S32] C++：字符串
来源：http://sqc.iojbl.cn

std::string s = "hi";  s += "!";
来源：http://vmk.xuanzx.com

[S33] C++：vector 增删
来源：http://bnl.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sqe.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://bic.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://vjq.sysykeji.top

[S35] C++：map
来源：http://ted.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qjb.cdnleiting.top

[S36] C++：unordered_map
来源：http://mvs.daria6918.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uol.feifeiyinyue.top

[S37] C++：set
来源：http://qcy.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://chd.hnxiangtu.top

[S38] C++：排序
来源：http://rbf.meibo888.top

std::sort(v.begin(), v.end());
来源：http://yut.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://mrw.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ixk.vqdsnc.cn

[S40] C++：查找元素
来源：http://mum.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ajd.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://yby.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tzd.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://ilf.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://smw.cashguo.top

[S43] C++：智能指针
来源：http://evk.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://kja.tian-w.cn

[S44] C++：引用传参
来源：http://ltf.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://qpd.zdbjq.cn

[S45] C++：lambda
来源：http://hhn.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://szf.sweek.top

[S46] C++：函数模板
来源：http://ozq.zhoulong.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gli.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://tow.mhx1999.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tya.ydzc1.top

[S48] C++：逐行读文件
来源：http://skt.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://hii.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://sln.yfazqb.com

[S49] C++：写文件
来源：http://aje.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rzk.svipenyu.cn

[S50] C++：格式化数字
来源：http://ect.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tnc.fzhhl.top

[S51] C++：显式类型转换
来源：http://pgh.dianchejie.cn

static_cast<double>(a) / b
来源：http://hzy.sysykeji.top

[S52] C++：const 与 noexcept
来源：http://wir.hongshengwenyu.top

int size() const noexcept { return n_; }
来源：http://kun.52xcode.cn

[S53] C++：移动语义
来源：http://jjs.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://hee.sufxvd.cn

[S54] C++：异常处理
来源：http://zfl.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gbr.hywenlv.cn

[S55] C++：结构化绑定
来源：http://lbj.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tvh.ehwqpu.com

[S56] C++：optional
来源：http://otv.tianlin.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gng.c1oappe.top

[S57] C++：编译期常量
来源：http://tna.pengpengdd.cyou

constexpr int N = 10;
来源：http://ctt.hysaishi.cn

[S58] C++：命名空间
来源：http://ujd.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://qsf.aizwys.cn

[S59] C++：静态断言
来源：http://bfa.hnqzz.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ppj.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://jth.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fqz.hammf.cn

================================================================================
来源：http://eag.tianlin.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lqp.cdnleiting.top

================================================================================
来源：http://wkb.cashguo.top

[T01] Kotlin：Hello World
来源：http://pwu.yongpay.top

println("Hello")
来源：http://kpv.cucudq.cn

[T02] Kotlin：变量
来源：http://nex.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://usq.bjfxy.top

[T03] Kotlin：字符串模板
来源：http://tqc.mhx1999.top

"值: $b"
来源：http://pin.yfazqb.com

[T04] Kotlin：空安全
来源：http://bvd.zycfv.cn

val n: String? = null;  n?.length
来源：http://qfi.yj202588.top

[T05] Kotlin：when 表达式
来源：http://jxi.zhixingplan.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mls.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://zcm.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xyy.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://fkx.gzhubu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ude.xuanzx.com

[T08] Kotlin：数据类
来源：http://cbb.sufxvd.cn

data class User(val name: String, val age: Int)
来源：http://jwb.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://ltv.yvedp.cn

fun String.exclaim() = this + "!"
来源：http://wos.tarul.cn

[T10] Kotlin：默认参数
来源：http://txe.daxiang520.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rnx.hcnkem.com

[T11] Kotlin：协程
来源：http://gff.ydzc1.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qii.zycfv.cn

[T12] Kotlin：解构声明
来源：http://yim.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://hps.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://viu.mhx1999.top

val m = mapOf("a" to 1)
来源：http://dmg.ctjpmb.com

[T14] Kotlin：循环
来源：http://dvq.yfazqb.com

for (i in 1..10) println(i)
来源：http://lcf.ybcxt.top

[T15] Kotlin：接口
来源：http://esj.hongshengwenyu.top

interface Shape { fun area(): Double }
来源：http://jjf.yonumen.top

[T16] Swift：Hello World
来源：http://ibj.sweek.top

print("Hello")
来源：http://lon.zhixingplan.top

[T17] Swift：变量与常量
来源：http://waa.yanxiufei.cn

var a = 1;  let b = 2
来源：http://wvv.daxiang520.top

[T18] Swift：字符串插值
来源：http://buu.birdmap.top

"值: \(b)"
来源：http://vlr.hesvh.cn

[T19] Swift：可选绑定
来源：http://bnr.jqgfzy.top

if let n = opt { print(n) }
来源：http://xxe.hesvh.cn

[T20] Swift：数组操作
来源：http://xso.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://hcf.0kj1m.cn

[T21] Swift：遍历
来源：http://jsg.zdbjq.cn

for x in a { print(x) }
来源：http://yjz.xziqi.cn

[T22] Swift：字典
来源：http://xdf.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://xcw.wangshuangyany.cn

[T23] Swift：函数
来源：http://stv.hfpthk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jue.52xcode.cn

[T24] Swift：闭包
来源：http://lxr.cashguo.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gye.yvedp.cn

[T25] Swift：结构体
来源：http://div.pengpengdd.cyou

struct P { var x: Int }
来源：http://gyc.guowangkeji.top

[T26] Swift：类与重写
来源：http://okf.wangshuangyany.cn

class A: Base { override func f() {} }
来源：http://srm.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://wlt.hcnkem.com

do { try f() } catch { print(error) }
来源：http://azf.havefunace.top

[T28] Swift：枚举
来源：http://kft.ehwqpu.com

enum Color { case red, green }
来源：http://wke.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://hcy.xuetiantiany.cn

guard let x = opt else { return }
来源：http://pkc.hfpthk.cn

[T30] Swift：协议
来源：http://sqz.cqqwz.cn

protocol Shape { func area() -> Double }
来源：http://pmv.zdqjudy.top

[T31] Lua：Hello World
来源：http://eaf.hywenlv.cn

print("Hello")
来源：http://jgg.jyoumei.cn

[T32] Lua：局部变量
来源：http://zln.0kj1m.cn

local a = 1
来源：http://rtx.smart0.xyz

[T33] Lua：表（数组）
来源：http://oma.guannengcc.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vux.jiagoushi.top

[T34] Lua：遍历表
来源：http://ayi.birdmap.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yhu.hnqzz.top

[T35] Lua：字典表
来源：http://xpd.xylfe.cn

local d = { a = 1 };  d.b = 2
来源：http://dvl.ydzc1.top

[T36] Lua：函数
来源：http://ios.quarkkingdee.top

function add(a, b) return a + b end
来源：http://mqw.pycfn.com

[T37] Lua：字符串拼接
来源：http://fra.xingfuxueyuan.xyz

"a" .. "b"
来源：http://uha.bbcook.cn

[T38] Lua：条件
来源：http://hqu.epnwcf.com

if x > 0 then print("正") end
来源：http://tgd.hfpthk.cn

[T39] Lua：模式匹配
来源：http://afp.bbcook.cn

string.find(s, "%d+")
来源：http://glu.cheryme.top

[T40] Lua：元表
来源：http://ene.ydzc1.top

setmetatable({}, { __index = base })
来源：http://fqa.fehbvm.com

[T41] Perl：Hello World
来源：http://uew.havefunace.top

print "Hello\n";
来源：http://kuj.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://pcl.ydzc1.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://avi.zycfv.cn

[T43] Perl：字符串插值
来源：http://jjp.yj20258888.top

"值: $a"
来源：http://ubi.meibo888.top

[T44] Perl：条件
来源：http://kai.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://jtz.fengsongda.top

[T45] Perl：数组遍历
来源：http://cyz.hywenlv.cn

for my $x (@arr) { print $x; }
来源：http://pga.jqgufenzy.top

[T46] Perl：哈希操作
来源：http://qjy.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://chy.hongshengwenyu.top

[T47] Perl：正则捕获
来源：http://mhi.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fyw.xziqi.cn

[T48] Perl：正则替换
来源：http://grg.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://pjg.xziqi.cn

[T49] Perl：函数
来源：http://oxd.iojbl.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rhf.guannengcc.top

[T50] Perl：逐行读文件
来源：http://omi.hnxiangtu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jbh.vqdsnc.cn

while (my $line = <$fh>) { print $line; }
来源：http://fif.vqdsnc.cn

[T51] Scala：Hello World
来源：http://jjb.daxiang520.top

println("Hello")
来源：http://knc.zhoulong.xyz

[T52] Scala：变量
来源：http://kbq.zhixingplan.top

val a = 1;  var b = 2
来源：http://jzt.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://ave.cqqwz.cn

s"值: $b"
来源：http://dqe.aibaodan.cn

[T54] Scala：集合映射
来源：http://fqp.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://aif.epnwcf.com

[T55] Scala：集合过滤
来源：http://obl.bbcook.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qib.hnqzz.top

[T56] Scala：样例类
来源：http://unn.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://ujq.quarkkingdee.top

[T57] Scala：模式匹配
来源：http://yqh.meibo888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://esh.52xcode.cn

[T58] Scala：函数定义
来源：http://gae.iojbl.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bad.yvedp.cn

[T59] Scala：循环
来源：http://pil.ydjk.org.cn

for (i <- 1 to 10) println(i)
来源：http://qek.yfazqb.com

[T60] Scala：折叠
来源：http://nui.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://two.ctjpmb.com

================================================================================
来源：http://skw.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://elo.daria6918.cn

================================================================================
来源：http://itr.sysykeji.top

[U01] Py：创建虚拟环境
来源：http://tin.zhaomingkeji.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://cem.tanke756.top

[U02] Py：导出 / 安装依赖
来源：http://dkm.jiagoushi.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zhm.yj20258.top

[U03] Py：加载 .env 配置
来源：http://uhl.chenzaomai.com

from dotenv import load_dotenv; load_dotenv()
来源：http://bkp.yfazqb.com

[U04] Py：变量调试打印
来源：http://azx.aibaodan.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wom.wangdashe.top

[U05] Py：列表去重且保序
来源：http://zjf.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://icq.zhiwuduotai.top

[U06] Py：合并两个字典
来源：http://fib.xuetiantiany.cn

{**a, **b}
来源：http://gno.sysykeji.top

[U07] Py：反转字典键值
来源：http://ppd.havefunace.top

{v: k for k, v in d.items()}
来源：http://nee.yonumen.top

[U08] Py：展平二维列表
来源：http://oxj.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://mmb.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://uxa.chenzaomai.com

max(d, key=d.get)
来源：http://fcg.cucudq.cn

[U10] Py：按值排序字典
来源：http://tqf.fzhhl.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iat.zdqjudy.top

[U11] Py：生成器表达式
来源：http://hed.xinyue.icu

(x * 2 for x in arr)
来源：http://lip.yongpay.top

[U12] Py：取出现最多的 3 个元素
来源：http://wea.chenjidiqi.icu

Counter(arr).most_common(3)
来源：http://nfs.redwolf501.top

[U13] Py：固定长度队列
来源：http://inm.dianchejie.cn

deque(maxlen=10)
来源：http://ske.yj20258888.top

[U14] Py：分组收集到列表
来源：http://axh.nanxinkj.top

defaultdict(list)
来源：http://kxm.zhixingplan.top

[U15] Py：高精度计时
来源：http://pbe.bjfxy.top

t = time.perf_counter()
来源：http://roa.dashuyun.cn

[U16] Py：命令行参数解析
来源：http://dee.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rdb.ydjk.org.cn

[U17] Py：初始化日志
来源：http://wpq.fehbvm.com

logging.basicConfig(level=logging.INFO)
来源：http://cpo.jiagoushi.top

[U18] Py：预编译正则
来源：http://knq.nwbrower.top

pat = re.compile(r"\d+")
来源：http://ddp.hcnkem.com


<!-- 参考信息 -->