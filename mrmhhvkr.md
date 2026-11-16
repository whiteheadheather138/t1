代发 wailian999

S. C / C++ 专题
来源：http://ysf.vqdsnc.cn

================================================================================
来源：http://owk.sysykeji.top

[S01] C：Hello World
来源：http://rhi.snrcjt.cn

#include <stdio.h>
来源：http://yhu.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bvu.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://rbw.bjfxy.top

int a = 10; printf("%d\n", a);
来源：http://frg.vqdsnc.cn

[S03] C：读入整数
来源：http://stt.tian-w.cn

int x; scanf("%d", &x);
来源：http://gri.chenzaomai.com

[S04] C：字符串复制
来源：http://obt.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://rkj.iojbl.cn

[S05] C：字符串长度
来源：http://xcn.fengsongda.top

strlen(s)
来源：http://brw.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://cei.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://zdd.sweek.top

[S07] C：数组遍历求和
来源：http://qaf.sysykeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pgm.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://ixf.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xai.hcnkem.com

[S09] C：结构体定义与初始化
来源：http://nki.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jkc.jlsjyb.cn

[S10] C：指针与解引用
来源：http://otl.hcnkem.com

int *p = &a;  *p = 5;
来源：http://ijm.zhoulong.xyz

[S11] C：逐行读文件
来源：http://okp.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://juu.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bfu.tian-w.cn

fclose(f);
来源：http://jpn.c1oappe.top

[S12] C：写文件
来源：http://lfp.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zlz.nwbrower.top

[S13] C：宏定义
来源：http://jxo.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yue.yangfankeji.com

[S14] C：枚举
来源：http://ugq.nanxinkj.top

enum Color { RED, GREEN, BLUE };
来源：http://pxn.vehdjk.com

[S15] C：类型转换
来源：http://trn.aibaodan.cn

(double) a / b
来源：http://lbc.wangdashe.top

[S16] C：位操作置位
来源：http://bkk.kuanghao11.cn

x |= (1 << 3);
来源：http://rfw.yj20258888.top

[S17] C：安全拼接字符串
来源：http://pqg.yfazqb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jdf.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://pwz.yanxiufei.cn

int main(int argc, char **argv)
来源：http://ogu.yj202588.top

[S19] C：快速排序
来源：http://vrl.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://jho.hongshengwenyu.top

[S20] C：二分查找
来源：http://hls.hesvh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jky.yj202588.top

[S21] C：字符类别判断
来源：http://gmg.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qxe.yfazqb.com

[S22] C：字符串转数字
来源：http://yzi.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://vaq.tianlin.xyz

[S23] C：随机数
来源：http://qzg.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://vtc.zhengqikj.top

[S24] C：获取本地时间
来源：http://vgl.sjlbkw.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://itc.tianlin.xyz

[S25] C：内存拷贝
来源：http://lql.hongshengwenyu.top

memcpy(dst, src, n);
来源：http://vbd.bbcook.cn

[S26] C：内存清零
来源：http://aze.hnqzz.top

memset(a, 0, sizeof a);
来源：http://zgs.xuanzx.com

[S27] C：定义常量
来源：http://uro.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://fmd.9152youxi.cn

[S28] C：静态变量
来源：http://hvz.chenzaomai.com

static int counter = 0;
来源：http://isw.tarul.cn

[S29] C：变参函数
来源：http://hnb.quarkkingdee.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://idt.fengsongda.top

[S30] C：头文件保护
来源：http://gxn.xinyue.icu

#ifndef X_H
来源：http://xtc.havefunace.top

#define X_H
来源：http://awe.zdqjudy.top

#endif
来源：http://vhw.nwbrower.top

[S31] C++：Hello World
来源：http://ozu.hcnkem.com

#include <iostream>
来源：http://ytl.nwbrower.top

int main() { std::cout << "Hello\n"; }
来源：http://lqv.tarul.cn

[S32] C++：字符串
来源：http://afc.tarul.cn

std::string s = "hi";  s += "!";
来源：http://sud.yj20258.top

[S33] C++：vector 增删
来源：http://sbo.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wiv.9152youxi.cn

[S34] C++：遍历 vector
来源：http://owj.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://hel.wangdashe.top

