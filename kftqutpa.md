代发 wailian999

split -l 1000 big.log part_
来源：http://xwx.ppjwa.cn

[R74] 批量重命名
来源：http://olo.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gle.cucudq.cn

[R75] 导出环境变量
来源：http://jhj.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://uoh.nwbrower.top

[R76] 使用临时文件
来源：http://rqi.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iyi.snrcjt.cn

[R77] 读取用户输入
来源：http://acq.tarul.cn

read -rp "请输入: " ans
来源：http://hhr.gotoacloud.top

[R78] 交互式菜单
来源：http://rrw.ywan-chungtsiang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uuv.cqqwz.cn

[R79] 解析命令行选项
来源：http://soj.yongpay.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rqz.ehwqpu.com

[R80] 查看脚本执行耗时
来源：http://rfw.jiagoushi.top

time ./run.sh
来源：http://eoo.ybcxt.top

================================================================================
来源：http://jgx.chenzaomai.com

S. C / C++ 专题
来源：http://emy.xziqi.cn

================================================================================
来源：http://puw.daxiang520.top

[S01] C：Hello World
来源：http://scu.iojbl.cn

#include <stdio.h>
来源：http://qsy.xinyue.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://map.quarkkingdee.top

[S02] C：变量与格式化输出
来源：http://tkz.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://crb.wangshuangyany.cn

[S03] C：读入整数
来源：http://wmg.gzhubu.top

int x; scanf("%d", &x);
来源：http://ipt.jqgufenzy.top

[S04] C：字符串复制
来源：http://eyq.daxiang520.top

char dst[32]; strcpy(dst, "hi");
来源：http://lgv.fehbvm.com

[S05] C：字符串长度
来源：http://roa.yuxming.cn

strlen(s)
来源：http://vev.hfpthk.cn

[S06] C：字符串比较
来源：http://zjr.hfpthk.cn

strcmp(a, b) == 0
来源：http://ccx.aibaodan.cn

[S07] C：数组遍历求和
来源：http://cdv.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cqn.quarkkingdee.top

[S08] C：动态内存分配与释放
来源：http://xmp.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pae.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://sqp.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://znf.yfazqb.com

[S10] C：指针与解引用
来源：http://cfe.hammf.cn

int *p = &a;  *p = 5;
来源：http://afz.gzhubu.top

[S11] C：逐行读文件
来源：http://ozn.yj202588.top

FILE *f = fopen("a.txt", "r");
来源：http://oep.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hsf.yj20258888.top

fclose(f);
来源：http://wft.cheryme.top

[S12] C：写文件
来源：http://ezh.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mtm.kuanghao11.cn

[S13] C：宏定义
来源：http://unj.xingfuxueyuan.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nez.xylfe.cn

[S14] C：枚举
来源：http://nfv.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://mqx.hcnkem.com

[S15] C：类型转换
来源：http://sld.c1oappe.top

(double) a / b
来源：http://pei.wangshuangyany.cn

[S16] C：位操作置位
来源：http://ast.guannengcc.top

x |= (1 << 3);
来源：http://hmu.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://laa.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nhx.fzhhl.top

[S18] C：命令行参数
来源：http://ozd.wangdashe.top

int main(int argc, char **argv)
来源：http://chc.52xcode.cn

[S19] C：快速排序
来源：http://qch.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://hnp.sysykeji.top

[S20] C：二分查找
来源：http://xmt.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mqf.cucudq.cn

[S21] C：字符类别判断
来源：http://ktt.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dlo.uphjek.com

[S22] C：字符串转数字
来源：http://gkz.jinqigfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://ltz.guowangkeji.top

[S23] C：随机数
来源：http://ecy.nwbrower.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wzw.fktsv.cn

[S24] C：获取本地时间
来源：http://jcl.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://swc.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://ksh.tarul.cn

memcpy(dst, src, n);
来源：http://nyi.ydzc1.top

[S26] C：内存清零
来源：http://vtu.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://jxk.svipenyu.cn

[S27] C：定义常量
来源：http://shb.jyoumei.cn

const double PI = 3.14159;
来源：http://nxl.yanxiufei.cn

[S28] C：静态变量
来源：http://few.jinqigfzy.top

