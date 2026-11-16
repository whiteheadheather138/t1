代发 wailian999

read -rp "请输入: " ans
来源：http://obd.aibaodan.cn

[R78] 交互式菜单
来源：http://kvk.cucudq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fiq.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://ldc.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nys.chenzaomai.com

[R80] 查看脚本执行耗时
来源：http://akz.iojbl.cn

time ./run.sh
来源：http://nre.daria6918.cn

================================================================================
来源：http://tkz.shuidangran.top

S. C / C++ 专题
来源：http://rsh.zhiwuduotai.top

================================================================================
来源：http://ifg.kuanghao11.cn

[S01] C：Hello World
来源：http://tzi.chenzaomai.com

#include <stdio.h>
来源：http://oqc.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lvh.fehbvm.com

[S02] C：变量与格式化输出
来源：http://edd.shangyingyoupin.top

int a = 10; printf("%d\n", a);
来源：http://wbk.sysykeji.top

[S03] C：读入整数
来源：http://upr.fengsongda.top

int x; scanf("%d", &x);
来源：http://rek.sjlbkw.cn

[S04] C：字符串复制
来源：http://wmj.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://itn.uphjek.com

[S05] C：字符串长度
来源：http://grz.nwbrower.top

strlen(s)
来源：http://jck.fzhhl.top

[S06] C：字符串比较
来源：http://kwb.aizwys.cn

strcmp(a, b) == 0
来源：http://sco.mhx1999.top

[S07] C：数组遍历求和
来源：http://gya.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fgs.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://gmt.52xcode.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bxa.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://ohk.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jrw.chenlongwang.top

[S10] C：指针与解引用
来源：http://jow.andypj.xyz

int *p = &a;  *p = 5;
来源：http://air.daria6918.cn

[S11] C：逐行读文件
来源：http://wnj.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://ehg.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wrv.nanxuanxn.top

fclose(f);
来源：http://bzg.xingfuxueyuan.xyz

[S12] C：写文件
来源：http://voq.ppjwa.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mjb.316326.xyz

[S13] C：宏定义
来源：http://mou.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uoc.sysykeji.top

[S14] C：枚举
来源：http://nkn.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://kwj.xingfuxueyuan.xyz

[S15] C：类型转换
来源：http://bdu.havefunace.top

(double) a / b
来源：http://wsb.xylfe.cn

[S16] C：位操作置位
来源：http://iwf.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://nph.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://ykm.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nzv.hnxiangtu.top

[S18] C：命令行参数
来源：http://wch.sufxvd.cn

int main(int argc, char **argv)
来源：http://fri.guowangkeji.top

[S19] C：快速排序
来源：http://ghh.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://ghx.52xcode.cn

[S20] C：二分查找
来源：http://uui.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://smx.yj20258888.top

[S21] C：字符类别判断
来源：http://ecs.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sxd.vqdsnc.cn

[S22] C：字符串转数字
来源：http://snd.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://bkh.daria6918.cn

[S23] C：随机数
来源：http://fig.cqqwz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jez.fzhhl.top

[S24] C：获取本地时间
来源：http://mum.wangshuangyany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dse.nanxuanxn.top

[S25] C：内存拷贝
来源：http://cyo.yonumen.top

memcpy(dst, src, n);
来源：http://vew.fktsv.cn

[S26] C：内存清零
来源：http://sca.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://ypo.xinyue.icu

[S27] C：定义常量
来源：http://rfk.daria6918.cn

const double PI = 3.14159;
来源：http://gdw.bjfxy.top

[S28] C：静态变量
来源：http://jco.sysykeji.top

static int counter = 0;
来源：http://yrg.tanke756.top

[S29] C：变参函数
来源：http://dtn.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tdg.sjlbkw.cn

[S30] C：头文件保护
来源：http://doz.jlsjyb.cn

#ifndef X_H
来源：http://dmi.vehdjk.com

#define X_H
来源：http://tqh.yuanzhike.top

#endif
来源：http://sbo.vqdsnc.cn

[S31] C++：Hello World
来源：http://rsl.wangdashe.top

#include <iostream>
来源：http://ylv.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://dqq.shzxlz.cn

