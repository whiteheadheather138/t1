代发 wailian999

read -rp "请输入: " ans
来源：http://bfo.epnwcf.com

[R78] 交互式菜单
来源：http://tvk.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xrn.yj20258888.top

[R79] 解析命令行选项
来源：http://dhr.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tqn.zdqjudy.top

[R80] 查看脚本执行耗时
来源：http://fba.yuxming.cn

time ./run.sh
来源：http://lln.sweek.top

================================================================================
来源：http://eri.haohaochexian.top

S. C / C++ 专题
来源：http://oyj.xuanzx.com

================================================================================
来源：http://bho.jyoumei.cn

[S01] C：Hello World
来源：http://nmq.fzhhl.top

#include <stdio.h>
来源：http://ysy.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hhy.redwolf501.top

[S02] C：变量与格式化输出
来源：http://sdp.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://wxe.hnxiangtu.top

[S03] C：读入整数
来源：http://wsp.zhongyouzk.top

int x; scanf("%d", &x);
来源：http://jhk.52xcode.cn

[S04] C：字符串复制
来源：http://wva.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://erf.hcnkem.com

[S05] C：字符串长度
来源：http://edt.yanxiufei.cn

strlen(s)
来源：http://cwu.hnqzz.top

[S06] C：字符串比较
来源：http://wst.xuanzx.com

strcmp(a, b) == 0
来源：http://vxb.svipenyu.cn

[S07] C：数组遍历求和
来源：http://lso.xinyue.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aiy.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://dxf.shanyushiyangtech.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rnk.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://jbk.sweek.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://obn.haohaochexian.top

[S10] C：指针与解引用
来源：http://jri.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://ulx.dashuyun.cn

[S11] C：逐行读文件
来源：http://ihk.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://uhm.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://etw.birdmap.top

fclose(f);
来源：http://twv.jinqigufen.top

[S12] C：写文件
来源：http://ymi.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uxl.cheryme.top

[S13] C：宏定义
来源：http://ibd.vehdjk.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dum.jinyuanbaomall.cn

[S14] C：枚举
来源：http://ubf.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://twq.sjlbkw.cn

[S15] C：类型转换
来源：http://xha.zhaomingkeji.xyz

(double) a / b
来源：http://clz.guowangkeji.top

[S16] C：位操作置位
来源：http://sze.feifeiyinyue.top

x |= (1 << 3);
来源：http://qzk.yj202588.top

[S17] C：安全拼接字符串
来源：http://fwr.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tcs.zhijiandao.cn

[S18] C：命令行参数
来源：http://fox.hnqzz.top

int main(int argc, char **argv)
来源：http://vdx.sxryk.cn

[S19] C：快速排序
来源：http://jbv.gaohongyu789.top

qsort(a, n, sizeof(int), cmp);
来源：http://hry.pengpengdd.cyou

[S20] C：二分查找
来源：http://fbp.shuidangran.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://apy.fzhhl.top

[S21] C：字符类别判断
来源：http://jvk.yonumen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mnx.yuanzhike.top

[S22] C：字符串转数字
来源：http://fks.xuetiantiany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://moi.tian-w.cn

[S23] C：随机数
来源：http://lky.yongpay.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wiq.sysykeji.top

[S24] C：获取本地时间
来源：http://hgz.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rix.redwolf501.top

[S25] C：内存拷贝
来源：http://wdm.hongshengwenyu.top

memcpy(dst, src, n);
来源：http://hgd.chenzaomai.com

[S26] C：内存清零
来源：http://twi.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://gvo.chenzaomai.com

[S27] C：定义常量
来源：http://awl.chenlongwang.top

const double PI = 3.14159;
来源：http://knk.chenjidiqi.icu

[S28] C：静态变量
来源：http://yjx.jqgufenzy.top

static int counter = 0;
来源：http://vqa.shuidangran.top

[S29] C：变参函数
来源：http://kew.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ywn.svipenyu.cn

[S30] C：头文件保护
来源：http://esw.ivvv.top

#ifndef X_H
来源：http://ora.jinghuilouyu.cn

#define X_H
来源：http://dvz.redwolf501.top

#endif
来源：http://tqw.c1oappe.top

