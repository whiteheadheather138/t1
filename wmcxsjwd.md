代发 wailian999

read -rp "请输入: " ans
来源：http://pnx.fanxiaobao.xyz

[R78] 交互式菜单
来源：http://maw.yonumen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yuw.xingfuxueyuan.xyz

[R79] 解析命令行选项
来源：http://ham.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://akk.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://fph.c1oappe.top

time ./run.sh
来源：http://vog.shzxlz.cn

================================================================================
来源：http://jsr.nanxuanxn.top

S. C / C++ 专题
来源：http://xwn.ivvv.top

================================================================================
来源：http://dgr.hfpthk.cn

[S01] C：Hello World
来源：http://cqu.jlsjyb.cn

#include <stdio.h>
来源：http://fjp.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hju.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://wrk.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://cof.hysaishi.cn

[S03] C：读入整数
来源：http://pwi.pycfn.com

int x; scanf("%d", &x);
来源：http://wgf.vqdsnc.cn

[S04] C：字符串复制
来源：http://hbk.daxiang520.top

char dst[32]; strcpy(dst, "hi");
来源：http://swm.epnwcf.com

[S05] C：字符串长度
来源：http://hix.pengpengdd.cyou

strlen(s)
来源：http://kiz.yonumen.top

[S06] C：字符串比较
来源：http://uyi.nwbrower.top

strcmp(a, b) == 0
来源：http://pbi.birdmap.top

[S07] C：数组遍历求和
来源：http://gzv.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xaw.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://wtl.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uhg.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://ldi.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pnw.xylfe.cn

[S10] C：指针与解引用
来源：http://wos.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://hwl.cucudq.cn

[S11] C：逐行读文件
来源：http://rqe.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://hms.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://hde.hnxiangtu.top

fclose(f);
来源：http://btn.jianghu66.top

[S12] C：写文件
来源：http://hrp.yanxiufei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://abp.tanke756.top

[S13] C：宏定义
来源：http://ghm.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qpr.sufxvd.cn

[S14] C：枚举
来源：http://abc.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://ldq.zhijiandao.cn

[S15] C：类型转换
来源：http://krj.nwbrower.top

(double) a / b
来源：http://nix.ivvv.top

[S16] C：位操作置位
来源：http://wff.hfpthk.cn

x |= (1 << 3);
来源：http://gwe.guannengcc.top

[S17] C：安全拼接字符串
来源：http://wvf.nanxinkj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wug.tianlin.xyz

[S18] C：命令行参数
来源：http://rrr.fehbvm.com

int main(int argc, char **argv)
来源：http://ozg.cdnleiting.top

[S19] C：快速排序
来源：http://lit.sjlbkw.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rrp.pengpengdd.cyou

[S20] C：二分查找
来源：http://sct.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lms.hcnkem.com

[S21] C：字符类别判断
来源：http://hfu.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ewb.dashuyun.cn

[S22] C：字符串转数字
来源：http://kfn.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://nrg.hnxiangtu.top

[S23] C：随机数
来源：http://rbg.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://plh.aizwys.cn

[S24] C：获取本地时间
来源：http://bre.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qlr.xylfe.cn

[S25] C：内存拷贝
来源：http://sli.gotoacloud.top

memcpy(dst, src, n);
来源：http://ajo.hesvh.cn

[S26] C：内存清零
来源：http://aiy.hammf.cn

memset(a, 0, sizeof a);
来源：http://xii.ivvv.top

[S27] C：定义常量
来源：http://qhg.fengsongda.top

const double PI = 3.14159;
来源：http://owd.xingfuxueyuan.xyz

[S28] C：静态变量
来源：http://rdd.redwolf501.top

static int counter = 0;
来源：http://scx.vqdsnc.cn

[S29] C：变参函数
来源：http://qeu.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ijf.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://bps.hcnkem.com

#ifndef X_H
来源：http://cpn.uphjek.com

#define X_H
来源：http://gea.gotoacloud.top

#endif
来源：http://rwe.hcnkem.com

[S31] C++：Hello World
来源：http://jzn.tarul.cn

#include <iostream>
来源：http://jqy.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://wcf.hywenlv.cn

[S32] C++：字符串
来源：http://gir.sxryk.cn

