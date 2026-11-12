代发 wailian999

int x; scanf("%d", &x);
来源：http://tcn.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://hkc.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yth.chenzaomai.com

[S05] C：字符串长度
来源：http://uch.birdmap.top

strlen(s)
来源：http://blz.pycfn.com

[S06] C：字符串比较
来源：http://fvb.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://ewq.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://apg.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vmq.gzhubu.top

[S08] C：动态内存分配与释放
来源：http://fqn.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nuj.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://hkb.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://amu.ivvv.top

[S10] C：指针与解引用
来源：http://jwa.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://tbk.guowangkeji.top

[S11] C：逐行读文件
来源：http://bdd.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://ley.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rtb.cdnleiting.top

fclose(f);
来源：http://fqo.jianghu66.top

[S12] C：写文件
来源：http://wth.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ltc.jqgufenzy.top

[S13] C：宏定义
来源：http://rfa.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ros.shanyushiyangkeji.top

[S14] C：枚举
来源：http://cwy.snrcjt.cn

enum Color { RED, GREEN, BLUE };
来源：http://lkj.fengsongda.top

[S15] C：类型转换
来源：http://ipe.wangshuangyany.cn

(double) a / b
来源：http://jjv.birdmap.top

[S16] C：位操作置位
来源：http://efw.zhijiandao.cn

x |= (1 << 3);
来源：http://cpq.hysaishi.cn

[S17] C：安全拼接字符串
来源：http://exs.gzhubu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xzu.316326.xyz

[S18] C：命令行参数
来源：http://lsn.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://yfq.sxryk.cn

[S19] C：快速排序
来源：http://oso.cucudq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://abs.316326.xyz

[S20] C：二分查找
来源：http://whv.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ncf.hysaishi.cn

[S21] C：字符类别判断
来源：http://dbm.shzxlz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mti.wangdashe.top

[S22] C：字符串转数字
来源：http://cof.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ity.hammf.cn

[S23] C：随机数
来源：http://mgq.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dfo.c1oappe.top

[S24] C：获取本地时间
来源：http://woo.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yzk.zdqjudy.top

[S25] C：内存拷贝
来源：http://hws.wangdashe.top

memcpy(dst, src, n);
来源：http://lnt.tanke756.top

[S26] C：内存清零
来源：http://mmv.jianghu66.top

memset(a, 0, sizeof a);
来源：http://oyn.ehwqpu.com

[S27] C：定义常量
来源：http://yjj.ctjpmb.com

const double PI = 3.14159;
来源：http://mdr.ctjpmb.com

[S28] C：静态变量
来源：http://bxl.iojbl.cn

static int counter = 0;
来源：http://srl.chenlongwang.top

[S29] C：变参函数
来源：http://snz.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hac.cdnleiting.top

[S30] C：头文件保护
来源：http://jva.daxiang520.top

#ifndef X_H
来源：http://pej.zhaomingkeji.xyz

#define X_H
来源：http://jrt.hfpthk.cn

#endif
来源：http://kpq.ivvv.top

[S31] C++：Hello World
来源：http://yzq.nwbrower.top

#include <iostream>
来源：http://cds.pycfn.com

int main() { std::cout << "Hello\n"; }
来源：http://skj.fanxiaobao.xyz

[S32] C++：字符串
来源：http://npd.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://upc.jinqigufen.top

[S33] C++：vector 增删
来源：http://sso.dashuyun.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://spb.fktsv.cn

[S34] C++：遍历 vector
来源：http://fiq.zdqjudy.top

for (auto &x : v) { std::cout << x; }
来源：http://zkh.xziqi.cn

[S35] C++：map
来源：http://yys.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xsf.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://gsl.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mwo.52xcode.cn

[S37] C++：set
来源：http://gdb.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tai.kuanghao11.cn

[S38] C++：排序
来源：http://fjc.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://weg.yonumen.top

[S39] C++：自定义比较器排序
来源：http://mdn.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://grs.tian-w.cn

[S40] C++：查找元素
来源：http://eob.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mob.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://bge.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kxn.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://qwy.ywan-chungtsiang.top