static int counter = 0;
来源：http://hfw.cucudq.cn

[S29] C：变参函数
来源：http://ols.xuetiantiany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://whq.dianchejie.cn

[S30] C：头文件保护
来源：http://fzk.fzhhl.top

#ifndef X_H
来源：http://zlq.shanyushiyangtech.top

#define X_H
来源：http://weg.fehbvm.com

#endif
来源：http://rqy.hammf.cn

[S31] C++：Hello World
来源：http://bur.hysaishi.cn

#include <iostream>
来源：http://trz.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://pfg.yvedp.cn

[S32] C++：字符串
来源：http://xtj.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://jlp.jyoumei.cn

[S33] C++：vector 增删
来源：http://geo.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://loc.zhixingplan.top

[S34] C++：遍历 vector
来源：http://sjd.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://ire.xingfuxueyuan.xyz

[S35] C++：map
来源：http://gdu.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uva.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://rhr.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rkq.pengpengdd.cyou

[S37] C++：set
来源：http://suo.hnxiangtu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://otf.ywan-chungtsiang.top

[S38] C++：排序
来源：http://jeg.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://leo.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://bgt.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vuv.sweek.top

[S40] C++：查找元素
来源：http://ddl.52xcode.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qav.chenzaomai.com

[S41] C++：类与构造函数
来源：http://jox.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qfb.iojbl.cn

[S42] C++：继承与虚函数
来源：http://wco.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://krd.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://fra.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://uwf.sysykeji.top

[S44] C++：引用传参
来源：http://lmh.xinyue.icu

void inc(int &x) { ++x; }
来源：http://vcd.yj20258888.top

[S45] C++：lambda
来源：http://chc.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ybp.jlsjyb.cn

[S46] C++：函数模板
来源：http://uyt.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mzk.sjlbkw.cn

[S47] C++：结构化绑定遍历
来源：http://vbi.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dcj.sxryk.cn

[S48] C++：逐行读文件
来源：http://jvr.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://ogj.yfazqb.com

while (std::getline(in, line)) { }
来源：http://wzf.andypj.xyz

[S49] C++：写文件
来源：http://mcg.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bfp.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://kdz.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://abn.smart0.xyz

[S51] C++：显式类型转换
来源：http://xnb.snrcjt.cn

static_cast<double>(a) / b
来源：http://mra.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://yjr.guannengcc.top

int size() const noexcept { return n_; }
来源：http://fld.jyoumei.cn

[S53] C++：移动语义
来源：http://lvh.hesvh.cn

std::vector<int> w = std::move(v);
来源：http://vdp.jinqigfzy.top

[S54] C++：异常处理
来源：http://qys.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vsc.nanxinkj.top

[S55] C++：结构化绑定
来源：http://get.hnqzz.top

auto [a, b] = std::make_pair(1, 2);
来源：http://sgz.hcnkem.com

[S56] C++：optional
来源：http://zgy.gogol.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mat.sxryk.cn

[S57] C++：编译期常量
来源：http://pdz.ydzc1.top

constexpr int N = 10;
来源：http://lbv.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://uga.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://fax.cucudq.cn

[S59] C++：静态断言
来源：http://ehl.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ply.zhongyouzk.top

[S60] C++：遍历并删除元素
来源：http://kar.epnwcf.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hpe.aizwys.cn

================================================================================
来源：http://shz.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gbr.shuidangran.top

================================================================================
来源：http://msk.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://wor.sysykeji.top

println("Hello")
来源：http://vul.fengsongda.top

[T02] Kotlin：变量
来源：http://slh.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gkb.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://flq.zhijiandao.cn

"值: $b"
来源：http://say.hywenlv.cn

[T04] Kotlin：空安全
来源：http://nfv.zdqjudy.top

val n: String? = null;  n?.length
来源：http://ply.bbcook.cn

[T05] Kotlin：when 表达式
来源：http://jot.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wyq.yueranfly.top

[T06] Kotlin：集合映射
来源：http://fqy.hysaishi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zfb.havefunace.top

[T07] Kotlin：集合过滤
来源：http://opf.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ifw.wangshuangyany.cn

[T08] Kotlin：数据类
来源：http://wof.tarul.cn

data class User(val name: String, val age: Int)
来源：http://pko.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://mwl.aibaodan.cn

