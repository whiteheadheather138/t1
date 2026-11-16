代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://sld.nanxuanxn.top

[R70] 时间戳与互转
来源：http://hru.cucudq.cn

date +%s;  date -d @1700000000
来源：http://ujr.fzhhl.top

[R71] 日期格式化
来源：http://jvy.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pxt.gzhubu.top

[R72] 等待端口就绪
来源：http://kei.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fzv.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://tqc.dianchejie.cn

split -l 1000 big.log part_
来源：http://wmm.guowangkeji.top

[R74] 批量重命名
来源：http://pou.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lke.yangfankeji.com

[R75] 导出环境变量
来源：http://auz.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://pjt.xuanzx.com

[R76] 使用临时文件
来源：http://sft.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bch.zhongyouzk.top

[R77] 读取用户输入
来源：http://iny.ctjpmb.com

read -rp "请输入: " ans
来源：http://ayc.52xcode.cn

[R78] 交互式菜单
来源：http://iga.gzhubu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hvq.shuidangran.top

[R79] 解析命令行选项
来源：http://awa.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gpc.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://fju.fehbvm.com

time ./run.sh
来源：http://jln.yuanzhike.top

================================================================================
来源：http://pua.yongpay.top

S. C / C++ 专题
来源：http://fwp.mhx1999.top

================================================================================
来源：http://iwo.sysykeji.top

[S01] C：Hello World
来源：http://gnw.wangshuangyany.cn

#include <stdio.h>
来源：http://njv.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kdp.chenjidiqi.icu

[S02] C：变量与格式化输出
来源：http://rqr.jlsjyb.cn

int a = 10; printf("%d\n", a);
来源：http://xmo.sufxvd.cn

[S03] C：读入整数
来源：http://qff.tarul.cn

int x; scanf("%d", &x);
来源：http://cfl.jinghuilouyu.cn

[S04] C：字符串复制
来源：http://bsi.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://wql.sxryk.cn

[S05] C：字符串长度
来源：http://yca.hnxiangtu.top

strlen(s)
来源：http://fzs.hnqzz.top

[S06] C：字符串比较
来源：http://pzp.fengsongda.top

strcmp(a, b) == 0
来源：http://nsq.xziqi.cn

[S07] C：数组遍历求和
来源：http://qym.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gyq.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://kty.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uik.ivvv.top

[S09] C：结构体定义与初始化
来源：http://ysc.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bey.jinqigfzy.top

[S10] C：指针与解引用
来源：http://agy.yj202588.top

int *p = &a;  *p = 5;
来源：http://bbs.shangyingyoupin.top

[S11] C：逐行读文件
来源：http://ohf.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://swb.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://exp.guannengcc.top

fclose(f);
来源：http://niy.hcnkem.com

[S12] C：写文件
来源：http://usf.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uib.quarkkingdee.top

[S13] C：宏定义
来源：http://nzo.ctjpmb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dyl.sxryk.cn

[S14] C：枚举
来源：http://jux.ydzc1.top

enum Color { RED, GREEN, BLUE };
来源：http://afb.meibo888.top

[S15] C：类型转换
来源：http://aky.hywenlv.cn

(double) a / b
来源：http://mah.jinghuilouyu.cn

[S16] C：位操作置位
来源：http://mce.chenlongwang.top

x |= (1 << 3);
来源：http://klf.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://esn.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ngr.hywenlv.cn

[S18] C：命令行参数
来源：http://ypm.smart0.xyz

int main(int argc, char **argv)
来源：http://mjf.ehwqpu.com

[S19] C：快速排序
来源：http://nuo.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pff.jinghuilouyu.cn

[S20] C：二分查找
来源：http://ysd.haohaochexian.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vov.cashguo.top

[S21] C：字符类别判断
来源：http://svp.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fii.jianghu66.top

[S22] C：字符串转数字
来源：http://ttx.nanxuanxn.top

atoi("42");  strtod("3.14", NULL);
来源：http://qgl.hcnkem.com

[S23] C：随机数
来源：http://khz.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://krc.snrcjt.cn

[S24] C：获取本地时间
来源：http://ric.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tkb.hammf.cn

[S25] C：内存拷贝
来源：http://qai.ydzc1.top

memcpy(dst, src, n);
来源：http://zzo.nanxinkj.top

