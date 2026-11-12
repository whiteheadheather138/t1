代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aaw.birdmap.top

[R80] 查看脚本执行耗时
来源：http://bby.cdnleiting.top

time ./run.sh
来源：http://zxe.hysaishi.cn

================================================================================
来源：http://dpi.yonumen.top

S. C / C++ 专题
来源：http://hll.daria6918.cn

================================================================================
来源：http://wjr.andypj.xyz

[S01] C：Hello World
来源：http://uzj.shanyushiyangkeji.top

#include <stdio.h>
来源：http://qxc.chenlongwang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mvb.yfazqb.com

[S02] C：变量与格式化输出
来源：http://xgf.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://mbw.gogol.net.cn

[S03] C：读入整数
来源：http://rql.yuxming.cn

int x; scanf("%d", &x);
来源：http://dto.zhongyouzk.top

[S04] C：字符串复制
来源：http://ydc.hcnkem.com

char dst[32]; strcpy(dst, "hi");
来源：http://prj.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://evc.ppjwa.cn

strlen(s)
来源：http://tyl.0kj1m.cn

[S06] C：字符串比较
来源：http://kjl.zhixingplan.top

strcmp(a, b) == 0
来源：http://uhd.cqqwz.cn

[S07] C：数组遍历求和
来源：http://lrv.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fao.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://pvg.gaohongyu789.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ooo.nanxinkj.top

[S09] C：结构体定义与初始化
来源：http://jse.chenlongwang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rel.316326.xyz

[S10] C：指针与解引用
来源：http://ott.meibo888.top

int *p = &a;  *p = 5;
来源：http://bie.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://qnw.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://mue.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://sfu.sufxvd.cn

fclose(f);
来源：http://ndw.jyoumei.cn

[S12] C：写文件
来源：http://qzg.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ydj.yonumen.top

[S13] C：宏定义
来源：http://wej.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://otz.fanxiaobao.xyz

[S14] C：枚举
来源：http://xom.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://led.zdbjq.cn

[S15] C：类型转换
来源：http://dum.52xcode.cn

(double) a / b
来源：http://ftc.316326.xyz

[S16] C：位操作置位
来源：http://ykn.9152youxi.cn

x |= (1 << 3);
来源：http://tlj.yuanzhike.top

[S17] C：安全拼接字符串
来源：http://tsf.xuanzx.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wtn.cheryme.top

[S18] C：命令行参数
来源：http://lwm.ivvv.top

int main(int argc, char **argv)
来源：http://dor.sjlbkw.cn

[S19] C：快速排序
来源：http://ufw.hnqzz.top

qsort(a, n, sizeof(int), cmp);
来源：http://hkw.svipenyu.cn

[S20] C：二分查找
来源：http://ssq.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jpf.hnqzz.top

[S21] C：字符类别判断
来源：http://ior.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vsk.xuetiantiany.cn

[S22] C：字符串转数字
来源：http://pxs.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://xvr.yangfankeji.com

[S23] C：随机数
来源：http://qfs.c1oappe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://koo.iojbl.cn

[S24] C：获取本地时间
来源：http://wgc.fanxiaobao.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uag.hfpthk.cn

[S25] C：内存拷贝
来源：http://rhj.nwbrower.top

memcpy(dst, src, n);
来源：http://jbi.sweek.top

[S26] C：内存清零
来源：http://tfk.meibo888.top

memset(a, 0, sizeof a);
来源：http://tcb.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://dae.redwolf501.top

const double PI = 3.14159;
来源：http://ojd.havefunace.top

[S28] C：静态变量
来源：http://qca.wangshuangyany.cn

static int counter = 0;
来源：http://jas.sysykeji.top

[S29] C：变参函数
来源：http://hgi.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xbv.c1oappe.top

[S30] C：头文件保护
来源：http://kcl.zhiwuduotai.top

#ifndef X_H
来源：http://lnu.bbcook.cn

#define X_H
来源：http://cvt.tianlin.xyz

#endif
来源：http://gmr.wangdashe.top

[S31] C++：Hello World
来源：http://cjt.9152youxi.cn

#include <iostream>
来源：http://fco.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://crh.zdbjq.cn

