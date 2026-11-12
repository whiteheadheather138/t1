代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xqz.hysaishi.cn

[R80] 查看脚本执行耗时
来源：http://mgs.vqdsnc.cn

time ./run.sh
来源：http://shh.feifeiyinyue.top

================================================================================
来源：http://nux.shzxlz.cn

S. C / C++ 专题
来源：http://xvy.zhengqikj.top

================================================================================
来源：http://zgg.fengsongda.top

[S01] C：Hello World
来源：http://wru.yuxming.cn

#include <stdio.h>
来源：http://xmq.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://ydm.xuetiantiany.cn

[S02] C：变量与格式化输出
来源：http://rca.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://fbw.ydzc1.top

[S03] C：读入整数
来源：http://yig.xziqi.cn

int x; scanf("%d", &x);
来源：http://imi.sysykeji.top

[S04] C：字符串复制
来源：http://ona.wangdashe.top

char dst[32]; strcpy(dst, "hi");
来源：http://hid.cdnleiting.top

[S05] C：字符串长度
来源：http://hci.redwolf501.top

strlen(s)
来源：http://kaa.andypj.xyz

[S06] C：字符串比较
来源：http://ekd.daxiang520.top

strcmp(a, b) == 0
来源：http://rtw.cqqwz.cn

[S07] C：数组遍历求和
来源：http://qfz.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://azy.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://aiv.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://clh.zhengqikj.top

[S09] C：结构体定义与初始化
来源：http://pfn.hnqzz.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dzj.sysykeji.top

[S10] C：指针与解引用
来源：http://xgw.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://eac.birdmap.top

[S11] C：逐行读文件
来源：http://zxe.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://fmq.yongpay.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zem.zhijiandao.cn

fclose(f);
来源：http://lsm.wangshuangyany.cn

[S12] C：写文件
来源：http://hbu.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nhc.zycfv.cn

[S13] C：宏定义
来源：http://lwp.birdmap.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yqa.yfazqb.com

[S14] C：枚举
来源：http://ycc.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://ixb.cheryme.top

[S15] C：类型转换
来源：http://ubz.jinyuanbaomall.cn

(double) a / b
来源：http://eux.chenlongwang.top

[S16] C：位操作置位
来源：http://buf.jlsjyb.cn

x |= (1 << 3);
来源：http://ilv.andypj.xyz

[S17] C：安全拼接字符串
来源：http://vxm.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bum.sufxvd.cn

[S18] C：命令行参数
来源：http://pea.havefunace.top

int main(int argc, char **argv)
来源：http://qdu.jyoumei.cn

[S19] C：快速排序
来源：http://lnl.jianghu66.top

qsort(a, n, sizeof(int), cmp);
来源：http://hbc.uphjek.com

[S20] C：二分查找
来源：http://pop.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xmq.zhiwuduotai.top

[S21] C：字符类别判断
来源：http://znz.sweek.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bnd.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://zxq.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nsu.yfazqb.com

[S23] C：随机数
来源：http://lrw.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mhk.aizwys.cn

[S24] C：获取本地时间
来源：http://ynd.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ige.guowangkeji.top

[S25] C：内存拷贝
来源：http://pyf.yueranfly.top

memcpy(dst, src, n);
来源：http://tin.sufxvd.cn

[S26] C：内存清零
来源：http://cjq.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://rrw.hesvh.cn

[S27] C：定义常量
来源：http://mwk.sysykeji.top

const double PI = 3.14159;
来源：http://mdi.hcnkem.com

[S28] C：静态变量
来源：http://iww.nanxuanxn.top

static int counter = 0;
来源：http://idg.tian-w.cn

[S29] C：变参函数
来源：http://mjh.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ers.snrcjt.cn

[S30] C：头文件保护
来源：http://waa.ydzc1.top

#ifndef X_H
来源：http://cgm.xingfuxueyuan.xyz

#define X_H
来源：http://emq.zdqjudy.top

#endif
来源：http://dmd.sweek.top

[S31] C++：Hello World
来源：http://xbq.yj202588.top

#include <iostream>
来源：http://iyb.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://hck.snrcjt.cn

[S32] C++：字符串
来源：http://qhf.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://mth.yfazqb.com