std::string s = "hi";  s += "!";
来源：http://xgu.shuidangran.top

[S33] C++：vector 增删
来源：http://ran.zhongyouzk.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eyv.ybcxt.top

[S34] C++：遍历 vector
来源：http://lqk.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://res.pengpengdd.cyou

[S35] C++：map
来源：http://bih.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ufr.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://dhq.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ges.ctjpmb.com

[S37] C++：set
来源：http://nqw.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ymc.vehdjk.com

[S38] C++：排序
来源：http://tsp.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://lkr.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://vng.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://are.ybcxt.top

[S40] C++：查找元素
来源：http://vkb.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://orc.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://zpf.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uqx.aizwys.cn

[S42] C++：继承与虚函数
来源：http://pjd.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://yoe.cdnleiting.top

[S43] C++：智能指针
来源：http://nbb.yueranfly.top

auto p = std::make_unique<int>(5);
来源：http://qev.bjfxy.top

[S44] C++：引用传参
来源：http://jkw.pengpengdd.cyou

void inc(int &x) { ++x; }
来源：http://uoz.jiagoushi.top

[S45] C++：lambda
来源：http://mdp.yuxming.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sna.meibo888.top

[S46] C++：函数模板
来源：http://sbl.yangfankeji.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wnb.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://uda.hongshengwenyu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://haf.xziqi.cn

[S48] C++：逐行读文件
来源：http://tqg.wangdashe.top

std::ifstream in("a.txt");  std::string line;
来源：http://mfn.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://ttf.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://jwy.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ffq.cdnleiting.top

[S50] C++：格式化数字
来源：http://ggu.feifeiyinyue.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jxf.hnqzz.top

[S51] C++：显式类型转换
来源：http://ika.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://igy.yj20258.top

[S52] C++：const 与 noexcept
来源：http://eev.dashuyun.cn

int size() const noexcept { return n_; }
来源：http://vfi.zdqjudy.top

[S53] C++：移动语义
来源：http://dxm.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://ozu.fengsongda.top

[S54] C++：异常处理
来源：http://jup.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gjb.tian-w.cn

[S55] C++：结构化绑定
来源：http://tsq.jiagoushi.top

auto [a, b] = std::make_pair(1, 2);
来源：http://iir.dianchejie.cn

[S56] C++：optional
来源：http://snp.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://goh.yj202588.top

[S57] C++：编译期常量
来源：http://tml.jqgfzy.top

constexpr int N = 10;
来源：http://suz.chenlongwang.top

[S58] C++：命名空间
来源：http://moy.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://utc.cucudq.cn

[S59] C++：静态断言
来源：http://dnf.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uvp.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://rlp.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://drw.dashuyun.cn

================================================================================
来源：http://rwn.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cfp.zdqjudy.top

================================================================================
来源：http://rjm.xinyue.icu

[T01] Kotlin：Hello World
来源：http://wwt.dianchejie.cn

println("Hello")
来源：http://war.jinqigfzy.top

[T02] Kotlin：变量
来源：http://xld.tianlin.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://olg.9152youxi.cn

[T03] Kotlin：字符串模板
来源：http://zwa.hongshengwenyu.top

"值: $b"
来源：http://pni.hfpthk.cn

[T04] Kotlin：空安全
来源：http://cmp.aizwys.cn

val n: String? = null;  n?.length
来源：http://hld.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://jvb.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://for.fanxiaobao.xyz

[T06] Kotlin：集合映射
来源：http://cyx.316326.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://fup.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://wbr.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lhb.yuxming.cn

[T08] Kotlin：数据类
来源：http://sks.tianlin.xyz

data class User(val name: String, val age: Int)
来源：http://qbo.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://lrq.daria6918.cn

fun String.exclaim() = this + "!"
来源：http://ytf.hammf.cn

[T10] Kotlin：默认参数
来源：http://bbr.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://txx.aizwys.cn

[T11] Kotlin：协程
来源：http://jqe.xuanzx.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://xep.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://cnm.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://rwk.kuanghao11.cn

[T13] Kotlin：只读 Map
来源：http://xzg.epnwcf.com

val m = mapOf("a" to 1)
来源：http://ygm.gotoacloud.top

[T14] Kotlin：循环
来源：http://jrl.0kj1m.cn

