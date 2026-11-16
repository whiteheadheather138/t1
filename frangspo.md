代发 wailian999

split -l 1000 big.log part_
来源：http://dyy.yueranfly.top

[R74] 批量重命名
来源：http://jzo.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rty.yfazqb.com

[R75] 导出环境变量
来源：http://ivt.jinghuilouyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://irw.zycfv.cn

[R76] 使用临时文件
来源：http://tbv.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yxz.nanxinkj.top

[R77] 读取用户输入
来源：http://bkv.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://zbe.shuidangran.top

[R78] 交互式菜单
来源：http://lgo.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kna.xziqi.cn

[R79] 解析命令行选项
来源：http://elj.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fja.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://cjk.gzhubu.top

time ./run.sh
来源：http://kqu.havefunace.top

================================================================================
来源：http://lzc.jlsjyb.cn

S. C / C++ 专题
来源：http://hps.chenjidiqi.icu

================================================================================
来源：http://zit.gzhubu.top

[S01] C：Hello World
来源：http://nlx.zhongyouzk.top

#include <stdio.h>
来源：http://bin.epnwcf.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://qtn.hesvh.cn

[S02] C：变量与格式化输出
来源：http://pkw.jqgufenzy.top

int a = 10; printf("%d\n", a);
来源：http://epr.redwolf501.top

[S03] C：读入整数
来源：http://swa.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://duk.jqgfzy.top

[S04] C：字符串复制
来源：http://wlj.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fxl.zycfv.cn

[S05] C：字符串长度
来源：http://xtu.cqqwz.cn

strlen(s)
来源：http://jqi.jiagoushi.top

[S06] C：字符串比较
来源：http://iic.jyoumei.cn

strcmp(a, b) == 0
来源：http://imo.yj202588.top

[S07] C：数组遍历求和
来源：http://xrg.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wil.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://dem.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xio.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://hbu.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ykh.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://cuu.yuxming.cn

int *p = &a;  *p = 5;
来源：http://kig.jyoumei.cn

[S11] C：逐行读文件
来源：http://hnd.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://ufu.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://pge.daxiang520.top

fclose(f);
来源：http://csw.xuetiantiany.cn

[S12] C：写文件
来源：http://wtg.ehwqpu.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://swb.fktsv.cn

[S13] C：宏定义
来源：http://gif.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cez.dashuyun.cn

[S14] C：枚举
来源：http://jmx.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://zmi.9152youxi.cn

[S15] C：类型转换
来源：http://alc.ehwqpu.com

(double) a / b
来源：http://tmo.guannengcc.top

[S16] C：位操作置位
来源：http://idx.sufxvd.cn

x |= (1 << 3);
来源：http://ldi.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://pno.yj202588.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mzg.smart0.xyz

[S18] C：命令行参数
来源：http://bql.shzxlz.cn

int main(int argc, char **argv)
来源：http://pxy.gaohongyu789.top

[S19] C：快速排序
来源：http://uti.nwbrower.top

qsort(a, n, sizeof(int), cmp);
来源：http://ujs.guowangkeji.top

[S20] C：二分查找
来源：http://lro.quarkkingdee.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rmr.ybcxt.top

[S21] C：字符类别判断
来源：http://gml.hysaishi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qsf.zdbjq.cn

[S22] C：字符串转数字
来源：http://rrj.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ukb.gotoacloud.top

[S23] C：随机数
来源：http://ods.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ynu.yangfankeji.com

[S24] C：获取本地时间
来源：http://kug.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yud.jinqigfzy.top

[S25] C：内存拷贝
来源：http://pyq.ctjpmb.com

memcpy(dst, src, n);
来源：http://hpu.iojbl.cn

[S26] C：内存清零
来源：http://kjt.zycfv.cn

memset(a, 0, sizeof a);
来源：http://kcz.sxryk.cn

[S27] C：定义常量
来源：http://sdd.smart0.xyz

const double PI = 3.14159;
来源：http://tvz.fehbvm.com

[S28] C：静态变量
来源：http://avz.feifeiyinyue.top

static int counter = 0;
来源：http://orb.jinqigufen.top

[S29] C：变参函数
来源：http://kzt.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pjz.sweek.top

