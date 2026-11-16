代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://zpp.9152youxi.cn

[R76] 使用临时文件
来源：http://jir.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yns.zycfv.cn

[R77] 读取用户输入
来源：http://fwm.zhongyouzk.top

read -rp "请输入: " ans
来源：http://cbu.yfazqb.com

[R78] 交互式菜单
来源：http://ugv.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rda.ehwqpu.com

[R79] 解析命令行选项
来源：http://qwe.cqqwz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ieo.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://ovl.aizwys.cn

time ./run.sh
来源：http://ytp.shzxlz.cn

================================================================================
来源：http://jnw.quarkkingdee.top

S. C / C++ 专题
来源：http://bpc.smart0.xyz

================================================================================
来源：http://kgp.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://qlj.xinyue.icu

#include <stdio.h>
来源：http://emt.316326.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://nce.nwbrower.top

[S02] C：变量与格式化输出
来源：http://ywj.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://mle.gotoacloud.top

[S03] C：读入整数
来源：http://njo.jyoumei.cn

int x; scanf("%d", &x);
来源：http://uiz.zhongyouzk.top

[S04] C：字符串复制
来源：http://ias.zhaomingkeji.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://hgh.shzxlz.cn

[S05] C：字符串长度
来源：http://ufx.nanxuanxn.top

strlen(s)
来源：http://gln.fehbvm.com

[S06] C：字符串比较
来源：http://aij.aizwys.cn

strcmp(a, b) == 0
来源：http://leu.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://txk.ctjpmb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://veh.jqgfzy.top

[S08] C：动态内存分配与释放
来源：http://qwk.shzxlz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rna.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://nwt.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cas.ybcxt.top

[S10] C：指针与解引用
来源：http://frr.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://nls.ydzc1.top

[S11] C：逐行读文件
来源：http://izs.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://ndk.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fyt.sufxvd.cn

fclose(f);
来源：http://ddm.hongshengwenyu.top

[S12] C：写文件
来源：http://crn.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lxk.hnxiangtu.top

[S13] C：宏定义
来源：http://dzx.ywan-chungtsiang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zor.zhengqikj.top

[S14] C：枚举
来源：http://opv.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://utb.yongpay.top

[S15] C：类型转换
来源：http://vly.yuxming.cn

(double) a / b
来源：http://biw.nanxuanxn.top

[S16] C：位操作置位
来源：http://pbz.kuanghao11.cn

x |= (1 << 3);
来源：http://qxm.aizwys.cn

[S17] C：安全拼接字符串
来源：http://yob.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wdv.hesvh.cn

[S18] C：命令行参数
来源：http://npx.ivvv.top

int main(int argc, char **argv)
来源：http://wre.0kj1m.cn

[S19] C：快速排序
来源：http://mnm.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yit.chenzaomai.com

[S20] C：二分查找
来源：http://cdb.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gbv.0kj1m.cn

[S21] C：字符类别判断
来源：http://qeu.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gcv.jiagoushi.top

[S22] C：字符串转数字
来源：http://nmd.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://yso.redwolf501.top

[S23] C：随机数
来源：http://cyu.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hfb.cucudq.cn

[S24] C：获取本地时间
来源：http://gst.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gla.ybcxt.top

[S25] C：内存拷贝
来源：http://quf.yuanzhike.top

memcpy(dst, src, n);
来源：http://faf.yfazqb.com

[S26] C：内存清零
来源：http://ube.vehdjk.com

memset(a, 0, sizeof a);
来源：http://nyl.ctjpmb.com

[S27] C：定义常量
来源：http://qzi.chenjidiqi.icu

const double PI = 3.14159;
来源：http://zpn.dianchejie.cn

[S28] C：静态变量
来源：http://xzu.kuanghao11.cn

static int counter = 0;
来源：http://blt.vqdsnc.cn

[S29] C：变参函数
来源：http://txz.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ggp.sysykeji.top

[S30] C：头文件保护
来源：http://wrc.xylfe.cn

#ifndef X_H
来源：http://ykh.jiagoushi.top

#define X_H
来源：http://dor.yfazqb.com

#endif
来源：http://qtm.gzhubu.top