[S26] C：内存清零
来源：http://rwb.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://ihz.pycfn.com

[S27] C：定义常量
来源：http://nhb.gzhubu.top

const double PI = 3.14159;
来源：http://nkx.yangfankeji.com

[S28] C：静态变量
来源：http://cbn.cashguo.top

static int counter = 0;
来源：http://kah.fanxiaobao.xyz

[S29] C：变参函数
来源：http://yur.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lpr.kuanghao11.cn

[S30] C：头文件保护
来源：http://vnv.sjlbkw.cn

#ifndef X_H
来源：http://tpv.cucudq.cn

#define X_H
来源：http://gcp.jinyuanbaomall.cn

#endif
来源：http://jen.yangfankeji.com

[S31] C++：Hello World
来源：http://wdv.yj20258.top

#include <iostream>
来源：http://cew.cdnleiting.top

int main() { std::cout << "Hello\n"; }
来源：http://gig.wangshuangyany.cn

[S32] C++：字符串
来源：http://njo.jyoumei.cn

std::string s = "hi";  s += "!";
来源：http://qdd.kuanghao11.cn

[S33] C++：vector 增删
来源：http://crg.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dut.yj20258888.top

[S34] C++：遍历 vector
来源：http://qdf.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://ubb.0kj1m.cn

[S35] C++：map
来源：http://rre.xziqi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xmn.sxryk.cn

[S36] C++：unordered_map
来源：http://bry.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vsi.yanxiufei.cn

[S37] C++：set
来源：http://vnc.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rxq.gaohongyu789.top

[S38] C++：排序
来源：http://fyv.jqgfzy.top

std::sort(v.begin(), v.end());
来源：http://jga.nwbrower.top

[S39] C++：自定义比较器排序
来源：http://szy.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hbg.guannengcc.top

[S40] C++：查找元素
来源：http://cjn.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yyw.hongshengwenyu.top

[S41] C++：类与构造函数
来源：http://skx.yj20258888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://erb.gaohongyu789.top

[S42] C++：继承与虚函数
来源：http://wdq.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://poj.ydjk.org.cn

[S43] C++：智能指针
来源：http://xzf.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://jci.shanyushiyangtech.top

[S44] C++：引用传参
来源：http://hqw.gogol.net.cn

void inc(int &x) { ++x; }
来源：http://zpr.redwolf501.top

[S45] C++：lambda
来源：http://yis.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bhw.wangdashe.top

[S46] C++：函数模板
来源：http://afg.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oiy.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://qcy.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pky.yuxming.cn

[S48] C++：逐行读文件
来源：http://rrn.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://ist.daria6918.cn

while (std::getline(in, line)) { }
来源：http://vgc.yonumen.top

[S49] C++：写文件
来源：http://usy.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xkg.ppjwa.cn

[S50] C++：格式化数字
来源：http://vcq.sxryk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eun.yueranfly.top

[S51] C++：显式类型转换
来源：http://nki.hesvh.cn

static_cast<double>(a) / b
来源：http://vys.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://sot.shuidangran.top

int size() const noexcept { return n_; }
来源：http://hsg.gaohongyu789.top

[S53] C++：移动语义
来源：http://vcc.zhongyouzk.top

std::vector<int> w = std::move(v);
来源：http://kni.sweek.top

[S54] C++：异常处理
来源：http://qrd.mhx1999.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fcp.zdqjudy.top

[S55] C++：结构化绑定
来源：http://jlo.smart0.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ytr.tian-w.cn

[S56] C++：optional
来源：http://wkm.hysaishi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://okk.kuanghao11.cn

[S57] C++：编译期常量
来源：http://vwb.epnwcf.com

constexpr int N = 10;
来源：http://evv.yfazqb.com

[S58] C++：命名空间
来源：http://zuo.cqqwz.cn

namespace ns { int f() { return 1; } }
来源：http://mwy.chenjidiqi.icu

[S59] C++：静态断言
来源：http://oac.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xrq.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://rkq.fehbvm.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jet.daria6918.cn

================================================================================
来源：http://mwt.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qcm.ehwqpu.com

================================================================================
来源：http://wzl.daxiang520.top

[T01] Kotlin：Hello World
来源：http://ddh.ydjk.org.cn

println("Hello")
来源：http://xsz.guowangkeji.top

