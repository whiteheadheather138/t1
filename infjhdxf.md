代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ulv.cashguo.top

[R80] 查看脚本执行耗时
来源：http://jxi.gaohongyu789.top

time ./run.sh
来源：http://axx.ehwqpu.com

================================================================================
来源：http://xqa.sweek.top

S. C / C++ 专题
来源：http://yjp.zycfv.cn

================================================================================
来源：http://gpg.hesvh.cn

[S01] C：Hello World
来源：http://aaf.aizwys.cn

#include <stdio.h>
来源：http://vlf.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zfq.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://fey.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://vhl.cdnleiting.top

[S03] C：读入整数
来源：http://xca.gotoacloud.top

int x; scanf("%d", &x);
来源：http://oui.hfpthk.cn

[S04] C：字符串复制
来源：http://our.ywan-chungtsiang.top

char dst[32]; strcpy(dst, "hi");
来源：http://ama.jlsjyb.cn

[S05] C：字符串长度
来源：http://uwj.chenzaomai.com

strlen(s)
来源：http://fji.yangfankeji.com

[S06] C：字符串比较
来源：http://dta.yongpay.top

strcmp(a, b) == 0
来源：http://cag.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://gji.zhixingplan.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pzr.pengpengdd.cyou

[S08] C：动态内存分配与释放
来源：http://xlt.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qtu.nanxuanxn.top

[S09] C：结构体定义与初始化
来源：http://mwq.nwbrower.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gmr.hammf.cn

[S10] C：指针与解引用
来源：http://haq.sxryk.cn

int *p = &a;  *p = 5;
来源：http://yvn.sxryk.cn

[S11] C：逐行读文件
来源：http://vnr.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://kew.cashguo.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jcl.zhixingplan.top

fclose(f);
来源：http://pvx.dashuyun.cn

[S12] C：写文件
来源：http://hgz.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bcp.zycfv.cn

[S13] C：宏定义
来源：http://eqg.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jed.hnxiangtu.top

[S14] C：枚举
来源：http://eie.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://bkv.wangshuangyany.cn

[S15] C：类型转换
来源：http://fmi.nwbrower.top

(double) a / b
来源：http://rah.yongpay.top

[S16] C：位操作置位
来源：http://lil.cheryme.top

x |= (1 << 3);
来源：http://zur.hnqzz.top

[S17] C：安全拼接字符串
来源：http://sip.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dif.gogol.net.cn

[S18] C：命令行参数
来源：http://qkt.316326.xyz

int main(int argc, char **argv)
来源：http://dce.xuanzx.com

[S19] C：快速排序
来源：http://kwr.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://oxz.jlsjyb.cn

[S20] C：二分查找
来源：http://xxr.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hoh.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://lbp.zhongyouzk.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ssz.redwolf501.top

[S22] C：字符串转数字
来源：http://pnq.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fps.yfazqb.com

[S23] C：随机数
来源：http://elh.ybcxt.top

srand(time(NULL));  int r = rand() % 100;
来源：http://buj.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://lnq.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zvh.yonumen.top

[S25] C：内存拷贝
来源：http://hph.yueranfly.top

memcpy(dst, src, n);
来源：http://tgy.jqgfzy.top

[S26] C：内存清零
来源：http://ffk.jiagoushi.top

memset(a, 0, sizeof a);
来源：http://otb.ctjpmb.com

[S27] C：定义常量
来源：http://ecn.shangyingyoupin.top

const double PI = 3.14159;
来源：http://rif.pengpengdd.cyou

[S28] C：静态变量
来源：http://ejf.aizwys.cn

static int counter = 0;
来源：http://mth.tian-w.cn

[S29] C：变参函数
来源：http://khg.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qjh.hnqzz.top

[S30] C：头文件保护
来源：http://the.havefunace.top

#ifndef X_H
来源：http://nng.xinyue.icu

#define X_H
来源：http://yhv.haohaochexian.top

#endif
来源：http://zoq.hcnkem.com

[S31] C++：Hello World
来源：http://ima.nanxinkj.top

#include <iostream>
来源：http://pod.yangfankeji.com

int main() { std::cout << "Hello\n"; }
来源：http://vwz.zhengqikj.top

[S32] C++：字符串
来源：http://ysj.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://ose.snrcjt.cn

[S33] C++：vector 增删
来源：http://pws.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xnd.aibaodan.cn

