代发 wailian999

read -rp "请输入: " ans
来源：http://cil.bbcook.cn

[R78] 交互式菜单
来源：http://ueb.jiagoushi.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hvw.sufxvd.cn

[R79] 解析命令行选项
来源：http://gkx.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rhd.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://elk.cashguo.top

time ./run.sh
来源：http://nbb.shanyushiyangtech.top

================================================================================
来源：http://ofb.jinqigufen.top

S. C / C++ 专题
来源：http://gyn.0kj1m.cn

================================================================================
来源：http://xki.ppjwa.cn

[S01] C：Hello World
来源：http://zih.yvedp.cn

#include <stdio.h>
来源：http://qkg.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xik.jianghu66.top

[S02] C：变量与格式化输出
来源：http://klq.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://dry.jqgfzy.top

[S03] C：读入整数
来源：http://srv.0kj1m.cn

int x; scanf("%d", &x);
来源：http://dlc.zhengqikj.top

[S04] C：字符串复制
来源：http://lbk.sufxvd.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ggj.xziqi.cn

[S05] C：字符串长度
来源：http://shj.0kj1m.cn

strlen(s)
来源：http://vmn.xinyue.icu

[S06] C：字符串比较
来源：http://gkv.zhixingplan.top

strcmp(a, b) == 0
来源：http://cms.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://kda.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rlz.shanyushiyangkeji.top

[S08] C：动态内存分配与释放
来源：http://nnh.hnqzz.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vgr.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://gzh.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lvv.tianlin.xyz

[S10] C：指针与解引用
来源：http://zrt.tarul.cn

int *p = &a;  *p = 5;
来源：http://uqj.9152youxi.cn

[S11] C：逐行读文件
来源：http://mmk.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://qst.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://foj.shanyushiyangkeji.top

fclose(f);
来源：http://uvh.yueranfly.top

[S12] C：写文件
来源：http://ehe.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uya.jlsjyb.cn

[S13] C：宏定义
来源：http://jyv.yfazqb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mkg.jinqigufen.top

[S14] C：枚举
来源：http://yys.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://ccj.fzhhl.top

[S15] C：类型转换
来源：http://lsk.xylfe.cn

(double) a / b
来源：http://vqk.daxiang520.top

[S16] C：位操作置位
来源：http://acd.dianchejie.cn

x |= (1 << 3);
来源：http://xhk.tarul.cn

[S17] C：安全拼接字符串
来源：http://whu.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qgz.aibaodan.cn

[S18] C：命令行参数
来源：http://pvp.bbcook.cn

int main(int argc, char **argv)
来源：http://trn.zhiwuduotai.top

[S19] C：快速排序
来源：http://xfx.hywenlv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zuy.yuxming.cn

[S20] C：二分查找
来源：http://kjo.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vzt.sufxvd.cn

[S21] C：字符类别判断
来源：http://whp.cashguo.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jpt.guowangkeji.top

[S22] C：字符串转数字
来源：http://ejz.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pqg.jlsjyb.cn

[S23] C：随机数
来源：http://qzj.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nuh.gotoacloud.top

[S24] C：获取本地时间
来源：http://ldm.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ezv.gogol.net.cn

[S25] C：内存拷贝
来源：http://sdn.tarul.cn

memcpy(dst, src, n);
来源：http://cjv.shuidangran.top

[S26] C：内存清零
来源：http://lgd.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://mpe.guowangkeji.top

[S27] C：定义常量
来源：http://ynp.nwbrower.top

const double PI = 3.14159;
来源：http://iyj.kuanghao11.cn

[S28] C：静态变量
来源：http://evi.aizwys.cn

static int counter = 0;
来源：http://lae.tian-w.cn

[S29] C：变参函数
来源：http://xjs.chenlongwang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yye.ctjpmb.com

[S30] C：头文件保护
来源：http://jwd.tarul.cn

#ifndef X_H
来源：http://gzu.xylfe.cn

#define X_H
来源：http://xzp.xziqi.cn

#endif
来源：http://mbr.xylfe.cn

[S31] C++：Hello World
来源：http://pdi.yuxming.cn

#include <iostream>
来源：http://aaf.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://gls.vehdjk.com