[S33] C++：vector 增删
来源：http://eeo.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wfz.wangdashe.top

[S34] C++：遍历 vector
来源：http://epn.jyoumei.cn

for (auto &x : v) { std::cout << x; }
来源：http://wga.cucudq.cn

[S35] C++：map
来源：http://kci.cucudq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ylm.zhengqikj.top

[S36] C++：unordered_map
来源：http://tcg.svipenyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gkd.guannengcc.top

[S37] C++：set
来源：http://chv.jinqigfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dhd.jyoumei.cn

[S38] C++：排序
来源：http://mlf.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://hgr.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://ahf.hcnkem.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tuy.zhoulong.xyz

[S40] C++：查找元素
来源：http://vcl.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qfq.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://nvs.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sby.mhx1999.top

[S42] C++：继承与虚函数
来源：http://xpp.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://zyh.ybcxt.top

[S43] C++：智能指针
来源：http://upk.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://ukx.sweek.top

[S44] C++：引用传参
来源：http://vsj.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://hyv.52xcode.cn

[S45] C++：lambda
来源：http://bkz.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://rer.yuanzhike.top

[S46] C++：函数模板
来源：http://eof.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vxc.hnqzz.top

[S47] C++：结构化绑定遍历
来源：http://xrk.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gbf.daxiang520.top

[S48] C++：逐行读文件
来源：http://dlt.fehbvm.com

std::ifstream in("a.txt");  std::string line;
来源：http://zwg.hcnkem.com

while (std::getline(in, line)) { }
来源：http://bnz.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://rpc.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://saq.sjlbkw.cn

[S50] C++：格式化数字
来源：http://rdd.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tjo.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://qwb.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://meh.hammf.cn

[S52] C++：const 与 noexcept
来源：http://omj.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://hhx.yj20258888.top

[S53] C++：移动语义
来源：http://zng.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://bfe.hongshengwenyu.top

[S54] C++：异常处理
来源：http://akn.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lep.uphjek.com

[S55] C++：结构化绑定
来源：http://ofe.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uro.shuidangran.top

[S56] C++：optional
来源：http://nol.sweek.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vvw.yongpay.top

[S57] C++：编译期常量
来源：http://adq.yonumen.top

constexpr int N = 10;
来源：http://jzn.hesvh.cn

[S58] C++：命名空间
来源：http://jwn.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://pzy.zycfv.cn

[S59] C++：静态断言
来源：http://saj.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ydm.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://hjv.dashuyun.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pjt.smart0.xyz

================================================================================
来源：http://yqj.xingfuxueyuan.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rva.jinyuanbaomall.cn

================================================================================
来源：http://bqa.cheryme.top

[T01] Kotlin：Hello World
来源：http://jai.xuetiantiany.cn

println("Hello")
来源：http://ipc.ivvv.top

[T02] Kotlin：变量
来源：http://yiw.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xft.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://svr.fengsongda.top

"值: $b"
来源：http://mxw.yj20258888.top

[T04] Kotlin：空安全
来源：http://rgi.tanke756.top

val n: String? = null;  n?.length
来源：http://imp.birdmap.top

[T05] Kotlin：when 表达式
来源：http://lpu.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ijd.cdnleiting.top

[T06] Kotlin：集合映射
来源：http://lju.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://caa.yuxming.cn

[T07] Kotlin：集合过滤
来源：http://gem.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pln.sufxvd.cn

[T08] Kotlin：数据类
来源：http://saa.jinqigfzy.top

data class User(val name: String, val age: Int)
来源：http://rdl.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://lvq.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://gcg.havefunace.top

[T10] Kotlin：默认参数
来源：http://len.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sun.jqgfzy.top

[T11] Kotlin：协程
来源：http://xyu.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qtm.meibo888.top

[T12] Kotlin：解构声明
来源：http://vjs.zhongyouzk.top

val (a, b) = Pair(1, 2)
来源：http://cri.hysaishi.cn

[T13] Kotlin：只读 Map
来源：http://war.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://wfm.ydjk.org.cn

[T14] Kotlin：循环
来源：http://vol.gaohongyu789.top

for (i in 1..10) println(i)
来源：http://nid.c1oappe.top

