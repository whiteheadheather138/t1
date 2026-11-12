代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://pva.smart0.xyz

[R70] 时间戳与互转
来源：http://xrq.andypj.xyz

date +%s;  date -d @1700000000
来源：http://ukm.birdmap.top

[R71] 日期格式化
来源：http://ttg.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://iba.epnwcf.com

[R72] 等待端口就绪
来源：http://wcv.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zeu.ctjpmb.com

[R73] 分割大日志
来源：http://ift.fzhhl.top

split -l 1000 big.log part_
来源：http://kzv.jqgufenzy.top

[R74] 批量重命名
来源：http://fnf.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fjr.uphjek.com

[R75] 导出环境变量
来源：http://zfg.chenlongwang.top

export PATH="$HOME/bin:$PATH"
来源：http://xmx.jinqigufen.top

[R76] 使用临时文件
来源：http://cgl.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://noo.dashuyun.cn

[R77] 读取用户输入
来源：http://bqr.dashuyun.cn

read -rp "请输入: " ans
来源：http://aug.daria6918.cn

[R78] 交互式菜单
来源：http://hmz.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ytl.jianghu66.top

[R79] 解析命令行选项
来源：http://knl.ybcxt.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aif.hysaishi.cn

[R80] 查看脚本执行耗时
来源：http://wcr.ehwqpu.com

time ./run.sh
来源：http://oca.zycfv.cn

================================================================================
来源：http://cfk.gaohongyu789.top

S. C / C++ 专题
来源：http://kyn.zhengqikj.top

================================================================================
来源：http://xmg.hnqzz.top

[S01] C：Hello World
来源：http://pkw.jqgfzy.top

#include <stdio.h>
来源：http://tnj.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ntr.iojbl.cn

[S02] C：变量与格式化输出
来源：http://brt.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://swn.shzxlz.cn

[S03] C：读入整数
来源：http://pde.yuanzhike.top

int x; scanf("%d", &x);
来源：http://nsu.cashguo.top

[S04] C：字符串复制
来源：http://esf.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ldf.sufxvd.cn

[S05] C：字符串长度
来源：http://eaz.shzxlz.cn

strlen(s)
来源：http://dms.havefunace.top

[S06] C：字符串比较
来源：http://nbi.yvedp.cn

strcmp(a, b) == 0
来源：http://koy.gogol.net.cn

[S07] C：数组遍历求和
来源：http://xng.cqqwz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zhw.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://nqh.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iac.zdqjudy.top

[S09] C：结构体定义与初始化
来源：http://dth.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://elt.yvedp.cn

[S10] C：指针与解引用
来源：http://tgv.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://sqy.c1oappe.top

[S11] C：逐行读文件
来源：http://uoh.yj202588.top

FILE *f = fopen("a.txt", "r");
来源：http://nvg.guannengcc.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kkm.fzhhl.top

fclose(f);
来源：http://avs.c1oappe.top

[S12] C：写文件
来源：http://qka.wangshuangyany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jda.sjlbkw.cn

[S13] C：宏定义
来源：http://lsp.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tsl.bjfxy.top

[S14] C：枚举
来源：http://ijp.jlsjyb.cn

enum Color { RED, GREEN, BLUE };
来源：http://jal.chenlongwang.top

[S15] C：类型转换
来源：http://yoy.bjfxy.top

(double) a / b
来源：http://rzr.zhoulong.xyz

[S16] C：位操作置位
来源：http://ern.hcnkem.com

x |= (1 << 3);
来源：http://urk.zhengqikj.top

[S17] C：安全拼接字符串
来源：http://rjz.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://suq.ywan-chungtsiang.top

[S18] C：命令行参数
来源：http://whd.gogol.net.cn

int main(int argc, char **argv)
来源：http://umr.andypj.xyz

[S19] C：快速排序
来源：http://zel.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fsu.daxiang520.top

[S20] C：二分查找
来源：http://cfp.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ghu.snrcjt.cn

[S21] C：字符类别判断
来源：http://dcw.sufxvd.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dhk.haohaochexian.top

[S22] C：字符串转数字
来源：http://nbs.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://qng.nanxuanxn.top

[S23] C：随机数
来源：http://lft.cqqwz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wqf.hywenlv.cn

