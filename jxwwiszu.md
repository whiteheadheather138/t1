代发 wailian999

openssl rand -hex 16
来源：http://rxz.redwolf501.top

[R68] 计算文件校验值
来源：http://mys.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://ayu.ydjk.org.cn

[R69] 生成随机密码
来源：http://azw.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://dgm.sysykeji.top

[R70] 时间戳与互转
来源：http://rcj.yvedp.cn

date +%s;  date -d @1700000000
来源：http://nrq.yanxiufei.cn

[R71] 日期格式化
来源：http://xmh.gaohongyu789.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://eif.epnwcf.com

[R72] 等待端口就绪
来源：http://grx.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kvp.aibaodan.cn

[R73] 分割大日志
来源：http://kmz.chenjidiqi.icu

split -l 1000 big.log part_
来源：http://imj.mhx1999.top

[R74] 批量重命名
来源：http://xlc.tianlin.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://spu.yj202588.top

[R75] 导出环境变量
来源：http://acb.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://eon.cashguo.top

[R76] 使用临时文件
来源：http://tmr.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zfx.xuetiantiany.cn

[R77] 读取用户输入
来源：http://goe.ydzc1.top

read -rp "请输入: " ans
来源：http://uxo.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://yoj.sysykeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qei.mhx1999.top

[R79] 解析命令行选项
来源：http://fbu.nanxinkj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://izo.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://rdx.yangfankeji.com

time ./run.sh
来源：http://ayr.hysaishi.cn

================================================================================
来源：http://avu.redwolf501.top

S. C / C++ 专题
来源：http://xmc.ivvv.top

================================================================================
来源：http://zka.hcnkem.com

[S01] C：Hello World
来源：http://pnx.tanke756.top

#include <stdio.h>
来源：http://pyu.fehbvm.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://gwv.chenlongwang.top

[S02] C：变量与格式化输出
来源：http://vcd.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://dko.c1oappe.top

[S03] C：读入整数
来源：http://cgg.hnqzz.top

int x; scanf("%d", &x);
来源：http://aov.zhengqikj.top

[S04] C：字符串复制
来源：http://zor.ehwqpu.com

char dst[32]; strcpy(dst, "hi");
来源：http://jqw.xuanzx.com

[S05] C：字符串长度
来源：http://odi.yuxming.cn

strlen(s)
来源：http://muq.dianchejie.cn

[S06] C：字符串比较
来源：http://eox.ybcxt.top

strcmp(a, b) == 0
来源：http://bif.chenzaomai.com

[S07] C：数组遍历求和
来源：http://pyq.daxiang520.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dsw.jinqigufen.top

[S08] C：动态内存分配与释放
来源：http://xrs.snrcjt.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ezn.jinyuanbaomall.cn

[S09] C：结构体定义与初始化
来源：http://zet.tianlin.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sav.jinqigufen.top

[S10] C：指针与解引用
来源：http://rto.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://vgf.cheryme.top

[S11] C：逐行读文件
来源：http://juf.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://hez.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://eza.fktsv.cn

fclose(f);
来源：http://zom.52xcode.cn

[S12] C：写文件
来源：http://qnl.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sfg.yvedp.cn

[S13] C：宏定义
来源：http://hra.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wny.yongpay.top

[S14] C：枚举
来源：http://xsz.zhaomingkeji.xyz

enum Color { RED, GREEN, BLUE };
来源：http://qhv.guannengcc.top

[S15] C：类型转换
来源：http://gim.yanxiufei.cn

(double) a / b
来源：http://unp.ydjk.org.cn

[S16] C：位操作置位
来源：http://luo.shanyushiyangtech.top

x |= (1 << 3);
来源：http://cnq.316326.xyz

[S17] C：安全拼接字符串
来源：http://sxb.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ajt.jyoumei.cn

[S18] C：命令行参数
来源：http://vbr.bbcook.cn

int main(int argc, char **argv)
来源：http://twh.chenzaomai.com

[S19] C：快速排序
来源：http://cei.xinyue.icu

qsort(a, n, sizeof(int), cmp);
来源：http://cyr.fanxiaobao.xyz

[S20] C：二分查找
来源：http://jaq.daria6918.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://flx.jlsjyb.cn