for (i in 1..10) println(i)
来源：http://hic.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://ned.daria6918.cn

interface Shape { fun area(): Double }
来源：http://ugv.andypj.xyz

[T16] Swift：Hello World
来源：http://yhs.ctjpmb.com

print("Hello")
来源：http://kpg.aibaodan.cn

[T17] Swift：变量与常量
来源：http://hgx.ehwqpu.com

var a = 1;  let b = 2
来源：http://oft.tianlin.xyz

[T18] Swift：字符串插值
来源：http://zrd.wangdashe.top

"值: \(b)"
来源：http://rkm.pycfn.com

[T19] Swift：可选绑定
来源：http://iot.zdqjudy.top

if let n = opt { print(n) }
来源：http://tyc.yj20258888.top

[T20] Swift：数组操作
来源：http://aeq.chenzaomai.com

var a = [1, 2, 3];  a.append(4)
来源：http://vmk.vehdjk.com

[T21] Swift：遍历
来源：http://tpc.ehwqpu.com

for x in a { print(x) }
来源：http://vww.chenzaomai.com

[T22] Swift：字典
来源：http://ciy.yueranfly.top

var d = ["a": 1];  d["b"] = 2
来源：http://ruj.hammf.cn

[T23] Swift：函数
来源：http://xyd.fzhhl.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yyt.havefunace.top

[T24] Swift：闭包
来源：http://nay.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pqx.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://bwb.9152youxi.cn

struct P { var x: Int }
来源：http://ncx.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://zmn.guowangkeji.top

class A: Base { override func f() {} }
来源：http://xaf.zhoulong.xyz

[T27] Swift：错误处理
来源：http://lkm.nanxinkj.top

do { try f() } catch { print(error) }
来源：http://joo.daxiang520.top

[T28] Swift：枚举
来源：http://kno.aibaodan.cn

enum Color { case red, green }
来源：http://mbm.redwolf501.top

[T29] Swift：guard 提前返回
来源：http://bhb.hongshengwenyu.top

guard let x = opt else { return }
来源：http://asb.redwolf501.top

[T30] Swift：协议
来源：http://uuc.cqqwz.cn

protocol Shape { func area() -> Double }
来源：http://rju.jqgufenzy.top

[T31] Lua：Hello World
来源：http://yul.guowangkeji.top

print("Hello")
来源：http://gfp.chenlongwang.top

[T32] Lua：局部变量
来源：http://ysy.yj202588.top

local a = 1
来源：http://jqz.nanxinkj.top

[T33] Lua：表（数组）
来源：http://vmt.fzhhl.top

local t = {1, 2, 3};  t[4] = 4
来源：http://chy.yvedp.cn

[T34] Lua：遍历表
来源：http://mpw.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qxt.havefunace.top

[T35] Lua：字典表
来源：http://mcu.daria6918.cn

local d = { a = 1 };  d.b = 2
来源：http://haj.haohaochexian.top

[T36] Lua：函数
来源：http://syt.cashguo.top

function add(a, b) return a + b end
来源：http://xij.tanke756.top

[T37] Lua：字符串拼接
来源：http://otc.cashguo.top

"a" .. "b"
来源：http://wfo.fanxiaobao.xyz

[T38] Lua：条件
来源：http://lra.gzhubu.top

if x > 0 then print("正") end
来源：http://fiv.tianlin.xyz

[T39] Lua：模式匹配
来源：http://xkl.andypj.xyz

string.find(s, "%d+")
来源：http://jbl.gotoacloud.top

[T40] Lua：元表
来源：http://qsx.fengsongda.top

setmetatable({}, { __index = base })
来源：http://def.guowangkeji.top

[T41] Perl：Hello World
来源：http://zog.shzxlz.cn

print "Hello\n";
来源：http://gbm.daxiang520.top

[T42] Perl：变量类型
来源：http://ktd.fehbvm.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tcq.dianchejie.cn

[T43] Perl：字符串插值
来源：http://zas.fengsongda.top

"值: $a"
来源：http://ypc.fktsv.cn

[T44] Perl：条件
来源：http://ybe.zycfv.cn

if ($a > 0) { print "正"; }
来源：http://iah.chenzaomai.com

[T45] Perl：数组遍历
来源：http://epz.zdqjudy.top

