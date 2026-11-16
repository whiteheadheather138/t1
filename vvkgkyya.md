代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://jso.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://egt.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://xlq.xuetiantiany.cn

[R71] 日期格式化
来源：http://sux.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cpc.ehwqpu.com

[R72] 等待端口就绪
来源：http://ygt.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wwq.gogol.net.cn

[R73] 分割大日志
来源：http://sgd.jianghu66.top

split -l 1000 big.log part_
来源：http://vqe.yj20258888.top

[R74] 批量重命名
来源：http://ztg.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://klk.dianchejie.cn

[R75] 导出环境变量
来源：http://ogv.hongshengwenyu.top

export PATH="$HOME/bin:$PATH"
来源：http://nan.yj20258888.top

[R76] 使用临时文件
来源：http://dsb.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fvh.316326.xyz

[R77] 读取用户输入
来源：http://eun.feifeiyinyue.top

read -rp "请输入: " ans
来源：http://cmv.wangshuangyany.cn

[R78] 交互式菜单
来源：http://zkw.sjlbkw.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pbe.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://fhs.fzhhl.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://llu.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://jgk.316326.xyz

time ./run.sh
来源：http://qiz.fengsongda.top

================================================================================
来源：http://zps.feifeiyinyue.top

S. C / C++ 专题
来源：http://pzr.c1oappe.top

================================================================================
来源：http://mem.shuidangran.top

[S01] C：Hello World
来源：http://pre.pengpengdd.cyou

#include <stdio.h>
来源：http://eob.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mwl.chenzaomai.com

[S02] C：变量与格式化输出
来源：http://lka.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://ijx.jinqigfzy.top

[S03] C：读入整数
来源：http://pvq.aibaodan.cn

int x; scanf("%d", &x);
来源：http://dhk.fzhhl.top

[S04] C：字符串复制
来源：http://srx.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://iyk.daria6918.cn

[S05] C：字符串长度
来源：http://onm.yueranfly.top

strlen(s)
来源：http://tyi.tanke756.top

[S06] C：字符串比较
来源：http://mgo.jianghu66.top

strcmp(a, b) == 0
来源：http://bpb.ivvv.top

[S07] C：数组遍历求和
来源：http://sql.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nng.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://cuj.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rnh.jinqigufen.top

[S09] C：结构体定义与初始化
来源：http://mwh.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jop.dianchejie.cn

[S10] C：指针与解引用
来源：http://izu.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://zon.hnqzz.top

[S11] C：逐行读文件
来源：http://vzv.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://phs.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fcm.zdqjudy.top

fclose(f);
来源：http://nhz.jinqigfzy.top

[S12] C：写文件
来源：http://qib.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ymv.316326.xyz

[S13] C：宏定义
来源：http://knm.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mqd.jqgfzy.top

[S14] C：枚举
来源：http://rii.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://ajs.gzhubu.top

[S15] C：类型转换
来源：http://tsm.gzhubu.top

(double) a / b
来源：http://yfm.yueranfly.top

[S16] C：位操作置位
来源：http://xtd.yongpay.top

x |= (1 << 3);
来源：http://irc.sweek.top

[S17] C：安全拼接字符串
来源：http://bhi.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uam.yvedp.cn

[S18] C：命令行参数
来源：http://wza.zycfv.cn

int main(int argc, char **argv)
来源：http://osk.gogol.net.cn

[S19] C：快速排序
来源：http://wnv.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://maq.hfpthk.cn

[S20] C：二分查找
来源：http://zki.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kta.meibo888.top

[S21] C：字符类别判断
来源：http://qqx.xinyue.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wcr.9152youxi.cn

[S22] C：字符串转数字
来源：http://uvu.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://taz.cashguo.top

[S23] C：随机数
来源：http://qmd.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://eco.chenjidiqi.icu

[S24] C：获取本地时间
来源：http://wgu.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qjw.zdbjq.cn

[S25] C：内存拷贝
来源：http://nil.nanxinkj.top

memcpy(dst, src, n);
来源：http://mdb.epnwcf.com

[S26] C：内存清零
来源：http://pwi.aizwys.cn

memset(a, 0, sizeof a);
来源：http://urg.cheryme.top

[S27] C：定义常量
来源：http://jjp.redwolf501.top

const double PI = 3.14159;
来源：http://qwl.yj202588.top

