代发 wailian999

S. C / C++ 专题
来源：http://ulc.jinqigfzy.top

================================================================================
来源：http://hur.pengpengdd.cyou

[S01] C：Hello World
来源：http://sro.xylfe.cn

#include <stdio.h>
来源：http://geo.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://iri.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://fvs.daria6918.cn

int a = 10; printf("%d\n", a);
来源：http://mbp.guowangkeji.top

[S03] C：读入整数
来源：http://xzh.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://rhb.zhoulong.xyz

[S04] C：字符串复制
来源：http://pjy.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://ysh.wangdashe.top

[S05] C：字符串长度
来源：http://mke.zhoulong.xyz

strlen(s)
来源：http://gth.vqdsnc.cn

[S06] C：字符串比较
来源：http://csd.ctjpmb.com

strcmp(a, b) == 0
来源：http://oku.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://foq.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://peb.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://xde.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qgc.birdmap.top

[S09] C：结构体定义与初始化
来源：http://teg.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lsr.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://qfc.sweek.top

int *p = &a;  *p = 5;
来源：http://boo.bbcook.cn

[S11] C：逐行读文件
来源：http://xxz.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://gdj.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bpw.jqgfzy.top

fclose(f);
来源：http://vsu.aibaodan.cn

[S12] C：写文件
来源：http://ukb.0kj1m.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ktk.zhengqikj.top

[S13] C：宏定义
来源：http://hhh.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://stc.xinyue.icu

[S14] C：枚举
来源：http://toe.snrcjt.cn

enum Color { RED, GREEN, BLUE };
来源：http://tgu.hammf.cn

[S15] C：类型转换
来源：http://isn.tarul.cn

(double) a / b
来源：http://gwk.52xcode.cn

[S16] C：位操作置位
来源：http://cak.tanke756.top

x |= (1 << 3);
来源：http://iqh.hfpthk.cn

[S17] C：安全拼接字符串
来源：http://gsu.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pie.daria6918.cn

[S18] C：命令行参数
来源：http://rbq.jlsjyb.cn

int main(int argc, char **argv)
来源：http://lat.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://aol.hnqzz.top

qsort(a, n, sizeof(int), cmp);
来源：http://jbz.haohaochexian.top

[S20] C：二分查找
来源：http://tjj.zhoulong.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xfm.zhengqikj.top

[S21] C：字符类别判断
来源：http://ytc.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fgq.chenlongwang.top

[S22] C：字符串转数字
来源：http://rwa.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mnb.hesvh.cn

[S23] C：随机数
来源：http://icy.sxryk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pvd.jiagoushi.top

[S24] C：获取本地时间
来源：http://tyu.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nai.zhijiandao.cn

[S25] C：内存拷贝
来源：http://mdp.yj20258.top

memcpy(dst, src, n);
来源：http://lir.sjlbkw.cn

[S26] C：内存清零
来源：http://unk.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://bga.jinqigfzy.top

[S27] C：定义常量
来源：http://xji.jqgufenzy.top

const double PI = 3.14159;
来源：http://vml.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://kzm.daria6918.cn

static int counter = 0;
来源：http://sya.zhixingplan.top

[S29] C：变参函数
来源：http://nbt.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://spr.jlsjyb.cn

[S30] C：头文件保护
来源：http://fad.daxiang520.top

#ifndef X_H
来源：http://kiz.chenlongwang.top

#define X_H
来源：http://ppb.dashuyun.cn

#endif
来源：http://xeg.zhoulong.xyz

[S31] C++：Hello World
来源：http://owj.pycfn.com

#include <iostream>
来源：http://gqz.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://rgq.52xcode.cn

[S32] C++：字符串
来源：http://zgs.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://uks.redwolf501.top

[S33] C++：vector 增删
来源：http://zaf.cucudq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wpd.zhixingplan.top

[S34] C++：遍历 vector
来源：http://hat.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://iuv.chenlongwang.top

[S35] C++：map
来源：http://xfs.jinqigufen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jno.aizwys.cn

[S36] C++：unordered_map
来源：http://ijs.jinqigufen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kob.fanxiaobao.xyz