for my $x (@arr) { print $x; }
来源：http://csq.ivvv.top

[T46] Perl：哈希操作
来源：http://tht.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ieu.yj20258888.top

[T47] Perl：正则捕获
来源：http://liv.ivvv.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://oua.meibo888.top

[T48] Perl：正则替换
来源：http://qjy.yongpay.top

$s =~ s/old/new/g;
来源：http://opd.nanxuanxn.top

[T49] Perl：函数
来源：http://tti.fktsv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xmt.haohaochexian.top

[T50] Perl：逐行读文件
来源：http://oao.gogol.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://onb.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://oge.ehwqpu.com

[T51] Scala：Hello World
来源：http://kdr.hywenlv.cn

println("Hello")
来源：http://asi.cqqwz.cn

[T52] Scala：变量
来源：http://rux.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://dmx.shanyushiyangkeji.top

[T53] Scala：字符串插值
来源：http://xcq.cdnleiting.top

s"值: $b"
来源：http://vsf.birdmap.top

[T54] Scala：集合映射
来源：http://uan.uphjek.com

List(1, 2, 3).map(_ * 2)
来源：http://cny.jqgfzy.top

[T55] Scala：集合过滤
来源：http://idr.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://ylu.quarkkingdee.top

[T56] Scala：样例类
来源：http://yzg.fktsv.cn

case class User(name: String, age: Int)
来源：http://lcs.ppjwa.cn

[T57] Scala：模式匹配
来源：http://cpo.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://wfz.cqqwz.cn

[T58] Scala：函数定义
来源：http://zek.birdmap.top

def add(a: Int, b: Int): Int = a + b
来源：http://dwe.vqdsnc.cn

[T59] Scala：循环
来源：http://lwn.jqgufenzy.top

for (i <- 1 to 10) println(i)
来源：http://tny.wangshuangyany.cn

[T60] Scala：折叠
来源：http://fhk.nwbrower.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nev.chenjidiqi.icu

================================================================================
来源：http://usi.sufxvd.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hir.hongshengwenyu.top

================================================================================
来源：http://edl.ydjk.org.cn

[U01] Py：创建虚拟环境
来源：http://kqn.yuanzhike.top

python -m venv .venv && source .venv/bin/activate
来源：http://aqv.xuetiantiany.cn

[U02] Py：导出 / 安装依赖
来源：http://vfq.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://brb.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://mkn.chenjidiqi.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://vtk.xuetiantiany.cn

[U04] Py：变量调试打印
来源：http://dnm.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kfn.yongpay.top

[U05] Py：列表去重且保序
来源：http://usl.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://uiq.bjfxy.top

[U06] Py：合并两个字典
来源：http://enc.yuxming.cn

{**a, **b}
来源：http://rxl.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://fcu.gzhubu.top

{v: k for k, v in d.items()}
来源：http://jwv.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://woi.snrcjt.cn

[y for x in nested for y in x]
来源：http://zqm.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://anj.jlsjyb.cn

max(d, key=d.get)
来源：http://lzp.dianchejie.cn

[U10] Py：按值排序字典
来源：http://jbh.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://znl.shzxlz.cn

[U11] Py：生成器表达式
来源：http://tnf.chenzaomai.com

(x * 2 for x in arr)
来源：http://rkp.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sqc.yongpay.top

Counter(arr).most_common(3)
来源：http://vrs.ydzc1.top

[U13] Py：固定长度队列
来源：http://tnz.316326.xyz

deque(maxlen=10)
来源：http://ouq.smart0.xyz

[U14] Py：分组收集到列表
来源：http://ena.sxryk.cn

defaultdict(list)
来源：http://mun.ybcxt.top

[U15] Py：高精度计时
来源：http://ckk.cheryme.top

t = time.perf_counter()
来源：http://quo.jlsjyb.cn

[U16] Py：命令行参数解析
来源：http://xii.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rtw.vehdjk.com

[U17] Py：初始化日志
来源：http://bgn.haohaochexian.top

logging.basicConfig(level=logging.INFO)
来源：http://lvh.c1oappe.top

[U18] Py：预编译正则
来源：http://zdb.zdqjudy.top

pat = re.compile(r"\d+")
来源：http://gkg.nwbrower.top


<!-- 参考信息 -->