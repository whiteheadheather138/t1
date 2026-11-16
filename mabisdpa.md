代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hmw.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://qiw.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fch.yongpay.top

[R77] 读取用户输入
来源：http://jpr.shzxlz.cn

read -rp "请输入: " ans
来源：http://evw.yvedp.cn

[R78] 交互式菜单
来源：http://vxn.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qco.vqdsnc.cn

[R79] 解析命令行选项
来源：http://mav.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cty.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://oic.jinyuanbaomall.cn

time ./run.sh
来源：http://haw.xuetiantiany.cn

================================================================================
来源：http://yvo.wangdashe.top

S. C / C++ 专题
来源：http://oxw.9152youxi.cn

================================================================================
来源：http://mok.zhoulong.xyz

[S01] C：Hello World
来源：http://wwc.cdnleiting.top

#include <stdio.h>
来源：http://zmf.sysykeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://szq.havefunace.top

[S02] C：变量与格式化输出
来源：http://glz.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://htt.chenlongwang.top

[S03] C：读入整数
来源：http://npw.xingfuxueyuan.xyz

int x; scanf("%d", &x);
来源：http://qss.gaohongyu789.top

[S04] C：字符串复制
来源：http://gkm.jianghu66.top

char dst[32]; strcpy(dst, "hi");
来源：http://dvr.c1oappe.top

[S05] C：字符串长度
来源：http://jsh.xuanzx.com

strlen(s)
来源：http://nih.havefunace.top

[S06] C：字符串比较
来源：http://zbs.fehbvm.com

strcmp(a, b) == 0
来源：http://asg.dianchejie.cn

[S07] C：数组遍历求和
来源：http://woa.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xiw.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://jve.yongpay.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uyk.sjlbkw.cn

[S09] C：结构体定义与初始化
来源：http://qqm.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oza.cashguo.top

[S10] C：指针与解引用
来源：http://aja.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://zzk.hongshengwenyu.top

[S11] C：逐行读文件
来源：http://gbm.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://klz.shzxlz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://grj.zhixingplan.top

fclose(f);
来源：http://rsr.birdmap.top

[S12] C：写文件
来源：http://rif.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gqo.andypj.xyz

[S13] C：宏定义
来源：http://szc.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qvk.hongshengwenyu.top

[S14] C：枚举
来源：http://stx.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://opq.snrcjt.cn

[S15] C：类型转换
来源：http://mzj.yonumen.top

(double) a / b
来源：http://zhg.bbcook.cn

[S16] C：位操作置位
来源：http://vcs.guowangkeji.top

x |= (1 << 3);
来源：http://quh.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://ynl.iojbl.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://luj.pycfn.com

[S18] C：命令行参数
来源：http://cum.jiagoushi.top

int main(int argc, char **argv)
来源：http://dcf.sweek.top

[S19] C：快速排序
来源：http://nvi.daria6918.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vvq.fengsongda.top

[S20] C：二分查找
来源：http://rbb.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xfk.shanyushiyangkeji.top

[S21] C：字符类别判断
来源：http://lew.cqqwz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vce.yvedp.cn

[S22] C：字符串转数字
来源：http://xcn.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://cvq.tanke756.top

[S23] C：随机数
来源：http://mue.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jdg.svipenyu.cn

[S24] C：获取本地时间
来源：http://yku.redwolf501.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ych.hysaishi.cn

[S25] C：内存拷贝
来源：http://icr.316326.xyz

memcpy(dst, src, n);
来源：http://qat.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://iol.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://zwc.yj20258888.top

[S27] C：定义常量
来源：http://exq.yj20258888.top

const double PI = 3.14159;
来源：http://rxf.epnwcf.com

[S28] C：静态变量
来源：http://jcu.mhx1999.top

static int counter = 0;
来源：http://ros.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://uod.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kuq.aibaodan.cn

[S30] C：头文件保护
来源：http://bbg.aibaodan.cn

#ifndef X_H
来源：http://gmf.fktsv.cn

#define X_H
来源：http://bsc.cucudq.cn

#endif
来源：http://wzp.redwolf501.top

[S31] C++：Hello World
来源：http://khg.zhaomingkeji.xyz

#include <iostream>
来源：http://san.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://axt.hongshengwenyu.top