class B : public Base { public: void f() override {} };
来源：http://cro.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://das.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://azo.sxryk.cn

[S44] C++：引用传参
来源：http://aen.xinyue.icu

void inc(int &x) { ++x; }
来源：http://grg.bjfxy.top

[S45] C++：lambda
来源：http://upw.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zgl.hongshengwenyu.top

[S46] C++：函数模板
来源：http://djp.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://krn.cucudq.cn

[S47] C++：结构化绑定遍历
来源：http://psn.shanyushiyangtech.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bvd.gotoacloud.top

[S48] C++：逐行读文件
来源：http://rqj.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://rhg.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://awo.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://fwm.xinyue.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dzm.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://ffi.hcnkem.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rna.ybcxt.top

[S51] C++：显式类型转换
来源：http://xtr.bbcook.cn

static_cast<double>(a) / b
来源：http://pwx.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://ouw.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://rlw.chenlongwang.top

[S53] C++：移动语义
来源：http://rtr.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://orq.jinqigufen.top

[S54] C++：异常处理
来源：http://zdv.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://otz.hnqzz.top

[S55] C++：结构化绑定
来源：http://jlx.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ixw.ivvv.top

[S56] C++：optional
来源：http://ncl.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://brb.gzhubu.top

[S57] C++：编译期常量
来源：http://rpr.fanxiaobao.xyz

constexpr int N = 10;
来源：http://fay.yangfankeji.com

[S58] C++：命名空间
来源：http://pos.yueranfly.top

namespace ns { int f() { return 1; } }
来源：http://qeu.ybcxt.top

[S59] C++：静态断言
来源：http://dlm.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cez.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://btr.hammf.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mjl.xuetiantiany.cn

================================================================================
来源：http://pwl.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xid.feifeiyinyue.top

================================================================================
来源：http://jkx.tarul.cn

[T01] Kotlin：Hello World
来源：http://hlf.pycfn.com

println("Hello")
来源：http://eql.jiagoushi.top

[T02] Kotlin：变量
来源：http://spl.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dpp.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://rli.316326.xyz

"值: $b"
来源：http://czn.zhiwuduotai.top

[T04] Kotlin：空安全
来源：http://juf.ctjpmb.com

val n: String? = null;  n?.length
来源：http://hef.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://dgx.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uqt.tarul.cn

[T06] Kotlin：集合映射
来源：http://dwa.ivvv.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jtz.fktsv.cn

[T07] Kotlin：集合过滤
来源：http://uxa.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ahz.chenzaomai.com

[T08] Kotlin：数据类
来源：http://yja.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://rur.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://wnv.cheryme.top

fun String.exclaim() = this + "!"
来源：http://zcd.cdnleiting.top

[T10] Kotlin：默认参数
来源：http://byf.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ozr.ehwqpu.com

[T11] Kotlin：协程
来源：http://din.zhijiandao.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uzc.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://key.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://amb.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://mic.zhoulong.xyz

val m = mapOf("a" to 1)
来源：http://hzg.xingfuxueyuan.xyz

[T14] Kotlin：循环
来源：http://wke.xinyue.icu

for (i in 1..10) println(i)
来源：http://ooh.shangyingyoupin.top

[T15] Kotlin：接口
来源：http://lnn.yonumen.top

interface Shape { fun area(): Double }
来源：http://ehe.jiagoushi.top

[T16] Swift：Hello World
来源：http://xdm.nanxinkj.top

print("Hello")
来源：http://vgn.vqdsnc.cn

[T17] Swift：变量与常量
来源：http://kxq.chenlongwang.top

var a = 1;  let b = 2
来源：http://nve.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://eue.yj202588.top

"值: \(b)"
来源：http://fth.snrcjt.cn

[T19] Swift：可选绑定
来源：http://uwc.hnqzz.top

if let n = opt { print(n) }
来源：http://jqk.hfpthk.cn

[T20] Swift：数组操作
来源：http://ozv.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bie.bbcook.cn

[T21] Swift：遍历
来源：http://koo.fktsv.cn

for x in a { print(x) }
来源：http://sgi.sjlbkw.cn

