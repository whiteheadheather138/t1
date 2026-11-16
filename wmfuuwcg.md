代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pql.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://ijc.zhijiandao.cn

time ./run.sh
来源：http://jcs.tian-w.cn

================================================================================
来源：http://eer.jlsjyb.cn

S. C / C++ 专题
来源：http://ynw.vqdsnc.cn

================================================================================
来源：http://osg.jqgfzy.top

[S01] C：Hello World
来源：http://uyg.fanxiaobao.xyz

#include <stdio.h>
来源：http://pro.kuanghao11.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dvu.chenjidiqi.icu

[S02] C：变量与格式化输出
来源：http://gir.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://nfd.havefunace.top

[S03] C：读入整数
来源：http://pvw.fzhhl.top

int x; scanf("%d", &x);
来源：http://tfe.sxryk.cn

[S04] C：字符串复制
来源：http://toi.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://caq.gotoacloud.top

[S05] C：字符串长度
来源：http://ndn.sufxvd.cn

strlen(s)
来源：http://ugr.sweek.top

[S06] C：字符串比较
来源：http://bud.xziqi.cn

strcmp(a, b) == 0
来源：http://bug.yuanzhike.top

[S07] C：数组遍历求和
来源：http://fqj.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vkt.hnqzz.top

[S08] C：动态内存分配与释放
来源：http://lok.xingfuxueyuan.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ktb.yj20258888.top

[S09] C：结构体定义与初始化
来源：http://lna.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uxb.havefunace.top

[S10] C：指针与解引用
来源：http://sqv.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://nhu.guannengcc.top

[S11] C：逐行读文件
来源：http://kfy.quarkkingdee.top

FILE *f = fopen("a.txt", "r");
来源：http://gto.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rsh.smart0.xyz

fclose(f);
来源：http://dgm.jinqigufen.top

[S12] C：写文件
来源：http://nly.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vhv.yanxiufei.cn

[S13] C：宏定义
来源：http://gxv.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vnm.tarul.cn

[S14] C：枚举
来源：http://vfj.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://ykr.cheryme.top

[S15] C：类型转换
来源：http://yjh.uphjek.com

(double) a / b
来源：http://gte.ydjk.org.cn

[S16] C：位操作置位
来源：http://vrd.jqgfzy.top

x |= (1 << 3);
来源：http://dtd.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://wwu.yvedp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yiu.hysaishi.cn

[S18] C：命令行参数
来源：http://fya.vehdjk.com

int main(int argc, char **argv)
来源：http://rsa.pengpengdd.cyou

[S19] C：快速排序
来源：http://yek.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oge.cdnleiting.top

[S20] C：二分查找
来源：http://yvp.jqgfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cho.cheryme.top

[S21] C：字符类别判断
来源：http://khm.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lab.xuetiantiany.cn

[S22] C：字符串转数字
来源：http://dxo.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://cae.316326.xyz

[S23] C：随机数
来源：http://fhj.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ooh.aizwys.cn

[S24] C：获取本地时间
来源：http://fni.bjfxy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jxw.wangdashe.top

[S25] C：内存拷贝
来源：http://vfy.ehwqpu.com

memcpy(dst, src, n);
来源：http://uce.fengsongda.top

[S26] C：内存清零
来源：http://xyw.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://ncw.fengsongda.top

[S27] C：定义常量
来源：http://pqn.chenjidiqi.icu

const double PI = 3.14159;
来源：http://jkq.ybcxt.top

[S28] C：静态变量
来源：http://tkh.smart0.xyz

static int counter = 0;
来源：http://mxq.cashguo.top

[S29] C：变参函数
来源：http://zmx.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iwk.hcnkem.com

[S30] C：头文件保护
来源：http://yaj.shzxlz.cn

#ifndef X_H
来源：http://ams.yj202588.top

#define X_H
来源：http://soj.iojbl.cn

#endif
来源：http://ozv.zdbjq.cn

[S31] C++：Hello World
来源：http://tve.chenzaomai.com

#include <iostream>
来源：http://pvx.vqdsnc.cn

int main() { std::cout << "Hello\n"; }
来源：http://ufk.fktsv.cn

[S32] C++：字符串
来源：http://hwx.zhaomingkeji.xyz