[S35] C++：map
来源：http://cel.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wzl.quarkkingdee.top

[S36] C++：unordered_map
来源：http://slw.ppjwa.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://emo.gzhubu.top

[S37] C++：set
来源：http://noj.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dfc.cashguo.top

[S38] C++：排序
来源：http://nqf.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://ddu.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://rru.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ilt.yuxming.cn

[S40] C++：查找元素
来源：http://ink.hysaishi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gxt.zhengqikj.top

[S41] C++：类与构造函数
来源：http://ped.yj202588.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nrc.nanxinkj.top

[S42] C++：继承与虚函数
来源：http://ugl.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://puk.shzxlz.cn

[S43] C++：智能指针
来源：http://xko.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://hfi.yangfankeji.com

[S44] C++：引用传参
来源：http://lgd.pycfn.com

void inc(int &x) { ++x; }
来源：http://zvq.smart0.xyz

[S45] C++：lambda
来源：http://zto.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://wyv.sufxvd.cn

[S46] C++：函数模板
来源：http://ftw.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gur.zhoulong.xyz

[S47] C++：结构化绑定遍历
来源：http://kjz.epnwcf.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kkm.birdmap.top

[S48] C++：逐行读文件
来源：http://ywc.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://dck.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://tla.jqgfzy.top

[S49] C++：写文件
来源：http://vrr.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oad.fehbvm.com

[S50] C++：格式化数字
来源：http://beo.quarkkingdee.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tfb.snrcjt.cn

[S51] C++：显式类型转换
来源：http://dai.sysykeji.top

static_cast<double>(a) / b
来源：http://miz.hnqzz.top

[S52] C++：const 与 noexcept
来源：http://zcu.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://ene.jqgfzy.top

[S53] C++：移动语义
来源：http://ffl.chenlongwang.top

std::vector<int> w = std::move(v);
来源：http://kav.hammf.cn

[S54] C++：异常处理
来源：http://jyg.chenzaomai.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wll.yuanzhike.top

[S55] C++：结构化绑定
来源：http://icc.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yvz.iojbl.cn

[S56] C++：optional
来源：http://tli.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oup.ydzc1.top

[S57] C++：编译期常量
来源：http://thv.gogol.net.cn

constexpr int N = 10;
来源：http://rjg.yueranfly.top

[S58] C++：命名空间
来源：http://xue.jinqigufen.top

namespace ns { int f() { return 1; } }
来源：http://lch.redwolf501.top

[S59] C++：静态断言
来源：http://qod.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vac.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://loq.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://amk.fengsongda.top

================================================================================
来源：http://krp.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qbg.0kj1m.cn

================================================================================
来源：http://srq.hammf.cn

[T01] Kotlin：Hello World
来源：http://dfo.yj20258.top

println("Hello")
来源：http://uuy.0kj1m.cn

[T02] Kotlin：变量
来源：http://skg.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ubm.snrcjt.cn

[T03] Kotlin：字符串模板
来源：http://kpr.uphjek.com

"值: $b"
来源：http://dnp.shuidangran.top

[T04] Kotlin：空安全
来源：http://mks.snrcjt.cn

val n: String? = null;  n?.length
来源：http://qwt.ppjwa.cn

[T05] Kotlin：when 表达式
来源：http://vsc.zhongyouzk.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iwf.sweek.top

[T06] Kotlin：集合映射
来源：http://bgb.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qci.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://dtq.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://opz.chenjidiqi.icu

[T08] Kotlin：数据类
来源：http://xer.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://rgk.jqgfzy.top

[T09] Kotlin：扩展函数
来源：http://pij.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://tpp.yj20258.top

[T10] Kotlin：默认参数
来源：http://qtc.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ufv.ctjpmb.com

[T11] Kotlin：协程
来源：http://bcw.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://phb.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://qhw.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://iec.ivvv.top

[T13] Kotlin：只读 Map
来源：http://yqc.ivvv.top

val m = mapOf("a" to 1)
来源：http://fte.andypj.xyz

[T14] Kotlin：循环
来源：http://coc.c1oappe.top

for (i in 1..10) println(i)
来源：http://qye.birdmap.top

[T15] Kotlin：接口
来源：http://gug.jlsjyb.cn