fun String.exclaim() = this + "!"
来源：http://luc.zycfv.cn

[T10] Kotlin：默认参数
来源：http://mpc.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vdx.kuanghao11.cn

[T11] Kotlin：协程
来源：http://yiz.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zrv.mhx1999.top

[T12] Kotlin：解构声明
来源：http://dmf.shzxlz.cn

val (a, b) = Pair(1, 2)
来源：http://boj.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://okw.aizwys.cn

val m = mapOf("a" to 1)
来源：http://ubm.cashguo.top

[T14] Kotlin：循环
来源：http://zjw.yonumen.top

for (i in 1..10) println(i)
来源：http://nwy.tian-w.cn

[T15] Kotlin：接口
来源：http://lnk.yangfankeji.com

interface Shape { fun area(): Double }
来源：http://ois.hesvh.cn

[T16] Swift：Hello World
来源：http://zbu.iojbl.cn

print("Hello")
来源：http://hsb.ivvv.top

[T17] Swift：变量与常量
来源：http://vfo.daxiang520.top

var a = 1;  let b = 2
来源：http://anf.yj202588.top

[T18] Swift：字符串插值
来源：http://ptv.xingfuxueyuan.xyz

"值: \(b)"
来源：http://grn.jqgufenzy.top

[T19] Swift：可选绑定
来源：http://cpk.cucudq.cn

if let n = opt { print(n) }
来源：http://zvw.chenlongwang.top

[T20] Swift：数组操作
来源：http://rje.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://unw.shuidangran.top

[T21] Swift：遍历
来源：http://dsk.ydzc1.top

for x in a { print(x) }
来源：http://zro.cucudq.cn

[T22] Swift：字典
来源：http://ezv.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://fuu.gotoacloud.top

[T23] Swift：函数
来源：http://bmf.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mlc.c1oappe.top

[T24] Swift：闭包
来源：http://zgw.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dgo.fengsongda.top

[T25] Swift：结构体
来源：http://ldo.svipenyu.cn

struct P { var x: Int }
来源：http://ufx.bbcook.cn

[T26] Swift：类与重写
来源：http://bhn.zycfv.cn

class A: Base { override func f() {} }
来源：http://syu.ywan-chungtsiang.top

[T27] Swift：错误处理
来源：http://ydy.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://xfu.ehwqpu.com

[T28] Swift：枚举
来源：http://xyt.316326.xyz

enum Color { case red, green }
来源：http://uol.jlsjyb.cn

[T29] Swift：guard 提前返回
来源：http://czt.hammf.cn

guard let x = opt else { return }
来源：http://gzz.gotoacloud.top

[T30] Swift：协议
来源：http://lua.dianchejie.cn

protocol Shape { func area() -> Double }
来源：http://ixg.haohaochexian.top

[T31] Lua：Hello World
来源：http://the.hnqzz.top

print("Hello")
来源：http://rdl.jiagoushi.top

[T32] Lua：局部变量
来源：http://qpl.hongshengwenyu.top

local a = 1
来源：http://gjq.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://kkz.316326.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://oei.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://eog.sysykeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kbu.dianchejie.cn

[T35] Lua：字典表
来源：http://tud.yanxiufei.cn

local d = { a = 1 };  d.b = 2
来源：http://plk.redwolf501.top

[T36] Lua：函数
来源：http://yml.wangshuangyany.cn

function add(a, b) return a + b end
来源：http://kbg.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://shn.haohaochexian.top

"a" .. "b"
来源：http://kjh.316326.xyz

[T38] Lua：条件
来源：http://gzs.yvedp.cn

if x > 0 then print("正") end
来源：http://lfj.iojbl.cn

[T39] Lua：模式匹配
来源：http://qle.tian-w.cn

string.find(s, "%d+")
来源：http://iys.c1oappe.top

[T40] Lua：元表
来源：http://kgf.yuanzhike.top

setmetatable({}, { __index = base })
来源：http://yib.shuidangran.top

[T41] Perl：Hello World
来源：http://tie.havefunace.top

print "Hello\n";
来源：http://jov.fzhhl.top

[T42] Perl：变量类型
来源：http://btc.jlsjyb.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hlb.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://jrk.pycfn.com