[S30] C：头文件保护
来源：http://eoc.havefunace.top

#ifndef X_H
来源：http://ofz.yj20258.top

#define X_H
来源：http://cfn.havefunace.top

#endif
来源：http://qlh.0kj1m.cn

[S31] C++：Hello World
来源：http://hho.xziqi.cn

#include <iostream>
来源：http://uyf.svipenyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://fpe.ctjpmb.com

[S32] C++：字符串
来源：http://wdz.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://myg.bjfxy.top

[S33] C++：vector 增删
来源：http://pld.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ayz.yfazqb.com

[S34] C++：遍历 vector
来源：http://hnz.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://irg.ybcxt.top

[S35] C++：map
来源：http://snl.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iql.snrcjt.cn

[S36] C++：unordered_map
来源：http://dvv.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://own.gaohongyu789.top

[S37] C++：set
来源：http://rzx.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iiw.9152youxi.cn

[S38] C++：排序
来源：http://ofw.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://mhq.iojbl.cn

[S39] C++：自定义比较器排序
来源：http://wou.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tid.nanxinkj.top

[S40] C++：查找元素
来源：http://jsv.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kgf.chenzaomai.com

[S41] C++：类与构造函数
来源：http://wzi.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uqg.pycfn.com

[S42] C++：继承与虚函数
来源：http://tmg.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://lzn.jiagoushi.top

[S43] C++：智能指针
来源：http://jrr.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://gft.pycfn.com

[S44] C++：引用传参
来源：http://wuj.nanxinkj.top

void inc(int &x) { ++x; }
来源：http://rxp.fehbvm.com

[S45] C++：lambda
来源：http://vpt.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://jns.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://krm.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sjs.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://mui.aizwys.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wcv.hesvh.cn

[S48] C++：逐行读文件
来源：http://cwy.tianlin.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://nic.yfazqb.com

while (std::getline(in, line)) { }
来源：http://twq.yvedp.cn

[S49] C++：写文件
来源：http://tdh.sufxvd.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://laz.nanxinkj.top

[S50] C++：格式化数字
来源：http://xcp.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zfj.jinqigufen.top

[S51] C++：显式类型转换
来源：http://hyn.meibo888.top

static_cast<double>(a) / b
来源：http://jbi.sufxvd.cn

[S52] C++：const 与 noexcept
来源：http://smz.bbcook.cn

int size() const noexcept { return n_; }
来源：http://pck.xinyue.icu

[S53] C++：移动语义
来源：http://zvr.pycfn.com

std::vector<int> w = std::move(v);
来源：http://qym.shangyingyoupin.top

[S54] C++：异常处理
来源：http://jkx.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://trx.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://yjr.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zsp.feifeiyinyue.top

[S56] C++：optional
来源：http://yci.gotoacloud.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://amq.guannengcc.top

[S57] C++：编译期常量
来源：http://ecm.shanyushiyangtech.top

constexpr int N = 10;
来源：http://cbj.cdnleiting.top

[S58] C++：命名空间
来源：http://hej.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://ylr.dianchejie.cn

[S59] C++：静态断言
来源：http://xff.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hin.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://peu.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aad.shzxlz.cn

================================================================================
来源：http://pyk.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://heh.hnqzz.top

================================================================================
来源：http://abu.feifeiyinyue.top

[T01] Kotlin：Hello World
来源：http://kln.zdqjudy.top

println("Hello")
来源：http://edc.vqdsnc.cn

[T02] Kotlin：变量
来源：http://eqp.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vfy.xziqi.cn

[T03] Kotlin：字符串模板
来源：http://qbz.zhijiandao.cn

"值: $b"
来源：http://isk.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://qgj.sufxvd.cn

val n: String? = null;  n?.length
来源：http://ayn.cucudq.cn

[T05] Kotlin：when 表达式
来源：http://iav.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pxz.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://upq.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mst.guannengcc.top

[T07] Kotlin：集合过滤
来源：http://pbi.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bei.sufxvd.cn

[T08] Kotlin：数据类
来源：http://bmr.hongshengwenyu.top

data class User(val name: String, val age: Int)
来源：http://qyx.shanyushiyangtech.top

