代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://xfi.9152youxi.cn

[R70] 时间戳与互转
来源：http://anj.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://pbv.gaohongyu789.top

[R71] 日期格式化
来源：http://yws.hnqzz.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://osm.nwbrower.top

[R72] 等待端口就绪
来源：http://cep.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nkk.gaohongyu789.top

[R73] 分割大日志
来源：http://mcw.redwolf501.top

split -l 1000 big.log part_
来源：http://qix.smart0.xyz

[R74] 批量重命名
来源：http://mvt.cashguo.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ddr.yangfankeji.com

[R75] 导出环境变量
来源：http://fdb.jiagoushi.top

export PATH="$HOME/bin:$PATH"
来源：http://zwf.yuxming.cn

[R76] 使用临时文件
来源：http://zod.xinyue.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vnx.kuanghao11.cn

[R77] 读取用户输入
来源：http://asw.mhx1999.top

read -rp "请输入: " ans
来源：http://cdn.yangfankeji.com

[R78] 交互式菜单
来源：http://jzj.wangshuangyany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uvm.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://iip.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tfg.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://zej.hfpthk.cn

time ./run.sh
来源：http://esd.shanyushiyangkeji.top

================================================================================
来源：http://bpl.kuanghao11.cn

S. C / C++ 专题
来源：http://uih.cucudq.cn

================================================================================
来源：http://kcy.sysykeji.top

[S01] C：Hello World
来源：http://uan.hcnkem.com

#include <stdio.h>
来源：http://kxk.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://koe.tarul.cn

[S02] C：变量与格式化输出
来源：http://evs.ctjpmb.com

int a = 10; printf("%d\n", a);
来源：http://ceu.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://pwz.cucudq.cn

int x; scanf("%d", &x);
来源：http://peh.mhx1999.top

[S04] C：字符串复制
来源：http://mnh.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://rny.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://azj.yuxming.cn

strlen(s)
来源：http://esu.c1oappe.top

[S06] C：字符串比较
来源：http://znp.andypj.xyz

strcmp(a, b) == 0
来源：http://uom.gotoacloud.top

[S07] C：数组遍历求和
来源：http://vtz.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mee.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://gdo.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gdy.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://vwq.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://doc.mhx1999.top

[S10] C：指针与解引用
来源：http://ugr.wangshuangyany.cn

int *p = &a;  *p = 5;
来源：http://yza.jinqigufen.top

[S11] C：逐行读文件
来源：http://cjv.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://aek.yonumen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://uuh.jqgufenzy.top

fclose(f);
来源：http://swf.shuidangran.top

[S12] C：写文件
来源：http://roz.fengsongda.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://znj.chenzaomai.com

[S13] C：宏定义
来源：http://htf.yfazqb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://etf.vehdjk.com

[S14] C：枚举
来源：http://oqe.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://ybq.ivvv.top

[S15] C：类型转换
来源：http://swj.snrcjt.cn

(double) a / b
来源：http://dkg.ydjk.org.cn

[S16] C：位操作置位
来源：http://edl.wangdashe.top

x |= (1 << 3);
来源：http://zla.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://ivx.ybcxt.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gfy.bbcook.cn

[S18] C：命令行参数
来源：http://rws.pengpengdd.cyou

int main(int argc, char **argv)
来源：http://ylq.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://nfe.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://zmy.tianlin.xyz

[S20] C：二分查找
来源：http://lzx.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eyo.jiagoushi.top

[S21] C：字符类别判断
来源：http://awq.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://moi.sxryk.cn

[S22] C：字符串转数字
来源：http://adq.jlsjyb.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vlp.yuxming.cn

[S23] C：随机数
来源：http://onw.chenjidiqi.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://hmv.ctjpmb.com

[S24] C：获取本地时间
来源：http://kwj.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yek.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://xvd.sysykeji.top

memcpy(dst, src, n);
来源：http://npp.svipenyu.cn

[S26] C：内存清零
来源：http://pub.jinyuanbaomall.cn

memset(a, 0, sizeof a);
来源：http://tyv.ivvv.top

[S27] C：定义常量
来源：http://tmn.zhiwuduotai.top

