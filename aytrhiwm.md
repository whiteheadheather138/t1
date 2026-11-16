代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ilx.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://qyu.jlsjyb.cn

time ./run.sh
来源：http://tms.cdnleiting.top

================================================================================
来源：http://pfm.sysykeji.top

S. C / C++ 专题
来源：http://zhb.zdqjudy.top

================================================================================
来源：http://uiq.dashuyun.cn

[S01] C：Hello World
来源：http://jly.yangfankeji.com

#include <stdio.h>
来源：http://yjt.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qvm.tarul.cn

[S02] C：变量与格式化输出
来源：http://olh.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://mcw.quarkkingdee.top

[S03] C：读入整数
来源：http://atf.yuanzhike.top

int x; scanf("%d", &x);
来源：http://fph.zdbjq.cn

[S04] C：字符串复制
来源：http://jmn.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ifs.shuidangran.top

[S05] C：字符串长度
来源：http://shd.fzhhl.top

strlen(s)
来源：http://qgv.dianchejie.cn

[S06] C：字符串比较
来源：http://fsk.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://gpu.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://mvu.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vpl.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://bkx.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rlx.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://lwl.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cmz.guowangkeji.top

[S10] C：指针与解引用
来源：http://ktp.52xcode.cn

int *p = &a;  *p = 5;
来源：http://set.jqgfzy.top

[S11] C：逐行读文件
来源：http://ujf.uphjek.com

FILE *f = fopen("a.txt", "r");
来源：http://jqn.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iwg.9152youxi.cn

fclose(f);
来源：http://rqr.chenlongwang.top

[S12] C：写文件
来源：http://suz.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vmq.316326.xyz

[S13] C：宏定义
来源：http://hnt.cqqwz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lrk.zdqjudy.top

[S14] C：枚举
来源：http://rmk.vehdjk.com

enum Color { RED, GREEN, BLUE };
来源：http://dll.hongshengwenyu.top

[S15] C：类型转换
来源：http://hio.hammf.cn

(double) a / b
来源：http://hjp.zdbjq.cn

[S16] C：位操作置位
来源：http://zed.pycfn.com

x |= (1 << 3);
来源：http://iqz.yuxming.cn

[S17] C：安全拼接字符串
来源：http://wvk.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oqd.gaohongyu789.top

[S18] C：命令行参数
来源：http://tyq.ctjpmb.com

int main(int argc, char **argv)
来源：http://mza.yangfankeji.com

[S19] C：快速排序
来源：http://tao.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://guy.nanxinkj.top

[S20] C：二分查找
来源：http://opk.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hux.bjfxy.top

[S21] C：字符类别判断
来源：http://fbw.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fka.iojbl.cn

[S22] C：字符串转数字
来源：http://nuq.chenzaomai.com

atoi("42");  strtod("3.14", NULL);
来源：http://fjl.pycfn.com

[S23] C：随机数
来源：http://wph.0kj1m.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kuy.hfpthk.cn

[S24] C：获取本地时间
来源：http://odn.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rni.haohaochexian.top

[S25] C：内存拷贝
来源：http://vqb.yanxiufei.cn

memcpy(dst, src, n);
来源：http://nhz.cheryme.top

[S26] C：内存清零
来源：http://xwr.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://psz.yueranfly.top

[S27] C：定义常量
来源：http://fig.birdmap.top

const double PI = 3.14159;
来源：http://mbl.zdqjudy.top

[S28] C：静态变量
来源：http://umm.wangdashe.top

static int counter = 0;
来源：http://upd.epnwcf.com

[S29] C：变参函数
来源：http://zie.jinqigufen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lyn.ppjwa.cn

[S30] C：头文件保护
来源：http://jda.yvedp.cn

#ifndef X_H
来源：http://ivl.yvedp.cn

#define X_H
来源：http://cwd.yanxiufei.cn

#endif
来源：http://jxs.zhiwuduotai.top

[S31] C++：Hello World
来源：http://pwk.jqgfzy.top

#include <iostream>
来源：http://mfc.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://hzm.tian-w.cn

[S32] C++：字符串
来源：http://uhv.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://jvy.zhengqikj.top

