代发 wailian999

read -rp "请输入: " ans
来源：http://xvn.jyoumei.cn

[R78] 交互式菜单
来源：http://zel.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://odk.yonumen.top

[R79] 解析命令行选项
来源：http://jid.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jpi.dashuyun.cn

[R80] 查看脚本执行耗时
来源：http://jxh.ehwqpu.com

time ./run.sh
来源：http://flf.9152youxi.cn

================================================================================
来源：http://eod.nanxinkj.top

S. C / C++ 专题
来源：http://ute.cucudq.cn

================================================================================
来源：http://sty.hysaishi.cn

[S01] C：Hello World
来源：http://sld.hysaishi.cn

#include <stdio.h>
来源：http://bxz.hcnkem.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://cei.hysaishi.cn

[S02] C：变量与格式化输出
来源：http://rqe.jianghu66.top

int a = 10; printf("%d\n", a);
来源：http://qld.shuidangran.top

[S03] C：读入整数
来源：http://woi.chenzaomai.com

int x; scanf("%d", &x);
来源：http://lla.zhoulong.xyz

[S04] C：字符串复制
来源：http://was.nanxinkj.top

char dst[32]; strcpy(dst, "hi");
来源：http://kyr.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://sne.meibo888.top

strlen(s)
来源：http://dbx.gogol.net.cn

[S06] C：字符串比较
来源：http://sgw.guannengcc.top

strcmp(a, b) == 0
来源：http://bbr.fehbvm.com

[S07] C：数组遍历求和
来源：http://fzf.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ktk.xziqi.cn

[S08] C：动态内存分配与释放
来源：http://jya.zhiwuduotai.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ccp.yj20258.top

[S09] C：结构体定义与初始化
来源：http://opc.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pjk.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://hyl.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://lyd.cucudq.cn

[S11] C：逐行读文件
来源：http://oen.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://ead.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://djr.bjfxy.top

fclose(f);
来源：http://kda.zhongyouzk.top

[S12] C：写文件
来源：http://fjl.cdnleiting.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://otu.ppjwa.cn

[S13] C：宏定义
来源：http://rog.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ucz.gotoacloud.top

[S14] C：枚举
来源：http://aan.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://okc.svipenyu.cn

[S15] C：类型转换
来源：http://czt.tanke756.top

(double) a / b
来源：http://wxs.fanxiaobao.xyz

[S16] C：位操作置位
来源：http://dla.nanxuanxn.top

x |= (1 << 3);
来源：http://uri.fzhhl.top

[S17] C：安全拼接字符串
来源：http://mqf.hysaishi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ixk.yangfankeji.com

[S18] C：命令行参数
来源：http://klz.sufxvd.cn

int main(int argc, char **argv)
来源：http://wbg.pycfn.com

[S19] C：快速排序
来源：http://jpj.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://cym.chenzaomai.com

[S20] C：二分查找
来源：http://tfn.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://btz.pycfn.com

[S21] C：字符类别判断
来源：http://zjj.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://flc.nwbrower.top

[S22] C：字符串转数字
来源：http://uqx.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cqr.cdnleiting.top

[S23] C：随机数
来源：http://uwq.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vlf.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://bdj.cucudq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xwv.gaohongyu789.top

[S25] C：内存拷贝
来源：http://kin.cdnleiting.top

memcpy(dst, src, n);
来源：http://zar.iojbl.cn

[S26] C：内存清零
来源：http://ccd.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://wgl.cqqwz.cn

[S27] C：定义常量
来源：http://vze.tianlin.xyz

const double PI = 3.14159;
来源：http://gjp.cqqwz.cn

[S28] C：静态变量
来源：http://vmd.hongshengwenyu.top

static int counter = 0;
来源：http://nwx.wangdashe.top

[S29] C：变参函数
来源：http://vte.zycfv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://liw.bbcook.cn

[S30] C：头文件保护
来源：http://lwq.52xcode.cn

#ifndef X_H
来源：http://kdy.snrcjt.cn

#define X_H
来源：http://hnv.cucudq.cn

#endif
来源：http://lrx.sufxvd.cn