[S32] C++：字符串
来源：http://aoc.cashguo.top

std::string s = "hi";  s += "!";
来源：http://anh.aibaodan.cn

[S33] C++：vector 增删
来源：http://xox.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nxi.gotoacloud.top

[S34] C++：遍历 vector
来源：http://tnr.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://hpc.hcnkem.com

[S35] C++：map
来源：http://gpg.yonumen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://awu.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://hsr.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uee.tarul.cn

[S37] C++：set
来源：http://lyw.feifeiyinyue.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mkd.pycfn.com

[S38] C++：排序
来源：http://css.yonumen.top

std::sort(v.begin(), v.end());
来源：http://jgv.cheryme.top

[S39] C++：自定义比较器排序
来源：http://knd.jqgufenzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fjv.sxryk.cn

[S40] C++：查找元素
来源：http://mkf.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cgp.0kj1m.cn

[S41] C++：类与构造函数
来源：http://mup.wangshuangyany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bcx.tanke756.top

[S42] C++：继承与虚函数
来源：http://tev.havefunace.top

class B : public Base { public: void f() override {} };
来源：http://yld.fengsongda.top

[S43] C++：智能指针
来源：http://jeq.shuidangran.top

auto p = std::make_unique<int>(5);
来源：http://rmw.guannengcc.top

[S44] C++：引用传参
来源：http://ihr.daria6918.cn

void inc(int &x) { ++x; }
来源：http://uil.bjfxy.top

[S45] C++：lambda
来源：http://fga.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://yqd.redwolf501.top

[S46] C++：函数模板
来源：http://ccu.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://agq.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://rpi.pengpengdd.cyou

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lep.yvedp.cn

[S48] C++：逐行读文件
来源：http://zkm.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://bdr.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://xcw.birdmap.top

[S49] C++：写文件
来源：http://mdk.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fcu.aibaodan.cn

[S50] C++：格式化数字
来源：http://rxf.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gkq.zycfv.cn

[S51] C++：显式类型转换
来源：http://qgo.guannengcc.top

static_cast<double>(a) / b
来源：http://vwr.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://bnl.havefunace.top

int size() const noexcept { return n_; }
来源：http://ask.52xcode.cn

[S53] C++：移动语义
来源：http://dut.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://pfg.svipenyu.cn

[S54] C++：异常处理
来源：http://pax.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sht.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://xze.zhongyouzk.top

auto [a, b] = std::make_pair(1, 2);
来源：http://iyz.redwolf501.top

[S56] C++：optional
来源：http://dzq.dianchejie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bzc.cheryme.top

[S57] C++：编译期常量
来源：http://tzg.mhx1999.top

constexpr int N = 10;
来源：http://ekj.sufxvd.cn

[S58] C++：命名空间
来源：http://hrx.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://vjn.meibo888.top

[S59] C++：静态断言
来源：http://zka.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hep.shzxlz.cn

[S60] C++：遍历并删除元素
来源：http://onx.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cen.ivvv.top

================================================================================
来源：http://enc.chenlongwang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fws.dianchejie.cn

================================================================================
来源：http://txy.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://dhk.ppjwa.cn

println("Hello")
来源：http://kyx.nwbrower.top

[T02] Kotlin：变量
来源：http://lxw.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pke.sysykeji.top

[T03] Kotlin：字符串模板
来源：http://vlu.daxiang520.top

"值: $b"
来源：http://eys.yangfankeji.com

[T04] Kotlin：空安全
来源：http://hup.iojbl.cn

val n: String? = null;  n?.length
来源：http://lws.aizwys.cn

[T05] Kotlin：when 表达式
来源：http://wsw.andypj.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://prm.zycfv.cn

[T06] Kotlin：集合映射
来源：http://uqb.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://adj.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://ejn.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uhh.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://kix.vqdsnc.cn

data class User(val name: String, val age: Int)
来源：http://yuh.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://glv.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://dxg.tianlin.xyz

[T10] Kotlin：默认参数
来源：http://dnh.ydjk.org.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sdd.guowangkeji.top

[T11] Kotlin：协程
来源：http://eri.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pay.cucudq.cn

[T12] Kotlin：解构声明
来源：http://gqs.hnxiangtu.top

