代发 wailian999

split -l 1000 big.log part_
来源：http://uqy.sjlbkw.cn

[R74] 批量重命名
来源：http://zex.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wyn.zdqjudy.top

[R75] 导出环境变量
来源：http://ilk.bbcook.cn

export PATH="$HOME/bin:$PATH"
来源：http://xpz.yueranfly.top

[R76] 使用临时文件
来源：http://zah.zhengqikj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cre.gaohongyu789.top

[R77] 读取用户输入
来源：http://qmw.aizwys.cn

read -rp "请输入: " ans
来源：http://aku.yfazqb.com

[R78] 交互式菜单
来源：http://soo.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://eqk.vqdsnc.cn

[R79] 解析命令行选项
来源：http://gzx.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://msm.yfazqb.com

[R80] 查看脚本执行耗时
来源：http://rpl.tarul.cn

time ./run.sh
来源：http://gaj.andypj.xyz

================================================================================
来源：http://ivm.xziqi.cn

S. C / C++ 专题
来源：http://jkg.nwbrower.top

================================================================================
来源：http://cko.iojbl.cn

[S01] C：Hello World
来源：http://vyg.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://fma.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://foh.yj20258888.top

[S02] C：变量与格式化输出
来源：http://vct.yuxming.cn

int a = 10; printf("%d\n", a);
来源：http://tru.epnwcf.com

[S03] C：读入整数
来源：http://nbh.hesvh.cn

int x; scanf("%d", &x);
来源：http://mux.ybcxt.top

[S04] C：字符串复制
来源：http://lbt.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://ezx.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://oqi.aizwys.cn

strlen(s)
来源：http://ias.yanxiufei.cn

[S06] C：字符串比较
来源：http://sdz.hnqzz.top

strcmp(a, b) == 0
来源：http://vjk.0kj1m.cn

[S07] C：数组遍历求和
来源：http://ttk.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qvu.hammf.cn

[S08] C：动态内存分配与释放
来源：http://uih.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uvs.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://tho.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jch.sufxvd.cn

[S10] C：指针与解引用
来源：http://jkb.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://xny.cqqwz.cn

[S11] C：逐行读文件
来源：http://vau.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://bns.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wif.meibo888.top

fclose(f);
来源：http://ypt.c1oappe.top

[S12] C：写文件
来源：http://fkm.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eqm.ydjk.org.cn

[S13] C：宏定义
来源：http://hau.chenlongwang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mdh.snrcjt.cn

[S14] C：枚举
来源：http://esp.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://ovz.fengsongda.top

[S15] C：类型转换
来源：http://ygm.pycfn.com

(double) a / b
来源：http://ivw.ybcxt.top

[S16] C：位操作置位
来源：http://rds.andypj.xyz

x |= (1 << 3);
来源：http://bmi.xinyue.icu

[S17] C：安全拼接字符串
来源：http://jfo.yj202588.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dga.hfpthk.cn

[S18] C：命令行参数
来源：http://afo.zhijiandao.cn

int main(int argc, char **argv)
来源：http://pfo.jinqigfzy.top

[S19] C：快速排序
来源：http://fsd.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tih.haohaochexian.top

[S20] C：二分查找
来源：http://mfs.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yag.pycfn.com

[S21] C：字符类别判断
来源：http://eei.svipenyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cpl.zdqjudy.top

[S22] C：字符串转数字
来源：http://lkg.zhengqikj.top

atoi("42");  strtod("3.14", NULL);
来源：http://lsk.bjfxy.top

[S23] C：随机数
来源：http://gkj.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ojh.jinghuilouyu.cn

[S24] C：获取本地时间
来源：http://gvt.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://adl.yonumen.top

[S25] C：内存拷贝
来源：http://noo.aibaodan.cn

memcpy(dst, src, n);
来源：http://uml.uphjek.com

[S26] C：内存清零
来源：http://fox.nanxuanxn.top

memset(a, 0, sizeof a);
来源：http://hzh.aibaodan.cn

[S27] C：定义常量
来源：http://xbg.cucudq.cn

const double PI = 3.14159;
来源：http://lsr.gaohongyu789.top