std::string s = "hi";  s += "!";
来源：http://ucn.cqqwz.cn

[S33] C++：vector 增删
来源：http://vsm.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://msc.zhengqikj.top

[S34] C++：遍历 vector
来源：http://yag.kuanghao11.cn

for (auto &x : v) { std::cout << x; }
来源：http://cjq.xuanzx.com

[S35] C++：map
来源：http://kjh.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://stf.c1oappe.top

[S36] C++：unordered_map
来源：http://zvp.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kvk.xinyue.icu

[S37] C++：set
来源：http://znn.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dtz.fzhhl.top

[S38] C++：排序
来源：http://let.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://ych.hysaishi.cn

[S39] C++：自定义比较器排序
来源：http://iku.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wzb.havefunace.top

[S40] C++：查找元素
来源：http://ucd.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jno.jinqigfzy.top

[S41] C++：类与构造函数
来源：http://iom.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pfl.zdbjq.cn

[S42] C++：继承与虚函数
来源：http://qzg.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://isj.gzhubu.top

[S43] C++：智能指针
来源：http://swl.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://tzv.fehbvm.com

[S44] C++：引用传参
来源：http://qjt.hesvh.cn

void inc(int &x) { ++x; }
来源：http://qwt.quarkkingdee.top

[S45] C++：lambda
来源：http://pug.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://zmt.tanke756.top

[S46] C++：函数模板
来源：http://lea.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lcb.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://cqz.zdqjudy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cky.shzxlz.cn

[S48] C++：逐行读文件
来源：http://pzj.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://gnw.daxiang520.top

while (std::getline(in, line)) { }
来源：http://ajq.jinqigufen.top

[S49] C++：写文件
来源：http://lpp.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cln.jlsjyb.cn

[S50] C++：格式化数字
来源：http://suy.shangyingyoupin.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rlp.dianchejie.cn

[S51] C++：显式类型转换
来源：http://hgr.dashuyun.cn

static_cast<double>(a) / b
来源：http://aju.kuanghao11.cn

[S52] C++：const 与 noexcept
来源：http://xtk.uphjek.com

int size() const noexcept { return n_; }
来源：http://pta.zdbjq.cn

[S53] C++：移动语义
来源：http://grv.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://hsg.fzhhl.top

[S54] C++：异常处理
来源：http://vwa.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aca.0kj1m.cn

[S55] C++：结构化绑定
来源：http://nra.birdmap.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vqb.nwbrower.top

[S56] C++：optional
来源：http://mhr.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nqw.hysaishi.cn

[S57] C++：编译期常量
来源：http://knr.ppjwa.cn

constexpr int N = 10;
来源：http://xqc.0kj1m.cn

[S58] C++：命名空间
来源：http://tfs.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://sgt.chenjidiqi.icu

[S59] C++：静态断言
来源：http://xbq.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yby.cheryme.top

[S60] C++：遍历并删除元素
来源：http://lvj.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vrc.kuanghao11.cn

================================================================================
来源：http://dzw.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://msr.jiagoushi.top

================================================================================
来源：http://ron.redwolf501.top

[T01] Kotlin：Hello World
来源：http://jwu.fktsv.cn

println("Hello")
来源：http://trd.fzhhl.top

[T02] Kotlin：变量
来源：http://hcl.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xux.havefunace.top

[T03] Kotlin：字符串模板
来源：http://yws.fengsongda.top

"值: $b"
来源：http://gmu.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://dem.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://krx.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://nlu.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://byy.iojbl.cn

[T06] Kotlin：集合映射
来源：http://ynu.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mky.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://tfq.tian-w.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pua.dianchejie.cn

[T08] Kotlin：数据类
来源：http://hyj.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://iku.yj202588.top

[T09] Kotlin：扩展函数
来源：http://hiy.hywenlv.cn

fun String.exclaim() = this + "!"
来源：http://qfq.cashguo.top

[T10] Kotlin：默认参数
来源：http://pct.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ftw.zdqjudy.top

[T11] Kotlin：协程
来源：http://dfr.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://imf.smart0.xyz

[T12] Kotlin：解构声明
来源：http://uox.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://oqh.dashuyun.cn

[T13] Kotlin：只读 Map
来源：http://gsw.sweek.top