[T22] Swift：字典
来源：http://ppf.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://clh.yj202588.top

[T23] Swift：函数
来源：http://znz.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fgj.iojbl.cn

[T24] Swift：闭包
来源：http://gub.tian-w.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ssv.guannengcc.top

[T25] Swift：结构体
来源：http://ndt.zhongyouzk.top

struct P { var x: Int }
来源：http://zay.sweek.top

[T26] Swift：类与重写
来源：http://sjy.cashguo.top

class A: Base { override func f() {} }
来源：http://hye.bbcook.cn

[T27] Swift：错误处理
来源：http://jvn.yfazqb.com

do { try f() } catch { print(error) }
来源：http://mea.jianghu66.top

[T28] Swift：枚举
来源：http://yfv.ywan-chungtsiang.top

enum Color { case red, green }
来源：http://hca.yj20258.top

[T29] Swift：guard 提前返回
来源：http://vnf.cucudq.cn

guard let x = opt else { return }
来源：http://tzt.jlsjyb.cn

[T30] Swift：协议
来源：http://lvq.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://odg.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://mrd.yj20258888.top

print("Hello")
来源：http://ubv.bjfxy.top

[T32] Lua：局部变量
来源：http://pya.kuanghao11.cn

local a = 1
来源：http://aev.hywenlv.cn

[T33] Lua：表（数组）
来源：http://qkd.jinqigufen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://clc.fktsv.cn

[T34] Lua：遍历表
来源：http://pfy.yj202588.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jhu.sjlbkw.cn

[T35] Lua：字典表
来源：http://eoq.sxryk.cn

local d = { a = 1 };  d.b = 2
来源：http://ems.jianghu66.top

[T36] Lua：函数
来源：http://icx.sufxvd.cn

function add(a, b) return a + b end
来源：http://xhw.chenlongwang.top

[T37] Lua：字符串拼接
来源：http://mql.zhiwuduotai.top

"a" .. "b"
来源：http://urw.nanxinkj.top

[T38] Lua：条件
来源：http://jab.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://rmv.yj202588.top

[T39] Lua：模式匹配
来源：http://cgu.shuidangran.top

string.find(s, "%d+")
来源：http://okx.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://usm.smart0.xyz

setmetatable({}, { __index = base })
来源：http://one.yfazqb.com

[T41] Perl：Hello World
来源：http://lgj.hnxiangtu.top

print "Hello\n";
来源：http://iqj.hnxiangtu.top

[T42] Perl：变量类型
来源：http://jth.xuanzx.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cgj.shuidangran.top

[T43] Perl：字符串插值
来源：http://chs.zdbjq.cn

"值: $a"
来源：http://ojl.cdnleiting.top

[T44] Perl：条件
来源：http://ham.yj202588.top

if ($a > 0) { print "正"; }
来源：http://qmf.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://uis.hfpthk.cn

for my $x (@arr) { print $x; }
来源：http://tvv.yj202588.top

[T46] Perl：哈希操作
来源：http://crr.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gji.bbcook.cn

[T47] Perl：正则捕获
来源：http://ztd.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wnw.hesvh.cn

[T48] Perl：正则替换
来源：http://mtj.ywan-chungtsiang.top

$s =~ s/old/new/g;
来源：http://rsv.havefunace.top

[T49] Perl：函数
来源：http://yuz.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ejq.zhijiandao.cn

[T50] Perl：逐行读文件
来源：http://hpb.nanxinkj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ewb.fengsongda.top

while (my $line = <$fh>) { print $line; }
来源：http://pgd.52xcode.cn

[T51] Scala：Hello World
来源：http://sel.shangyingyoupin.top

println("Hello")
来源：http://kvc.zhoulong.xyz

[T52] Scala：变量
来源：http://srf.ppjwa.cn

val a = 1;  var b = 2
来源：http://oqq.9152youxi.cn

[T53] Scala：字符串插值
来源：http://acb.shangyingyoupin.top

s"值: $b"
来源：http://mkt.xingfuxueyuan.xyz

[T54] Scala：集合映射
来源：http://yfi.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://kau.daria6918.cn