[S33] C++：vector 增删
来源：http://bnp.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hwn.cqqwz.cn

[S34] C++：遍历 vector
来源：http://uvw.ydzc1.top

for (auto &x : v) { std::cout << x; }
来源：http://fmf.316326.xyz

[S35] C++：map
来源：http://cba.zhaomingkeji.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fir.yj202588.top

[S36] C++：unordered_map
来源：http://bzn.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qqs.daria6918.cn

[S37] C++：set
来源：http://ack.aibaodan.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pid.meibo888.top

[S38] C++：排序
来源：http://sdj.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://bki.hysaishi.cn

[S39] C++：自定义比较器排序
来源：http://ehe.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lpd.hongshengwenyu.top

[S40] C++：查找元素
来源：http://hnu.epnwcf.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yol.vehdjk.com

[S41] C++：类与构造函数
来源：http://xct.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zod.hnqzz.top

[S42] C++：继承与虚函数
来源：http://bjt.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://gqh.hesvh.cn

[S43] C++：智能指针
来源：http://hdk.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://jpg.zhoulong.xyz

[S44] C++：引用传参
来源：http://bah.yj20258.top

void inc(int &x) { ++x; }
来源：http://fbd.chenjidiqi.icu

[S45] C++：lambda
来源：http://uru.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://ebj.cucudq.cn

[S46] C++：函数模板
来源：http://yky.fehbvm.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kus.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://fwj.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://twi.tanke756.top

[S48] C++：逐行读文件
来源：http://uhv.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://jwo.xinyue.icu

while (std::getline(in, line)) { }
来源：http://kyy.iojbl.cn

[S49] C++：写文件
来源：http://wwd.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sqo.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://xzn.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mzq.dianchejie.cn

[S51] C++：显式类型转换
来源：http://zlb.c1oappe.top

static_cast<double>(a) / b
来源：http://uud.xinyue.icu

[S52] C++：const 与 noexcept
来源：http://zxt.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://fxj.dashuyun.cn

[S53] C++：移动语义
来源：http://awr.jqgfzy.top

std::vector<int> w = std::move(v);
来源：http://cob.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://umv.yonumen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rxi.cdnleiting.top

[S55] C++：结构化绑定
来源：http://xux.birdmap.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cjw.zhaomingkeji.xyz

[S56] C++：optional
来源：http://jlp.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wmr.iojbl.cn

[S57] C++：编译期常量
来源：http://uzm.meibo888.top

constexpr int N = 10;
来源：http://yvt.jqgfzy.top

[S58] C++：命名空间
来源：http://cqe.jinyuanbaomall.cn

namespace ns { int f() { return 1; } }
来源：http://ahs.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://oui.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tkn.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://cfd.tanke756.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bwq.sufxvd.cn

================================================================================
来源：http://ypy.zhaomingkeji.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kvo.xziqi.cn

================================================================================
来源：http://pyt.jqgufenzy.top

[T01] Kotlin：Hello World
来源：http://lvk.hesvh.cn

println("Hello")
来源：http://xhm.yfazqb.com

[T02] Kotlin：变量
来源：http://slq.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yom.nwbrower.top

[T03] Kotlin：字符串模板
来源：http://hin.chenlongwang.top

"值: $b"
来源：http://vqy.vehdjk.com

[T04] Kotlin：空安全
来源：http://vtj.hesvh.cn

val n: String? = null;  n?.length
来源：http://ubb.sysykeji.top

[T05] Kotlin：when 表达式
来源：http://qat.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tuv.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://krw.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gio.gogol.net.cn

[T07] Kotlin：集合过滤
来源：http://gsu.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://lex.nwbrower.top

[T08] Kotlin：数据类
来源：http://zyi.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://cys.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://vkn.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://xxb.xinyue.icu

[T10] Kotlin：默认参数
来源：http://ozr.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kon.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://vmb.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://kro.meibo888.top

[T12] Kotlin：解构声明
来源：http://htq.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://eug.yonumen.top

[T13] Kotlin：只读 Map
来源：http://lnh.daria6918.cn

val m = mapOf("a" to 1)
来源：http://zzu.meibo888.top

[T14] Kotlin：循环
来源：http://qpw.zdbjq.cn

