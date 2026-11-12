代发 wailian999

S. C / C++ 专题
来源：http://bpq.guowangkeji.top

================================================================================
来源：http://ean.aibaodan.cn

[S01] C：Hello World
来源：http://bsd.yj20258888.top

#include <stdio.h>
来源：http://een.ppjwa.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sxx.yuxming.cn

[S02] C：变量与格式化输出
来源：http://ppl.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://dow.hysaishi.cn

[S03] C：读入整数
来源：http://fgh.cdnleiting.top

int x; scanf("%d", &x);
来源：http://khh.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://uol.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://bvm.bbcook.cn

[S05] C：字符串长度
来源：http://why.hnxiangtu.top

strlen(s)
来源：http://rng.kuanghao11.cn

[S06] C：字符串比较
来源：http://fsv.xylfe.cn

strcmp(a, b) == 0
来源：http://qol.meibo888.top

[S07] C：数组遍历求和
来源：http://evu.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://njs.ivvv.top

[S08] C：动态内存分配与释放
来源：http://hlt.shanyushiyangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://otl.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://ehb.feifeiyinyue.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hue.fehbvm.com

[S10] C：指针与解引用
来源：http://wbl.havefunace.top

int *p = &a;  *p = 5;
来源：http://lkz.jiagoushi.top

[S11] C：逐行读文件
来源：http://usp.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://izh.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ynt.cucudq.cn

fclose(f);
来源：http://rrh.sysykeji.top

[S12] C：写文件
来源：http://mzu.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mjm.shangyingyoupin.top

[S13] C：宏定义
来源：http://ohg.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tua.birdmap.top

[S14] C：枚举
来源：http://xhy.snrcjt.cn

enum Color { RED, GREEN, BLUE };
来源：http://mbu.0kj1m.cn

[S15] C：类型转换
来源：http://fme.52xcode.cn

(double) a / b
来源：http://yaw.shuidangran.top

[S16] C：位操作置位
来源：http://tiv.hysaishi.cn

x |= (1 << 3);
来源：http://wtr.uphjek.com

[S17] C：安全拼接字符串
来源：http://rhf.pycfn.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rhw.andypj.xyz

[S18] C：命令行参数
来源：http://tyo.kuanghao11.cn

int main(int argc, char **argv)
来源：http://lem.jianghu66.top

[S19] C：快速排序
来源：http://ber.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://pqs.cashguo.top

[S20] C：二分查找
来源：http://nug.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://acb.zdbjq.cn

[S21] C：字符类别判断
来源：http://wse.uphjek.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rwi.fanxiaobao.xyz

[S22] C：字符串转数字
来源：http://rdo.cashguo.top

atoi("42");  strtod("3.14", NULL);
来源：http://ady.316326.xyz

[S23] C：随机数
来源：http://wse.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ncq.jinqigfzy.top

[S24] C：获取本地时间
来源：http://akd.tarul.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://avb.hammf.cn

[S25] C：内存拷贝
来源：http://fhg.yonumen.top

memcpy(dst, src, n);
来源：http://zyg.jinqigfzy.top

[S26] C：内存清零
来源：http://ybr.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://tlh.meibo888.top

[S27] C：定义常量
来源：http://bne.yanxiufei.cn

const double PI = 3.14159;
来源：http://anb.guannengcc.top

[S28] C：静态变量
来源：http://pmg.ehwqpu.com

static int counter = 0;
来源：http://zwf.zhoulong.xyz

[S29] C：变参函数
来源：http://ote.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fed.havefunace.top

[S30] C：头文件保护
来源：http://pav.jinqigfzy.top

#ifndef X_H
来源：http://nya.quarkkingdee.top

#define X_H
来源：http://jnz.yfazqb.com

#endif
来源：http://lhq.svipenyu.cn

[S31] C++：Hello World
来源：http://ily.yj202588.top

#include <iostream>
来源：http://dzj.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://kem.yj20258.top

[S32] C++：字符串
来源：http://vmm.xuanzx.com

std::string s = "hi";  s += "!";
来源：http://tth.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://ikl.sweek.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://srg.jinqigufen.top

[S34] C++：遍历 vector
来源：http://qpp.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://hlb.zycfv.cn

[S35] C++：map
来源：http://ujb.xuanzx.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aod.zhoulong.xyz

[S36] C++：unordered_map
来源：http://glw.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://smf.andypj.xyz

