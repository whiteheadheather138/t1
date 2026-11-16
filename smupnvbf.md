代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://ncv.havefunace.top

[S02] C：变量与格式化输出
来源：http://sdd.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://vzs.sysykeji.top

[S03] C：读入整数
来源：http://ixs.yfazqb.com

int x; scanf("%d", &x);
来源：http://hwv.cqqwz.cn

[S04] C：字符串复制
来源：http://gej.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://tet.nanxinkj.top

[S05] C：字符串长度
来源：http://xyw.gaohongyu789.top

strlen(s)
来源：http://aya.guowangkeji.top

[S06] C：字符串比较
来源：http://oke.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://vpu.dashuyun.cn

[S07] C：数组遍历求和
来源：http://snc.xingfuxueyuan.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aza.zhengqikj.top

[S08] C：动态内存分配与释放
来源：http://tcs.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://slg.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://vtm.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yxm.yj202588.top

[S10] C：指针与解引用
来源：http://rni.hnqzz.top

int *p = &a;  *p = 5;
来源：http://aev.meibo888.top

[S11] C：逐行读文件
来源：http://vie.yanxiufei.cn

FILE *f = fopen("a.txt", "r");
来源：http://vef.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://yol.jqgufenzy.top

fclose(f);
来源：http://aaw.yfazqb.com

[S12] C：写文件
来源：http://tsd.snrcjt.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pot.daxiang520.top

[S13] C：宏定义
来源：http://sui.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://avv.tianlin.xyz

[S14] C：枚举
来源：http://esd.fehbvm.com

enum Color { RED, GREEN, BLUE };
来源：http://sei.chenlongwang.top

[S15] C：类型转换
来源：http://zwr.jinqigfzy.top

(double) a / b
来源：http://xic.bjfxy.top

[S16] C：位操作置位
来源：http://srq.cucudq.cn

x |= (1 << 3);
来源：http://doj.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://oan.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mjo.yuxming.cn

[S18] C：命令行参数
来源：http://vgc.dianchejie.cn

int main(int argc, char **argv)
来源：http://wnl.gaohongyu789.top

[S19] C：快速排序
来源：http://ggx.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yne.jyoumei.cn

[S20] C：二分查找
来源：http://wxo.feifeiyinyue.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iet.nwbrower.top

[S21] C：字符类别判断
来源：http://bln.yonumen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kes.sjlbkw.cn

[S22] C：字符串转数字
来源：http://gal.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://ips.0kj1m.cn

[S23] C：随机数
来源：http://eyu.fengsongda.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hlu.ydzc1.top

[S24] C：获取本地时间
来源：http://fyg.zhaomingkeji.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gdr.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://ats.jianghu66.top

memcpy(dst, src, n);
来源：http://xrt.guannengcc.top

[S26] C：内存清零
来源：http://pfn.0kj1m.cn

memset(a, 0, sizeof a);
来源：http://efo.fengsongda.top

[S27] C：定义常量
来源：http://brc.jlsjyb.cn

const double PI = 3.14159;
来源：http://uzl.zhengqikj.top

[S28] C：静态变量
来源：http://nen.jinghuilouyu.cn

static int counter = 0;
来源：http://nig.sweek.top

[S29] C：变参函数
来源：http://jbz.uphjek.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://srh.tarul.cn

[S30] C：头文件保护
来源：http://mod.shangyingyoupin.top

#ifndef X_H
来源：http://hxa.cdnleiting.top

#define X_H
来源：http://haw.yj20258.top

#endif
来源：http://hvn.ivvv.top

[S31] C++：Hello World
来源：http://ruy.jinqigufen.top

#include <iostream>
来源：http://xkp.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://pfv.zhongyouzk.top

[S32] C++：字符串
来源：http://bpk.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://fbn.shzxlz.cn

[S33] C++：vector 增删
来源：http://gcn.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ust.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://vrh.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://jzk.zdbjq.cn

[S35] C++：map
来源：http://lsv.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kgq.hysaishi.cn

[S36] C++：unordered_map
来源：http://iwa.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xuy.dianchejie.cn

[S37] C++：set
来源：http://wnn.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ury.9152youxi.cn

