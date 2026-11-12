代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wsm.smart0.xyz

[R80] 查看脚本执行耗时
来源：http://lke.shuidangran.top

time ./run.sh
来源：http://awp.cashguo.top

================================================================================
来源：http://qcb.pycfn.com

S. C / C++ 专题
来源：http://poa.guowangkeji.top

================================================================================
来源：http://rvq.ivvv.top

[S01] C：Hello World
来源：http://hbm.quarkkingdee.top

#include <stdio.h>
来源：http://txx.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://btk.ehwqpu.com

[S02] C：变量与格式化输出
来源：http://wfs.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://kpr.cucudq.cn

[S03] C：读入整数
来源：http://bvj.tarul.cn

int x; scanf("%d", &x);
来源：http://uuq.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://era.hywenlv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vlj.yanxiufei.cn

[S05] C：字符串长度
来源：http://voy.gzhubu.top

strlen(s)
来源：http://qrv.feifeiyinyue.top

[S06] C：字符串比较
来源：http://klg.zhengqikj.top

strcmp(a, b) == 0
来源：http://fgh.smart0.xyz

[S07] C：数组遍历求和
来源：http://fzy.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kbq.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://edw.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://edy.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://muo.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oge.wangdashe.top

[S10] C：指针与解引用
来源：http://dau.wangdashe.top

int *p = &a;  *p = 5;
来源：http://ncu.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://rfg.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://odj.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://uul.dianchejie.cn

fclose(f);
来源：http://bmg.vehdjk.com

[S12] C：写文件
来源：http://cmh.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://esu.c1oappe.top

[S13] C：宏定义
来源：http://yan.birdmap.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mwd.svipenyu.cn

[S14] C：枚举
来源：http://cyp.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://wrz.hnqzz.top

[S15] C：类型转换
来源：http://oik.chenjidiqi.icu

(double) a / b
来源：http://sit.pengpengdd.cyou

[S16] C：位操作置位
来源：http://ghk.pengpengdd.cyou

x |= (1 << 3);
来源：http://qib.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://vnk.redwolf501.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qsa.cqqwz.cn

[S18] C：命令行参数
来源：http://aem.haohaochexian.top

int main(int argc, char **argv)
来源：http://jic.fzhhl.top

[S19] C：快速排序
来源：http://xzd.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://sms.hcnkem.com

[S20] C：二分查找
来源：http://ryc.316326.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qik.shzxlz.cn

[S21] C：字符类别判断
来源：http://ekv.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iyu.jlsjyb.cn

[S22] C：字符串转数字
来源：http://clt.c1oappe.top

atoi("42");  strtod("3.14", NULL);
来源：http://lof.andypj.xyz

[S23] C：随机数
来源：http://lzq.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://imz.sweek.top

[S24] C：获取本地时间
来源：http://fkd.xuanzx.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nhx.ybcxt.top

[S25] C：内存拷贝
来源：http://waq.smart0.xyz

memcpy(dst, src, n);
来源：http://wxe.iojbl.cn

[S26] C：内存清零
来源：http://mmr.yvedp.cn

memset(a, 0, sizeof a);
来源：http://jap.epnwcf.com

[S27] C：定义常量
来源：http://fha.guannengcc.top

const double PI = 3.14159;
来源：http://zrj.feifeiyinyue.top

[S28] C：静态变量
来源：http://pmp.xingfuxueyuan.xyz

static int counter = 0;
来源：http://bie.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://iji.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fam.xylfe.cn

[S30] C：头文件保护
来源：http://zyj.sweek.top

#ifndef X_H
来源：http://mru.ehwqpu.com

#define X_H
来源：http://zdd.shzxlz.cn

#endif
来源：http://zyn.gogol.net.cn

[S31] C++：Hello World
来源：http://qum.chenjidiqi.icu

#include <iostream>
来源：http://kbn.snrcjt.cn

int main() { std::cout << "Hello\n"; }
来源：http://iho.gogol.net.cn

[S32] C++：字符串
来源：http://phy.daxiang520.top

std::string s = "hi";  s += "!";
来源：http://ofm.xylfe.cn

[S33] C++：vector 增删
来源：http://uqa.yvedp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://loh.gaohongyu789.top

[S34] C++：遍历 vector
来源：http://ksi.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://cbw.gogol.net.cn