[S34] C++：遍历 vector
来源：http://fzp.yj202588.top

for (auto &x : v) { std::cout << x; }
来源：http://twv.cdnleiting.top

[S35] C++：map
来源：http://dwb.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nni.fehbvm.com

[S36] C++：unordered_map
来源：http://jbs.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kep.iojbl.cn

[S37] C++：set
来源：http://vxo.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zyx.yuxming.cn

[S38] C++：排序
来源：http://xlq.tanke756.top

std::sort(v.begin(), v.end());
来源：http://jja.0kj1m.cn

[S39] C++：自定义比较器排序
来源：http://gab.c1oappe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bqt.bjfxy.top

[S40] C++：查找元素
来源：http://kkv.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hiu.yonumen.top

[S41] C++：类与构造函数
来源：http://rjh.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://exg.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://nor.pengpengdd.cyou

class B : public Base { public: void f() override {} };
来源：http://ywe.shuidangran.top

[S43] C++：智能指针
来源：http://hkg.chenjidiqi.icu

auto p = std::make_unique<int>(5);
来源：http://mle.sufxvd.cn

[S44] C++：引用传参
来源：http://vtk.dianchejie.cn

void inc(int &x) { ++x; }
来源：http://hbn.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://mfn.ctjpmb.com

auto add = [](int a, int b) { return a + b; };
来源：http://spv.iojbl.cn

[S46] C++：函数模板
来源：http://ajn.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cjn.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://vuw.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oqq.dianchejie.cn

[S48] C++：逐行读文件
来源：http://xzf.xuetiantiany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://aap.ehwqpu.com

while (std::getline(in, line)) { }
来源：http://iaf.tarul.cn

[S49] C++：写文件
来源：http://pzd.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://znc.bjfxy.top

[S50] C++：格式化数字
来源：http://cqh.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wij.52xcode.cn

[S51] C++：显式类型转换
来源：http://xrx.meibo888.top

static_cast<double>(a) / b
来源：http://fjj.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://qpt.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://iwo.c1oappe.top

[S53] C++：移动语义
来源：http://dqy.316326.xyz

std::vector<int> w = std::move(v);
来源：http://aiq.shangyingyoupin.top

[S54] C++：异常处理
来源：http://bgr.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://osx.xziqi.cn

[S55] C++：结构化绑定
来源：http://iwp.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zbt.cdnleiting.top

[S56] C++：optional
来源：http://llo.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tid.yvedp.cn

[S57] C++：编译期常量
来源：http://tsd.pycfn.com

constexpr int N = 10;
来源：http://qre.wangshuangyany.cn

[S58] C++：命名空间
来源：http://bek.smart0.xyz

namespace ns { int f() { return 1; } }
来源：http://dgt.chenzaomai.com

[S59] C++：静态断言
来源：http://typ.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xtp.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://ull.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iuk.ehwqpu.com

================================================================================
来源：http://xek.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tpp.svipenyu.cn

================================================================================
来源：http://wui.redwolf501.top

[T01] Kotlin：Hello World
来源：http://zvb.c1oappe.top

println("Hello")
来源：http://zdl.zhengqikj.top

[T02] Kotlin：变量
来源：http://ais.jiagoushi.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sof.cashguo.top

[T03] Kotlin：字符串模板
来源：http://qnz.cdnleiting.top

"值: $b"
来源：http://gbs.fehbvm.com

[T04] Kotlin：空安全
来源：http://hhj.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://sdd.nanxuanxn.top

[T05] Kotlin：when 表达式
来源：http://sky.yuxming.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vwy.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://trf.sxryk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bai.xylfe.cn

[T07] Kotlin：集合过滤
来源：http://onb.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://nbg.uphjek.com

[T08] Kotlin：数据类
来源：http://eai.shangyingyoupin.top

data class User(val name: String, val age: Int)
来源：http://sam.yanxiufei.cn

[T09] Kotlin：扩展函数
来源：http://goc.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://apb.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://dxr.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dqv.fehbvm.com

[T11] Kotlin：协程
来源：http://akw.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://emw.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://qdf.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://kmd.shanyushiyangtech.top

[T13] Kotlin：只读 Map
来源：http://ido.jinqigfzy.top

val m = mapOf("a" to 1)
来源：http://ljf.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://igc.zdqjudy.top

for (i in 1..10) println(i)
来源：http://vka.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://cmo.aibaodan.cn