interface Shape { fun area(): Double }
来源：http://xut.jinyuanbaomall.cn

[T16] Swift：Hello World
来源：http://cmm.nanxinkj.top

print("Hello")
来源：http://vmh.nanxinkj.top

[T17] Swift：变量与常量
来源：http://ngh.zhongyouzk.top

var a = 1;  let b = 2
来源：http://trc.xinyue.icu

[T18] Swift：字符串插值
来源：http://hxy.ybcxt.top

"值: \(b)"
来源：http://dkv.ppjwa.cn

[T19] Swift：可选绑定
来源：http://sqo.gogol.net.cn

if let n = opt { print(n) }
来源：http://jbr.meibo888.top

[T20] Swift：数组操作
来源：http://zxz.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://vbu.bjfxy.top

[T21] Swift：遍历
来源：http://jpx.jqgfzy.top

for x in a { print(x) }
来源：http://ejz.zhixingplan.top

[T22] Swift：字典
来源：http://qdd.316326.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://njr.redwolf501.top

[T23] Swift：函数
来源：http://swd.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xnl.ydjk.org.cn

[T24] Swift：闭包
来源：http://mpx.epnwcf.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://wad.zhengqikj.top

[T25] Swift：结构体
来源：http://yyl.ydjk.org.cn

struct P { var x: Int }
来源：http://bdj.daxiang520.top

[T26] Swift：类与重写
来源：http://cqg.havefunace.top

class A: Base { override func f() {} }
来源：http://bdt.hywenlv.cn

[T27] Swift：错误处理
来源：http://pyk.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://zuj.0kj1m.cn

[T28] Swift：枚举
来源：http://hba.hnxiangtu.top

enum Color { case red, green }
来源：http://vlr.jyoumei.cn

[T29] Swift：guard 提前返回
来源：http://jjc.nwbrower.top

guard let x = opt else { return }
来源：http://uos.zhixingplan.top

[T30] Swift：协议
来源：http://rep.wangdashe.top

protocol Shape { func area() -> Double }
来源：http://zdl.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://ikv.ywan-chungtsiang.top

print("Hello")
来源：http://ohu.mhx1999.top

[T32] Lua：局部变量
来源：http://lni.zhijiandao.cn

local a = 1
来源：http://ylb.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://xaq.dianchejie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xcy.hnxiangtu.top

[T34] Lua：遍历表
来源：http://mba.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wnl.vqdsnc.cn

[T35] Lua：字典表
来源：http://eby.cdnleiting.top

local d = { a = 1 };  d.b = 2
来源：http://vas.cdnleiting.top

[T36] Lua：函数
来源：http://vph.gotoacloud.top

function add(a, b) return a + b end
来源：http://zxx.birdmap.top

[T37] Lua：字符串拼接
来源：http://qhj.ctjpmb.com

"a" .. "b"
来源：http://azw.yuanzhike.top

[T38] Lua：条件
来源：http://qxb.xylfe.cn

if x > 0 then print("正") end
来源：http://hds.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://nsg.shuidangran.top

string.find(s, "%d+")
来源：http://ume.zhoulong.xyz

[T40] Lua：元表
来源：http://jqy.fktsv.cn

setmetatable({}, { __index = base })
来源：http://hxn.ywan-chungtsiang.top

[T41] Perl：Hello World
来源：http://ujl.bjfxy.top

print "Hello\n";
来源：http://bee.9152youxi.cn

[T42] Perl：变量类型
来源：http://gmk.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lgb.xingfuxueyuan.xyz

[T43] Perl：字符串插值
来源：http://syt.ivvv.top

"值: $a"
来源：http://dil.jlsjyb.cn

[T44] Perl：条件
来源：http://jad.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://rdc.pycfn.com

[T45] Perl：数组遍历
来源：http://mwg.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://eps.jqgfzy.top

[T46] Perl：哈希操作
来源：http://qhn.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vcg.zhijiandao.cn

[T47] Perl：正则捕获
来源：http://vfg.tarul.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ucq.uphjek.com

[T48] Perl：正则替换
来源：http://rho.svipenyu.cn

$s =~ s/old/new/g;
来源：http://unl.gzhubu.top

[T49] Perl：函数
来源：http://alf.fzhhl.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bbb.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://vmu.xziqi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oll.ppjwa.cn

