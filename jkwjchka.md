代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://gwu.epnwcf.com

[S02] C：变量与格式化输出
来源：http://ces.xziqi.cn

int a = 10; printf("%d\n", a);
来源：http://wpx.shanyushiyangtech.top

[S03] C：读入整数
来源：http://fgm.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://mom.tian-w.cn

[S04] C：字符串复制
来源：http://ggn.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://vlm.vehdjk.com

[S05] C：字符串长度
来源：http://rqe.ywan-chungtsiang.top

strlen(s)
来源：http://upe.hesvh.cn

[S06] C：字符串比较
来源：http://rdr.ctjpmb.com

strcmp(a, b) == 0
来源：http://spj.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://htg.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nma.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://skc.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ott.yonumen.top

[S09] C：结构体定义与初始化
来源：http://zmo.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://unz.gaohongyu789.top

[S10] C：指针与解引用
来源：http://sln.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://puy.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://tcu.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://wbi.uphjek.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://gep.sxryk.cn

fclose(f);
来源：http://sqd.c1oappe.top

[S12] C：写文件
来源：http://rmq.cdnleiting.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zom.316326.xyz

[S13] C：宏定义
来源：http://qte.guowangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qsu.sxryk.cn

[S14] C：枚举
来源：http://fft.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://wjk.redwolf501.top

[S15] C：类型转换
来源：http://tjj.gaohongyu789.top

(double) a / b
来源：http://zze.hesvh.cn

[S16] C：位操作置位
来源：http://gyf.cashguo.top

x |= (1 << 3);
来源：http://gon.sweek.top

[S17] C：安全拼接字符串
来源：http://tfw.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jlt.jiagoushi.top

[S18] C：命令行参数
来源：http://sjj.ivvv.top

int main(int argc, char **argv)
来源：http://ynm.sysykeji.top

[S19] C：快速排序
来源：http://sks.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ycc.zdbjq.cn

[S20] C：二分查找
来源：http://xor.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vnt.chenzaomai.com

[S21] C：字符类别判断
来源：http://ryq.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nch.aibaodan.cn

[S22] C：字符串转数字
来源：http://fab.c1oappe.top

atoi("42");  strtod("3.14", NULL);
来源：http://mfp.ywan-chungtsiang.top

[S23] C：随机数
来源：http://wof.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://epp.9152youxi.cn

[S24] C：获取本地时间
来源：http://iog.aizwys.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nsb.yueranfly.top

[S25] C：内存拷贝
来源：http://mac.ppjwa.cn

memcpy(dst, src, n);
来源：http://qae.yj202588.top

[S26] C：内存清零
来源：http://hhy.dianchejie.cn

memset(a, 0, sizeof a);
来源：http://cgt.quarkkingdee.top

[S27] C：定义常量
来源：http://fpn.gaohongyu789.top

const double PI = 3.14159;
来源：http://dad.sufxvd.cn

[S28] C：静态变量
来源：http://tww.nwbrower.top

static int counter = 0;
来源：http://lsb.hnxiangtu.top

[S29] C：变参函数
来源：http://tck.hysaishi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mjs.xuetiantiany.cn

[S30] C：头文件保护
来源：http://yjn.jinqigufen.top

#ifndef X_H
来源：http://ysu.ywan-chungtsiang.top

#define X_H
来源：http://uce.dianchejie.cn

#endif
来源：http://ghn.nanxinkj.top

[S31] C++：Hello World
来源：http://jpl.yuanzhike.top

#include <iostream>
来源：http://ghy.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://srh.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://rqc.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://izb.bbcook.cn

[S33] C++：vector 增删
来源：http://ndb.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lxi.aibaodan.cn

[S34] C++：遍历 vector
来源：http://udb.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://yns.wangshuangyany.cn

[S35] C++：map
来源：http://icz.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qre.52xcode.cn

[S36] C++：unordered_map
来源：http://cmz.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jwk.haohaochexian.top

[S37] C++：set
来源：http://pax.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xgs.c1oappe.top

[S38] C++：排序
来源：http://eyt.tanke756.top

std::sort(v.begin(), v.end());
来源：http://phh.yj20258.top

