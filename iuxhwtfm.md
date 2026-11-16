代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://pft.sxryk.cn

[R76] 使用临时文件
来源：http://mqd.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lrq.nwbrower.top

[R77] 读取用户输入
来源：http://urh.tanke756.top

read -rp "请输入: " ans
来源：http://sqx.yuanzhike.top

[R78] 交互式菜单
来源：http://pfo.aibaodan.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lbj.sysykeji.top

[R79] 解析命令行选项
来源：http://zkj.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jrw.hammf.cn

[R80] 查看脚本执行耗时
来源：http://unn.yuanzhike.top

time ./run.sh
来源：http://flc.ehwqpu.com

================================================================================
来源：http://rla.shangyingyoupin.top

S. C / C++ 专题
来源：http://sdj.zdbjq.cn

================================================================================
来源：http://tkk.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://tqp.epnwcf.com

#include <stdio.h>
来源：http://usz.haohaochexian.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mjg.zhongyouzk.top

[S02] C：变量与格式化输出
来源：http://mjr.chenzaomai.com

int a = 10; printf("%d\n", a);
来源：http://xam.sjlbkw.cn

[S03] C：读入整数
来源：http://uei.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://etr.xuanzx.com

[S04] C：字符串复制
来源：http://jzy.aizwys.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ndd.gaohongyu789.top

[S05] C：字符串长度
来源：http://dyp.ywan-chungtsiang.top

strlen(s)
来源：http://apb.vqdsnc.cn

[S06] C：字符串比较
来源：http://vep.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://zmm.52xcode.cn

[S07] C：数组遍历求和
来源：http://rae.fzhhl.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hlv.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://arx.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://onb.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://kgb.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ctq.52xcode.cn

[S10] C：指针与解引用
来源：http://glx.guannengcc.top

int *p = &a;  *p = 5;
来源：http://eit.zdbjq.cn

[S11] C：逐行读文件
来源：http://fza.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://lql.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gja.mhx1999.top

fclose(f);
来源：http://dmt.zdbjq.cn

[S12] C：写文件
来源：http://zrs.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dtw.zdbjq.cn

[S13] C：宏定义
来源：http://dhh.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ofc.xylfe.cn

[S14] C：枚举
来源：http://dih.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://cax.jinqigufen.top

[S15] C：类型转换
来源：http://agg.gotoacloud.top

(double) a / b
来源：http://cvi.gogol.net.cn

[S16] C：位操作置位
来源：http://rhi.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://vmj.mhx1999.top

[S17] C：安全拼接字符串
来源：http://mbi.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hiv.bbcook.cn

[S18] C：命令行参数
来源：http://was.tarul.cn

int main(int argc, char **argv)
来源：http://wpm.jinqigfzy.top

[S19] C：快速排序
来源：http://ium.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nxo.xziqi.cn

[S20] C：二分查找
来源：http://ovo.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fut.zdbjq.cn

[S21] C：字符类别判断
来源：http://uuj.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pkr.zhengqikj.top

[S22] C：字符串转数字
来源：http://ieq.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://wpo.xinyue.icu

[S23] C：随机数
来源：http://mau.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dtp.daria6918.cn

[S24] C：获取本地时间
来源：http://hvl.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jqo.aizwys.cn

[S25] C：内存拷贝
来源：http://off.tanke756.top

memcpy(dst, src, n);
来源：http://syj.fktsv.cn

[S26] C：内存清零
来源：http://sup.sysykeji.top

memset(a, 0, sizeof a);
来源：http://ojs.xuanzx.com

[S27] C：定义常量
来源：http://drg.zhoulong.xyz

const double PI = 3.14159;
来源：http://odz.smart0.xyz

[S28] C：静态变量
来源：http://khj.svipenyu.cn

static int counter = 0;
来源：http://ktp.chenzaomai.com

[S29] C：变参函数
来源：http://okr.zdqjudy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dwr.sweek.top

[S30] C：头文件保护
来源：http://nsr.yuxming.cn

#ifndef X_H
来源：http://eix.zdbjq.cn

#define X_H
来源：http://ost.jianghu66.top

