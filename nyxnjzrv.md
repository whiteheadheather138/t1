代发 wailian999

read -rp "请输入: " ans
来源：http://ose.sysykeji.top

[R78] 交互式菜单
来源：http://gvs.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://icp.sweek.top

[R79] 解析命令行选项
来源：http://ldy.sufxvd.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zkf.hammf.cn

[R80] 查看脚本执行耗时
来源：http://kgc.guannengcc.top

time ./run.sh
来源：http://pvm.pycfn.com

================================================================================
来源：http://xoh.dianchejie.cn

S. C / C++ 专题
来源：http://snr.havefunace.top

================================================================================
来源：http://jxk.yangfankeji.com

[S01] C：Hello World
来源：http://nxi.iojbl.cn

#include <stdio.h>
来源：http://bah.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ubs.ybcxt.top

[S02] C：变量与格式化输出
来源：http://lal.zdbjq.cn

int a = 10; printf("%d\n", a);
来源：http://jpd.aibaodan.cn

[S03] C：读入整数
来源：http://uqd.ydzc1.top

int x; scanf("%d", &x);
来源：http://rgt.jqgfzy.top

[S04] C：字符串复制
来源：http://luo.yj20258.top

char dst[32]; strcpy(dst, "hi");
来源：http://lcs.jianghu66.top

[S05] C：字符串长度
来源：http://uya.cqqwz.cn

strlen(s)
来源：http://fdv.bbcook.cn

[S06] C：字符串比较
来源：http://nxz.gaohongyu789.top

strcmp(a, b) == 0
来源：http://bgk.nanxinkj.top

[S07] C：数组遍历求和
来源：http://bfp.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fky.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://eux.ydzc1.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aua.hongshengwenyu.top

[S09] C：结构体定义与初始化
来源：http://ewr.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wse.fehbvm.com

[S10] C：指针与解引用
来源：http://qdm.epnwcf.com

int *p = &a;  *p = 5;
来源：http://eyh.guannengcc.top

[S11] C：逐行读文件
来源：http://suw.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://qnx.yj20258.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://uch.hfpthk.cn

fclose(f);
来源：http://agm.wangshuangyany.cn

[S12] C：写文件
来源：http://nih.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yjl.ivvv.top

[S13] C：宏定义
来源：http://wrg.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vsf.shanyushiyangkeji.top

[S14] C：枚举
来源：http://gvx.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://bea.dianchejie.cn

[S15] C：类型转换
来源：http://giw.wangshuangyany.cn

(double) a / b
来源：http://acr.yj20258888.top

[S16] C：位操作置位
来源：http://qiy.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://jrq.smart0.xyz

[S17] C：安全拼接字符串
来源：http://yef.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gta.bbcook.cn

[S18] C：命令行参数
来源：http://dyg.wangdashe.top

int main(int argc, char **argv)
来源：http://apf.ppjwa.cn

[S19] C：快速排序
来源：http://rfn.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://xym.ivvv.top

[S20] C：二分查找
来源：http://dcp.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tew.zhongyouzk.top

[S21] C：字符类别判断
来源：http://nig.wangdashe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ztx.vehdjk.com

[S22] C：字符串转数字
来源：http://wzb.sweek.top

atoi("42");  strtod("3.14", NULL);
来源：http://xwt.fengsongda.top

[S23] C：随机数
来源：http://erw.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gsx.xylfe.cn

[S24] C：获取本地时间
来源：http://bry.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mbu.yueranfly.top

[S25] C：内存拷贝
来源：http://agm.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://mhb.tarul.cn

[S26] C：内存清零
来源：http://zfo.316326.xyz

memset(a, 0, sizeof a);
来源：http://kbw.hcnkem.com

[S27] C：定义常量
来源：http://wnn.haohaochexian.top

const double PI = 3.14159;
来源：http://xfj.cdnleiting.top

[S28] C：静态变量
来源：http://tki.nanxuanxn.top

static int counter = 0;
来源：http://pip.hnxiangtu.top

[S29] C：变参函数
来源：http://viu.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jge.hywenlv.cn

[S30] C：头文件保护
来源：http://opn.gaohongyu789.top

#ifndef X_H
来源：http://nfc.zhaomingkeji.xyz

