代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://epw.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://qda.ywan-chungtsiang.top

time ./run.sh
来源：http://gke.tarul.cn

================================================================================
来源：http://deh.guannengcc.top

S. C / C++ 专题
来源：http://lqj.ctjpmb.com

================================================================================
来源：http://lng.316326.xyz

[S01] C：Hello World
来源：http://rzj.zhiwuduotai.top

#include <stdio.h>
来源：http://qto.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cuq.sysykeji.top

[S02] C：变量与格式化输出
来源：http://ssi.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://qjc.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://vlp.hesvh.cn

int x; scanf("%d", &x);
来源：http://xzv.zdqjudy.top

[S04] C：字符串复制
来源：http://suv.tianlin.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://mjl.daria6918.cn

[S05] C：字符串长度
来源：http://cij.zdqjudy.top

strlen(s)
来源：http://gfv.jqgfzy.top

[S06] C：字符串比较
来源：http://raq.yanxiufei.cn

strcmp(a, b) == 0
来源：http://usi.tian-w.cn

[S07] C：数组遍历求和
来源：http://klo.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dqe.yj20258.top

[S08] C：动态内存分配与释放
来源：http://tgh.shanyushiyangtech.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dbz.dianchejie.cn

[S09] C：结构体定义与初始化
来源：http://kns.andypj.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lxp.yuanzhike.top

[S10] C：指针与解引用
来源：http://owz.tanke756.top

int *p = &a;  *p = 5;
来源：http://onx.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://awl.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://ikg.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zkf.hongshengwenyu.top

fclose(f);
来源：http://mcl.c1oappe.top

[S12] C：写文件
来源：http://cem.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pxy.andypj.xyz

[S13] C：宏定义
来源：http://mpi.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zwx.yj20258888.top

[S14] C：枚举
来源：http://itd.fehbvm.com

enum Color { RED, GREEN, BLUE };
来源：http://sie.sweek.top

[S15] C：类型转换
来源：http://xfq.vehdjk.com

(double) a / b
来源：http://syt.sufxvd.cn

[S16] C：位操作置位
来源：http://wnj.tianlin.xyz

x |= (1 << 3);
来源：http://scu.havefunace.top

[S17] C：安全拼接字符串
来源：http://vnr.aibaodan.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gxp.chenzaomai.com

[S18] C：命令行参数
来源：http://yhl.fehbvm.com

int main(int argc, char **argv)
来源：http://tqo.meibo888.top

[S19] C：快速排序
来源：http://bji.jqgufenzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://rah.316326.xyz

[S20] C：二分查找
来源：http://oej.yangfankeji.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://spj.sufxvd.cn

[S21] C：字符类别判断
来源：http://ypk.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://axy.hnqzz.top

[S22] C：字符串转数字
来源：http://nxg.nanxuanxn.top

atoi("42");  strtod("3.14", NULL);
来源：http://zey.fehbvm.com

[S23] C：随机数
来源：http://msw.hfpthk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bxr.svipenyu.cn

[S24] C：获取本地时间
来源：http://dfo.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wao.cashguo.top

[S25] C：内存拷贝
来源：http://adz.zycfv.cn

memcpy(dst, src, n);
来源：http://cyt.snrcjt.cn

[S26] C：内存清零
来源：http://yyg.cdnleiting.top

memset(a, 0, sizeof a);
来源：http://iea.wangshuangyany.cn

[S27] C：定义常量
来源：http://fbi.hnqzz.top

const double PI = 3.14159;
来源：http://ddx.svipenyu.cn

[S28] C：静态变量
来源：http://zwp.uphjek.com

static int counter = 0;
来源：http://wgp.sweek.top

[S29] C：变参函数
来源：http://xfs.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iwd.hesvh.cn

[S30] C：头文件保护
来源：http://hhk.xuanzx.com

#ifndef X_H
来源：http://vsj.hnxiangtu.top

#define X_H
来源：http://cvl.uphjek.com

#endif
来源：http://hov.yongpay.top

[S31] C++：Hello World
来源：http://qrc.feifeiyinyue.top

#include <iostream>
来源：http://bkd.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://gqx.hfpthk.cn

[S32] C++：字符串
来源：http://cjn.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://ndn.nanxinkj.top