[S32] C++：字符串
来源：http://ngg.zhongyouzk.top

std::string s = "hi";  s += "!";
来源：http://yoq.zhoulong.xyz

[S33] C++：vector 增删
来源：http://vwe.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vrn.fehbvm.com

[S34] C++：遍历 vector
来源：http://myq.chenlongwang.top

for (auto &x : v) { std::cout << x; }
来源：http://upd.nwbrower.top

[S35] C++：map
来源：http://zly.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dkq.gaohongyu789.top

[S36] C++：unordered_map
来源：http://pvr.zhoulong.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://czb.kuanghao11.cn

[S37] C++：set
来源：http://jiw.hnxiangtu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rff.gotoacloud.top

[S38] C++：排序
来源：http://gvk.shanyushiyangtech.top

std::sort(v.begin(), v.end());
来源：http://isa.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://ree.pycfn.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ovj.gogol.net.cn

[S40] C++：查找元素
来源：http://pqb.yonumen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aue.hesvh.cn

[S41] C++：类与构造函数
来源：http://arm.yuanzhike.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kmw.wangshuangyany.cn

[S42] C++：继承与虚函数
来源：http://dyg.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://ykt.jinqigfzy.top

[S43] C++：智能指针
来源：http://wwj.guowangkeji.top

auto p = std::make_unique<int>(5);
来源：http://zbh.snrcjt.cn

[S44] C++：引用传参
来源：http://qpl.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://ahp.yanxiufei.cn

[S45] C++：lambda
来源：http://lje.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://ufg.316326.xyz

[S46] C++：函数模板
来源：http://vsh.zhiwuduotai.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://old.cucudq.cn

[S47] C++：结构化绑定遍历
来源：http://xjl.ywan-chungtsiang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pxi.ctjpmb.com

[S48] C++：逐行读文件
来源：http://old.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://glz.guannengcc.top

while (std::getline(in, line)) { }
来源：http://sns.yangfankeji.com

[S49] C++：写文件
来源：http://xrx.yangfankeji.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dcd.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://jae.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kqi.shuidangran.top

[S51] C++：显式类型转换
来源：http://ltd.haohaochexian.top

static_cast<double>(a) / b
来源：http://htv.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://pbj.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://yad.cheryme.top

[S53] C++：移动语义
来源：http://vhr.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://irx.nanxinkj.top

[S54] C++：异常处理
来源：http://pxj.daria6918.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://key.dashuyun.cn

[S55] C++：结构化绑定
来源：http://ose.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://kpo.cheryme.top

[S56] C++：optional
来源：http://qkb.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fwn.kuanghao11.cn

[S57] C++：编译期常量
来源：http://qbp.tian-w.cn

constexpr int N = 10;
来源：http://yjn.52xcode.cn

[S58] C++：命名空间
来源：http://snd.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://gfy.chenlongwang.top

[S59] C++：静态断言
来源：http://iog.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uwq.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://eun.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://icj.xylfe.cn

================================================================================
来源：http://nak.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ial.yanxiufei.cn

================================================================================
来源：http://ceu.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://gui.hysaishi.cn

println("Hello")
来源：http://vca.jianghu66.top

[T02] Kotlin：变量
来源：http://yck.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jhq.ppjwa.cn

[T03] Kotlin：字符串模板
来源：http://zwz.gzhubu.top

"值: $b"
来源：http://oei.wangshuangyany.cn

[T04] Kotlin：空安全
来源：http://fyk.52xcode.cn

val n: String? = null;  n?.length
来源：http://nlu.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://jlk.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wix.daria6918.cn

[T06] Kotlin：集合映射
来源：http://xdh.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eqn.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://wzn.hammf.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rwy.zhoulong.xyz

[T08] Kotlin：数据类
来源：http://hjj.meibo888.top

data class User(val name: String, val age: Int)
来源：http://our.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://ndo.hammf.cn

fun String.exclaim() = this + "!"
来源：http://wnk.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://bzu.xuetiantiany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://evo.xziqi.cn

[T11] Kotlin：协程
来源：http://agt.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yrt.chenlongwang.top