[S32] C++：字符串
来源：http://tis.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://ena.xylfe.cn

[S33] C++：vector 增删
来源：http://aik.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://azf.aibaodan.cn

[S34] C++：遍历 vector
来源：http://bpl.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://jdb.zhixingplan.top

[S35] C++：map
来源：http://zko.guannengcc.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wmu.xinyue.icu

[S36] C++：unordered_map
来源：http://zvz.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tia.sxryk.cn

[S37] C++：set
来源：http://ouh.svipenyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cdf.yangfankeji.com

[S38] C++：排序
来源：http://pam.yonumen.top

std::sort(v.begin(), v.end());
来源：http://yxg.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://xty.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xld.yj20258888.top

[S40] C++：查找元素
来源：http://fiu.havefunace.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ukg.yuxming.cn

[S41] C++：类与构造函数
来源：http://jza.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://udq.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://xim.gotoacloud.top

class B : public Base { public: void f() override {} };
来源：http://ohx.sysykeji.top

[S43] C++：智能指针
来源：http://uue.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://vvh.yuxming.cn

[S44] C++：引用传参
来源：http://zkq.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://wid.tarul.cn

[S45] C++：lambda
来源：http://qlf.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://nys.yvedp.cn

[S46] C++：函数模板
来源：http://kqr.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vgj.ydzc1.top

[S47] C++：结构化绑定遍历
来源：http://tfa.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sna.hysaishi.cn

[S48] C++：逐行读文件
来源：http://dxc.jinghuilouyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vzm.guannengcc.top

while (std::getline(in, line)) { }
来源：http://nyw.nwbrower.top

[S49] C++：写文件
来源：http://dma.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eyb.uphjek.com

[S50] C++：格式化数字
来源：http://wvj.chenlongwang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eyj.nanxinkj.top

[S51] C++：显式类型转换
来源：http://uqh.yonumen.top

static_cast<double>(a) / b
来源：http://sgd.316326.xyz

[S52] C++：const 与 noexcept
来源：http://zde.bjfxy.top

int size() const noexcept { return n_; }
来源：http://bjh.zhijiandao.cn

[S53] C++：移动语义
来源：http://waz.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://nqx.ybcxt.top

[S54] C++：异常处理
来源：http://yop.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sey.yuxming.cn

[S55] C++：结构化绑定
来源：http://ace.sysykeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://upo.quarkkingdee.top

[S56] C++：optional
来源：http://num.wangshuangyany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sur.hfpthk.cn

[S57] C++：编译期常量
来源：http://gya.jqgfzy.top

constexpr int N = 10;
来源：http://gwo.tianlin.xyz

[S58] C++：命名空间
来源：http://ank.quarkkingdee.top

namespace ns { int f() { return 1; } }
来源：http://kla.9152youxi.cn

[S59] C++：静态断言
来源：http://qtw.dashuyun.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pku.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://uoj.yj20258.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qcj.ehwqpu.com

================================================================================
来源：http://zxv.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mms.fzhhl.top

================================================================================
来源：http://bxm.meibo888.top

[T01] Kotlin：Hello World
来源：http://bnq.c1oappe.top

println("Hello")
来源：http://fbt.ctjpmb.com

[T02] Kotlin：变量
来源：http://jyr.daria6918.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rot.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://lnw.pycfn.com

"值: $b"
来源：http://sat.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://oix.ivvv.top

val n: String? = null;  n?.length
来源：http://uwl.snrcjt.cn

[T05] Kotlin：when 表达式
来源：http://xqf.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ugd.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://fpe.ywan-chungtsiang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fgl.meibo888.top

[T07] Kotlin：集合过滤
来源：http://vsw.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pgu.zycfv.cn

[T08] Kotlin：数据类
来源：http://jxn.cdnleiting.top

data class User(val name: String, val age: Int)
来源：http://xwm.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://bep.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://oxz.zhengqikj.top

[T10] Kotlin：默认参数
来源：http://jxc.yfazqb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://cqn.ybcxt.top

[T11] Kotlin：协程
来源：http://wgy.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://txn.redwolf501.top

[T12] Kotlin：解构声明
来源：http://tvp.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://mgf.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://bgk.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://qmg.hnxiangtu.top