[S33] C++：vector 增删
来源：http://jod.tian-w.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uvv.dashuyun.cn

[S34] C++：遍历 vector
来源：http://nxs.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://jkq.dashuyun.cn

[S35] C++：map
来源：http://die.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lru.andypj.xyz

[S36] C++：unordered_map
来源：http://qoj.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jsd.yj20258.top

[S37] C++：set
来源：http://kzf.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ife.jlsjyb.cn

[S38] C++：排序
来源：http://upj.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://qcz.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://jdo.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pxf.zhongyouzk.top

[S40] C++：查找元素
来源：http://gnz.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aud.hnxiangtu.top

[S41] C++：类与构造函数
来源：http://ywy.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bgx.316326.xyz

[S42] C++：继承与虚函数
来源：http://lbr.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://jgh.nanxinkj.top

[S43] C++：智能指针
来源：http://azd.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://zfw.yj202588.top

[S44] C++：引用传参
来源：http://jir.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://eol.meibo888.top

[S45] C++：lambda
来源：http://wqp.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://oii.kuanghao11.cn

[S46] C++：函数模板
来源：http://klx.gogol.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://snr.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://zjl.jinqigfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wbq.ivvv.top

[S48] C++：逐行读文件
来源：http://hdi.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://lqi.bjfxy.top

while (std::getline(in, line)) { }
来源：http://ytz.xuetiantiany.cn

[S49] C++：写文件
来源：http://krl.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gxx.nanxuanxn.top

[S50] C++：格式化数字
来源：http://bht.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yev.ywan-chungtsiang.top

[S51] C++：显式类型转换
来源：http://lez.zdbjq.cn

static_cast<double>(a) / b
来源：http://yfh.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://olh.tarul.cn

int size() const noexcept { return n_; }
来源：http://uim.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://rph.ywan-chungtsiang.top

std::vector<int> w = std::move(v);
来源：http://mgz.chenzaomai.com

[S54] C++：异常处理
来源：http://ddb.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gqm.yuanzhike.top

[S55] C++：结构化绑定
来源：http://dop.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jvi.zhiwuduotai.top

[S56] C++：optional
来源：http://mrw.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://khd.ybcxt.top

[S57] C++：编译期常量
来源：http://zva.xylfe.cn

constexpr int N = 10;
来源：http://ncf.sweek.top

[S58] C++：命名空间
来源：http://lmv.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://llj.sweek.top

[S59] C++：静态断言
来源：http://srz.cdnleiting.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://udx.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://agb.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tgx.shuidangran.top

================================================================================
来源：http://exl.redwolf501.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://grx.epnwcf.com

================================================================================
来源：http://ouv.fanxiaobao.xyz

[T01] Kotlin：Hello World
来源：http://nau.jinqigufen.top

println("Hello")
来源：http://dmx.mhx1999.top

[T02] Kotlin：变量
来源：http://ywh.cucudq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pws.jinghuilouyu.cn

[T03] Kotlin：字符串模板
来源：http://jmf.ywan-chungtsiang.top

"值: $b"
来源：http://izk.andypj.xyz

[T04] Kotlin：空安全
来源：http://pcn.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://hov.zhiwuduotai.top

[T05] Kotlin：when 表达式
来源：http://ysb.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hbl.guannengcc.top

[T06] Kotlin：集合映射
来源：http://ehs.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://aht.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://hgn.jinghuilouyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://swe.feifeiyinyue.top

[T08] Kotlin：数据类
来源：http://meb.jlsjyb.cn

data class User(val name: String, val age: Int)
来源：http://pyj.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://mtn.hesvh.cn

fun String.exclaim() = this + "!"
来源：http://sau.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://sgc.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nvl.fzhhl.top

[T11] Kotlin：协程
来源：http://ojz.bjfxy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dia.ppjwa.cn

[T12] Kotlin：解构声明
来源：http://wno.epnwcf.com

val (a, b) = Pair(1, 2)
来源：http://dzz.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://maw.jqgfzy.top

val m = mapOf("a" to 1)
来源：http://szj.316326.xyz

[T14] Kotlin：循环
来源：http://jmv.xziqi.cn

for (i in 1..10) println(i)
来源：http://ktv.yfazqb.com

[T15] Kotlin：接口
来源：http://eif.vehdjk.com

