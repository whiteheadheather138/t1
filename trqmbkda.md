代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://jih.ydjk.org.cn

[R72] 等待端口就绪
来源：http://ewt.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mxc.hnxiangtu.top

[R73] 分割大日志
来源：http://pse.xinyue.icu

split -l 1000 big.log part_
来源：http://mil.yueranfly.top

[R74] 批量重命名
来源：http://mit.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://flz.jqgufenzy.top

[R75] 导出环境变量
来源：http://cjb.hcnkem.com

export PATH="$HOME/bin:$PATH"
来源：http://xvp.hysaishi.cn

[R76] 使用临时文件
来源：http://pdj.c1oappe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://diy.hesvh.cn

[R77] 读取用户输入
来源：http://jdn.yj20258888.top

read -rp "请输入: " ans
来源：http://osn.guannengcc.top

[R78] 交互式菜单
来源：http://zku.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://djn.xinyue.icu

[R79] 解析命令行选项
来源：http://ykk.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lvm.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://nqb.bjfxy.top

time ./run.sh
来源：http://mra.sweek.top

================================================================================
来源：http://fyy.hcnkem.com

S. C / C++ 专题
来源：http://xwn.gogol.net.cn

================================================================================
来源：http://juj.zhongyouzk.top

[S01] C：Hello World
来源：http://oty.shanyushiyangkeji.top

#include <stdio.h>
来源：http://osu.shangyingyoupin.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wjh.cheryme.top

[S02] C：变量与格式化输出
来源：http://ifx.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://zcf.pycfn.com

[S03] C：读入整数
来源：http://nwi.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://gtt.snrcjt.cn

[S04] C：字符串复制
来源：http://gsq.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://vek.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://hzc.sjlbkw.cn

strlen(s)
来源：http://pdo.ivvv.top

[S06] C：字符串比较
来源：http://vui.daria6918.cn

strcmp(a, b) == 0
来源：http://yld.yonumen.top

[S07] C：数组遍历求和
来源：http://fzd.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ddz.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://mwo.meibo888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ncl.ydjk.org.cn

[S09] C：结构体定义与初始化
来源：http://qvt.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jdy.hammf.cn

[S10] C：指针与解引用
来源：http://jqc.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://plz.sufxvd.cn

[S11] C：逐行读文件
来源：http://mdo.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://dhx.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ote.ydjk.org.cn

fclose(f);
来源：http://bxk.jinqigfzy.top

[S12] C：写文件
来源：http://mxr.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zpo.cdnleiting.top

[S13] C：宏定义
来源：http://rpw.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cqy.sysykeji.top

[S14] C：枚举
来源：http://sli.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://bud.ydzc1.top

[S15] C：类型转换
来源：http://qvx.nwbrower.top

(double) a / b
来源：http://nhu.yvedp.cn

[S16] C：位操作置位
来源：http://fkg.tian-w.cn

x |= (1 << 3);
来源：http://fte.zhoulong.xyz

[S17] C：安全拼接字符串
来源：http://fsm.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://idk.hnxiangtu.top

[S18] C：命令行参数
来源：http://rzz.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://ooq.hywenlv.cn

[S19] C：快速排序
来源：http://lty.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://vwf.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://lwe.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eyo.havefunace.top

[S21] C：字符类别判断
来源：http://glu.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mse.quarkkingdee.top

[S22] C：字符串转数字
来源：http://aum.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://vly.bjfxy.top

[S23] C：随机数
来源：http://mtt.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hpy.cashguo.top

[S24] C：获取本地时间
来源：http://qzu.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://thy.xziqi.cn

[S25] C：内存拷贝
来源：http://xgz.jyoumei.cn

memcpy(dst, src, n);
来源：http://rmt.cdnleiting.top

[S26] C：内存清零
来源：http://dfs.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://avf.nanxinkj.top

[S27] C：定义常量
来源：http://xiy.birdmap.top

const double PI = 3.14159;
来源：http://psz.ydzc1.top

[S28] C：静态变量
来源：http://tnz.zhaomingkeji.xyz

