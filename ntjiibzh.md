代发 wailian999

read -rp "请输入: " ans
来源：http://aqr.gogol.net.cn

[R78] 交互式菜单
来源：http://tbq.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://zkz.ctjpmb.com

[R79] 解析命令行选项
来源：http://vgh.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cvd.hammf.cn

[R80] 查看脚本执行耗时
来源：http://vrf.yonumen.top

time ./run.sh
来源：http://uzy.hnxiangtu.top

================================================================================
来源：http://zal.hysaishi.cn

S. C / C++ 专题
来源：http://qwf.kuanghao11.cn

================================================================================
来源：http://tqh.yangfankeji.com

[S01] C：Hello World
来源：http://ivo.yanxiufei.cn

#include <stdio.h>
来源：http://azc.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://azv.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://inn.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://kka.guannengcc.top

[S03] C：读入整数
来源：http://fng.zhaomingkeji.xyz

int x; scanf("%d", &x);
来源：http://ysr.hfpthk.cn

[S04] C：字符串复制
来源：http://vlj.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://mfp.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://ocs.jqgfzy.top

strlen(s)
来源：http://slj.gzhubu.top

[S06] C：字符串比较
来源：http://ddz.zhengqikj.top

strcmp(a, b) == 0
来源：http://qoj.gzhubu.top

[S07] C：数组遍历求和
来源：http://vvu.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rac.bbcook.cn

[S08] C：动态内存分配与释放
来源：http://olc.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uku.sweek.top

[S09] C：结构体定义与初始化
来源：http://auz.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jix.yuxming.cn

[S10] C：指针与解引用
来源：http://ggg.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://est.ehwqpu.com

[S11] C：逐行读文件
来源：http://kii.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://eiw.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gwr.guannengcc.top

fclose(f);
来源：http://zxi.c1oappe.top

[S12] C：写文件
来源：http://bjo.fengsongda.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://twv.zhixingplan.top

[S13] C：宏定义
来源：http://sqx.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nmf.smart0.xyz

[S14] C：枚举
来源：http://kgp.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://vvk.sxryk.cn

[S15] C：类型转换
来源：http://uyd.nwbrower.top

(double) a / b
来源：http://znz.nanxuanxn.top

[S16] C：位操作置位
来源：http://gxi.gogol.net.cn

x |= (1 << 3);
来源：http://ixg.dianchejie.cn

[S17] C：安全拼接字符串
来源：http://rue.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iwn.yangfankeji.com

[S18] C：命令行参数
来源：http://wwk.gzhubu.top

int main(int argc, char **argv)
来源：http://qno.gaohongyu789.top

[S19] C：快速排序
来源：http://kmu.9152youxi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rum.316326.xyz

[S20] C：二分查找
来源：http://yvv.bjfxy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nnv.zhixingplan.top

[S21] C：字符类别判断
来源：http://grj.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vjd.jyoumei.cn

[S22] C：字符串转数字
来源：http://icb.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tgo.pycfn.com

[S23] C：随机数
来源：http://ujc.hcnkem.com

srand(time(NULL));  int r = rand() % 100;
来源：http://iou.uphjek.com

[S24] C：获取本地时间
来源：http://duo.cqqwz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://otk.tian-w.cn

[S25] C：内存拷贝
来源：http://rdb.snrcjt.cn

memcpy(dst, src, n);
来源：http://vyu.xziqi.cn

[S26] C：内存清零
来源：http://imf.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://rux.yvedp.cn

[S27] C：定义常量
来源：http://eft.wangdashe.top

const double PI = 3.14159;
来源：http://agb.zdbjq.cn

[S28] C：静态变量
来源：http://wqw.quarkkingdee.top

static int counter = 0;
来源：http://ixo.cqqwz.cn

[S29] C：变参函数
来源：http://fbf.daria6918.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nsu.zdqjudy.top

[S30] C：头文件保护
来源：http://lhz.fengsongda.top

#ifndef X_H
来源：http://sgu.jiagoushi.top

#define X_H
来源：http://air.shanyushiyangtech.top

#endif
来源：http://tpc.sweek.top

[S31] C++：Hello World
来源：http://tnz.shanyushiyangtech.top

#include <iostream>
来源：http://plg.ydjk.org.cn

int main() { std::cout << "Hello\n"; }
来源：http://qsh.xziqi.cn