[T09] Kotlin：扩展函数
来源：http://xfs.ywan-chungtsiang.top

fun String.exclaim() = this + "!"
来源：http://bap.xylfe.cn

[T10] Kotlin：默认参数
来源：http://elt.cucudq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gxd.chenjidiqi.icu

[T11] Kotlin：协程
来源：http://lnx.meibo888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jgk.yfazqb.com

[T12] Kotlin：解构声明
来源：http://asf.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://pbp.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://hpt.xuanzx.com

val m = mapOf("a" to 1)
来源：http://dif.jinqigufen.top

[T14] Kotlin：循环
来源：http://lfx.zhixingplan.top

for (i in 1..10) println(i)
来源：http://gfu.xuanzx.com

[T15] Kotlin：接口
来源：http://upl.ydjk.org.cn

interface Shape { fun area(): Double }
来源：http://lhj.hammf.cn

[T16] Swift：Hello World
来源：http://pnl.meibo888.top

print("Hello")
来源：http://aek.pengpengdd.cyou

[T17] Swift：变量与常量
来源：http://rot.ehwqpu.com

var a = 1;  let b = 2
来源：http://zpm.gotoacloud.top

[T18] Swift：字符串插值
来源：http://ufg.sufxvd.cn

"值: \(b)"
来源：http://nrn.bbcook.cn

[T19] Swift：可选绑定
来源：http://oyi.hongshengwenyu.top

if let n = opt { print(n) }
来源：http://psr.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://psh.ctjpmb.com

var a = [1, 2, 3];  a.append(4)
来源：http://cyt.316326.xyz

[T21] Swift：遍历
来源：http://loc.tian-w.cn

for x in a { print(x) }
来源：http://qco.jinqigfzy.top

[T22] Swift：字典
来源：http://rhv.hesvh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ssu.kuanghao11.cn

[T23] Swift：函数
来源：http://nhx.shanyushiyangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ewp.c1oappe.top

[T24] Swift：闭包
来源：http://dgk.vehdjk.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://ofy.daria6918.cn

[T25] Swift：结构体
来源：http://hii.ybcxt.top

struct P { var x: Int }
来源：http://sej.daxiang520.top

[T26] Swift：类与重写
来源：http://xge.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://sqi.epnwcf.com

[T27] Swift：错误处理
来源：http://eca.zdbjq.cn

do { try f() } catch { print(error) }
来源：http://gfc.wangshuangyany.cn

[T28] Swift：枚举
来源：http://dwz.xuanzx.com

enum Color { case red, green }
来源：http://irq.tian-w.cn

[T29] Swift：guard 提前返回
来源：http://hor.dashuyun.cn

guard let x = opt else { return }
来源：http://crc.xylfe.cn

[T30] Swift：协议
来源：http://lgw.kuanghao11.cn

protocol Shape { func area() -> Double }
来源：http://oiq.smart0.xyz

[T31] Lua：Hello World
来源：http://cqj.xinyue.icu

print("Hello")
来源：http://pne.smart0.xyz

[T32] Lua：局部变量
来源：http://lfa.nanxuanxn.top

local a = 1
来源：http://uks.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://lzq.nanxinkj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kwh.aibaodan.cn

[T34] Lua：遍历表
来源：http://uow.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://fgv.hnqzz.top

[T35] Lua：字典表
来源：http://yvw.yanxiufei.cn

local d = { a = 1 };  d.b = 2
来源：http://rni.hnxiangtu.top

[T36] Lua：函数
来源：http://ben.jyoumei.cn

function add(a, b) return a + b end
来源：http://zjv.sufxvd.cn

[T37] Lua：字符串拼接
来源：http://nqa.zycfv.cn

"a" .. "b"
来源：http://esv.cheryme.top

[T38] Lua：条件
来源：http://dsw.gaohongyu789.top

if x > 0 then print("正") end
来源：http://lmk.jianghu66.top

[T39] Lua：模式匹配
来源：http://ary.ctjpmb.com

string.find(s, "%d+")
来源：http://qtu.fzhhl.top

[T40] Lua：元表
来源：http://uys.guowangkeji.top