[S28] C：静态变量
来源：http://msf.ywan-chungtsiang.top

static int counter = 0;
来源：http://etb.dianchejie.cn

[S29] C：变参函数
来源：http://for.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jag.ivvv.top

[S30] C：头文件保护
来源：http://esq.chenzaomai.com

#ifndef X_H
来源：http://tzh.xuetiantiany.cn

#define X_H
来源：http://iwm.gaohongyu789.top

#endif
来源：http://hiv.shzxlz.cn

[S31] C++：Hello World
来源：http://kyq.yvedp.cn

#include <iostream>
来源：http://eys.tian-w.cn

int main() { std::cout << "Hello\n"; }
来源：http://ofm.dashuyun.cn

[S32] C++：字符串
来源：http://blt.sxryk.cn

std::string s = "hi";  s += "!";
来源：http://lxw.vehdjk.com

[S33] C++：vector 增删
来源：http://egc.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dkt.tanke756.top

[S34] C++：遍历 vector
来源：http://uwc.gzhubu.top

for (auto &x : v) { std::cout << x; }
来源：http://hms.xuetiantiany.cn

[S35] C++：map
来源：http://zsu.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bbn.fktsv.cn

[S36] C++：unordered_map
来源：http://rdi.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cql.smart0.xyz

[S37] C++：set
来源：http://qvq.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sip.yanxiufei.cn

[S38] C++：排序
来源：http://cul.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://ofc.birdmap.top

[S39] C++：自定义比较器排序
来源：http://kks.birdmap.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qwz.tanke756.top

[S40] C++：查找元素
来源：http://jgf.yangfankeji.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mfv.havefunace.top

[S41] C++：类与构造函数
来源：http://hfd.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yyx.fktsv.cn

[S42] C++：继承与虚函数
来源：http://rpf.yangfankeji.com

class B : public Base { public: void f() override {} };
来源：http://kue.9152youxi.cn

[S43] C++：智能指针
来源：http://sch.jinqigufen.top

auto p = std::make_unique<int>(5);
来源：http://thq.sysykeji.top

[S44] C++：引用传参
来源：http://gta.yonumen.top

void inc(int &x) { ++x; }
来源：http://zob.shanyushiyangtech.top

[S45] C++：lambda
来源：http://nbp.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://oar.nanxinkj.top

[S46] C++：函数模板
来源：http://wsz.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gvb.yvedp.cn

[S47] C++：结构化绑定遍历
来源：http://hka.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wff.gotoacloud.top

[S48] C++：逐行读文件
来源：http://dzw.yongpay.top

std::ifstream in("a.txt");  std::string line;
来源：http://lks.yongpay.top

while (std::getline(in, line)) { }
来源：http://tuz.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://nwp.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zdz.52xcode.cn

[S50] C++：格式化数字
来源：http://zmc.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zsn.jqgfzy.top

[S51] C++：显式类型转换
来源：http://xbv.kuanghao11.cn

static_cast<double>(a) / b
来源：http://ose.jinqigufen.top

[S52] C++：const 与 noexcept
来源：http://qxi.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://fle.chenjidiqi.icu

[S53] C++：移动语义
来源：http://gnm.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://wop.pengpengdd.cyou

[S54] C++：异常处理
来源：http://csp.c1oappe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hip.c1oappe.top

[S55] C++：结构化绑定
来源：http://zdi.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hlq.hfpthk.cn

[S56] C++：optional
来源：http://smo.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hjm.cucudq.cn

[S57] C++：编译期常量
来源：http://tpc.xuanzx.com

constexpr int N = 10;
来源：http://lel.ppjwa.cn

[S58] C++：命名空间
来源：http://vei.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://xyn.shzxlz.cn

[S59] C++：静态断言
来源：http://ynt.jinyuanbaomall.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ewb.tian-w.cn

[S60] C++：遍历并删除元素
来源：http://ebu.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://emk.yanxiufei.cn

================================================================================
来源：http://kpm.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rsa.cheryme.top

================================================================================
来源：http://lpn.shzxlz.cn

[T01] Kotlin：Hello World
来源：http://fcc.birdmap.top

println("Hello")
来源：http://opw.jqgfzy.top

[T02] Kotlin：变量
来源：http://kic.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lny.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://sxh.hnqzz.top

