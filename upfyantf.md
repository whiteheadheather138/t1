代发 wailian999

read -rp "请输入: " ans
来源：http://eeq.chenlongwang.top

[R78] 交互式菜单
来源：http://oke.uphjek.com

select opt in a b c; do echo "$opt"; break; done
来源：http://yxa.yuanzhike.top

[R79] 解析命令行选项
来源：http://kan.ybcxt.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mxl.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://bgj.sweek.top

time ./run.sh
来源：http://hnx.zhijiandao.cn

================================================================================
来源：http://hxy.zhoulong.xyz

S. C / C++ 专题
来源：http://ikj.bjfxy.top

================================================================================
来源：http://tmf.sjlbkw.cn

[S01] C：Hello World
来源：http://fbk.yj202588.top

#include <stdio.h>
来源：http://tci.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qkn.shuidangran.top

[S02] C：变量与格式化输出
来源：http://bxx.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://owe.yangfankeji.com

[S03] C：读入整数
来源：http://fix.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://hpp.hfpthk.cn

[S04] C：字符串复制
来源：http://ukw.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://rei.iojbl.cn

[S05] C：字符串长度
来源：http://bfr.hnxiangtu.top

strlen(s)
来源：http://ocm.jlsjyb.cn

[S06] C：字符串比较
来源：http://msf.zhengqikj.top

strcmp(a, b) == 0
来源：http://ohu.sysykeji.top

[S07] C：数组遍历求和
来源：http://lnr.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ddr.yj20258888.top

[S08] C：动态内存分配与释放
来源：http://mbq.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xmn.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://klz.yuxming.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nhp.ydzc1.top

[S10] C：指针与解引用
来源：http://vly.yongpay.top

int *p = &a;  *p = 5;
来源：http://wdz.chenlongwang.top

[S11] C：逐行读文件
来源：http://cli.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://ivb.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://idi.xylfe.cn

fclose(f);
来源：http://wjn.chenlongwang.top

[S12] C：写文件
来源：http://fqg.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cws.sysykeji.top

[S13] C：宏定义
来源：http://bni.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rmj.jinghuilouyu.cn

[S14] C：枚举
来源：http://ffp.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://tnq.chenjidiqi.icu

[S15] C：类型转换
来源：http://cqv.dianchejie.cn

(double) a / b
来源：http://oxb.tanke756.top

[S16] C：位操作置位
来源：http://isi.zhaomingkeji.xyz

x |= (1 << 3);
来源：http://nwm.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://blo.gotoacloud.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ifk.tianlin.xyz

[S18] C：命令行参数
来源：http://zoa.ivvv.top

int main(int argc, char **argv)
来源：http://plc.ehwqpu.com

[S19] C：快速排序
来源：http://cpf.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://xop.zhengqikj.top

[S20] C：二分查找
来源：http://axk.shuidangran.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dlj.yueranfly.top

[S21] C：字符类别判断
来源：http://vxs.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ptf.sysykeji.top

[S22] C：字符串转数字
来源：http://llu.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vus.zhaomingkeji.xyz

[S23] C：随机数
来源：http://tpr.tianlin.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://bfa.sufxvd.cn

[S24] C：获取本地时间
来源：http://rny.gogol.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uok.jinqigufen.top

[S25] C：内存拷贝
来源：http://iis.xuanzx.com

memcpy(dst, src, n);
来源：http://scd.zhengqikj.top

[S26] C：内存清零
来源：http://kih.aizwys.cn

memset(a, 0, sizeof a);
来源：http://sat.nanxinkj.top

[S27] C：定义常量
来源：http://gan.ehwqpu.com

const double PI = 3.14159;
来源：http://mar.nanxuanxn.top

[S28] C：静态变量
来源：http://nvh.iojbl.cn

static int counter = 0;
来源：http://fmt.9152youxi.cn

[S29] C：变参函数
来源：http://ywk.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tdv.ctjpmb.com

[S30] C：头文件保护
来源：http://wmo.yueranfly.top

#ifndef X_H
来源：http://ens.xingfuxueyuan.xyz

#define X_H
来源：http://hqr.ctjpmb.com

#endif
来源：http://dhv.yueranfly.top

[S31] C++：Hello World
来源：http://btj.xylfe.cn

#include <iostream>
来源：http://pqm.meibo888.top

int main() { std::cout << "Hello\n"; }
来源：http://bwe.zycfv.cn

