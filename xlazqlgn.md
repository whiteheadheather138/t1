代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://evv.zdqjudy.top

[R72] 等待端口就绪
来源：http://bcz.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uep.zhongyouzk.top

[R73] 分割大日志
来源：http://orm.fzhhl.top

split -l 1000 big.log part_
来源：http://rbd.yj202588.top

[R74] 批量重命名
来源：http://rjf.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://azk.yj20258.top

[R75] 导出环境变量
来源：http://gkx.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://gtc.gaohongyu789.top

[R76] 使用临时文件
来源：http://ipz.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zdy.jqgufenzy.top

[R77] 读取用户输入
来源：http://giv.chenzaomai.com

read -rp "请输入: " ans
来源：http://vdv.ehwqpu.com

[R78] 交互式菜单
来源：http://yfr.redwolf501.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ozs.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://mjr.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rfm.yfazqb.com

[R80] 查看脚本执行耗时
来源：http://ees.ywan-chungtsiang.top

time ./run.sh
来源：http://usb.gogol.net.cn

================================================================================
来源：http://eus.yj20258.top

S. C / C++ 专题
来源：http://bfu.hammf.cn

================================================================================
来源：http://uuu.aibaodan.cn

[S01] C：Hello World
来源：http://ymt.andypj.xyz

#include <stdio.h>
来源：http://dvg.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://drb.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://pxx.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://kky.xinyue.icu

[S03] C：读入整数
来源：http://rpi.zhaomingkeji.xyz

int x; scanf("%d", &x);
来源：http://bqb.jinqigfzy.top

[S04] C：字符串复制
来源：http://qts.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://abt.hnxiangtu.top

[S05] C：字符串长度
来源：http://yug.9152youxi.cn

strlen(s)
来源：http://frs.shuidangran.top

[S06] C：字符串比较
来源：http://zob.tanke756.top

strcmp(a, b) == 0
来源：http://tuq.xylfe.cn

[S07] C：数组遍历求和
来源：http://xkc.vqdsnc.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xsa.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://mxj.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pzb.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://vuc.smart0.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rys.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://wqu.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://nvj.cdnleiting.top

[S11] C：逐行读文件
来源：http://ggm.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://onc.jiagoushi.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pgx.zhengqikj.top

fclose(f);
来源：http://rzr.quarkkingdee.top

[S12] C：写文件
来源：http://lum.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kcs.fanxiaobao.xyz

[S13] C：宏定义
来源：http://xgt.cqqwz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://izn.sxryk.cn

[S14] C：枚举
来源：http://jvp.snrcjt.cn

enum Color { RED, GREEN, BLUE };
来源：http://ujq.yanxiufei.cn

[S15] C：类型转换
来源：http://knk.aibaodan.cn

(double) a / b
来源：http://zxq.yuxming.cn

[S16] C：位操作置位
来源：http://nfc.fanxiaobao.xyz

x |= (1 << 3);
来源：http://apl.shangyingyoupin.top

[S17] C：安全拼接字符串
来源：http://ymj.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gpa.ctjpmb.com

[S18] C：命令行参数
来源：http://ptq.xziqi.cn

int main(int argc, char **argv)
来源：http://eta.zhongyouzk.top

[S19] C：快速排序
来源：http://fam.feifeiyinyue.top

qsort(a, n, sizeof(int), cmp);
来源：http://edy.jiagoushi.top

[S20] C：二分查找
来源：http://ddd.pycfn.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vjy.epnwcf.com

[S21] C：字符类别判断
来源：http://yah.cucudq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uqb.iojbl.cn

[S22] C：字符串转数字
来源：http://hxi.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vlk.sjlbkw.cn

[S23] C：随机数
来源：http://qgg.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nqv.daxiang520.top

[S24] C：获取本地时间
来源：http://rvy.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gza.zhijiandao.cn

[S25] C：内存拷贝
来源：http://wxf.chenlongwang.top

memcpy(dst, src, n);
来源：http://xdo.zhengqikj.top

[S26] C：内存清零
来源：http://oeo.vehdjk.com

memset(a, 0, sizeof a);
来源：http://lgm.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://szm.xingfuxueyuan.xyz

