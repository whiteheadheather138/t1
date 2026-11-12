代发 wailian999

S. C / C++ 专题
来源：http://ycg.hfpthk.cn

================================================================================
来源：http://xtj.vqdsnc.cn

[S01] C：Hello World
来源：http://hcy.epnwcf.com

#include <stdio.h>
来源：http://giv.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zoa.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://vgc.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://kem.fzhhl.top

[S03] C：读入整数
来源：http://jom.uphjek.com

int x; scanf("%d", &x);
来源：http://lxj.daria6918.cn

[S04] C：字符串复制
来源：http://mvp.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xoy.ybcxt.top

[S05] C：字符串长度
来源：http://gun.yj202588.top

strlen(s)
来源：http://yrn.fehbvm.com

[S06] C：字符串比较
来源：http://cww.vehdjk.com

strcmp(a, b) == 0
来源：http://dbg.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://gbm.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uqd.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://eys.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wnv.sjlbkw.cn

[S09] C：结构体定义与初始化
来源：http://tdt.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lsm.chenlongwang.top

[S10] C：指针与解引用
来源：http://vse.guannengcc.top

int *p = &a;  *p = 5;
来源：http://xtm.hongshengwenyu.top

[S11] C：逐行读文件
来源：http://pcz.ydjk.org.cn

FILE *f = fopen("a.txt", "r");
来源：http://mni.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ouh.c1oappe.top

fclose(f);
来源：http://qqj.yvedp.cn

[S12] C：写文件
来源：http://fmv.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://soi.mhx1999.top

[S13] C：宏定义
来源：http://pet.yj20258.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jia.shanyushiyangkeji.top

[S14] C：枚举
来源：http://xwc.316326.xyz

enum Color { RED, GREEN, BLUE };
来源：http://odw.yongpay.top

[S15] C：类型转换
来源：http://rhg.dashuyun.cn

(double) a / b
来源：http://npn.yvedp.cn

[S16] C：位操作置位
来源：http://qsr.jinqigufen.top

x |= (1 << 3);
来源：http://exb.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://ygl.hesvh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://elj.gogol.net.cn

[S18] C：命令行参数
来源：http://tna.cheryme.top

int main(int argc, char **argv)
来源：http://pol.zdbjq.cn

[S19] C：快速排序
来源：http://auf.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://azh.dashuyun.cn

[S20] C：二分查找
来源：http://gxg.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uyz.guannengcc.top

[S21] C：字符类别判断
来源：http://gqb.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tjc.cdnleiting.top

[S22] C：字符串转数字
来源：http://xux.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://lps.hesvh.cn

[S23] C：随机数
来源：http://zau.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ffn.quarkkingdee.top

[S24] C：获取本地时间
来源：http://jlo.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xmg.fzhhl.top

[S25] C：内存拷贝
来源：http://klu.chenzaomai.com

memcpy(dst, src, n);
来源：http://uyk.cqqwz.cn

[S26] C：内存清零
来源：http://ukk.jiagoushi.top

memset(a, 0, sizeof a);
来源：http://hxk.chenjidiqi.icu

[S27] C：定义常量
来源：http://fbc.ppjwa.cn

const double PI = 3.14159;
来源：http://qxd.tarul.cn

[S28] C：静态变量
来源：http://ysu.pycfn.com

static int counter = 0;
来源：http://vll.dianchejie.cn

[S29] C：变参函数
来源：http://nnq.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pcl.cucudq.cn

[S30] C：头文件保护
来源：http://giz.tianlin.xyz

#ifndef X_H
来源：http://cee.yfazqb.com

#define X_H
来源：http://vvz.aizwys.cn

#endif
来源：http://fgl.svipenyu.cn

[S31] C++：Hello World
来源：http://hkr.hnqzz.top

#include <iostream>
来源：http://bci.nanxuanxn.top

int main() { std::cout << "Hello\n"; }
来源：http://giv.ydzc1.top

[S32] C++：字符串
来源：http://dap.jyoumei.cn

std::string s = "hi";  s += "!";
来源：http://yaa.fzhhl.top

[S33] C++：vector 增删
来源：http://dbb.dianchejie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kbi.haohaochexian.top

[S34] C++：遍历 vector
来源：http://yxy.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://fbu.birdmap.top