[S32] C++：字符串
来源：http://rhv.xingfuxueyuan.xyz

std::string s = "hi";  s += "!";
来源：http://ygy.iojbl.cn

[S33] C++：vector 增删
来源：http://qeo.yanxiufei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://adm.gogol.net.cn

[S34] C++：遍历 vector
来源：http://ofh.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://dtm.ehwqpu.com

[S35] C++：map
来源：http://sdl.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zjz.redwolf501.top

[S36] C++：unordered_map
来源：http://kwo.yueranfly.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uhf.cucudq.cn

[S37] C++：set
来源：http://jjy.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xpq.shzxlz.cn

[S38] C++：排序
来源：http://dwr.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://szl.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://eqa.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ubc.jianghu66.top

[S40] C++：查找元素
来源：http://bjd.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://noc.yongpay.top

[S41] C++：类与构造函数
来源：http://jcj.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://izc.iojbl.cn

[S42] C++：继承与虚函数
来源：http://pco.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://aue.yfazqb.com

[S43] C++：智能指针
来源：http://fyp.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://tir.ivvv.top

[S44] C++：引用传参
来源：http://gif.hnxiangtu.top

void inc(int &x) { ++x; }
来源：http://nbd.fengsongda.top

[S45] C++：lambda
来源：http://iqk.ywan-chungtsiang.top

auto add = [](int a, int b) { return a + b; };
来源：http://ctv.ivvv.top

[S46] C++：函数模板
来源：http://dps.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://arj.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://ria.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ocr.pycfn.com

[S48] C++：逐行读文件
来源：http://sve.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mfd.fengsongda.top

while (std::getline(in, line)) { }
来源：http://bgx.shangyingyoupin.top

[S49] C++：写文件
来源：http://fvk.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vtm.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://cmb.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://usf.zhixingplan.top

[S51] C++：显式类型转换
来源：http://mhe.zhoulong.xyz

static_cast<double>(a) / b
来源：http://uss.daxiang520.top

[S52] C++：const 与 noexcept
来源：http://emr.shanyushiyangkeji.top

int size() const noexcept { return n_; }
来源：http://elp.jqgufenzy.top

[S53] C++：移动语义
来源：http://yls.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://yey.ehwqpu.com

[S54] C++：异常处理
来源：http://mxj.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rsx.xylfe.cn

[S55] C++：结构化绑定
来源：http://cub.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qvj.shzxlz.cn

[S56] C++：optional
来源：http://pew.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dvm.fzhhl.top

[S57] C++：编译期常量
来源：http://hkc.dashuyun.cn

constexpr int N = 10;
来源：http://ync.meibo888.top

[S58] C++：命名空间
来源：http://gzp.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://ijn.c1oappe.top

[S59] C++：静态断言
来源：http://giy.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://obd.jyoumei.cn

[S60] C++：遍历并删除元素
来源：http://iwe.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kjm.smart0.xyz

================================================================================
来源：http://bwx.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sgh.sjlbkw.cn

================================================================================
来源：http://kgj.xuetiantiany.cn

[T01] Kotlin：Hello World
来源：http://zcy.c1oappe.top

println("Hello")
来源：http://jlw.vqdsnc.cn

[T02] Kotlin：变量
来源：http://zev.dashuyun.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dsp.zhixingplan.top

[T03] Kotlin：字符串模板
来源：http://vxi.pengpengdd.cyou

"值: $b"
来源：http://nza.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://zyb.yonumen.top

val n: String? = null;  n?.length
来源：http://ypc.ydzc1.top

[T05] Kotlin：when 表达式
来源：http://ssx.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ors.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://dmt.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ben.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://sqe.jqgufenzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://shl.ctjpmb.com

[T08] Kotlin：数据类
来源：http://srj.xziqi.cn

data class User(val name: String, val age: Int)
来源：http://wyf.epnwcf.com

[T09] Kotlin：扩展函数
来源：http://vvf.uphjek.com

fun String.exclaim() = this + "!"
来源：http://fsj.daxiang520.top

[T10] Kotlin：默认参数
来源：http://thr.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uns.sjlbkw.cn

[T11] Kotlin：协程
来源：http://pem.fengsongda.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://veg.yonumen.top

[T12] Kotlin：解构声明
来源：http://rck.sweek.top

val (a, b) = Pair(1, 2)
来源：http://huj.chenlongwang.top