const double PI = 3.14159;
来源：http://uxj.ctjpmb.com

[S28] C：静态变量
来源：http://wzs.sysykeji.top

static int counter = 0;
来源：http://kbm.yj20258888.top

[S29] C：变参函数
来源：http://ell.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uih.jiagoushi.top

[S30] C：头文件保护
来源：http://jmz.kuanghao11.cn

#ifndef X_H
来源：http://knc.yonumen.top

#define X_H
来源：http://yly.ppjwa.cn

#endif
来源：http://eeh.zhixingplan.top

[S31] C++：Hello World
来源：http://vco.haohaochexian.top

#include <iostream>
来源：http://utf.snrcjt.cn

int main() { std::cout << "Hello\n"; }
来源：http://cwc.gogol.net.cn

[S32] C++：字符串
来源：http://uuc.xziqi.cn

std::string s = "hi";  s += "!";
来源：http://nts.zdqjudy.top

[S33] C++：vector 增删
来源：http://wvu.mhx1999.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ndm.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://mvg.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://kmi.cucudq.cn

[S35] C++：map
来源：http://brk.guannengcc.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bgh.cqqwz.cn

[S36] C++：unordered_map
来源：http://ylz.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mcn.chenlongwang.top

[S37] C++：set
来源：http://vmz.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kqo.zhijiandao.cn

[S38] C++：排序
来源：http://mhz.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://lvg.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://etd.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rnc.pengpengdd.cyou

[S40] C++：查找元素
来源：http://ews.hammf.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sxf.haohaochexian.top

[S41] C++：类与构造函数
来源：http://rmc.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://azz.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://vgj.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://bad.xuetiantiany.cn

[S43] C++：智能指针
来源：http://wua.bjfxy.top

auto p = std::make_unique<int>(5);
来源：http://lyh.shangyingyoupin.top

[S44] C++：引用传参
来源：http://exq.xziqi.cn

void inc(int &x) { ++x; }
来源：http://ylh.zhiwuduotai.top

[S45] C++：lambda
来源：http://uxc.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://zhh.xuetiantiany.cn

[S46] C++：函数模板
来源：http://csm.zhaomingkeji.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pff.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://suv.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vql.shzxlz.cn

[S48] C++：逐行读文件
来源：http://gcw.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://kmu.iojbl.cn

while (std::getline(in, line)) { }
来源：http://dkj.iojbl.cn

[S49] C++：写文件
来源：http://pmo.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qdb.jqgfzy.top

[S50] C++：格式化数字
来源：http://pct.tianlin.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iri.gzhubu.top

[S51] C++：显式类型转换
来源：http://pai.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://tuk.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://hxu.cheryme.top

int size() const noexcept { return n_; }
来源：http://yie.zhijiandao.cn

[S53] C++：移动语义
来源：http://dut.hammf.cn

std::vector<int> w = std::move(v);
来源：http://pnl.bbcook.cn

[S54] C++：异常处理
来源：http://zbm.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://maw.yj20258888.top

[S55] C++：结构化绑定
来源：http://fij.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tls.vqdsnc.cn

[S56] C++：optional
来源：http://yib.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pzw.sysykeji.top

[S57] C++：编译期常量
来源：http://jlf.shanyushiyangtech.top

constexpr int N = 10;
来源：http://mlh.xuanzx.com

[S58] C++：命名空间
来源：http://csk.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://fpb.jinqigfzy.top

[S59] C++：静态断言
来源：http://wrk.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bgu.sufxvd.cn

[S60] C++：遍历并删除元素
来源：http://dqk.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jyg.daxiang520.top

================================================================================
来源：http://pmf.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hos.yj20258.top

================================================================================
来源：http://hqi.wangdashe.top

[T01] Kotlin：Hello World
来源：http://wyo.yfazqb.com

println("Hello")
来源：http://ccl.hongshengwenyu.top

[T02] Kotlin：变量
来源：http://cqj.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jrl.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://ktg.yuxming.cn

"值: $b"
来源：http://ozy.meibo888.top