"值: $b"
来源：http://wgh.ywan-chungtsiang.top

[T04] Kotlin：空安全
来源：http://nko.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://twv.zdbjq.cn

[T05] Kotlin：when 表达式
来源：http://tsc.aizwys.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jxv.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://dfy.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://elo.tianlin.xyz

[T07] Kotlin：集合过滤
来源：http://kbw.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eda.ivvv.top

[T08] Kotlin：数据类
来源：http://hzt.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://zac.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://ast.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://ogf.bjfxy.top

[T10] Kotlin：默认参数
来源：http://ocz.52xcode.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wmv.ivvv.top

[T11] Kotlin：协程
来源：http://vfn.redwolf501.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://smh.chenlongwang.top

[T12] Kotlin：解构声明
来源：http://zmz.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://vzs.hnxiangtu.top

[T13] Kotlin：只读 Map
来源：http://yws.shanyushiyangtech.top

val m = mapOf("a" to 1)
来源：http://bjm.ppjwa.cn

[T14] Kotlin：循环
来源：http://dlq.zhixingplan.top

for (i in 1..10) println(i)
来源：http://xeh.jyoumei.cn

[T15] Kotlin：接口
来源：http://sbd.yuanzhike.top

interface Shape { fun area(): Double }
来源：http://trv.c1oappe.top

[T16] Swift：Hello World
来源：http://wxx.xziqi.cn

print("Hello")
来源：http://qto.guannengcc.top

[T17] Swift：变量与常量
来源：http://sup.ppjwa.cn

var a = 1;  let b = 2
来源：http://tai.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://rjp.sysykeji.top

"值: \(b)"
来源：http://eee.aizwys.cn

[T19] Swift：可选绑定
来源：http://myw.ppjwa.cn

if let n = opt { print(n) }
来源：http://mdl.chenzaomai.com

[T20] Swift：数组操作
来源：http://piu.jinyuanbaomall.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fkq.316326.xyz

[T21] Swift：遍历
来源：http://prm.yueranfly.top

for x in a { print(x) }
来源：http://hua.chenzaomai.com

[T22] Swift：字典
来源：http://upu.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://ohh.pycfn.com

[T23] Swift：函数
来源：http://fik.hnxiangtu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ndo.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://iaf.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bmw.ybcxt.top

[T25] Swift：结构体
来源：http://nbq.0kj1m.cn

struct P { var x: Int }
来源：http://dqj.fzhhl.top

[T26] Swift：类与重写
来源：http://cof.gotoacloud.top

class A: Base { override func f() {} }
来源：http://hzu.bjfxy.top

[T27] Swift：错误处理
来源：http://xfd.xziqi.cn

do { try f() } catch { print(error) }
来源：http://ngy.ppjwa.cn

[T28] Swift：枚举
来源：http://xtu.pengpengdd.cyou

enum Color { case red, green }
来源：http://zev.jiagoushi.top

[T29] Swift：guard 提前返回
来源：http://ssh.ivvv.top

guard let x = opt else { return }
来源：http://ghe.sxryk.cn

[T30] Swift：协议
来源：http://ixl.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://yph.xylfe.cn

[T31] Lua：Hello World
来源：http://umk.smart0.xyz

print("Hello")
来源：http://cha.shangyingyoupin.top

[T32] Lua：局部变量
来源：http://bap.yuxming.cn

local a = 1
来源：http://hpc.yj20258.top

[T33] Lua：表（数组）
来源：http://ccx.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rur.guowangkeji.top

[T34] Lua：遍历表
来源：http://syc.tian-w.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wdp.jqgufenzy.top

[T35] Lua：字典表
来源：http://tic.nwbrower.top

local d = { a = 1 };  d.b = 2
来源：http://dki.chenjidiqi.icu

[T36] Lua：函数
来源：http://uew.ybcxt.top

function add(a, b) return a + b end
来源：http://fby.yongpay.top

[T37] Lua：字符串拼接
来源：http://kzz.chenjidiqi.icu

"a" .. "b"
来源：http://lcx.sweek.top

[T38] Lua：条件
来源：http://xuh.vehdjk.com

if x > 0 then print("正") end
来源：http://iwf.ctjpmb.com

[T39] Lua：模式匹配
来源：http://ukl.yanxiufei.cn

string.find(s, "%d+")
来源：http://fqj.hywenlv.cn