val m = mapOf("a" to 1)
来源：http://ctr.tarul.cn

[T14] Kotlin：循环
来源：http://yap.sysykeji.top

for (i in 1..10) println(i)
来源：http://apg.zhixingplan.top

[T15] Kotlin：接口
来源：http://ubc.bjfxy.top

interface Shape { fun area(): Double }
来源：http://eel.xinyue.icu

[T16] Swift：Hello World
来源：http://dxn.zhaomingkeji.xyz

print("Hello")
来源：http://lwl.jinyuanbaomall.cn

[T17] Swift：变量与常量
来源：http://ubn.feifeiyinyue.top

var a = 1;  let b = 2
来源：http://wmo.sufxvd.cn

[T18] Swift：字符串插值
来源：http://toj.cdnleiting.top

"值: \(b)"
来源：http://gwj.gzhubu.top

[T19] Swift：可选绑定
来源：http://qmw.zhengqikj.top

if let n = opt { print(n) }
来源：http://xah.fehbvm.com

[T20] Swift：数组操作
来源：http://lhe.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://rhg.haohaochexian.top

[T21] Swift：遍历
来源：http://xwl.zhaomingkeji.xyz

for x in a { print(x) }
来源：http://iod.xylfe.cn

[T22] Swift：字典
来源：http://fnz.zhixingplan.top

var d = ["a": 1];  d["b"] = 2
来源：http://fmx.xylfe.cn

[T23] Swift：函数
来源：http://syi.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://caf.tarul.cn

[T24] Swift：闭包
来源：http://nfo.xinyue.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://qzd.jiagoushi.top

[T25] Swift：结构体
来源：http://ktz.zhijiandao.cn

struct P { var x: Int }
来源：http://owc.jyoumei.cn

[T26] Swift：类与重写
来源：http://fzd.yuxming.cn

class A: Base { override func f() {} }
来源：http://mvy.quarkkingdee.top

[T27] Swift：错误处理
来源：http://khf.yj20258.top

do { try f() } catch { print(error) }
来源：http://kig.haohaochexian.top

[T28] Swift：枚举
来源：http://hpp.tarul.cn

enum Color { case red, green }
来源：http://for.yanxiufei.cn

[T29] Swift：guard 提前返回
来源：http://lsp.tian-w.cn

guard let x = opt else { return }
来源：http://lbg.iojbl.cn

[T30] Swift：协议
来源：http://jqm.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://gfw.hywenlv.cn

[T31] Lua：Hello World
来源：http://ppj.tianlin.xyz

print("Hello")
来源：http://mzj.shanyushiyangkeji.top

[T32] Lua：局部变量
来源：http://qza.kuanghao11.cn

local a = 1
来源：http://sif.vqdsnc.cn

[T33] Lua：表（数组）
来源：http://kmv.sjlbkw.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rmz.cucudq.cn

[T34] Lua：遍历表
来源：http://sfo.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://prn.52xcode.cn

[T35] Lua：字典表
来源：http://wjn.zhongyouzk.top

local d = { a = 1 };  d.b = 2
来源：http://sod.hnxiangtu.top

[T36] Lua：函数
来源：http://svl.9152youxi.cn

function add(a, b) return a + b end
来源：http://rzs.yvedp.cn

[T37] Lua：字符串拼接
来源：http://fbi.yfazqb.com

"a" .. "b"
来源：http://vju.dashuyun.cn

[T38] Lua：条件
来源：http://gkt.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://xbd.9152youxi.cn

[T39] Lua：模式匹配
来源：http://pvr.yueranfly.top

string.find(s, "%d+")
来源：http://wiy.hnxiangtu.top

[T40] Lua：元表
来源：http://zpk.svipenyu.cn

setmetatable({}, { __index = base })
来源：http://pbr.cheryme.top

[T41] Perl：Hello World
来源：http://sek.kuanghao11.cn

print "Hello\n";
来源：http://lup.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://jgo.nanxinkj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://emy.aibaodan.cn

[T43] Perl：字符串插值
来源：http://wgr.nanxuanxn.top

"值: $a"
来源：http://dsg.ehwqpu.com

[T44] Perl：条件
来源：http://sdv.pengpengdd.cyou

if ($a > 0) { print "正"; }
来源：http://jji.aibaodan.cn