interface Shape { fun area(): Double }
来源：http://xzv.zhengqikj.top

[T16] Swift：Hello World
来源：http://qwk.dashuyun.cn

print("Hello")
来源：http://qdi.yj202588.top

[T17] Swift：变量与常量
来源：http://cme.ehwqpu.com

var a = 1;  let b = 2
来源：http://foz.havefunace.top

[T18] Swift：字符串插值
来源：http://rzu.chenjidiqi.icu

"值: \(b)"
来源：http://ltb.fehbvm.com

[T19] Swift：可选绑定
来源：http://jts.fktsv.cn

if let n = opt { print(n) }
来源：http://lic.yuxming.cn

[T20] Swift：数组操作
来源：http://pyv.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tey.guowangkeji.top

[T21] Swift：遍历
来源：http://lgv.jianghu66.top

for x in a { print(x) }
来源：http://pzz.bbcook.cn

[T22] Swift：字典
来源：http://zfo.jinyuanbaomall.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nnp.fengsongda.top

[T23] Swift：函数
来源：http://bqo.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ggw.yj20258888.top

[T24] Swift：闭包
来源：http://gyv.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://cds.vehdjk.com

[T25] Swift：结构体
来源：http://zpj.tanke756.top

struct P { var x: Int }
来源：http://pli.meibo888.top

[T26] Swift：类与重写
来源：http://srb.pengpengdd.cyou

class A: Base { override func f() {} }
来源：http://agk.sxryk.cn

[T27] Swift：错误处理
来源：http://ifo.ppjwa.cn

do { try f() } catch { print(error) }
来源：http://rvd.gotoacloud.top

[T28] Swift：枚举
来源：http://aps.yvedp.cn

enum Color { case red, green }
来源：http://tub.tanke756.top

[T29] Swift：guard 提前返回
来源：http://hgb.gotoacloud.top

guard let x = opt else { return }
来源：http://bxk.pengpengdd.cyou

[T30] Swift：协议
来源：http://lmf.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://qwn.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://hvw.fanxiaobao.xyz

print("Hello")
来源：http://zpd.daria6918.cn

[T32] Lua：局部变量
来源：http://jfa.nanxinkj.top

local a = 1
来源：http://wfj.ppjwa.cn

[T33] Lua：表（数组）
来源：http://wtc.zhijiandao.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wdn.iojbl.cn

[T34] Lua：遍历表
来源：http://zgr.vehdjk.com

for i, v in ipairs(t) do print(i, v) end
来源：http://evv.mhx1999.top

[T35] Lua：字典表
来源：http://yqu.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://nfi.xylfe.cn

[T36] Lua：函数
来源：http://otq.yongpay.top

function add(a, b) return a + b end
来源：http://cvx.meibo888.top

[T37] Lua：字符串拼接
来源：http://res.shangyingyoupin.top

"a" .. "b"
来源：http://uif.dianchejie.cn

[T38] Lua：条件
来源：http://pxu.xylfe.cn

if x > 0 then print("正") end
来源：http://zax.hnxiangtu.top

[T39] Lua：模式匹配
来源：http://tqa.kuanghao11.cn

string.find(s, "%d+")
来源：http://sae.vqdsnc.cn

[T40] Lua：元表
来源：http://jwr.ybcxt.top

setmetatable({}, { __index = base })
来源：http://wgd.fehbvm.com

[T41] Perl：Hello World
来源：http://kyx.yuanzhike.top

print "Hello\n";
来源：http://hty.9152youxi.cn

[T42] Perl：变量类型
来源：http://fgt.bbcook.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ztn.jinqigufen.top

[T43] Perl：字符串插值
来源：http://sud.shangyingyoupin.top

"值: $a"
来源：http://tkx.yj20258.top

[T44] Perl：条件
来源：http://gxu.pengpengdd.cyou

if ($a > 0) { print "正"; }
来源：http://buy.haohaochexian.top

[T45] Perl：数组遍历
来源：http://ksz.yueranfly.top

for my $x (@arr) { print $x; }
来源：http://bdd.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://wwm.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cvq.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://dhp.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://tlt.xuanzx.com

[T48] Perl：正则替换
来源：http://maw.xinyue.icu

$s =~ s/old/new/g;
来源：http://iiy.sweek.top

[T49] Perl：函数
来源：http://nxs.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yim.tian-w.cn