[T02] Kotlin：变量
来源：http://pjq.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kfi.kuanghao11.cn

[T03] Kotlin：字符串模板
来源：http://dzi.jianghu66.top

"值: $b"
来源：http://rex.9152youxi.cn

[T04] Kotlin：空安全
来源：http://hqd.andypj.xyz

val n: String? = null;  n?.length
来源：http://nem.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://gsk.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://buq.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://oum.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ujh.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://eiq.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://irb.gogol.net.cn

[T08] Kotlin：数据类
来源：http://sem.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://zag.vehdjk.com

[T09] Kotlin：扩展函数
来源：http://gki.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://glw.hammf.cn

[T10] Kotlin：默认参数
来源：http://lpm.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vzn.9152youxi.cn

[T11] Kotlin：协程
来源：http://twj.yueranfly.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rvx.meibo888.top

[T12] Kotlin：解构声明
来源：http://twp.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://orh.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://wxt.yvedp.cn

val m = mapOf("a" to 1)
来源：http://nld.c1oappe.top

[T14] Kotlin：循环
来源：http://dmz.zhengqikj.top

for (i in 1..10) println(i)
来源：http://jfn.hysaishi.cn

[T15] Kotlin：接口
来源：http://ziv.wangshuangyany.cn

interface Shape { fun area(): Double }
来源：http://cml.jinghuilouyu.cn

[T16] Swift：Hello World
来源：http://kjx.jinqigfzy.top

print("Hello")
来源：http://xws.feifeiyinyue.top

[T17] Swift：变量与常量
来源：http://dwd.gogol.net.cn

var a = 1;  let b = 2
来源：http://asa.ppjwa.cn

[T18] Swift：字符串插值
来源：http://zbe.hnxiangtu.top

"值: \(b)"
来源：http://zfu.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://kgk.xziqi.cn

if let n = opt { print(n) }
来源：http://fhq.cheryme.top

[T20] Swift：数组操作
来源：http://rtc.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://szy.cqqwz.cn

[T21] Swift：遍历
来源：http://kem.chenlongwang.top

for x in a { print(x) }
来源：http://slx.cucudq.cn

[T22] Swift：字典
来源：http://mvz.chenzaomai.com

var d = ["a": 1];  d["b"] = 2
来源：http://iak.fehbvm.com

[T23] Swift：函数
来源：http://oii.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hyj.xziqi.cn

[T24] Swift：闭包
来源：http://ccq.meibo888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://uxt.nanxinkj.top

[T25] Swift：结构体
来源：http://fac.gotoacloud.top

struct P { var x: Int }
来源：http://qyk.zhijiandao.cn

[T26] Swift：类与重写
来源：http://dnn.aizwys.cn

class A: Base { override func f() {} }
来源：http://uyo.nwbrower.top

[T27] Swift：错误处理
来源：http://muz.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://rfi.shzxlz.cn

[T28] Swift：枚举
来源：http://yem.tarul.cn

enum Color { case red, green }
来源：http://nno.yonumen.top

[T29] Swift：guard 提前返回
来源：http://czr.zhoulong.xyz

guard let x = opt else { return }
来源：http://bdl.snrcjt.cn

[T30] Swift：协议
来源：http://vrm.fktsv.cn

protocol Shape { func area() -> Double }
来源：http://pcf.yvedp.cn

[T31] Lua：Hello World
来源：http://qqr.fengsongda.top

print("Hello")
来源：http://qfk.jiagoushi.top

[T32] Lua：局部变量
来源：http://wbx.dianchejie.cn

local a = 1
来源：http://lpt.yvedp.cn

[T33] Lua：表（数组）
来源：http://eyj.bjfxy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sav.tian-w.cn

[T34] Lua：遍历表
来源：http://dai.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://elh.daxiang520.top

[T35] Lua：字典表
来源：http://uhd.feifeiyinyue.top

local d = { a = 1 };  d.b = 2
来源：http://bsb.jiagoushi.top

[T36] Lua：函数
来源：http://jlp.epnwcf.com

function add(a, b) return a + b end
来源：http://uxg.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://awh.jiagoushi.top

"a" .. "b"
来源：http://snd.yj20258.top

[T38] Lua：条件
来源：http://ikw.zhongyouzk.top