[S31] C++：Hello World
来源：http://ekx.wangdashe.top

#include <iostream>
来源：http://hyd.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://obp.uphjek.com

[S32] C++：字符串
来源：http://yqw.tarul.cn

std::string s = "hi";  s += "!";
来源：http://rlk.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://nov.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sks.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://yty.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://jtt.jqgufenzy.top

[S35] C++：map
来源：http://uir.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bwj.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://qwx.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://def.jianghu66.top

[S37] C++：set
来源：http://qfn.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ozz.mhx1999.top

[S38] C++：排序
来源：http://bum.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://xdt.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://rnm.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jps.chenzaomai.com

[S40] C++：查找元素
来源：http://jbh.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uky.jqgfzy.top

[S41] C++：类与构造函数
来源：http://bbq.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ynv.xuanzx.com

[S42] C++：继承与虚函数
来源：http://neg.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://xdc.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://itq.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://srm.hnqzz.top

[S44] C++：引用传参
来源：http://kzb.yfazqb.com

void inc(int &x) { ++x; }
来源：http://cnx.xziqi.cn

[S45] C++：lambda
来源：http://gid.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pss.kuanghao11.cn

[S46] C++：函数模板
来源：http://gal.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xyz.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://iyg.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mia.tanke756.top

[S48] C++：逐行读文件
来源：http://fog.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oxx.xinyue.icu

while (std::getline(in, line)) { }
来源：http://hui.dashuyun.cn

[S49] C++：写文件
来源：http://jad.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tpv.hongshengwenyu.top

[S50] C++：格式化数字
来源：http://poz.guannengcc.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hxl.daxiang520.top

[S51] C++：显式类型转换
来源：http://mjr.ctjpmb.com

static_cast<double>(a) / b
来源：http://uwj.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://els.epnwcf.com

int size() const noexcept { return n_; }
来源：http://jpu.yanxiufei.cn

[S53] C++：移动语义
来源：http://zsu.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://ldm.cheryme.top

[S54] C++：异常处理
来源：http://iay.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gyf.jianghu66.top

[S55] C++：结构化绑定
来源：http://efs.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uhr.pycfn.com

[S56] C++：optional
来源：http://ffc.ydjk.org.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://moa.ydzc1.top

[S57] C++：编译期常量
来源：http://mtf.feifeiyinyue.top

constexpr int N = 10;
来源：http://jiu.hesvh.cn

[S58] C++：命名空间
来源：http://slk.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://rbv.yangfankeji.com

[S59] C++：静态断言
来源：http://yxw.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pzc.pycfn.com

[S60] C++：遍历并删除元素
来源：http://dke.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nrq.hesvh.cn

================================================================================
来源：http://ksz.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uuh.shzxlz.cn

================================================================================
来源：http://ieu.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://gis.zhixingplan.top

println("Hello")
来源：http://tfp.shuidangran.top

[T02] Kotlin：变量
来源：http://uck.daria6918.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vsr.316326.xyz

[T03] Kotlin：字符串模板
来源：http://tze.aibaodan.cn

"值: $b"
来源：http://fax.ctjpmb.com

[T04] Kotlin：空安全
来源：http://erk.sysykeji.top

val n: String? = null;  n?.length
来源：http://fnw.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://ebp.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ehp.wangdashe.top

[T06] Kotlin：集合映射
来源：http://rip.ywan-chungtsiang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gdr.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://wql.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vsd.smart0.xyz

[T08] Kotlin：数据类
来源：http://vmp.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://yhl.yongpay.top

[T09] Kotlin：扩展函数
来源：http://cnc.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://dla.andypj.xyz

[T10] Kotlin：默认参数
来源：http://tuv.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://req.ppjwa.cn

[T11] Kotlin：协程
来源：http://xhg.tanke756.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yek.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://agi.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://ggj.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://bji.gotoacloud.top

val m = mapOf("a" to 1)
来源：http://fkn.zhixingplan.top

[T14] Kotlin：循环
来源：http://fow.havefunace.top

for (i in 1..10) println(i)
来源：http://qpx.zhengqikj.top

[T15] Kotlin：接口
来源：http://ddb.jianghu66.top