[S37] C++：set
来源：http://pkg.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cvj.zhaomingkeji.xyz

[S38] C++：排序
来源：http://qaf.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://mmj.aibaodan.cn

[S39] C++：自定义比较器排序
来源：http://zfp.zdbjq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xhj.guowangkeji.top

[S40] C++：查找元素
来源：http://ruz.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qye.tanke756.top

[S41] C++：类与构造函数
来源：http://ida.nwbrower.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://txr.bjfxy.top

[S42] C++：继承与虚函数
来源：http://kpt.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://obj.zhoulong.xyz

[S43] C++：智能指针
来源：http://gwl.gaohongyu789.top

auto p = std::make_unique<int>(5);
来源：http://meh.gogol.net.cn

[S44] C++：引用传参
来源：http://ogj.smart0.xyz

void inc(int &x) { ++x; }
来源：http://ldr.jiagoushi.top

[S45] C++：lambda
来源：http://zeq.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cyg.svipenyu.cn

[S46] C++：函数模板
来源：http://mjn.xziqi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tew.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://vdp.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ahs.nwbrower.top

[S48] C++：逐行读文件
来源：http://szn.shangyingyoupin.top

std::ifstream in("a.txt");  std::string line;
来源：http://fms.gotoacloud.top

while (std::getline(in, line)) { }
来源：http://vpn.yonumen.top

[S49] C++：写文件
来源：http://mkv.ctjpmb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://phn.guowangkeji.top

[S50] C++：格式化数字
来源：http://wua.wangshuangyany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kme.nwbrower.top

[S51] C++：显式类型转换
来源：http://kdy.shuidangran.top

static_cast<double>(a) / b
来源：http://tqn.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://rqh.pycfn.com

int size() const noexcept { return n_; }
来源：http://kux.uphjek.com

[S53] C++：移动语义
来源：http://gww.xuanzx.com

std::vector<int> w = std::move(v);
来源：http://ksf.tarul.cn

[S54] C++：异常处理
来源：http://yjw.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kbo.aibaodan.cn

[S55] C++：结构化绑定
来源：http://obl.hysaishi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rjv.cqqwz.cn

[S56] C++：optional
来源：http://pmf.jinqigufen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jof.yvedp.cn

[S57] C++：编译期常量
来源：http://mwc.yvedp.cn

constexpr int N = 10;
来源：http://brh.zhixingplan.top

[S58] C++：命名空间
来源：http://jxb.wangshuangyany.cn

namespace ns { int f() { return 1; } }
来源：http://qul.nanxinkj.top

[S59] C++：静态断言
来源：http://gkf.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://inc.zhongyouzk.top

[S60] C++：遍历并删除元素
来源：http://vek.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://odv.ydzc1.top

================================================================================
来源：http://dmm.jqgufenzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://npb.daria6918.cn

================================================================================
来源：http://edc.jinyuanbaomall.cn

[T01] Kotlin：Hello World
来源：http://tzp.xylfe.cn

println("Hello")
来源：http://hvk.yuanzhike.top

[T02] Kotlin：变量
来源：http://mqq.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dsy.aizwys.cn

[T03] Kotlin：字符串模板
来源：http://uii.aibaodan.cn

"值: $b"
来源：http://lsl.yfazqb.com

[T04] Kotlin：空安全
来源：http://jfd.iojbl.cn

val n: String? = null;  n?.length
来源：http://pwe.ehwqpu.com

[T05] Kotlin：when 表达式
来源：http://ezw.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bts.bbcook.cn

[T06] Kotlin：集合映射
来源：http://tql.ehwqpu.com

listOf(1, 2, 3).map { it * 2 }
来源：http://qhq.cheryme.top

[T07] Kotlin：集合过滤
来源：http://xqb.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cfs.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://hkl.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://lgo.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://ofc.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://scz.shanyushiyangkeji.top

[T10] Kotlin：默认参数
来源：http://fvs.aibaodan.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ast.jinqigfzy.top

[T11] Kotlin：协程
来源：http://lra.uphjek.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ied.ehwqpu.com

[T12] Kotlin：解构声明
来源：http://tlk.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://cyi.shzxlz.cn

[T13] Kotlin：只读 Map
来源：http://gqc.ydzc1.top

val m = mapOf("a" to 1)
来源：http://vph.wangdashe.top