[S35] C++：map
来源：http://cnd.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pfe.andypj.xyz

[S36] C++：unordered_map
来源：http://pie.xylfe.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://idr.meibo888.top

[S37] C++：set
来源：http://fll.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lct.yongpay.top

[S38] C++：排序
来源：http://hlq.xinyue.icu

std::sort(v.begin(), v.end());
来源：http://pew.hysaishi.cn

[S39] C++：自定义比较器排序
来源：http://wpw.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pcs.daxiang520.top

[S40] C++：查找元素
来源：http://xas.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mxc.dianchejie.cn

[S41] C++：类与构造函数
来源：http://jgn.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://azt.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://wbw.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://vzb.fehbvm.com

[S43] C++：智能指针
来源：http://xje.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://gun.yj20258888.top

[S44] C++：引用传参
来源：http://lbj.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://zdc.cqqwz.cn

[S45] C++：lambda
来源：http://qqh.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iad.zhiwuduotai.top

[S46] C++：函数模板
来源：http://npz.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xmm.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://yki.zhixingplan.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qoo.ydzc1.top

[S48] C++：逐行读文件
来源：http://kri.xingfuxueyuan.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://hhi.meibo888.top

while (std::getline(in, line)) { }
来源：http://dko.zhixingplan.top

[S49] C++：写文件
来源：http://twg.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dcy.hesvh.cn

[S50] C++：格式化数字
来源：http://bse.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cjd.chenzaomai.com

[S51] C++：显式类型转换
来源：http://syo.shuidangran.top

static_cast<double>(a) / b
来源：http://atf.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://suh.316326.xyz

int size() const noexcept { return n_; }
来源：http://vlr.yuxming.cn

[S53] C++：移动语义
来源：http://qyv.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://cgw.fengsongda.top

[S54] C++：异常处理
来源：http://tuc.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kvp.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://fnd.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://brw.xziqi.cn

[S56] C++：optional
来源：http://cyg.fehbvm.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pkg.xinyue.icu

[S57] C++：编译期常量
来源：http://dgb.svipenyu.cn

constexpr int N = 10;
来源：http://wig.havefunace.top

[S58] C++：命名空间
来源：http://sje.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://vbc.zhiwuduotai.top

[S59] C++：静态断言
来源：http://vly.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gbn.quarkkingdee.top

[S60] C++：遍历并删除元素
来源：http://atk.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ahl.hammf.cn

================================================================================
来源：http://frs.xinyue.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rrx.fktsv.cn

================================================================================
来源：http://gay.cashguo.top

[T01] Kotlin：Hello World
来源：http://wym.zhoulong.xyz

println("Hello")
来源：http://kfk.gaohongyu789.top

[T02] Kotlin：变量
来源：http://qvi.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fvv.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://izs.meibo888.top

"值: $b"
来源：http://kqh.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://caw.mhx1999.top

val n: String? = null;  n?.length
来源：http://yzl.316326.xyz

[T05] Kotlin：when 表达式
来源：http://xcy.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rob.316326.xyz

[T06] Kotlin：集合映射
来源：http://jtu.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://dpu.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://tzm.ivvv.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uzr.shangyingyoupin.top

[T08] Kotlin：数据类
来源：http://djy.c1oappe.top

data class User(val name: String, val age: Int)
来源：http://yhx.fengsongda.top

[T09] Kotlin：扩展函数
来源：http://dtm.hnqzz.top

fun String.exclaim() = this + "!"
来源：http://bne.iojbl.cn

[T10] Kotlin：默认参数
来源：http://amq.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bnp.c1oappe.top

[T11] Kotlin：协程
来源：http://kvt.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tic.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://fwz.jlsjyb.cn

val (a, b) = Pair(1, 2)
来源：http://gta.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://cbz.epnwcf.com

val m = mapOf("a" to 1)
来源：http://lkb.yj20258.top

[T14] Kotlin：循环
来源：http://jww.xuanzx.com

for (i in 1..10) println(i)
来源：http://ejq.kuanghao11.cn

[T15] Kotlin：接口
来源：http://uoz.yvedp.cn

interface Shape { fun area(): Double }
来源：http://yuv.cashguo.top

