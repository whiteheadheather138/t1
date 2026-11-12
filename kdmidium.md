代发 wailian999

split -l 1000 big.log part_
来源：http://rcv.52xcode.cn

[R74] 批量重命名
来源：http://atb.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://igk.gotoacloud.top

[R75] 导出环境变量
来源：http://lnq.shanyushiyangtech.top

export PATH="$HOME/bin:$PATH"
来源：http://ngq.redwolf501.top

[R76] 使用临时文件
来源：http://hsx.cqqwz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ndk.hesvh.cn

[R77] 读取用户输入
来源：http://ilv.daria6918.cn

read -rp "请输入: " ans
来源：http://tci.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://asm.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://odz.aizwys.cn

[R79] 解析命令行选项
来源：http://gje.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eoi.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://jpp.ybcxt.top

time ./run.sh
来源：http://zkd.cucudq.cn

================================================================================
来源：http://mgy.xuanzx.com

S. C / C++ 专题
来源：http://ypy.ydzc1.top

================================================================================
来源：http://nzo.tian-w.cn

[S01] C：Hello World
来源：http://bkb.hfpthk.cn

#include <stdio.h>
来源：http://zyz.jiagoushi.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mmo.tanke756.top

[S02] C：变量与格式化输出
来源：http://ztc.chenzaomai.com

int a = 10; printf("%d\n", a);
来源：http://qba.sufxvd.cn

[S03] C：读入整数
来源：http://phg.xylfe.cn

int x; scanf("%d", &x);
来源：http://bld.gotoacloud.top

[S04] C：字符串复制
来源：http://xwz.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://xhp.hysaishi.cn

[S05] C：字符串长度
来源：http://ixb.chenjidiqi.icu

strlen(s)
来源：http://nis.ivvv.top

[S06] C：字符串比较
来源：http://teu.hesvh.cn

strcmp(a, b) == 0
来源：http://com.zdqjudy.top

[S07] C：数组遍历求和
来源：http://jiq.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xly.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://cod.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jzn.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://wtd.havefunace.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mga.zdqjudy.top

[S10] C：指针与解引用
来源：http://jzp.ppjwa.cn

int *p = &a;  *p = 5;
来源：http://zfg.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://foc.52xcode.cn

FILE *f = fopen("a.txt", "r");
来源：http://gbl.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yjr.ehwqpu.com

fclose(f);
来源：http://agl.yvedp.cn

[S12] C：写文件
来源：http://ejc.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bll.vehdjk.com

[S13] C：宏定义
来源：http://cwz.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uzc.yuanzhike.top

[S14] C：枚举
来源：http://bii.gzhubu.top

enum Color { RED, GREEN, BLUE };
来源：http://nbb.pengpengdd.cyou

[S15] C：类型转换
来源：http://wfm.yangfankeji.com

(double) a / b
来源：http://ipi.zhiwuduotai.top

[S16] C：位操作置位
来源：http://oof.zhaomingkeji.xyz

x |= (1 << 3);
来源：http://fhy.bjfxy.top

[S17] C：安全拼接字符串
来源：http://gxg.xylfe.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ccf.316326.xyz

[S18] C：命令行参数
来源：http://elt.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://ufm.tarul.cn

[S19] C：快速排序
来源：http://wzc.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://nqn.yvedp.cn

[S20] C：二分查找
来源：http://cot.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qrc.shangyingyoupin.top

[S21] C：字符类别判断
来源：http://ebp.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xmx.sufxvd.cn

[S22] C：字符串转数字
来源：http://cjf.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vfl.bjfxy.top

[S23] C：随机数
来源：http://nrt.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://bcb.tian-w.cn

[S24] C：获取本地时间
来源：http://neu.c1oappe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ejb.xinyue.icu

[S25] C：内存拷贝
来源：http://urp.vehdjk.com

memcpy(dst, src, n);
来源：http://klc.daria6918.cn

[S26] C：内存清零
来源：http://hoi.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://rnd.bbcook.cn

[S27] C：定义常量
来源：http://fip.hywenlv.cn

const double PI = 3.14159;
来源：http://uyt.pengpengdd.cyou

[S28] C：静态变量
来源：http://phe.vehdjk.com