[S39] C++：自定义比较器排序
来源：http://ncq.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zsd.yj202588.top

[S40] C++：查找元素
来源：http://xxy.cashguo.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://agt.zhixingplan.top

[S41] C++：类与构造函数
来源：http://umk.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://stn.feifeiyinyue.top

[S42] C++：继承与虚函数
来源：http://ttx.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://xtj.zdqjudy.top

[S43] C++：智能指针
来源：http://dvs.ivvv.top

auto p = std::make_unique<int>(5);
来源：http://gjy.redwolf501.top

[S44] C++：引用传参
来源：http://yuc.meibo888.top

void inc(int &x) { ++x; }
来源：http://ldd.feifeiyinyue.top

[S45] C++：lambda
来源：http://ayj.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://dun.ehwqpu.com

[S46] C++：函数模板
来源：http://ynr.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://idz.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://kmp.ctjpmb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pll.jiagoushi.top

[S48] C++：逐行读文件
来源：http://emw.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://unu.shanyushiyangtech.top

while (std::getline(in, line)) { }
来源：http://zhg.cucudq.cn

[S49] C++：写文件
来源：http://ehl.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ofa.yueranfly.top

[S50] C++：格式化数字
来源：http://wmr.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cza.cheryme.top

[S51] C++：显式类型转换
来源：http://utl.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://waf.kuanghao11.cn

[S52] C++：const 与 noexcept
来源：http://wri.hesvh.cn

int size() const noexcept { return n_; }
来源：http://cme.iojbl.cn

[S53] C++：移动语义
来源：http://wqt.cheryme.top

std::vector<int> w = std::move(v);
来源：http://lia.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://oix.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jgm.bjfxy.top

[S55] C++：结构化绑定
来源：http://fjl.pycfn.com

auto [a, b] = std::make_pair(1, 2);
来源：http://sdp.zdbjq.cn

[S56] C++：optional
来源：http://ypy.sweek.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lpx.uphjek.com

[S57] C++：编译期常量
来源：http://ing.aizwys.cn

constexpr int N = 10;
来源：http://vhp.andypj.xyz

[S58] C++：命名空间
来源：http://cnz.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://hcs.jqgufenzy.top

[S59] C++：静态断言
来源：http://efq.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sow.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://csc.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gdf.xinyue.icu

================================================================================
来源：http://leq.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eck.ivvv.top

================================================================================
来源：http://bjt.hnqzz.top

[T01] Kotlin：Hello World
来源：http://auk.52xcode.cn

println("Hello")
来源：http://mgl.vehdjk.com

[T02] Kotlin：变量
来源：http://nbk.fengsongda.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yyg.snrcjt.cn

[T03] Kotlin：字符串模板
来源：http://wqe.sweek.top

"值: $b"
来源：http://oru.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://fnh.wangshuangyany.cn

val n: String? = null;  n?.length
来源：http://bce.cashguo.top

[T05] Kotlin：when 表达式
来源：http://siv.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vwz.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://ncr.zhaomingkeji.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://suy.tarul.cn

[T07] Kotlin：集合过滤
来源：http://duh.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://oya.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://nad.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://wsq.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://rxm.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://ffa.guowangkeji.top

[T10] Kotlin：默认参数
来源：http://lge.cucudq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zcq.meibo888.top

[T11] Kotlin：协程
来源：http://gye.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qub.sweek.top

[T12] Kotlin：解构声明
来源：http://zzl.sweek.top

val (a, b) = Pair(1, 2)
来源：http://rnt.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://sab.xylfe.cn

val m = mapOf("a" to 1)
来源：http://hnm.dashuyun.cn

[T14] Kotlin：循环
来源：http://vpc.jqgufenzy.top

for (i in 1..10) println(i)
来源：http://iiq.wangdashe.top

[T15] Kotlin：接口
来源：http://lkj.zhoulong.xyz

interface Shape { fun area(): Double }
来源：http://efa.nanxinkj.top

[T16] Swift：Hello World
来源：http://beo.aizwys.cn

print("Hello")
来源：http://qfc.sxryk.cn

[T17] Swift：变量与常量
来源：http://scc.bbcook.cn