[T55] Scala：集合过滤
来源：http://tiq.316326.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://see.meibo888.top

[T56] Scala：样例类
来源：http://ery.gotoacloud.top

case class User(name: String, age: Int)
来源：http://fsj.jinyuanbaomall.cn

[T57] Scala：模式匹配
来源：http://wfn.pycfn.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://qat.daxiang520.top

[T58] Scala：函数定义
来源：http://jxb.shanyushiyangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://trv.zhixingplan.top

[T59] Scala：循环
来源：http://owy.snrcjt.cn

for (i <- 1 to 10) println(i)
来源：http://dxm.sjlbkw.cn

[T60] Scala：折叠
来源：http://bae.yfazqb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qbv.vehdjk.com

================================================================================
来源：http://wta.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ajb.zdbjq.cn

================================================================================
来源：http://acy.cqqwz.cn

[U01] Py：创建虚拟环境
来源：http://icq.yj202588.top

python -m venv .venv && source .venv/bin/activate
来源：http://evb.nanxuanxn.top

[U02] Py：导出 / 安装依赖
来源：http://qqg.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tbf.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://ydb.ydjk.org.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rwm.ydjk.org.cn

[U04] Py：变量调试打印
来源：http://wce.zhiwuduotai.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zuf.epnwcf.com

[U05] Py：列表去重且保序
来源：http://nbg.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://ext.yongpay.top

[U06] Py：合并两个字典
来源：http://lkv.shuidangran.top

{**a, **b}
来源：http://prl.gotoacloud.top

[U07] Py：反转字典键值
来源：http://zuw.feifeiyinyue.top

{v: k for k, v in d.items()}
来源：http://zwl.aizwys.cn

[U08] Py：展平二维列表
来源：http://vsr.uphjek.com

[y for x in nested for y in x]
来源：http://afb.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://xvz.jyoumei.cn

max(d, key=d.get)
来源：http://nfs.bjfxy.top

[U10] Py：按值排序字典
来源：http://rdl.tarul.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ive.zhijiandao.cn

[U11] Py：生成器表达式
来源：http://eli.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://ttz.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://zqc.nanxinkj.top

Counter(arr).most_common(3)
来源：http://nbz.9152youxi.cn

[U13] Py：固定长度队列
来源：http://akk.quarkkingdee.top

deque(maxlen=10)
来源：http://qda.316326.xyz

[U14] Py：分组收集到列表
来源：http://hwi.gotoacloud.top

defaultdict(list)
来源：http://ons.ybcxt.top

[U15] Py：高精度计时
来源：http://jjo.hesvh.cn

t = time.perf_counter()
来源：http://bez.ydzc1.top

[U16] Py：命令行参数解析
来源：http://kmc.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tvh.zdbjq.cn

[U17] Py：初始化日志
来源：http://dth.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://tgy.ivvv.top

[U18] Py：预编译正则
来源：http://bou.9152youxi.cn

pat = re.compile(r"\d+")
来源：http://crb.gogol.net.cn

[U19] Py：正则替换带回调
来源：http://fit.shzxlz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nbo.daria6918.cn

[U20] Py：缓存函数结果
来源：http://yan.52xcode.cn

@functools.lru_cache(maxsize=None)
来源：http://ufb.zhaomingkeji.xyz

[U21] Py：自定义上下文管理器
来源：http://rnn.zhijiandao.cn

@contextlib.contextmanager
来源：http://nwe.iojbl.cn

[U22] Py：矩阵转置
来源：http://ybk.tianlin.xyz

list(zip(*m))
来源：http://tky.zhaomingkeji.xyz

[U23] Py：分块读取大文件
来源：http://ntp.daria6918.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eds.shangyingyoupin.top

[U24] Py：路径操作
来源：http://mjh.shangyingyoupin.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tbj.zycfv.cn

[U25] Py：CSV 按字典读
来源：http://kla.hywenlv.cn

csv.DictReader(f)
来源：http://wxs.xinyue.icu

[U26] Py：并发下载
来源：http://utq.nanxuanxn.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fhs.vqdsnc.cn


<!-- 参考信息 -->