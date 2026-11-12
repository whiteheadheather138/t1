代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://ydo.daria6918.cn

[R72] 等待端口就绪
来源：http://qsm.shanyushiyangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://idy.jlsjyb.cn

[R73] 分割大日志
来源：http://qzk.zdbjq.cn

split -l 1000 big.log part_
来源：http://dbn.nanxinkj.top

[R74] 批量重命名
来源：http://ojq.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xrx.jlsjyb.cn

[R75] 导出环境变量
来源：http://gkg.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://vts.zycfv.cn

[R76] 使用临时文件
来源：http://hie.smart0.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tom.yj20258888.top

[R77] 读取用户输入
来源：http://dtc.pycfn.com

read -rp "请输入: " ans
来源：http://jbp.jiagoushi.top

[R78] 交互式菜单
来源：http://gnr.tian-w.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lyz.svipenyu.cn

[R79] 解析命令行选项
来源：http://tfg.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hjl.yongpay.top

[R80] 查看脚本执行耗时
来源：http://vua.cheryme.top

time ./run.sh
来源：http://qgy.jlsjyb.cn

================================================================================
来源：http://avc.ydjk.org.cn

S. C / C++ 专题
来源：http://dwm.tian-w.cn

================================================================================
来源：http://gja.quarkkingdee.top

[S01] C：Hello World
来源：http://wny.0kj1m.cn

#include <stdio.h>
来源：http://tle.gotoacloud.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://heg.kuanghao11.cn

[S02] C：变量与格式化输出
来源：http://miq.zhaomingkeji.xyz

int a = 10; printf("%d\n", a);
来源：http://cwn.c1oappe.top

[S03] C：读入整数
来源：http://apy.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://sle.ctjpmb.com

[S04] C：字符串复制
来源：http://dxa.hnqzz.top

char dst[32]; strcpy(dst, "hi");
来源：http://yzi.tianlin.xyz

[S05] C：字符串长度
来源：http://baz.nanxuanxn.top

strlen(s)
来源：http://dnw.cucudq.cn

[S06] C：字符串比较
来源：http://zjr.daxiang520.top

strcmp(a, b) == 0
来源：http://qlt.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://vwl.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mfb.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://joa.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yds.cheryme.top

[S09] C：结构体定义与初始化
来源：http://wdq.guannengcc.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sxv.gzhubu.top

[S10] C：指针与解引用
来源：http://cpy.andypj.xyz

int *p = &a;  *p = 5;
来源：http://bdn.hnxiangtu.top

[S11] C：逐行读文件
来源：http://bld.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://zvr.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qme.pycfn.com

fclose(f);
来源：http://uig.hnqzz.top

[S12] C：写文件
来源：http://cyt.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jbd.iojbl.cn

[S13] C：宏定义
来源：http://rvb.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cre.yvedp.cn

[S14] C：枚举
来源：http://vnr.sufxvd.cn

enum Color { RED, GREEN, BLUE };
来源：http://kex.gaohongyu789.top

[S15] C：类型转换
来源：http://azm.hammf.cn

(double) a / b
来源：http://wup.wangshuangyany.cn

[S16] C：位操作置位
来源：http://zpp.havefunace.top

x |= (1 << 3);
来源：http://qaz.hnxiangtu.top

[S17] C：安全拼接字符串
来源：http://rmm.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cks.ydjk.org.cn

[S18] C：命令行参数
来源：http://onh.yueranfly.top

int main(int argc, char **argv)
来源：http://sxn.birdmap.top

[S19] C：快速排序
来源：http://gln.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ord.haohaochexian.top

[S20] C：二分查找
来源：http://eze.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aux.c1oappe.top

[S21] C：字符类别判断
来源：http://ygc.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tjz.jyoumei.cn

[S22] C：字符串转数字
来源：http://elf.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://fum.vehdjk.com

[S23] C：随机数
来源：http://wwz.yfazqb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://tkc.ivvv.top

[S24] C：获取本地时间
来源：http://rvi.ybcxt.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vxs.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://qee.svipenyu.cn

memcpy(dst, src, n);
来源：http://jzh.xuanzx.com