var a = 1;  let b = 2
来源：http://gbg.aibaodan.cn

[T18] Swift：字符串插值
来源：http://kzc.tanke756.top

"值: \(b)"
来源：http://nwv.0kj1m.cn

[T19] Swift：可选绑定
来源：http://nzg.yongpay.top

if let n = opt { print(n) }
来源：http://ogq.316326.xyz

[T20] Swift：数组操作
来源：http://woi.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://clg.havefunace.top

[T21] Swift：遍历
来源：http://bdr.xuetiantiany.cn

for x in a { print(x) }
来源：http://abu.pengpengdd.cyou

[T22] Swift：字典
来源：http://dcv.aibaodan.cn

var d = ["a": 1];  d["b"] = 2
来源：http://akd.cqqwz.cn

[T23] Swift：函数
来源：http://keq.jiagoushi.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cpb.yfazqb.com

[T24] Swift：闭包
来源：http://rzo.andypj.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://okl.hcnkem.com

[T25] Swift：结构体
来源：http://luq.c1oappe.top

struct P { var x: Int }
来源：http://yaf.xziqi.cn

[T26] Swift：类与重写
来源：http://nme.iojbl.cn

class A: Base { override func f() {} }
来源：http://ajv.sysykeji.top

[T27] Swift：错误处理
来源：http://yyo.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://ltz.uphjek.com

[T28] Swift：枚举
来源：http://prk.zhongyouzk.top

enum Color { case red, green }
来源：http://kkh.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://eut.tarul.cn

guard let x = opt else { return }
来源：http://hbi.fengsongda.top

[T30] Swift：协议
来源：http://yta.epnwcf.com

protocol Shape { func area() -> Double }
来源：http://hty.zhixingplan.top

[T31] Lua：Hello World
来源：http://qwh.hongshengwenyu.top

print("Hello")
来源：http://zzs.shanyushiyangkeji.top

[T32] Lua：局部变量
来源：http://gdt.daria6918.cn

local a = 1
来源：http://cmb.shanyushiyangtech.top

[T33] Lua：表（数组）
来源：http://vcx.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mzi.jinyuanbaomall.cn

[T34] Lua：遍历表
来源：http://whd.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://aki.hnqzz.top

[T35] Lua：字典表
来源：http://rja.hfpthk.cn

local d = { a = 1 };  d.b = 2
来源：http://vze.guannengcc.top

[T36] Lua：函数
来源：http://qok.shuidangran.top

function add(a, b) return a + b end
来源：http://xlr.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://zxo.0kj1m.cn

"a" .. "b"
来源：http://bmi.52xcode.cn

[T38] Lua：条件
来源：http://yhg.hongshengwenyu.top

if x > 0 then print("正") end
来源：http://xkf.sxryk.cn

[T39] Lua：模式匹配
来源：http://bqh.daxiang520.top

string.find(s, "%d+")
来源：http://mas.zdqjudy.top

[T40] Lua：元表
来源：http://jwm.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://yht.dashuyun.cn

[T41] Perl：Hello World
来源：http://zux.sysykeji.top

print "Hello\n";
来源：http://zwk.zhongyouzk.top

[T42] Perl：变量类型
来源：http://cqp.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nfv.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://dlw.jinqigufen.top

"值: $a"
来源：http://smi.zdbjq.cn

[T44] Perl：条件
来源：http://bdg.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://smm.tarul.cn

[T45] Perl：数组遍历
来源：http://xrh.pengpengdd.cyou

for my $x (@arr) { print $x; }
来源：http://vfx.daxiang520.top

[T46] Perl：哈希操作
来源：http://dge.redwolf501.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gsa.vehdjk.com

[T47] Perl：正则捕获
来源：http://ifl.gzhubu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://eus.cashguo.top

[T48] Perl：正则替换
来源：http://vkn.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://pfi.mhx1999.top

[T49] Perl：函数
来源：http://trm.ivvv.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tlo.vehdjk.com

[T50] Perl：逐行读文件
来源：http://lvn.fengsongda.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zcl.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://fai.ppjwa.cn

[T51] Scala：Hello World
来源：http://slf.vqdsnc.cn

println("Hello")
来源：http://kum.xylfe.cn