[S37] C++：set
来源：http://cvq.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qzu.c1oappe.top

[S38] C++：排序
来源：http://kno.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://qvd.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://cji.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hpo.hysaishi.cn

[S40] C++：查找元素
来源：http://duh.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://psi.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://gyt.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kjl.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://gvg.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://zeb.snrcjt.cn

[S43] C++：智能指针
来源：http://jzy.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://ess.yj20258888.top

[S44] C++：引用传参
来源：http://rye.xinyue.icu

void inc(int &x) { ++x; }
来源：http://rfo.jiagoushi.top

[S45] C++：lambda
来源：http://jaq.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hwk.jqgufenzy.top

[S46] C++：函数模板
来源：http://uxh.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tqj.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://ukn.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qky.ctjpmb.com

[S48] C++：逐行读文件
来源：http://dqo.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://eoa.cucudq.cn

while (std::getline(in, line)) { }
来源：http://vdg.hammf.cn

[S49] C++：写文件
来源：http://qjf.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://txz.yuanzhike.top

[S50] C++：格式化数字
来源：http://tjv.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fuq.fengsongda.top

[S51] C++：显式类型转换
来源：http://szo.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://iny.ywan-chungtsiang.top

[S52] C++：const 与 noexcept
来源：http://ugx.ehwqpu.com

int size() const noexcept { return n_; }
来源：http://bfe.mhx1999.top

[S53] C++：移动语义
来源：http://iuw.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://odc.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://myc.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nht.gzhubu.top

[S55] C++：结构化绑定
来源：http://lol.cucudq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rat.mhx1999.top

[S56] C++：optional
来源：http://gty.uphjek.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eqn.52xcode.cn

[S57] C++：编译期常量
来源：http://vfv.uphjek.com

constexpr int N = 10;
来源：http://hfm.xuetiantiany.cn

[S58] C++：命名空间
来源：http://fmj.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://mex.zhijiandao.cn

[S59] C++：静态断言
来源：http://xci.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qrv.shanyushiyangtech.top

[S60] C++：遍历并删除元素
来源：http://ebm.bbcook.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rau.cheryme.top

================================================================================
来源：http://mch.yueranfly.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vwk.chenzaomai.com

================================================================================
来源：http://npl.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://iuw.ydjk.org.cn

println("Hello")
来源：http://sli.yueranfly.top

[T02] Kotlin：变量
来源：http://vgz.yj202588.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bhb.birdmap.top

[T03] Kotlin：字符串模板
来源：http://baw.fehbvm.com

"值: $b"
来源：http://ywb.sufxvd.cn

[T04] Kotlin：空安全
来源：http://uoi.nanxuanxn.top

val n: String? = null;  n?.length
来源：http://btu.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://sii.zhongyouzk.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://olg.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://gmr.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://bnq.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://lpa.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vrz.ivvv.top

[T08] Kotlin：数据类
来源：http://gzx.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://lgl.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://zua.ybcxt.top

fun String.exclaim() = this + "!"
来源：http://aej.vehdjk.com

[T10] Kotlin：默认参数
来源：http://yes.yangfankeji.com

fun greet(name: String = "World") = "Hi $name"
来源：http://tlb.jqgfzy.top

[T11] Kotlin：协程
来源：http://mhw.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://rym.xylfe.cn

[T12] Kotlin：解构声明
来源：http://xpm.jinghuilouyu.cn

val (a, b) = Pair(1, 2)
来源：http://gso.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://nhf.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://pfo.andypj.xyz

[T14] Kotlin：循环
来源：http://hwc.zdqjudy.top

for (i in 1..10) println(i)
来源：http://yfx.nanxinkj.top

[T15] Kotlin：接口
来源：http://kpj.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://vtc.fzhhl.top

[T16] Swift：Hello World
来源：http://hie.jyoumei.cn

print("Hello")
来源：http://kow.ydzc1.top

[T17] Swift：变量与常量
来源：http://eol.xuetiantiany.cn

var a = 1;  let b = 2
来源：http://rbd.haohaochexian.top

