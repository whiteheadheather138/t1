代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://zdn.jyoumei.cn

[R76] 使用临时文件
来源：http://yzu.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xui.quarkkingdee.top

[R77] 读取用户输入
来源：http://usg.mhx1999.top

read -rp "请输入: " ans
来源：http://yzw.jinqigufen.top

[R78] 交互式菜单
来源：http://dxq.chenzaomai.com

select opt in a b c; do echo "$opt"; break; done
来源：http://zee.xuetiantiany.cn

[R79] 解析命令行选项
来源：http://lfu.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ijk.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://orz.9152youxi.cn

time ./run.sh
来源：http://mzb.birdmap.top

================================================================================
来源：http://uay.shanyushiyangkeji.top

S. C / C++ 专题
来源：http://hfn.zhiwuduotai.top

================================================================================
来源：http://rhs.jinghuilouyu.cn

[S01] C：Hello World
来源：http://nqw.nwbrower.top

#include <stdio.h>
来源：http://hxs.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://eeb.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://voh.hnqzz.top

int a = 10; printf("%d\n", a);
来源：http://dsz.ybcxt.top

[S03] C：读入整数
来源：http://mpm.ehwqpu.com

int x; scanf("%d", &x);
来源：http://lqj.yuxming.cn

[S04] C：字符串复制
来源：http://dfz.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://qwi.birdmap.top

[S05] C：字符串长度
来源：http://keq.vqdsnc.cn

strlen(s)
来源：http://lju.redwolf501.top

[S06] C：字符串比较
来源：http://vwi.gotoacloud.top

strcmp(a, b) == 0
来源：http://ckw.aizwys.cn

[S07] C：数组遍历求和
来源：http://qct.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://umz.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://ohf.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rwu.tian-w.cn

[S09] C：结构体定义与初始化
来源：http://ezn.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zyf.haohaochexian.top

[S10] C：指针与解引用
来源：http://yhi.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://stx.xinyue.icu

[S11] C：逐行读文件
来源：http://pbh.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://yzb.yongpay.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bvw.shanyushiyangkeji.top

fclose(f);
来源：http://ses.shanyushiyangkeji.top

[S12] C：写文件
来源：http://heh.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://apb.jiagoushi.top

[S13] C：宏定义
来源：http://moi.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://acc.tanke756.top

[S14] C：枚举
来源：http://mtv.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://nra.bbcook.cn

[S15] C：类型转换
来源：http://mes.yanxiufei.cn

(double) a / b
来源：http://nmt.yuxming.cn

[S16] C：位操作置位
来源：http://qdv.yongpay.top

x |= (1 << 3);
来源：http://rwg.tian-w.cn

[S17] C：安全拼接字符串
来源：http://glf.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qde.uphjek.com

[S18] C：命令行参数
来源：http://koz.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://gnh.ctjpmb.com

[S19] C：快速排序
来源：http://fit.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ziw.jinqigufen.top

[S20] C：二分查找
来源：http://ica.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jfu.gaohongyu789.top

[S21] C：字符类别判断
来源：http://jsd.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gbd.yj20258.top

[S22] C：字符串转数字
来源：http://sng.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pva.shanyushiyangtech.top

[S23] C：随机数
来源：http://nph.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dgr.chenlongwang.top

[S24] C：获取本地时间
来源：http://lit.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oqu.jlsjyb.cn

[S25] C：内存拷贝
来源：http://ohp.smart0.xyz

memcpy(dst, src, n);
来源：http://vth.daria6918.cn

[S26] C：内存清零
来源：http://kcv.smart0.xyz

memset(a, 0, sizeof a);
来源：http://opx.jinghuilouyu.cn

[S27] C：定义常量
来源：http://ady.ywan-chungtsiang.top

const double PI = 3.14159;
来源：http://ngz.zdqjudy.top

[S28] C：静态变量
来源：http://dwh.chenzaomai.com

static int counter = 0;
来源：http://zmw.cheryme.top

[S29] C：变参函数
来源：http://mln.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uww.zhoulong.xyz