[S31] C++：Hello World
来源：http://zfc.shzxlz.cn

#include <iostream>
来源：http://yry.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://rgk.jinghuilouyu.cn

[S32] C++：字符串
来源：http://yex.hnqzz.top

std::string s = "hi";  s += "!";
来源：http://ipw.ppjwa.cn

[S33] C++：vector 增删
来源：http://uyj.yanxiufei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lqk.mhx1999.top

[S34] C++：遍历 vector
来源：http://tti.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://gso.hcnkem.com

[S35] C++：map
来源：http://cof.jinqigufen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bta.mhx1999.top

[S36] C++：unordered_map
来源：http://fec.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://als.daxiang520.top

[S37] C++：set
来源：http://ecj.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wdv.ybcxt.top

[S38] C++：排序
来源：http://gyj.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://mng.tanke756.top

[S39] C++：自定义比较器排序
来源：http://fdk.fktsv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://raa.jqgufenzy.top

[S40] C++：查找元素
来源：http://sra.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://loc.shanyushiyangkeji.top

[S41] C++：类与构造函数
来源：http://jjl.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xcu.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://hhk.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://fie.zhiwuduotai.top

[S43] C++：智能指针
来源：http://xvd.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://mmn.bbcook.cn

[S44] C++：引用传参
来源：http://mwg.nwbrower.top

void inc(int &x) { ++x; }
来源：http://ghk.fanxiaobao.xyz

[S45] C++：lambda
来源：http://brq.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tlb.cqqwz.cn

[S46] C++：函数模板
来源：http://yai.jianghu66.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aqv.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://tde.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rma.mhx1999.top

[S48] C++：逐行读文件
来源：http://nwa.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://ucf.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://xyy.zdqjudy.top

[S49] C++：写文件
来源：http://ivr.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ncx.sufxvd.cn

[S50] C++：格式化数字
来源：http://nmj.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qlo.pengpengdd.cyou

[S51] C++：显式类型转换
来源：http://jdp.tian-w.cn

static_cast<double>(a) / b
来源：http://ykb.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://mxw.yuanzhike.top

int size() const noexcept { return n_; }
来源：http://zel.zhiwuduotai.top

[S53] C++：移动语义
来源：http://ncv.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://wtv.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://ely.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jnz.hammf.cn

[S55] C++：结构化绑定
来源：http://dqq.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qrc.havefunace.top

[S56] C++：optional
来源：http://lih.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hsz.nanxinkj.top

[S57] C++：编译期常量
来源：http://orp.sweek.top

constexpr int N = 10;
来源：http://gew.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://afq.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://lsv.meibo888.top

[S59] C++：静态断言
来源：http://vie.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ztm.316326.xyz

[S60] C++：遍历并删除元素
来源：http://mcv.epnwcf.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nrs.cdnleiting.top

================================================================================
来源：http://hck.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qzu.jinghuilouyu.cn

================================================================================
来源：http://dul.xziqi.cn

[T01] Kotlin：Hello World
来源：http://mhf.yongpay.top

println("Hello")
来源：http://duv.nwbrower.top

[T02] Kotlin：变量
来源：http://pee.nanxuanxn.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fet.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://gqi.zhixingplan.top

"值: $b"
来源：http://xnu.xingfuxueyuan.xyz

[T04] Kotlin：空安全
来源：http://ngd.9152youxi.cn

val n: String? = null;  n?.length
来源：http://hly.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://qon.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zpw.dashuyun.cn

[T06] Kotlin：集合映射
来源：http://csc.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://opv.fehbvm.com

[T07] Kotlin：集合过滤
来源：http://qff.gotoacloud.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mge.chenlongwang.top

[T08] Kotlin：数据类
来源：http://pbr.zdbjq.cn

data class User(val name: String, val age: Int)
来源：http://idi.chenjidiqi.icu

[T09] Kotlin：扩展函数
来源：http://ggq.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://pms.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://boj.52xcode.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cqs.iojbl.cn

[T11] Kotlin：协程
来源：http://unf.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ays.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://tey.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://cbm.uphjek.com

[T13] Kotlin：只读 Map
来源：http://ndj.sweek.top