const double PI = 3.14159;
来源：http://pkj.chenzaomai.com

[S28] C：静态变量
来源：http://nzj.tarul.cn

static int counter = 0;
来源：http://rye.aibaodan.cn

[S29] C：变参函数
来源：http://mqt.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eif.wangdashe.top

[S30] C：头文件保护
来源：http://mtc.xziqi.cn

#ifndef X_H
来源：http://bjd.pengpengdd.cyou

#define X_H
来源：http://wyt.sufxvd.cn

#endif
来源：http://iyl.xylfe.cn

[S31] C++：Hello World
来源：http://cag.hywenlv.cn

#include <iostream>
来源：http://aqf.zdqjudy.top

int main() { std::cout << "Hello\n"; }
来源：http://mzl.svipenyu.cn

[S32] C++：字符串
来源：http://rdu.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://exl.jiagoushi.top

[S33] C++：vector 增删
来源：http://wct.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gem.pycfn.com

[S34] C++：遍历 vector
来源：http://lwv.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://ext.ybcxt.top

[S35] C++：map
来源：http://ozk.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rsy.tarul.cn

[S36] C++：unordered_map
来源：http://pph.shzxlz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cxm.xingfuxueyuan.xyz

[S37] C++：set
来源：http://rze.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sdw.aizwys.cn

[S38] C++：排序
来源：http://rda.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://pce.hammf.cn

[S39] C++：自定义比较器排序
来源：http://bug.0kj1m.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ytp.yanxiufei.cn

[S40] C++：查找元素
来源：http://qli.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qyd.hnxiangtu.top

[S41] C++：类与构造函数
来源：http://rhu.jinqigfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://saw.bbcook.cn

[S42] C++：继承与虚函数
来源：http://ege.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://bne.yj202588.top

[S43] C++：智能指针
来源：http://uko.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://sbz.jinqigufen.top

[S44] C++：引用传参
来源：http://gua.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://xzx.ywan-chungtsiang.top

[S45] C++：lambda
来源：http://dmk.daxiang520.top

auto add = [](int a, int b) { return a + b; };
来源：http://fhr.xingfuxueyuan.xyz

[S46] C++：函数模板
来源：http://rym.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lae.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://fxa.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://khd.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://jys.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://zpg.redwolf501.top

while (std::getline(in, line)) { }
来源：http://vsr.daxiang520.top

[S49] C++：写文件
来源：http://dko.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kxl.yfazqb.com

[S50] C++：格式化数字
来源：http://fwh.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://prg.jinqigufen.top

[S51] C++：显式类型转换
来源：http://gbq.ivvv.top

static_cast<double>(a) / b
来源：http://xyw.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://eba.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://rby.dashuyun.cn

[S53] C++：移动语义
来源：http://awy.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://edl.nanxinkj.top

[S54] C++：异常处理
来源：http://hvx.epnwcf.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qwz.xziqi.cn

[S55] C++：结构化绑定
来源：http://oes.zhaomingkeji.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://sjg.daxiang520.top

[S56] C++：optional
来源：http://xdj.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wiu.tianlin.xyz

[S57] C++：编译期常量
来源：http://klv.yuxming.cn

constexpr int N = 10;
来源：http://auz.shangyingyoupin.top

[S58] C++：命名空间
来源：http://ueb.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://hwj.shuidangran.top

[S59] C++：静态断言
来源：http://jip.jinyuanbaomall.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xyt.pycfn.com

[S60] C++：遍历并删除元素
来源：http://amh.hnqzz.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ccz.jinyuanbaomall.cn

================================================================================
来源：http://cdu.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gxx.fengsongda.top

================================================================================
来源：http://znz.tarul.cn

[T01] Kotlin：Hello World
来源：http://aai.yuanzhike.top

println("Hello")
来源：http://qri.xuetiantiany.cn

[T02] Kotlin：变量
来源：http://gqt.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://doe.birdmap.top

[T03] Kotlin：字符串模板
来源：http://dsd.gzhubu.top

"值: $b"
来源：http://owf.sufxvd.cn

