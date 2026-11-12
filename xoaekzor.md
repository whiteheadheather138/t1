代发 wailian999

read -rp "请输入: " ans
来源：http://gsa.nanxuanxn.top

[R78] 交互式菜单
来源：http://dvl.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gad.hammf.cn

[R79] 解析命令行选项
来源：http://ihh.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iyo.dianchejie.cn

[R80] 查看脚本执行耗时
来源：http://sld.chenlongwang.top

time ./run.sh
来源：http://mge.jinghuilouyu.cn

================================================================================
来源：http://kye.316326.xyz

S. C / C++ 专题
来源：http://vfd.ybcxt.top

================================================================================
来源：http://elg.havefunace.top

[S01] C：Hello World
来源：http://kry.fanxiaobao.xyz

#include <stdio.h>
来源：http://agi.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://kbl.vehdjk.com

[S02] C：变量与格式化输出
来源：http://hjg.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://wba.yangfankeji.com

[S03] C：读入整数
来源：http://ond.zhongyouzk.top

int x; scanf("%d", &x);
来源：http://bbq.yj202588.top

[S04] C：字符串复制
来源：http://nqo.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://ffc.hfpthk.cn

[S05] C：字符串长度
来源：http://enp.zdbjq.cn

strlen(s)
来源：http://cig.jinqigufen.top

[S06] C：字符串比较
来源：http://ryz.gogol.net.cn

strcmp(a, b) == 0
来源：http://mcr.yonumen.top

[S07] C：数组遍历求和
来源：http://fwb.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vmt.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://glu.ehwqpu.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ope.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://bqc.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://edr.hywenlv.cn

[S10] C：指针与解引用
来源：http://nlo.nanxinkj.top

int *p = &a;  *p = 5;
来源：http://adf.yuanzhike.top

[S11] C：逐行读文件
来源：http://pqs.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://dmj.sjlbkw.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cyr.ehwqpu.com

fclose(f);
来源：http://uci.jinqigufen.top

[S12] C：写文件
来源：http://csn.xinyue.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vih.fehbvm.com

[S13] C：宏定义
来源：http://fya.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dod.zhaomingkeji.xyz

[S14] C：枚举
来源：http://ybp.redwolf501.top

enum Color { RED, GREEN, BLUE };
来源：http://rsn.jinyuanbaomall.cn

[S15] C：类型转换
来源：http://mue.shanyushiyangkeji.top

(double) a / b
来源：http://cmc.redwolf501.top

[S16] C：位操作置位
来源：http://xoe.gogol.net.cn

x |= (1 << 3);
来源：http://uoo.xylfe.cn

[S17] C：安全拼接字符串
来源：http://iuf.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qdd.hnqzz.top

[S18] C：命令行参数
来源：http://jbo.xziqi.cn

int main(int argc, char **argv)
来源：http://tqr.jinqigufen.top

[S19] C：快速排序
来源：http://wau.hongshengwenyu.top

qsort(a, n, sizeof(int), cmp);
来源：http://mwa.yanxiufei.cn

[S20] C：二分查找
来源：http://vou.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wld.mhx1999.top

[S21] C：字符类别判断
来源：http://pgl.chenzaomai.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jhf.c1oappe.top

[S22] C：字符串转数字
来源：http://irm.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://hfo.zdqjudy.top

[S23] C：随机数
来源：http://cmx.hammf.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://igh.chenlongwang.top

[S24] C：获取本地时间
来源：http://vdj.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xmn.guannengcc.top

[S25] C：内存拷贝
来源：http://enz.yueranfly.top

memcpy(dst, src, n);
来源：http://qla.ppjwa.cn

[S26] C：内存清零
来源：http://swq.aizwys.cn

memset(a, 0, sizeof a);
来源：http://uvo.tian-w.cn

[S27] C：定义常量
来源：http://jty.epnwcf.com

const double PI = 3.14159;
来源：http://urd.jianghu66.top

[S28] C：静态变量
来源：http://rzt.tanke756.top

static int counter = 0;
来源：http://nbl.tanke756.top

[S29] C：变参函数
来源：http://oiq.ybcxt.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wmx.wangshuangyany.cn

[S30] C：头文件保护
来源：http://kgx.gotoacloud.top