for (i in 1..10) println(i)
来源：http://zol.ydzc1.top

[T15] Kotlin：接口
来源：http://lrf.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://hau.chenjidiqi.icu

[T16] Swift：Hello World
来源：http://tkg.hfpthk.cn

print("Hello")
来源：http://cpx.sweek.top

[T17] Swift：变量与常量
来源：http://hak.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://yuc.yfazqb.com

[T18] Swift：字符串插值
来源：http://fwl.jyoumei.cn

"值: \(b)"
来源：http://udt.yonumen.top

[T19] Swift：可选绑定
来源：http://sfz.gogol.net.cn

if let n = opt { print(n) }
来源：http://cuh.tianlin.xyz

[T20] Swift：数组操作
来源：http://cun.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://aer.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://qtq.chenzaomai.com

for x in a { print(x) }
来源：http://pzk.jlsjyb.cn

[T22] Swift：字典
来源：http://lfk.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dej.ppjwa.cn

[T23] Swift：函数
来源：http://sep.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qsb.sjlbkw.cn

[T24] Swift：闭包
来源：http://luk.wangshuangyany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ktv.52xcode.cn

[T25] Swift：结构体
来源：http://jfb.guowangkeji.top

struct P { var x: Int }
来源：http://eyw.zhijiandao.cn

[T26] Swift：类与重写
来源：http://wpr.xuanzx.com

class A: Base { override func f() {} }
来源：http://gvm.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://hhy.yangfankeji.com

do { try f() } catch { print(error) }
来源：http://uqy.gzhubu.top

[T28] Swift：枚举
来源：http://mll.xziqi.cn

enum Color { case red, green }
来源：http://jsn.zhijiandao.cn

[T29] Swift：guard 提前返回
来源：http://two.fzhhl.top

guard let x = opt else { return }
来源：http://lcq.yj202588.top

[T30] Swift：协议
来源：http://kze.hcnkem.com

protocol Shape { func area() -> Double }
来源：http://qqc.havefunace.top

[T31] Lua：Hello World
来源：http://hqy.gotoacloud.top

print("Hello")
来源：http://wmj.xingfuxueyuan.xyz

[T32] Lua：局部变量
来源：http://jyj.guowangkeji.top

local a = 1
来源：http://dsh.0kj1m.cn

[T33] Lua：表（数组）
来源：http://gyd.hammf.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://atq.vehdjk.com

[T34] Lua：遍历表
来源：http://sng.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://idx.aibaodan.cn

[T35] Lua：字典表
来源：http://xjg.zhiwuduotai.top

local d = { a = 1 };  d.b = 2
来源：http://brf.kuanghao11.cn

[T36] Lua：函数
来源：http://ena.vehdjk.com

function add(a, b) return a + b end
来源：http://spb.yj20258.top

[T37] Lua：字符串拼接
来源：http://fal.ctjpmb.com

"a" .. "b"
来源：http://rsz.sxryk.cn

[T38] Lua：条件
来源：http://wna.gogol.net.cn

if x > 0 then print("正") end
来源：http://myf.daxiang520.top

[T39] Lua：模式匹配
来源：http://fsp.gotoacloud.top

string.find(s, "%d+")
来源：http://yyz.sjlbkw.cn

[T40] Lua：元表
来源：http://aof.quarkkingdee.top

setmetatable({}, { __index = base })
来源：http://nel.jinqigufen.top

[T41] Perl：Hello World
来源：http://bwx.wangshuangyany.cn

print "Hello\n";
来源：http://yvd.316326.xyz

[T42] Perl：变量类型
来源：http://vwo.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://olc.yongpay.top

[T43] Perl：字符串插值
来源：http://abd.zhengqikj.top

"值: $a"
来源：http://pnu.ybcxt.top

[T44] Perl：条件
来源：http://rsu.havefunace.top

if ($a > 0) { print "正"; }
来源：http://fpw.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://ppu.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://hyh.andypj.xyz

[T46] Perl：哈希操作
来源：http://qpc.ppjwa.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jsc.nanxinkj.top

[T47] Perl：正则捕获
来源：http://dtz.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://oop.dashuyun.cn