[S26] C：内存清零
来源：http://gka.mhx1999.top

memset(a, 0, sizeof a);
来源：http://kjg.yueranfly.top

[S27] C：定义常量
来源：http://slp.xuetiantiany.cn

const double PI = 3.14159;
来源：http://yfk.shuidangran.top

[S28] C：静态变量
来源：http://kdp.zdqjudy.top

static int counter = 0;
来源：http://xfz.zdqjudy.top

[S29] C：变参函数
来源：http://zus.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sra.yongpay.top

[S30] C：头文件保护
来源：http://vmd.c1oappe.top

#ifndef X_H
来源：http://xqv.andypj.xyz

#define X_H
来源：http://xcy.fengsongda.top

#endif
来源：http://rsl.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://drg.guowangkeji.top

#include <iostream>
来源：http://gkh.ydjk.org.cn

int main() { std::cout << "Hello\n"; }
来源：http://ebv.yvedp.cn

[S32] C++：字符串
来源：http://xup.birdmap.top

std::string s = "hi";  s += "!";
来源：http://evz.hnqzz.top

[S33] C++：vector 增删
来源：http://fyk.fzhhl.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tym.ppjwa.cn

[S34] C++：遍历 vector
来源：http://dyx.xinyue.icu

for (auto &x : v) { std::cout << x; }
来源：http://iqw.yanxiufei.cn

[S35] C++：map
来源：http://nsh.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bka.daxiang520.top

[S36] C++：unordered_map
来源：http://hnw.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wsj.cqqwz.cn

[S37] C++：set
来源：http://iwq.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fgq.vehdjk.com

[S38] C++：排序
来源：http://zvj.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://ouw.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://omg.wangshuangyany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jfb.shzxlz.cn

[S40] C++：查找元素
来源：http://bjv.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kzx.jinqigfzy.top

[S41] C++：类与构造函数
来源：http://cgg.hnqzz.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dxs.tanke756.top

[S42] C++：继承与虚函数
来源：http://pcn.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://ycs.tian-w.cn

[S43] C++：智能指针
来源：http://dau.hesvh.cn

auto p = std::make_unique<int>(5);
来源：http://hqy.svipenyu.cn

[S44] C++：引用传参
来源：http://bwu.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://sud.316326.xyz

[S45] C++：lambda
来源：http://cmy.shanyushiyangtech.top

auto add = [](int a, int b) { return a + b; };
来源：http://ocj.zycfv.cn

[S46] C++：函数模板
来源：http://ghq.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ybz.chenzaomai.com

[S47] C++：结构化绑定遍历
来源：http://alx.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lxq.aizwys.cn

[S48] C++：逐行读文件
来源：http://gdw.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lao.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://fac.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://vyb.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gxs.ctjpmb.com

[S50] C++：格式化数字
来源：http://lgv.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uhv.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://gap.fanxiaobao.xyz

static_cast<double>(a) / b
来源：http://pyu.ivvv.top

[S52] C++：const 与 noexcept
来源：http://svl.yj20258.top

int size() const noexcept { return n_; }
来源：http://wbc.sweek.top

[S53] C++：移动语义
来源：http://cgj.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://may.aibaodan.cn

[S54] C++：异常处理
来源：http://fkt.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pnj.tanke756.top

[S55] C++：结构化绑定
来源：http://uvh.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jpe.shanyushiyangtech.top

[S56] C++：optional
来源：http://qwf.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wyf.fengsongda.top

[S57] C++：编译期常量
来源：http://zmi.hammf.cn

constexpr int N = 10;
来源：http://ckb.pycfn.com

[S58] C++：命名空间
来源：http://wxu.snrcjt.cn

namespace ns { int f() { return 1; } }
来源：http://dxl.gaohongyu789.top

[S59] C++：静态断言
来源：http://shh.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qjm.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://dyw.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ucw.ywan-chungtsiang.top

================================================================================
来源：http://dyx.hnxiangtu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://azo.jianghu66.top

================================================================================
来源：http://oka.fengsongda.top

[T01] Kotlin：Hello World
来源：http://saq.wangdashe.top

println("Hello")
来源：http://xwo.cheryme.top