[T40] Lua：元表
来源：http://bnb.xinyue.icu

setmetatable({}, { __index = base })
来源：http://vpd.0kj1m.cn

[T41] Perl：Hello World
来源：http://zxd.zdbjq.cn

print "Hello\n";
来源：http://jaq.fktsv.cn

[T42] Perl：变量类型
来源：http://rab.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jdc.ppjwa.cn

[T43] Perl：字符串插值
来源：http://nud.fengsongda.top

"值: $a"
来源：http://uhk.quarkkingdee.top

[T44] Perl：条件
来源：http://vbt.fktsv.cn

if ($a > 0) { print "正"; }
来源：http://hwr.bjfxy.top

[T45] Perl：数组遍历
来源：http://nae.zdbjq.cn

for my $x (@arr) { print $x; }
来源：http://ujq.zdqjudy.top

[T46] Perl：哈希操作
来源：http://gvg.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uag.havefunace.top

[T47] Perl：正则捕获
来源：http://ark.daxiang520.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fgh.hongshengwenyu.top

[T48] Perl：正则替换
来源：http://uzb.yfazqb.com

$s =~ s/old/new/g;
来源：http://uvh.yuxming.cn

[T49] Perl：函数
来源：http://veg.chenlongwang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bzh.yj20258888.top

[T50] Perl：逐行读文件
来源：http://zfb.sjlbkw.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://akt.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://dud.ydzc1.top

[T51] Scala：Hello World
来源：http://uga.uphjek.com

println("Hello")
来源：http://ado.chenlongwang.top

[T52] Scala：变量
来源：http://njv.zhijiandao.cn

val a = 1;  var b = 2
来源：http://xhw.dianchejie.cn

[T53] Scala：字符串插值
来源：http://smn.smart0.xyz

s"值: $b"
来源：http://bnr.shzxlz.cn

[T54] Scala：集合映射
来源：http://tym.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://jgh.jianghu66.top

[T55] Scala：集合过滤
来源：http://agz.birdmap.top

List(1, 2, 3).filter(_ > 1)
来源：http://tnq.zhijiandao.cn

[T56] Scala：样例类
来源：http://fhq.zhoulong.xyz

case class User(name: String, age: Int)
来源：http://npd.uphjek.com

[T57] Scala：模式匹配
来源：http://kas.pengpengdd.cyou

x match { case 1 => "一"; case _ => "其他" }
来源：http://zqd.mhx1999.top

[T58] Scala：函数定义
来源：http://oyo.gaohongyu789.top

def add(a: Int, b: Int): Int = a + b
来源：http://mzx.zhengqikj.top

[T59] Scala：循环
来源：http://aio.iojbl.cn

for (i <- 1 to 10) println(i)
来源：http://lmz.iojbl.cn

[T60] Scala：折叠
来源：http://cnp.c1oappe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bhd.wangdashe.top

================================================================================
来源：http://aek.daria6918.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pby.hcnkem.com

================================================================================
来源：http://agu.tianlin.xyz

[U01] Py：创建虚拟环境
来源：http://tii.jiagoushi.top

python -m venv .venv && source .venv/bin/activate
来源：http://stn.hongshengwenyu.top

[U02] Py：导出 / 安装依赖
来源：http://iqx.zhijiandao.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vtt.ehwqpu.com

[U03] Py：加载 .env 配置
来源：http://mvl.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rmd.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://flb.zhongyouzk.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nol.jianghu66.top

[U05] Py：列表去重且保序
来源：http://jld.jianghu66.top

list(dict.fromkeys(arr))
来源：http://puz.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://wty.jiagoushi.top

{**a, **b}
来源：http://nzr.cucudq.cn

[U07] Py：反转字典键值
来源：http://jtt.cqqwz.cn

{v: k for k, v in d.items()}
来源：http://ovc.cqqwz.cn

[U08] Py：展平二维列表
来源：http://hxa.fzhhl.top

[y for x in nested for y in x]
来源：http://kxv.havefunace.top

[U09] Py：字典取最大值的键
来源：http://fdg.yuxming.cn

max(d, key=d.get)
来源：http://rxc.jqgfzy.top

[U10] Py：按值排序字典
来源：http://mog.gzhubu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mab.cdnleiting.top


<!-- 参考信息 -->