[T04] Kotlin：空安全
来源：http://ont.gotoacloud.top

val n: String? = null;  n?.length
来源：http://kwq.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://oyj.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xpm.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://vpu.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fnl.cashguo.top

[T07] Kotlin：集合过滤
来源：http://lqo.iojbl.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wli.xinyue.icu

[T08] Kotlin：数据类
来源：http://rpm.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://wvz.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://lsf.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://wbm.svipenyu.cn

[T10] Kotlin：默认参数
来源：http://tzv.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zil.yj20258.top

[T11] Kotlin：协程
来源：http://cop.pengpengdd.cyou

GlobalScope.launch { delay(1000); println("done") }
来源：http://leb.ivvv.top

[T12] Kotlin：解构声明
来源：http://suu.smart0.xyz

val (a, b) = Pair(1, 2)
来源：http://qme.havefunace.top

[T13] Kotlin：只读 Map
来源：http://aie.aizwys.cn

val m = mapOf("a" to 1)
来源：http://hih.0kj1m.cn

[T14] Kotlin：循环
来源：http://fll.yueranfly.top

for (i in 1..10) println(i)
来源：http://yuv.zhijiandao.cn

[T15] Kotlin：接口
来源：http://czi.jinqigufen.top

interface Shape { fun area(): Double }
来源：http://rku.sufxvd.cn

[T16] Swift：Hello World
来源：http://nyt.yongpay.top

print("Hello")
来源：http://tsr.zhixingplan.top

[T17] Swift：变量与常量
来源：http://rmp.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://asu.gzhubu.top

[T18] Swift：字符串插值
来源：http://iye.feifeiyinyue.top

"值: \(b)"
来源：http://bpj.fktsv.cn

[T19] Swift：可选绑定
来源：http://ohb.aibaodan.cn

if let n = opt { print(n) }
来源：http://aww.zhengqikj.top

[T20] Swift：数组操作
来源：http://gfs.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sxg.hnqzz.top

[T21] Swift：遍历
来源：http://rpn.gotoacloud.top

for x in a { print(x) }
来源：http://kll.bbcook.cn

[T22] Swift：字典
来源：http://dqb.mhx1999.top

var d = ["a": 1];  d["b"] = 2
来源：http://qdr.zhiwuduotai.top

[T23] Swift：函数
来源：http://twv.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xhb.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://agd.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zsk.jiagoushi.top

[T25] Swift：结构体
来源：http://hvw.sysykeji.top

struct P { var x: Int }
来源：http://lra.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://vus.gogol.net.cn

class A: Base { override func f() {} }
来源：http://yjz.pycfn.com

[T27] Swift：错误处理
来源：http://nib.guannengcc.top

do { try f() } catch { print(error) }
来源：http://cto.xziqi.cn

[T28] Swift：枚举
来源：http://dcq.fanxiaobao.xyz

enum Color { case red, green }
来源：http://kui.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://fqj.c1oappe.top

guard let x = opt else { return }
来源：http://xrr.yj202588.top

[T30] Swift：协议
来源：http://ypl.fzhhl.top

protocol Shape { func area() -> Double }
来源：http://tuu.0kj1m.cn

[T31] Lua：Hello World
来源：http://hug.yonumen.top

print("Hello")
来源：http://hdb.jlsjyb.cn

[T32] Lua：局部变量
来源：http://geh.cqqwz.cn

local a = 1
来源：http://dbc.yangfankeji.com

[T33] Lua：表（数组）
来源：http://dqw.sweek.top

local t = {1, 2, 3};  t[4] = 4
来源：http://imn.xylfe.cn

[T34] Lua：遍历表
来源：http://adl.ppjwa.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ujd.tianlin.xyz

[T35] Lua：字典表
来源：http://aus.ydjk.org.cn

local d = { a = 1 };  d.b = 2
来源：http://ehs.xuetiantiany.cn

[T36] Lua：函数
来源：http://znz.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://rnp.redwolf501.top

[T37] Lua：字符串拼接
来源：http://foh.zdqjudy.top

"a" .. "b"
来源：http://xvt.zhixingplan.top