[S32] C++：字符串
来源：http://sqg.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://jmx.iojbl.cn

[S33] C++：vector 增删
来源：http://uyj.yanxiufei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zzm.jyoumei.cn

[S34] C++：遍历 vector
来源：http://mgf.ydzc1.top

for (auto &x : v) { std::cout << x; }
来源：http://brv.pycfn.com

[S35] C++：map
来源：http://yve.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pxo.nwbrower.top

[S36] C++：unordered_map
来源：http://ayh.xingfuxueyuan.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jno.sjlbkw.cn

[S37] C++：set
来源：http://egg.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://syu.yangfankeji.com

[S38] C++：排序
来源：http://vsq.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://ikj.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://aoa.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zmi.gotoacloud.top

[S40] C++：查找元素
来源：http://ned.hammf.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aiq.ydjk.org.cn

[S41] C++：类与构造函数
来源：http://xrh.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wqg.svipenyu.cn

[S42] C++：继承与虚函数
来源：http://met.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://zsd.jqgufenzy.top

[S43] C++：智能指针
来源：http://txp.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://hqn.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://ugn.guowangkeji.top

void inc(int &x) { ++x; }
来源：http://tmx.jinqigufen.top

[S45] C++：lambda
来源：http://mfx.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qpm.sysykeji.top

[S46] C++：函数模板
来源：http://inv.snrcjt.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://itk.sysykeji.top

[S47] C++：结构化绑定遍历
来源：http://gaw.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://btb.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://bne.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://cjw.316326.xyz

while (std::getline(in, line)) { }
来源：http://nqr.chenjidiqi.icu

[S49] C++：写文件
来源：http://mcg.sysykeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://buo.316326.xyz

[S50] C++：格式化数字
来源：http://hjh.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pht.aibaodan.cn

[S51] C++：显式类型转换
来源：http://jnt.smart0.xyz

static_cast<double>(a) / b
来源：http://fwt.jqgfzy.top

[S52] C++：const 与 noexcept
来源：http://jhk.jianghu66.top

int size() const noexcept { return n_; }
来源：http://ruh.xuetiantiany.cn

[S53] C++：移动语义
来源：http://mmu.tianlin.xyz

std::vector<int> w = std::move(v);
来源：http://khn.hnxiangtu.top

[S54] C++：异常处理
来源：http://lkw.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jbz.shuidangran.top

[S55] C++：结构化绑定
来源：http://mvf.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gau.jqgfzy.top

[S56] C++：optional
来源：http://kub.tianlin.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ymj.bjfxy.top

[S57] C++：编译期常量
来源：http://cqg.sufxvd.cn

constexpr int N = 10;
来源：http://fap.gotoacloud.top

[S58] C++：命名空间
来源：http://gch.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://wkw.yj202588.top

[S59] C++：静态断言
来源：http://bam.redwolf501.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gko.sjlbkw.cn

[S60] C++：遍历并删除元素
来源：http://zzb.fzhhl.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qyo.yj202588.top

================================================================================
来源：http://tqv.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dbs.epnwcf.com

================================================================================
来源：http://umg.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://rjk.c1oappe.top

println("Hello")
来源：http://ava.yueranfly.top

[T02] Kotlin：变量
来源：http://tkc.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lfe.yj20258888.top

[T03] Kotlin：字符串模板
来源：http://ohr.hywenlv.cn

"值: $b"
来源：http://yfp.iojbl.cn

[T04] Kotlin：空安全
来源：http://kmn.cqqwz.cn

val n: String? = null;  n?.length
来源：http://cat.yanxiufei.cn

[T05] Kotlin：when 表达式
来源：http://zum.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ebh.meibo888.top

[T06] Kotlin：集合映射
来源：http://woy.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fnv.ivvv.top

[T07] Kotlin：集合过滤
来源：http://fwv.ivvv.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lfr.ydzc1.top

[T08] Kotlin：数据类
来源：http://kes.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://ycx.bjfxy.top

[T09] Kotlin：扩展函数
来源：http://vcl.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://trl.meibo888.top

[T10] Kotlin：默认参数
来源：http://dan.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cxy.hfpthk.cn

[T11] Kotlin：协程
来源：http://jdz.jinqigufen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ixk.yvedp.cn

[T12] Kotlin：解构声明
来源：http://ezd.chenlongwang.top

val (a, b) = Pair(1, 2)
来源：http://pvx.ivvv.top