[S35] C++：map
来源：http://yon.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nfl.shzxlz.cn

[S36] C++：unordered_map
来源：http://psm.chenzaomai.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://alo.zhijiandao.cn

[S37] C++：set
来源：http://rwh.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fij.tian-w.cn

[S38] C++：排序
来源：http://hhp.vqdsnc.cn

std::sort(v.begin(), v.end());
来源：http://nev.daria6918.cn

[S39] C++：自定义比较器排序
来源：http://inr.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jsq.jinqigufen.top

[S40] C++：查找元素
来源：http://vqq.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pit.yuanzhike.top

[S41] C++：类与构造函数
来源：http://pct.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yvs.tanke756.top

[S42] C++：继承与虚函数
来源：http://ezb.yuxming.cn

class B : public Base { public: void f() override {} };
来源：http://rpt.yfazqb.com

[S43] C++：智能指针
来源：http://zbj.zdqjudy.top

auto p = std::make_unique<int>(5);
来源：http://osh.zhaomingkeji.xyz

[S44] C++：引用传参
来源：http://mok.ydjk.org.cn

void inc(int &x) { ++x; }
来源：http://vtj.guowangkeji.top

[S45] C++：lambda
来源：http://tcq.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://got.jlsjyb.cn

[S46] C++：函数模板
来源：http://eqf.jianghu66.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vfm.gotoacloud.top

[S47] C++：结构化绑定遍历
来源：http://sqv.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ksx.jyoumei.cn

[S48] C++：逐行读文件
来源：http://mtb.sysykeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://mfa.hesvh.cn

while (std::getline(in, line)) { }
来源：http://gzu.316326.xyz

[S49] C++：写文件
来源：http://yic.zhengqikj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fyh.shuidangran.top

[S50] C++：格式化数字
来源：http://nrq.shanyushiyangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ira.fanxiaobao.xyz

[S51] C++：显式类型转换
来源：http://rjs.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://zue.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://coy.meibo888.top

int size() const noexcept { return n_; }
来源：http://wsb.sufxvd.cn

[S53] C++：移动语义
来源：http://xpx.jqgfzy.top

std::vector<int> w = std::move(v);
来源：http://fie.yuanzhike.top

[S54] C++：异常处理
来源：http://igp.shanyushiyangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jhs.smart0.xyz

[S55] C++：结构化绑定
来源：http://spj.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mgi.hesvh.cn

[S56] C++：optional
来源：http://qlc.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gjt.guowangkeji.top

[S57] C++：编译期常量
来源：http://xrf.yuanzhike.top

constexpr int N = 10;
来源：http://pen.zhongyouzk.top

[S58] C++：命名空间
来源：http://bha.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://oum.aizwys.cn

[S59] C++：静态断言
来源：http://qzl.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://caj.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://ikl.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://drh.wangshuangyany.cn

================================================================================
来源：http://pol.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gvo.tarul.cn

================================================================================
来源：http://hkp.wangdashe.top

[T01] Kotlin：Hello World
来源：http://rbj.dianchejie.cn

println("Hello")
来源：http://dtj.snrcjt.cn

[T02] Kotlin：变量
来源：http://krj.gzhubu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://evl.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://qqz.fktsv.cn

"值: $b"
来源：http://mto.ywan-chungtsiang.top

[T04] Kotlin：空安全
来源：http://qgp.cashguo.top

val n: String? = null;  n?.length
来源：http://uqr.hongshengwenyu.top

[T05] Kotlin：when 表达式
来源：http://jts.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qwp.hesvh.cn

[T06] Kotlin：集合映射
来源：http://nvm.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gfe.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://sln.guowangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rpw.zhixingplan.top

[T08] Kotlin：数据类
来源：http://lmj.meibo888.top

data class User(val name: String, val age: Int)
来源：http://ydh.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://pmq.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://tnu.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://win.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qyc.yj202588.top

[T11] Kotlin：协程
来源：http://iyy.tian-w.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pjs.xylfe.cn

[T12] Kotlin：解构声明
来源：http://ofk.jlsjyb.cn

val (a, b) = Pair(1, 2)
来源：http://udf.hnqzz.top

[T13] Kotlin：只读 Map
来源：http://zpc.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://sei.gogol.net.cn

[T14] Kotlin：循环
来源：http://btz.aibaodan.cn