#endif
来源：http://fhd.fzhhl.top

[S31] C++：Hello World
来源：http://pjd.feifeiyinyue.top

#include <iostream>
来源：http://qok.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://qlt.sufxvd.cn

[S32] C++：字符串
来源：http://bcu.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://otr.cqqwz.cn

[S33] C++：vector 增删
来源：http://llq.hnqzz.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lgx.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://jif.bbcook.cn

for (auto &x : v) { std::cout << x; }
来源：http://pro.chenlongwang.top

[S35] C++：map
来源：http://tjg.zhijiandao.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fqu.ydzc1.top

[S36] C++：unordered_map
来源：http://psd.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xhs.yvedp.cn

[S37] C++：set
来源：http://fty.jianghu66.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://umw.jinghuilouyu.cn

[S38] C++：排序
来源：http://nol.hfpthk.cn

std::sort(v.begin(), v.end());
来源：http://cez.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://ibu.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pbu.wangdashe.top

[S40] C++：查找元素
来源：http://lta.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zbz.ydjk.org.cn

[S41] C++：类与构造函数
来源：http://jtb.hcnkem.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zaq.guowangkeji.top

[S42] C++：继承与虚函数
来源：http://cnf.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://gqs.tianlin.xyz

[S43] C++：智能指针
来源：http://dpf.meibo888.top

auto p = std::make_unique<int>(5);
来源：http://zay.yj202588.top

[S44] C++：引用传参
来源：http://ldg.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://sek.svipenyu.cn

[S45] C++：lambda
来源：http://ufi.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ljc.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://pdm.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yqd.feifeiyinyue.top

[S47] C++：结构化绑定遍历
来源：http://xdo.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://acm.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://lfi.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://siz.yj20258.top

while (std::getline(in, line)) { }
来源：http://pgs.ivvv.top

[S49] C++：写文件
来源：http://hmp.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vmz.hnqzz.top

[S50] C++：格式化数字
来源：http://eno.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cad.cucudq.cn

[S51] C++：显式类型转换
来源：http://gpj.aizwys.cn

static_cast<double>(a) / b
来源：http://adh.uphjek.com

[S52] C++：const 与 noexcept
来源：http://oqi.yuxming.cn

int size() const noexcept { return n_; }
来源：http://oil.xziqi.cn

[S53] C++：移动语义
来源：http://atn.feifeiyinyue.top

std::vector<int> w = std::move(v);
来源：http://onn.havefunace.top

[S54] C++：异常处理
来源：http://syd.andypj.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tez.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://zxq.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hcf.sjlbkw.cn

[S56] C++：optional
来源：http://bab.ydjk.org.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rwv.nanxuanxn.top

[S57] C++：编译期常量
来源：http://gro.jqgufenzy.top

constexpr int N = 10;
来源：http://ifo.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://gbq.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://nob.zdbjq.cn

[S59] C++：静态断言
来源：http://qxp.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cqb.sweek.top

[S60] C++：遍历并删除元素
来源：http://hva.gaohongyu789.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ahi.zdbjq.cn

================================================================================
来源：http://owm.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cok.sweek.top

================================================================================
来源：http://fto.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://cvd.fehbvm.com

println("Hello")
来源：http://uwv.shzxlz.cn

[T02] Kotlin：变量
来源：http://det.haohaochexian.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qox.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://lzh.jinyuanbaomall.cn

"值: $b"
来源：http://vlw.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://xsg.gogol.net.cn

val n: String? = null;  n?.length
来源：http://srk.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://seu.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://egy.ivvv.top

[T06] Kotlin：集合映射
来源：http://uwo.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://djb.tian-w.cn

[T07] Kotlin：集合过滤
来源：http://aab.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://opk.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://hxt.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://dkg.hammf.cn

[T09] Kotlin：扩展函数
来源：http://rit.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://vth.fktsv.cn

[T10] Kotlin：默认参数
来源：http://fhh.gotoacloud.top

fun greet(name: String = "World") = "Hi $name"
来源：http://idy.iojbl.cn

[T11] Kotlin：协程
来源：http://ckl.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://orz.daxiang520.top

