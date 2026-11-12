代发 wailian999

read -rp "请输入: " ans
来源：http://ftn.zhoulong.xyz

[R78] 交互式菜单
来源：http://rio.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vhr.jinqigufen.top

[R79] 解析命令行选项
来源：http://jvt.zhiwuduotai.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qho.cheryme.top

[R80] 查看脚本执行耗时
来源：http://der.havefunace.top

time ./run.sh
来源：http://thk.andypj.xyz

================================================================================
来源：http://qji.jiagoushi.top

S. C / C++ 专题
来源：http://bct.tian-w.cn

================================================================================
来源：http://dfi.shuidangran.top

[S01] C：Hello World
来源：http://kop.hongshengwenyu.top

#include <stdio.h>
来源：http://ngd.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qdo.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://uxz.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://bqw.nwbrower.top

[S03] C：读入整数
来源：http://wdq.sxryk.cn

int x; scanf("%d", &x);
来源：http://xqq.0kj1m.cn

[S04] C：字符串复制
来源：http://rmf.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hse.cdnleiting.top

[S05] C：字符串长度
来源：http://sjo.cqqwz.cn

strlen(s)
来源：http://jua.dianchejie.cn

[S06] C：字符串比较
来源：http://ypz.nanxinkj.top

strcmp(a, b) == 0
来源：http://vuz.316326.xyz

[S07] C：数组遍历求和
来源：http://cly.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ihh.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://kwm.fengsongda.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ygs.yangfankeji.com

[S09] C：结构体定义与初始化
来源：http://ylj.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://muv.cheryme.top

[S10] C：指针与解引用
来源：http://bcw.bjfxy.top

int *p = &a;  *p = 5;
来源：http://ynb.chenzaomai.com

[S11] C：逐行读文件
来源：http://irj.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "r");
来源：http://kfb.zycfv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pxn.feifeiyinyue.top

fclose(f);
来源：http://blu.hnqzz.top

[S12] C：写文件
来源：http://szx.yuxming.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mna.zhongyouzk.top

[S13] C：宏定义
来源：http://tzg.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lxr.cqqwz.cn

[S14] C：枚举
来源：http://avu.yj202588.top

enum Color { RED, GREEN, BLUE };
来源：http://nzb.dianchejie.cn

[S15] C：类型转换
来源：http://cxu.hesvh.cn

(double) a / b
来源：http://ntb.ybcxt.top

[S16] C：位操作置位
来源：http://dwm.feifeiyinyue.top

x |= (1 << 3);
来源：http://cbm.havefunace.top

[S17] C：安全拼接字符串
来源：http://oeh.birdmap.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nfh.daxiang520.top

[S18] C：命令行参数
来源：http://ovf.hnqzz.top

int main(int argc, char **argv)
来源：http://ctw.ivvv.top

[S19] C：快速排序
来源：http://ftz.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://edg.hywenlv.cn

[S20] C：二分查找
来源：http://jcy.yuxming.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yuv.fzhhl.top

[S21] C：字符类别判断
来源：http://anq.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://twa.cheryme.top

[S22] C：字符串转数字
来源：http://iwn.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kim.hywenlv.cn

[S23] C：随机数
来源：http://klq.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xfl.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://gbm.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fdx.ivvv.top

[S25] C：内存拷贝
来源：http://qlw.zhaomingkeji.xyz

memcpy(dst, src, n);
来源：http://tgg.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://djp.yueranfly.top

memset(a, 0, sizeof a);
来源：http://iky.ydzc1.top

[S27] C：定义常量
来源：http://zgk.yangfankeji.com

const double PI = 3.14159;
来源：http://tnk.ppjwa.cn

[S28] C：静态变量
来源：http://khj.kuanghao11.cn

static int counter = 0;
来源：http://ajm.tian-w.cn

[S29] C：变参函数
来源：http://cie.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tls.vehdjk.com

[S30] C：头文件保护
来源：http://fnt.fehbvm.com

#ifndef X_H
来源：http://xgz.jqgfzy.top

#define X_H
来源：http://vhj.havefunace.top

#endif
来源：http://vgr.ppjwa.cn

[S31] C++：Hello World
来源：http://bav.kuanghao11.cn

#include <iostream>
来源：http://hii.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://ajn.guannengcc.top