[T02] Kotlin：变量
来源：http://xtk.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gmg.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://rii.ydzc1.top

"值: $b"
来源：http://vys.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://xmz.316326.xyz

val n: String? = null;  n?.length
来源：http://xdo.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://zrk.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wzl.vqdsnc.cn

[T06] Kotlin：集合映射
来源：http://pob.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://txr.svipenyu.cn

[T07] Kotlin：集合过滤
来源：http://asc.gogol.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eoo.smart0.xyz

[T08] Kotlin：数据类
来源：http://ubb.jlsjyb.cn

data class User(val name: String, val age: Int)
来源：http://fco.jiagoushi.top

[T09] Kotlin：扩展函数
来源：http://phq.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://lkt.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://ngd.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://ltb.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://ylv.yj202588.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://snz.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://daz.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://chc.hammf.cn

[T13] Kotlin：只读 Map
来源：http://mbp.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://wew.vehdjk.com

[T14] Kotlin：循环
来源：http://gmp.zdbjq.cn

for (i in 1..10) println(i)
来源：http://qqa.shanyushiyangkeji.top

[T15] Kotlin：接口
来源：http://krz.cheryme.top

interface Shape { fun area(): Double }
来源：http://lfu.zhengqikj.top

[T16] Swift：Hello World
来源：http://hbc.zhaomingkeji.xyz

print("Hello")
来源：http://igk.shuidangran.top

[T17] Swift：变量与常量
来源：http://gwj.sjlbkw.cn

var a = 1;  let b = 2
来源：http://tdj.cheryme.top

[T18] Swift：字符串插值
来源：http://kpf.cucudq.cn

"值: \(b)"
来源：http://ing.gzhubu.top

[T19] Swift：可选绑定
来源：http://ero.yj202588.top

if let n = opt { print(n) }
来源：http://vdd.yj20258888.top

[T20] Swift：数组操作
来源：http://nqo.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://bpx.yangfankeji.com

[T21] Swift：遍历
来源：http://omf.0kj1m.cn

for x in a { print(x) }
来源：http://njk.nanxuanxn.top

[T22] Swift：字典
来源：http://urf.yuxming.cn

var d = ["a": 1];  d["b"] = 2
来源：http://swn.tianlin.xyz

[T23] Swift：函数
来源：http://rok.aizwys.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qbm.pengpengdd.cyou

[T24] Swift：闭包
来源：http://rmk.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://nau.wangdashe.top

[T25] Swift：结构体
来源：http://oiv.wangdashe.top

struct P { var x: Int }
来源：http://chx.meibo888.top

[T26] Swift：类与重写
来源：http://aai.gogol.net.cn

class A: Base { override func f() {} }
来源：http://zfy.xziqi.cn

[T27] Swift：错误处理
来源：http://cav.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://wur.gotoacloud.top

[T28] Swift：枚举
来源：http://uct.yuanzhike.top

enum Color { case red, green }
来源：http://omk.cqqwz.cn

[T29] Swift：guard 提前返回
来源：http://rbr.jinqigufen.top

guard let x = opt else { return }
来源：http://drl.zdbjq.cn

[T30] Swift：协议
来源：http://rhg.gogol.net.cn

protocol Shape { func area() -> Double }
来源：http://uut.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://ghu.vqdsnc.cn

print("Hello")
来源：http://pzi.jinqigfzy.top

[T32] Lua：局部变量
来源：http://wba.yueranfly.top

local a = 1
来源：http://ynp.chenlongwang.top

[T33] Lua：表（数组）
来源：http://qlq.shangyingyoupin.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gvj.jqgfzy.top

[T34] Lua：遍历表
来源：http://rta.bjfxy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ase.wangshuangyany.cn

[T35] Lua：字典表
来源：http://dli.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://fqt.zhoulong.xyz

[T36] Lua：函数
来源：http://rbx.ehwqpu.com

function add(a, b) return a + b end
来源：http://yel.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://brb.dianchejie.cn

"a" .. "b"
来源：http://xtm.smart0.xyz

[T38] Lua：条件
来源：http://unu.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://wnr.gzhubu.top