[S31] C++：Hello World
来源：http://syb.shanyushiyangtech.top

#include <iostream>
来源：http://alw.yfazqb.com

int main() { std::cout << "Hello\n"; }
来源：http://ikw.fehbvm.com

[S32] C++：字符串
来源：http://kgx.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://kiq.yvedp.cn

[S33] C++：vector 增删
来源：http://fry.zhaomingkeji.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://afn.yfazqb.com

[S34] C++：遍历 vector
来源：http://bur.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://rvw.shzxlz.cn

[S35] C++：map
来源：http://jfp.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pbf.nwbrower.top

[S36] C++：unordered_map
来源：http://pop.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://byu.tanke756.top

[S37] C++：set
来源：http://hgc.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vgv.wangshuangyany.cn

[S38] C++：排序
来源：http://ujk.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://jgl.aizwys.cn

[S39] C++：自定义比较器排序
来源：http://nkg.fktsv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://haz.xuanzx.com

[S40] C++：查找元素
来源：http://mim.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wwv.gogol.net.cn

[S41] C++：类与构造函数
来源：http://bjh.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rml.fktsv.cn

[S42] C++：继承与虚函数
来源：http://cnu.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://bes.snrcjt.cn

[S43] C++：智能指针
来源：http://ztt.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://ygb.wangdashe.top

[S44] C++：引用传参
来源：http://xpy.316326.xyz

void inc(int &x) { ++x; }
来源：http://slr.nanxinkj.top

[S45] C++：lambda
来源：http://jwp.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://amz.jlsjyb.cn

[S46] C++：函数模板
来源：http://xda.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pic.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://tjg.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zxg.yvedp.cn

[S48] C++：逐行读文件
来源：http://tjb.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://dlj.zhongyouzk.top

while (std::getline(in, line)) { }
来源：http://lwh.meibo888.top

[S49] C++：写文件
来源：http://olo.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pgc.gzhubu.top

[S50] C++：格式化数字
来源：http://rrh.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dje.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://dxe.ywan-chungtsiang.top

static_cast<double>(a) / b
来源：http://iks.xuanzx.com

[S52] C++：const 与 noexcept
来源：http://yla.wangshuangyany.cn

int size() const noexcept { return n_; }
来源：http://krn.316326.xyz

[S53] C++：移动语义
来源：http://zqy.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://ytm.tarul.cn

[S54] C++：异常处理
来源：http://swj.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zcz.bjfxy.top

[S55] C++：结构化绑定
来源：http://qsu.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fxe.yangfankeji.com

[S56] C++：optional
来源：http://xgp.chenjidiqi.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vwi.shzxlz.cn

[S57] C++：编译期常量
来源：http://rzm.yj20258888.top

constexpr int N = 10;
来源：http://rco.meibo888.top

[S58] C++：命名空间
来源：http://yyt.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://ryh.gogol.net.cn

[S59] C++：静态断言
来源：http://trh.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ope.chenzaomai.com

[S60] C++：遍历并删除元素
来源：http://qtz.xingfuxueyuan.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lnb.sxryk.cn

================================================================================
来源：http://yyu.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kpv.zhijiandao.cn

================================================================================
来源：http://qce.yueranfly.top

[T01] Kotlin：Hello World
来源：http://fzy.andypj.xyz

println("Hello")
来源：http://qxb.bbcook.cn

[T02] Kotlin：变量
来源：http://lgf.xingfuxueyuan.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vch.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://kbu.fengsongda.top

"值: $b"
来源：http://yza.yuanzhike.top

[T04] Kotlin：空安全
来源：http://qst.c1oappe.top

val n: String? = null;  n?.length
来源：http://zgo.yueranfly.top

[T05] Kotlin：when 表达式
来源：http://jqu.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iog.shuidangran.top

[T06] Kotlin：集合映射
来源：http://xiq.sjlbkw.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ocq.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://mhs.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://uwq.yj202588.top

[T08] Kotlin：数据类
来源：http://qsd.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://ioq.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://ais.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://bvx.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://xnj.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xhm.sweek.top

[T11] Kotlin：协程
来源：http://yxi.fehbvm.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://zbj.sysykeji.top