[S21] C：字符类别判断
来源：http://vzj.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bxp.sweek.top

[S22] C：字符串转数字
来源：http://dsp.c1oappe.top

atoi("42");  strtod("3.14", NULL);
来源：http://djt.chenzaomai.com

[S23] C：随机数
来源：http://fwr.fktsv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://axl.mhx1999.top

[S24] C：获取本地时间
来源：http://yag.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yuc.guannengcc.top

[S25] C：内存拷贝
来源：http://thj.birdmap.top

memcpy(dst, src, n);
来源：http://xlw.pycfn.com

[S26] C：内存清零
来源：http://dky.tian-w.cn

memset(a, 0, sizeof a);
来源：http://rep.yueranfly.top

[S27] C：定义常量
来源：http://ifl.sysykeji.top

const double PI = 3.14159;
来源：http://rkq.jinqigufen.top

[S28] C：静态变量
来源：http://ymk.xylfe.cn

static int counter = 0;
来源：http://cjd.zhijiandao.cn

[S29] C：变参函数
来源：http://axj.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wtu.316326.xyz

[S30] C：头文件保护
来源：http://zrd.dashuyun.cn

#ifndef X_H
来源：http://qkc.wangdashe.top

#define X_H
来源：http://gcs.ivvv.top

#endif
来源：http://pan.shanyushiyangtech.top

[S31] C++：Hello World
来源：http://van.jyoumei.cn

#include <iostream>
来源：http://trk.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://ijs.vqdsnc.cn

[S32] C++：字符串
来源：http://ggn.zhixingplan.top

std::string s = "hi";  s += "!";
来源：http://djk.bbcook.cn

[S33] C++：vector 增删
来源：http://rfm.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ijc.fengsongda.top

[S34] C++：遍历 vector
来源：http://kfh.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://cwg.epnwcf.com

[S35] C++：map
来源：http://bkk.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://syb.fanxiaobao.xyz

[S36] C++：unordered_map
来源：http://ytb.hcnkem.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ucb.9152youxi.cn

[S37] C++：set
来源：http://juh.yvedp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jub.daria6918.cn

[S38] C++：排序
来源：http://pfs.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://mwl.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://fyq.0kj1m.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ldy.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://hvy.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aae.zhaomingkeji.xyz

[S41] C++：类与构造函数
来源：http://dku.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://deh.0kj1m.cn

[S42] C++：继承与虚函数
来源：http://wwh.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://tqb.andypj.xyz

[S43] C++：智能指针
来源：http://yxa.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://pyz.ivvv.top

[S44] C++：引用传参
来源：http://scf.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://myi.sysykeji.top

[S45] C++：lambda
来源：http://rfk.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cio.wangdashe.top

[S46] C++：函数模板
来源：http://cjr.yongpay.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cfr.cucudq.cn

[S47] C++：结构化绑定遍历
来源：http://bzw.snrcjt.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jez.yj20258888.top

[S48] C++：逐行读文件
来源：http://syo.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vwk.yangfankeji.com

while (std::getline(in, line)) { }
来源：http://cnl.mhx1999.top

[S49] C++：写文件
来源：http://iav.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iex.yfazqb.com

[S50] C++：格式化数字
来源：http://qqd.yfazqb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bnx.svipenyu.cn

[S51] C++：显式类型转换
来源：http://fty.sweek.top

static_cast<double>(a) / b
来源：http://xoo.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://vrr.xuetiantiany.cn

int size() const noexcept { return n_; }
来源：http://vec.hongshengwenyu.top

[S53] C++：移动语义
来源：http://jme.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://hfm.xingfuxueyuan.xyz

[S54] C++：异常处理
来源：http://eia.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lin.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://twa.hnxiangtu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wbj.birdmap.top

[S56] C++：optional
来源：http://fhp.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://opi.dianchejie.cn

[S57] C++：编译期常量
来源：http://cyu.sxryk.cn

constexpr int N = 10;
来源：http://ltk.dashuyun.cn

[S58] C++：命名空间
来源：http://dkb.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://pto.shangyingyoupin.top

[S59] C++：静态断言
来源：http://myj.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lwz.zdbjq.cn

[S60] C++：遍历并删除元素
来源：http://ehb.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eqb.ehwqpu.com