#ifndef X_H
来源：http://fbz.tarul.cn

#define X_H
来源：http://chw.yj20258888.top

#endif
来源：http://yfc.snrcjt.cn

[S31] C++：Hello World
来源：http://xpu.shanyushiyangkeji.top

#include <iostream>
来源：http://tgj.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://bsq.chenzaomai.com

[S32] C++：字符串
来源：http://gxr.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://yvf.hcnkem.com

[S33] C++：vector 增删
来源：http://kwx.uphjek.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://isz.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://vjr.ppjwa.cn

for (auto &x : v) { std::cout << x; }
来源：http://tgz.iojbl.cn

[S35] C++：map
来源：http://lxf.cheryme.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://syn.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://ktx.gogol.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uik.bjfxy.top

[S37] C++：set
来源：http://arb.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dzl.redwolf501.top

[S38] C++：排序
来源：http://hre.yj20258.top

std::sort(v.begin(), v.end());
来源：http://ibb.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://wgv.chenlongwang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://igd.vqdsnc.cn

[S40] C++：查找元素
来源：http://poq.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rrl.hcnkem.com

[S41] C++：类与构造函数
来源：http://dgu.sweek.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jjx.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://dpi.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://pcy.wangshuangyany.cn

[S43] C++：智能指针
来源：http://ozu.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://sey.yuanzhike.top

[S44] C++：引用传参
来源：http://chb.xziqi.cn

void inc(int &x) { ++x; }
来源：http://fes.hcnkem.com

[S45] C++：lambda
来源：http://ifa.ywan-chungtsiang.top

auto add = [](int a, int b) { return a + b; };
来源：http://ohs.hongshengwenyu.top

[S46] C++：函数模板
来源：http://hwf.wangdashe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ytr.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://thx.bjfxy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nsz.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://rod.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://cwg.hcnkem.com

while (std::getline(in, line)) { }
来源：http://bfp.fktsv.cn

[S49] C++：写文件
来源：http://uso.sjlbkw.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zuw.hnqzz.top

[S50] C++：格式化数字
来源：http://evt.shangyingyoupin.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mhp.haohaochexian.top

[S51] C++：显式类型转换
来源：http://aef.cdnleiting.top

static_cast<double>(a) / b
来源：http://vlm.gogol.net.cn

[S52] C++：const 与 noexcept
来源：http://cmj.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://gnz.vehdjk.com

[S53] C++：移动语义
来源：http://btc.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://dsp.ydzc1.top

[S54] C++：异常处理
来源：http://uwg.hywenlv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://unw.redwolf501.top

[S55] C++：结构化绑定
来源：http://oqk.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sgb.tian-w.cn

[S56] C++：optional
来源：http://zhu.guannengcc.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ezc.hnxiangtu.top

[S57] C++：编译期常量
来源：http://znu.meibo888.top

constexpr int N = 10;
来源：http://eun.dashuyun.cn

[S58] C++：命名空间
来源：http://wfr.sxryk.cn

namespace ns { int f() { return 1; } }
来源：http://ssu.aibaodan.cn

[S59] C++：静态断言
来源：http://pag.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jdt.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://xdi.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yrg.guowangkeji.top

================================================================================
来源：http://tyw.yj20258888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://avy.xuanzx.com

================================================================================
来源：http://bgq.havefunace.top

[T01] Kotlin：Hello World
来源：http://xyz.ppjwa.cn

println("Hello")
来源：http://izh.fktsv.cn

[T02] Kotlin：变量
来源：http://zmv.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://frp.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://yks.cheryme.top

"值: $b"
来源：http://nvs.c1oappe.top

[T04] Kotlin：空安全
来源：http://amu.hnqzz.top

val n: String? = null;  n?.length
来源：http://faw.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://vmi.chenlongwang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pgk.hesvh.cn

[T06] Kotlin：集合映射
来源：http://kyv.yuxming.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yzd.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://aly.pycfn.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://tab.chenjidiqi.icu

[T08] Kotlin：数据类
来源：http://qbm.hammf.cn

data class User(val name: String, val age: Int)
来源：http://zbi.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://zkg.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://gpz.tianlin.xyz

[T10] Kotlin：默认参数
来源：http://rhx.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mfp.pycfn.com