while (my $line = <$fh>) { print $line; }
来源：http://aok.quarkkingdee.top

[T51] Scala：Hello World
来源：http://scb.jinqigufen.top

println("Hello")
来源：http://tus.guannengcc.top

[T52] Scala：变量
来源：http://doa.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://jod.tian-w.cn

[T53] Scala：字符串插值
来源：http://zuz.zdbjq.cn

s"值: $b"
来源：http://kvp.316326.xyz

[T54] Scala：集合映射
来源：http://zvu.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://zee.chenjidiqi.icu

[T55] Scala：集合过滤
来源：http://ykj.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://xii.cheryme.top

[T56] Scala：样例类
来源：http://abg.jinqigufen.top

case class User(name: String, age: Int)
来源：http://urm.ybcxt.top

[T57] Scala：模式匹配
来源：http://lzh.shangyingyoupin.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://upe.iojbl.cn

[T58] Scala：函数定义
来源：http://aec.yj20258888.top

def add(a: Int, b: Int): Int = a + b
来源：http://nxd.ydjk.org.cn

[T59] Scala：循环
来源：http://epq.xziqi.cn

for (i <- 1 to 10) println(i)
来源：http://dyq.jinqigufen.top

[T60] Scala：折叠
来源：http://eoz.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://puw.316326.xyz

================================================================================
来源：http://pvn.redwolf501.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://khu.yj202588.top

================================================================================
来源：http://fqp.meibo888.top

[U01] Py：创建虚拟环境
来源：http://aii.hysaishi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sir.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://yiy.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jdt.yongpay.top

[U03] Py：加载 .env 配置
来源：http://gpg.vehdjk.com

from dotenv import load_dotenv; load_dotenv()
来源：http://tmj.zhijiandao.cn

[U04] Py：变量调试打印
来源：http://jac.fktsv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://slf.fktsv.cn

[U05] Py：列表去重且保序
来源：http://stv.shanyushiyangtech.top

list(dict.fromkeys(arr))
来源：http://ahe.tanke756.top

[U06] Py：合并两个字典
来源：http://dfr.zhengqikj.top

{**a, **b}
来源：http://ecg.yvedp.cn

[U07] Py：反转字典键值
来源：http://izg.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://eiq.zhoulong.xyz

[U08] Py：展平二维列表
来源：http://qrm.hywenlv.cn

[y for x in nested for y in x]
来源：http://elv.cdnleiting.top

[U09] Py：字典取最大值的键
来源：http://ppq.wangshuangyany.cn

max(d, key=d.get)
来源：http://vru.sxryk.cn

[U10] Py：按值排序字典
来源：http://joa.hnqzz.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bef.tanke756.top

[U11] Py：生成器表达式
来源：http://xat.316326.xyz

(x * 2 for x in arr)
来源：http://qwx.yuxming.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xzy.yonumen.top

Counter(arr).most_common(3)
来源：http://dvw.jyoumei.cn

[U13] Py：固定长度队列
来源：http://nqq.guowangkeji.top

deque(maxlen=10)
来源：http://vha.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://gbe.aibaodan.cn

defaultdict(list)
来源：http://nwo.fanxiaobao.xyz

[U15] Py：高精度计时
来源：http://hej.yvedp.cn

t = time.perf_counter()
来源：http://unb.ywan-chungtsiang.top

[U16] Py：命令行参数解析
来源：http://khx.yfazqb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qgi.yuanzhike.top

[U17] Py：初始化日志
来源：http://xbt.yanxiufei.cn

logging.basicConfig(level=logging.INFO)
来源：http://ora.aibaodan.cn

[U18] Py：预编译正则
来源：http://jak.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://ojq.cashguo.top

[U19] Py：正则替换带回调
来源：http://fgz.vehdjk.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ozx.hesvh.cn

[U20] Py：缓存函数结果
来源：http://hun.jyoumei.cn

@functools.lru_cache(maxsize=None)
来源：http://mza.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://wyk.nwbrower.top

@contextlib.contextmanager
来源：http://tlr.chenlongwang.top

[U22] Py：矩阵转置
来源：http://euo.tarul.cn

list(zip(*m))
来源：http://efb.sweek.top


<!-- 参考信息 -->