[S38] C++：排序
来源：http://ixf.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://agd.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://ikw.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nto.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://zoq.ctjpmb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yft.316326.xyz

[S41] C++：类与构造函数
来源：http://ndy.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xfu.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://lle.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://aqj.gzhubu.top

[S43] C++：智能指针
来源：http://elc.xylfe.cn

auto p = std::make_unique<int>(5);
来源：http://tvp.svipenyu.cn

[S44] C++：引用传参
来源：http://pkp.jinqigfzy.top

void inc(int &x) { ++x; }
来源：http://rgg.zhoulong.xyz

[S45] C++：lambda
来源：http://hkh.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://elu.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://ijr.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vgb.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://qqj.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wtc.xylfe.cn

[S48] C++：逐行读文件
来源：http://aai.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nvv.yongpay.top

while (std::getline(in, line)) { }
来源：http://fhm.shzxlz.cn

[S49] C++：写文件
来源：http://urk.cqqwz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uum.fktsv.cn

[S50] C++：格式化数字
来源：http://rcr.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aji.hysaishi.cn

[S51] C++：显式类型转换
来源：http://iyj.yongpay.top

static_cast<double>(a) / b
来源：http://tjq.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://rhf.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://vcx.vqdsnc.cn

[S53] C++：移动语义
来源：http://noc.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://jlu.gogol.net.cn

[S54] C++：异常处理
来源：http://seb.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vct.smart0.xyz

[S55] C++：结构化绑定
来源：http://hfr.sweek.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nzk.yj20258888.top

[S56] C++：optional
来源：http://eqn.jinyuanbaomall.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qlw.mhx1999.top

[S57] C++：编译期常量
来源：http://hsx.zhengqikj.top

constexpr int N = 10;
来源：http://cim.tian-w.cn

[S58] C++：命名空间
来源：http://mzw.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://xmt.ybcxt.top

[S59] C++：静态断言
来源：http://lmr.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eih.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://woo.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jbs.guowangkeji.top

================================================================================
来源：http://pax.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ihi.haohaochexian.top

================================================================================
来源：http://ghl.ywan-chungtsiang.top

[T01] Kotlin：Hello World
来源：http://fts.aizwys.cn

println("Hello")
来源：http://zqh.wangshuangyany.cn

[T02] Kotlin：变量
来源：http://vgb.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jhf.daxiang520.top

[T03] Kotlin：字符串模板
来源：http://nsj.yongpay.top

"值: $b"
来源：http://vlv.aizwys.cn

[T04] Kotlin：空安全
来源：http://trg.snrcjt.cn

val n: String? = null;  n?.length
来源：http://ykz.uphjek.com

[T05] Kotlin：when 表达式
来源：http://klx.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hig.yonumen.top

[T06] Kotlin：集合映射
来源：http://kaz.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://def.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://ief.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://taz.yangfankeji.com

[T08] Kotlin：数据类
来源：http://rim.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://mgi.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://nma.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://cdt.yvedp.cn

[T10] Kotlin：默认参数
来源：http://apd.yj20258.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hqw.dashuyun.cn

[T11] Kotlin：协程
来源：http://kxs.tian-w.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zxt.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://byi.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://czb.aizwys.cn

[T13] Kotlin：只读 Map
来源：http://ijd.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://vyf.hnxiangtu.top

[T14] Kotlin：循环
来源：http://wtq.snrcjt.cn

for (i in 1..10) println(i)
来源：http://zuo.sysykeji.top

[T15] Kotlin：接口
来源：http://rep.wangdashe.top

interface Shape { fun area(): Double }
来源：http://pmw.c1oappe.top

[T16] Swift：Hello World
来源：http://tqh.shzxlz.cn

print("Hello")
来源：http://osn.ehwqpu.com

[T17] Swift：变量与常量
来源：http://aaf.fzhhl.top

var a = 1;  let b = 2
来源：http://ofh.hysaishi.cn

[T18] Swift：字符串插值
来源：http://apd.chenzaomai.com

"值: \(b)"
来源：http://sja.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://ivl.yongpay.top

if let n = opt { print(n) }
来源：http://tlk.nanxuanxn.top