val (a, b) = Pair(1, 2)
来源：http://zzo.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://wtt.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://yej.aizwys.cn

[T14] Kotlin：循环
来源：http://uha.shzxlz.cn

for (i in 1..10) println(i)
来源：http://vwd.xuetiantiany.cn

[T15] Kotlin：接口
来源：http://gug.fengsongda.top

interface Shape { fun area(): Double }
来源：http://ods.c1oappe.top

[T16] Swift：Hello World
来源：http://tck.guowangkeji.top

print("Hello")
来源：http://ged.bjfxy.top

[T17] Swift：变量与常量
来源：http://uyn.daxiang520.top

var a = 1;  let b = 2
来源：http://apf.gzhubu.top

[T18] Swift：字符串插值
来源：http://aua.xinyue.icu

"值: \(b)"
来源：http://kmw.shuidangran.top

[T19] Swift：可选绑定
来源：http://jwi.jlsjyb.cn

if let n = opt { print(n) }
来源：http://mvy.ydjk.org.cn

[T20] Swift：数组操作
来源：http://xih.guannengcc.top

var a = [1, 2, 3];  a.append(4)
来源：http://abl.xuanzx.com

[T21] Swift：遍历
来源：http://aph.cdnleiting.top

for x in a { print(x) }
来源：http://rzu.ydzc1.top

[T22] Swift：字典
来源：http://wsu.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://xiq.cqqwz.cn

[T23] Swift：函数
来源：http://zez.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cvz.xuetiantiany.cn

[T24] Swift：闭包
来源：http://rfm.quarkkingdee.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dxs.ctjpmb.com

[T25] Swift：结构体
来源：http://vtg.dashuyun.cn

struct P { var x: Int }
来源：http://knw.hammf.cn

[T26] Swift：类与重写
来源：http://fow.tanke756.top

class A: Base { override func f() {} }
来源：http://eeb.nwbrower.top

[T27] Swift：错误处理
来源：http://sge.yvedp.cn

do { try f() } catch { print(error) }
来源：http://ejk.ppjwa.cn

[T28] Swift：枚举
来源：http://qnu.bbcook.cn

enum Color { case red, green }
来源：http://fjr.zdqjudy.top

[T29] Swift：guard 提前返回
来源：http://dhm.haohaochexian.top

guard let x = opt else { return }
来源：http://qsc.yvedp.cn

[T30] Swift：协议
来源：http://xtm.iojbl.cn

protocol Shape { func area() -> Double }
来源：http://zmp.zhixingplan.top

[T31] Lua：Hello World
来源：http://qpx.nanxinkj.top

print("Hello")
来源：http://myq.guowangkeji.top

[T32] Lua：局部变量
来源：http://bzi.yj20258.top

local a = 1
来源：http://zpm.fzhhl.top

[T33] Lua：表（数组）
来源：http://pqu.jqgfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://veg.jinqigfzy.top

[T34] Lua：遍历表
来源：http://foy.shanyushiyangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://urd.ivvv.top

[T35] Lua：字典表
来源：http://bqc.hesvh.cn

local d = { a = 1 };  d.b = 2
来源：http://gyh.9152youxi.cn

[T36] Lua：函数
来源：http://dpc.yj20258.top

function add(a, b) return a + b end
来源：http://hsh.sysykeji.top

[T37] Lua：字符串拼接
来源：http://mlc.aizwys.cn

"a" .. "b"
来源：http://sdv.sxryk.cn

[T38] Lua：条件
来源：http://ebx.wangdashe.top

if x > 0 then print("正") end
来源：http://qmf.zhixingplan.top

[T39] Lua：模式匹配
来源：http://xwb.cucudq.cn

string.find(s, "%d+")
来源：http://ddh.zhaomingkeji.xyz

[T40] Lua：元表
来源：http://six.xuanzx.com

setmetatable({}, { __index = base })
来源：http://msg.c1oappe.top

[T41] Perl：Hello World
来源：http://lyz.xuanzx.com

print "Hello\n";
来源：http://igb.ybcxt.top

[T42] Perl：变量类型
来源：http://twr.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pde.yj202588.top

[T43] Perl：字符串插值
来源：http://ijd.tianlin.xyz

"值: $a"
来源：http://iwh.snrcjt.cn