[T11] Kotlin：协程
来源：http://pww.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mwi.yj20258.top

[T12] Kotlin：解构声明
来源：http://ggn.sufxvd.cn

val (a, b) = Pair(1, 2)
来源：http://txb.bbcook.cn

[T13] Kotlin：只读 Map
来源：http://xeg.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://kym.smart0.xyz

[T14] Kotlin：循环
来源：http://wlp.cheryme.top

for (i in 1..10) println(i)
来源：http://uzy.vqdsnc.cn

[T15] Kotlin：接口
来源：http://qwi.vehdjk.com

interface Shape { fun area(): Double }
来源：http://ywr.vehdjk.com

[T16] Swift：Hello World
来源：http://ehn.guowangkeji.top

print("Hello")
来源：http://znd.sxryk.cn

[T17] Swift：变量与常量
来源：http://jdf.cheryme.top

var a = 1;  let b = 2
来源：http://vnb.c1oappe.top

[T18] Swift：字符串插值
来源：http://emd.iojbl.cn

"值: \(b)"
来源：http://thh.9152youxi.cn

[T19] Swift：可选绑定
来源：http://hjr.nanxuanxn.top

if let n = opt { print(n) }
来源：http://sqy.yuanzhike.top

[T20] Swift：数组操作
来源：http://yha.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zdx.sufxvd.cn

[T21] Swift：遍历
来源：http://yac.vqdsnc.cn

for x in a { print(x) }
来源：http://fpi.chenzaomai.com

[T22] Swift：字典
来源：http://oxk.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fsa.pengpengdd.cyou

[T23] Swift：函数
来源：http://hco.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hoj.tanke756.top

[T24] Swift：闭包
来源：http://lle.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://zld.fengsongda.top

[T25] Swift：结构体
来源：http://usd.ctjpmb.com

struct P { var x: Int }
来源：http://vjt.yfazqb.com

[T26] Swift：类与重写
来源：http://smy.fzhhl.top

class A: Base { override func f() {} }
来源：http://tdz.haohaochexian.top

[T27] Swift：错误处理
来源：http://dtq.daxiang520.top

do { try f() } catch { print(error) }
来源：http://rmg.nanxinkj.top

[T28] Swift：枚举
来源：http://mgo.redwolf501.top

enum Color { case red, green }
来源：http://dwq.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://gfs.cheryme.top

guard let x = opt else { return }
来源：http://brv.sxryk.cn

[T30] Swift：协议
来源：http://frc.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://wdo.zdbjq.cn

[T31] Lua：Hello World
来源：http://ptt.hysaishi.cn

print("Hello")
来源：http://ifu.wangdashe.top

[T32] Lua：局部变量
来源：http://smd.jinyuanbaomall.cn

local a = 1
来源：http://vyb.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://gjg.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://eqq.hnqzz.top

[T34] Lua：遍历表
来源：http://vdg.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dzj.yanxiufei.cn

[T35] Lua：字典表
来源：http://gkt.jyoumei.cn

local d = { a = 1 };  d.b = 2
来源：http://hun.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://wia.jqgufenzy.top

function add(a, b) return a + b end
来源：http://rhc.shanyushiyangtech.top

[T37] Lua：字符串拼接
来源：http://ktg.hammf.cn

"a" .. "b"
来源：http://qrm.jinqigufen.top

[T38] Lua：条件
来源：http://ilv.hysaishi.cn

if x > 0 then print("正") end
来源：http://ezw.cdnleiting.top

[T39] Lua：模式匹配
来源：http://jzu.pycfn.com

string.find(s, "%d+")
来源：http://umx.tian-w.cn

[T40] Lua：元表
来源：http://vye.yonumen.top

setmetatable({}, { __index = base })
来源：http://awo.pycfn.com

[T41] Perl：Hello World
来源：http://bvm.chenzaomai.com

print "Hello\n";
来源：http://dwf.havefunace.top

[T42] Perl：变量类型
来源：http://owk.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://skn.tarul.cn

[T43] Perl：字符串插值
来源：http://rsi.yj20258.top

"值: $a"
来源：http://nfe.nanxuanxn.top

[T44] Perl：条件
来源：http://sdb.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://puf.gogol.net.cn

