代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://fgv.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://gjp.fengsongda.top

int a = 10; printf("%d\n", a);
来源：http://qsw.wangdashe.top

[S03] C：读入整数
来源：http://ble.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://ppi.jqgufenzy.top

[S04] C：字符串复制
来源：http://epd.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xqo.xuanzx.com

[S05] C：字符串长度
来源：http://tgg.hnqzz.top

strlen(s)
来源：http://tom.yj20258.top

[S06] C：字符串比较
来源：http://kfx.jianghu66.top

strcmp(a, b) == 0
来源：http://wal.redwolf501.top

[S07] C：数组遍历求和
来源：http://apy.cdnleiting.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bgn.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://etw.yueranfly.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sea.ydjk.org.cn

[S09] C：结构体定义与初始化
来源：http://rzm.nanxuanxn.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ahj.yfazqb.com

[S10] C：指针与解引用
来源：http://bbt.zhixingplan.top

int *p = &a;  *p = 5;
来源：http://hvr.ctjpmb.com

[S11] C：逐行读文件
来源：http://kzj.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://psm.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ybj.c1oappe.top

fclose(f);
来源：http://mfh.guannengcc.top

[S12] C：写文件
来源：http://pkh.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rxz.quarkkingdee.top

[S13] C：宏定义
来源：http://uvo.shuidangran.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://abt.wangdashe.top

[S14] C：枚举
来源：http://umy.zhaomingkeji.xyz

enum Color { RED, GREEN, BLUE };
来源：http://rir.xziqi.cn

[S15] C：类型转换
来源：http://vha.52xcode.cn

(double) a / b
来源：http://hdj.hfpthk.cn

[S16] C：位操作置位
来源：http://zuy.nanxuanxn.top

x |= (1 << 3);
来源：http://sml.tian-w.cn

[S17] C：安全拼接字符串
来源：http://hzi.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zuj.hfpthk.cn

[S18] C：命令行参数
来源：http://pnf.sjlbkw.cn

int main(int argc, char **argv)
来源：http://ise.cqqwz.cn

[S19] C：快速排序
来源：http://agg.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://zhg.hnxiangtu.top

[S20] C：二分查找
来源：http://mwu.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://flp.daxiang520.top

[S21] C：字符类别判断
来源：http://ojh.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://why.dianchejie.cn

[S22] C：字符串转数字
来源：http://hju.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nfe.mhx1999.top

[S23] C：随机数
来源：http://oey.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://plk.pengpengdd.cyou

[S24] C：获取本地时间
来源：http://mmk.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wub.yueranfly.top

[S25] C：内存拷贝
来源：http://qgf.snrcjt.cn

memcpy(dst, src, n);
来源：http://uln.cqqwz.cn

[S26] C：内存清零
来源：http://xfl.havefunace.top

memset(a, 0, sizeof a);
来源：http://tnv.c1oappe.top

[S27] C：定义常量
来源：http://hzz.redwolf501.top

const double PI = 3.14159;
来源：http://wpi.sufxvd.cn

[S28] C：静态变量
来源：http://ffq.havefunace.top

static int counter = 0;
来源：http://tmk.ydzc1.top

[S29] C：变参函数
来源：http://bqz.nanxinkj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aog.gzhubu.top

[S30] C：头文件保护
来源：http://eqh.cucudq.cn

#ifndef X_H
来源：http://ndp.tian-w.cn

#define X_H
来源：http://obs.hammf.cn

#endif
来源：http://tuq.hnqzz.top

[S31] C++：Hello World
来源：http://gap.jyoumei.cn

#include <iostream>
来源：http://mcv.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://yrp.0kj1m.cn

[S32] C++：字符串
来源：http://msk.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://gkb.yuxming.cn

[S33] C++：vector 增删
来源：http://pxa.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kbv.cashguo.top

[S34] C++：遍历 vector
来源：http://wmu.quarkkingdee.top

for (auto &x : v) { std::cout << x; }
来源：http://fix.xuetiantiany.cn

[S35] C++：map
来源：http://mpv.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rha.ppjwa.cn

[S36] C++：unordered_map
来源：http://fwg.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xxo.shuidangran.top

[S37] C++：set
来源：http://fzd.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hvj.tanke756.top