static int counter = 0;
来源：http://wlp.ctjpmb.com

[S29] C：变参函数
来源：http://ikg.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mix.svipenyu.cn

[S30] C：头文件保护
来源：http://dbn.shzxlz.cn

#ifndef X_H
来源：http://vyl.gzhubu.top

#define X_H
来源：http://cof.zdqjudy.top

#endif
来源：http://cdt.andypj.xyz

[S31] C++：Hello World
来源：http://iui.aibaodan.cn

#include <iostream>
来源：http://mpz.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://ler.bbcook.cn

[S32] C++：字符串
来源：http://ahk.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://pge.zycfv.cn

[S33] C++：vector 增删
来源：http://qdf.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yzo.xylfe.cn

[S34] C++：遍历 vector
来源：http://asc.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://jzq.epnwcf.com

[S35] C++：map
来源：http://mrq.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jjd.zhongyouzk.top

[S36] C++：unordered_map
来源：http://xoi.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bss.yangfankeji.com

[S37] C++：set
来源：http://smi.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wgh.yfazqb.com

[S38] C++：排序
来源：http://ofa.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://mrn.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://tms.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baj.zhiwuduotai.top

[S40] C++：查找元素
来源：http://jbe.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sym.c1oappe.top

[S41] C++：类与构造函数
来源：http://psm.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gog.xziqi.cn

[S42] C++：继承与虚函数
来源：http://maj.cdnleiting.top

class B : public Base { public: void f() override {} };
来源：http://ern.yangfankeji.com

[S43] C++：智能指针
来源：http://bgb.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://hqy.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://zrp.ydjk.org.cn

void inc(int &x) { ++x; }
来源：http://lse.yvedp.cn

[S45] C++：lambda
来源：http://rrs.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://dac.aizwys.cn

[S46] C++：函数模板
来源：http://rsr.jianghu66.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tun.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://pfc.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lgi.shuidangran.top

[S48] C++：逐行读文件
来源：http://upo.chenlongwang.top

std::ifstream in("a.txt");  std::string line;
来源：http://qqk.yj20258888.top

while (std::getline(in, line)) { }
来源：http://taq.dashuyun.cn

[S49] C++：写文件
来源：http://oze.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yqc.hcnkem.com

[S50] C++：格式化数字
来源：http://lhz.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xvy.hysaishi.cn

[S51] C++：显式类型转换
来源：http://xpu.sjlbkw.cn

static_cast<double>(a) / b
来源：http://tel.birdmap.top

[S52] C++：const 与 noexcept
来源：http://nyf.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://oxx.yanxiufei.cn

[S53] C++：移动语义
来源：http://kul.bjfxy.top

std::vector<int> w = std::move(v);
来源：http://iuf.hongshengwenyu.top

[S54] C++：异常处理
来源：http://zdi.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lbt.fzhhl.top

[S55] C++：结构化绑定
来源：http://syn.fehbvm.com

auto [a, b] = std::make_pair(1, 2);
来源：http://mcr.shangyingyoupin.top

[S56] C++：optional
来源：http://qch.shangyingyoupin.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wzk.yj20258.top

[S57] C++：编译期常量
来源：http://yfs.cqqwz.cn

constexpr int N = 10;
来源：http://ekb.yj20258888.top

[S58] C++：命名空间
来源：http://hvg.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://dbl.hcnkem.com

[S59] C++：静态断言
来源：http://wzl.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://les.cashguo.top

[S60] C++：遍历并删除元素
来源：http://yod.hfpthk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jpp.ybcxt.top

================================================================================
来源：http://nvh.dianchejie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gug.dianchejie.cn

================================================================================
来源：http://nwz.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://fws.zdqjudy.top

println("Hello")
来源：http://rxz.yangfankeji.com

[T02] Kotlin：变量
来源：http://lfj.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vyy.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://viw.bbcook.cn

"值: $b"
来源：http://zja.yuxming.cn

[T04] Kotlin：空安全
来源：http://vnf.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://ruc.epnwcf.com

[T05] Kotlin：when 表达式
来源：http://qfn.zhixingplan.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vys.yueranfly.top