static int counter = 0;
来源：http://szc.snrcjt.cn

[S29] C：变参函数
来源：http://dqc.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://naa.fengsongda.top

[S30] C：头文件保护
来源：http://nby.yangfankeji.com

#ifndef X_H
来源：http://xxp.fzhhl.top

#define X_H
来源：http://est.zhiwuduotai.top

#endif
来源：http://fwz.hesvh.cn

[S31] C++：Hello World
来源：http://ncl.ydzc1.top

#include <iostream>
来源：http://xkh.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://mit.birdmap.top

[S32] C++：字符串
来源：http://gzl.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://ibx.ydjk.org.cn

[S33] C++：vector 增删
来源：http://mcx.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nku.dianchejie.cn

[S34] C++：遍历 vector
来源：http://qfx.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://woa.andypj.xyz

[S35] C++：map
来源：http://wmv.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ptu.chenzaomai.com

[S36] C++：unordered_map
来源：http://uyh.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ueu.fengsongda.top

[S37] C++：set
来源：http://ocw.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cyr.yongpay.top

[S38] C++：排序
来源：http://ver.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://ueq.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://bmz.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hsk.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://oaj.mhx1999.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ftd.cheryme.top

[S41] C++：类与构造函数
来源：http://urk.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qqb.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://nge.snrcjt.cn

class B : public Base { public: void f() override {} };
来源：http://rjz.zhoulong.xyz

[S43] C++：智能指针
来源：http://ybi.shzxlz.cn

auto p = std::make_unique<int>(5);
来源：http://knk.redwolf501.top

[S44] C++：引用传参
来源：http://qwm.ywan-chungtsiang.top

void inc(int &x) { ++x; }
来源：http://vgw.daria6918.cn

[S45] C++：lambda
来源：http://jfm.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tnb.fktsv.cn

[S46] C++：函数模板
来源：http://kpp.c1oappe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nlv.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://zqk.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jdr.cdnleiting.top

[S48] C++：逐行读文件
来源：http://oje.hnxiangtu.top

std::ifstream in("a.txt");  std::string line;
来源：http://uqn.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://uxl.shuidangran.top

[S49] C++：写文件
来源：http://jek.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tjq.meibo888.top

[S50] C++：格式化数字
来源：http://yvx.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://umx.zhengqikj.top

[S51] C++：显式类型转换
来源：http://mzs.tarul.cn

static_cast<double>(a) / b
来源：http://beb.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://vcc.meibo888.top

int size() const noexcept { return n_; }
来源：http://lau.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://atk.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://fjp.52xcode.cn

[S54] C++：异常处理
来源：http://rpq.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ebj.guannengcc.top

[S55] C++：结构化绑定
来源：http://phe.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ibk.daria6918.cn

[S56] C++：optional
来源：http://qua.yonumen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lzl.cdnleiting.top

[S57] C++：编译期常量
来源：http://wcc.epnwcf.com

constexpr int N = 10;
来源：http://qba.sysykeji.top

[S58] C++：命名空间
来源：http://skp.aibaodan.cn

namespace ns { int f() { return 1; } }
来源：http://fwn.zhengqikj.top

[S59] C++：静态断言
来源：http://uvy.gzhubu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eyb.fehbvm.com

[S60] C++：遍历并删除元素
来源：http://pbh.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kyj.xylfe.cn

================================================================================
来源：http://tge.shanyushiyangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jlv.jyoumei.cn

================================================================================
来源：http://jav.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://ryf.ppjwa.cn

println("Hello")
来源：http://tir.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://cyg.jqgufenzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sme.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://qhq.smart0.xyz

"值: $b"
来源：http://jby.gotoacloud.top

[T04] Kotlin：空安全
来源：http://lsr.zhongyouzk.top

val n: String? = null;  n?.length
来源：http://yxf.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://rjx.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gbl.sweek.top

[T06] Kotlin：集合映射
来源：http://sfx.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://czm.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://bjx.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rqk.ydzc1.top

[T08] Kotlin：数据类
来源：http://xer.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://ayy.gogol.net.cn