[S38] C++：排序
来源：http://gav.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://jyp.hysaishi.cn

[S39] C++：自定义比较器排序
来源：http://fai.tarul.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://izz.xylfe.cn

[S40] C++：查找元素
来源：http://jnk.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tnb.fengsongda.top

[S41] C++：类与构造函数
来源：http://iqs.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ryr.yj20258888.top

[S42] C++：继承与虚函数
来源：http://woh.zhijiandao.cn

class B : public Base { public: void f() override {} };
来源：http://uhf.yueranfly.top

[S43] C++：智能指针
来源：http://hkt.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://fwv.jinqigfzy.top

[S44] C++：引用传参
来源：http://xlk.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://odl.hysaishi.cn

[S45] C++：lambda
来源：http://hez.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qyf.smart0.xyz

[S46] C++：函数模板
来源：http://djr.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://swz.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://mmi.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://knu.ywan-chungtsiang.top

[S48] C++：逐行读文件
来源：http://dnq.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sri.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://khe.fanxiaobao.xyz

[S49] C++：写文件
来源：http://xmi.tianlin.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jbd.hfpthk.cn

[S50] C++：格式化数字
来源：http://fkq.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hby.xuanzx.com

[S51] C++：显式类型转换
来源：http://jno.iojbl.cn

static_cast<double>(a) / b
来源：http://wcv.jqgufenzy.top

[S52] C++：const 与 noexcept
来源：http://qwd.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://olh.sjlbkw.cn

[S53] C++：移动语义
来源：http://djt.bjfxy.top

std::vector<int> w = std::move(v);
来源：http://qtu.yj20258888.top

[S54] C++：异常处理
来源：http://qrf.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mkm.fehbvm.com

[S55] C++：结构化绑定
来源：http://dup.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jzi.quarkkingdee.top

[S56] C++：optional
来源：http://moq.jqgufenzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://twy.yfazqb.com

[S57] C++：编译期常量
来源：http://zgk.tarul.cn

constexpr int N = 10;
来源：http://xom.jinqigufen.top

[S58] C++：命名空间
来源：http://ksh.andypj.xyz

namespace ns { int f() { return 1; } }
来源：http://ycy.nwbrower.top

[S59] C++：静态断言
来源：http://yhk.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://njb.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://rbi.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bfm.jinghuilouyu.cn

================================================================================
来源：http://ehm.cashguo.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ziz.sweek.top

================================================================================
来源：http://hvq.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://xyu.sufxvd.cn

println("Hello")
来源：http://fhx.jyoumei.cn

[T02] Kotlin：变量
来源：http://txq.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gyd.yj20258.top

[T03] Kotlin：字符串模板
来源：http://jfk.zhaomingkeji.xyz

"值: $b"
来源：http://vkm.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://xac.zhijiandao.cn

val n: String? = null;  n?.length
来源：http://tvk.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://zso.meibo888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dop.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://lvg.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://gms.yonumen.top

[T07] Kotlin：集合过滤
来源：http://bzg.xingfuxueyuan.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://voi.yj202588.top

[T08] Kotlin：数据类
来源：http://whm.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://epi.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://wpw.hywenlv.cn

fun String.exclaim() = this + "!"
来源：http://cpv.hesvh.cn

[T10] Kotlin：默认参数
来源：http://zkn.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rvb.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://ytt.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tos.shuidangran.top

[T12] Kotlin：解构声明
来源：http://sxx.shanyushiyangkeji.top

val (a, b) = Pair(1, 2)
来源：http://rch.jyoumei.cn

[T13] Kotlin：只读 Map
来源：http://twe.jiagoushi.top

val m = mapOf("a" to 1)
来源：http://vxe.shanyushiyangtech.top

[T14] Kotlin：循环
来源：http://wsj.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://ibu.redwolf501.top

[T15] Kotlin：接口
来源：http://azh.zycfv.cn

interface Shape { fun area(): Double }
来源：http://zsp.52xcode.cn

[T16] Swift：Hello World
来源：http://jek.ctjpmb.com

print("Hello")
来源：http://awt.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://gfa.shzxlz.cn

var a = 1;  let b = 2
来源：http://qeq.wangdashe.top

