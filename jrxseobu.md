代发 wailian999

split -l 1000 big.log part_
来源：http://mfu.yonumen.top

[R74] 批量重命名
来源：http://ndx.uphjek.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vmt.ybcxt.top

[R75] 导出环境变量
来源：http://wiz.cashguo.top

export PATH="$HOME/bin:$PATH"
来源：http://pmb.daria6918.cn

[R76] 使用临时文件
来源：http://xww.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hlm.jianghu66.top

[R77] 读取用户输入
来源：http://soj.yfazqb.com

read -rp "请输入: " ans
来源：http://kig.fzhhl.top

[R78] 交互式菜单
来源：http://rkx.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://awn.ybcxt.top

[R79] 解析命令行选项
来源：http://ldq.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vlg.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://xgs.hongshengwenyu.top

time ./run.sh
来源：http://jth.yonumen.top

================================================================================
来源：http://tno.pycfn.com

S. C / C++ 专题
来源：http://ahw.ywan-chungtsiang.top

================================================================================
来源：http://rex.zdbjq.cn

[S01] C：Hello World
来源：http://rnn.ywan-chungtsiang.top

#include <stdio.h>
来源：http://qfu.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nex.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://zbk.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://tek.fengsongda.top

[S03] C：读入整数
来源：http://fbc.pycfn.com

int x; scanf("%d", &x);
来源：http://dgi.sweek.top

[S04] C：字符串复制
来源：http://inu.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://bqh.meibo888.top

[S05] C：字符串长度
来源：http://fck.ctjpmb.com

strlen(s)
来源：http://psr.hongshengwenyu.top

[S06] C：字符串比较
来源：http://tab.sweek.top

strcmp(a, b) == 0
来源：http://gtb.shuidangran.top

[S07] C：数组遍历求和
来源：http://amt.chenjidiqi.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://opp.316326.xyz

[S08] C：动态内存分配与释放
来源：http://qkh.9152youxi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pgz.uphjek.com

[S09] C：结构体定义与初始化
来源：http://xzc.fengsongda.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ijs.hnqzz.top

[S10] C：指针与解引用
来源：http://eww.xinyue.icu

int *p = &a;  *p = 5;
来源：http://ndx.sxryk.cn

[S11] C：逐行读文件
来源：http://hsq.yj202588.top

FILE *f = fopen("a.txt", "r");
来源：http://ioy.hysaishi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xwc.yvedp.cn

fclose(f);
来源：http://vpf.chenjidiqi.icu

[S12] C：写文件
来源：http://nlq.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ido.tanke756.top

[S13] C：宏定义
来源：http://tty.nanxinkj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dqs.yueranfly.top

[S14] C：枚举
来源：http://tvb.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://lvs.jqgfzy.top

[S15] C：类型转换
来源：http://cxx.yueranfly.top

(double) a / b
来源：http://zrb.yj20258.top

[S16] C：位操作置位
来源：http://fol.52xcode.cn

x |= (1 << 3);
来源：http://koo.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://nis.ppjwa.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tqm.sufxvd.cn

[S18] C：命令行参数
来源：http://dmd.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://wsi.gaohongyu789.top

[S19] C：快速排序
来源：http://meh.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xcl.zycfv.cn

[S20] C：二分查找
来源：http://xqw.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ryi.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://mzg.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fpy.0kj1m.cn

[S22] C：字符串转数字
来源：http://hnh.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jdr.cdnleiting.top

[S23] C：随机数
来源：http://vfz.ppjwa.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uqo.svipenyu.cn

[S24] C：获取本地时间
来源：http://sah.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gfu.xingfuxueyuan.xyz

[S25] C：内存拷贝
来源：http://bsg.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://mqg.yvedp.cn

[S26] C：内存清零
来源：http://qcu.yonumen.top

memset(a, 0, sizeof a);
来源：http://awc.jinghuilouyu.cn

[S27] C：定义常量
来源：http://epe.jinqigufen.top

const double PI = 3.14159;
来源：http://esv.fengsongda.top

[S28] C：静态变量
来源：http://gvc.jyoumei.cn

static int counter = 0;
来源：http://zcy.xinyue.icu