[T12] Kotlin：解构声明
来源：http://kqm.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://juh.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://thl.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://qod.gotoacloud.top

[T14] Kotlin：循环
来源：http://nyg.yonumen.top

for (i in 1..10) println(i)
来源：http://uru.xinyue.icu

[T15] Kotlin：接口
来源：http://jkf.redwolf501.top

interface Shape { fun area(): Double }
来源：http://axi.316326.xyz

[T16] Swift：Hello World
来源：http://sfm.sysykeji.top

print("Hello")
来源：http://xqx.daria6918.cn

[T17] Swift：变量与常量
来源：http://ojw.redwolf501.top

var a = 1;  let b = 2
来源：http://jkt.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://eyv.meibo888.top

"值: \(b)"
来源：http://oic.chenzaomai.com

[T19] Swift：可选绑定
来源：http://vvo.xuanzx.com

if let n = opt { print(n) }
来源：http://otj.dianchejie.cn

[T20] Swift：数组操作
来源：http://psi.gotoacloud.top

var a = [1, 2, 3];  a.append(4)
来源：http://tkj.jqgfzy.top

[T21] Swift：遍历
来源：http://frb.epnwcf.com

for x in a { print(x) }
来源：http://vck.aibaodan.cn

[T22] Swift：字典
来源：http://lbf.uphjek.com

var d = ["a": 1];  d["b"] = 2
来源：http://rca.sysykeji.top

[T23] Swift：函数
来源：http://gwj.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jux.xuanzx.com

[T24] Swift：闭包
来源：http://suu.xylfe.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iey.yonumen.top

[T25] Swift：结构体
来源：http://ajm.svipenyu.cn

struct P { var x: Int }
来源：http://aly.9152youxi.cn

[T26] Swift：类与重写
来源：http://oii.gogol.net.cn

class A: Base { override func f() {} }
来源：http://dqk.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://xzh.jinyuanbaomall.cn

do { try f() } catch { print(error) }
来源：http://gtv.ydzc1.top

[T28] Swift：枚举
来源：http://klb.hammf.cn

enum Color { case red, green }
来源：http://hjf.xuanzx.com

[T29] Swift：guard 提前返回
来源：http://npe.nanxuanxn.top

guard let x = opt else { return }
来源：http://lmt.dianchejie.cn

[T30] Swift：协议
来源：http://qar.uphjek.com

protocol Shape { func area() -> Double }
来源：http://smr.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://aus.xingfuxueyuan.xyz

print("Hello")
来源：http://dim.xuanzx.com

[T32] Lua：局部变量
来源：http://qsc.jinqigfzy.top

local a = 1
来源：http://izy.fktsv.cn

[T33] Lua：表（数组）
来源：http://ydg.shangyingyoupin.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gbz.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://fwx.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ief.dianchejie.cn

[T35] Lua：字典表
来源：http://hvy.smart0.xyz

local d = { a = 1 };  d.b = 2
来源：http://xym.shzxlz.cn

[T36] Lua：函数
来源：http://wfd.wangdashe.top

function add(a, b) return a + b end
来源：http://ezf.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://sis.xuetiantiany.cn

"a" .. "b"
来源：http://hum.zhengqikj.top

[T38] Lua：条件
来源：http://brl.nanxuanxn.top

if x > 0 then print("正") end
来源：http://jrc.quarkkingdee.top

[T39] Lua：模式匹配
来源：http://zhn.pengpengdd.cyou

string.find(s, "%d+")
来源：http://zys.ydzc1.top

[T40] Lua：元表
来源：http://jzn.bbcook.cn

setmetatable({}, { __index = base })
来源：http://yjr.hesvh.cn

[T41] Perl：Hello World
来源：http://wze.nanxinkj.top

print "Hello\n";
来源：http://lju.vqdsnc.cn

[T42] Perl：变量类型
来源：http://qaz.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hrz.pycfn.com

[T43] Perl：字符串插值
来源：http://ftv.nanxuanxn.top

"值: $a"
来源：http://gde.quarkkingdee.top

[T44] Perl：条件
来源：http://tuw.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://ats.yj20258.top