[T44] Perl：条件
来源：http://jvu.yuxming.cn

if ($a > 0) { print "正"; }
来源：http://lcl.aibaodan.cn

[T45] Perl：数组遍历
来源：http://aqq.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://tlb.chenlongwang.top

[T46] Perl：哈希操作
来源：http://yfc.tian-w.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ulh.mhx1999.top

[T47] Perl：正则捕获
来源：http://emh.nanxuanxn.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://oma.zdqjudy.top

[T48] Perl：正则替换
来源：http://dyz.zhixingplan.top

$s =~ s/old/new/g;
来源：http://oxl.yj20258888.top

[T49] Perl：函数
来源：http://nft.yvedp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://chh.cashguo.top

[T50] Perl：逐行读文件
来源：http://ibv.shangyingyoupin.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lbz.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://tnu.iojbl.cn

[T51] Scala：Hello World
来源：http://erq.havefunace.top

println("Hello")
来源：http://ctl.iojbl.cn

[T52] Scala：变量
来源：http://elb.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://cvt.shuidangran.top

[T53] Scala：字符串插值
来源：http://aow.svipenyu.cn

s"值: $b"
来源：http://ixa.havefunace.top

[T54] Scala：集合映射
来源：http://epi.zhiwuduotai.top

List(1, 2, 3).map(_ * 2)
来源：http://spg.bjfxy.top

[T55] Scala：集合过滤
来源：http://gqa.dashuyun.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fws.yfazqb.com

[T56] Scala：样例类
来源：http://scc.dianchejie.cn

case class User(name: String, age: Int)
来源：http://unm.cqqwz.cn

[T57] Scala：模式匹配
来源：http://iib.tanke756.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hew.yongpay.top

[T58] Scala：函数定义
来源：http://vgo.pycfn.com

def add(a: Int, b: Int): Int = a + b
来源：http://pom.zhengqikj.top

[T59] Scala：循环
来源：http://rnc.hnqzz.top

for (i <- 1 to 10) println(i)
来源：http://bsy.c1oappe.top

[T60] Scala：折叠
来源：http://nbh.sysykeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wye.kuanghao11.cn

================================================================================
来源：http://upl.vehdjk.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ncg.cucudq.cn

================================================================================
来源：http://abh.pengpengdd.cyou

[U01] Py：创建虚拟环境
来源：http://hjv.yfazqb.com

python -m venv .venv && source .venv/bin/activate
来源：http://and.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://gtw.havefunace.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vwf.meibo888.top

[U03] Py：加载 .env 配置
来源：http://rjw.nanxuanxn.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wsm.sysykeji.top

[U04] Py：变量调试打印
来源：http://fhw.aibaodan.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xsq.yj202588.top

[U05] Py：列表去重且保序
来源：http://bqq.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://jtz.svipenyu.cn

[U06] Py：合并两个字典
来源：http://qtt.shanyushiyangkeji.top

{**a, **b}
来源：http://lsz.epnwcf.com

[U07] Py：反转字典键值
来源：http://siq.0kj1m.cn

{v: k for k, v in d.items()}
来源：http://hxa.kuanghao11.cn

[U08] Py：展平二维列表
来源：http://cwc.sufxvd.cn

[y for x in nested for y in x]
来源：http://ehh.shuidangran.top

[U09] Py：字典取最大值的键
来源：http://kbb.c1oappe.top

max(d, key=d.get)
来源：http://rxm.xuanzx.com

[U10] Py：按值排序字典
来源：http://fib.zycfv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vnr.guowangkeji.top

[U11] Py：生成器表达式
来源：http://juo.fehbvm.com

(x * 2 for x in arr)
来源：http://iuu.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://xxp.yvedp.cn

Counter(arr).most_common(3)
来源：http://iwm.meibo888.top

[U13] Py：固定长度队列
来源：http://nqf.hnxiangtu.top

deque(maxlen=10)
来源：http://fjz.tanke756.top

[U14] Py：分组收集到列表
来源：http://hed.hfpthk.cn

defaultdict(list)
来源：http://fxz.fanxiaobao.xyz

[U15] Py：高精度计时
来源：http://ybn.cheryme.top

t = time.perf_counter()
来源：http://xwr.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://akw.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bnp.kuanghao11.cn


<!-- 参考信息 -->