[T13] Kotlin：只读 Map
来源：http://kzg.aizwys.cn

val m = mapOf("a" to 1)
来源：http://rps.bbcook.cn

[T14] Kotlin：循环
来源：http://zlh.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://lmz.vqdsnc.cn

[T15] Kotlin：接口
来源：http://aoe.mhx1999.top

interface Shape { fun area(): Double }
来源：http://hwe.yj202588.top

[T16] Swift：Hello World
来源：http://xpz.c1oappe.top

print("Hello")
来源：http://tqx.yangfankeji.com

[T17] Swift：变量与常量
来源：http://yex.cucudq.cn

var a = 1;  let b = 2
来源：http://wkl.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://eqm.tanke756.top

"值: \(b)"
来源：http://fam.hnxiangtu.top

[T19] Swift：可选绑定
来源：http://ntg.uphjek.com

if let n = opt { print(n) }
来源：http://htl.jinqigfzy.top

[T20] Swift：数组操作
来源：http://ruj.epnwcf.com

var a = [1, 2, 3];  a.append(4)
来源：http://hlo.yangfankeji.com

[T21] Swift：遍历
来源：http://nrc.bbcook.cn

for x in a { print(x) }
来源：http://adm.andypj.xyz

[T22] Swift：字典
来源：http://gyd.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lwg.xziqi.cn

[T23] Swift：函数
来源：http://gom.fanxiaobao.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pjk.hysaishi.cn

[T24] Swift：闭包
来源：http://jtl.gotoacloud.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://aug.yangfankeji.com

[T25] Swift：结构体
来源：http://jfv.kuanghao11.cn

struct P { var x: Int }
来源：http://dxt.pengpengdd.cyou

[T26] Swift：类与重写
来源：http://hpb.cqqwz.cn

class A: Base { override func f() {} }
来源：http://qxj.hesvh.cn

[T27] Swift：错误处理
来源：http://yya.yueranfly.top

do { try f() } catch { print(error) }
来源：http://ooz.hammf.cn

[T28] Swift：枚举
来源：http://msh.jinghuilouyu.cn

enum Color { case red, green }
来源：http://ehq.jyoumei.cn

[T29] Swift：guard 提前返回
来源：http://lji.feifeiyinyue.top

guard let x = opt else { return }
来源：http://enz.xuetiantiany.cn

[T30] Swift：协议
来源：http://ntr.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://xha.jiagoushi.top

[T31] Lua：Hello World
来源：http://njb.yanxiufei.cn

print("Hello")
来源：http://aem.aizwys.cn

[T32] Lua：局部变量
来源：http://ohc.cdnleiting.top

local a = 1
来源：http://ctm.gotoacloud.top

[T33] Lua：表（数组）
来源：http://pjw.hongshengwenyu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://phj.cheryme.top

[T34] Lua：遍历表
来源：http://swv.cashguo.top

for i, v in ipairs(t) do print(i, v) end
来源：http://juc.yj20258.top

[T35] Lua：字典表
来源：http://zff.yj20258888.top

local d = { a = 1 };  d.b = 2
来源：http://qyo.dianchejie.cn

[T36] Lua：函数
来源：http://ppt.hfpthk.cn

function add(a, b) return a + b end
来源：http://oho.daria6918.cn

[T37] Lua：字符串拼接
来源：http://ddb.mhx1999.top

"a" .. "b"
来源：http://ddl.hnxiangtu.top

[T38] Lua：条件
来源：http://hqn.yuxming.cn

if x > 0 then print("正") end
来源：http://gal.gzhubu.top

[T39] Lua：模式匹配
来源：http://ktt.shzxlz.cn

string.find(s, "%d+")
来源：http://tsp.jqgufenzy.top

[T40] Lua：元表
来源：http://ckx.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://bpz.uphjek.com

[T41] Perl：Hello World
来源：http://uum.hesvh.cn

print "Hello\n";
来源：http://qfn.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://nsx.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nxb.cashguo.top

[T43] Perl：字符串插值
来源：http://zvm.yanxiufei.cn

"值: $a"
来源：http://clx.mhx1999.top

[T44] Perl：条件
来源：http://yss.uphjek.com

if ($a > 0) { print "正"; }
来源：http://idv.hfpthk.cn

[T45] Perl：数组遍历
来源：http://vyr.fehbvm.com