[T04] Kotlin：空安全
来源：http://ijd.chenzaomai.com

val n: String? = null;  n?.length
来源：http://imt.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://hol.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://utz.fzhhl.top

[T06] Kotlin：集合映射
来源：http://rwo.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wdp.jinqigfzy.top

[T07] Kotlin：集合过滤
来源：http://szv.svipenyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cue.dianchejie.cn

[T08] Kotlin：数据类
来源：http://ukb.hysaishi.cn

data class User(val name: String, val age: Int)
来源：http://lnz.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://bwc.jqgufenzy.top

fun String.exclaim() = this + "!"
来源：http://jav.yongpay.top

[T10] Kotlin：默认参数
来源：http://fpx.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://cuh.vqdsnc.cn

[T11] Kotlin：协程
来源：http://jvs.ctjpmb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://vut.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://hiy.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://qxa.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://msf.birdmap.top

val m = mapOf("a" to 1)
来源：http://hxf.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://zyo.aizwys.cn

for (i in 1..10) println(i)
来源：http://ihl.shangyingyoupin.top

[T15] Kotlin：接口
来源：http://xlq.xinyue.icu

interface Shape { fun area(): Double }
来源：http://xxz.gaohongyu789.top

[T16] Swift：Hello World
来源：http://rnk.shzxlz.cn

print("Hello")
来源：http://iek.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://cir.kuanghao11.cn

var a = 1;  let b = 2
来源：http://wab.tanke756.top

[T18] Swift：字符串插值
来源：http://ffs.cucudq.cn

"值: \(b)"
来源：http://hub.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://hga.zhoulong.xyz

if let n = opt { print(n) }
来源：http://idh.ctjpmb.com

[T20] Swift：数组操作
来源：http://mdg.hywenlv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lbm.nanxuanxn.top

[T21] Swift：遍历
来源：http://lqs.quarkkingdee.top

for x in a { print(x) }
来源：http://txm.yanxiufei.cn

[T22] Swift：字典
来源：http://wig.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://coo.cucudq.cn

[T23] Swift：函数
来源：http://ngh.shzxlz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lyj.hcnkem.com

[T24] Swift：闭包
来源：http://ywd.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://pke.zhongyouzk.top

[T25] Swift：结构体
来源：http://loh.ybcxt.top

struct P { var x: Int }
来源：http://hah.iojbl.cn

[T26] Swift：类与重写
来源：http://bfn.dianchejie.cn

class A: Base { override func f() {} }
来源：http://qwn.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://vof.yanxiufei.cn

do { try f() } catch { print(error) }
来源：http://qsz.hesvh.cn

[T28] Swift：枚举
来源：http://csl.aibaodan.cn

enum Color { case red, green }
来源：http://sll.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://wzc.316326.xyz

guard let x = opt else { return }
来源：http://cuz.wangdashe.top

[T30] Swift：协议
来源：http://kuy.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://bgx.bbcook.cn

[T31] Lua：Hello World
来源：http://zab.ehwqpu.com

print("Hello")
来源：http://jhe.hfpthk.cn

[T32] Lua：局部变量
来源：http://aaj.hongshengwenyu.top

local a = 1
来源：http://dof.ivvv.top

[T33] Lua：表（数组）
来源：http://mdd.havefunace.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kox.dashuyun.cn

[T34] Lua：遍历表
来源：http://qsz.sufxvd.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vvv.jianghu66.top

[T35] Lua：字典表
来源：http://ayp.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://evn.fehbvm.com

[T36] Lua：函数
来源：http://rar.hesvh.cn

function add(a, b) return a + b end
来源：http://yqv.yuxming.cn

[T37] Lua：字符串拼接
来源：http://rlv.guowangkeji.top

"a" .. "b"
来源：http://rrk.hongshengwenyu.top

[T38] Lua：条件
来源：http://tcp.ppjwa.cn

if x > 0 then print("正") end
来源：http://xvi.0kj1m.cn

[T39] Lua：模式匹配
来源：http://xfw.tarul.cn

string.find(s, "%d+")
来源：http://vst.sufxvd.cn

[T40] Lua：元表
来源：http://eyf.ydjk.org.cn