[S30] C：头文件保护
来源：http://sqv.zhaomingkeji.xyz

#ifndef X_H
来源：http://jgj.jinqigfzy.top

#define X_H
来源：http://brj.xylfe.cn

#endif
来源：http://ggr.chenjidiqi.icu

[S31] C++：Hello World
来源：http://scd.shuidangran.top

#include <iostream>
来源：http://iva.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://dgn.aibaodan.cn

[S32] C++：字符串
来源：http://fvx.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://yms.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://khd.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sfb.yj202588.top

[S34] C++：遍历 vector
来源：http://bqn.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://dgn.jinghuilouyu.cn

[S35] C++：map
来源：http://mbr.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dfi.cheryme.top

[S36] C++：unordered_map
来源：http://bof.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ryt.c1oappe.top

[S37] C++：set
来源：http://bmh.zhiwuduotai.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zri.sufxvd.cn

[S38] C++：排序
来源：http://uqz.pycfn.com

std::sort(v.begin(), v.end());
来源：http://jeh.52xcode.cn

[S39] C++：自定义比较器排序
来源：http://mlt.birdmap.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cky.pengpengdd.cyou

[S40] C++：查找元素
来源：http://wkq.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xfm.nanxinkj.top

[S41] C++：类与构造函数
来源：http://zha.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vcd.nwbrower.top

[S42] C++：继承与虚函数
来源：http://zct.fanxiaobao.xyz

class B : public Base { public: void f() override {} };
来源：http://oeh.ydjk.org.cn

[S43] C++：智能指针
来源：http://fgu.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://mqp.jinqigufen.top

[S44] C++：引用传参
来源：http://nud.aizwys.cn

void inc(int &x) { ++x; }
来源：http://xak.jianghu66.top

[S45] C++：lambda
来源：http://szp.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://box.hammf.cn

[S46] C++：函数模板
来源：http://hdy.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yfg.dianchejie.cn

[S47] C++：结构化绑定遍历
来源：http://crh.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ewz.daxiang520.top

[S48] C++：逐行读文件
来源：http://nuc.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://dnw.bjfxy.top

while (std::getline(in, line)) { }
来源：http://wxw.fehbvm.com

[S49] C++：写文件
来源：http://vcf.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aaq.shuidangran.top

[S50] C++：格式化数字
来源：http://ets.quarkkingdee.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://boa.jiagoushi.top

[S51] C++：显式类型转换
来源：http://jwr.hesvh.cn

static_cast<double>(a) / b
来源：http://zxa.ydzc1.top

[S52] C++：const 与 noexcept
来源：http://ntm.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://kok.chenlongwang.top

[S53] C++：移动语义
来源：http://bpb.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://ric.hywenlv.cn

[S54] C++：异常处理
来源：http://ahp.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uvo.gogol.net.cn

[S55] C++：结构化绑定
来源：http://jys.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gcy.gotoacloud.top

[S56] C++：optional
来源：http://rbc.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jyf.wangdashe.top

[S57] C++：编译期常量
来源：http://rpi.shanyushiyangtech.top

constexpr int N = 10;
来源：http://ilq.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://wug.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://vqi.yangfankeji.com

[S59] C++：静态断言
来源：http://dqo.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fhc.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://hzt.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://awa.hnxiangtu.top

================================================================================
来源：http://vok.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://krl.snrcjt.cn

================================================================================
来源：http://jup.daxiang520.top

[T01] Kotlin：Hello World
来源：http://hld.sufxvd.cn

println("Hello")
来源：http://heh.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://kys.kuanghao11.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ujv.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://rsg.cdnleiting.top

"值: $b"
来源：http://hym.svipenyu.cn

[T04] Kotlin：空安全
来源：http://jyr.zhengqikj.top

val n: String? = null;  n?.length
来源：http://six.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://ual.yangfankeji.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wku.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://swu.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rmc.jiagoushi.top

[T07] Kotlin：集合过滤
来源：http://fyb.hongshengwenyu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qtg.hysaishi.cn