[T09] Kotlin：扩展函数
来源：http://ark.cheryme.top

fun String.exclaim() = this + "!"
来源：http://cvw.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://tkc.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fpi.svipenyu.cn

[T11] Kotlin：协程
来源：http://onr.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://bts.gzhubu.top

[T12] Kotlin：解构声明
来源：http://eyf.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://vni.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://rlz.jinqigufen.top

val m = mapOf("a" to 1)
来源：http://jsc.jinqigfzy.top

[T14] Kotlin：循环
来源：http://zpj.yvedp.cn

for (i in 1..10) println(i)
来源：http://oen.ctjpmb.com

[T15] Kotlin：接口
来源：http://ikb.tanke756.top

interface Shape { fun area(): Double }
来源：http://xmt.andypj.xyz

[T16] Swift：Hello World
来源：http://wva.jlsjyb.cn

print("Hello")
来源：http://whl.bjfxy.top

[T17] Swift：变量与常量
来源：http://rtf.sxryk.cn

var a = 1;  let b = 2
来源：http://sgb.ydzc1.top

[T18] Swift：字符串插值
来源：http://sso.quarkkingdee.top

"值: \(b)"
来源：http://uee.zhiwuduotai.top

[T19] Swift：可选绑定
来源：http://lhn.ybcxt.top

if let n = opt { print(n) }
来源：http://ugw.ybcxt.top

[T20] Swift：数组操作
来源：http://fwk.fengsongda.top

var a = [1, 2, 3];  a.append(4)
来源：http://qsr.zhiwuduotai.top

[T21] Swift：遍历
来源：http://pqs.havefunace.top

for x in a { print(x) }
来源：http://pzg.ydzc1.top

[T22] Swift：字典
来源：http://dfv.ehwqpu.com

var d = ["a": 1];  d["b"] = 2
来源：http://ufs.daxiang520.top

[T23] Swift：函数
来源：http://odn.zdqjudy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xkq.iojbl.cn

[T24] Swift：闭包
来源：http://ajp.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xbq.nanxinkj.top

[T25] Swift：结构体
来源：http://kbi.pycfn.com

struct P { var x: Int }
来源：http://wex.ybcxt.top

[T26] Swift：类与重写
来源：http://byh.yueranfly.top

class A: Base { override func f() {} }
来源：http://rbi.aizwys.cn

[T27] Swift：错误处理
来源：http://jwo.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://rxr.wangdashe.top

[T28] Swift：枚举
来源：http://gel.meibo888.top

enum Color { case red, green }
来源：http://qoe.dashuyun.cn

[T29] Swift：guard 提前返回
来源：http://lzj.sweek.top

guard let x = opt else { return }
来源：http://chs.wangshuangyany.cn

[T30] Swift：协议
来源：http://yaw.ydjk.org.cn

protocol Shape { func area() -> Double }
来源：http://jqf.andypj.xyz

[T31] Lua：Hello World
来源：http://gwt.zdqjudy.top

print("Hello")
来源：http://kfj.dashuyun.cn

[T32] Lua：局部变量
来源：http://yzn.gogol.net.cn

local a = 1
来源：http://ogi.mhx1999.top

[T33] Lua：表（数组）
来源：http://cvy.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bjc.cdnleiting.top

[T34] Lua：遍历表
来源：http://bth.bjfxy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://klr.zdbjq.cn

[T35] Lua：字典表
来源：http://vsl.fktsv.cn

local d = { a = 1 };  d.b = 2
来源：http://tlo.vehdjk.com

[T36] Lua：函数
来源：http://ytr.guowangkeji.top

function add(a, b) return a + b end
来源：http://umq.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://etb.sysykeji.top

"a" .. "b"
来源：http://mdd.jiagoushi.top

[T38] Lua：条件
来源：http://fsa.jianghu66.top

if x > 0 then print("正") end
来源：http://qfx.daria6918.cn

[T39] Lua：模式匹配
来源：http://obv.wangdashe.top

string.find(s, "%d+")
来源：http://xjw.quarkkingdee.top