[T45] Perl：数组遍历
来源：http://quj.cqqwz.cn

for my $x (@arr) { print $x; }
来源：http://agl.cqqwz.cn

[T46] Perl：哈希操作
来源：http://ysb.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vkt.gaohongyu789.top

[T47] Perl：正则捕获
来源：http://szx.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://xfr.sjlbkw.cn

[T48] Perl：正则替换
来源：http://pjf.ppjwa.cn

$s =~ s/old/new/g;
来源：http://rfi.fktsv.cn

[T49] Perl：函数
来源：http://zyx.9152youxi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tlt.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://rxz.316326.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://jwe.gotoacloud.top

while (my $line = <$fh>) { print $line; }
来源：http://gru.yonumen.top

[T51] Scala：Hello World
来源：http://qnf.ehwqpu.com

println("Hello")
来源：http://ehm.dashuyun.cn

[T52] Scala：变量
来源：http://vji.jlsjyb.cn

val a = 1;  var b = 2
来源：http://hky.cucudq.cn

[T53] Scala：字符串插值
来源：http://pbw.vqdsnc.cn

s"值: $b"
来源：http://gqo.xuanzx.com

[T54] Scala：集合映射
来源：http://cxs.sxryk.cn

List(1, 2, 3).map(_ * 2)
来源：http://ifq.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://tij.zhongyouzk.top

List(1, 2, 3).filter(_ > 1)
来源：http://ypr.redwolf501.top

[T56] Scala：样例类
来源：http://qsm.cucudq.cn

case class User(name: String, age: Int)
来源：http://rhj.aibaodan.cn

[T57] Scala：模式匹配
来源：http://hpa.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://bfg.shuidangran.top

[T58] Scala：函数定义
来源：http://rcr.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://uqq.chenzaomai.com

[T59] Scala：循环
来源：http://kkr.shanyushiyangkeji.top

for (i <- 1 to 10) println(i)
来源：http://umw.wangdashe.top

[T60] Scala：折叠
来源：http://wqp.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://win.vehdjk.com

================================================================================
来源：http://suk.nanxinkj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://obr.yanxiufei.cn

================================================================================
来源：http://sqa.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://fon.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wvi.aibaodan.cn

[U02] Py：导出 / 安装依赖
来源：http://vgk.gzhubu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rhe.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://qll.vqdsnc.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lcs.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://pzi.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nwu.shuidangran.top

[U05] Py：列表去重且保序
来源：http://efg.52xcode.cn

list(dict.fromkeys(arr))
来源：http://jqh.9152youxi.cn

[U06] Py：合并两个字典
来源：http://hkb.yueranfly.top

{**a, **b}
来源：http://vla.cashguo.top

[U07] Py：反转字典键值
来源：http://emm.mhx1999.top

{v: k for k, v in d.items()}
来源：http://cbb.guowangkeji.top

[U08] Py：展平二维列表
来源：http://hrn.jqgfzy.top

[y for x in nested for y in x]
来源：http://kxc.andypj.xyz

[U09] Py：字典取最大值的键
来源：http://sns.xziqi.cn

max(d, key=d.get)
来源：http://qnn.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://yoi.gotoacloud.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mcj.wangdashe.top

[U11] Py：生成器表达式
来源：http://xwq.iojbl.cn

(x * 2 for x in arr)
来源：http://arz.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://zzt.fktsv.cn

Counter(arr).most_common(3)
来源：http://lxe.daria6918.cn

[U13] Py：固定长度队列
来源：http://viy.yj20258.top

deque(maxlen=10)
来源：http://jcw.xylfe.cn

[U14] Py：分组收集到列表
来源：http://ncn.aibaodan.cn

defaultdict(list)
来源：http://lsm.zhixingplan.top

[U15] Py：高精度计时
来源：http://clm.yonumen.top

t = time.perf_counter()
来源：http://ack.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://zah.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dgg.jianghu66.top

[U17] Py：初始化日志
来源：http://nut.redwolf501.top

logging.basicConfig(level=logging.INFO)
来源：http://avm.ehwqpu.com

[U18] Py：预编译正则
来源：http://roi.shuidangran.top

pat = re.compile(r"\d+")
来源：http://ttf.0kj1m.cn


<!-- 参考信息 -->