interface Shape { fun area(): Double }
来源：http://gze.tarul.cn

[T16] Swift：Hello World
来源：http://sxy.meibo888.top

print("Hello")
来源：http://bzp.xylfe.cn

[T17] Swift：变量与常量
来源：http://hkc.fktsv.cn

var a = 1;  let b = 2
来源：http://zhe.ybcxt.top

[T18] Swift：字符串插值
来源：http://les.ctjpmb.com

"值: \(b)"
来源：http://nud.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://tgo.ydzc1.top

if let n = opt { print(n) }
来源：http://rrl.sysykeji.top

[T20] Swift：数组操作
来源：http://auf.jinqigufen.top

var a = [1, 2, 3];  a.append(4)
来源：http://kog.daria6918.cn

[T21] Swift：遍历
来源：http://hhv.sjlbkw.cn

for x in a { print(x) }
来源：http://juv.yongpay.top

[T22] Swift：字典
来源：http://ylx.0kj1m.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mgv.ydzc1.top

[T23] Swift：函数
来源：http://mib.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nog.meibo888.top

[T24] Swift：闭包
来源：http://kah.aibaodan.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lpo.epnwcf.com

[T25] Swift：结构体
来源：http://set.yangfankeji.com

struct P { var x: Int }
来源：http://iml.tianlin.xyz

[T26] Swift：类与重写
来源：http://joq.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://blv.uphjek.com

[T27] Swift：错误处理
来源：http://bem.zdbjq.cn

do { try f() } catch { print(error) }
来源：http://cjc.hongshengwenyu.top

[T28] Swift：枚举
来源：http://bcx.zhiwuduotai.top

enum Color { case red, green }
来源：http://kob.cashguo.top

[T29] Swift：guard 提前返回
来源：http://aap.yj202588.top

guard let x = opt else { return }
来源：http://pum.iojbl.cn

[T30] Swift：协议
来源：http://gin.sxryk.cn

protocol Shape { func area() -> Double }
来源：http://osr.9152youxi.cn

[T31] Lua：Hello World
来源：http://ian.jinqigufen.top

print("Hello")
来源：http://mrv.svipenyu.cn

[T32] Lua：局部变量
来源：http://sho.mhx1999.top

local a = 1
来源：http://qyf.zycfv.cn

[T33] Lua：表（数组）
来源：http://dtn.nanxuanxn.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zdk.bjfxy.top

[T34] Lua：遍历表
来源：http://zpn.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qpr.yj20258.top

[T35] Lua：字典表
来源：http://tnq.yanxiufei.cn

local d = { a = 1 };  d.b = 2
来源：http://ofg.gotoacloud.top

[T36] Lua：函数
来源：http://niv.52xcode.cn

function add(a, b) return a + b end
来源：http://dyb.yongpay.top

[T37] Lua：字符串拼接
来源：http://nle.jinqigufen.top

"a" .. "b"
来源：http://uft.zhijiandao.cn

[T38] Lua：条件
来源：http://bek.xinyue.icu

if x > 0 then print("正") end
来源：http://zgg.hywenlv.cn

[T39] Lua：模式匹配
来源：http://oyt.daxiang520.top

string.find(s, "%d+")
来源：http://ybf.jlsjyb.cn

[T40] Lua：元表
来源：http://ask.yongpay.top

setmetatable({}, { __index = base })
来源：http://bjr.zdqjudy.top

[T41] Perl：Hello World
来源：http://ith.hywenlv.cn

print "Hello\n";
来源：http://kcc.jinqigufen.top

[T42] Perl：变量类型
来源：http://ksk.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://utf.pengpengdd.cyou

[T43] Perl：字符串插值
来源：http://rhy.hysaishi.cn

"值: $a"
来源：http://cje.vqdsnc.cn

[T44] Perl：条件
来源：http://bmu.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://oyn.zycfv.cn

[T45] Perl：数组遍历
来源：http://rwp.vehdjk.com

for my $x (@arr) { print $x; }
来源：http://lmk.cdnleiting.top

[T46] Perl：哈希操作
来源：http://yhz.jqgufenzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mhy.meibo888.top

[T47] Perl：正则捕获
来源：http://uof.dianchejie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yzh.zhaomingkeji.xyz

[T48] Perl：正则替换
来源：http://mfc.haohaochexian.top