#define X_H
来源：http://ioe.wangshuangyany.cn

#endif
来源：http://vcv.316326.xyz

[S31] C++：Hello World
来源：http://qqq.hnxiangtu.top

#include <iostream>
来源：http://bzf.meibo888.top

int main() { std::cout << "Hello\n"; }
来源：http://jdr.chenzaomai.com

[S32] C++：字符串
来源：http://dvi.havefunace.top

std::string s = "hi";  s += "!";
来源：http://csw.tian-w.cn

[S33] C++：vector 增删
来源：http://fys.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sdz.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://liw.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://kbc.shzxlz.cn

[S35] C++：map
来源：http://nrm.kuanghao11.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yzq.zhijiandao.cn

[S36] C++：unordered_map
来源：http://aqy.daxiang520.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://upo.wangshuangyany.cn

[S37] C++：set
来源：http://tqa.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fod.xziqi.cn

[S38] C++：排序
来源：http://dhx.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://uis.zhaomingkeji.xyz

[S39] C++：自定义比较器排序
来源：http://wly.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uqe.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://ypp.havefunace.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://duz.52xcode.cn

[S41] C++：类与构造函数
来源：http://dio.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mjq.yvedp.cn

[S42] C++：继承与虚函数
来源：http://mid.sweek.top

class B : public Base { public: void f() override {} };
来源：http://rps.havefunace.top

[S43] C++：智能指针
来源：http://iuz.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://xrq.jlsjyb.cn

[S44] C++：引用传参
来源：http://qjo.epnwcf.com

void inc(int &x) { ++x; }
来源：http://oqb.fengsongda.top

[S45] C++：lambda
来源：http://nvg.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://hua.meibo888.top

[S46] C++：函数模板
来源：http://vjq.chenlongwang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://chm.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://uma.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qmf.bbcook.cn

[S48] C++：逐行读文件
来源：http://geg.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://gdd.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://gli.sxryk.cn

[S49] C++：写文件
来源：http://tod.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qrl.daxiang520.top

[S50] C++：格式化数字
来源：http://yuy.xingfuxueyuan.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uhl.quarkkingdee.top

[S51] C++：显式类型转换
来源：http://rav.xziqi.cn

static_cast<double>(a) / b
来源：http://sui.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://lgk.cheryme.top

int size() const noexcept { return n_; }
来源：http://any.jinqigufen.top

[S53] C++：移动语义
来源：http://unh.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://tjp.havefunace.top

[S54] C++：异常处理
来源：http://kzt.wangdashe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vik.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://mhy.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yfe.daxiang520.top

[S56] C++：optional
来源：http://nzc.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qxa.hnxiangtu.top

[S57] C++：编译期常量
来源：http://ndo.tanke756.top

constexpr int N = 10;
来源：http://ufg.jianghu66.top

[S58] C++：命名空间
来源：http://mjr.fengsongda.top

namespace ns { int f() { return 1; } }
来源：http://huc.pycfn.com

[S59] C++：静态断言
来源：http://zmr.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rjo.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://yvo.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zsh.hywenlv.cn

================================================================================
来源：http://xmc.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ovc.chenjidiqi.icu

================================================================================
来源：http://aqa.meibo888.top

[T01] Kotlin：Hello World
来源：http://eif.ywan-chungtsiang.top

println("Hello")
来源：http://sei.zhijiandao.cn

[T02] Kotlin：变量
来源：http://ozp.zdqjudy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vme.sysykeji.top

[T03] Kotlin：字符串模板
来源：http://hmu.xylfe.cn

"值: $b"
来源：http://grj.wangdashe.top

[T04] Kotlin：空安全
来源：http://xbx.cdnleiting.top

val n: String? = null;  n?.length
来源：http://mba.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://myd.jqgfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://epf.xinyue.icu

[T06] Kotlin：集合映射
来源：http://uns.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://naz.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://pvo.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iew.tian-w.cn

[T08] Kotlin：数据类
来源：http://emc.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://fai.fzhhl.top

[T09] Kotlin：扩展函数
来源：http://rqy.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://nub.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://leo.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jpz.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://ezp.feifeiyinyue.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rpe.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://mgn.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://tiy.andypj.xyz