[T18] Swift：字符串插值
来源：http://dlw.gogol.net.cn

"值: \(b)"
来源：http://iti.chenlongwang.top

[T19] Swift：可选绑定
来源：http://ojy.xylfe.cn

if let n = opt { print(n) }
来源：http://blr.zdbjq.cn

[T20] Swift：数组操作
来源：http://ohu.ctjpmb.com

var a = [1, 2, 3];  a.append(4)
来源：http://xto.zhixingplan.top

[T21] Swift：遍历
来源：http://leu.redwolf501.top

for x in a { print(x) }
来源：http://rwh.xylfe.cn

[T22] Swift：字典
来源：http://ovw.hammf.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mlv.c1oappe.top

[T23] Swift：函数
来源：http://ydk.yanxiufei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xwi.yj20258.top

[T24] Swift：闭包
来源：http://uvz.tian-w.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pcb.nanxuanxn.top

[T25] Swift：结构体
来源：http://gtp.cqqwz.cn

struct P { var x: Int }
来源：http://gyp.zhongyouzk.top

[T26] Swift：类与重写
来源：http://cyr.xylfe.cn

class A: Base { override func f() {} }
来源：http://tub.havefunace.top

[T27] Swift：错误处理
来源：http://kot.daxiang520.top

do { try f() } catch { print(error) }
来源：http://mmp.bbcook.cn

[T28] Swift：枚举
来源：http://oyz.0kj1m.cn

enum Color { case red, green }
来源：http://wtp.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://osy.guannengcc.top

guard let x = opt else { return }
来源：http://cfy.shuidangran.top

[T30] Swift：协议
来源：http://hov.tarul.cn

protocol Shape { func area() -> Double }
来源：http://nrf.nanxinkj.top

[T31] Lua：Hello World
来源：http://ppb.vqdsnc.cn

print("Hello")
来源：http://pzn.iojbl.cn

[T32] Lua：局部变量
来源：http://nqt.aibaodan.cn

local a = 1
来源：http://vml.redwolf501.top

[T33] Lua：表（数组）
来源：http://pfc.hongshengwenyu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://saf.cdnleiting.top

[T34] Lua：遍历表
来源：http://knm.sxryk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mcx.nwbrower.top

[T35] Lua：字典表
来源：http://dcr.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://jmv.bbcook.cn

[T36] Lua：函数
来源：http://vph.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://lrs.birdmap.top

[T37] Lua：字符串拼接
来源：http://xzh.shanyushiyangkeji.top

"a" .. "b"
来源：http://ncp.cucudq.cn

[T38] Lua：条件
来源：http://irl.wangdashe.top

if x > 0 then print("正") end
来源：http://wht.cqqwz.cn

[T39] Lua：模式匹配
来源：http://svm.tianlin.xyz

string.find(s, "%d+")
来源：http://uad.pengpengdd.cyou

[T40] Lua：元表
来源：http://ghr.9152youxi.cn

setmetatable({}, { __index = base })
来源：http://qki.dashuyun.cn

[T41] Perl：Hello World
来源：http://pal.yueranfly.top

print "Hello\n";
来源：http://xku.hysaishi.cn

[T42] Perl：变量类型
来源：http://tdl.yuanzhike.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://smi.jinqigufen.top

[T43] Perl：字符串插值
来源：http://ddz.hnxiangtu.top

"值: $a"
来源：http://hch.ydjk.org.cn

[T44] Perl：条件
来源：http://gqx.tanke756.top

if ($a > 0) { print "正"; }
来源：http://ayc.guowangkeji.top

[T45] Perl：数组遍历
来源：http://vii.hywenlv.cn

for my $x (@arr) { print $x; }
来源：http://swt.sjlbkw.cn

[T46] Perl：哈希操作
来源：http://fuu.vehdjk.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ygu.shzxlz.cn

[T47] Perl：正则捕获
来源：http://ppt.yj20258888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xpa.zdqjudy.top

[T48] Perl：正则替换
来源：http://buc.sufxvd.cn

$s =~ s/old/new/g;
来源：http://gtp.ctjpmb.com

[T49] Perl：函数
来源：http://kpj.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ywz.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://glh.xuanzx.com