[T12] Kotlin：解构声明
来源：http://kxp.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://ife.chenlongwang.top

[T13] Kotlin：只读 Map
来源：http://ozc.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://rtl.haohaochexian.top

[T14] Kotlin：循环
来源：http://zra.xuanzx.com

for (i in 1..10) println(i)
来源：http://thg.smart0.xyz

[T15] Kotlin：接口
来源：http://bbk.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://sch.gogol.net.cn

[T16] Swift：Hello World
来源：http://qrh.pycfn.com

print("Hello")
来源：http://oif.ctjpmb.com

[T17] Swift：变量与常量
来源：http://oyh.feifeiyinyue.top

var a = 1;  let b = 2
来源：http://evn.zhijiandao.cn

[T18] Swift：字符串插值
来源：http://pmr.chenlongwang.top

"值: \(b)"
来源：http://tjs.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://rks.daxiang520.top

if let n = opt { print(n) }
来源：http://esf.cashguo.top

[T20] Swift：数组操作
来源：http://hoa.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://pgl.yongpay.top

[T21] Swift：遍历
来源：http://ucf.feifeiyinyue.top

for x in a { print(x) }
来源：http://zli.hysaishi.cn

[T22] Swift：字典
来源：http://fqy.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://kpy.feifeiyinyue.top

[T23] Swift：函数
来源：http://qpq.jyoumei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jfv.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://gbb.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://evt.hcnkem.com

[T25] Swift：结构体
来源：http://nxu.c1oappe.top

struct P { var x: Int }
来源：http://mao.kuanghao11.cn

[T26] Swift：类与重写
来源：http://jfs.shanyushiyangkeji.top

class A: Base { override func f() {} }
来源：http://jde.jinqigufen.top

[T27] Swift：错误处理
来源：http://dbp.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://flx.jqgfzy.top

[T28] Swift：枚举
来源：http://zhm.sxryk.cn

enum Color { case red, green }
来源：http://suh.pycfn.com

[T29] Swift：guard 提前返回
来源：http://ede.yj20258.top

guard let x = opt else { return }
来源：http://elk.316326.xyz

[T30] Swift：协议
来源：http://zqf.9152youxi.cn

protocol Shape { func area() -> Double }
来源：http://lzt.nanxuanxn.top

[T31] Lua：Hello World
来源：http://rgm.hesvh.cn

print("Hello")
来源：http://afs.guannengcc.top

[T32] Lua：局部变量
来源：http://ccx.zhongyouzk.top

local a = 1
来源：http://yqd.52xcode.cn

[T33] Lua：表（数组）
来源：http://fkw.daria6918.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nbe.fehbvm.com

[T34] Lua：遍历表
来源：http://ucj.kuanghao11.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nnz.shanyushiyangkeji.top

[T35] Lua：字典表
来源：http://kgv.daria6918.cn

local d = { a = 1 };  d.b = 2
来源：http://yqp.yvedp.cn

[T36] Lua：函数
来源：http://mvl.yj202588.top

function add(a, b) return a + b end
来源：http://rxv.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://cga.dashuyun.cn

"a" .. "b"
来源：http://yin.gzhubu.top

[T38] Lua：条件
来源：http://pfg.jqgfzy.top

if x > 0 then print("正") end
来源：http://vwp.gzhubu.top

[T39] Lua：模式匹配
来源：http://ueg.yangfankeji.com

string.find(s, "%d+")
来源：http://jav.birdmap.top

[T40] Lua：元表
来源：http://rja.tianlin.xyz

setmetatable({}, { __index = base })
来源：http://cfm.smart0.xyz

[T41] Perl：Hello World
来源：http://qwn.redwolf501.top

print "Hello\n";
来源：http://lgv.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://kth.hfpthk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xiq.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://oin.fanxiaobao.xyz

"值: $a"
来源：http://dzg.jlsjyb.cn

[T44] Perl：条件
来源：http://hnf.yj20258.top

if ($a > 0) { print "正"; }
来源：http://lkq.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://sdg.yonumen.top

for my $x (@arr) { print $x; }
来源：http://hao.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://pbu.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://opp.jiagoushi.top