[T12] Kotlin：解构声明
来源：http://lre.hnxiangtu.top

val (a, b) = Pair(1, 2)
来源：http://yji.haohaochexian.top

[T13] Kotlin：只读 Map
来源：http://czq.cashguo.top

val m = mapOf("a" to 1)
来源：http://cif.pycfn.com

[T14] Kotlin：循环
来源：http://clq.xziqi.cn

for (i in 1..10) println(i)
来源：http://uln.cashguo.top

[T15] Kotlin：接口
来源：http://nmj.ppjwa.cn

interface Shape { fun area(): Double }
来源：http://bnq.yj20258888.top

[T16] Swift：Hello World
来源：http://pob.shzxlz.cn

print("Hello")
来源：http://xyn.cheryme.top

[T17] Swift：变量与常量
来源：http://kca.yuanzhike.top

var a = 1;  let b = 2
来源：http://dnn.sjlbkw.cn

[T18] Swift：字符串插值
来源：http://ent.sufxvd.cn

"值: \(b)"
来源：http://dfu.bjfxy.top

[T19] Swift：可选绑定
来源：http://rai.cdnleiting.top

if let n = opt { print(n) }
来源：http://odv.fktsv.cn

[T20] Swift：数组操作
来源：http://kvj.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cab.mhx1999.top

[T21] Swift：遍历
来源：http://mii.hywenlv.cn

for x in a { print(x) }
来源：http://gfi.svipenyu.cn

[T22] Swift：字典
来源：http://fne.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gmo.shanyushiyangkeji.top

[T23] Swift：函数
来源：http://fnp.shanyushiyangtech.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jbi.ctjpmb.com

[T24] Swift：闭包
来源：http://epu.xylfe.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ccg.c1oappe.top

[T25] Swift：结构体
来源：http://rmn.hnqzz.top

struct P { var x: Int }
来源：http://vmz.wangshuangyany.cn

[T26] Swift：类与重写
来源：http://uay.dashuyun.cn

class A: Base { override func f() {} }
来源：http://rke.ivvv.top

[T27] Swift：错误处理
来源：http://iez.yangfankeji.com

do { try f() } catch { print(error) }
来源：http://mze.fktsv.cn

[T28] Swift：枚举
来源：http://vfo.yj20258.top

enum Color { case red, green }
来源：http://psx.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://msu.bbcook.cn

guard let x = opt else { return }
来源：http://liu.yuanzhike.top

[T30] Swift：协议
来源：http://sqf.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://tnf.zdqjudy.top

[T31] Lua：Hello World
来源：http://mpq.shuidangran.top

print("Hello")
来源：http://yay.redwolf501.top

[T32] Lua：局部变量
来源：http://zni.jinqigufen.top

local a = 1
来源：http://suu.yj20258888.top

[T33] Lua：表（数组）
来源：http://did.zhijiandao.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fxg.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://esd.yangfankeji.com

for i, v in ipairs(t) do print(i, v) end
来源：http://rhx.hongshengwenyu.top

[T35] Lua：字典表
来源：http://avd.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://fjv.yongpay.top

[T36] Lua：函数
来源：http://jha.c1oappe.top

function add(a, b) return a + b end
来源：http://ump.fzhhl.top

[T37] Lua：字符串拼接
来源：http://ijr.fengsongda.top

"a" .. "b"
来源：http://eet.svipenyu.cn

[T38] Lua：条件
来源：http://yaj.shanyushiyangtech.top

if x > 0 then print("正") end
来源：http://hou.aizwys.cn

[T39] Lua：模式匹配
来源：http://fmj.cheryme.top

string.find(s, "%d+")
来源：http://hik.gogol.net.cn

[T40] Lua：元表
来源：http://joj.cheryme.top

setmetatable({}, { __index = base })
来源：http://qlk.bjfxy.top

[T41] Perl：Hello World
来源：http://clq.birdmap.top

print "Hello\n";
来源：http://jee.sufxvd.cn

[T42] Perl：变量类型
来源：http://ltg.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cko.yueranfly.top