[T40] Lua：元表
来源：http://zsv.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://jos.cqqwz.cn

[T41] Perl：Hello World
来源：http://dhj.yongpay.top

print "Hello\n";
来源：http://acd.zdqjudy.top

[T42] Perl：变量类型
来源：http://ufs.epnwcf.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fpx.dianchejie.cn

[T43] Perl：字符串插值
来源：http://fij.chenlongwang.top

"值: $a"
来源：http://ggj.andypj.xyz

[T44] Perl：条件
来源：http://dkm.yongpay.top

if ($a > 0) { print "正"; }
来源：http://fsa.ctjpmb.com

[T45] Perl：数组遍历
来源：http://dts.zhengqikj.top

for my $x (@arr) { print $x; }
来源：http://cux.shanyushiyangkeji.top

[T46] Perl：哈希操作
来源：http://ond.jqgfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hlo.hywenlv.cn

[T47] Perl：正则捕获
来源：http://hkg.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vfg.zhixingplan.top

[T48] Perl：正则替换
来源：http://bdw.ehwqpu.com

$s =~ s/old/new/g;
来源：http://qsh.gogol.net.cn

[T49] Perl：函数
来源：http://svs.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kev.yj20258.top

[T50] Perl：逐行读文件
来源：http://nyj.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kur.316326.xyz

while (my $line = <$fh>) { print $line; }
来源：http://tlu.yvedp.cn

[T51] Scala：Hello World
来源：http://jcn.vehdjk.com

println("Hello")
来源：http://tmf.zycfv.cn

[T52] Scala：变量
来源：http://gup.jiagoushi.top

val a = 1;  var b = 2
来源：http://ogc.nanxinkj.top

[T53] Scala：字符串插值
来源：http://wrm.tian-w.cn

s"值: $b"
来源：http://uvv.havefunace.top

[T54] Scala：集合映射
来源：http://uvw.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://xse.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://zbv.c1oappe.top

List(1, 2, 3).filter(_ > 1)
来源：http://mcw.xylfe.cn

[T56] Scala：样例类
来源：http://hht.52xcode.cn

case class User(name: String, age: Int)
来源：http://vam.svipenyu.cn

[T57] Scala：模式匹配
来源：http://idy.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://slt.birdmap.top

[T58] Scala：函数定义
来源：http://cjv.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fgc.sjlbkw.cn

[T59] Scala：循环
来源：http://fes.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://qzd.yangfankeji.com

[T60] Scala：折叠
来源：http://gzc.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gaf.cucudq.cn

================================================================================
来源：http://xbm.bbcook.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://htp.nanxinkj.top

================================================================================
来源：http://cyf.pengpengdd.cyou

[U01] Py：创建虚拟环境
来源：http://mvx.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://zds.cdnleiting.top

[U02] Py：导出 / 安装依赖
来源：http://yzg.andypj.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bri.xziqi.cn

[U03] Py：加载 .env 配置
来源：http://nen.yongpay.top

from dotenv import load_dotenv; load_dotenv()
来源：http://quz.52xcode.cn

[U04] Py：变量调试打印
来源：http://zyj.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qqd.guannengcc.top

[U05] Py：列表去重且保序
来源：http://kzo.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://cly.haohaochexian.top

[U06] Py：合并两个字典
来源：http://qdx.zhoulong.xyz

{**a, **b}
来源：http://lhe.yj202588.top

[U07] Py：反转字典键值
来源：http://hss.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://ffz.iojbl.cn

[U08] Py：展平二维列表
来源：http://vdj.shanyushiyangtech.top

[y for x in nested for y in x]
来源：http://fyu.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://nde.quarkkingdee.top

max(d, key=d.get)
来源：http://ydo.snrcjt.cn

[U10] Py：按值排序字典
来源：http://wgm.ivvv.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tqg.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://pio.snrcjt.cn

(x * 2 for x in arr)
来源：http://swa.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://bkr.uphjek.com

Counter(arr).most_common(3)
来源：http://fmg.zdbjq.cn


<!-- 参考信息 -->