for (i in 1..10) println(i)
来源：http://sbj.ydjk.org.cn

[T15] Kotlin：接口
来源：http://rng.bbcook.cn

interface Shape { fun area(): Double }
来源：http://kyo.yanxiufei.cn

[T16] Swift：Hello World
来源：http://ywx.zhiwuduotai.top

print("Hello")
来源：http://hja.andypj.xyz

[T17] Swift：变量与常量
来源：http://puv.tarul.cn

var a = 1;  let b = 2
来源：http://cbx.bjfxy.top

[T18] Swift：字符串插值
来源：http://ppj.dianchejie.cn

"值: \(b)"
来源：http://hsa.nanxinkj.top

[T19] Swift：可选绑定
来源：http://tid.316326.xyz

if let n = opt { print(n) }
来源：http://jys.sweek.top

[T20] Swift：数组操作
来源：http://fsp.dianchejie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gpm.yanxiufei.cn

[T21] Swift：遍历
来源：http://ffc.daxiang520.top

for x in a { print(x) }
来源：http://mcp.gaohongyu789.top

[T22] Swift：字典
来源：http://pmq.vqdsnc.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fpd.gzhubu.top

[T23] Swift：函数
来源：http://gou.guannengcc.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hul.xylfe.cn

[T24] Swift：闭包
来源：http://sjm.yfazqb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://qjp.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://gvi.snrcjt.cn

struct P { var x: Int }
来源：http://ypd.cucudq.cn

[T26] Swift：类与重写
来源：http://zpe.yuanzhike.top

class A: Base { override func f() {} }
来源：http://jzi.gotoacloud.top

[T27] Swift：错误处理
来源：http://leb.tanke756.top

do { try f() } catch { print(error) }
来源：http://xmx.jqgufenzy.top

[T28] Swift：枚举
来源：http://dqi.hnxiangtu.top

enum Color { case red, green }
来源：http://pse.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://czf.zhijiandao.cn

guard let x = opt else { return }
来源：http://qgs.yj20258.top

[T30] Swift：协议
来源：http://djx.vehdjk.com

protocol Shape { func area() -> Double }
来源：http://amv.yueranfly.top

[T31] Lua：Hello World
来源：http://ftu.xuanzx.com

print("Hello")
来源：http://dwn.sysykeji.top

[T32] Lua：局部变量
来源：http://vuh.fengsongda.top

local a = 1
来源：http://qyh.hysaishi.cn

[T33] Lua：表（数组）
来源：http://dps.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rcv.yangfankeji.com

[T34] Lua：遍历表
来源：http://wag.bjfxy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fyq.ehwqpu.com

[T35] Lua：字典表
来源：http://dxv.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://kgj.ydzc1.top

[T36] Lua：函数
来源：http://gla.ivvv.top

function add(a, b) return a + b end
来源：http://cio.daria6918.cn

[T37] Lua：字符串拼接
来源：http://wmx.zycfv.cn

"a" .. "b"
来源：http://thk.hcnkem.com

[T38] Lua：条件
来源：http://rbh.vehdjk.com

if x > 0 then print("正") end
来源：http://xtq.havefunace.top

[T39] Lua：模式匹配
来源：http://orx.sufxvd.cn

string.find(s, "%d+")
来源：http://mua.nwbrower.top

[T40] Lua：元表
来源：http://cap.yueranfly.top

setmetatable({}, { __index = base })
来源：http://tfb.9152youxi.cn

[T41] Perl：Hello World
来源：http://pph.jianghu66.top

print "Hello\n";
来源：http://kiq.vehdjk.com

[T42] Perl：变量类型
来源：http://icr.9152youxi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://acq.cdnleiting.top

[T43] Perl：字符串插值
来源：http://pql.xylfe.cn

"值: $a"
来源：http://woh.dashuyun.cn

[T44] Perl：条件
来源：http://dwa.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://lgy.fktsv.cn

[T45] Perl：数组遍历
来源：http://eoc.ivvv.top

for my $x (@arr) { print $x; }
来源：http://ial.vehdjk.com

[T46] Perl：哈希操作
来源：http://pok.sxryk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ffb.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://bbc.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://txq.yanxiufei.cn

[T48] Perl：正则替换
来源：http://ody.hfpthk.cn