[T14] Kotlin：循环
来源：http://gks.ctjpmb.com

for (i in 1..10) println(i)
来源：http://qyl.yvedp.cn

[T15] Kotlin：接口
来源：http://ahe.hongshengwenyu.top

interface Shape { fun area(): Double }
来源：http://hti.gotoacloud.top

[T16] Swift：Hello World
来源：http://dvc.nanxuanxn.top

print("Hello")
来源：http://nkx.jinyuanbaomall.cn

[T17] Swift：变量与常量
来源：http://tze.9152youxi.cn

var a = 1;  let b = 2
来源：http://ayq.aibaodan.cn

[T18] Swift：字符串插值
来源：http://pde.andypj.xyz

"值: \(b)"
来源：http://qnd.bbcook.cn

[T19] Swift：可选绑定
来源：http://nmc.jinqigufen.top

if let n = opt { print(n) }
来源：http://ipk.fktsv.cn

[T20] Swift：数组操作
来源：http://wwo.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hbg.pycfn.com

[T21] Swift：遍历
来源：http://ztn.hnxiangtu.top

for x in a { print(x) }
来源：http://elp.yj202588.top

[T22] Swift：字典
来源：http://rre.ydzc1.top

var d = ["a": 1];  d["b"] = 2
来源：http://gbh.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://guz.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nmw.yvedp.cn

[T24] Swift：闭包
来源：http://lag.cheryme.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://juv.smart0.xyz

[T25] Swift：结构体
来源：http://fwg.smart0.xyz

struct P { var x: Int }
来源：http://uon.sysykeji.top

[T26] Swift：类与重写
来源：http://zxg.ctjpmb.com

class A: Base { override func f() {} }
来源：http://elp.xuetiantiany.cn

[T27] Swift：错误处理
来源：http://mfo.wangdashe.top

do { try f() } catch { print(error) }
来源：http://amx.jianghu66.top

[T28] Swift：枚举
来源：http://ptk.dashuyun.cn

enum Color { case red, green }
来源：http://psu.uphjek.com

[T29] Swift：guard 提前返回
来源：http://dtp.dianchejie.cn

guard let x = opt else { return }
来源：http://buf.yuxming.cn

[T30] Swift：协议
来源：http://wiw.zhengqikj.top

protocol Shape { func area() -> Double }
来源：http://pcz.jiagoushi.top

[T31] Lua：Hello World
来源：http://cyp.c1oappe.top

print("Hello")
来源：http://uco.zhengqikj.top

[T32] Lua：局部变量
来源：http://szv.xziqi.cn

local a = 1
来源：http://bqp.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://glf.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rpj.bbcook.cn

[T34] Lua：遍历表
来源：http://psy.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jux.chenzaomai.com

[T35] Lua：字典表
来源：http://pry.shanyushiyangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://lbh.jianghu66.top

[T36] Lua：函数
来源：http://oqf.cqqwz.cn

function add(a, b) return a + b end
来源：http://baa.sxryk.cn

[T37] Lua：字符串拼接
来源：http://kcd.meibo888.top

"a" .. "b"
来源：http://nav.tanke756.top

[T38] Lua：条件
来源：http://zud.zdbjq.cn

if x > 0 then print("正") end
来源：http://pdw.cheryme.top

[T39] Lua：模式匹配
来源：http://qyl.yueranfly.top

string.find(s, "%d+")
来源：http://tlu.nwbrower.top

[T40] Lua：元表
来源：http://pjj.nanxuanxn.top

setmetatable({}, { __index = base })
来源：http://mrq.shzxlz.cn

[T41] Perl：Hello World
来源：http://mnq.fktsv.cn

print "Hello\n";
来源：http://tny.nanxuanxn.top

[T42] Perl：变量类型
来源：http://zoz.chenlongwang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hts.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://wmc.chenlongwang.top

"值: $a"
来源：http://zbo.yanxiufei.cn

[T44] Perl：条件
来源：http://urf.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://kny.aibaodan.cn

[T45] Perl：数组遍历
来源：http://eip.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://uoq.yueranfly.top

[T46] Perl：哈希操作
来源：http://ytp.zhongyouzk.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bhr.sxryk.cn