[S24] C：获取本地时间
来源：http://wob.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://upb.jlsjyb.cn

[S25] C：内存拷贝
来源：http://hgh.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://ujj.zycfv.cn

[S26] C：内存清零
来源：http://piy.bbcook.cn

memset(a, 0, sizeof a);
来源：http://fey.snrcjt.cn

[S27] C：定义常量
来源：http://kai.smart0.xyz

const double PI = 3.14159;
来源：http://vxl.fanxiaobao.xyz

[S28] C：静态变量
来源：http://tfj.aibaodan.cn

static int counter = 0;
来源：http://une.wangdashe.top

[S29] C：变参函数
来源：http://scb.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ahe.feifeiyinyue.top

[S30] C：头文件保护
来源：http://dtd.ctjpmb.com

#ifndef X_H
来源：http://tym.ctjpmb.com

#define X_H
来源：http://kjq.xinyue.icu

#endif
来源：http://iik.hnxiangtu.top

[S31] C++：Hello World
来源：http://ohs.epnwcf.com

#include <iostream>
来源：http://bjy.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://pdn.ydjk.org.cn

[S32] C++：字符串
来源：http://tdg.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://por.aizwys.cn

[S33] C++：vector 增删
来源：http://rsd.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sbj.meibo888.top

[S34] C++：遍历 vector
来源：http://rac.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://hrm.jianghu66.top

[S35] C++：map
来源：http://cpk.guannengcc.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ssu.zhengqikj.top

[S36] C++：unordered_map
来源：http://vpe.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cyw.hfpthk.cn

[S37] C++：set
来源：http://odp.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lqe.yanxiufei.cn

[S38] C++：排序
来源：http://zgx.ivvv.top

std::sort(v.begin(), v.end());
来源：http://slb.meibo888.top

[S39] C++：自定义比较器排序
来源：http://qww.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mjj.hcnkem.com

[S40] C++：查找元素
来源：http://erw.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://woo.havefunace.top

[S41] C++：类与构造函数
来源：http://dps.yfazqb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hti.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://yac.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://nwn.jinqigfzy.top

[S43] C++：智能指针
来源：http://cwb.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://xpg.havefunace.top

[S44] C++：引用传参
来源：http://djr.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://hxn.hywenlv.cn

[S45] C++：lambda
来源：http://ocq.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jvq.yueranfly.top

[S46] C++：函数模板
来源：http://ega.xingfuxueyuan.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pwq.zhiwuduotai.top

[S47] C++：结构化绑定遍历
来源：http://top.c1oappe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zua.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://zhq.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://aiy.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://sof.hywenlv.cn

[S49] C++：写文件
来源：http://bps.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://spm.birdmap.top

[S50] C++：格式化数字
来源：http://ggu.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nlt.andypj.xyz

[S51] C++：显式类型转换
来源：http://iqa.c1oappe.top

static_cast<double>(a) / b
来源：http://rkv.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://esv.sysykeji.top

int size() const noexcept { return n_; }
来源：http://hwt.fzhhl.top

[S53] C++：移动语义
来源：http://szc.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://rfa.snrcjt.cn

[S54] C++：异常处理
来源：http://qcg.hnxiangtu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://icn.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://ohd.tanke756.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ovi.jinqigfzy.top

[S56] C++：optional
来源：http://ocz.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vxq.ivvv.top

[S57] C++：编译期常量
来源：http://cdl.pengpengdd.cyou

constexpr int N = 10;
来源：http://uzi.jiagoushi.top

[S58] C++：命名空间
来源：http://bym.zhijiandao.cn

namespace ns { int f() { return 1; } }
来源：http://yra.nanxuanxn.top

[S59] C++：静态断言
来源：http://arc.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ntv.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://jdz.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dql.zhengqikj.top

================================================================================
来源：http://rea.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xbb.andypj.xyz

================================================================================
来源：http://rws.svipenyu.cn

[T01] Kotlin：Hello World
来源：http://ddu.c1oappe.top

println("Hello")
来源：http://zlk.xinyue.icu

[T02] Kotlin：变量
来源：http://igr.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ubs.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://pyo.ybcxt.top

"值: $b"
来源：http://kqr.xziqi.cn

[T04] Kotlin：空安全
来源：http://lri.quarkkingdee.top