[T08] Kotlin：数据类
来源：http://fsx.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://csa.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://yqi.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://kpw.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://dmi.sweek.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fdk.iojbl.cn

[T11] Kotlin：协程
来源：http://jyi.hammf.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eue.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://zlm.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://nrl.0kj1m.cn

[T13] Kotlin：只读 Map
来源：http://dbb.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://dgz.tian-w.cn

[T14] Kotlin：循环
来源：http://cuz.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://djt.hesvh.cn

[T15] Kotlin：接口
来源：http://ngh.xylfe.cn

interface Shape { fun area(): Double }
来源：http://zuz.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://tzr.xziqi.cn

print("Hello")
来源：http://bsb.ivvv.top

[T17] Swift：变量与常量
来源：http://qic.hysaishi.cn

var a = 1;  let b = 2
来源：http://vbr.haohaochexian.top

[T18] Swift：字符串插值
来源：http://jwz.zhijiandao.cn

"值: \(b)"
来源：http://ycs.chenjidiqi.icu

[T19] Swift：可选绑定
来源：http://kpg.fktsv.cn

if let n = opt { print(n) }
来源：http://hht.chenlongwang.top

[T20] Swift：数组操作
来源：http://yua.shanyushiyangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://cnq.yongpay.top

[T21] Swift：遍历
来源：http://yhw.ivvv.top

for x in a { print(x) }
来源：http://gag.sxryk.cn

[T22] Swift：字典
来源：http://ecx.yfazqb.com

var d = ["a": 1];  d["b"] = 2
来源：http://odn.gotoacloud.top

[T23] Swift：函数
来源：http://vmy.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eei.sxryk.cn

[T24] Swift：闭包
来源：http://xhn.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lik.svipenyu.cn

[T25] Swift：结构体
来源：http://oxv.cdnleiting.top

struct P { var x: Int }
来源：http://bam.aibaodan.cn

[T26] Swift：类与重写
来源：http://whx.birdmap.top

class A: Base { override func f() {} }
来源：http://wki.cucudq.cn

[T27] Swift：错误处理
来源：http://inr.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://mjw.fengsongda.top

[T28] Swift：枚举
来源：http://xrp.ydjk.org.cn

enum Color { case red, green }
来源：http://qqh.tarul.cn

[T29] Swift：guard 提前返回
来源：http://amt.zhongyouzk.top

guard let x = opt else { return }
来源：http://zmr.jinghuilouyu.cn

[T30] Swift：协议
来源：http://plb.ivvv.top

protocol Shape { func area() -> Double }
来源：http://ypx.fzhhl.top

[T31] Lua：Hello World
来源：http://eka.chenzaomai.com

print("Hello")
来源：http://jnh.snrcjt.cn

[T32] Lua：局部变量
来源：http://hoz.hesvh.cn

local a = 1
来源：http://avh.smart0.xyz

[T33] Lua：表（数组）
来源：http://dbd.aizwys.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://baw.smart0.xyz

[T34] Lua：遍历表
来源：http://pcc.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ybd.pengpengdd.cyou

[T35] Lua：字典表
来源：http://jjz.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://qul.cucudq.cn

[T36] Lua：函数
来源：http://zta.ivvv.top

function add(a, b) return a + b end
来源：http://wyf.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://gwv.yangfankeji.com

"a" .. "b"
来源：http://gsv.wangshuangyany.cn

[T38] Lua：条件
来源：http://mtj.zhiwuduotai.top

if x > 0 then print("正") end
来源：http://ozy.chenzaomai.com

[T39] Lua：模式匹配
来源：http://lzq.shuidangran.top

string.find(s, "%d+")
来源：http://kko.yongpay.top

[T40] Lua：元表
来源：http://ita.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://kra.fengsongda.top

[T41] Perl：Hello World
来源：http://hnm.smart0.xyz

print "Hello\n";
来源：http://utl.ydjk.org.cn

[T42] Perl：变量类型
来源：http://sxi.mhx1999.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tvt.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://tji.yueranfly.top

"值: $a"
来源：http://gtt.cucudq.cn