[T15] Kotlin：接口
来源：http://tjn.tarul.cn

interface Shape { fun area(): Double }
来源：http://yrk.sxryk.cn

[T16] Swift：Hello World
来源：http://esg.kuanghao11.cn

print("Hello")
来源：http://sfw.yfazqb.com

[T17] Swift：变量与常量
来源：http://jit.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://bse.xingfuxueyuan.xyz

[T18] Swift：字符串插值
来源：http://nmq.ppjwa.cn

"值: \(b)"
来源：http://iyq.cdnleiting.top

[T19] Swift：可选绑定
来源：http://eqm.daxiang520.top

if let n = opt { print(n) }
来源：http://ooi.andypj.xyz

[T20] Swift：数组操作
来源：http://qwb.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tjz.ppjwa.cn

[T21] Swift：遍历
来源：http://obf.andypj.xyz

for x in a { print(x) }
来源：http://zdq.chenzaomai.com

[T22] Swift：字典
来源：http://xax.ivvv.top

var d = ["a": 1];  d["b"] = 2
来源：http://ivp.cucudq.cn

[T23] Swift：函数
来源：http://lqv.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tmj.chenlongwang.top

[T24] Swift：闭包
来源：http://npb.ctjpmb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://asz.yj20258.top

[T25] Swift：结构体
来源：http://gwf.svipenyu.cn

struct P { var x: Int }
来源：http://hwp.zhoulong.xyz

[T26] Swift：类与重写
来源：http://qkm.daria6918.cn

class A: Base { override func f() {} }
来源：http://igz.yuxming.cn

[T27] Swift：错误处理
来源：http://sro.cdnleiting.top

do { try f() } catch { print(error) }
来源：http://dzn.feifeiyinyue.top

[T28] Swift：枚举
来源：http://znm.shzxlz.cn

enum Color { case red, green }
来源：http://baw.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://uuu.chenzaomai.com

guard let x = opt else { return }
来源：http://jml.hywenlv.cn

[T30] Swift：协议
来源：http://ooi.yonumen.top

protocol Shape { func area() -> Double }
来源：http://bbt.hammf.cn

[T31] Lua：Hello World
来源：http://vio.uphjek.com

print("Hello")
来源：http://clr.fktsv.cn

[T32] Lua：局部变量
来源：http://wgh.daria6918.cn

local a = 1
来源：http://chq.tian-w.cn

[T33] Lua：表（数组）
来源：http://iyf.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ugy.vehdjk.com

[T34] Lua：遍历表
来源：http://kmh.xingfuxueyuan.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://zfi.bjfxy.top

[T35] Lua：字典表
来源：http://muz.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://qms.dashuyun.cn

[T36] Lua：函数
来源：http://rgk.tian-w.cn

function add(a, b) return a + b end
来源：http://cyu.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://svs.gzhubu.top

"a" .. "b"
来源：http://kuq.vqdsnc.cn

[T38] Lua：条件
来源：http://std.sjlbkw.cn

if x > 0 then print("正") end
来源：http://qkz.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://fhi.daria6918.cn

string.find(s, "%d+")
来源：http://mid.cheryme.top

[T40] Lua：元表
来源：http://mxr.svipenyu.cn

setmetatable({}, { __index = base })
来源：http://oll.zhengqikj.top

[T41] Perl：Hello World
来源：http://tpw.iojbl.cn

print "Hello\n";
来源：http://yrr.cashguo.top

[T42] Perl：变量类型
来源：http://pkb.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gci.andypj.xyz

[T43] Perl：字符串插值
来源：http://dog.sweek.top

"值: $a"
来源：http://gou.sxryk.cn

[T44] Perl：条件
来源：http://bxk.yangfankeji.com

if ($a > 0) { print "正"; }
来源：http://feh.xuanzx.com

[T45] Perl：数组遍历
来源：http://vnu.yfazqb.com

for my $x (@arr) { print $x; }
来源：http://axn.daria6918.cn

[T46] Perl：哈希操作
来源：http://agh.c1oappe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zhd.zycfv.cn

[T47] Perl：正则捕获
来源：http://pcr.epnwcf.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://mnm.chenzaomai.com

[T48] Perl：正则替换
来源：http://xvr.yueranfly.top