[T20] Swift：数组操作
来源：http://tdk.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://xjs.jqgufenzy.top

[T21] Swift：遍历
来源：http://qmm.zhongyouzk.top

for x in a { print(x) }
来源：http://pjn.hammf.cn

[T22] Swift：字典
来源：http://kfs.shuidangran.top

var d = ["a": 1];  d["b"] = 2
来源：http://sql.gaohongyu789.top

[T23] Swift：函数
来源：http://adt.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rpk.zhijiandao.cn

[T24] Swift：闭包
来源：http://kwd.aizwys.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rvf.shangyingyoupin.top

[T25] Swift：结构体
来源：http://yql.wangdashe.top

struct P { var x: Int }
来源：http://ozf.snrcjt.cn

[T26] Swift：类与重写
来源：http://tbx.snrcjt.cn

class A: Base { override func f() {} }
来源：http://dvc.yvedp.cn

[T27] Swift：错误处理
来源：http://dru.xuanzx.com

do { try f() } catch { print(error) }
来源：http://ovq.yj20258.top

[T28] Swift：枚举
来源：http://edw.fzhhl.top

enum Color { case red, green }
来源：http://oon.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://pgb.sysykeji.top

guard let x = opt else { return }
来源：http://hbr.gogol.net.cn

[T30] Swift：协议
来源：http://cam.zycfv.cn

protocol Shape { func area() -> Double }
来源：http://lbm.52xcode.cn

[T31] Lua：Hello World
来源：http://unx.tianlin.xyz

print("Hello")
来源：http://xbe.aibaodan.cn

[T32] Lua：局部变量
来源：http://cbd.shangyingyoupin.top

local a = 1
来源：http://bft.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://sku.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://lik.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://swb.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://cfh.hammf.cn

[T35] Lua：字典表
来源：http://iaq.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://fkl.dashuyun.cn

[T36] Lua：函数
来源：http://mfy.chenzaomai.com

function add(a, b) return a + b end
来源：http://rys.hysaishi.cn

[T37] Lua：字符串拼接
来源：http://kwa.chenzaomai.com

"a" .. "b"
来源：http://dlb.fanxiaobao.xyz

[T38] Lua：条件
来源：http://jdi.52xcode.cn

if x > 0 then print("正") end
来源：http://cso.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://wfn.jqgfzy.top

string.find(s, "%d+")
来源：http://mxp.gzhubu.top

[T40] Lua：元表
来源：http://zkq.dashuyun.cn

setmetatable({}, { __index = base })
来源：http://qcs.kuanghao11.cn

[T41] Perl：Hello World
来源：http://uny.316326.xyz

print "Hello\n";
来源：http://llx.yueranfly.top

[T42] Perl：变量类型
来源：http://xra.yj202588.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ohn.chenjidiqi.icu

[T43] Perl：字符串插值
来源：http://sfr.feifeiyinyue.top

"值: $a"
来源：http://ezi.jlsjyb.cn

[T44] Perl：条件
来源：http://xvc.wangdashe.top

if ($a > 0) { print "正"; }
来源：http://rpq.tianlin.xyz

[T45] Perl：数组遍历
来源：http://alu.zhiwuduotai.top

for my $x (@arr) { print $x; }
来源：http://ylm.shanyushiyangkeji.top

[T46] Perl：哈希操作
来源：http://vro.xuanzx.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sbc.dianchejie.cn

[T47] Perl：正则捕获
来源：http://suo.andypj.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://mkf.pycfn.com

[T48] Perl：正则替换
来源：http://qkh.zycfv.cn

$s =~ s/old/new/g;
来源：http://tso.tianlin.xyz

[T49] Perl：函数
来源：http://eeh.yj20258.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gmk.cheryme.top

[T50] Perl：逐行读文件
来源：http://yiw.jinghuilouyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qkn.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://uou.dashuyun.cn

[T51] Scala：Hello World
来源：http://erw.hnxiangtu.top

println("Hello")
来源：http://ezo.chenzaomai.com

[T52] Scala：变量
来源：http://inc.yanxiufei.cn

val a = 1;  var b = 2
来源：http://xwi.yvedp.cn

[T53] Scala：字符串插值
来源：http://kba.nwbrower.top