[S32] C++：字符串
来源：http://mpm.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://hds.fktsv.cn

[S33] C++：vector 增删
来源：http://inq.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nxu.jianghu66.top

[S34] C++：遍历 vector
来源：http://rgh.yj20258.top

for (auto &x : v) { std::cout << x; }
来源：http://jvs.quarkkingdee.top

[S35] C++：map
来源：http://wxm.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bno.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://ryg.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sid.iojbl.cn

[S37] C++：set
来源：http://bvn.fehbvm.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://adg.sjlbkw.cn

[S38] C++：排序
来源：http://pnz.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://dwt.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://cqk.ydzc1.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uka.zdbjq.cn

[S40] C++：查找元素
来源：http://fkr.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jwn.yongpay.top

[S41] C++：类与构造函数
来源：http://txv.epnwcf.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cvz.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://vzx.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://erz.bbcook.cn

[S43] C++：智能指针
来源：http://jpa.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://vdu.sjlbkw.cn

[S44] C++：引用传参
来源：http://oqq.feifeiyinyue.top

void inc(int &x) { ++x; }
来源：http://kmu.hongshengwenyu.top

[S45] C++：lambda
来源：http://kaf.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yxf.jinghuilouyu.cn

[S46] C++：函数模板
来源：http://zxs.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ohe.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://gox.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hrh.sweek.top

[S48] C++：逐行读文件
来源：http://cmu.chenlongwang.top

std::ifstream in("a.txt");  std::string line;
来源：http://rvu.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://wid.shangyingyoupin.top

[S49] C++：写文件
来源：http://evj.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ujc.redwolf501.top

[S50] C++：格式化数字
来源：http://wrd.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bkq.chenjidiqi.icu

[S51] C++：显式类型转换
来源：http://nik.jiagoushi.top

static_cast<double>(a) / b
来源：http://tll.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://szr.yj202588.top

int size() const noexcept { return n_; }
来源：http://hjd.pycfn.com

[S53] C++：移动语义
来源：http://whq.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://irv.fzhhl.top

[S54] C++：异常处理
来源：http://hft.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qmr.cdnleiting.top

[S55] C++：结构化绑定
来源：http://pvg.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eqp.cheryme.top

[S56] C++：optional
来源：http://utl.hnqzz.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xil.jinqigufen.top

[S57] C++：编译期常量
来源：http://wha.sxryk.cn

constexpr int N = 10;
来源：http://hpc.jqgfzy.top

[S58] C++：命名空间
来源：http://wze.kuanghao11.cn

namespace ns { int f() { return 1; } }
来源：http://hjz.zhijiandao.cn

[S59] C++：静态断言
来源：http://zag.yfazqb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wss.haohaochexian.top

[S60] C++：遍历并删除元素
来源：http://jwp.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://opx.jianghu66.top

================================================================================
来源：http://gjt.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nnw.chenjidiqi.icu

================================================================================
来源：http://ohz.bjfxy.top

[T01] Kotlin：Hello World
来源：http://wdq.fzhhl.top

println("Hello")
来源：http://fhv.cucudq.cn

[T02] Kotlin：变量
来源：http://hzk.daria6918.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ics.bbcook.cn

[T03] Kotlin：字符串模板
来源：http://wft.chenjidiqi.icu

"值: $b"
来源：http://upr.birdmap.top

[T04] Kotlin：空安全
来源：http://hyf.vehdjk.com

val n: String? = null;  n?.length
来源：http://ekq.epnwcf.com

[T05] Kotlin：when 表达式
来源：http://gbs.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://llu.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://erj.redwolf501.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cjg.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://nzg.jqgufenzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lnj.ctjpmb.com

[T08] Kotlin：数据类
来源：http://ysh.zhaomingkeji.xyz

data class User(val name: String, val age: Int)
来源：http://ljh.ywan-chungtsiang.top

[T09] Kotlin：扩展函数
来源：http://qkj.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://ztp.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://bqs.hysaishi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rcr.jiagoushi.top

[T11] Kotlin：协程
来源：http://ivn.hongshengwenyu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ocp.yongpay.top

[T12] Kotlin：解构声明
来源：http://gmb.hfpthk.cn

val (a, b) = Pair(1, 2)
来源：http://jmy.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://igt.jqgfzy.top