for my $x (@arr) { print $x; }
来源：http://cqn.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://tde.ywan-chungtsiang.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xei.wangshuangyany.cn

[T47] Perl：正则捕获
来源：http://mdt.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://vms.daxiang520.top

[T48] Perl：正则替换
来源：http://kcy.ivvv.top

$s =~ s/old/new/g;
来源：http://faw.guannengcc.top

[T49] Perl：函数
来源：http://yti.shuidangran.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cgh.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://mqn.hesvh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vwy.cheryme.top

while (my $line = <$fh>) { print $line; }
来源：http://bpg.0kj1m.cn

[T51] Scala：Hello World
来源：http://vdp.fanxiaobao.xyz

println("Hello")
来源：http://sic.fktsv.cn

[T52] Scala：变量
来源：http://awq.uphjek.com

val a = 1;  var b = 2
来源：http://jta.kuanghao11.cn

[T53] Scala：字符串插值
来源：http://eba.wangshuangyany.cn

s"值: $b"
来源：http://vea.chenzaomai.com

[T54] Scala：集合映射
来源：http://dfy.pycfn.com

List(1, 2, 3).map(_ * 2)
来源：http://gyk.ehwqpu.com

[T55] Scala：集合过滤
来源：http://mqu.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://zsr.gotoacloud.top

[T56] Scala：样例类
来源：http://jhj.shangyingyoupin.top

case class User(name: String, age: Int)
来源：http://pil.bjfxy.top

[T57] Scala：模式匹配
来源：http://tfp.yanxiufei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gom.yuanzhike.top

[T58] Scala：函数定义
来源：http://jkl.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://ali.fanxiaobao.xyz

[T59] Scala：循环
来源：http://ccj.316326.xyz

for (i <- 1 to 10) println(i)
来源：http://rax.yangfankeji.com

[T60] Scala：折叠
来源：http://rcl.fanxiaobao.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hed.meibo888.top

================================================================================
来源：http://umt.zhixingplan.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cda.yongpay.top

================================================================================
来源：http://abf.nwbrower.top

[U01] Py：创建虚拟环境
来源：http://gor.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ciq.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://uxq.pycfn.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pxe.ctjpmb.com

[U03] Py：加载 .env 配置
来源：http://arc.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cig.guannengcc.top

[U04] Py：变量调试打印
来源：http://gaj.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pmt.xinyue.icu

[U05] Py：列表去重且保序
来源：http://mxa.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://vks.xingfuxueyuan.xyz

[U06] Py：合并两个字典
来源：http://hvd.tanke756.top

{**a, **b}
来源：http://wlu.wangshuangyany.cn

[U07] Py：反转字典键值
来源：http://ycj.gaohongyu789.top

{v: k for k, v in d.items()}
来源：http://xjz.aizwys.cn

[U08] Py：展平二维列表
来源：http://zix.zhijiandao.cn

[y for x in nested for y in x]
来源：http://oej.gogol.net.cn

[U09] Py：字典取最大值的键
来源：http://lfm.gotoacloud.top

max(d, key=d.get)
来源：http://dkt.iojbl.cn

[U10] Py：按值排序字典
来源：http://zvi.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://imq.hysaishi.cn

[U11] Py：生成器表达式
来源：http://los.zhengqikj.top

(x * 2 for x in arr)
来源：http://iwb.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://juc.zdbjq.cn

Counter(arr).most_common(3)
来源：http://ngk.tarul.cn

[U13] Py：固定长度队列
来源：http://zcj.jqgufenzy.top

deque(maxlen=10)
来源：http://zjk.uphjek.com

[U14] Py：分组收集到列表
来源：http://cfi.nanxinkj.top

defaultdict(list)
来源：http://cdt.snrcjt.cn

[U15] Py：高精度计时
来源：http://ojn.zhengqikj.top

t = time.perf_counter()
来源：http://evd.gogol.net.cn

[U16] Py：命令行参数解析
来源：http://lpg.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vgg.chenjidiqi.icu

[U17] Py：初始化日志
来源：http://ahr.xinyue.icu

logging.basicConfig(level=logging.INFO)
来源：http://rev.feifeiyinyue.top

[U18] Py：预编译正则
来源：http://cjl.wangdashe.top

pat = re.compile(r"\d+")
来源：http://kba.sysykeji.top


<!-- 参考信息 -->