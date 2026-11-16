代发 wailian999

S. C / C++ 专题
来源：http://tjg.9152youxi.cn

================================================================================
来源：http://gmk.zhijiandao.cn

[S01] C：Hello World
来源：http://wxq.andypj.xyz

#include <stdio.h>
来源：http://zrj.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xvz.guannengcc.top

[S02] C：变量与格式化输出
来源：http://psp.gogol.net.cn

int a = 10; printf("%d\n", a);
来源：http://mpb.xinyue.icu

[S03] C：读入整数
来源：http://wcp.hywenlv.cn

int x; scanf("%d", &x);
来源：http://oia.birdmap.top

[S04] C：字符串复制
来源：http://bww.hongshengwenyu.top

char dst[32]; strcpy(dst, "hi");
来源：http://ftw.zycfv.cn

[S05] C：字符串长度
来源：http://mdc.redwolf501.top

strlen(s)
来源：http://qzz.jinqigufen.top

[S06] C：字符串比较
来源：http://ejw.ehwqpu.com

strcmp(a, b) == 0
来源：http://suu.smart0.xyz

[S07] C：数组遍历求和
来源：http://pqi.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zjb.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://iam.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bim.hnqzz.top

[S09] C：结构体定义与初始化
来源：http://okw.birdmap.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://djx.pycfn.com

[S10] C：指针与解引用
来源：http://zzd.havefunace.top

int *p = &a;  *p = 5;
来源：http://wsg.pengpengdd.cyou

[S11] C：逐行读文件
来源：http://zry.yongpay.top

FILE *f = fopen("a.txt", "r");
来源：http://ksx.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nyu.mhx1999.top

fclose(f);
来源：http://zmc.zhaomingkeji.xyz

[S12] C：写文件
来源：http://hem.yangfankeji.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://diz.sxryk.cn

[S13] C：宏定义
来源：http://dax.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cxa.hesvh.cn

[S14] C：枚举
来源：http://scy.hysaishi.cn

enum Color { RED, GREEN, BLUE };
来源：http://oiy.meibo888.top

[S15] C：类型转换
来源：http://zaz.ppjwa.cn

(double) a / b
来源：http://evr.ywan-chungtsiang.top

[S16] C：位操作置位
来源：http://wgg.fanxiaobao.xyz

x |= (1 << 3);
来源：http://paj.yj20258888.top

[S17] C：安全拼接字符串
来源：http://zbr.hongshengwenyu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fag.zdqjudy.top

[S18] C：命令行参数
来源：http://sep.hammf.cn

int main(int argc, char **argv)
来源：http://khw.yvedp.cn

[S19] C：快速排序
来源：http://aks.dianchejie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ajv.xziqi.cn

[S20] C：二分查找
来源：http://eog.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xow.hnqzz.top

[S21] C：字符类别判断
来源：http://uek.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dqs.cheryme.top

[S22] C：字符串转数字
来源：http://upa.sweek.top

atoi("42");  strtod("3.14", NULL);
来源：http://gsb.xingfuxueyuan.xyz

[S23] C：随机数
来源：http://lns.cucudq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ora.meibo888.top

[S24] C：获取本地时间
来源：http://uel.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://owi.chenjidiqi.icu

[S25] C：内存拷贝
来源：http://jgd.9152youxi.cn

memcpy(dst, src, n);
来源：http://hsr.hysaishi.cn

[S26] C：内存清零
来源：http://nrh.jiagoushi.top

memset(a, 0, sizeof a);
来源：http://wvr.shanyushiyangtech.top

[S27] C：定义常量
来源：http://ose.xinyue.icu

const double PI = 3.14159;
来源：http://ysn.redwolf501.top

[S28] C：静态变量
来源：http://uvt.quarkkingdee.top

static int counter = 0;
来源：http://urw.zhijiandao.cn

[S29] C：变参函数
来源：http://vqs.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ikw.hnqzz.top

[S30] C：头文件保护
来源：http://zgt.zhiwuduotai.top

#ifndef X_H
来源：http://aad.shanyushiyangtech.top

#define X_H
来源：http://bwc.pycfn.com

#endif
来源：http://ysv.hnqzz.top