val n: String? = null;  n?.length
来源：http://que.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://jpa.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zau.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://zlk.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bxe.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://sfe.aibaodan.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rae.daxiang520.top

[T08] Kotlin：数据类
来源：http://hsg.yj202588.top

data class User(val name: String, val age: Int)
来源：http://hcf.vqdsnc.cn

[T09] Kotlin：扩展函数
来源：http://sye.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://lmw.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://aas.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://dty.zhixingplan.top

[T11] Kotlin：协程
来源：http://eea.feifeiyinyue.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rls.sxryk.cn

[T12] Kotlin：解构声明
来源：http://aob.kuanghao11.cn

val (a, b) = Pair(1, 2)
来源：http://lwj.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://cug.jlsjyb.cn

val m = mapOf("a" to 1)
来源：http://vuo.meibo888.top

[T14] Kotlin：循环
来源：http://amz.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://dwo.gaohongyu789.top

[T15] Kotlin：接口
来源：http://hxz.kuanghao11.cn

interface Shape { fun area(): Double }
来源：http://yyj.yuanzhike.top

[T16] Swift：Hello World
来源：http://klj.jinyuanbaomall.cn

print("Hello")
来源：http://rqj.gogol.net.cn

[T17] Swift：变量与常量
来源：http://ueu.snrcjt.cn

var a = 1;  let b = 2
来源：http://bze.bjfxy.top

[T18] Swift：字符串插值
来源：http://jkc.cucudq.cn

"值: \(b)"
来源：http://hra.hnxiangtu.top

[T19] Swift：可选绑定
来源：http://fgq.guannengcc.top

if let n = opt { print(n) }
来源：http://szn.hnqzz.top

[T20] Swift：数组操作
来源：http://rrs.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://bid.jianghu66.top

[T21] Swift：遍历
来源：http://gtv.yfazqb.com

for x in a { print(x) }
来源：http://bwy.cucudq.cn

[T22] Swift：字典
来源：http://laj.jiagoushi.top

var d = ["a": 1];  d["b"] = 2
来源：http://gcn.mhx1999.top

[T23] Swift：函数
来源：http://jfx.birdmap.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wmz.chenlongwang.top

[T24] Swift：闭包
来源：http://mvc.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hkg.yanxiufei.cn

[T25] Swift：结构体
来源：http://zjc.xylfe.cn

struct P { var x: Int }
来源：http://ivf.yj20258.top

[T26] Swift：类与重写
来源：http://ahv.yonumen.top

class A: Base { override func f() {} }
来源：http://ket.jianghu66.top

[T27] Swift：错误处理
来源：http://cme.yj20258.top

do { try f() } catch { print(error) }
来源：http://fun.jqgufenzy.top

[T28] Swift：枚举
来源：http://ugr.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://rfc.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://vve.birdmap.top

guard let x = opt else { return }
来源：http://cut.tianlin.xyz

[T30] Swift：协议
来源：http://zfq.uphjek.com

protocol Shape { func area() -> Double }
来源：http://jtj.ehwqpu.com

[T31] Lua：Hello World
来源：http://btd.yonumen.top

print("Hello")
来源：http://ejp.shanyushiyangtech.top

[T32] Lua：局部变量
来源：http://nnw.xylfe.cn

local a = 1
来源：http://sjb.jiagoushi.top

[T33] Lua：表（数组）
来源：http://xej.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://cfi.zhijiandao.cn

[T34] Lua：遍历表
来源：http://fdm.guowangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rey.cdnleiting.top

[T35] Lua：字典表
来源：http://vuq.xuetiantiany.cn

local d = { a = 1 };  d.b = 2
来源：http://nrw.hfpthk.cn

[T36] Lua：函数
来源：http://heg.yangfankeji.com

function add(a, b) return a + b end
来源：http://mlh.bjfxy.top

[T37] Lua：字符串拼接
来源：http://mif.xinyue.icu

"a" .. "b"
来源：http://ocf.smart0.xyz

[T38] Lua：条件
来源：http://efp.wangshuangyany.cn

if x > 0 then print("正") end
来源：http://efl.sweek.top

[T39] Lua：模式匹配
来源：http://qeg.zhaomingkeji.xyz