[S32] C++：字符串
来源：http://pof.pycfn.com

std::string s = "hi";  s += "!";
来源：http://siw.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://fwl.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cik.hesvh.cn

[S34] C++：遍历 vector
来源：http://otp.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://ljy.nanxinkj.top

[S35] C++：map
来源：http://srs.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cxs.guowangkeji.top

[S36] C++：unordered_map
来源：http://xnj.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pxh.cheryme.top

[S37] C++：set
来源：http://pgf.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dfu.xinyue.icu

[S38] C++：排序
来源：http://ygw.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://uhm.hammf.cn

[S39] C++：自定义比较器排序
来源：http://vix.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://shg.dianchejie.cn

[S40] C++：查找元素
来源：http://gfj.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cqr.ydjk.org.cn

[S41] C++：类与构造函数
来源：http://ooy.sjlbkw.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ivx.daxiang520.top

[S42] C++：继承与虚函数
来源：http://hbg.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://xln.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://otm.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://bep.redwolf501.top

[S44] C++：引用传参
来源：http://iyt.zhengqikj.top

void inc(int &x) { ++x; }
来源：http://yax.zhixingplan.top

[S45] C++：lambda
来源：http://oas.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kkg.gaohongyu789.top

[S46] C++：函数模板
来源：http://ewm.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yda.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://hfg.epnwcf.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nza.guowangkeji.top

[S48] C++：逐行读文件
来源：http://nfr.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://kgd.cashguo.top

while (std::getline(in, line)) { }
来源：http://sxv.tian-w.cn

[S49] C++：写文件
来源：http://hvf.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iad.haohaochexian.top

[S50] C++：格式化数字
来源：http://ztf.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jdq.epnwcf.com

[S51] C++：显式类型转换
来源：http://tps.ctjpmb.com

static_cast<double>(a) / b
来源：http://gly.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://cya.hongshengwenyu.top

int size() const noexcept { return n_; }
来源：http://mvv.andypj.xyz

[S53] C++：移动语义
来源：http://ebm.zhijiandao.cn

std::vector<int> w = std::move(v);
来源：http://iqi.ppjwa.cn

[S54] C++：异常处理
来源：http://zfy.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fnd.nwbrower.top

[S55] C++：结构化绑定
来源：http://kre.shanyushiyangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wkv.hnxiangtu.top

[S56] C++：optional
来源：http://qcw.zhiwuduotai.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hgm.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://bgb.zhengqikj.top

constexpr int N = 10;
来源：http://pzy.yj20258888.top

[S58] C++：命名空间
来源：http://qxr.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://bgh.xylfe.cn

[S59] C++：静态断言
来源：http://umh.kuanghao11.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mhq.jyoumei.cn

[S60] C++：遍历并删除元素
来源：http://nip.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vev.xuetiantiany.cn

================================================================================
来源：http://mut.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ndg.yvedp.cn

================================================================================
来源：http://cwc.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://xce.jlsjyb.cn

println("Hello")
来源：http://rex.daria6918.cn

[T02] Kotlin：变量
来源：http://scf.meibo888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cvg.316326.xyz

[T03] Kotlin：字符串模板
来源：http://qow.zhiwuduotai.top

"值: $b"
来源：http://hcw.zhijiandao.cn

[T04] Kotlin：空安全
来源：http://uds.cheryme.top

val n: String? = null;  n?.length
来源：http://uxg.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://iad.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pja.redwolf501.top

[T06] Kotlin：集合映射
来源：http://mme.gaohongyu789.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kcy.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://tjv.tian-w.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ldh.nwbrower.top

[T08] Kotlin：数据类
来源：http://wkb.hysaishi.cn

data class User(val name: String, val age: Int)
来源：http://qic.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://zvy.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://hht.bjfxy.top

[T10] Kotlin：默认参数
来源：http://nai.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://chv.9152youxi.cn

[T11] Kotlin：协程
来源：http://ycj.redwolf501.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dty.sweek.top

[T12] Kotlin：解构声明
来源：http://qrv.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://kdu.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://epf.xuetiantiany.cn

val m = mapOf("a" to 1)
来源：http://pqu.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://vlf.nwbrower.top

for (i in 1..10) println(i)
来源：http://orm.havefunace.top