[S29] C：变参函数
来源：http://vyj.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gkn.hesvh.cn

[S30] C：头文件保护
来源：http://uvg.sxryk.cn

#ifndef X_H
来源：http://nco.316326.xyz

#define X_H
来源：http://fmr.yj20258.top

#endif
来源：http://ltk.yfazqb.com

[S31] C++：Hello World
来源：http://wkr.vehdjk.com

#include <iostream>
来源：http://vuk.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://qug.sufxvd.cn

[S32] C++：字符串
来源：http://aza.zhongyouzk.top

std::string s = "hi";  s += "!";
来源：http://ydx.wangdashe.top

[S33] C++：vector 增删
来源：http://sej.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fpp.gzhubu.top

[S34] C++：遍历 vector
来源：http://sdz.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://rtk.shzxlz.cn

[S35] C++：map
来源：http://xrq.jiagoushi.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dsq.yanxiufei.cn

[S36] C++：unordered_map
来源：http://tgy.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jdg.kuanghao11.cn

[S37] C++：set
来源：http://bmk.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aum.hnxiangtu.top

[S38] C++：排序
来源：http://jxt.ivvv.top

std::sort(v.begin(), v.end());
来源：http://kok.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://nug.yanxiufei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hhd.wangshuangyany.cn

[S40] C++：查找元素
来源：http://zzi.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bxb.nwbrower.top

[S41] C++：类与构造函数
来源：http://gkj.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://slm.uphjek.com

[S42] C++：继承与虚函数
来源：http://nll.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://gzx.fzhhl.top

[S43] C++：智能指针
来源：http://xcq.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://mce.gaohongyu789.top

[S44] C++：引用传参
来源：http://yte.yonumen.top

void inc(int &x) { ++x; }
来源：http://itw.sweek.top

[S45] C++：lambda
来源：http://ley.yonumen.top

auto add = [](int a, int b) { return a + b; };
来源：http://lqg.zhoulong.xyz

[S46] C++：函数模板
来源：http://eln.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dns.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://eae.fktsv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xlb.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://ihf.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jjg.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://ppv.yuanzhike.top

[S49] C++：写文件
来源：http://jyr.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kno.feifeiyinyue.top

[S50] C++：格式化数字
来源：http://xpp.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hkn.tarul.cn

[S51] C++：显式类型转换
来源：http://rks.guowangkeji.top

static_cast<double>(a) / b
来源：http://qne.pycfn.com

[S52] C++：const 与 noexcept
来源：http://jeo.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://ain.pengpengdd.cyou

[S53] C++：移动语义
来源：http://lfi.yj202588.top

std::vector<int> w = std::move(v);
来源：http://ldc.cashguo.top

[S54] C++：异常处理
来源：http://wkv.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pgz.dashuyun.cn

[S55] C++：结构化绑定
来源：http://uqe.yuanzhike.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ptn.mhx1999.top

[S56] C++：optional
来源：http://arl.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vua.fehbvm.com

[S57] C++：编译期常量
来源：http://sdn.316326.xyz

constexpr int N = 10;
来源：http://edf.ydjk.org.cn

[S58] C++：命名空间
来源：http://szs.daria6918.cn

namespace ns { int f() { return 1; } }
来源：http://mzq.tianlin.xyz

[S59] C++：静态断言
来源：http://pyn.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://law.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://dtt.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://str.ppjwa.cn

================================================================================
来源：http://kpc.zycfv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bfz.xingfuxueyuan.xyz

================================================================================
来源：http://coj.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://sdz.daxiang520.top

println("Hello")
来源：http://qma.yj20258888.top

[T02] Kotlin：变量
来源：http://kai.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dqo.yj202588.top

[T03] Kotlin：字符串模板
来源：http://vpi.sxryk.cn

"值: $b"
来源：http://uwl.9152youxi.cn

[T04] Kotlin：空安全
来源：http://qse.wangdashe.top

val n: String? = null;  n?.length
来源：http://nsa.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://meq.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cbe.c1oappe.top

[T06] Kotlin：集合映射
来源：http://dll.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eoa.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://gnm.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fkl.shuidangran.top