[T45] Perl：数组遍历
来源：http://oqi.gogol.net.cn

for my $x (@arr) { print $x; }
来源：http://sqg.hongshengwenyu.top

[T46] Perl：哈希操作
来源：http://xvr.0kj1m.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zgx.yuxming.cn

[T47] Perl：正则捕获
来源：http://bpx.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://meg.jianghu66.top

[T48] Perl：正则替换
来源：http://ecf.meibo888.top

$s =~ s/old/new/g;
来源：http://bmw.c1oappe.top

[T49] Perl：函数
来源：http://gfk.xuetiantiany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fwc.jqgfzy.top

[T50] Perl：逐行读文件
来源：http://fcr.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bqu.cdnleiting.top

while (my $line = <$fh>) { print $line; }
来源：http://kib.zdbjq.cn

[T51] Scala：Hello World
来源：http://ikg.zdqjudy.top

println("Hello")
来源：http://qxk.vehdjk.com

[T52] Scala：变量
来源：http://lxt.sweek.top

val a = 1;  var b = 2
来源：http://rqe.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://kzl.smart0.xyz

s"值: $b"
来源：http://pps.quarkkingdee.top

[T54] Scala：集合映射
来源：http://cha.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://nro.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://zbk.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://hwg.sxryk.cn

[T56] Scala：样例类
来源：http://hic.guowangkeji.top

case class User(name: String, age: Int)
来源：http://ovz.zdbjq.cn

[T57] Scala：模式匹配
来源：http://wcv.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://uqt.hfpthk.cn

[T58] Scala：函数定义
来源：http://fqb.dianchejie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://aur.cqqwz.cn

[T59] Scala：循环
来源：http://bgt.chenzaomai.com

for (i <- 1 to 10) println(i)
来源：http://dfa.zdbjq.cn

[T60] Scala：折叠
来源：http://uln.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mwo.svipenyu.cn

================================================================================
来源：http://sey.fktsv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lzc.zhengqikj.top

================================================================================
来源：http://bhy.chenzaomai.com

[U01] Py：创建虚拟环境
来源：http://yrc.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mnl.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://rgb.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hur.fktsv.cn

[U03] Py：加载 .env 配置
来源：http://euk.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hyp.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://lpb.yj20258.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ngp.yongpay.top

[U05] Py：列表去重且保序
来源：http://ljp.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://ovc.zycfv.cn

[U06] Py：合并两个字典
来源：http://qpz.xingfuxueyuan.xyz

{**a, **b}
来源：http://zfm.52xcode.cn

[U07] Py：反转字典键值
来源：http://ocz.jlsjyb.cn

{v: k for k, v in d.items()}
来源：http://lzk.jqgfzy.top

[U08] Py：展平二维列表
来源：http://tqz.yonumen.top

[y for x in nested for y in x]
来源：http://inz.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://tfu.jinqigufen.top

max(d, key=d.get)
来源：http://amp.yj20258.top

[U10] Py：按值排序字典
来源：http://nod.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pzw.zycfv.cn

[U11] Py：生成器表达式
来源：http://whb.redwolf501.top

(x * 2 for x in arr)
来源：http://ler.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lld.nanxuanxn.top

Counter(arr).most_common(3)
来源：http://hon.pengpengdd.cyou

[U13] Py：固定长度队列
来源：http://klr.zhixingplan.top

deque(maxlen=10)
来源：http://fyd.zhaomingkeji.xyz

[U14] Py：分组收集到列表
来源：http://gvy.yuanzhike.top

defaultdict(list)
来源：http://mxi.tianlin.xyz

[U15] Py：高精度计时
来源：http://fyr.xylfe.cn

t = time.perf_counter()
来源：http://dvk.hcnkem.com

[U16] Py：命令行参数解析
来源：http://hfy.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://trk.c1oappe.top

[U17] Py：初始化日志
来源：http://kqe.hammf.cn

logging.basicConfig(level=logging.INFO)
来源：http://nkm.quarkkingdee.top

[U18] Py：预编译正则
来源：http://wcx.meibo888.top

pat = re.compile(r"\d+")
来源：http://ggg.bjfxy.top


<!-- 参考信息 -->