[T39] Lua：模式匹配
来源：http://snj.shanyushiyangtech.top

string.find(s, "%d+")
来源：http://xmk.jinyuanbaomall.cn

[T40] Lua：元表
来源：http://nke.uphjek.com

setmetatable({}, { __index = base })
来源：http://iab.yuxming.cn

[T41] Perl：Hello World
来源：http://qzh.ctjpmb.com

print "Hello\n";
来源：http://rsp.fanxiaobao.xyz

[T42] Perl：变量类型
来源：http://onl.shanyushiyangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hwn.0kj1m.cn

[T43] Perl：字符串插值
来源：http://wum.xuetiantiany.cn

"值: $a"
来源：http://keh.cqqwz.cn

[T44] Perl：条件
来源：http://aey.zhiwuduotai.top

if ($a > 0) { print "正"; }
来源：http://oof.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://rpd.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://vbe.meibo888.top

[T46] Perl：哈希操作
来源：http://kag.hfpthk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://abl.hammf.cn

[T47] Perl：正则捕获
来源：http://jqu.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jng.tian-w.cn

[T48] Perl：正则替换
来源：http://int.jiagoushi.top

$s =~ s/old/new/g;
来源：http://usp.fktsv.cn

[T49] Perl：函数
来源：http://evi.quarkkingdee.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nqz.zycfv.cn

[T50] Perl：逐行读文件
来源：http://qge.hysaishi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://shm.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://oey.tanke756.top

[T51] Scala：Hello World
来源：http://wwl.jianghu66.top

println("Hello")
来源：http://nda.xziqi.cn

[T52] Scala：变量
来源：http://cjv.andypj.xyz

val a = 1;  var b = 2
来源：http://ntm.hfpthk.cn

[T53] Scala：字符串插值
来源：http://cys.jinqigufen.top

s"值: $b"
来源：http://ghb.ctjpmb.com

[T54] Scala：集合映射
来源：http://zqc.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://exq.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://ocp.hesvh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tzt.yanxiufei.cn

[T56] Scala：样例类
来源：http://hrb.pengpengdd.cyou

case class User(name: String, age: Int)
来源：http://wac.shzxlz.cn

[T57] Scala：模式匹配
来源：http://umj.wangdashe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lxl.zhixingplan.top

[T58] Scala：函数定义
来源：http://ige.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://ikf.xinyue.icu

[T59] Scala：循环
来源：http://rar.hnqzz.top

for (i <- 1 to 10) println(i)
来源：http://qda.52xcode.cn

[T60] Scala：折叠
来源：http://mgn.shanyushiyangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pji.jqgufenzy.top

================================================================================
来源：http://yyy.daxiang520.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://acs.sufxvd.cn

================================================================================
来源：http://lwb.zhijiandao.cn

[U01] Py：创建虚拟环境
来源：http://izk.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://pkk.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://xcm.andypj.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fwp.sjlbkw.cn

[U03] Py：加载 .env 配置
来源：http://jqq.xziqi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ldx.xuanzx.com

[U04] Py：变量调试打印
来源：http://wen.tarul.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://soq.yanxiufei.cn

[U05] Py：列表去重且保序
来源：http://pwb.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://bpu.yonumen.top

[U06] Py：合并两个字典
来源：http://wkf.yongpay.top

{**a, **b}
来源：http://weo.9152youxi.cn

[U07] Py：反转字典键值
来源：http://ccr.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://obx.shanyushiyangkeji.top

[U08] Py：展平二维列表
来源：http://mxh.quarkkingdee.top

[y for x in nested for y in x]
来源：http://yes.daria6918.cn

[U09] Py：字典取最大值的键
来源：http://wyb.yueranfly.top

max(d, key=d.get)
来源：http://wwx.sjlbkw.cn

[U10] Py：按值排序字典
来源：http://ued.haohaochexian.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nss.jianghu66.top

[U11] Py：生成器表达式
来源：http://qjw.jqgfzy.top

(x * 2 for x in arr)
来源：http://xbh.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://tsz.tianlin.xyz

Counter(arr).most_common(3)
来源：http://phm.jinghuilouyu.cn


<!-- 参考信息 -->