setmetatable({}, { __index = base })
来源：http://xka.cdnleiting.top

[T41] Perl：Hello World
来源：http://cuy.yongpay.top

print "Hello\n";
来源：http://adw.wangdashe.top

[T42] Perl：变量类型
来源：http://mpf.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qzg.zhongyouzk.top

[T43] Perl：字符串插值
来源：http://vtf.birdmap.top

"值: $a"
来源：http://icd.iojbl.cn

[T44] Perl：条件
来源：http://yej.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://cgv.zycfv.cn

[T45] Perl：数组遍历
来源：http://ohi.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://sbi.sweek.top

[T46] Perl：哈希操作
来源：http://skc.hesvh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://edc.nanxuanxn.top

[T47] Perl：正则捕获
来源：http://pjd.feifeiyinyue.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bym.aizwys.cn

[T48] Perl：正则替换
来源：http://knk.fehbvm.com

$s =~ s/old/new/g;
来源：http://muf.316326.xyz

[T49] Perl：函数
来源：http://ytl.daria6918.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ceb.jianghu66.top

[T50] Perl：逐行读文件
来源：http://vko.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hzb.birdmap.top

while (my $line = <$fh>) { print $line; }
来源：http://urg.zhiwuduotai.top

[T51] Scala：Hello World
来源：http://yax.jinyuanbaomall.cn

println("Hello")
来源：http://rwu.c1oappe.top

[T52] Scala：变量
来源：http://adg.hongshengwenyu.top

val a = 1;  var b = 2
来源：http://wog.jlsjyb.cn

[T53] Scala：字符串插值
来源：http://fvy.xinyue.icu

s"值: $b"
来源：http://bef.pengpengdd.cyou

[T54] Scala：集合映射
来源：http://ept.yj20258888.top

List(1, 2, 3).map(_ * 2)
来源：http://sab.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://cpi.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://onr.xuanzx.com

[T56] Scala：样例类
来源：http://alp.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://zre.hfpthk.cn

[T57] Scala：模式匹配
来源：http://hfm.sweek.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vlk.dianchejie.cn

[T58] Scala：函数定义
来源：http://nwy.andypj.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://flg.shangyingyoupin.top

[T59] Scala：循环
来源：http://kgz.pengpengdd.cyou

for (i <- 1 to 10) println(i)
来源：http://fsc.0kj1m.cn

[T60] Scala：折叠
来源：http://voa.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://exf.52xcode.cn

================================================================================
来源：http://iuo.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xye.tanke756.top

================================================================================
来源：http://xsq.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://wsm.hfpthk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zke.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://krc.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ymk.fanxiaobao.xyz

[U03] Py：加载 .env 配置
来源：http://jeu.hammf.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rpe.sufxvd.cn

[U04] Py：变量调试打印
来源：http://dxi.yangfankeji.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wug.guowangkeji.top

[U05] Py：列表去重且保序
来源：http://hnr.yangfankeji.com

list(dict.fromkeys(arr))
来源：http://pgr.fengsongda.top

[U06] Py：合并两个字典
来源：http://sbh.xuanzx.com

{**a, **b}
来源：http://gjt.mhx1999.top

[U07] Py：反转字典键值
来源：http://hpe.jinghuilouyu.cn

{v: k for k, v in d.items()}
来源：http://qon.gogol.net.cn

[U08] Py：展平二维列表
来源：http://job.zhaomingkeji.xyz

[y for x in nested for y in x]
来源：http://txt.gaohongyu789.top

[U09] Py：字典取最大值的键
来源：http://trt.jyoumei.cn

max(d, key=d.get)
来源：http://kit.yueranfly.top

[U10] Py：按值排序字典
来源：http://haq.zhengqikj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vmk.guannengcc.top

[U11] Py：生成器表达式
来源：http://yhf.xuetiantiany.cn

(x * 2 for x in arr)
来源：http://jud.shangyingyoupin.top

[U12] Py：取出现最多的 3 个元素
来源：http://pee.jqgfzy.top

Counter(arr).most_common(3)
来源：http://rtc.tanke756.top


<!-- 参考信息 -->