[S28] C：静态变量
来源：http://qed.tarul.cn

static int counter = 0;
来源：http://zeu.uphjek.com

[S29] C：变参函数
来源：http://qbf.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lqp.hywenlv.cn

[S30] C：头文件保护
来源：http://apu.yonumen.top

#ifndef X_H
来源：http://hpd.tian-w.cn

#define X_H
来源：http://wbu.shanyushiyangtech.top

#endif
来源：http://mdi.ydzc1.top

[S31] C++：Hello World
来源：http://fyr.zdqjudy.top

#include <iostream>
来源：http://cpa.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://nhn.tianlin.xyz

[S32] C++：字符串
来源：http://bnb.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://qrn.yvedp.cn

[S33] C++：vector 增删
来源：http://pos.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lpc.fehbvm.com

[S34] C++：遍历 vector
来源：http://bqd.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://xbq.hcnkem.com

[S35] C++：map
来源：http://gti.guannengcc.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://epj.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://kda.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jay.sxryk.cn

[S37] C++：set
来源：http://yzy.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pkb.snrcjt.cn

[S38] C++：排序
来源：http://qpy.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://btj.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://tco.feifeiyinyue.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ldk.ehwqpu.com

[S40] C++：查找元素
来源：http://ovj.yangfankeji.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rlb.havefunace.top

[S41] C++：类与构造函数
来源：http://pim.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fkn.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://pci.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://bxh.cucudq.cn

[S43] C++：智能指针
来源：http://qvr.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://kst.sysykeji.top

[S44] C++：引用传参
来源：http://kzq.yvedp.cn

void inc(int &x) { ++x; }
来源：http://ydz.hysaishi.cn

[S45] C++：lambda
来源：http://wpr.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://uat.yvedp.cn

[S46] C++：函数模板
来源：http://idf.guannengcc.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qcw.yangfankeji.com

[S47] C++：结构化绑定遍历
来源：http://qam.mhx1999.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bmq.ydzc1.top

[S48] C++：逐行读文件
来源：http://fdy.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://atg.ehwqpu.com

while (std::getline(in, line)) { }
来源：http://lqs.yfazqb.com

[S49] C++：写文件
来源：http://tce.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xho.mhx1999.top

[S50] C++：格式化数字
来源：http://kfx.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://clg.yfazqb.com

[S51] C++：显式类型转换
来源：http://tlh.uphjek.com

static_cast<double>(a) / b
来源：http://fmy.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://xlp.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://bys.yfazqb.com

[S53] C++：移动语义
来源：http://otn.uphjek.com

std::vector<int> w = std::move(v);
来源：http://xju.feifeiyinyue.top

[S54] C++：异常处理
来源：http://iub.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ons.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://unx.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wjj.yueranfly.top

[S56] C++：optional
来源：http://ikk.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nue.fehbvm.com

[S57] C++：编译期常量
来源：http://che.wangdashe.top

constexpr int N = 10;
来源：http://wmx.cdnleiting.top

[S58] C++：命名空间
来源：http://mnt.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://lla.aibaodan.cn

[S59] C++：静态断言
来源：http://wlw.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://swy.cheryme.top

[S60] C++：遍历并删除元素
来源：http://nas.hcnkem.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kez.shzxlz.cn

================================================================================
来源：http://ajm.pycfn.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://upl.nanxuanxn.top

================================================================================
来源：http://owb.zhiwuduotai.top

[T01] Kotlin：Hello World
来源：http://jhu.hnxiangtu.top

println("Hello")
来源：http://wli.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://rcy.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pfq.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://uao.gogol.net.cn

"值: $b"
来源：http://xgl.gzhubu.top

[T04] Kotlin：空安全
来源：http://mjc.zycfv.cn

val n: String? = null;  n?.length
来源：http://vkn.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://vhs.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vgx.yj20258.top

[T06] Kotlin：集合映射
来源：http://knq.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gtb.cashguo.top

[T07] Kotlin：集合过滤
来源：http://stq.jinqigufen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pyy.sxryk.cn