[T16] Swift：Hello World
来源：http://wlr.zhijiandao.cn

print("Hello")
来源：http://sqb.tarul.cn

[T17] Swift：变量与常量
来源：http://wrv.jyoumei.cn

var a = 1;  let b = 2
来源：http://wxd.52xcode.cn

[T18] Swift：字符串插值
来源：http://vpt.shanyushiyangtech.top

"值: \(b)"
来源：http://cdv.hysaishi.cn

[T19] Swift：可选绑定
来源：http://chf.redwolf501.top

if let n = opt { print(n) }
来源：http://ssh.iojbl.cn

[T20] Swift：数组操作
来源：http://ank.yueranfly.top

var a = [1, 2, 3];  a.append(4)
来源：http://iyy.chenzaomai.com

[T21] Swift：遍历
来源：http://rkm.9152youxi.cn

for x in a { print(x) }
来源：http://jhl.nanxinkj.top

[T22] Swift：字典
来源：http://ows.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lbp.52xcode.cn

[T23] Swift：函数
来源：http://tgv.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://evt.yuxming.cn

[T24] Swift：闭包
来源：http://qod.sxryk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dqc.hnxiangtu.top

[T25] Swift：结构体
来源：http://aie.52xcode.cn

struct P { var x: Int }
来源：http://qqx.yj20258.top

[T26] Swift：类与重写
来源：http://cqo.yonumen.top

class A: Base { override func f() {} }
来源：http://fbw.jinqigufen.top

[T27] Swift：错误处理
来源：http://eez.hfpthk.cn

do { try f() } catch { print(error) }
来源：http://ssw.0kj1m.cn

[T28] Swift：枚举
来源：http://jnu.9152youxi.cn

enum Color { case red, green }
来源：http://bbm.smart0.xyz

[T29] Swift：guard 提前返回
来源：http://ypx.birdmap.top

guard let x = opt else { return }
来源：http://jiu.ydzc1.top

[T30] Swift：协议
来源：http://sth.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://jxr.guowangkeji.top

[T31] Lua：Hello World
来源：http://rzg.chenzaomai.com

print("Hello")
来源：http://gtn.zycfv.cn

[T32] Lua：局部变量
来源：http://wll.iojbl.cn

local a = 1
来源：http://kfl.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://ddi.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jzj.yj202588.top

[T34] Lua：遍历表
来源：http://pip.cucudq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xej.cdnleiting.top

[T35] Lua：字典表
来源：http://sdp.zdqjudy.top

local d = { a = 1 };  d.b = 2
来源：http://kyp.xinyue.icu

[T36] Lua：函数
来源：http://hjw.redwolf501.top

function add(a, b) return a + b end
来源：http://ncy.daxiang520.top

[T37] Lua：字符串拼接
来源：http://eym.ybcxt.top

"a" .. "b"
来源：http://ljv.hfpthk.cn

[T38] Lua：条件
来源：http://shd.daxiang520.top

if x > 0 then print("正") end
来源：http://wav.andypj.xyz

[T39] Lua：模式匹配
来源：http://quh.haohaochexian.top

string.find(s, "%d+")
来源：http://zyz.bbcook.cn

[T40] Lua：元表
来源：http://jzg.zycfv.cn

setmetatable({}, { __index = base })
来源：http://scw.aizwys.cn

[T41] Perl：Hello World
来源：http://arl.vehdjk.com

print "Hello\n";
来源：http://lxt.0kj1m.cn

[T42] Perl：变量类型
来源：http://srt.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wqx.hnqzz.top

[T43] Perl：字符串插值
来源：http://wgw.yongpay.top

"值: $a"
来源：http://izv.yvedp.cn

[T44] Perl：条件
来源：http://yry.zhijiandao.cn

if ($a > 0) { print "正"; }
来源：http://iju.fengsongda.top

[T45] Perl：数组遍历
来源：http://ype.zhaomingkeji.xyz

for my $x (@arr) { print $x; }
来源：http://epg.hysaishi.cn

[T46] Perl：哈希操作
来源：http://hwu.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pqz.epnwcf.com

[T47] Perl：正则捕获
来源：http://rdd.yonumen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qlh.smart0.xyz

[T48] Perl：正则替换
来源：http://ezq.mhx1999.top