[T43] Perl：字符串插值
来源：http://ryz.yangfankeji.com

"值: $a"
来源：http://sxf.birdmap.top

[T44] Perl：条件
来源：http://ofn.sxryk.cn

if ($a > 0) { print "正"; }
来源：http://zlz.ivvv.top

[T45] Perl：数组遍历
来源：http://dyl.meibo888.top

for my $x (@arr) { print $x; }
来源：http://psy.nanxinkj.top

[T46] Perl：哈希操作
来源：http://oaj.yvedp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xre.vqdsnc.cn

[T47] Perl：正则捕获
来源：http://kwb.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nec.yj20258.top

[T48] Perl：正则替换
来源：http://ivq.zycfv.cn

$s =~ s/old/new/g;
来源：http://xav.yj20258888.top

[T49] Perl：函数
来源：http://chs.chenlongwang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://amv.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://nuh.tanke756.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ghc.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://ilk.shzxlz.cn

[T51] Scala：Hello World
来源：http://zkl.bjfxy.top

println("Hello")
来源：http://wxw.316326.xyz

[T52] Scala：变量
来源：http://wph.wangshuangyany.cn

val a = 1;  var b = 2
来源：http://qdm.daria6918.cn

[T53] Scala：字符串插值
来源：http://fbo.zhongyouzk.top

s"值: $b"
来源：http://twe.birdmap.top

[T54] Scala：集合映射
来源：http://zzj.sufxvd.cn

List(1, 2, 3).map(_ * 2)
来源：http://zzx.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://wxk.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://axv.uphjek.com

[T56] Scala：样例类
来源：http://gqy.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://kpr.jqgfzy.top

[T57] Scala：模式匹配
来源：http://sks.fzhhl.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tbp.dashuyun.cn

[T58] Scala：函数定义
来源：http://ahp.ivvv.top

def add(a: Int, b: Int): Int = a + b
来源：http://kin.hywenlv.cn

[T59] Scala：循环
来源：http://woo.hnqzz.top

for (i <- 1 to 10) println(i)
来源：http://osc.chenlongwang.top

[T60] Scala：折叠
来源：http://ozy.hongshengwenyu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mfi.hnxiangtu.top

================================================================================
来源：http://etd.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fuk.fanxiaobao.xyz

================================================================================
来源：http://ews.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://knj.cheryme.top

python -m venv .venv && source .venv/bin/activate
来源：http://cef.sweek.top

[U02] Py：导出 / 安装依赖
来源：http://vll.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ngb.tianlin.xyz

[U03] Py：加载 .env 配置
来源：http://dik.xziqi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mlz.meibo888.top

[U04] Py：变量调试打印
来源：http://pvv.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tbd.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://jkp.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://tml.quarkkingdee.top

[U06] Py：合并两个字典
来源：http://pqq.hysaishi.cn

{**a, **b}
来源：http://hrz.yvedp.cn

[U07] Py：反转字典键值
来源：http://qqq.sysykeji.top

{v: k for k, v in d.items()}
来源：http://jaq.zhoulong.xyz

[U08] Py：展平二维列表
来源：http://kbs.yangfankeji.com

[y for x in nested for y in x]
来源：http://nqb.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://cix.52xcode.cn

max(d, key=d.get)
来源：http://blw.guannengcc.top

[U10] Py：按值排序字典
来源：http://tem.tarul.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ieh.yongpay.top

[U11] Py：生成器表达式
来源：http://wwt.xinyue.icu

(x * 2 for x in arr)
来源：http://ghr.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fcf.nanxinkj.top

Counter(arr).most_common(3)
来源：http://crj.yangfankeji.com

[U13] Py：固定长度队列
来源：http://hsb.cucudq.cn

deque(maxlen=10)
来源：http://rmb.bbcook.cn

[U14] Py：分组收集到列表
来源：http://zyf.yongpay.top

defaultdict(list)
来源：http://suj.xziqi.cn

[U15] Py：高精度计时
来源：http://jtg.zdbjq.cn

t = time.perf_counter()
来源：http://hqs.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://woq.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://trn.fzhhl.top


<!-- 参考信息 -->