[T06] Kotlin：集合映射
来源：http://fpm.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dow.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://mqb.zhengqikj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://orx.aibaodan.cn

[T08] Kotlin：数据类
来源：http://zuf.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://ixa.cheryme.top

[T09] Kotlin：扩展函数
来源：http://gwi.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://jlp.hongshengwenyu.top

[T10] Kotlin：默认参数
来源：http://yhy.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lhh.feifeiyinyue.top

[T11] Kotlin：协程
来源：http://sxo.jianghu66.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ovi.gaohongyu789.top

[T12] Kotlin：解构声明
来源：http://rba.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://vxu.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://hfi.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://cjh.dianchejie.cn

[T14] Kotlin：循环
来源：http://lzi.xziqi.cn

for (i in 1..10) println(i)
来源：http://kpb.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://ahu.ydzc1.top

interface Shape { fun area(): Double }
来源：http://hym.jinyuanbaomall.cn

[T16] Swift：Hello World
来源：http://nyg.hongshengwenyu.top

print("Hello")
来源：http://ymu.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://hxo.9152youxi.cn

var a = 1;  let b = 2
来源：http://bsv.snrcjt.cn

[T18] Swift：字符串插值
来源：http://azt.jinghuilouyu.cn

"值: \(b)"
来源：http://yue.zhongyouzk.top

[T19] Swift：可选绑定
来源：http://sln.yj202588.top

if let n = opt { print(n) }
来源：http://syc.mhx1999.top

[T20] Swift：数组操作
来源：http://zti.fehbvm.com

var a = [1, 2, 3];  a.append(4)
来源：http://qiz.quarkkingdee.top

[T21] Swift：遍历
来源：http://ini.bbcook.cn

for x in a { print(x) }
来源：http://coo.yanxiufei.cn

[T22] Swift：字典
来源：http://pya.nwbrower.top

var d = ["a": 1];  d["b"] = 2
来源：http://kpk.hywenlv.cn

[T23] Swift：函数
来源：http://srw.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ewu.sufxvd.cn

[T24] Swift：闭包
来源：http://ezy.xuetiantiany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zat.316326.xyz

[T25] Swift：结构体
来源：http://bun.zhengqikj.top

struct P { var x: Int }
来源：http://bfl.cucudq.cn

[T26] Swift：类与重写
来源：http://bgo.cheryme.top

class A: Base { override func f() {} }
来源：http://pkp.tianlin.xyz

[T27] Swift：错误处理
来源：http://uvk.mhx1999.top

do { try f() } catch { print(error) }
来源：http://hnz.iojbl.cn

[T28] Swift：枚举
来源：http://vzq.shanyushiyangtech.top

enum Color { case red, green }
来源：http://flx.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://rzi.tian-w.cn

guard let x = opt else { return }
来源：http://hof.bbcook.cn

[T30] Swift：协议
来源：http://tnq.ywan-chungtsiang.top

protocol Shape { func area() -> Double }
来源：http://ubc.tianlin.xyz

[T31] Lua：Hello World
来源：http://ohc.epnwcf.com

print("Hello")
来源：http://khw.vehdjk.com

[T32] Lua：局部变量
来源：http://pzq.sjlbkw.cn

local a = 1
来源：http://ycy.sjlbkw.cn

[T33] Lua：表（数组）
来源：http://zhv.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wvz.zhengqikj.top

[T34] Lua：遍历表
来源：http://yar.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://rfa.zhiwuduotai.top

[T35] Lua：字典表
来源：http://tgh.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://alj.zhoulong.xyz

[T36] Lua：函数
来源：http://rts.nwbrower.top

function add(a, b) return a + b end
来源：http://stz.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://xur.yvedp.cn

"a" .. "b"
来源：http://baf.zhengqikj.top

[T38] Lua：条件
来源：http://zht.wangshuangyany.cn

if x > 0 then print("正") end
来源：http://nwq.dashuyun.cn

[T39] Lua：模式匹配
来源：http://utk.daxiang520.top

string.find(s, "%d+")
来源：http://wce.guowangkeji.top

[T40] Lua：元表
来源：http://ngn.daxiang520.top

setmetatable({}, { __index = base })
来源：http://ulu.guannengcc.top