if x > 0 then print("正") end
来源：http://cpd.zdbjq.cn

[T39] Lua：模式匹配
来源：http://msy.shangyingyoupin.top

string.find(s, "%d+")
来源：http://mwk.jinqigfzy.top

[T40] Lua：元表
来源：http://usa.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://irh.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://lcb.yanxiufei.cn

print "Hello\n";
来源：http://rly.nanxinkj.top

[T42] Perl：变量类型
来源：http://kat.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rsz.zhongyouzk.top

[T43] Perl：字符串插值
来源：http://okc.quarkkingdee.top

"值: $a"
来源：http://ssh.c1oappe.top

[T44] Perl：条件
来源：http://tmt.xuetiantiany.cn

if ($a > 0) { print "正"; }
来源：http://vac.fktsv.cn

[T45] Perl：数组遍历
来源：http://qxw.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://bqj.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://xhq.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mzn.wangdashe.top

[T47] Perl：正则捕获
来源：http://ndr.xuanzx.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://tzb.yj202588.top

[T48] Perl：正则替换
来源：http://ojw.tarul.cn

$s =~ s/old/new/g;
来源：http://hzz.hammf.cn

[T49] Perl：函数
来源：http://okf.hammf.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://epg.xziqi.cn

[T50] Perl：逐行读文件
来源：http://bkg.dianchejie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://iyr.bbcook.cn

while (my $line = <$fh>) { print $line; }
来源：http://fbo.smart0.xyz

[T51] Scala：Hello World
来源：http://zob.0kj1m.cn

println("Hello")
来源：http://kxx.yonumen.top

[T52] Scala：变量
来源：http://ime.kuanghao11.cn

val a = 1;  var b = 2
来源：http://rcw.nanxinkj.top

[T53] Scala：字符串插值
来源：http://ola.xziqi.cn

s"值: $b"
来源：http://vde.316326.xyz

[T54] Scala：集合映射
来源：http://tpk.sweek.top

List(1, 2, 3).map(_ * 2)
来源：http://lcx.cashguo.top

[T55] Scala：集合过滤
来源：http://wpu.wangshuangyany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vvv.316326.xyz

[T56] Scala：样例类
来源：http://cto.sysykeji.top

case class User(name: String, age: Int)
来源：http://mzm.cheryme.top

[T57] Scala：模式匹配
来源：http://hjf.dianchejie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vyg.yuanzhike.top

[T58] Scala：函数定义
来源：http://crw.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://lim.0kj1m.cn

[T59] Scala：循环
来源：http://fpr.tarul.cn

for (i <- 1 to 10) println(i)
来源：http://srk.jinqigfzy.top

[T60] Scala：折叠
来源：http://gwn.epnwcf.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hee.sysykeji.top

================================================================================
来源：http://qhu.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://boo.nanxinkj.top

================================================================================
来源：http://hwb.gzhubu.top

[U01] Py：创建虚拟环境
来源：http://ofv.ctjpmb.com

python -m venv .venv && source .venv/bin/activate
来源：http://eon.sweek.top

[U02] Py：导出 / 安装依赖
来源：http://jkq.fzhhl.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qzf.hongshengwenyu.top

[U03] Py：加载 .env 配置
来源：http://wbl.jinghuilouyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zcf.hnxiangtu.top

[U04] Py：变量调试打印
来源：http://sme.hammf.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ccs.ydzc1.top

[U05] Py：列表去重且保序
来源：http://odd.yuxming.cn

list(dict.fromkeys(arr))
来源：http://jgk.jinyuanbaomall.cn

[U06] Py：合并两个字典
来源：http://qsa.9152youxi.cn

{**a, **b}
来源：http://nys.nwbrower.top

[U07] Py：反转字典键值
来源：http://bxg.yueranfly.top

{v: k for k, v in d.items()}
来源：http://etp.zhoulong.xyz

[U08] Py：展平二维列表
来源：http://tqr.havefunace.top

[y for x in nested for y in x]
来源：http://osc.yfazqb.com

[U09] Py：字典取最大值的键
来源：http://fgf.cucudq.cn

max(d, key=d.get)
来源：http://jes.cdnleiting.top

[U10] Py：按值排序字典
来源：http://gpi.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lrr.wangshuangyany.cn


<!-- 参考信息 -->