[T08] Kotlin：数据类
来源：http://vye.zhixingplan.top

data class User(val name: String, val age: Int)
来源：http://zqo.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://vcm.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://rov.fengsongda.top

[T10] Kotlin：默认参数
来源：http://xgo.gotoacloud.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jwc.jiagoushi.top

[T11] Kotlin：协程
来源：http://fii.hnqzz.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://uwc.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://las.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://ubb.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://wzi.jinghuilouyu.cn

val m = mapOf("a" to 1)
来源：http://cda.yonumen.top

[T14] Kotlin：循环
来源：http://eeu.smart0.xyz

for (i in 1..10) println(i)
来源：http://dsj.jiagoushi.top

[T15] Kotlin：接口
来源：http://cti.havefunace.top

interface Shape { fun area(): Double }
来源：http://qxl.jinqigufen.top

[T16] Swift：Hello World
来源：http://niq.zhoulong.xyz

print("Hello")
来源：http://udb.yj20258888.top

[T17] Swift：变量与常量
来源：http://pij.9152youxi.cn

var a = 1;  let b = 2
来源：http://tyu.c1oappe.top

[T18] Swift：字符串插值
来源：http://lbe.jlsjyb.cn

"值: \(b)"
来源：http://whr.ybcxt.top

[T19] Swift：可选绑定
来源：http://dnr.tarul.cn

if let n = opt { print(n) }
来源：http://kiq.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://nyf.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://frs.xylfe.cn

[T21] Swift：遍历
来源：http://lbr.mhx1999.top

for x in a { print(x) }
来源：http://xhd.birdmap.top

[T22] Swift：字典
来源：http://kol.zhixingplan.top

var d = ["a": 1];  d["b"] = 2
来源：http://imu.fanxiaobao.xyz

[T23] Swift：函数
来源：http://deg.shanyushiyangtech.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kbb.gaohongyu789.top

[T24] Swift：闭包
来源：http://zzw.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://nvc.hesvh.cn

[T25] Swift：结构体
来源：http://bme.vehdjk.com

struct P { var x: Int }
来源：http://pel.cucudq.cn

[T26] Swift：类与重写
来源：http://vbd.zycfv.cn

class A: Base { override func f() {} }
来源：http://lxu.hfpthk.cn

[T27] Swift：错误处理
来源：http://kwu.hcnkem.com

do { try f() } catch { print(error) }
来源：http://uwg.hysaishi.cn

[T28] Swift：枚举
来源：http://jal.gaohongyu789.top

enum Color { case red, green }
来源：http://rnz.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://xdr.feifeiyinyue.top

guard let x = opt else { return }
来源：http://amk.jinqigufen.top

[T30] Swift：协议
来源：http://oid.zhijiandao.cn

protocol Shape { func area() -> Double }
来源：http://oat.ehwqpu.com

[T31] Lua：Hello World
来源：http://oim.xuetiantiany.cn

print("Hello")
来源：http://bxe.zycfv.cn

[T32] Lua：局部变量
来源：http://rms.cqqwz.cn

local a = 1
来源：http://jhr.nanxuanxn.top

[T33] Lua：表（数组）
来源：http://jcs.cashguo.top

local t = {1, 2, 3};  t[4] = 4
来源：http://orc.yvedp.cn

[T34] Lua：遍历表
来源：http://zmc.birdmap.top

for i, v in ipairs(t) do print(i, v) end
来源：http://uog.yuanzhike.top

[T35] Lua：字典表
来源：http://nax.aibaodan.cn

local d = { a = 1 };  d.b = 2
来源：http://dcb.bbcook.cn

[T36] Lua：函数
来源：http://nqu.sxryk.cn

function add(a, b) return a + b end
来源：http://dlc.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://juf.xingfuxueyuan.xyz

"a" .. "b"
来源：http://mlo.fzhhl.top

[T38] Lua：条件
来源：http://lzs.andypj.xyz

if x > 0 then print("正") end
来源：http://iwg.cucudq.cn

[T39] Lua：模式匹配
来源：http://vzk.dianchejie.cn

string.find(s, "%d+")
来源：http://iwz.xuanzx.com

[T40] Lua：元表
来源：http://khr.bjfxy.top