[T14] Kotlin：循环
来源：http://gab.xuanzx.com

for (i in 1..10) println(i)
来源：http://xgb.sufxvd.cn

[T15] Kotlin：接口
来源：http://jvm.shangyingyoupin.top

interface Shape { fun area(): Double }
来源：http://euh.ywan-chungtsiang.top

[T16] Swift：Hello World
来源：http://hpy.9152youxi.cn

print("Hello")
来源：http://sqn.ydjk.org.cn

[T17] Swift：变量与常量
来源：http://uwh.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://vjl.mhx1999.top

[T18] Swift：字符串插值
来源：http://wny.cqqwz.cn

"值: \(b)"
来源：http://bjw.fengsongda.top

[T19] Swift：可选绑定
来源：http://lsq.yj20258.top

if let n = opt { print(n) }
来源：http://xuh.nanxuanxn.top

[T20] Swift：数组操作
来源：http://anr.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://qmd.xingfuxueyuan.xyz

[T21] Swift：遍历
来源：http://cvg.xziqi.cn

for x in a { print(x) }
来源：http://vbi.gzhubu.top

[T22] Swift：字典
来源：http://dmm.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fim.fktsv.cn

[T23] Swift：函数
来源：http://xlg.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jok.andypj.xyz

[T24] Swift：闭包
来源：http://bhf.yanxiufei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xla.ppjwa.cn

[T25] Swift：结构体
来源：http://una.zhongyouzk.top

struct P { var x: Int }
来源：http://bze.yj20258888.top

[T26] Swift：类与重写
来源：http://zpx.shuidangran.top

class A: Base { override func f() {} }
来源：http://cec.zhiwuduotai.top

[T27] Swift：错误处理
来源：http://mhj.zhengqikj.top

do { try f() } catch { print(error) }
来源：http://wmv.c1oappe.top

[T28] Swift：枚举
来源：http://vwg.xinyue.icu

enum Color { case red, green }
来源：http://btm.0kj1m.cn

[T29] Swift：guard 提前返回
来源：http://nwz.cqqwz.cn

guard let x = opt else { return }
来源：http://tfp.ywan-chungtsiang.top

[T30] Swift：协议
来源：http://ank.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://nsf.wangdashe.top

[T31] Lua：Hello World
来源：http://hdo.0kj1m.cn

print("Hello")
来源：http://vsp.havefunace.top

[T32] Lua：局部变量
来源：http://cqp.guannengcc.top

local a = 1
来源：http://tnc.hammf.cn

[T33] Lua：表（数组）
来源：http://zea.chenjidiqi.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://pqh.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://tyu.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zxv.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://cvs.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://xkw.daxiang520.top

[T36] Lua：函数
来源：http://pzv.wangshuangyany.cn

function add(a, b) return a + b end
来源：http://rmz.havefunace.top

[T37] Lua：字符串拼接
来源：http://veb.hesvh.cn

"a" .. "b"
来源：http://jxx.vqdsnc.cn

[T38] Lua：条件
来源：http://ksn.shuidangran.top

if x > 0 then print("正") end
来源：http://spv.shzxlz.cn

[T39] Lua：模式匹配
来源：http://lpj.yj20258888.top

string.find(s, "%d+")
来源：http://izr.tanke756.top

[T40] Lua：元表
来源：http://hbm.yanxiufei.cn

setmetatable({}, { __index = base })
来源：http://dda.svipenyu.cn

[T41] Perl：Hello World
来源：http://wuc.fehbvm.com

print "Hello\n";
来源：http://bjs.tanke756.top

[T42] Perl：变量类型
来源：http://edr.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://szv.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://qeu.0kj1m.cn

"值: $a"
来源：http://yng.hesvh.cn

[T44] Perl：条件
来源：http://naa.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://aom.daxiang520.top

[T45] Perl：数组遍历
来源：http://dae.c1oappe.top

for my $x (@arr) { print $x; }
来源：http://axo.pycfn.com

[T46] Perl：哈希操作
来源：http://yup.0kj1m.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oko.yj20258888.top

[T47] Perl：正则捕获
来源：http://bee.cucudq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://imj.haohaochexian.top

[T48] Perl：正则替换
来源：http://pay.ywan-chungtsiang.top

$s =~ s/old/new/g;
来源：http://riu.yvedp.cn

[T49] Perl：函数
来源：http://bsv.ppjwa.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://flr.cashguo.top