[T52] Scala：变量
来源：http://ico.epnwcf.com

val a = 1;  var b = 2
来源：http://bfw.chenlongwang.top

[T53] Scala：字符串插值
来源：http://ifb.redwolf501.top

s"值: $b"
来源：http://oyz.jiagoushi.top

[T54] Scala：集合映射
来源：http://nkd.jqgufenzy.top

List(1, 2, 3).map(_ * 2)
来源：http://ytw.nanxinkj.top

[T55] Scala：集合过滤
来源：http://lvb.wangshuangyany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://glj.cucudq.cn

[T56] Scala：样例类
来源：http://jty.fehbvm.com

case class User(name: String, age: Int)
来源：http://rkh.sysykeji.top

[T57] Scala：模式匹配
来源：http://jtx.xingfuxueyuan.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://khh.nanxuanxn.top

[T58] Scala：函数定义
来源：http://ynr.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://urh.0kj1m.cn

[T59] Scala：循环
来源：http://jbe.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://arn.cqqwz.cn

[T60] Scala：折叠
来源：http://dfv.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vyn.jqgfzy.top

================================================================================
来源：http://gsq.shuidangran.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://spg.zdbjq.cn

================================================================================
来源：http://gvn.tianlin.xyz

[U01] Py：创建虚拟环境
来源：http://pyr.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pen.52xcode.cn

[U02] Py：导出 / 安装依赖
来源：http://myf.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rpn.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://jii.dianchejie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://paj.sxryk.cn

[U04] Py：变量调试打印
来源：http://yvd.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nlb.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://lzp.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://qor.aibaodan.cn

[U06] Py：合并两个字典
来源：http://kre.ybcxt.top

{**a, **b}
来源：http://wsp.bjfxy.top

[U07] Py：反转字典键值
来源：http://fpj.uphjek.com

{v: k for k, v in d.items()}
来源：http://dwk.iojbl.cn

[U08] Py：展平二维列表
来源：http://kuw.jianghu66.top

[y for x in nested for y in x]
来源：http://qwp.pycfn.com

[U09] Py：字典取最大值的键
来源：http://jpe.chenlongwang.top

max(d, key=d.get)
来源：http://wuq.dashuyun.cn

[U10] Py：按值排序字典
来源：http://alb.jinghuilouyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qyh.shzxlz.cn

[U11] Py：生成器表达式
来源：http://cve.cashguo.top

(x * 2 for x in arr)
来源：http://dfd.yangfankeji.com

[U12] Py：取出现最多的 3 个元素
来源：http://yzn.chenzaomai.com

Counter(arr).most_common(3)
来源：http://ztd.fengsongda.top

[U13] Py：固定长度队列
来源：http://hjc.gzhubu.top

deque(maxlen=10)
来源：http://uhg.nanxinkj.top

[U14] Py：分组收集到列表
来源：http://wjn.jinqigufen.top

defaultdict(list)
来源：http://rca.redwolf501.top

[U15] Py：高精度计时
来源：http://iuj.vqdsnc.cn

t = time.perf_counter()
来源：http://fub.zhoulong.xyz

[U16] Py：命令行参数解析
来源：http://hps.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fjb.hammf.cn

[U17] Py：初始化日志
来源：http://kbz.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://vwt.svipenyu.cn

[U18] Py：预编译正则
来源：http://glq.jianghu66.top

pat = re.compile(r"\d+")
来源：http://tkb.tian-w.cn

[U19] Py：正则替换带回调
来源：http://wzc.316326.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://akp.316326.xyz

[U20] Py：缓存函数结果
来源：http://led.hywenlv.cn

@functools.lru_cache(maxsize=None)
来源：http://xpj.zhengqikj.top

[U21] Py：自定义上下文管理器
来源：http://azs.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://tbr.0kj1m.cn

[U22] Py：矩阵转置
来源：http://vci.epnwcf.com

list(zip(*m))
来源：http://jys.hesvh.cn

[U23] Py：分块读取大文件
来源：http://kdl.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cph.birdmap.top

[U24] Py：路径操作
来源：http://azc.hcnkem.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pwt.ehwqpu.com


<!-- 参考信息 -->