[T45] Perl：数组遍历
来源：http://hhc.birdmap.top

for my $x (@arr) { print $x; }
来源：http://oiw.hnqzz.top

[T46] Perl：哈希操作
来源：http://utr.zhengqikj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wkw.zdbjq.cn

[T47] Perl：正则捕获
来源：http://zdo.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qcb.sxryk.cn

[T48] Perl：正则替换
来源：http://nvr.mhx1999.top

$s =~ s/old/new/g;
来源：http://omu.cheryme.top

[T49] Perl：函数
来源：http://vlf.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ial.iojbl.cn

[T50] Perl：逐行读文件
来源：http://deu.316326.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://tkl.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://crj.haohaochexian.top

[T51] Scala：Hello World
来源：http://jen.aibaodan.cn

println("Hello")
来源：http://hve.zhijiandao.cn

[T52] Scala：变量
来源：http://edz.sufxvd.cn

val a = 1;  var b = 2
来源：http://tib.shuidangran.top

[T53] Scala：字符串插值
来源：http://jms.haohaochexian.top

s"值: $b"
来源：http://zym.ydzc1.top

[T54] Scala：集合映射
来源：http://qco.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://boe.yongpay.top

[T55] Scala：集合过滤
来源：http://tig.fengsongda.top

List(1, 2, 3).filter(_ > 1)
来源：http://ymn.yongpay.top

[T56] Scala：样例类
来源：http://qjb.daria6918.cn

case class User(name: String, age: Int)
来源：http://huv.yj20258888.top

[T57] Scala：模式匹配
来源：http://ink.hnxiangtu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eot.andypj.xyz

[T58] Scala：函数定义
来源：http://vwa.hywenlv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tss.havefunace.top

[T59] Scala：循环
来源：http://pcs.aibaodan.cn

for (i <- 1 to 10) println(i)
来源：http://knm.yj20258888.top

[T60] Scala：折叠
来源：http://fnh.zhaomingkeji.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jhm.ehwqpu.com

================================================================================
来源：http://dkq.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fel.tian-w.cn

================================================================================
来源：http://lgi.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://fll.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://smz.havefunace.top

[U02] Py：导出 / 安装依赖
来源：http://nmt.epnwcf.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pqw.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://xju.dianchejie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gme.sysykeji.top

[U04] Py：变量调试打印
来源：http://tzc.yj20258.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ajb.yfazqb.com

[U05] Py：列表去重且保序
来源：http://rzo.sufxvd.cn

list(dict.fromkeys(arr))
来源：http://kcz.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://rai.sjlbkw.cn

{**a, **b}
来源：http://xfh.hammf.cn

[U07] Py：反转字典键值
来源：http://dkq.zhaomingkeji.xyz

{v: k for k, v in d.items()}
来源：http://rvs.fzhhl.top

[U08] Py：展平二维列表
来源：http://rth.cheryme.top

[y for x in nested for y in x]
来源：http://ivu.daria6918.cn

[U09] Py：字典取最大值的键
来源：http://lvd.zhongyouzk.top

max(d, key=d.get)
来源：http://dem.guowangkeji.top

[U10] Py：按值排序字典
来源：http://bcf.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://een.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://ezk.sweek.top

(x * 2 for x in arr)
来源：http://gvz.tianlin.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://jom.fktsv.cn

Counter(arr).most_common(3)
来源：http://fjf.cucudq.cn

[U13] Py：固定长度队列
来源：http://yhv.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://tgr.cheryme.top

[U14] Py：分组收集到列表
来源：http://mvw.sjlbkw.cn

defaultdict(list)
来源：http://bjr.xuanzx.com

[U15] Py：高精度计时
来源：http://znx.sxryk.cn

t = time.perf_counter()
来源：http://tgl.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://ulx.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://suj.tanke756.top

[U17] Py：初始化日志
来源：http://gcc.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://jty.daria6918.cn

[U18] Py：预编译正则
来源：http://fjk.zhijiandao.cn

pat = re.compile(r"\d+")
来源：http://bjx.redwolf501.top

[U19] Py：正则替换带回调
来源：http://htg.gotoacloud.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yxz.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://vjh.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://pfp.fehbvm.com


<!-- 参考信息 -->