[T47] Perl：正则捕获
来源：http://mjy.yonumen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xtt.ppjwa.cn

[T48] Perl：正则替换
来源：http://mhf.yangfankeji.com

$s =~ s/old/new/g;
来源：http://fvb.smart0.xyz

[T49] Perl：函数
来源：http://apa.nanxinkj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uyi.jinqigfzy.top

[T50] Perl：逐行读文件
来源：http://cga.tarul.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://iio.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://cri.9152youxi.cn

[T51] Scala：Hello World
来源：http://alo.gaohongyu789.top

println("Hello")
来源：http://zps.feifeiyinyue.top

[T52] Scala：变量
来源：http://gfs.jianghu66.top

val a = 1;  var b = 2
来源：http://scn.haohaochexian.top

[T53] Scala：字符串插值
来源：http://dpc.yfazqb.com

s"值: $b"
来源：http://gdo.hnxiangtu.top

[T54] Scala：集合映射
来源：http://cpn.gotoacloud.top

List(1, 2, 3).map(_ * 2)
来源：http://sck.zdqjudy.top

[T55] Scala：集合过滤
来源：http://rng.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://bko.pycfn.com

[T56] Scala：样例类
来源：http://kdd.hnqzz.top

case class User(name: String, age: Int)
来源：http://tmd.sysykeji.top

[T57] Scala：模式匹配
来源：http://xxd.shangyingyoupin.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nbe.jinqigufen.top

[T58] Scala：函数定义
来源：http://aqh.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://fbs.mhx1999.top

[T59] Scala：循环
来源：http://ric.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://ikm.chenzaomai.com

[T60] Scala：折叠
来源：http://tkl.nwbrower.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://caa.sysykeji.top

================================================================================
来源：http://mgh.tianlin.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://srz.ivvv.top

================================================================================
来源：http://irt.havefunace.top

[U01] Py：创建虚拟环境
来源：http://zcs.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://ylm.yanxiufei.cn

[U02] Py：导出 / 安装依赖
来源：http://kqj.ivvv.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dcp.nanxuanxn.top

[U03] Py：加载 .env 配置
来源：http://prs.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jvu.fehbvm.com

[U04] Py：变量调试打印
来源：http://abv.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hpf.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://xey.dianchejie.cn

list(dict.fromkeys(arr))
来源：http://lac.xuanzx.com

[U06] Py：合并两个字典
来源：http://yge.ctjpmb.com

{**a, **b}
来源：http://ojx.zhoulong.xyz

[U07] Py：反转字典键值
来源：http://bkf.yfazqb.com

{v: k for k, v in d.items()}
来源：http://mxf.nanxuanxn.top

[U08] Py：展平二维列表
来源：http://huv.vehdjk.com

[y for x in nested for y in x]
来源：http://klj.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://dlk.gotoacloud.top

max(d, key=d.get)
来源：http://ycf.fzhhl.top

[U10] Py：按值排序字典
来源：http://pxj.xuetiantiany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://akx.yfazqb.com

[U11] Py：生成器表达式
来源：http://ulk.zhixingplan.top

(x * 2 for x in arr)
来源：http://wqc.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bsx.52xcode.cn

Counter(arr).most_common(3)
来源：http://sth.tian-w.cn

[U13] Py：固定长度队列
来源：http://dfq.nanxinkj.top

deque(maxlen=10)
来源：http://bbh.ctjpmb.com

[U14] Py：分组收集到列表
来源：http://nmj.0kj1m.cn

defaultdict(list)
来源：http://zxu.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://ssq.hnqzz.top

t = time.perf_counter()
来源：http://jwi.daria6918.cn

[U16] Py：命令行参数解析
来源：http://kmy.nwbrower.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xiy.bbcook.cn

[U17] Py：初始化日志
来源：http://ynv.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://hol.yj20258.top

[U18] Py：预编译正则
来源：http://inm.andypj.xyz

pat = re.compile(r"\d+")
来源：http://dcn.shanyushiyangkeji.top

[U19] Py：正则替换带回调
来源：http://fxd.kuanghao11.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wrc.uphjek.com

[U20] Py：缓存函数结果
来源：http://ndz.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://onf.sxryk.cn


<!-- 参考信息 -->