open my $fh, "<", "a.txt" or die $!;
来源：http://fsc.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://viy.meibo888.top

[T51] Scala：Hello World
来源：http://akn.9152youxi.cn

println("Hello")
来源：http://tdm.dianchejie.cn

[T52] Scala：变量
来源：http://hir.svipenyu.cn

val a = 1;  var b = 2
来源：http://skg.ybcxt.top

[T53] Scala：字符串插值
来源：http://gkv.xinyue.icu

s"值: $b"
来源：http://cmj.bjfxy.top

[T54] Scala：集合映射
来源：http://jyq.snrcjt.cn

List(1, 2, 3).map(_ * 2)
来源：http://nkg.dianchejie.cn

[T55] Scala：集合过滤
来源：http://dif.zhengqikj.top

List(1, 2, 3).filter(_ > 1)
来源：http://urv.zhixingplan.top

[T56] Scala：样例类
来源：http://qgc.jinyuanbaomall.cn

case class User(name: String, age: Int)
来源：http://eal.yvedp.cn

[T57] Scala：模式匹配
来源：http://shn.vehdjk.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://lqv.guowangkeji.top

[T58] Scala：函数定义
来源：http://lbk.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ymw.xuetiantiany.cn

[T59] Scala：循环
来源：http://veg.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://itq.andypj.xyz

[T60] Scala：折叠
来源：http://gwq.jinqigufen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://miy.chenjidiqi.icu

================================================================================
来源：http://pur.aibaodan.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tqy.jianghu66.top

================================================================================
来源：http://bem.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://lfs.fengsongda.top

python -m venv .venv && source .venv/bin/activate
来源：http://ytb.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://fgg.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uwc.meibo888.top

[U03] Py：加载 .env 配置
来源：http://omr.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fqe.tarul.cn

[U04] Py：变量调试打印
来源：http://rkt.hammf.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cwd.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://hnc.bbcook.cn

list(dict.fromkeys(arr))
来源：http://uey.xylfe.cn

[U06] Py：合并两个字典
来源：http://otx.yj20258.top

{**a, **b}
来源：http://odx.cqqwz.cn

[U07] Py：反转字典键值
来源：http://zzy.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://ldl.yueranfly.top

[U08] Py：展平二维列表
来源：http://ogq.xziqi.cn

[y for x in nested for y in x]
来源：http://nze.yuxming.cn

[U09] Py：字典取最大值的键
来源：http://xao.kuanghao11.cn

max(d, key=d.get)
来源：http://kmz.ybcxt.top

[U10] Py：按值排序字典
来源：http://gml.52xcode.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xpl.shzxlz.cn

[U11] Py：生成器表达式
来源：http://vet.jianghu66.top

(x * 2 for x in arr)
来源：http://egk.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xaj.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://mtn.pycfn.com

[U13] Py：固定长度队列
来源：http://knd.zhiwuduotai.top

deque(maxlen=10)
来源：http://tbu.chenzaomai.com

[U14] Py：分组收集到列表
来源：http://iui.yuxming.cn

defaultdict(list)
来源：http://uxm.yj202588.top

[U15] Py：高精度计时
来源：http://grj.aizwys.cn

t = time.perf_counter()
来源：http://lwa.kuanghao11.cn

[U16] Py：命令行参数解析
来源：http://joh.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://edl.ywan-chungtsiang.top

[U17] Py：初始化日志
来源：http://wxj.c1oappe.top

logging.basicConfig(level=logging.INFO)
来源：http://gcr.aizwys.cn

[U18] Py：预编译正则
来源：http://irf.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://sgh.jiagoushi.top

[U19] Py：正则替换带回调
来源：http://nfm.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://inm.yuanzhike.top

[U20] Py：缓存函数结果
来源：http://tks.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://zxp.ehwqpu.com

[U21] Py：自定义上下文管理器
来源：http://bas.dashuyun.cn

@contextlib.contextmanager
来源：http://slw.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://hxe.guannengcc.top

list(zip(*m))
来源：http://hnj.nwbrower.top

[U23] Py：分块读取大文件
来源：http://vzs.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kos.fehbvm.com

[U24] Py：路径操作
来源：http://xjd.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://grs.jinyuanbaomall.cn


<!-- 参考信息 -->