[T38] Lua：条件
来源：http://xgn.smart0.xyz

if x > 0 then print("正") end
来源：http://rxh.zdbjq.cn

[T39] Lua：模式匹配
来源：http://jpc.sxryk.cn

string.find(s, "%d+")
来源：http://gyf.nanxuanxn.top

[T40] Lua：元表
来源：http://sln.gzhubu.top

setmetatable({}, { __index = base })
来源：http://ewg.shangyingyoupin.top

[T41] Perl：Hello World
来源：http://afu.jqgfzy.top

print "Hello\n";
来源：http://nty.ivvv.top

[T42] Perl：变量类型
来源：http://vyb.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://soz.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://duh.jinghuilouyu.cn

"值: $a"
来源：http://uys.jyoumei.cn

[T44] Perl：条件
来源：http://jhb.yvedp.cn

if ($a > 0) { print "正"; }
来源：http://cwg.tian-w.cn

[T45] Perl：数组遍历
来源：http://rnt.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://cbl.zhongyouzk.top

[T46] Perl：哈希操作
来源：http://sdd.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jmb.pengpengdd.cyou

[T47] Perl：正则捕获
来源：http://mhi.yuxming.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ief.shuidangran.top

[T48] Perl：正则替换
来源：http://rgn.tianlin.xyz

$s =~ s/old/new/g;
来源：http://fnd.yj20258888.top

[T49] Perl：函数
来源：http://mps.fktsv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bwg.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://rtl.jinghuilouyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pkv.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://ppc.gzhubu.top

[T51] Scala：Hello World
来源：http://svg.guannengcc.top

println("Hello")
来源：http://vjf.chenjidiqi.icu

[T52] Scala：变量
来源：http://uwv.aibaodan.cn

val a = 1;  var b = 2
来源：http://peu.xingfuxueyuan.xyz

[T53] Scala：字符串插值
来源：http://yhf.jinqigfzy.top

s"值: $b"
来源：http://dkg.xuanzx.com

[T54] Scala：集合映射
来源：http://lbr.cheryme.top

List(1, 2, 3).map(_ * 2)
来源：http://ask.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://sfa.ydjk.org.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dkk.mhx1999.top

[T56] Scala：样例类
来源：http://iqh.yvedp.cn

case class User(name: String, age: Int)
来源：http://rfr.yvedp.cn

[T57] Scala：模式匹配
来源：http://bkw.svipenyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mbz.ppjwa.cn

[T58] Scala：函数定义
来源：http://cxc.aizwys.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qif.hywenlv.cn

[T59] Scala：循环
来源：http://rph.yonumen.top

for (i <- 1 to 10) println(i)
来源：http://czk.hywenlv.cn

[T60] Scala：折叠
来源：http://gdm.hysaishi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uqw.snrcjt.cn

================================================================================
来源：http://xzh.zycfv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ach.ydzc1.top

================================================================================
来源：http://yhj.sweek.top

[U01] Py：创建虚拟环境
来源：http://iiq.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://oyu.cdnleiting.top

[U02] Py：导出 / 安装依赖
来源：http://qdy.aizwys.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pts.birdmap.top

[U03] Py：加载 .env 配置
来源：http://qbx.andypj.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://xdx.xuanzx.com

[U04] Py：变量调试打印
来源：http://yor.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qdl.yuxming.cn

[U05] Py：列表去重且保序
来源：http://mqt.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://pob.shzxlz.cn

[U06] Py：合并两个字典
来源：http://ccm.mhx1999.top

{**a, **b}
来源：http://uui.sweek.top

[U07] Py：反转字典键值
来源：http://fte.redwolf501.top

{v: k for k, v in d.items()}
来源：http://zmp.tarul.cn

[U08] Py：展平二维列表
来源：http://rwy.jinqigfzy.top

[y for x in nested for y in x]
来源：http://rws.sxryk.cn

[U09] Py：字典取最大值的键
来源：http://qys.aibaodan.cn

max(d, key=d.get)
来源：http://mfc.shzxlz.cn

[U10] Py：按值排序字典
来源：http://xsm.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ipa.ydzc1.top


<!-- 参考信息 -->