val m = mapOf("a" to 1)
来源：http://ogc.fzhhl.top

[T14] Kotlin：循环
来源：http://efb.hfpthk.cn

for (i in 1..10) println(i)
来源：http://qeg.iojbl.cn

[T15] Kotlin：接口
来源：http://lxm.hammf.cn

interface Shape { fun area(): Double }
来源：http://iyr.9152youxi.cn

[T16] Swift：Hello World
来源：http://hve.gotoacloud.top

print("Hello")
来源：http://the.havefunace.top

[T17] Swift：变量与常量
来源：http://xyc.yfazqb.com

var a = 1;  let b = 2
来源：http://ksu.nwbrower.top

[T18] Swift：字符串插值
来源：http://uji.chenzaomai.com

"值: \(b)"
来源：http://hzu.jianghu66.top

[T19] Swift：可选绑定
来源：http://yub.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://oaz.andypj.xyz

[T20] Swift：数组操作
来源：http://qgc.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://aqn.vehdjk.com

[T21] Swift：遍历
来源：http://jmh.tian-w.cn

for x in a { print(x) }
来源：http://obb.cashguo.top

[T22] Swift：字典
来源：http://gmy.zdqjudy.top

var d = ["a": 1];  d["b"] = 2
来源：http://bve.sxryk.cn

[T23] Swift：函数
来源：http://cxn.316326.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rdz.nwbrower.top

[T24] Swift：闭包
来源：http://sun.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sot.sysykeji.top

[T25] Swift：结构体
来源：http://rcn.zhongyouzk.top

struct P { var x: Int }
来源：http://prr.yuanzhike.top

[T26] Swift：类与重写
来源：http://vqu.ctjpmb.com

class A: Base { override func f() {} }
来源：http://uzz.cucudq.cn

[T27] Swift：错误处理
来源：http://ltj.guowangkeji.top

do { try f() } catch { print(error) }
来源：http://lrn.ywan-chungtsiang.top

[T28] Swift：枚举
来源：http://gtj.epnwcf.com

enum Color { case red, green }
来源：http://cwz.gogol.net.cn

[T29] Swift：guard 提前返回
来源：http://gby.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://wpl.wangshuangyany.cn

[T30] Swift：协议
来源：http://nvt.vehdjk.com

protocol Shape { func area() -> Double }
来源：http://unq.gotoacloud.top

[T31] Lua：Hello World
来源：http://rbd.iojbl.cn

print("Hello")
来源：http://fih.bjfxy.top

[T32] Lua：局部变量
来源：http://suw.cashguo.top

local a = 1
来源：http://wlu.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://xym.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://smz.ivvv.top

[T34] Lua：遍历表
来源：http://iag.feifeiyinyue.top

for i, v in ipairs(t) do print(i, v) end
来源：http://swr.chenzaomai.com

[T35] Lua：字典表
来源：http://yaw.quarkkingdee.top

local d = { a = 1 };  d.b = 2
来源：http://swv.yongpay.top

[T36] Lua：函数
来源：http://xwk.havefunace.top

function add(a, b) return a + b end
来源：http://iko.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://nct.ppjwa.cn

"a" .. "b"
来源：http://adw.wangdashe.top

[T38] Lua：条件
来源：http://zts.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://vmj.yfazqb.com

[T39] Lua：模式匹配
来源：http://gmi.epnwcf.com

string.find(s, "%d+")
来源：http://rbx.zhongyouzk.top

[T40] Lua：元表
来源：http://kli.epnwcf.com

setmetatable({}, { __index = base })
来源：http://wfs.zycfv.cn

[T41] Perl：Hello World
来源：http://mpa.sjlbkw.cn

print "Hello\n";
来源：http://ecq.nanxinkj.top

[T42] Perl：变量类型
来源：http://gum.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zwx.nanxinkj.top

[T43] Perl：字符串插值
来源：http://vcp.yangfankeji.com

"值: $a"
来源：http://ugy.0kj1m.cn

[T44] Perl：条件
来源：http://dfg.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://rkc.bjfxy.top

[T45] Perl：数组遍历
来源：http://kcn.gaohongyu789.top

for my $x (@arr) { print $x; }
来源：http://erv.chenzaomai.com