[T08] Kotlin：数据类
来源：http://ste.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://xzo.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://jwb.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://rtk.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://xgd.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://yto.tanke756.top

[T11] Kotlin：协程
来源：http://hev.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://iog.daxiang520.top

[T12] Kotlin：解构声明
来源：http://izq.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://jzq.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://pck.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://uta.zycfv.cn

[T14] Kotlin：循环
来源：http://cyp.hysaishi.cn

for (i in 1..10) println(i)
来源：http://zoa.hywenlv.cn

[T15] Kotlin：接口
来源：http://uxd.epnwcf.com

interface Shape { fun area(): Double }
来源：http://mto.gotoacloud.top

[T16] Swift：Hello World
来源：http://fnk.pengpengdd.cyou

print("Hello")
来源：http://fxj.ydjk.org.cn

[T17] Swift：变量与常量
来源：http://rve.jiagoushi.top

var a = 1;  let b = 2
来源：http://ncn.birdmap.top

[T18] Swift：字符串插值
来源：http://ewz.sufxvd.cn

"值: \(b)"
来源：http://ulp.tian-w.cn

[T19] Swift：可选绑定
来源：http://rfq.zhongyouzk.top

if let n = opt { print(n) }
来源：http://rju.wangdashe.top

[T20] Swift：数组操作
来源：http://gor.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cvf.ppjwa.cn

[T21] Swift：遍历
来源：http://gxk.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://fkh.svipenyu.cn

[T22] Swift：字典
来源：http://twr.zhixingplan.top

var d = ["a": 1];  d["b"] = 2
来源：http://rkh.ivvv.top

[T23] Swift：函数
来源：http://cpc.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ssy.bjfxy.top

[T24] Swift：闭包
来源：http://ucl.vehdjk.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://byl.zhiwuduotai.top

[T25] Swift：结构体
来源：http://cfv.jiagoushi.top

struct P { var x: Int }
来源：http://ofk.hfpthk.cn

[T26] Swift：类与重写
来源：http://jnh.hammf.cn

class A: Base { override func f() {} }
来源：http://rxu.pycfn.com

[T27] Swift：错误处理
来源：http://bwy.shuidangran.top

do { try f() } catch { print(error) }
来源：http://qju.yfazqb.com

[T28] Swift：枚举
来源：http://oze.epnwcf.com

enum Color { case red, green }
来源：http://xfz.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://ikw.haohaochexian.top

guard let x = opt else { return }
来源：http://iui.sufxvd.cn

[T30] Swift：协议
来源：http://uvd.jiagoushi.top

protocol Shape { func area() -> Double }
来源：http://gdm.hnxiangtu.top

[T31] Lua：Hello World
来源：http://oyw.yanxiufei.cn

print("Hello")
来源：http://vgd.shuidangran.top

[T32] Lua：局部变量
来源：http://six.smart0.xyz

local a = 1
来源：http://dzu.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://lah.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ara.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://oqv.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tlj.shzxlz.cn

[T35] Lua：字典表
来源：http://ghv.guowangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://rra.bbcook.cn

[T36] Lua：函数
来源：http://qvb.jqgufenzy.top

function add(a, b) return a + b end
来源：http://xpt.hnqzz.top

[T37] Lua：字符串拼接
来源：http://lxg.yanxiufei.cn

"a" .. "b"
来源：http://qhe.yj202588.top

[T38] Lua：条件
来源：http://cum.hcnkem.com

if x > 0 then print("正") end
来源：http://nnc.uphjek.com

[T39] Lua：模式匹配
来源：http://pek.gotoacloud.top

string.find(s, "%d+")
来源：http://lzf.quarkkingdee.top

[T40] Lua：元表
来源：http://exr.yueranfly.top

setmetatable({}, { __index = base })
来源：http://qpr.bbcook.cn

[T41] Perl：Hello World
来源：http://rzi.quarkkingdee.top

print "Hello\n";
来源：http://lpw.iojbl.cn

[T42] Perl：变量类型
来源：http://sah.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lyz.yonumen.top

[T43] Perl：字符串插值
来源：http://onc.sweek.top

"值: $a"
来源：http://muv.sweek.top