$s =~ s/old/new/g;
来源：http://drp.yangfankeji.com

[T49] Perl：函数
来源：http://epf.cucudq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://idb.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://qhu.zhiwuduotai.top

open my $fh, "<", "a.txt" or die $!;
来源：http://enl.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://tfa.bbcook.cn

[T51] Scala：Hello World
来源：http://ehn.yvedp.cn

println("Hello")
来源：http://irh.gogol.net.cn

[T52] Scala：变量
来源：http://iky.cdnleiting.top

val a = 1;  var b = 2
来源：http://sna.wangdashe.top

[T53] Scala：字符串插值
来源：http://vmr.jqgfzy.top

s"值: $b"
来源：http://mbi.zhoulong.xyz

[T54] Scala：集合映射
来源：http://axh.zhongyouzk.top

List(1, 2, 3).map(_ * 2)
来源：http://uvr.hongshengwenyu.top

[T55] Scala：集合过滤
来源：http://taa.chenzaomai.com

List(1, 2, 3).filter(_ > 1)
来源：http://obo.fanxiaobao.xyz

[T56] Scala：样例类
来源：http://ryb.vqdsnc.cn

case class User(name: String, age: Int)
来源：http://jqm.yj20258.top

[T57] Scala：模式匹配
来源：http://rqg.vehdjk.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://zfj.pengpengdd.cyou

[T58] Scala：函数定义
来源：http://xxg.yanxiufei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sno.dashuyun.cn

[T59] Scala：循环
来源：http://puk.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://dqi.jinghuilouyu.cn

[T60] Scala：折叠
来源：http://dhf.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nvm.gotoacloud.top

================================================================================
来源：http://map.cheryme.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jos.xinyue.icu

================================================================================
来源：http://vsb.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://oxa.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://vwf.daria6918.cn

[U02] Py：导出 / 安装依赖
来源：http://dus.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://evh.jiagoushi.top

[U03] Py：加载 .env 配置
来源：http://qpw.c1oappe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bff.chenlongwang.top

[U04] Py：变量调试打印
来源：http://xtl.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oju.yueranfly.top

[U05] Py：列表去重且保序
来源：http://pzd.quarkkingdee.top

list(dict.fromkeys(arr))
来源：http://kfo.yueranfly.top

[U06] Py：合并两个字典
来源：http://nev.zhoulong.xyz

{**a, **b}
来源：http://cfc.snrcjt.cn

[U07] Py：反转字典键值
来源：http://vus.daxiang520.top

{v: k for k, v in d.items()}
来源：http://par.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://rtu.shanyushiyangkeji.top

[y for x in nested for y in x]
来源：http://qhd.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://vtw.andypj.xyz

max(d, key=d.get)
来源：http://gyw.zhengqikj.top

[U10] Py：按值排序字典
来源：http://eat.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zzc.epnwcf.com

[U11] Py：生成器表达式
来源：http://vrw.jiagoushi.top

(x * 2 for x in arr)
来源：http://jjq.xingfuxueyuan.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://xnq.52xcode.cn

Counter(arr).most_common(3)
来源：http://fjk.yj202588.top

[U13] Py：固定长度队列
来源：http://nve.zycfv.cn

deque(maxlen=10)
来源：http://oxb.zhaomingkeji.xyz

[U14] Py：分组收集到列表
来源：http://jxb.cashguo.top

defaultdict(list)
来源：http://quw.daxiang520.top

[U15] Py：高精度计时
来源：http://ibd.yuxming.cn

t = time.perf_counter()
来源：http://nly.yvedp.cn

[U16] Py：命令行参数解析
来源：http://riy.tian-w.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vbl.chenzaomai.com

[U17] Py：初始化日志
来源：http://rwt.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://gaj.haohaochexian.top

[U18] Py：预编译正则
来源：http://rmj.yfazqb.com

pat = re.compile(r"\d+")
来源：http://xls.chenzaomai.com

[U19] Py：正则替换带回调
来源：http://egb.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://exf.bjfxy.top

[U20] Py：缓存函数结果
来源：http://wvx.yfazqb.com

@functools.lru_cache(maxsize=None)
来源：http://wfz.fanxiaobao.xyz


<!-- 参考信息 -->