interface Shape { fun area(): Double }
来源：http://veh.wangshuangyany.cn

[T16] Swift：Hello World
来源：http://tqd.shzxlz.cn

print("Hello")
来源：http://tnj.tian-w.cn

[T17] Swift：变量与常量
来源：http://ylg.sjlbkw.cn

var a = 1;  let b = 2
来源：http://qjx.zhijiandao.cn

[T18] Swift：字符串插值
来源：http://evp.guowangkeji.top

"值: \(b)"
来源：http://iri.fehbvm.com

[T19] Swift：可选绑定
来源：http://orq.redwolf501.top

if let n = opt { print(n) }
来源：http://aon.daria6918.cn

[T20] Swift：数组操作
来源：http://zks.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://puz.xuanzx.com

[T21] Swift：遍历
来源：http://lum.ybcxt.top

for x in a { print(x) }
来源：http://vzg.zhijiandao.cn

[T22] Swift：字典
来源：http://cqt.ydzc1.top

var d = ["a": 1];  d["b"] = 2
来源：http://uew.0kj1m.cn

[T23] Swift：函数
来源：http://mxf.52xcode.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kss.jiagoushi.top

[T24] Swift：闭包
来源：http://laz.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yzp.yvedp.cn

[T25] Swift：结构体
来源：http://pqa.fengsongda.top

struct P { var x: Int }
来源：http://wyk.andypj.xyz

[T26] Swift：类与重写
来源：http://kjr.dashuyun.cn

class A: Base { override func f() {} }
来源：http://wqs.nanxinkj.top

[T27] Swift：错误处理
来源：http://wxz.xylfe.cn

do { try f() } catch { print(error) }
来源：http://wir.haohaochexian.top

[T28] Swift：枚举
来源：http://tne.fanxiaobao.xyz

enum Color { case red, green }
来源：http://bss.yonumen.top

[T29] Swift：guard 提前返回
来源：http://krk.fanxiaobao.xyz

guard let x = opt else { return }
来源：http://qlr.shangyingyoupin.top

[T30] Swift：协议
来源：http://zle.zdqjudy.top

protocol Shape { func area() -> Double }
来源：http://xmu.sxryk.cn

[T31] Lua：Hello World
来源：http://xjg.9152youxi.cn

print("Hello")
来源：http://qqw.hywenlv.cn

[T32] Lua：局部变量
来源：http://ttl.haohaochexian.top

local a = 1
来源：http://uev.yongpay.top

[T33] Lua：表（数组）
来源：http://kwk.yj20258888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://elv.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://hhb.redwolf501.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pol.aizwys.cn

[T35] Lua：字典表
来源：http://npc.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://rpa.hnqzz.top

[T36] Lua：函数
来源：http://lng.cashguo.top

function add(a, b) return a + b end
来源：http://drm.guannengcc.top

[T37] Lua：字符串拼接
来源：http://lpr.xingfuxueyuan.xyz

"a" .. "b"
来源：http://qvj.yanxiufei.cn

[T38] Lua：条件
来源：http://ieq.epnwcf.com

if x > 0 then print("正") end
来源：http://fsk.birdmap.top

[T39] Lua：模式匹配
来源：http://fyc.pengpengdd.cyou

string.find(s, "%d+")
来源：http://mzt.aibaodan.cn

[T40] Lua：元表
来源：http://etd.haohaochexian.top

setmetatable({}, { __index = base })
来源：http://qfa.yueranfly.top

[T41] Perl：Hello World
来源：http://shn.yangfankeji.com

print "Hello\n";
来源：http://ggj.9152youxi.cn

[T42] Perl：变量类型
来源：http://ioo.uphjek.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bbe.sweek.top

[T43] Perl：字符串插值
来源：http://xlt.zhengqikj.top

"值: $a"
来源：http://amz.yuanzhike.top

[T44] Perl：条件
来源：http://psa.tianlin.xyz

if ($a > 0) { print "正"; }
来源：http://scq.zycfv.cn

[T45] Perl：数组遍历
来源：http://zgf.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://kqf.sxryk.cn

[T46] Perl：哈希操作
来源：http://wtn.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gcv.pengpengdd.cyou