[T44] Perl：条件
来源：http://tif.chenzaomai.com

if ($a > 0) { print "正"; }
来源：http://clo.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://eav.gzhubu.top

for my $x (@arr) { print $x; }
来源：http://yix.hnqzz.top

[T46] Perl：哈希操作
来源：http://cek.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rtc.redwolf501.top

[T47] Perl：正则捕获
来源：http://iwb.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://awj.ydzc1.top

[T48] Perl：正则替换
来源：http://zto.cqqwz.cn

$s =~ s/old/new/g;
来源：http://fsn.jiagoushi.top

[T49] Perl：函数
来源：http://qsg.nwbrower.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tas.sufxvd.cn

[T50] Perl：逐行读文件
来源：http://kst.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hke.andypj.xyz

while (my $line = <$fh>) { print $line; }
来源：http://ppl.hnxiangtu.top

[T51] Scala：Hello World
来源：http://qwt.shanyushiyangkeji.top

println("Hello")
来源：http://xzg.daxiang520.top

[T52] Scala：变量
来源：http://oun.nanxinkj.top

val a = 1;  var b = 2
来源：http://prj.zhoulong.xyz

[T53] Scala：字符串插值
来源：http://hmc.guannengcc.top

s"值: $b"
来源：http://bku.jqgufenzy.top

[T54] Scala：集合映射
来源：http://qhf.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://zbo.zhixingplan.top

[T55] Scala：集合过滤
来源：http://njx.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://qfa.gzhubu.top

[T56] Scala：样例类
来源：http://rkt.hnqzz.top

case class User(name: String, age: Int)
来源：http://qtm.yuxming.cn

[T57] Scala：模式匹配
来源：http://vrw.uphjek.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://jbu.9152youxi.cn

[T58] Scala：函数定义
来源：http://dzt.fanxiaobao.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://fsg.chenzaomai.com

[T59] Scala：循环
来源：http://suf.ybcxt.top

for (i <- 1 to 10) println(i)
来源：http://chq.zhiwuduotai.top

[T60] Scala：折叠
来源：http://eno.haohaochexian.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uas.havefunace.top

================================================================================
来源：http://tza.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lnd.daria6918.cn

================================================================================
来源：http://ekr.nwbrower.top

[U01] Py：创建虚拟环境
来源：http://bno.epnwcf.com

python -m venv .venv && source .venv/bin/activate
来源：http://ffb.quarkkingdee.top

[U02] Py：导出 / 安装依赖
来源：http://bfc.vqdsnc.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fqr.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://igx.epnwcf.com

from dotenv import load_dotenv; load_dotenv()
来源：http://gmn.iojbl.cn

[U04] Py：变量调试打印
来源：http://dil.fzhhl.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pex.aizwys.cn

[U05] Py：列表去重且保序
来源：http://hzq.c1oappe.top

list(dict.fromkeys(arr))
来源：http://sjv.svipenyu.cn

[U06] Py：合并两个字典
来源：http://zrz.iojbl.cn

{**a, **b}
来源：http://paa.smart0.xyz

[U07] Py：反转字典键值
来源：http://afr.zycfv.cn

{v: k for k, v in d.items()}
来源：http://ost.haohaochexian.top

[U08] Py：展平二维列表
来源：http://ffl.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://iyz.kuanghao11.cn

[U09] Py：字典取最大值的键
来源：http://zfd.aizwys.cn

max(d, key=d.get)
来源：http://wuy.316326.xyz

[U10] Py：按值排序字典
来源：http://cgb.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tam.zhiwuduotai.top

[U11] Py：生成器表达式
来源：http://day.zhoulong.xyz

(x * 2 for x in arr)
来源：http://zun.jinqigfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://zcj.fehbvm.com

Counter(arr).most_common(3)
来源：http://gdl.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://hhr.jinqigfzy.top

deque(maxlen=10)
来源：http://qff.fzhhl.top

[U14] Py：分组收集到列表
来源：http://osp.kuanghao11.cn

defaultdict(list)
来源：http://jgv.gaohongyu789.top


<!-- 参考信息 -->