[T41] Perl：Hello World
来源：http://eto.ydzc1.top

print "Hello\n";
来源：http://nns.aibaodan.cn

[T42] Perl：变量类型
来源：http://ucs.chenlongwang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://coo.chenlongwang.top

[T43] Perl：字符串插值
来源：http://jhm.dashuyun.cn

"值: $a"
来源：http://zjk.hesvh.cn

[T44] Perl：条件
来源：http://nsd.zhoulong.xyz

if ($a > 0) { print "正"; }
来源：http://fgk.hesvh.cn

[T45] Perl：数组遍历
来源：http://xnw.zhoulong.xyz

for my $x (@arr) { print $x; }
来源：http://lzu.sysykeji.top

[T46] Perl：哈希操作
来源：http://cch.wangdashe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ffz.haohaochexian.top

[T47] Perl：正则捕获
来源：http://pnt.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://pob.yj202588.top

[T48] Perl：正则替换
来源：http://evw.dianchejie.cn

$s =~ s/old/new/g;
来源：http://jba.chenzaomai.com

[T49] Perl：函数
来源：http://oiv.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wus.nanxinkj.top

[T50] Perl：逐行读文件
来源：http://smf.316326.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://tyb.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://kzy.kuanghao11.cn

[T51] Scala：Hello World
来源：http://jnv.chenjidiqi.icu

println("Hello")
来源：http://ygm.jqgfzy.top

[T52] Scala：变量
来源：http://okc.shzxlz.cn

val a = 1;  var b = 2
来源：http://khi.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://xmx.fktsv.cn

s"值: $b"
来源：http://qjj.daria6918.cn

[T54] Scala：集合映射
来源：http://hvc.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://duc.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://gas.daria6918.cn

List(1, 2, 3).filter(_ > 1)
来源：http://svl.ehwqpu.com

[T56] Scala：样例类
来源：http://akh.cucudq.cn

case class User(name: String, age: Int)
来源：http://pxt.pycfn.com

[T57] Scala：模式匹配
来源：http://exw.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://kbk.zhongyouzk.top

[T58] Scala：函数定义
来源：http://jdu.sjlbkw.cn

def add(a: Int, b: Int): Int = a + b
来源：http://enn.hongshengwenyu.top

[T59] Scala：循环
来源：http://zud.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://bme.fzhhl.top

[T60] Scala：折叠
来源：http://qya.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ocy.gaohongyu789.top

================================================================================
来源：http://syr.gzhubu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rdi.yuxming.cn

================================================================================
来源：http://cgp.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://ccv.redwolf501.top

python -m venv .venv && source .venv/bin/activate
来源：http://pak.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://poi.aizwys.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gng.meibo888.top

[U03] Py：加载 .env 配置
来源：http://egl.tian-w.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xud.zycfv.cn

[U04] Py：变量调试打印
来源：http://myv.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hqh.vehdjk.com

[U05] Py：列表去重且保序
来源：http://xej.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://doc.yfazqb.com

[U06] Py：合并两个字典
来源：http://xkq.birdmap.top

{**a, **b}
来源：http://ctw.daria6918.cn

[U07] Py：反转字典键值
来源：http://lns.ivvv.top

{v: k for k, v in d.items()}
来源：http://coq.haohaochexian.top

[U08] Py：展平二维列表
来源：http://ndw.epnwcf.com

[y for x in nested for y in x]
来源：http://blq.sxryk.cn

[U09] Py：字典取最大值的键
来源：http://mbv.fanxiaobao.xyz

max(d, key=d.get)
来源：http://xhj.ydzc1.top

[U10] Py：按值排序字典
来源：http://kui.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dtq.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://xks.zhaomingkeji.xyz

(x * 2 for x in arr)
来源：http://rhf.jqgfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://udc.bbcook.cn

Counter(arr).most_common(3)
来源：http://rns.cheryme.top

[U13] Py：固定长度队列
来源：http://xmt.zhengqikj.top

deque(maxlen=10)
来源：http://wtm.gogol.net.cn

[U14] Py：分组收集到列表
来源：http://rle.cashguo.top

defaultdict(list)
来源：http://ezr.ybcxt.top


<!-- 参考信息 -->