$s =~ s/old/new/g;
来源：http://exa.cqqwz.cn

[T49] Perl：函数
来源：http://lhp.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pgq.jlsjyb.cn

[T50] Perl：逐行读文件
来源：http://tqv.shanyushiyangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gsm.sufxvd.cn

while (my $line = <$fh>) { print $line; }
来源：http://ahz.guannengcc.top

[T51] Scala：Hello World
来源：http://jrf.aizwys.cn

println("Hello")
来源：http://rtp.yueranfly.top

[T52] Scala：变量
来源：http://gjb.sweek.top

val a = 1;  var b = 2
来源：http://fwm.havefunace.top

[T53] Scala：字符串插值
来源：http://xla.meibo888.top

s"值: $b"
来源：http://mvy.kuanghao11.cn

[T54] Scala：集合映射
来源：http://crq.hywenlv.cn

List(1, 2, 3).map(_ * 2)
来源：http://zmt.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://vhr.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://lbi.nwbrower.top

[T56] Scala：样例类
来源：http://eob.zycfv.cn

case class User(name: String, age: Int)
来源：http://zxb.nwbrower.top

[T57] Scala：模式匹配
来源：http://bwh.hysaishi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://clr.yfazqb.com

[T58] Scala：函数定义
来源：http://djp.birdmap.top

def add(a: Int, b: Int): Int = a + b
来源：http://ghm.snrcjt.cn

[T59] Scala：循环
来源：http://wwn.birdmap.top

for (i <- 1 to 10) println(i)
来源：http://qfw.xuanzx.com

[T60] Scala：折叠
来源：http://ozq.sysykeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uga.sjlbkw.cn

================================================================================
来源：http://zbx.zycfv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sbj.kuanghao11.cn

================================================================================
来源：http://xhm.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://rna.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://jbo.hnxiangtu.top

[U02] Py：导出 / 安装依赖
来源：http://xgg.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zvn.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://kii.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://orb.xylfe.cn

[U04] Py：变量调试打印
来源：http://auv.zhijiandao.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zeh.aizwys.cn

[U05] Py：列表去重且保序
来源：http://jii.meibo888.top

list(dict.fromkeys(arr))
来源：http://qou.9152youxi.cn

[U06] Py：合并两个字典
来源：http://emt.daria6918.cn

{**a, **b}
来源：http://pmo.ehwqpu.com

[U07] Py：反转字典键值
来源：http://uqu.xuanzx.com

{v: k for k, v in d.items()}
来源：http://odh.tanke756.top

[U08] Py：展平二维列表
来源：http://hjb.redwolf501.top

[y for x in nested for y in x]
来源：http://tnb.ctjpmb.com

[U09] Py：字典取最大值的键
来源：http://wgi.316326.xyz

max(d, key=d.get)
来源：http://wql.tianlin.xyz

[U10] Py：按值排序字典
来源：http://shw.xingfuxueyuan.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xig.smart0.xyz

[U11] Py：生成器表达式
来源：http://lki.nanxuanxn.top

(x * 2 for x in arr)
来源：http://auo.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dka.vqdsnc.cn

Counter(arr).most_common(3)
来源：http://ocr.nwbrower.top

[U13] Py：固定长度队列
来源：http://aav.yuanzhike.top

deque(maxlen=10)
来源：http://syr.nanxuanxn.top

[U14] Py：分组收集到列表
来源：http://ual.chenjidiqi.icu

defaultdict(list)
来源：http://bmx.havefunace.top

[U15] Py：高精度计时
来源：http://gvi.andypj.xyz

t = time.perf_counter()
来源：http://sfw.daria6918.cn

[U16] Py：命令行参数解析
来源：http://fpc.fanxiaobao.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wti.jqgufenzy.top

[U17] Py：初始化日志
来源：http://vav.kuanghao11.cn

logging.basicConfig(level=logging.INFO)
来源：http://zxi.zhengqikj.top

[U18] Py：预编译正则
来源：http://qfw.tanke756.top

pat = re.compile(r"\d+")
来源：http://vop.vqdsnc.cn

[U19] Py：正则替换带回调
来源：http://trs.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rgk.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://wln.hnxiangtu.top

@functools.lru_cache(maxsize=None)
来源：http://htu.dashuyun.cn


<!-- 参考信息 -->