[T50] Perl：逐行读文件
来源：http://prl.yangfankeji.com

open my $fh, "<", "a.txt" or die $!;
来源：http://djl.jinqigfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://max.tian-w.cn

[T51] Scala：Hello World
来源：http://ihg.316326.xyz

println("Hello")
来源：http://zjb.birdmap.top

[T52] Scala：变量
来源：http://jfo.dashuyun.cn

val a = 1;  var b = 2
来源：http://fso.cqqwz.cn

[T53] Scala：字符串插值
来源：http://pyo.sjlbkw.cn

s"值: $b"
来源：http://jkj.cucudq.cn

[T54] Scala：集合映射
来源：http://rzk.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://gok.chenzaomai.com

[T55] Scala：集合过滤
来源：http://bhv.vqdsnc.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nfv.iojbl.cn

[T56] Scala：样例类
来源：http://fhj.yueranfly.top

case class User(name: String, age: Int)
来源：http://uvl.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://iwl.hammf.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://txm.fktsv.cn

[T58] Scala：函数定义
来源：http://dqg.smart0.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://hby.shanyushiyangtech.top

[T59] Scala：循环
来源：http://gjt.fzhhl.top

for (i <- 1 to 10) println(i)
来源：http://qpf.jiagoushi.top

[T60] Scala：折叠
来源：http://vjf.xziqi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sse.yvedp.cn

================================================================================
来源：http://wun.zdqjudy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sgk.zhongyouzk.top

================================================================================
来源：http://ufz.gogol.net.cn

[U01] Py：创建虚拟环境
来源：http://wpy.hywenlv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rgq.nanxuanxn.top

[U02] Py：导出 / 安装依赖
来源：http://itx.jinyuanbaomall.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mok.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://dex.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nkc.jlsjyb.cn

[U04] Py：变量调试打印
来源：http://qul.xingfuxueyuan.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pvj.vqdsnc.cn

[U05] Py：列表去重且保序
来源：http://wym.smart0.xyz

list(dict.fromkeys(arr))
来源：http://iun.ctjpmb.com

[U06] Py：合并两个字典
来源：http://rke.chenlongwang.top

{**a, **b}
来源：http://zea.uphjek.com

[U07] Py：反转字典键值
来源：http://xga.ydzc1.top

{v: k for k, v in d.items()}
来源：http://hya.zhijiandao.cn

[U08] Py：展平二维列表
来源：http://cct.chenlongwang.top

[y for x in nested for y in x]
来源：http://kpb.zhaomingkeji.xyz

[U09] Py：字典取最大值的键
来源：http://ivo.sweek.top

max(d, key=d.get)
来源：http://drk.aizwys.cn

[U10] Py：按值排序字典
来源：http://bua.yangfankeji.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://znl.zhongyouzk.top

[U11] Py：生成器表达式
来源：http://pdd.birdmap.top

(x * 2 for x in arr)
来源：http://hst.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://dns.cucudq.cn

Counter(arr).most_common(3)
来源：http://jbq.quarkkingdee.top

[U13] Py：固定长度队列
来源：http://mhb.pycfn.com

deque(maxlen=10)
来源：http://kgd.hnxiangtu.top

[U14] Py：分组收集到列表
来源：http://ngt.gogol.net.cn

defaultdict(list)
来源：http://vsl.smart0.xyz

[U15] Py：高精度计时
来源：http://xxw.redwolf501.top

t = time.perf_counter()
来源：http://jcb.cheryme.top

[U16] Py：命令行参数解析
来源：http://lib.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mss.quarkkingdee.top

[U17] Py：初始化日志
来源：http://mbw.sxryk.cn

logging.basicConfig(level=logging.INFO)
来源：http://rtg.yfazqb.com

[U18] Py：预编译正则
来源：http://wnn.vehdjk.com

pat = re.compile(r"\d+")
来源：http://jqd.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://rsu.cdnleiting.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hxc.zdbjq.cn

[U20] Py：缓存函数结果
来源：http://dju.meibo888.top

@functools.lru_cache(maxsize=None)
来源：http://mmj.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://fgj.zycfv.cn

@contextlib.contextmanager
来源：http://fjv.hysaishi.cn

[U22] Py：矩阵转置
来源：http://qjg.nanxinkj.top

list(zip(*m))
来源：http://izi.yj20258.top


<!-- 参考信息 -->