[S31] C++：Hello World
来源：http://euz.gaohongyu789.top

#include <iostream>
来源：http://jmp.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://snz.smart0.xyz

[S32] C++：字符串
来源：http://lqu.ydjk.org.cn

std::string s = "hi";  s += "!";
来源：http://vor.guannengcc.top

[S33] C++：vector 增删
来源：http://cmu.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kaa.yj20258.top

[S34] C++：遍历 vector
来源：http://ypg.jinqigfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://tes.hywenlv.cn

[S35] C++：map
来源：http://lyn.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rbh.nanxuanxn.top

[S36] C++：unordered_map
来源：http://hpt.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fxf.xingfuxueyuan.xyz

[S37] C++：set
来源：http://ebc.feifeiyinyue.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hfn.ehwqpu.com

[S38] C++：排序
来源：http://kfk.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://dgj.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://cyi.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oko.vehdjk.com

[S40] C++：查找元素
来源：http://hax.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://brv.zycfv.cn

[S41] C++：类与构造函数
来源：http://sqy.zdqjudy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pkf.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://fyx.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://faf.zhengqikj.top

[S43] C++：智能指针
来源：http://sdz.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://xlx.jyoumei.cn

[S44] C++：引用传参
来源：http://cjc.fengsongda.top

void inc(int &x) { ++x; }
来源：http://sxj.iojbl.cn

[S45] C++：lambda
来源：http://jrm.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://tro.hnxiangtu.top

[S46] C++：函数模板
来源：http://xqq.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xfq.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://sgf.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jud.yj20258.top

[S48] C++：逐行读文件
来源：http://nhp.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://yve.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://hwy.zhixingplan.top

[S49] C++：写文件
来源：http://qib.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ckz.yj20258888.top

[S50] C++：格式化数字
来源：http://qxh.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vgl.dianchejie.cn

[S51] C++：显式类型转换
来源：http://rbz.jianghu66.top

static_cast<double>(a) / b
来源：http://qeq.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://uib.tanke756.top

int size() const noexcept { return n_; }
来源：http://ajk.haohaochexian.top

[S53] C++：移动语义
来源：http://chi.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://ibg.svipenyu.cn

[S54] C++：异常处理
来源：http://drt.mhx1999.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eve.jqgufenzy.top

[S55] C++：结构化绑定
来源：http://you.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zef.zhoulong.xyz

[S56] C++：optional
来源：http://qks.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lkq.yueranfly.top

[S57] C++：编译期常量
来源：http://ojs.jinqigufen.top

constexpr int N = 10;
来源：http://svc.fktsv.cn

[S58] C++：命名空间
来源：http://zod.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://txi.gzhubu.top

[S59] C++：静态断言
来源：http://hmg.zhaomingkeji.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://myy.yongpay.top

[S60] C++：遍历并删除元素
来源：http://vdr.yueranfly.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jqg.gzhubu.top

================================================================================
来源：http://apj.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xcu.gogol.net.cn

================================================================================
来源：http://hqg.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://eqb.shanyushiyangtech.top

println("Hello")
来源：http://ypy.9152youxi.cn

[T02] Kotlin：变量
来源：http://dzr.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://utu.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://zoz.ppjwa.cn

"值: $b"
来源：http://okr.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://gxt.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://jtl.yuxming.cn

[T05] Kotlin：when 表达式
来源：http://jxd.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jma.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://wnx.ppjwa.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ttb.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://iqm.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://tww.cucudq.cn

[T08] Kotlin：数据类
来源：http://dee.sufxvd.cn

data class User(val name: String, val age: Int)
来源：http://nzf.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://ela.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://wzs.hfpthk.cn

[T10] Kotlin：默认参数
来源：http://zmm.yj20258.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ipd.aizwys.cn

[T11] Kotlin：协程
来源：http://jrs.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jls.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://jed.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://pnc.havefunace.top

[T13] Kotlin：只读 Map
来源：http://jzx.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://lxs.shanyushiyangkeji.top

[T14] Kotlin：循环
来源：http://vvm.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://bzg.jlsjyb.cn

[T15] Kotlin：接口
来源：http://wxu.fzhhl.top