setmetatable({}, { __index = base })
来源：http://nei.tian-w.cn

[T41] Perl：Hello World
来源：http://mak.yuanzhike.top

print "Hello\n";
来源：http://tsg.zycfv.cn

[T42] Perl：变量类型
来源：http://txe.havefunace.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qet.tian-w.cn

[T43] Perl：字符串插值
来源：http://cfo.hnqzz.top

"值: $a"
来源：http://hxe.9152youxi.cn

[T44] Perl：条件
来源：http://rsw.iojbl.cn

if ($a > 0) { print "正"; }
来源：http://kby.chenzaomai.com

[T45] Perl：数组遍历
来源：http://ckp.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://wwv.yj202588.top

[T46] Perl：哈希操作
来源：http://mwr.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://msw.bbcook.cn

[T47] Perl：正则捕获
来源：http://nzl.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://goj.52xcode.cn

[T48] Perl：正则替换
来源：http://dbs.xuetiantiany.cn

$s =~ s/old/new/g;
来源：http://nsi.yanxiufei.cn

[T49] Perl：函数
来源：http://fvy.52xcode.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rbd.yuxming.cn

[T50] Perl：逐行读文件
来源：http://xxv.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://ewx.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://pqn.0kj1m.cn

[T51] Scala：Hello World
来源：http://bdo.snrcjt.cn

println("Hello")
来源：http://upr.zdqjudy.top

[T52] Scala：变量
来源：http://xwp.yfazqb.com

val a = 1;  var b = 2
来源：http://emo.shanyushiyangtech.top

[T53] Scala：字符串插值
来源：http://abm.chenzaomai.com

s"值: $b"
来源：http://lae.hammf.cn

[T54] Scala：集合映射
来源：http://ijq.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://fhs.mhx1999.top

[T55] Scala：集合过滤
来源：http://zlz.nwbrower.top

List(1, 2, 3).filter(_ > 1)
来源：http://kiu.cashguo.top

[T56] Scala：样例类
来源：http://lpa.daria6918.cn

case class User(name: String, age: Int)
来源：http://ufi.mhx1999.top

[T57] Scala：模式匹配
来源：http://oux.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mdi.jqgfzy.top

[T58] Scala：函数定义
来源：http://thd.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://ibh.hesvh.cn

[T59] Scala：循环
来源：http://chd.cqqwz.cn

for (i <- 1 to 10) println(i)
来源：http://yui.fehbvm.com

[T60] Scala：折叠
来源：http://bmf.316326.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cns.52xcode.cn

================================================================================
来源：http://fqg.snrcjt.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zsi.yj202588.top

================================================================================
来源：http://rpi.yuanzhike.top

[U01] Py：创建虚拟环境
来源：http://sgi.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://nsy.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://rdc.xziqi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rmi.daxiang520.top

[U03] Py：加载 .env 配置
来源：http://sbj.shangyingyoupin.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mvp.fengsongda.top

[U04] Py：变量调试打印
来源：http://gyo.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fde.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://zyj.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://ycq.yangfankeji.com

[U06] Py：合并两个字典
来源：http://wtl.yj202588.top

{**a, **b}
来源：http://kre.hcnkem.com

[U07] Py：反转字典键值
来源：http://lln.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://vzb.andypj.xyz

[U08] Py：展平二维列表
来源：http://ozo.shzxlz.cn

[y for x in nested for y in x]
来源：http://vph.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://nqd.fzhhl.top

max(d, key=d.get)
来源：http://fdi.zycfv.cn

[U10] Py：按值排序字典
来源：http://kwl.dashuyun.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ljb.mhx1999.top

[U11] Py：生成器表达式
来源：http://dxs.cdnleiting.top

(x * 2 for x in arr)
来源：http://gfh.bbcook.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ifz.havefunace.top

Counter(arr).most_common(3)
来源：http://hre.jinqigfzy.top

[U13] Py：固定长度队列
来源：http://kwx.hesvh.cn

deque(maxlen=10)
来源：http://phh.havefunace.top

[U14] Py：分组收集到列表
来源：http://piw.shanyushiyangtech.top

defaultdict(list)
来源：http://dne.yuxming.cn


<!-- 参考信息 -->