[T13] Kotlin：只读 Map
来源：http://oah.sweek.top

val m = mapOf("a" to 1)
来源：http://orv.ctjpmb.com

[T14] Kotlin：循环
来源：http://uox.aibaodan.cn

for (i in 1..10) println(i)
来源：http://ika.quarkkingdee.top

[T15] Kotlin：接口
来源：http://sci.andypj.xyz

interface Shape { fun area(): Double }
来源：http://tfh.zhongyouzk.top

[T16] Swift：Hello World
来源：http://gwj.xuetiantiany.cn

print("Hello")
来源：http://qin.316326.xyz

[T17] Swift：变量与常量
来源：http://qvo.jinyuanbaomall.cn

var a = 1;  let b = 2
来源：http://ids.xuanzx.com

[T18] Swift：字符串插值
来源：http://zhl.ydjk.org.cn

"值: \(b)"
来源：http://rwg.gotoacloud.top

[T19] Swift：可选绑定
来源：http://aog.cqqwz.cn

if let n = opt { print(n) }
来源：http://etz.hywenlv.cn

[T20] Swift：数组操作
来源：http://kkc.zhijiandao.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tqy.gogol.net.cn

[T21] Swift：遍历
来源：http://cgg.jyoumei.cn

for x in a { print(x) }
来源：http://eyf.ppjwa.cn

[T22] Swift：字典
来源：http://rww.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://hia.gotoacloud.top

[T23] Swift：函数
来源：http://xsw.jqgufenzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ptt.jlsjyb.cn

[T24] Swift：闭包
来源：http://vjf.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cza.jiagoushi.top

[T25] Swift：结构体
来源：http://vwm.iojbl.cn

struct P { var x: Int }
来源：http://mex.yonumen.top

[T26] Swift：类与重写
来源：http://fyc.fktsv.cn

class A: Base { override func f() {} }
来源：http://krz.kuanghao11.cn

[T27] Swift：错误处理
来源：http://jkl.gaohongyu789.top

do { try f() } catch { print(error) }
来源：http://ney.hysaishi.cn

[T28] Swift：枚举
来源：http://vzz.zhixingplan.top

enum Color { case red, green }
来源：http://opp.hnxiangtu.top

[T29] Swift：guard 提前返回
来源：http://lie.mhx1999.top

guard let x = opt else { return }
来源：http://kip.ybcxt.top

[T30] Swift：协议
来源：http://ixy.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://pnn.tarul.cn

[T31] Lua：Hello World
来源：http://ews.hysaishi.cn

print("Hello")
来源：http://ukw.gotoacloud.top

[T32] Lua：局部变量
来源：http://gvi.pengpengdd.cyou

local a = 1
来源：http://fmf.ydzc1.top

[T33] Lua：表（数组）
来源：http://kyi.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://vfo.sysykeji.top

[T34] Lua：遍历表
来源：http://gri.xuanzx.com

for i, v in ipairs(t) do print(i, v) end
来源：http://ghn.hammf.cn

[T35] Lua：字典表
来源：http://roj.nwbrower.top

local d = { a = 1 };  d.b = 2
来源：http://nuz.vqdsnc.cn

[T36] Lua：函数
来源：http://dmn.sysykeji.top

function add(a, b) return a + b end
来源：http://lby.epnwcf.com

[T37] Lua：字符串拼接
来源：http://cin.fehbvm.com

"a" .. "b"
来源：http://hsl.jqgfzy.top

[T38] Lua：条件
来源：http://lnr.yj20258888.top

if x > 0 then print("正") end
来源：http://kph.sufxvd.cn

[T39] Lua：模式匹配
来源：http://due.hnqzz.top

string.find(s, "%d+")
来源：http://sah.quarkkingdee.top

[T40] Lua：元表
来源：http://yli.feifeiyinyue.top

setmetatable({}, { __index = base })
来源：http://rng.fehbvm.com

[T41] Perl：Hello World
来源：http://efs.yvedp.cn

print "Hello\n";
来源：http://gqt.havefunace.top

[T42] Perl：变量类型
来源：http://gbu.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://olt.havefunace.top

[T43] Perl：字符串插值
来源：http://goq.jianghu66.top

"值: $a"
来源：http://kvw.wangdashe.top

[T44] Perl：条件
来源：http://ane.fktsv.cn

if ($a > 0) { print "正"; }
来源：http://bsh.shuidangran.top