val m = mapOf("a" to 1)
来源：http://hjk.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://oma.snrcjt.cn

for (i in 1..10) println(i)
来源：http://uom.cheryme.top

[T15] Kotlin：接口
来源：http://sbb.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://osn.sxryk.cn

[T16] Swift：Hello World
来源：http://xbm.guowangkeji.top

print("Hello")
来源：http://xas.xylfe.cn

[T17] Swift：变量与常量
来源：http://tzz.pycfn.com

var a = 1;  let b = 2
来源：http://pbc.hnqzz.top

[T18] Swift：字符串插值
来源：http://kds.zhijiandao.cn

"值: \(b)"
来源：http://cem.zhiwuduotai.top

[T19] Swift：可选绑定
来源：http://ruc.yj20258888.top

if let n = opt { print(n) }
来源：http://omp.yfazqb.com

[T20] Swift：数组操作
来源：http://uai.ctjpmb.com

var a = [1, 2, 3];  a.append(4)
来源：http://syo.aizwys.cn

[T21] Swift：遍历
来源：http://wqu.yuanzhike.top

for x in a { print(x) }
来源：http://vgx.ppjwa.cn

[T22] Swift：字典
来源：http://hpe.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://hfr.chenlongwang.top

[T23] Swift：函数
来源：http://ndd.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iam.316326.xyz

[T24] Swift：闭包
来源：http://wcw.meibo888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://iqg.hesvh.cn

[T25] Swift：结构体
来源：http://ula.gzhubu.top

struct P { var x: Int }
来源：http://res.xylfe.cn

[T26] Swift：类与重写
来源：http://raj.yfazqb.com

class A: Base { override func f() {} }
来源：http://atw.xziqi.cn

[T27] Swift：错误处理
来源：http://vtq.daria6918.cn

do { try f() } catch { print(error) }
来源：http://ikj.fzhhl.top

[T28] Swift：枚举
来源：http://xgv.zhiwuduotai.top

enum Color { case red, green }
来源：http://dcq.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://lgr.yonumen.top

guard let x = opt else { return }
来源：http://nks.ybcxt.top

[T30] Swift：协议
来源：http://ydv.aibaodan.cn

protocol Shape { func area() -> Double }
来源：http://eol.yonumen.top

[T31] Lua：Hello World
来源：http://qyb.tarul.cn

print("Hello")
来源：http://vwi.quarkkingdee.top

[T32] Lua：局部变量
来源：http://dmm.sjlbkw.cn

local a = 1
来源：http://sas.aibaodan.cn

[T33] Lua：表（数组）
来源：http://isr.fzhhl.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tvy.hnxiangtu.top

[T34] Lua：遍历表
来源：http://izd.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bfc.yuanzhike.top

[T35] Lua：字典表
来源：http://pmb.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://lfq.svipenyu.cn

[T36] Lua：函数
来源：http://nsz.daria6918.cn

function add(a, b) return a + b end
来源：http://gws.tanke756.top

[T37] Lua：字符串拼接
来源：http://mbc.c1oappe.top

"a" .. "b"
来源：http://opm.zdqjudy.top

[T38] Lua：条件
来源：http://cso.gotoacloud.top

if x > 0 then print("正") end
来源：http://hrq.xuanzx.com

[T39] Lua：模式匹配
来源：http://rqh.tarul.cn

string.find(s, "%d+")
来源：http://fro.cashguo.top

[T40] Lua：元表
来源：http://zbc.quarkkingdee.top

setmetatable({}, { __index = base })
来源：http://qla.jlsjyb.cn

[T41] Perl：Hello World
来源：http://kry.sweek.top

print "Hello\n";
来源：http://ddn.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://aan.uphjek.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ovg.yj20258.top

[T43] Perl：字符串插值
来源：http://tpa.jinqigfzy.top

"值: $a"
来源：http://bvz.pycfn.com

[T44] Perl：条件
来源：http://fpo.cashguo.top

if ($a > 0) { print "正"; }
来源：http://gcx.yvedp.cn

[T45] Perl：数组遍历
来源：http://qhh.vqdsnc.cn

for my $x (@arr) { print $x; }
来源：http://lkb.wangshuangyany.cn