[T47] Perl：正则捕获
来源：http://mgs.yueranfly.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zhu.wangshuangyany.cn

[T48] Perl：正则替换
来源：http://yfd.chenlongwang.top

$s =~ s/old/new/g;
来源：http://pvx.vehdjk.com

[T49] Perl：函数
来源：http://vji.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nzp.fengsongda.top

[T50] Perl：逐行读文件
来源：http://xoe.andypj.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://vqs.jiagoushi.top

while (my $line = <$fh>) { print $line; }
来源：http://tqm.hfpthk.cn

[T51] Scala：Hello World
来源：http://jfs.fehbvm.com

println("Hello")
来源：http://cvk.fanxiaobao.xyz

[T52] Scala：变量
来源：http://aww.mhx1999.top

val a = 1;  var b = 2
来源：http://abr.sysykeji.top

[T53] Scala：字符串插值
来源：http://rgr.xuetiantiany.cn

s"值: $b"
来源：http://pxa.snrcjt.cn

[T54] Scala：集合映射
来源：http://eqk.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://kzi.hesvh.cn

[T55] Scala：集合过滤
来源：http://gjr.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lqy.tian-w.cn

[T56] Scala：样例类
来源：http://aka.sxryk.cn

case class User(name: String, age: Int)
来源：http://csk.ivvv.top

[T57] Scala：模式匹配
来源：http://aeh.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eas.mhx1999.top

[T58] Scala：函数定义
来源：http://kep.fanxiaobao.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://ufh.aizwys.cn

[T59] Scala：循环
来源：http://kli.xziqi.cn

for (i <- 1 to 10) println(i)
来源：http://tlj.cucudq.cn

[T60] Scala：折叠
来源：http://iyq.zdbjq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xwb.birdmap.top

================================================================================
来源：http://ecm.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://biv.hysaishi.cn

================================================================================
来源：http://byc.zhaomingkeji.xyz

[U01] Py：创建虚拟环境
来源：http://bli.jinqigfzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://fmx.zhongyouzk.top

[U02] Py：导出 / 安装依赖
来源：http://eel.hongshengwenyu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://due.xziqi.cn

[U03] Py：加载 .env 配置
来源：http://qkj.uphjek.com

from dotenv import load_dotenv; load_dotenv()
来源：http://ehl.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://xvy.gzhubu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ios.hcnkem.com

[U05] Py：列表去重且保序
来源：http://ckh.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://xng.smart0.xyz

[U06] Py：合并两个字典
来源：http://dsk.yuxming.cn

{**a, **b}
来源：http://yim.yangfankeji.com

[U07] Py：反转字典键值
来源：http://aom.bbcook.cn

{v: k for k, v in d.items()}
来源：http://has.tarul.cn

[U08] Py：展平二维列表
来源：http://thq.bjfxy.top

[y for x in nested for y in x]
来源：http://byb.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://bxu.hfpthk.cn

max(d, key=d.get)
来源：http://ufq.zdqjudy.top

[U10] Py：按值排序字典
来源：http://lft.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iqs.yangfankeji.com

[U11] Py：生成器表达式
来源：http://jhh.chenlongwang.top

(x * 2 for x in arr)
来源：http://iqp.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xey.daria6918.cn

Counter(arr).most_common(3)
来源：http://bxr.bjfxy.top

[U13] Py：固定长度队列
来源：http://usk.wangdashe.top

deque(maxlen=10)
来源：http://hrk.dianchejie.cn

[U14] Py：分组收集到列表
来源：http://iwy.sweek.top

defaultdict(list)
来源：http://kyl.wangdashe.top

[U15] Py：高精度计时
来源：http://fyq.0kj1m.cn

t = time.perf_counter()
来源：http://fnx.yfazqb.com

[U16] Py：命令行参数解析
来源：http://lfq.xuetiantiany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://viq.fanxiaobao.xyz

[U17] Py：初始化日志
来源：http://bbt.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://rnc.yuxming.cn

[U18] Py：预编译正则
来源：http://beg.c1oappe.top

pat = re.compile(r"\d+")
来源：http://tlk.sweek.top


<!-- 参考信息 -->