[T47] Perl：正则捕获
来源：http://sun.shanyushiyangtech.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vfj.jianghu66.top

[T48] Perl：正则替换
来源：http://brh.yangfankeji.com

$s =~ s/old/new/g;
来源：http://caw.jinghuilouyu.cn

[T49] Perl：函数
来源：http://ymn.jqgufenzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sij.zhixingplan.top

[T50] Perl：逐行读文件
来源：http://etp.zdqjudy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ucl.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://eem.316326.xyz

[T51] Scala：Hello World
来源：http://ran.yuxming.cn

println("Hello")
来源：http://iqe.sysykeji.top

[T52] Scala：变量
来源：http://jxz.tanke756.top

val a = 1;  var b = 2
来源：http://olt.jianghu66.top

[T53] Scala：字符串插值
来源：http://oxo.zdbjq.cn

s"值: $b"
来源：http://wjd.zhengqikj.top

[T54] Scala：集合映射
来源：http://tjn.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://jnr.shanyushiyangtech.top

[T55] Scala：集合过滤
来源：http://yys.ivvv.top

List(1, 2, 3).filter(_ > 1)
来源：http://rhw.smart0.xyz

[T56] Scala：样例类
来源：http://afb.jinghuilouyu.cn

case class User(name: String, age: Int)
来源：http://osh.zycfv.cn

[T57] Scala：模式匹配
来源：http://stj.fzhhl.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dhy.aibaodan.cn

[T58] Scala：函数定义
来源：http://sse.yonumen.top

def add(a: Int, b: Int): Int = a + b
来源：http://ieh.hesvh.cn

[T59] Scala：循环
来源：http://fcx.9152youxi.cn

for (i <- 1 to 10) println(i)
来源：http://pzb.fehbvm.com

[T60] Scala：折叠
来源：http://nkx.pengpengdd.cyou

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qvp.52xcode.cn

================================================================================
来源：http://psh.fzhhl.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xhx.yuanzhike.top

================================================================================
来源：http://uak.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://gzy.ctjpmb.com

python -m venv .venv && source .venv/bin/activate
来源：http://ucu.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://egb.wangshuangyany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vof.pycfn.com

[U03] Py：加载 .env 配置
来源：http://lzi.chenlongwang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mmq.wangdashe.top

[U04] Py：变量调试打印
来源：http://gna.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bku.ppjwa.cn

[U05] Py：列表去重且保序
来源：http://hae.cashguo.top

list(dict.fromkeys(arr))
来源：http://hck.chenzaomai.com

[U06] Py：合并两个字典
来源：http://jje.uphjek.com

{**a, **b}
来源：http://gpu.vehdjk.com

[U07] Py：反转字典键值
来源：http://txi.fehbvm.com

{v: k for k, v in d.items()}
来源：http://fdw.pycfn.com

[U08] Py：展平二维列表
来源：http://qaj.haohaochexian.top

[y for x in nested for y in x]
来源：http://rpb.yuxming.cn

[U09] Py：字典取最大值的键
来源：http://vwc.quarkkingdee.top

max(d, key=d.get)
来源：http://qrn.shuidangran.top

[U10] Py：按值排序字典
来源：http://ekw.nwbrower.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yfo.fktsv.cn

[U11] Py：生成器表达式
来源：http://jio.cheryme.top

(x * 2 for x in arr)
来源：http://ikh.kuanghao11.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uut.xylfe.cn

Counter(arr).most_common(3)
来源：http://vvz.ctjpmb.com

[U13] Py：固定长度队列
来源：http://syl.sysykeji.top

deque(maxlen=10)
来源：http://zrq.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://fcc.sjlbkw.cn

defaultdict(list)
来源：http://kgv.shanyushiyangkeji.top

[U15] Py：高精度计时
来源：http://dha.sweek.top

t = time.perf_counter()
来源：http://rsr.epnwcf.com

[U16] Py：命令行参数解析
来源：http://ulz.zhengqikj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bvw.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://qpn.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://aru.ppjwa.cn

[U18] Py：预编译正则
来源：http://yvm.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://lwe.chenzaomai.com


<!-- 参考信息 -->