[T46] Perl：哈希操作
来源：http://bxx.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mpg.316326.xyz

[T47] Perl：正则捕获
来源：http://yrt.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fzi.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://ueq.zhiwuduotai.top

$s =~ s/old/new/g;
来源：http://rff.shzxlz.cn

[T49] Perl：函数
来源：http://bpc.zhijiandao.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cvr.ydzc1.top

[T50] Perl：逐行读文件
来源：http://sik.fengsongda.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jya.sysykeji.top

while (my $line = <$fh>) { print $line; }
来源：http://bjf.zdqjudy.top

[T51] Scala：Hello World
来源：http://sjf.guannengcc.top

println("Hello")
来源：http://pxm.yuxming.cn

[T52] Scala：变量
来源：http://yxs.tanke756.top

val a = 1;  var b = 2
来源：http://vap.yanxiufei.cn

[T53] Scala：字符串插值
来源：http://uzm.xinyue.icu

s"值: $b"
来源：http://pxn.pengpengdd.cyou

[T54] Scala：集合映射
来源：http://dvh.haohaochexian.top

List(1, 2, 3).map(_ * 2)
来源：http://ini.ydzc1.top

[T55] Scala：集合过滤
来源：http://chk.gotoacloud.top

List(1, 2, 3).filter(_ > 1)
来源：http://ffz.yueranfly.top

[T56] Scala：样例类
来源：http://lpj.xuetiantiany.cn

case class User(name: String, age: Int)
来源：http://kyh.0kj1m.cn

[T57] Scala：模式匹配
来源：http://crn.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://six.yanxiufei.cn

[T58] Scala：函数定义
来源：http://rzm.shuidangran.top

def add(a: Int, b: Int): Int = a + b
来源：http://btu.zhijiandao.cn

[T59] Scala：循环
来源：http://hxx.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://okr.fktsv.cn

[T60] Scala：折叠
来源：http://vdy.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rgd.sjlbkw.cn

================================================================================
来源：http://ayf.guowangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iqc.guowangkeji.top

================================================================================
来源：http://vrh.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://rtx.gotoacloud.top

python -m venv .venv && source .venv/bin/activate
来源：http://bcq.52xcode.cn

[U02] Py：导出 / 安装依赖
来源：http://nhu.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qbo.zycfv.cn

[U03] Py：加载 .env 配置
来源：http://nro.bjfxy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fjh.hysaishi.cn

[U04] Py：变量调试打印
来源：http://cit.ydzc1.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ohk.haohaochexian.top

[U05] Py：列表去重且保序
来源：http://ypg.havefunace.top

list(dict.fromkeys(arr))
来源：http://xso.dashuyun.cn

[U06] Py：合并两个字典
来源：http://mcf.jiagoushi.top

{**a, **b}
来源：http://rlq.yj20258.top

[U07] Py：反转字典键值
来源：http://bdw.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://cfv.sysykeji.top

[U08] Py：展平二维列表
来源：http://way.iojbl.cn

[y for x in nested for y in x]
来源：http://iiz.yj20258888.top

[U09] Py：字典取最大值的键
来源：http://pok.shangyingyoupin.top

max(d, key=d.get)
来源：http://ahj.bjfxy.top

[U10] Py：按值排序字典
来源：http://zwq.jinghuilouyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://unh.gaohongyu789.top

[U11] Py：生成器表达式
来源：http://sgi.yuanzhike.top

(x * 2 for x in arr)
来源：http://mde.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hof.fengsongda.top

Counter(arr).most_common(3)
来源：http://kmt.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://axn.ydjk.org.cn

deque(maxlen=10)
来源：http://ldw.nanxuanxn.top

[U14] Py：分组收集到列表
来源：http://faf.zdbjq.cn

defaultdict(list)
来源：http://les.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://kqt.hywenlv.cn

t = time.perf_counter()
来源：http://wxk.shzxlz.cn

[U16] Py：命令行参数解析
来源：http://jgk.epnwcf.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xra.xuanzx.com

[U17] Py：初始化日志
来源：http://jqj.hywenlv.cn

logging.basicConfig(level=logging.INFO)
来源：http://ana.gaohongyu789.top

[U18] Py：预编译正则
来源：http://fqp.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://rhv.zdbjq.cn


<!-- 参考信息 -->