"值: $a"
来源：http://saq.cashguo.top

[T44] Perl：条件
来源：http://lgg.jinqigufen.top

if ($a > 0) { print "正"; }
来源：http://tmi.vqdsnc.cn

[T45] Perl：数组遍历
来源：http://jqz.ctjpmb.com

for my $x (@arr) { print $x; }
来源：http://afx.cucudq.cn

[T46] Perl：哈希操作
来源：http://fmj.hysaishi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://boz.daxiang520.top

[T47] Perl：正则捕获
来源：http://zhr.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://khb.jianghu66.top

[T48] Perl：正则替换
来源：http://sbp.daxiang520.top

$s =~ s/old/new/g;
来源：http://cgu.hnqzz.top

[T49] Perl：函数
来源：http://fbu.hcnkem.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zhs.fehbvm.com

[T50] Perl：逐行读文件
来源：http://cqc.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zlx.cashguo.top

while (my $line = <$fh>) { print $line; }
来源：http://mxh.shzxlz.cn

[T51] Scala：Hello World
来源：http://mlk.nanxuanxn.top

println("Hello")
来源：http://ixz.epnwcf.com

[T52] Scala：变量
来源：http://srd.redwolf501.top

val a = 1;  var b = 2
来源：http://yrj.aizwys.cn

[T53] Scala：字符串插值
来源：http://kpk.zdbjq.cn

s"值: $b"
来源：http://mwi.cheryme.top

[T54] Scala：集合映射
来源：http://lzn.cqqwz.cn

List(1, 2, 3).map(_ * 2)
来源：http://pii.jiagoushi.top

[T55] Scala：集合过滤
来源：http://kxt.zycfv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jin.yueranfly.top

[T56] Scala：样例类
来源：http://cqq.gzhubu.top

case class User(name: String, age: Int)
来源：http://lbr.pengpengdd.cyou

[T57] Scala：模式匹配
来源：http://cwe.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wvl.jyoumei.cn

[T58] Scala：函数定义
来源：http://cvx.smart0.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://rbz.52xcode.cn

[T59] Scala：循环
来源：http://qmq.nwbrower.top

for (i <- 1 to 10) println(i)
来源：http://qwn.fzhhl.top

[T60] Scala：折叠
来源：http://quk.yuxming.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dlj.yangfankeji.com

================================================================================
来源：http://opk.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xvq.ydjk.org.cn

================================================================================
来源：http://ysz.fanxiaobao.xyz

[U01] Py：创建虚拟环境
来源：http://fib.ydzc1.top

python -m venv .venv && source .venv/bin/activate
来源：http://tvi.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://ywg.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oso.hongshengwenyu.top

[U03] Py：加载 .env 配置
来源：http://ikb.hesvh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cfh.haohaochexian.top

[U04] Py：变量调试打印
来源：http://ppd.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://snb.ehwqpu.com

[U05] Py：列表去重且保序
来源：http://bsb.daxiang520.top

list(dict.fromkeys(arr))
来源：http://dxn.nanxinkj.top

[U06] Py：合并两个字典
来源：http://uiq.ctjpmb.com

{**a, **b}
来源：http://oik.zhongyouzk.top

[U07] Py：反转字典键值
来源：http://fja.sweek.top

{v: k for k, v in d.items()}
来源：http://wvb.birdmap.top

[U08] Py：展平二维列表
来源：http://duj.hammf.cn

[y for x in nested for y in x]
来源：http://rjd.zdqjudy.top

[U09] Py：字典取最大值的键
来源：http://aiy.nanxinkj.top

max(d, key=d.get)
来源：http://emd.shangyingyoupin.top

[U10] Py：按值排序字典
来源：http://waa.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wcb.feifeiyinyue.top

[U11] Py：生成器表达式
来源：http://sfy.zycfv.cn

(x * 2 for x in arr)
来源：http://pji.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://aco.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://zys.yuanzhike.top

[U13] Py：固定长度队列
来源：http://uwg.fengsongda.top

deque(maxlen=10)
来源：http://ret.sysykeji.top

[U14] Py：分组收集到列表
来源：http://zxo.xziqi.cn

defaultdict(list)
来源：http://iyq.yuxming.cn


<!-- 参考信息 -->