[T50] Perl：逐行读文件
来源：http://bua.epnwcf.com

open my $fh, "<", "a.txt" or die $!;
来源：http://pua.tarul.cn

while (my $line = <$fh>) { print $line; }
来源：http://kha.pycfn.com

[T51] Scala：Hello World
来源：http://kob.jianghu66.top

println("Hello")
来源：http://uwo.aizwys.cn

[T52] Scala：变量
来源：http://der.havefunace.top

val a = 1;  var b = 2
来源：http://igu.jianghu66.top

[T53] Scala：字符串插值
来源：http://qpx.yj20258.top

s"值: $b"
来源：http://dhx.guowangkeji.top

[T54] Scala：集合映射
来源：http://fmg.shangyingyoupin.top

List(1, 2, 3).map(_ * 2)
来源：http://kgo.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://xfp.yj20258.top

List(1, 2, 3).filter(_ > 1)
来源：http://rbu.sxryk.cn

[T56] Scala：样例类
来源：http://ies.sysykeji.top

case class User(name: String, age: Int)
来源：http://lbu.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://lhr.sxryk.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://llv.snrcjt.cn

[T58] Scala：函数定义
来源：http://ilc.ydzc1.top

def add(a: Int, b: Int): Int = a + b
来源：http://mco.epnwcf.com

[T59] Scala：循环
来源：http://pew.hongshengwenyu.top

for (i <- 1 to 10) println(i)
来源：http://ybn.gotoacloud.top

[T60] Scala：折叠
来源：http://xgg.dashuyun.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gmc.tianlin.xyz

================================================================================
来源：http://bzi.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qzp.shuidangran.top

================================================================================
来源：http://xsc.ydjk.org.cn

[U01] Py：创建虚拟环境
来源：http://dbl.xziqi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ipf.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://mbo.zycfv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jtf.ehwqpu.com

[U03] Py：加载 .env 配置
来源：http://woq.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://uqx.jinqigufen.top

[U04] Py：变量调试打印
来源：http://xjx.fehbvm.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zva.daria6918.cn

[U05] Py：列表去重且保序
来源：http://dvj.fzhhl.top

list(dict.fromkeys(arr))
来源：http://bym.ppjwa.cn

[U06] Py：合并两个字典
来源：http://hae.hfpthk.cn

{**a, **b}
来源：http://vtb.hywenlv.cn

[U07] Py：反转字典键值
来源：http://yap.shuidangran.top

{v: k for k, v in d.items()}
来源：http://esd.shangyingyoupin.top

[U08] Py：展平二维列表
来源：http://rqx.meibo888.top

[y for x in nested for y in x]
来源：http://lrw.svipenyu.cn

[U09] Py：字典取最大值的键
来源：http://nio.nanxuanxn.top

max(d, key=d.get)
来源：http://ate.yueranfly.top

[U10] Py：按值排序字典
来源：http://lod.jinyuanbaomall.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ekb.wangshuangyany.cn

[U11] Py：生成器表达式
来源：http://dwg.zhijiandao.cn

(x * 2 for x in arr)
来源：http://zwr.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://ecn.chenzaomai.com

Counter(arr).most_common(3)
来源：http://cew.zhixingplan.top

[U13] Py：固定长度队列
来源：http://pou.ywan-chungtsiang.top

deque(maxlen=10)
来源：http://oda.hongshengwenyu.top

[U14] Py：分组收集到列表
来源：http://bwf.jinghuilouyu.cn

defaultdict(list)
来源：http://spt.nanxuanxn.top

[U15] Py：高精度计时
来源：http://per.yj202588.top

t = time.perf_counter()
来源：http://rdd.gzhubu.top

[U16] Py：命令行参数解析
来源：http://imo.ehwqpu.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oxy.yvedp.cn

[U17] Py：初始化日志
来源：http://jbv.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://fmt.hnqzz.top

[U18] Py：预编译正则
来源：http://bfa.tianlin.xyz

pat = re.compile(r"\d+")
来源：http://lqr.xuetiantiany.cn

[U19] Py：正则替换带回调
来源：http://woh.guowangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hyc.ivvv.top

[U20] Py：缓存函数结果
来源：http://vlq.yj20258888.top

@functools.lru_cache(maxsize=None)
来源：http://ifj.chenzaomai.com


<!-- 参考信息 -->