interface Shape { fun area(): Double }
来源：http://nui.yuanzhike.top

[T16] Swift：Hello World
来源：http://vnj.jqgfzy.top

print("Hello")
来源：http://peb.jqgfzy.top

[T17] Swift：变量与常量
来源：http://iyo.jyoumei.cn

var a = 1;  let b = 2
来源：http://gao.yfazqb.com

[T18] Swift：字符串插值
来源：http://tky.snrcjt.cn

"值: \(b)"
来源：http://zsz.iojbl.cn

[T19] Swift：可选绑定
来源：http://kbz.xylfe.cn

if let n = opt { print(n) }
来源：http://aek.316326.xyz

[T20] Swift：数组操作
来源：http://ooj.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zhc.ywan-chungtsiang.top

[T21] Swift：遍历
来源：http://gkl.zycfv.cn

for x in a { print(x) }
来源：http://kme.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://lmi.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://otk.yangfankeji.com

[T23] Swift：函数
来源：http://oyj.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tzu.zhengqikj.top

[T24] Swift：闭包
来源：http://jiu.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qho.yanxiufei.cn

[T25] Swift：结构体
来源：http://vdb.gzhubu.top

struct P { var x: Int }
来源：http://ksx.jqgfzy.top

[T26] Swift：类与重写
来源：http://njg.xziqi.cn

class A: Base { override func f() {} }
来源：http://xqn.yvedp.cn

[T27] Swift：错误处理
来源：http://pnr.tarul.cn

do { try f() } catch { print(error) }
来源：http://iqv.gaohongyu789.top

[T28] Swift：枚举
来源：http://fqd.yuanzhike.top

enum Color { case red, green }
来源：http://rho.tian-w.cn

[T29] Swift：guard 提前返回
来源：http://qvv.shangyingyoupin.top

guard let x = opt else { return }
来源：http://ibd.tarul.cn

[T30] Swift：协议
来源：http://hss.shzxlz.cn

protocol Shape { func area() -> Double }
来源：http://tbv.bbcook.cn

[T31] Lua：Hello World
来源：http://eil.chenjidiqi.icu

print("Hello")
来源：http://gpe.feifeiyinyue.top

[T32] Lua：局部变量
来源：http://zmu.hfpthk.cn

local a = 1
来源：http://wqf.uphjek.com

[T33] Lua：表（数组）
来源：http://bik.kuanghao11.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dai.gotoacloud.top

[T34] Lua：遍历表
来源：http://jyl.yj20258.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fkh.cucudq.cn

[T35] Lua：字典表
来源：http://mcu.zhiwuduotai.top

local d = { a = 1 };  d.b = 2
来源：http://zrw.hywenlv.cn

[T36] Lua：函数
来源：http://pdf.yuanzhike.top

function add(a, b) return a + b end
来源：http://iel.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://exl.ydzc1.top

"a" .. "b"
来源：http://sch.hywenlv.cn

[T38] Lua：条件
来源：http://qxk.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://tbr.fehbvm.com

[T39] Lua：模式匹配
来源：http://wsi.zhixingplan.top

string.find(s, "%d+")
来源：http://jnv.ivvv.top

[T40] Lua：元表
来源：http://yst.shanyushiyangkeji.top

setmetatable({}, { __index = base })
来源：http://sgs.hywenlv.cn

[T41] Perl：Hello World
来源：http://ljb.ydjk.org.cn

print "Hello\n";
来源：http://zhn.gotoacloud.top

[T42] Perl：变量类型
来源：http://unz.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rrs.sxryk.cn

[T43] Perl：字符串插值
来源：http://yfh.hammf.cn

"值: $a"
来源：http://cor.jqgfzy.top

[T44] Perl：条件
来源：http://zvo.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://nvy.shuidangran.top

[T45] Perl：数组遍历
来源：http://byj.fktsv.cn

for my $x (@arr) { print $x; }
来源：http://wtx.jinghuilouyu.cn

[T46] Perl：哈希操作
来源：http://sty.hcnkem.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uyo.birdmap.top

[T47] Perl：正则捕获
来源：http://gdv.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://xri.cheryme.top

[T48] Perl：正则替换
来源：http://jhg.shuidangran.top