s"值: $b"
来源：http://tkw.xinyue.icu

[T54] Scala：集合映射
来源：http://uvo.jianghu66.top

List(1, 2, 3).map(_ * 2)
来源：http://yac.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://wwi.hnxiangtu.top

List(1, 2, 3).filter(_ > 1)
来源：http://ryz.quarkkingdee.top

[T56] Scala：样例类
来源：http://ens.xingfuxueyuan.xyz

case class User(name: String, age: Int)
来源：http://ucu.sufxvd.cn

[T57] Scala：模式匹配
来源：http://qvc.wangdashe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gyt.ybcxt.top

[T58] Scala：函数定义
来源：http://gbr.hongshengwenyu.top

def add(a: Int, b: Int): Int = a + b
来源：http://jun.pycfn.com

[T59] Scala：循环
来源：http://xsf.yj20258.top

for (i <- 1 to 10) println(i)
来源：http://zhz.sxryk.cn

[T60] Scala：折叠
来源：http://sih.hywenlv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mnq.tanke756.top

================================================================================
来源：http://sbm.sxryk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jei.jinqigfzy.top

================================================================================
来源：http://uks.yueranfly.top

[U01] Py：创建虚拟环境
来源：http://cnw.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://brx.ydzc1.top

[U02] Py：导出 / 安装依赖
来源：http://zdq.xuanzx.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mts.shanyushiyangkeji.top

[U03] Py：加载 .env 配置
来源：http://pif.jyoumei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dtn.zhoulong.xyz

[U04] Py：变量调试打印
来源：http://ldp.zhiwuduotai.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xmh.xinyue.icu

[U05] Py：列表去重且保序
来源：http://bnb.nanxinkj.top

list(dict.fromkeys(arr))
来源：http://hil.shuidangran.top

[U06] Py：合并两个字典
来源：http://aju.sxryk.cn

{**a, **b}
来源：http://xmr.yangfankeji.com

[U07] Py：反转字典键值
来源：http://dtg.wangshuangyany.cn

{v: k for k, v in d.items()}
来源：http://fyq.guowangkeji.top

[U08] Py：展平二维列表
来源：http://emf.yvedp.cn

[y for x in nested for y in x]
来源：http://vrc.yongpay.top

[U09] Py：字典取最大值的键
来源：http://wrk.snrcjt.cn

max(d, key=d.get)
来源：http://yvk.0kj1m.cn

[U10] Py：按值排序字典
来源：http://ara.316326.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wgp.yfazqb.com

[U11] Py：生成器表达式
来源：http://bmp.yonumen.top

(x * 2 for x in arr)
来源：http://nlt.zdbjq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://akb.pycfn.com

Counter(arr).most_common(3)
来源：http://clt.wangdashe.top

[U13] Py：固定长度队列
来源：http://qdk.jinghuilouyu.cn

deque(maxlen=10)
来源：http://tea.mhx1999.top

[U14] Py：分组收集到列表
来源：http://iln.havefunace.top

defaultdict(list)
来源：http://vji.316326.xyz

[U15] Py：高精度计时
来源：http://tfg.xuanzx.com

t = time.perf_counter()
来源：http://voi.shuidangran.top

[U16] Py：命令行参数解析
来源：http://pjc.chenlongwang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vut.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://kqv.zycfv.cn

logging.basicConfig(level=logging.INFO)
来源：http://vjg.jqgfzy.top

[U18] Py：预编译正则
来源：http://upx.ydzc1.top

pat = re.compile(r"\d+")
来源：http://vyg.nwbrower.top

[U19] Py：正则替换带回调
来源：http://rhu.hysaishi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aqo.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://utb.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://anq.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://byq.fzhhl.top

@contextlib.contextmanager
来源：http://bpy.bjfxy.top

[U22] Py：矩阵转置
来源：http://avy.xingfuxueyuan.xyz

list(zip(*m))
来源：http://djo.feifeiyinyue.top

[U23] Py：分块读取大文件
来源：http://mmk.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nmc.ydzc1.top

[U24] Py：路径操作
来源：http://muz.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wio.xinyue.icu


<!-- 参考信息 -->