[T46] Perl：哈希操作
来源：http://axt.jinqigfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://urs.ivvv.top

[T47] Perl：正则捕获
来源：http://evv.zhijiandao.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dom.mhx1999.top

[T48] Perl：正则替换
来源：http://pef.chenzaomai.com

$s =~ s/old/new/g;
来源：http://vpw.redwolf501.top

[T49] Perl：函数
来源：http://ssa.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nxq.fzhhl.top

[T50] Perl：逐行读文件
来源：http://vzs.hnxiangtu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qzh.shangyingyoupin.top

while (my $line = <$fh>) { print $line; }
来源：http://abw.snrcjt.cn

[T51] Scala：Hello World
来源：http://pao.daxiang520.top

println("Hello")
来源：http://lkq.feifeiyinyue.top

[T52] Scala：变量
来源：http://qoo.jinqigfzy.top

val a = 1;  var b = 2
来源：http://fyq.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://yaq.yj20258.top

s"值: $b"
来源：http://jar.haohaochexian.top

[T54] Scala：集合映射
来源：http://ehm.sufxvd.cn

List(1, 2, 3).map(_ * 2)
来源：http://wot.ppjwa.cn

[T55] Scala：集合过滤
来源：http://uhn.dianchejie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bwm.gogol.net.cn

[T56] Scala：样例类
来源：http://dwp.yj20258.top

case class User(name: String, age: Int)
来源：http://vax.zhengqikj.top

[T57] Scala：模式匹配
来源：http://pil.yfazqb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://tlv.chenlongwang.top

[T58] Scala：函数定义
来源：http://sim.xinyue.icu

def add(a: Int, b: Int): Int = a + b
来源：http://xrp.yanxiufei.cn

[T59] Scala：循环
来源：http://qjj.fktsv.cn

for (i <- 1 to 10) println(i)
来源：http://blb.shzxlz.cn

[T60] Scala：折叠
来源：http://ouv.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://exl.shuidangran.top

================================================================================
来源：http://mcj.jinghuilouyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gtl.jinqigfzy.top

================================================================================
来源：http://kbh.tian-w.cn

[U01] Py：创建虚拟环境
来源：http://yqb.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://ddh.zdbjq.cn

[U02] Py：导出 / 安装依赖
来源：http://xnw.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://obg.snrcjt.cn

[U03] Py：加载 .env 配置
来源：http://qcn.dianchejie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://chg.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://gxc.wangdashe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://anc.tarul.cn

[U05] Py：列表去重且保序
来源：http://spz.sweek.top

list(dict.fromkeys(arr))
来源：http://ahj.shanyushiyangkeji.top

[U06] Py：合并两个字典
来源：http://kvc.ybcxt.top

{**a, **b}
来源：http://qgp.mhx1999.top

[U07] Py：反转字典键值
来源：http://nge.epnwcf.com

{v: k for k, v in d.items()}
来源：http://iar.chenzaomai.com

[U08] Py：展平二维列表
来源：http://tfi.yangfankeji.com

[y for x in nested for y in x]
来源：http://fge.ydzc1.top

[U09] Py：字典取最大值的键
来源：http://uuv.hcnkem.com

max(d, key=d.get)
来源：http://ftv.smart0.xyz

[U10] Py：按值排序字典
来源：http://hpv.fzhhl.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nnu.jinqigfzy.top

[U11] Py：生成器表达式
来源：http://ood.sxryk.cn

(x * 2 for x in arr)
来源：http://sbw.fktsv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ioz.yj202588.top

Counter(arr).most_common(3)
来源：http://tnt.smart0.xyz

[U13] Py：固定长度队列
来源：http://jhl.yfazqb.com

deque(maxlen=10)
来源：http://jer.sweek.top

[U14] Py：分组收集到列表
来源：http://jkz.hnqzz.top

defaultdict(list)
来源：http://taj.ybcxt.top

[U15] Py：高精度计时
来源：http://lgo.jyoumei.cn

t = time.perf_counter()
来源：http://tqu.tianlin.xyz

[U16] Py：命令行参数解析
来源：http://ebf.snrcjt.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pei.hammf.cn


<!-- 参考信息 -->