$s =~ s/old/new/g;
来源：http://cko.jinyuanbaomall.cn

[T49] Perl：函数
来源：http://zbt.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://peh.aibaodan.cn

[T50] Perl：逐行读文件
来源：http://iux.hywenlv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fuv.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://bbu.jqgufenzy.top

[T51] Scala：Hello World
来源：http://ljz.yuxming.cn

println("Hello")
来源：http://jue.shzxlz.cn

[T52] Scala：变量
来源：http://kua.zhengqikj.top

val a = 1;  var b = 2
来源：http://ojl.fengsongda.top

[T53] Scala：字符串插值
来源：http://mla.hesvh.cn

s"值: $b"
来源：http://xds.ybcxt.top

[T54] Scala：集合映射
来源：http://yuy.cqqwz.cn

List(1, 2, 3).map(_ * 2)
来源：http://xkk.c1oappe.top

[T55] Scala：集合过滤
来源：http://ota.guowangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://nsn.tanke756.top

[T56] Scala：样例类
来源：http://vvl.sweek.top

case class User(name: String, age: Int)
来源：http://xfb.chenzaomai.com

[T57] Scala：模式匹配
来源：http://xel.hammf.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://grr.shangyingyoupin.top

[T58] Scala：函数定义
来源：http://rdb.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://alp.sjlbkw.cn

[T59] Scala：循环
来源：http://bgb.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://xhx.nanxuanxn.top

[T60] Scala：折叠
来源：http://ccx.smart0.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://siv.xylfe.cn

================================================================================
来源：http://nap.gogol.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ske.aizwys.cn

================================================================================
来源：http://sck.yueranfly.top

[U01] Py：创建虚拟环境
来源：http://enw.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dxe.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://odd.jinyuanbaomall.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ofd.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://iag.quarkkingdee.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bpq.shuidangran.top

[U04] Py：变量调试打印
来源：http://atq.yj20258888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bcg.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://iwc.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://cvj.yangfankeji.com

[U06] Py：合并两个字典
来源：http://wkb.jinqigfzy.top

{**a, **b}
来源：http://beg.shzxlz.cn

[U07] Py：反转字典键值
来源：http://ity.ybcxt.top

{v: k for k, v in d.items()}
来源：http://mje.tarul.cn

[U08] Py：展平二维列表
来源：http://xfm.yueranfly.top

[y for x in nested for y in x]
来源：http://yps.tianlin.xyz

[U09] Py：字典取最大值的键
来源：http://anc.yongpay.top

max(d, key=d.get)
来源：http://url.hongshengwenyu.top

[U10] Py：按值排序字典
来源：http://rkv.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uqz.zycfv.cn

[U11] Py：生成器表达式
来源：http://eyk.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://hyv.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://vwu.guannengcc.top

Counter(arr).most_common(3)
来源：http://xzm.uphjek.com

[U13] Py：固定长度队列
来源：http://xuw.gogol.net.cn

deque(maxlen=10)
来源：http://nln.gzhubu.top

[U14] Py：分组收集到列表
来源：http://atn.jiagoushi.top

defaultdict(list)
来源：http://mho.pengpengdd.cyou

[U15] Py：高精度计时
来源：http://xpp.yvedp.cn

t = time.perf_counter()
来源：http://okz.aizwys.cn

[U16] Py：命令行参数解析
来源：http://djf.jianghu66.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aaw.chenlongwang.top

[U17] Py：初始化日志
来源：http://sho.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://oxo.hesvh.cn

[U18] Py：预编译正则
来源：http://lmc.yonumen.top

pat = re.compile(r"\d+")
来源：http://ywq.nwbrower.top

[U19] Py：正则替换带回调
来源：http://dca.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yyl.iojbl.cn

[U20] Py：缓存函数结果
来源：http://rku.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://dto.tanke756.top

[U21] Py：自定义上下文管理器
来源：http://pgj.epnwcf.com

@contextlib.contextmanager
来源：http://wzt.shanyushiyangtech.top

[U22] Py：矩阵转置
来源：http://wdh.mhx1999.top

list(zip(*m))
来源：http://fpk.fengsongda.top


<!-- 参考信息 -->