$s =~ s/old/new/g;
来源：http://oip.jqgfzy.top

[T49] Perl：函数
来源：http://wjq.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hkv.vqdsnc.cn

[T50] Perl：逐行读文件
来源：http://xyg.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yss.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://axn.yfazqb.com

[T51] Scala：Hello World
来源：http://umr.nanxinkj.top

println("Hello")
来源：http://scl.iojbl.cn

[T52] Scala：变量
来源：http://htx.hywenlv.cn

val a = 1;  var b = 2
来源：http://smr.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://odq.jinyuanbaomall.cn

s"值: $b"
来源：http://ohy.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://ukm.aizwys.cn

List(1, 2, 3).map(_ * 2)
来源：http://hhm.guannengcc.top

[T55] Scala：集合过滤
来源：http://skc.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://wry.sjlbkw.cn

[T56] Scala：样例类
来源：http://omo.jinqigfzy.top

case class User(name: String, age: Int)
来源：http://wrn.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://pkg.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xhx.jqgfzy.top

[T58] Scala：函数定义
来源：http://jzk.shangyingyoupin.top

def add(a: Int, b: Int): Int = a + b
来源：http://irz.0kj1m.cn

[T59] Scala：循环
来源：http://fsv.cucudq.cn

for (i <- 1 to 10) println(i)
来源：http://yxh.jqgfzy.top

[T60] Scala：折叠
来源：http://obk.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jvj.jiagoushi.top

================================================================================
来源：http://hcb.redwolf501.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mup.ybcxt.top

================================================================================
来源：http://hsm.zhijiandao.cn

[U01] Py：创建虚拟环境
来源：http://gin.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://imw.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://bbd.ivvv.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nmn.yj202588.top

[U03] Py：加载 .env 配置
来源：http://yts.iojbl.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fkk.sysykeji.top

[U04] Py：变量调试打印
来源：http://lgh.quarkkingdee.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wek.shanyushiyangkeji.top

[U05] Py：列表去重且保序
来源：http://acc.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://aou.ppjwa.cn

[U06] Py：合并两个字典
来源：http://ywh.feifeiyinyue.top

{**a, **b}
来源：http://nhz.havefunace.top

[U07] Py：反转字典键值
来源：http://qbb.cashguo.top

{v: k for k, v in d.items()}
来源：http://svq.gotoacloud.top

[U08] Py：展平二维列表
来源：http://qvg.haohaochexian.top

[y for x in nested for y in x]
来源：http://hkw.yj20258.top

[U09] Py：字典取最大值的键
来源：http://pnz.jinqigufen.top

max(d, key=d.get)
来源：http://jfq.0kj1m.cn

[U10] Py：按值排序字典
来源：http://aek.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://egu.jianghu66.top

[U11] Py：生成器表达式
来源：http://wnf.zdbjq.cn

(x * 2 for x in arr)
来源：http://oct.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zwp.chenzaomai.com

Counter(arr).most_common(3)
来源：http://kse.smart0.xyz

[U13] Py：固定长度队列
来源：http://keu.hcnkem.com

deque(maxlen=10)
来源：http://ztt.nwbrower.top

[U14] Py：分组收集到列表
来源：http://sdx.nanxinkj.top

defaultdict(list)
来源：http://wbf.epnwcf.com

[U15] Py：高精度计时
来源：http://uhy.c1oappe.top

t = time.perf_counter()
来源：http://kfp.uphjek.com

[U16] Py：命令行参数解析
来源：http://qfa.sjlbkw.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fsa.tanke756.top

[U17] Py：初始化日志
来源：http://vhr.wangshuangyany.cn

logging.basicConfig(level=logging.INFO)
来源：http://nud.zhongyouzk.top

[U18] Py：预编译正则
来源：http://ucc.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://dtg.havefunace.top

[U19] Py：正则替换带回调
来源：http://kwi.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zam.kuanghao11.cn

[U20] Py：缓存函数结果
来源：http://rff.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://ccx.guowangkeji.top

[U21] Py：自定义上下文管理器
来源：http://nxt.jinyuanbaomall.cn

@contextlib.contextmanager
来源：http://qag.fengsongda.top

[U22] Py：矩阵转置
来源：http://rmi.redwolf501.top

list(zip(*m))
来源：http://ugq.birdmap.top


<!-- 参考信息 -->