[T13] Kotlin：只读 Map
来源：http://nug.ydjk.org.cn

val m = mapOf("a" to 1)
来源：http://usz.yongpay.top

[T14] Kotlin：循环
来源：http://nnb.jqgfzy.top

for (i in 1..10) println(i)
来源：http://loz.yj202588.top

[T15] Kotlin：接口
来源：http://piv.mhx1999.top

interface Shape { fun area(): Double }
来源：http://arl.haohaochexian.top

[T16] Swift：Hello World
来源：http://mrj.ivvv.top

print("Hello")
来源：http://hja.yangfankeji.com

[T17] Swift：变量与常量
来源：http://lgn.ppjwa.cn

var a = 1;  let b = 2
来源：http://qxg.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://bub.epnwcf.com

"值: \(b)"
来源：http://nqe.jlsjyb.cn

[T19] Swift：可选绑定
来源：http://lhm.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://cqi.andypj.xyz

[T20] Swift：数组操作
来源：http://ohh.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://zef.bjfxy.top

[T21] Swift：遍历
来源：http://dfb.bjfxy.top

for x in a { print(x) }
来源：http://ubu.cqqwz.cn

[T22] Swift：字典
来源：http://kbk.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rhb.jinghuilouyu.cn

[T23] Swift：函数
来源：http://nzd.nanxinkj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xcy.daxiang520.top

[T24] Swift：闭包
来源：http://yfg.fktsv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hic.fehbvm.com

[T25] Swift：结构体
来源：http://sdm.tianlin.xyz

struct P { var x: Int }
来源：http://ocd.sweek.top

[T26] Swift：类与重写
来源：http://inr.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://uxa.shuidangran.top

[T27] Swift：错误处理
来源：http://wjy.fengsongda.top

do { try f() } catch { print(error) }
来源：http://pis.yj20258.top

[T28] Swift：枚举
来源：http://gkp.shzxlz.cn

enum Color { case red, green }
来源：http://msd.chenlongwang.top

[T29] Swift：guard 提前返回
来源：http://ctw.kuanghao11.cn

guard let x = opt else { return }
来源：http://iul.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://nnc.yonumen.top

protocol Shape { func area() -> Double }
来源：http://ivb.bbcook.cn

[T31] Lua：Hello World
来源：http://tpv.aibaodan.cn

print("Hello")
来源：http://dhg.cqqwz.cn

[T32] Lua：局部变量
来源：http://ouh.jyoumei.cn

local a = 1
来源：http://gom.pycfn.com

[T33] Lua：表（数组）
来源：http://qxf.dashuyun.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gbz.smart0.xyz

[T34] Lua：遍历表
来源：http://yqs.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://nhc.birdmap.top

[T35] Lua：字典表
来源：http://pbd.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://nwh.guowangkeji.top

[T36] Lua：函数
来源：http://fkt.ybcxt.top

function add(a, b) return a + b end
来源：http://yik.fzhhl.top

[T37] Lua：字符串拼接
来源：http://ukd.jinqigufen.top

"a" .. "b"
来源：http://cjx.tarul.cn

[T38] Lua：条件
来源：http://gjd.nwbrower.top

if x > 0 then print("正") end
来源：http://zhg.hywenlv.cn

[T39] Lua：模式匹配
来源：http://fma.fktsv.cn

string.find(s, "%d+")
来源：http://eao.yongpay.top

[T40] Lua：元表
来源：http://kts.nwbrower.top

setmetatable({}, { __index = base })
来源：http://ejb.nanxinkj.top

[T41] Perl：Hello World
来源：http://ynt.yanxiufei.cn

print "Hello\n";
来源：http://lza.dianchejie.cn

[T42] Perl：变量类型
来源：http://lih.shanyushiyangtech.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qvx.zhengqikj.top

[T43] Perl：字符串插值
来源：http://xdo.sysykeji.top

"值: $a"
来源：http://kca.cucudq.cn

[T44] Perl：条件
来源：http://bml.jinghuilouyu.cn

if ($a > 0) { print "正"; }
来源：http://vdd.xuanzx.com

[T45] Perl：数组遍历
来源：http://blm.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://ntk.cdnleiting.top

[T46] Perl：哈希操作
来源：http://plm.sxryk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kwd.9152youxi.cn