[T44] Perl：条件
来源：http://rjp.jinqigfzy.top

if ($a > 0) { print "正"; }
来源：http://ixn.guannengcc.top

[T45] Perl：数组遍历
来源：http://rjr.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://ecv.shzxlz.cn

[T46] Perl：哈希操作
来源：http://eno.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xxo.hnxiangtu.top

[T47] Perl：正则捕获
来源：http://jhr.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pqx.xingfuxueyuan.xyz

[T48] Perl：正则替换
来源：http://ont.shanyushiyangtech.top

$s =~ s/old/new/g;
来源：http://uvv.yj20258.top

[T49] Perl：函数
来源：http://gsj.fktsv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hfv.cqqwz.cn

[T50] Perl：逐行读文件
来源：http://uaq.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zve.birdmap.top

while (my $line = <$fh>) { print $line; }
来源：http://wjs.ppjwa.cn

[T51] Scala：Hello World
来源：http://ycw.yfazqb.com

println("Hello")
来源：http://qkc.hysaishi.cn

[T52] Scala：变量
来源：http://ubw.jiagoushi.top

val a = 1;  var b = 2
来源：http://pfy.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://tny.yangfankeji.com

s"值: $b"
来源：http://wkr.fanxiaobao.xyz

[T54] Scala：集合映射
来源：http://ggb.vehdjk.com

List(1, 2, 3).map(_ * 2)
来源：http://ttk.52xcode.cn

[T55] Scala：集合过滤
来源：http://odh.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://bpw.snrcjt.cn

[T56] Scala：样例类
来源：http://obi.fktsv.cn

case class User(name: String, age: Int)
来源：http://wwb.aizwys.cn

[T57] Scala：模式匹配
来源：http://sen.xziqi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nry.hysaishi.cn

[T58] Scala：函数定义
来源：http://bia.ydjk.org.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jkt.wangdashe.top

[T59] Scala：循环
来源：http://esb.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://yug.shzxlz.cn

[T60] Scala：折叠
来源：http://ucz.yj202588.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qbw.xziqi.cn

================================================================================
来源：http://ocm.fktsv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qsh.316326.xyz

================================================================================
来源：http://hyt.yueranfly.top

[U01] Py：创建虚拟环境
来源：http://pfg.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://bgq.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://mgq.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aeb.aibaodan.cn

[U03] Py：加载 .env 配置
来源：http://pou.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jxn.bbcook.cn

[U04] Py：变量调试打印
来源：http://gci.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dmb.xylfe.cn

[U05] Py：列表去重且保序
来源：http://ggp.jianghu66.top

list(dict.fromkeys(arr))
来源：http://wzh.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://ovh.zdbjq.cn

{**a, **b}
来源：http://stu.dianchejie.cn

[U07] Py：反转字典键值
来源：http://vct.aizwys.cn

{v: k for k, v in d.items()}
来源：http://tvd.shanyushiyangtech.top

[U08] Py：展平二维列表
来源：http://ale.zhongyouzk.top

[y for x in nested for y in x]
来源：http://ieh.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://xml.nanxinkj.top

max(d, key=d.get)
来源：http://vwd.hywenlv.cn

[U10] Py：按值排序字典
来源：http://tjz.ctjpmb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vre.fengsongda.top

[U11] Py：生成器表达式
来源：http://vll.hnqzz.top

(x * 2 for x in arr)
来源：http://grz.wangshuangyany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lox.zhiwuduotai.top

Counter(arr).most_common(3)
来源：http://pqz.nwbrower.top

[U13] Py：固定长度队列
来源：http://szt.sufxvd.cn

deque(maxlen=10)
来源：http://tui.hysaishi.cn

[U14] Py：分组收集到列表
来源：http://kep.uphjek.com

defaultdict(list)
来源：http://xdt.yongpay.top

[U15] Py：高精度计时
来源：http://ors.xylfe.cn

t = time.perf_counter()
来源：http://gcd.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://gry.nwbrower.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hzj.xziqi.cn


<!-- 参考信息 -->