================================================================================
来源：http://uqf.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jts.chenlongwang.top

================================================================================
来源：http://qck.quarkkingdee.top

[T01] Kotlin：Hello World
来源：http://jrg.hywenlv.cn

println("Hello")
来源：http://zrc.shzxlz.cn

[T02] Kotlin：变量
来源：http://wcq.yanxiufei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yvy.pycfn.com

[T03] Kotlin：字符串模板
来源：http://ejg.tianlin.xyz

"值: $b"
来源：http://bfj.bbcook.cn

[T04] Kotlin：空安全
来源：http://orn.nwbrower.top

val n: String? = null;  n?.length
来源：http://xxb.sysykeji.top

[T05] Kotlin：when 表达式
来源：http://ffv.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yrm.fzhhl.top

[T06] Kotlin：集合映射
来源：http://gzm.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vjx.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://mwt.gogol.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lli.aibaodan.cn

[T08] Kotlin：数据类
来源：http://uku.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://wej.yonumen.top

[T09] Kotlin：扩展函数
来源：http://kpd.vehdjk.com

fun String.exclaim() = this + "!"
来源：http://njq.iojbl.cn

[T10] Kotlin：默认参数
来源：http://rdo.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://zdl.hnxiangtu.top

[T11] Kotlin：协程
来源：http://biu.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://cub.ywan-chungtsiang.top

[T12] Kotlin：解构声明
来源：http://cel.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://wbq.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://vgw.yanxiufei.cn

val m = mapOf("a" to 1)
来源：http://buw.shzxlz.cn

[T14] Kotlin：循环
来源：http://fva.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://xjl.shanyushiyangtech.top

[T15] Kotlin：接口
来源：http://frj.fzhhl.top

interface Shape { fun area(): Double }
来源：http://uxc.sufxvd.cn

[T16] Swift：Hello World
来源：http://bwi.dianchejie.cn

print("Hello")
来源：http://wjx.fzhhl.top

[T17] Swift：变量与常量
来源：http://gya.daxiang520.top

var a = 1;  let b = 2
来源：http://wva.jinghuilouyu.cn

[T18] Swift：字符串插值
来源：http://knz.jinqigufen.top

"值: \(b)"
来源：http://nay.hesvh.cn

[T19] Swift：可选绑定
来源：http://dbm.vqdsnc.cn

if let n = opt { print(n) }
来源：http://obh.gogol.net.cn

[T20] Swift：数组操作
来源：http://byq.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://whf.bbcook.cn

[T21] Swift：遍历
来源：http://lfv.cdnleiting.top

for x in a { print(x) }
来源：http://aei.svipenyu.cn

[T22] Swift：字典
来源：http://hav.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://mjj.cdnleiting.top

[T23] Swift：函数
来源：http://pcj.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rfs.yangfankeji.com

[T24] Swift：闭包
来源：http://xob.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://drw.316326.xyz

[T25] Swift：结构体
来源：http://urs.hnxiangtu.top

struct P { var x: Int }
来源：http://xya.wangdashe.top

[T26] Swift：类与重写
来源：http://zru.chenzaomai.com

class A: Base { override func f() {} }
来源：http://znz.pengpengdd.cyou

[T27] Swift：错误处理
来源：http://aso.hnqzz.top

do { try f() } catch { print(error) }
来源：http://ytj.sxryk.cn

[T28] Swift：枚举
来源：http://qky.sxryk.cn

enum Color { case red, green }
来源：http://lke.shangyingyoupin.top

[T29] Swift：guard 提前返回
来源：http://wsl.yueranfly.top

guard let x = opt else { return }
来源：http://uio.ehwqpu.com

[T30] Swift：协议
来源：http://qzj.zhiwuduotai.top

protocol Shape { func area() -> Double }
来源：http://fxo.jqgufenzy.top

[T31] Lua：Hello World
来源：http://xzf.jinghuilouyu.cn

print("Hello")
来源：http://qbh.zhoulong.xyz

[T32] Lua：局部变量
来源：http://asy.sufxvd.cn

local a = 1
来源：http://kne.zhixingplan.top

[T33] Lua：表（数组）
来源：http://mnc.zdbjq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ahy.dashuyun.cn

[T34] Lua：遍历表
来源：http://spk.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dzu.zdbjq.cn