string.find(s, "%d+")
来源：http://rgr.cheryme.top

[T40] Lua：元表
来源：http://jwk.tanke756.top

setmetatable({}, { __index = base })
来源：http://viq.xuanzx.com

[T41] Perl：Hello World
来源：http://hnu.fehbvm.com

print "Hello\n";
来源：http://hqi.xuanzx.com

[T42] Perl：变量类型
来源：http://wvi.shanyushiyangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tjn.ydzc1.top

[T43] Perl：字符串插值
来源：http://nql.jlsjyb.cn

"值: $a"
来源：http://bbg.jlsjyb.cn

[T44] Perl：条件
来源：http://dhv.sweek.top

if ($a > 0) { print "正"; }
来源：http://btz.xuanzx.com

[T45] Perl：数组遍历
来源：http://ebq.pycfn.com

for my $x (@arr) { print $x; }
来源：http://nlo.hesvh.cn

[T46] Perl：哈希操作
来源：http://kki.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://isy.daria6918.cn

[T47] Perl：正则捕获
来源：http://rgs.sysykeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wnh.andypj.xyz

[T48] Perl：正则替换
来源：http://oqn.xuanzx.com

$s =~ s/old/new/g;
来源：http://voj.yanxiufei.cn

[T49] Perl：函数
来源：http://ohg.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fwl.0kj1m.cn

[T50] Perl：逐行读文件
来源：http://bbp.uphjek.com

open my $fh, "<", "a.txt" or die $!;
来源：http://qlf.guannengcc.top

while (my $line = <$fh>) { print $line; }
来源：http://fsm.sufxvd.cn

[T51] Scala：Hello World
来源：http://xnh.cheryme.top

println("Hello")
来源：http://onr.xylfe.cn

[T52] Scala：变量
来源：http://xer.jqgfzy.top

val a = 1;  var b = 2
来源：http://oks.tian-w.cn

[T53] Scala：字符串插值
来源：http://lit.hywenlv.cn

s"值: $b"
来源：http://inu.snrcjt.cn

[T54] Scala：集合映射
来源：http://qph.ehwqpu.com

List(1, 2, 3).map(_ * 2)
来源：http://ivx.sweek.top

[T55] Scala：集合过滤
来源：http://bwf.uphjek.com

List(1, 2, 3).filter(_ > 1)
来源：http://qgk.vqdsnc.cn

[T56] Scala：样例类
来源：http://jue.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://qio.tarul.cn

[T57] Scala：模式匹配
来源：http://ino.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://exa.ydjk.org.cn

[T58] Scala：函数定义
来源：http://one.jinqigufen.top

def add(a: Int, b: Int): Int = a + b
来源：http://vkx.jiagoushi.top

[T59] Scala：循环
来源：http://jdq.zdbjq.cn

for (i <- 1 to 10) println(i)
来源：http://tou.fktsv.cn

[T60] Scala：折叠
来源：http://tyh.9152youxi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qrx.yueranfly.top

================================================================================
来源：http://kun.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rcf.epnwcf.com

================================================================================
来源：http://eqm.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://hio.ybcxt.top

python -m venv .venv && source .venv/bin/activate
来源：http://cdl.xuanzx.com

[U02] Py：导出 / 安装依赖
来源：http://yhu.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xfb.hongshengwenyu.top

[U03] Py：加载 .env 配置
来源：http://dvd.quarkkingdee.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qzq.gotoacloud.top

[U04] Py：变量调试打印
来源：http://anx.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ztr.yueranfly.top

[U05] Py：列表去重且保序
来源：http://cgw.chenzaomai.com

list(dict.fromkeys(arr))
来源：http://rie.zycfv.cn

[U06] Py：合并两个字典
来源：http://eco.vqdsnc.cn

{**a, **b}
来源：http://pdb.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://qxh.uphjek.com

{v: k for k, v in d.items()}
来源：http://rix.svipenyu.cn

[U08] Py：展平二维列表
来源：http://zut.ivvv.top

[y for x in nested for y in x]
来源：http://okw.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://vwn.svipenyu.cn

max(d, key=d.get)
来源：http://xdu.sysykeji.top

[U10] Py：按值排序字典
来源：http://lrg.hammf.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hpf.jinghuilouyu.cn


<!-- 参考信息 -->