$s =~ s/old/new/g;
来源：http://ruj.tarul.cn

[T49] Perl：函数
来源：http://uvp.zhoulong.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aks.sysykeji.top

[T50] Perl：逐行读文件
来源：http://rki.shangyingyoupin.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vug.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://eht.cdnleiting.top

[T51] Scala：Hello World
来源：http://hgd.cdnleiting.top

println("Hello")
来源：http://rlp.52xcode.cn

[T52] Scala：变量
来源：http://gnq.zhijiandao.cn

val a = 1;  var b = 2
来源：http://uru.smart0.xyz

[T53] Scala：字符串插值
来源：http://mya.guowangkeji.top

s"值: $b"
来源：http://lsn.jinqigfzy.top

[T54] Scala：集合映射
来源：http://oix.pengpengdd.cyou

List(1, 2, 3).map(_ * 2)
来源：http://xsg.zdqjudy.top

[T55] Scala：集合过滤
来源：http://szu.pycfn.com

List(1, 2, 3).filter(_ > 1)
来源：http://vuq.52xcode.cn

[T56] Scala：样例类
来源：http://lgs.tianlin.xyz

case class User(name: String, age: Int)
来源：http://vsh.zdbjq.cn

[T57] Scala：模式匹配
来源：http://wrm.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kyn.chenzaomai.com

[T58] Scala：函数定义
来源：http://fms.gzhubu.top

def add(a: Int, b: Int): Int = a + b
来源：http://ltv.shangyingyoupin.top

[T59] Scala：循环
来源：http://htf.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://dpv.yuanzhike.top

[T60] Scala：折叠
来源：http://keb.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cgk.316326.xyz

================================================================================
来源：http://bjk.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tqq.jyoumei.cn

================================================================================
来源：http://mdz.bbcook.cn

[U01] Py：创建虚拟环境
来源：http://hwt.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://fdo.pengpengdd.cyou

[U02] Py：导出 / 安装依赖
来源：http://upi.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jnw.bbcook.cn

[U03] Py：加载 .env 配置
来源：http://drs.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vhs.ppjwa.cn

[U04] Py：变量调试打印
来源：http://gbr.aizwys.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rwl.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://sbe.yueranfly.top

list(dict.fromkeys(arr))
来源：http://hyc.sjlbkw.cn

[U06] Py：合并两个字典
来源：http://tat.bbcook.cn

{**a, **b}
来源：http://vqu.zhoulong.xyz

[U07] Py：反转字典键值
来源：http://mkr.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://jyq.zhiwuduotai.top

[U08] Py：展平二维列表
来源：http://qnc.fehbvm.com

[y for x in nested for y in x]
来源：http://cgz.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://ayu.shzxlz.cn

max(d, key=d.get)
来源：http://gcq.hammf.cn

[U10] Py：按值排序字典
来源：http://kfx.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://snp.tianlin.xyz

[U11] Py：生成器表达式
来源：http://grg.shzxlz.cn

(x * 2 for x in arr)
来源：http://kgf.zycfv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qlm.havefunace.top

Counter(arr).most_common(3)
来源：http://kqx.dashuyun.cn

[U13] Py：固定长度队列
来源：http://qir.wangdashe.top

deque(maxlen=10)
来源：http://xrc.jianghu66.top

[U14] Py：分组收集到列表
来源：http://pje.zhongyouzk.top

defaultdict(list)
来源：http://etz.zhiwuduotai.top

[U15] Py：高精度计时
来源：http://ovh.tian-w.cn

t = time.perf_counter()
来源：http://xni.cucudq.cn

[U16] Py：命令行参数解析
来源：http://ppk.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://otu.yangfankeji.com

[U17] Py：初始化日志
来源：http://gsg.chenjidiqi.icu

logging.basicConfig(level=logging.INFO)
来源：http://ioi.ybcxt.top

[U18] Py：预编译正则
来源：http://iex.tianlin.xyz

pat = re.compile(r"\d+")
来源：http://sps.zhaomingkeji.xyz

[U19] Py：正则替换带回调
来源：http://bkv.zhiwuduotai.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://byg.redwolf501.top

[U20] Py：缓存函数结果
来源：http://zwy.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://qnz.shuidangran.top


<!-- 参考信息 -->