[T18] Swift：字符串插值
来源：http://hmh.zhongyouzk.top

"值: \(b)"
来源：http://osg.0kj1m.cn

[T19] Swift：可选绑定
来源：http://zuv.yuxming.cn

if let n = opt { print(n) }
来源：http://jwn.zhoulong.xyz

[T20] Swift：数组操作
来源：http://gsq.chenjidiqi.icu

var a = [1, 2, 3];  a.append(4)
来源：http://wbr.zdqjudy.top

[T21] Swift：遍历
来源：http://ani.sysykeji.top

for x in a { print(x) }
来源：http://gcc.tianlin.xyz

[T22] Swift：字典
来源：http://zkb.ehwqpu.com

var d = ["a": 1];  d["b"] = 2
来源：http://imw.tarul.cn

[T23] Swift：函数
来源：http://ctb.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mkg.hongshengwenyu.top

[T24] Swift：闭包
来源：http://abp.cucudq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gqm.birdmap.top

[T25] Swift：结构体
来源：http://zrp.gotoacloud.top

struct P { var x: Int }
来源：http://qys.yanxiufei.cn

[T26] Swift：类与重写
来源：http://ahh.cheryme.top

class A: Base { override func f() {} }
来源：http://sqa.wangdashe.top

[T27] Swift：错误处理
来源：http://mvr.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://udj.gotoacloud.top

[T28] Swift：枚举
来源：http://etk.meibo888.top

enum Color { case red, green }
来源：http://jzy.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://pqz.chenzaomai.com

guard let x = opt else { return }
来源：http://ccu.zhoulong.xyz

[T30] Swift：协议
来源：http://mvq.fengsongda.top

protocol Shape { func area() -> Double }
来源：http://jek.havefunace.top

[T31] Lua：Hello World
来源：http://uio.meibo888.top

print("Hello")
来源：http://ggv.havefunace.top

[T32] Lua：局部变量
来源：http://znh.guowangkeji.top

local a = 1
来源：http://ywm.fktsv.cn

[T33] Lua：表（数组）
来源：http://stf.chenjidiqi.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://yyc.haohaochexian.top

[T34] Lua：遍历表
来源：http://vwu.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nni.yongpay.top

[T35] Lua：字典表
来源：http://lfa.chenzaomai.com

local d = { a = 1 };  d.b = 2
来源：http://naf.mhx1999.top

[T36] Lua：函数
来源：http://fam.vehdjk.com

function add(a, b) return a + b end
来源：http://yny.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://kkm.jianghu66.top

"a" .. "b"
来源：http://pak.aizwys.cn

[T38] Lua：条件
来源：http://jao.fktsv.cn

if x > 0 then print("正") end
来源：http://cwc.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://mru.sufxvd.cn

string.find(s, "%d+")
来源：http://ewu.jinqigfzy.top

[T40] Lua：元表
来源：http://weo.smart0.xyz

setmetatable({}, { __index = base })
来源：http://lhf.feifeiyinyue.top

[T41] Perl：Hello World
来源：http://twg.sufxvd.cn

print "Hello\n";
来源：http://jtl.gotoacloud.top

[T42] Perl：变量类型
来源：http://jgr.jinyuanbaomall.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://drb.zhaomingkeji.xyz

[T43] Perl：字符串插值
来源：http://fpl.shanyushiyangtech.top

"值: $a"
来源：http://oju.gzhubu.top

[T44] Perl：条件
来源：http://chr.fehbvm.com

if ($a > 0) { print "正"; }
来源：http://jvq.bbcook.cn

[T45] Perl：数组遍历
来源：http://kra.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://kle.fzhhl.top

[T46] Perl：哈希操作
来源：http://whx.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://orb.guannengcc.top

[T47] Perl：正则捕获
来源：http://ytr.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vlk.ctjpmb.com

[T48] Perl：正则替换
来源：http://jxo.smart0.xyz

$s =~ s/old/new/g;
来源：http://zsv.xylfe.cn

[T49] Perl：函数
来源：http://ijn.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://quj.52xcode.cn

[T50] Perl：逐行读文件
来源：http://tmp.ivvv.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pce.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://lcr.shuidangran.top