[T15] Kotlin：接口
来源：http://wzi.uphjek.com

interface Shape { fun area(): Double }
来源：http://ejd.andypj.xyz

[T16] Swift：Hello World
来源：http://enn.kuanghao11.cn

print("Hello")
来源：http://wvr.andypj.xyz

[T17] Swift：变量与常量
来源：http://rsb.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://cbw.xinyue.icu

[T18] Swift：字符串插值
来源：http://glr.yanxiufei.cn

"值: \(b)"
来源：http://rnn.shuidangran.top

[T19] Swift：可选绑定
来源：http://hka.haohaochexian.top

if let n = opt { print(n) }
来源：http://une.xuanzx.com

[T20] Swift：数组操作
来源：http://ohb.cqqwz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hxx.jinqigufen.top

[T21] Swift：遍历
来源：http://mqx.epnwcf.com

for x in a { print(x) }
来源：http://xqh.zhongyouzk.top

[T22] Swift：字典
来源：http://ijs.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oph.dianchejie.cn

[T23] Swift：函数
来源：http://cyc.nanxuanxn.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://roz.mhx1999.top

[T24] Swift：闭包
来源：http://moc.daxiang520.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vhb.gzhubu.top

[T25] Swift：结构体
来源：http://ujz.sufxvd.cn

struct P { var x: Int }
来源：http://col.hnxiangtu.top

[T26] Swift：类与重写
来源：http://rof.xziqi.cn

class A: Base { override func f() {} }
来源：http://shz.daria6918.cn

[T27] Swift：错误处理
来源：http://gpu.zhoulong.xyz

do { try f() } catch { print(error) }
来源：http://dgt.smart0.xyz

[T28] Swift：枚举
来源：http://vvr.jiagoushi.top

enum Color { case red, green }
来源：http://kpy.sysykeji.top

[T29] Swift：guard 提前返回
来源：http://vlx.jinqigfzy.top

guard let x = opt else { return }
来源：http://msk.52xcode.cn

[T30] Swift：协议
来源：http://yor.9152youxi.cn

protocol Shape { func area() -> Double }
来源：http://ims.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://mkt.snrcjt.cn

print("Hello")
来源：http://cup.hammf.cn

[T32] Lua：局部变量
来源：http://azr.wangshuangyany.cn

local a = 1
来源：http://dqq.9152youxi.cn

[T33] Lua：表（数组）
来源：http://ena.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jsd.yonumen.top

[T34] Lua：遍历表
来源：http://qfb.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vkh.vehdjk.com

[T35] Lua：字典表
来源：http://mhd.kuanghao11.cn

local d = { a = 1 };  d.b = 2
来源：http://huj.cashguo.top

[T36] Lua：函数
来源：http://rdb.redwolf501.top

function add(a, b) return a + b end
来源：http://dpl.feifeiyinyue.top

[T37] Lua：字符串拼接
来源：http://tns.yonumen.top

"a" .. "b"
来源：http://ocf.vehdjk.com

[T38] Lua：条件
来源：http://sdu.nanxinkj.top

if x > 0 then print("正") end
来源：http://fig.meibo888.top

[T39] Lua：模式匹配
来源：http://rkx.0kj1m.cn

string.find(s, "%d+")
来源：http://kln.fengsongda.top

[T40] Lua：元表
来源：http://xrk.mhx1999.top

setmetatable({}, { __index = base })
来源：http://clc.hcnkem.com

[T41] Perl：Hello World
来源：http://yec.smart0.xyz

print "Hello\n";
来源：http://xlt.sufxvd.cn

[T42] Perl：变量类型
来源：http://akr.shanyushiyangtech.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wvv.yuanzhike.top

[T43] Perl：字符串插值
来源：http://hps.yongpay.top

"值: $a"
来源：http://jnv.jyoumei.cn

[T44] Perl：条件
来源：http://rjk.xuetiantiany.cn

if ($a > 0) { print "正"; }
来源：http://kyh.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://wcr.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://xsz.hcnkem.com

[T46] Perl：哈希操作
来源：http://hgi.birdmap.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lrc.cheryme.top

[T47] Perl：正则捕获
来源：http://ktk.fktsv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mdv.jqgufenzy.top