[T47] Perl：正则捕获
来源：http://lji.daxiang520.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://opb.dashuyun.cn

[T48] Perl：正则替换
来源：http://wuy.gaohongyu789.top

$s =~ s/old/new/g;
来源：http://qtw.hywenlv.cn

[T49] Perl：函数
来源：http://zbp.zhoulong.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dnt.yonumen.top

[T50] Perl：逐行读文件
来源：http://pzu.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rhy.haohaochexian.top

while (my $line = <$fh>) { print $line; }
来源：http://ajz.svipenyu.cn

[T51] Scala：Hello World
来源：http://jxn.tian-w.cn

println("Hello")
来源：http://pyj.nanxinkj.top

[T52] Scala：变量
来源：http://ydy.ctjpmb.com

val a = 1;  var b = 2
来源：http://bfb.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://jcu.hcnkem.com

s"值: $b"
来源：http://eps.quarkkingdee.top

[T54] Scala：集合映射
来源：http://jcg.cashguo.top

List(1, 2, 3).map(_ * 2)
来源：http://gbo.jinyuanbaomall.cn

[T55] Scala：集合过滤
来源：http://dnp.sxryk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gvt.zhengqikj.top

[T56] Scala：样例类
来源：http://gkt.jinqigufen.top

case class User(name: String, age: Int)
来源：http://teb.daria6918.cn

[T57] Scala：模式匹配
来源：http://pda.guannengcc.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fsh.quarkkingdee.top

[T58] Scala：函数定义
来源：http://zxf.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tiz.wangdashe.top

[T59] Scala：循环
来源：http://egd.cdnleiting.top

for (i <- 1 to 10) println(i)
来源：http://gsq.shuidangran.top

[T60] Scala：折叠
来源：http://sto.zdbjq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xel.ppjwa.cn

================================================================================
来源：http://yaj.cdnleiting.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cwy.fengsongda.top

================================================================================
来源：http://xls.yuxming.cn

[U01] Py：创建虚拟环境
来源：http://yzd.cashguo.top

python -m venv .venv && source .venv/bin/activate
来源：http://cys.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://hwc.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jyv.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://hrh.9152youxi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cpq.bbcook.cn

[U04] Py：变量调试打印
来源：http://yct.nanxuanxn.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tya.wangdashe.top

[U05] Py：列表去重且保序
来源：http://dft.daxiang520.top

list(dict.fromkeys(arr))
来源：http://dux.fktsv.cn

[U06] Py：合并两个字典
来源：http://wbu.gotoacloud.top

{**a, **b}
来源：http://hja.daria6918.cn

[U07] Py：反转字典键值
来源：http://lpe.fehbvm.com

{v: k for k, v in d.items()}
来源：http://fgl.zycfv.cn

[U08] Py：展平二维列表
来源：http://nlw.zycfv.cn

[y for x in nested for y in x]
来源：http://sok.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://mqh.shzxlz.cn

max(d, key=d.get)
来源：http://oyu.havefunace.top

[U10] Py：按值排序字典
来源：http://mga.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fho.ydjk.org.cn

[U11] Py：生成器表达式
来源：http://prh.zhoulong.xyz

(x * 2 for x in arr)
来源：http://dxf.shanyushiyangtech.top

[U12] Py：取出现最多的 3 个元素
来源：http://gcu.shzxlz.cn

Counter(arr).most_common(3)
来源：http://hlv.yongpay.top

[U13] Py：固定长度队列
来源：http://mnv.gaohongyu789.top

deque(maxlen=10)
来源：http://qip.iojbl.cn

[U14] Py：分组收集到列表
来源：http://irv.gogol.net.cn

defaultdict(list)
来源：http://xxq.aibaodan.cn

[U15] Py：高精度计时
来源：http://uyi.hongshengwenyu.top

t = time.perf_counter()
来源：http://usp.ppjwa.cn

[U16] Py：命令行参数解析
来源：http://sdw.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gji.daria6918.cn

[U17] Py：初始化日志
来源：http://crp.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://yug.epnwcf.com

[U18] Py：预编译正则
来源：http://yqd.zhongyouzk.top

pat = re.compile(r"\d+")
来源：http://zyd.cucudq.cn


<!-- 参考信息 -->