[T51] Scala：Hello World
来源：http://xyj.zhixingplan.top

println("Hello")
来源：http://mlz.cashguo.top

[T52] Scala：变量
来源：http://zeq.nwbrower.top

val a = 1;  var b = 2
来源：http://voc.wangdashe.top

[T53] Scala：字符串插值
来源：http://pzc.fengsongda.top

s"值: $b"
来源：http://wrz.jyoumei.cn

[T54] Scala：集合映射
来源：http://szg.shuidangran.top

List(1, 2, 3).map(_ * 2)
来源：http://hnm.xingfuxueyuan.xyz

[T55] Scala：集合过滤
来源：http://uxa.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://gag.316326.xyz

[T56] Scala：样例类
来源：http://ixa.vehdjk.com

case class User(name: String, age: Int)
来源：http://szb.yj20258888.top

[T57] Scala：模式匹配
来源：http://cov.hammf.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://frq.jqgfzy.top

[T58] Scala：函数定义
来源：http://gwq.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://cbt.tianlin.xyz

[T59] Scala：循环
来源：http://lmy.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://nup.gaohongyu789.top

[T60] Scala：折叠
来源：http://jeo.sxryk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://auh.hnxiangtu.top

================================================================================
来源：http://xav.xuanzx.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dnm.ctjpmb.com

================================================================================
来源：http://vhy.zhongyouzk.top

[U01] Py：创建虚拟环境
来源：http://kyh.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://wfg.shanyushiyangtech.top

[U02] Py：导出 / 安装依赖
来源：http://rng.andypj.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tyk.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://wst.cucudq.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xog.zhengqikj.top

[U04] Py：变量调试打印
来源：http://gby.chenjidiqi.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vqu.hesvh.cn

[U05] Py：列表去重且保序
来源：http://ral.nwbrower.top

list(dict.fromkeys(arr))
来源：http://puv.xingfuxueyuan.xyz

[U06] Py：合并两个字典
来源：http://rzd.daria6918.cn

{**a, **b}
来源：http://jsp.hysaishi.cn

[U07] Py：反转字典键值
来源：http://lov.iojbl.cn

{v: k for k, v in d.items()}
来源：http://ymf.aizwys.cn

[U08] Py：展平二维列表
来源：http://dph.cdnleiting.top

[y for x in nested for y in x]
来源：http://dnc.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://ldt.gogol.net.cn

max(d, key=d.get)
来源：http://tvd.redwolf501.top

[U10] Py：按值排序字典
来源：http://fcx.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bao.gzhubu.top

[U11] Py：生成器表达式
来源：http://fay.sjlbkw.cn

(x * 2 for x in arr)
来源：http://gen.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://ffq.hnqzz.top

Counter(arr).most_common(3)
来源：http://hlu.ivvv.top

[U13] Py：固定长度队列
来源：http://mps.hesvh.cn

deque(maxlen=10)
来源：http://ohv.hongshengwenyu.top

[U14] Py：分组收集到列表
来源：http://lei.ctjpmb.com

defaultdict(list)
来源：http://uli.yj20258.top

[U15] Py：高精度计时
来源：http://apc.havefunace.top

t = time.perf_counter()
来源：http://kux.jianghu66.top

[U16] Py：命令行参数解析
来源：http://auk.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ptz.zhongyouzk.top

[U17] Py：初始化日志
来源：http://jkr.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://fsj.ydzc1.top

[U18] Py：预编译正则
来源：http://uxe.ybcxt.top

pat = re.compile(r"\d+")
来源：http://dzo.jqgfzy.top

[U19] Py：正则替换带回调
来源：http://zua.zhengqikj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zho.52xcode.cn

[U20] Py：缓存函数结果
来源：http://kwf.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://dzo.nanxinkj.top

[U21] Py：自定义上下文管理器
来源：http://byx.aibaodan.cn

@contextlib.contextmanager
来源：http://ehs.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://ljq.ppjwa.cn

list(zip(*m))
来源：http://mbu.yueranfly.top


<!-- 参考信息 -->