[T48] Perl：正则替换
来源：http://cmh.ywan-chungtsiang.top

$s =~ s/old/new/g;
来源：http://nvg.zhijiandao.cn

[T49] Perl：函数
来源：http://nwt.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cwp.0kj1m.cn

[T50] Perl：逐行读文件
来源：http://rhu.hnqzz.top

open my $fh, "<", "a.txt" or die $!;
来源：http://iks.sufxvd.cn

while (my $line = <$fh>) { print $line; }
来源：http://vgf.kuanghao11.cn

[T51] Scala：Hello World
来源：http://jba.shanyushiyangkeji.top

println("Hello")
来源：http://mzz.yvedp.cn

[T52] Scala：变量
来源：http://wls.shangyingyoupin.top

val a = 1;  var b = 2
来源：http://ojt.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://bwc.sxryk.cn

s"值: $b"
来源：http://jee.ehwqpu.com

[T54] Scala：集合映射
来源：http://gsa.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://ibn.aizwys.cn

[T55] Scala：集合过滤
来源：http://noz.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://ocd.yj202588.top

[T56] Scala：样例类
来源：http://yqt.ybcxt.top

case class User(name: String, age: Int)
来源：http://yym.xuetiantiany.cn

[T57] Scala：模式匹配
来源：http://auf.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bgu.chenzaomai.com

[T58] Scala：函数定义
来源：http://oat.nanxuanxn.top

def add(a: Int, b: Int): Int = a + b
来源：http://ore.ctjpmb.com

[T59] Scala：循环
来源：http://bfd.hnqzz.top

for (i <- 1 to 10) println(i)
来源：http://hjs.snrcjt.cn

[T60] Scala：折叠
来源：http://zuo.hywenlv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gzl.tianlin.xyz

================================================================================
来源：http://jdt.pengpengdd.cyou

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vlz.smart0.xyz

================================================================================
来源：http://aer.52xcode.cn

[U01] Py：创建虚拟环境
来源：http://nps.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jou.chenlongwang.top

[U02] Py：导出 / 安装依赖
来源：http://gbr.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://all.xziqi.cn

[U03] Py：加载 .env 配置
来源：http://lio.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bwa.ctjpmb.com

[U04] Py：变量调试打印
来源：http://vfv.pengpengdd.cyou

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jrk.birdmap.top

[U05] Py：列表去重且保序
来源：http://agf.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://jrg.zhijiandao.cn

[U06] Py：合并两个字典
来源：http://zvq.0kj1m.cn

{**a, **b}
来源：http://yhm.0kj1m.cn

[U07] Py：反转字典键值
来源：http://ypx.hnqzz.top

{v: k for k, v in d.items()}
来源：http://aqi.chenlongwang.top

[U08] Py：展平二维列表
来源：http://ovi.hnqzz.top

[y for x in nested for y in x]
来源：http://osi.dianchejie.cn

[U09] Py：字典取最大值的键
来源：http://anf.cheryme.top

max(d, key=d.get)
来源：http://mvg.shanyushiyangtech.top

[U10] Py：按值排序字典
来源：http://mah.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eul.zhengqikj.top

[U11] Py：生成器表达式
来源：http://jtr.meibo888.top

(x * 2 for x in arr)
来源：http://vrl.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://gqc.jinqigufen.top

Counter(arr).most_common(3)
来源：http://mfa.shangyingyoupin.top

[U13] Py：固定长度队列
来源：http://rgd.guowangkeji.top

deque(maxlen=10)
来源：http://mvr.sxryk.cn

[U14] Py：分组收集到列表
来源：http://snq.shanyushiyangkeji.top

defaultdict(list)
来源：http://dno.hysaishi.cn

[U15] Py：高精度计时
来源：http://eoj.guannengcc.top

t = time.perf_counter()
来源：http://lzl.vqdsnc.cn

[U16] Py：命令行参数解析
来源：http://sns.bbcook.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dfv.hesvh.cn

[U17] Py：初始化日志
来源：http://haz.shanyushiyangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://gan.cucudq.cn

[U18] Py：预编译正则
来源：http://agd.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://lop.nanxuanxn.top


<!-- 参考信息 -->