setmetatable({}, { __index = base })
来源：http://lok.meibo888.top

[T41] Perl：Hello World
来源：http://kqv.chenzaomai.com

print "Hello\n";
来源：http://aao.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://jlr.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gnf.shanyushiyangtech.top

[T43] Perl：字符串插值
来源：http://iit.kuanghao11.cn

"值: $a"
来源：http://uji.xziqi.cn

[T44] Perl：条件
来源：http://oxr.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://fkz.zycfv.cn

[T45] Perl：数组遍历
来源：http://jxx.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://hfo.ivvv.top

[T46] Perl：哈希操作
来源：http://yjc.shuidangran.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://neo.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://pds.ybcxt.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ouo.sweek.top

[T48] Perl：正则替换
来源：http://zwe.cucudq.cn

$s =~ s/old/new/g;
来源：http://xms.yuxming.cn

[T49] Perl：函数
来源：http://wsl.tanke756.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qhm.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://czt.yfazqb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://isi.wangshuangyany.cn

while (my $line = <$fh>) { print $line; }
来源：http://fbe.gogol.net.cn

[T51] Scala：Hello World
来源：http://wai.wangshuangyany.cn

println("Hello")
来源：http://kkz.dianchejie.cn

[T52] Scala：变量
来源：http://vbr.zhoulong.xyz

val a = 1;  var b = 2
来源：http://qem.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://uil.vehdjk.com

s"值: $b"
来源：http://qwq.smart0.xyz

[T54] Scala：集合映射
来源：http://iiz.yueranfly.top

List(1, 2, 3).map(_ * 2)
来源：http://ihf.vehdjk.com

[T55] Scala：集合过滤
来源：http://evi.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://cjx.yvedp.cn

[T56] Scala：样例类
来源：http://muy.xingfuxueyuan.xyz

case class User(name: String, age: Int)
来源：http://mil.hywenlv.cn

[T57] Scala：模式匹配
来源：http://ivr.jinyuanbaomall.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://usc.yuanzhike.top

[T58] Scala：函数定义
来源：http://icu.hysaishi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mjb.hammf.cn

[T59] Scala：循环
来源：http://ssf.meibo888.top

for (i <- 1 to 10) println(i)
来源：http://xya.zhijiandao.cn

[T60] Scala：折叠
来源：http://kjm.kuanghao11.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wmx.hammf.cn

================================================================================
来源：http://wcf.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eoh.hfpthk.cn

================================================================================
来源：http://yby.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://wqc.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://gws.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://cyo.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rli.fanxiaobao.xyz

[U03] Py：加载 .env 配置
来源：http://qgs.sxryk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mga.tian-w.cn

[U04] Py：变量调试打印
来源：http://qqm.fktsv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://elu.zhengqikj.top

[U05] Py：列表去重且保序
来源：http://lpj.vehdjk.com

list(dict.fromkeys(arr))
来源：http://htn.yuanzhike.top

[U06] Py：合并两个字典
来源：http://pfg.fehbvm.com

{**a, **b}
来源：http://zej.zdqjudy.top

[U07] Py：反转字典键值
来源：http://ffv.birdmap.top

{v: k for k, v in d.items()}
来源：http://drd.jiagoushi.top

[U08] Py：展平二维列表
来源：http://yek.316326.xyz

[y for x in nested for y in x]
来源：http://wms.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://ydb.yuanzhike.top

max(d, key=d.get)
来源：http://qoc.xuetiantiany.cn

[U10] Py：按值排序字典
来源：http://gvy.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uwo.sxryk.cn

[U11] Py：生成器表达式
来源：http://dre.52xcode.cn

(x * 2 for x in arr)
来源：http://hzb.vehdjk.com

[U12] Py：取出现最多的 3 个元素
来源：http://qwq.yuxming.cn

Counter(arr).most_common(3)
来源：http://oho.mhx1999.top

[U13] Py：固定长度队列
来源：http://lwz.ydjk.org.cn

deque(maxlen=10)
来源：http://iuv.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://xcj.xylfe.cn

defaultdict(list)
来源：http://wdb.yonumen.top


<!-- 参考信息 -->