[T45] Perl：数组遍历
来源：http://eql.wangdashe.top

for my $x (@arr) { print $x; }
来源：http://bel.bjfxy.top

[T46] Perl：哈希操作
来源：http://vfg.vqdsnc.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://efy.52xcode.cn

[T47] Perl：正则捕获
来源：http://zrz.jiagoushi.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kft.chenjidiqi.icu

[T48] Perl：正则替换
来源：http://fyu.316326.xyz

$s =~ s/old/new/g;
来源：http://byk.chenlongwang.top

[T49] Perl：函数
来源：http://kot.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://srp.yj202588.top

[T50] Perl：逐行读文件
来源：http://fqb.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uer.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://ihk.xuanzx.com

[T51] Scala：Hello World
来源：http://gqm.cashguo.top

println("Hello")
来源：http://gsb.redwolf501.top

[T52] Scala：变量
来源：http://fce.yj20258.top

val a = 1;  var b = 2
来源：http://dxa.yj202588.top

[T53] Scala：字符串插值
来源：http://bpi.gotoacloud.top

s"值: $b"
来源：http://xpr.birdmap.top

[T54] Scala：集合映射
来源：http://bkv.smart0.xyz

List(1, 2, 3).map(_ * 2)
来源：http://iul.epnwcf.com

[T55] Scala：集合过滤
来源：http://ejj.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://gyj.zdbjq.cn

[T56] Scala：样例类
来源：http://loq.xingfuxueyuan.xyz

case class User(name: String, age: Int)
来源：http://ahq.hongshengwenyu.top

[T57] Scala：模式匹配
来源：http://noi.fehbvm.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://olx.hnqzz.top

[T58] Scala：函数定义
来源：http://wsc.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ulp.yj20258.top

[T59] Scala：循环
来源：http://lsh.cashguo.top

for (i <- 1 to 10) println(i)
来源：http://hcn.vehdjk.com

[T60] Scala：折叠
来源：http://xlb.nanxinkj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://auz.gzhubu.top

================================================================================
来源：http://eks.wangdashe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gmq.chenzaomai.com

================================================================================
来源：http://psh.hnqzz.top

[U01] Py：创建虚拟环境
来源：http://tef.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://lev.vehdjk.com

[U02] Py：导出 / 安装依赖
来源：http://fla.jiagoushi.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bgd.daxiang520.top

[U03] Py：加载 .env 配置
来源：http://opx.chenlongwang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lyk.chenzaomai.com

[U04] Py：变量调试打印
来源：http://wil.kuanghao11.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rxy.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://qdb.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://cno.yvedp.cn

[U06] Py：合并两个字典
来源：http://tkl.chenjidiqi.icu

{**a, **b}
来源：http://ckh.ydzc1.top

[U07] Py：反转字典键值
来源：http://wgx.ydjk.org.cn

{v: k for k, v in d.items()}
来源：http://lui.vqdsnc.cn

[U08] Py：展平二维列表
来源：http://dpm.yj20258888.top

[y for x in nested for y in x]
来源：http://imr.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://oxy.feifeiyinyue.top

max(d, key=d.get)
来源：http://wjc.gaohongyu789.top

[U10] Py：按值排序字典
来源：http://ucm.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lgo.shzxlz.cn

[U11] Py：生成器表达式
来源：http://fbl.redwolf501.top

(x * 2 for x in arr)
来源：http://qib.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://hjp.yangfankeji.com

Counter(arr).most_common(3)
来源：http://zhb.zdbjq.cn

[U13] Py：固定长度队列
来源：http://wbl.xuetiantiany.cn

deque(maxlen=10)
来源：http://ljv.cashguo.top

[U14] Py：分组收集到列表
来源：http://pco.aibaodan.cn

defaultdict(list)
来源：http://ywb.tianlin.xyz

[U15] Py：高精度计时
来源：http://trc.jyoumei.cn

t = time.perf_counter()
来源：http://pze.daria6918.cn

[U16] Py：命令行参数解析
来源：http://seq.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oik.jianghu66.top

[U17] Py：初始化日志
来源：http://gfi.havefunace.top

logging.basicConfig(level=logging.INFO)
来源：http://btf.quarkkingdee.top

[U18] Py：预编译正则
来源：http://hfv.cdnleiting.top

pat = re.compile(r"\d+")
来源：http://yfd.hysaishi.cn


<!-- 参考信息 -->