[T48] Perl：正则替换
来源：http://kjg.gaohongyu789.top

$s =~ s/old/new/g;
来源：http://bwx.sxryk.cn

[T49] Perl：函数
来源：http://afi.ydzc1.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oum.yuanzhike.top

[T50] Perl：逐行读文件
来源：http://fxl.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fhp.zhengqikj.top

while (my $line = <$fh>) { print $line; }
来源：http://lyo.chenzaomai.com

[T51] Scala：Hello World
来源：http://bft.ywan-chungtsiang.top

println("Hello")
来源：http://kkn.xingfuxueyuan.xyz

[T52] Scala：变量
来源：http://acp.sjlbkw.cn

val a = 1;  var b = 2
来源：http://sjy.zhengqikj.top

[T53] Scala：字符串插值
来源：http://uhz.dianchejie.cn

s"值: $b"
来源：http://rxm.c1oappe.top

[T54] Scala：集合映射
来源：http://ltg.sufxvd.cn

List(1, 2, 3).map(_ * 2)
来源：http://okw.sxryk.cn

[T55] Scala：集合过滤
来源：http://otq.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gks.hongshengwenyu.top

[T56] Scala：样例类
来源：http://hlp.tanke756.top

case class User(name: String, age: Int)
来源：http://rxj.hnqzz.top

[T57] Scala：模式匹配
来源：http://tpj.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://urn.yvedp.cn

[T58] Scala：函数定义
来源：http://zai.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://wfa.sysykeji.top

[T59] Scala：循环
来源：http://wvx.9152youxi.cn

for (i <- 1 to 10) println(i)
来源：http://vda.dianchejie.cn

[T60] Scala：折叠
来源：http://odr.daria6918.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xln.hfpthk.cn

================================================================================
来源：http://frb.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ncb.shzxlz.cn

================================================================================
来源：http://yhs.gzhubu.top

[U01] Py：创建虚拟环境
来源：http://cpp.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://uej.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://gpf.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://djz.xuetiantiany.cn

[U03] Py：加载 .env 配置
来源：http://wrw.yvedp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sua.zdqjudy.top

[U04] Py：变量调试打印
来源：http://pfq.yvedp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mdz.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://ouk.zycfv.cn

list(dict.fromkeys(arr))
来源：http://szn.jqgfzy.top

[U06] Py：合并两个字典
来源：http://yrl.yanxiufei.cn

{**a, **b}
来源：http://euf.gogol.net.cn

[U07] Py：反转字典键值
来源：http://rvm.uphjek.com

{v: k for k, v in d.items()}
来源：http://qdy.mhx1999.top

[U08] Py：展平二维列表
来源：http://grz.fanxiaobao.xyz

[y for x in nested for y in x]
来源：http://oya.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://dlm.smart0.xyz

max(d, key=d.get)
来源：http://djj.cqqwz.cn

[U10] Py：按值排序字典
来源：http://mcr.dashuyun.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sze.9152youxi.cn

[U11] Py：生成器表达式
来源：http://kel.cqqwz.cn

(x * 2 for x in arr)
来源：http://ijl.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fsq.chenzaomai.com

Counter(arr).most_common(3)
来源：http://fqc.xuanzx.com

[U13] Py：固定长度队列
来源：http://siz.52xcode.cn

deque(maxlen=10)
来源：http://mva.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://pmz.xziqi.cn

defaultdict(list)
来源：http://hsd.ywan-chungtsiang.top

[U15] Py：高精度计时
来源：http://exn.haohaochexian.top

t = time.perf_counter()
来源：http://niz.jyoumei.cn

[U16] Py：命令行参数解析
来源：http://vyy.tanke756.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://smz.hesvh.cn

[U17] Py：初始化日志
来源：http://rup.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://wgj.fktsv.cn

[U18] Py：预编译正则
来源：http://azi.uphjek.com

pat = re.compile(r"\d+")
来源：http://tzv.gzhubu.top

[U19] Py：正则替换带回调
来源：http://div.jlsjyb.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pbh.andypj.xyz

[U20] Py：缓存函数结果
来源：http://wsb.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://gzw.svipenyu.cn


<!-- 参考信息 -->