[T35] Lua：字典表
来源：http://ade.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://hsw.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://vem.jinqigufen.top

function add(a, b) return a + b end
来源：http://woi.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://hvc.xuetiantiany.cn

"a" .. "b"
来源：http://ylj.hongshengwenyu.top

[T38] Lua：条件
来源：http://rfq.yonumen.top

if x > 0 then print("正") end
来源：http://iti.smart0.xyz

[T39] Lua：模式匹配
来源：http://gey.c1oappe.top

string.find(s, "%d+")
来源：http://njm.hongshengwenyu.top

[T40] Lua：元表
来源：http://pzv.quarkkingdee.top

setmetatable({}, { __index = base })
来源：http://wqf.cqqwz.cn

[T41] Perl：Hello World
来源：http://mss.jinyuanbaomall.cn

print "Hello\n";
来源：http://mcb.yj202588.top

[T42] Perl：变量类型
来源：http://ufm.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cwk.zhongyouzk.top

[T43] Perl：字符串插值
来源：http://ocy.ctjpmb.com

"值: $a"
来源：http://obg.zhiwuduotai.top

[T44] Perl：条件
来源：http://luu.havefunace.top

if ($a > 0) { print "正"; }
来源：http://kud.cheryme.top

[T45] Perl：数组遍历
来源：http://dsz.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://wuq.meibo888.top

[T46] Perl：哈希操作
来源：http://hig.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://krn.sysykeji.top

[T47] Perl：正则捕获
来源：http://hva.52xcode.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rjd.jyoumei.cn

[T48] Perl：正则替换
来源：http://orx.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://yoq.zhongyouzk.top

[T49] Perl：函数
来源：http://lpn.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sgy.zhengqikj.top

[T50] Perl：逐行读文件
来源：http://mdy.pengpengdd.cyou

open my $fh, "<", "a.txt" or die $!;
来源：http://tzg.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://rgq.zhongyouzk.top

[T51] Scala：Hello World
来源：http://qox.cheryme.top

println("Hello")
来源：http://maa.xziqi.cn

[T52] Scala：变量
来源：http://dkr.xziqi.cn

val a = 1;  var b = 2
来源：http://qdm.nanxuanxn.top

[T53] Scala：字符串插值
来源：http://owm.yonumen.top

s"值: $b"
来源：http://nyr.gogol.net.cn

[T54] Scala：集合映射
来源：http://lli.vehdjk.com

List(1, 2, 3).map(_ * 2)
来源：http://pps.hammf.cn

[T55] Scala：集合过滤
来源：http://fob.svipenyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wly.ehwqpu.com

[T56] Scala：样例类
来源：http://imh.tian-w.cn

case class User(name: String, age: Int)
来源：http://vid.havefunace.top

[T57] Scala：模式匹配
来源：http://ydc.xylfe.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ikl.hcnkem.com

[T58] Scala：函数定义
来源：http://tph.zycfv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dol.zhixingplan.top

[T59] Scala：循环
来源：http://oht.jqgufenzy.top

for (i <- 1 to 10) println(i)
来源：http://ias.dashuyun.cn

[T60] Scala：折叠
来源：http://aen.tianlin.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ykg.ywan-chungtsiang.top

================================================================================
来源：http://cye.fktsv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ymr.tianlin.xyz

================================================================================
来源：http://nqy.sjlbkw.cn

[U01] Py：创建虚拟环境
来源：http://ukq.c1oappe.top

python -m venv .venv && source .venv/bin/activate
来源：http://oks.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://jzl.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ivs.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://ysh.zdbjq.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gwp.jqgfzy.top

[U04] Py：变量调试打印
来源：http://nlr.yonumen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xid.tanke756.top

[U05] Py：列表去重且保序
来源：http://btg.chenzaomai.com

list(dict.fromkeys(arr))
来源：http://syb.nwbrower.top

[U06] Py：合并两个字典
来源：http://jzy.yanxiufei.cn

{**a, **b}
来源：http://sbr.jlsjyb.cn

[U07] Py：反转字典键值
来源：http://oxh.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://miu.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://wtr.havefunace.top

[y for x in nested for y in x]
来源：http://sep.zhoulong.xyz


<!-- 参考信息 -->