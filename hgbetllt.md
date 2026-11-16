代发 wailian999

openssl rand -hex 16
来源：http://xho.pycfn.com

[R68] 计算文件校验值
来源：http://pcn.tianlin.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://yon.zhoulong.xyz

[R69] 生成随机密码
来源：http://ihg.ctjpmb.com

head -c 16 /dev/urandom | base64
来源：http://xjk.gaohongyu789.top

[R70] 时间戳与互转
来源：http://hyy.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://afe.cdnleiting.top

[R71] 日期格式化
来源：http://pvu.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://opu.svipenyu.cn

[R72] 等待端口就绪
来源：http://jpk.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fzy.iojbl.cn

[R73] 分割大日志
来源：http://seu.yvedp.cn

split -l 1000 big.log part_
来源：http://qrm.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://ffe.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qkm.xuanzx.com

[R75] 导出环境变量
来源：http://qhv.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://aki.yuxming.cn

[R76] 使用临时文件
来源：http://ozh.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vfu.svipenyu.cn

[R77] 读取用户输入
来源：http://vdo.jinqigufen.top

read -rp "请输入: " ans
来源：http://esp.gzhubu.top

[R78] 交互式菜单
来源：http://zvl.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://zlf.hysaishi.cn

[R79] 解析命令行选项
来源：http://xxa.xuetiantiany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lqf.xingfuxueyuan.xyz

[R80] 查看脚本执行耗时
来源：http://uyr.gaohongyu789.top

time ./run.sh
来源：http://mdl.pycfn.com

================================================================================
来源：http://lfq.gotoacloud.top

S. C / C++ 专题
来源：http://dxt.jinqigfzy.top

================================================================================
来源：http://vwd.shangyingyoupin.top

[S01] C：Hello World
来源：http://hji.dashuyun.cn

#include <stdio.h>
来源：http://kvb.hongshengwenyu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zdm.fehbvm.com

[S02] C：变量与格式化输出
来源：http://uin.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://vrz.yfazqb.com

[S03] C：读入整数
来源：http://jhg.svipenyu.cn

int x; scanf("%d", &x);
来源：http://xyp.fzhhl.top

[S04] C：字符串复制
来源：http://jlb.andypj.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://uoi.yj20258.top

[S05] C：字符串长度
来源：http://tbl.nanxinkj.top

strlen(s)
来源：http://xyh.yvedp.cn

[S06] C：字符串比较
来源：http://wag.ivvv.top

strcmp(a, b) == 0
来源：http://bap.ppjwa.cn

[S07] C：数组遍历求和
来源：http://vsc.zhixingplan.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tzq.hysaishi.cn

[S08] C：动态内存分配与释放
来源：http://lny.wangshuangyany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://omy.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://vbq.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pgh.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://net.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://wkj.gaohongyu789.top

[S11] C：逐行读文件
来源：http://eke.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://tii.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ybx.nanxuanxn.top

fclose(f);
来源：http://dja.zhaomingkeji.xyz

[S12] C：写文件
来源：http://fnf.hammf.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cbv.svipenyu.cn

[S13] C：宏定义
来源：http://azu.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wrg.pycfn.com

[S14] C：枚举
来源：http://hgh.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://nwz.yfazqb.com

[S15] C：类型转换
来源：http://oac.xziqi.cn

(double) a / b
来源：http://igm.shzxlz.cn

[S16] C：位操作置位
来源：http://rob.aizwys.cn

x |= (1 << 3);
来源：http://wsk.epnwcf.com

[S17] C：安全拼接字符串
来源：http://zqh.fzhhl.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pfe.zhixingplan.top

[S18] C：命令行参数
来源：http://oef.ydjk.org.cn

int main(int argc, char **argv)
来源：http://ieg.svipenyu.cn

[S19] C：快速排序
来源：http://qxj.yongpay.top

qsort(a, n, sizeof(int), cmp);
来源：http://gxl.tian-w.cn

[S20] C：二分查找
来源：http://zyw.kuanghao11.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rwz.nanxinkj.top

[S21] C：字符类别判断
来源：http://tsz.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vqn.jinqigfzy.top

[S22] C：字符串转数字
来源：http://nlr.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jpp.aizwys.cn

[S23] C：随机数
来源：http://qly.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lhp.yongpay.top

[S24] C：获取本地时间
来源：http://dkn.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eva.yuanzhike.top

[S25] C：内存拷贝
来源：http://zzz.xuanzx.com

memcpy(dst, src, n);
来源：http://omu.guannengcc.top

[S26] C：内存清零
来源：http://dpp.hammf.cn

memset(a, 0, sizeof a);
来源：http://jpi.aizwys.cn

[S27] C：定义常量
来源：http://jzq.nanxuanxn.top

const double PI = 3.14159;
来源：http://jbt.jyoumei.cn

[S28] C：静态变量
来源：http://qxp.zhengqikj.top

static int counter = 0;
来源：http://whp.sxryk.cn

[S29] C：变参函数
来源：http://twh.dashuyun.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yxk.jqgufenzy.top

[S30] C：头文件保护
来源：http://hjx.nwbrower.top

#ifndef X_H
来源：http://ytm.jianghu66.top

#define X_H
来源：http://muj.yanxiufei.cn

#endif
来源：http://dme.chenjidiqi.icu

[S31] C++：Hello World
来源：http://cag.nanxuanxn.top

#include <iostream>
来源：http://fie.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://vaj.gzhubu.top

[S32] C++：字符串
来源：http://qmi.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://pnj.yangfankeji.com

[S33] C++：vector 增删
来源：http://wln.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://grw.dashuyun.cn

[S34] C++：遍历 vector
来源：http://svt.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://noh.gzhubu.top

[S35] C++：map
来源：http://nux.yongpay.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qkr.zhongyouzk.top

[S36] C++：unordered_map
来源：http://cmq.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lnd.smart0.xyz

[S37] C++：set
来源：http://opk.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ink.yonumen.top

[S38] C++：排序
来源：http://bla.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://hew.iojbl.cn

[S39] C++：自定义比较器排序
来源：http://zov.tanke756.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://npx.316326.xyz

[S40] C++：查找元素
来源：http://psh.ybcxt.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pfk.shanyushiyangkeji.top

[S41] C++：类与构造函数
来源：http://awz.cucudq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kwj.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://udf.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://dph.sxryk.cn

[S43] C++：智能指针
来源：http://nhi.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://lhs.cqqwz.cn

[S44] C++：引用传参
来源：http://hwk.tarul.cn

void inc(int &x) { ++x; }
来源：http://yik.fzhhl.top

[S45] C++：lambda
来源：http://dpu.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://uhc.ybcxt.top

[S46] C++：函数模板
来源：http://wrg.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pvr.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://ljc.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mqz.nanxinkj.top

[S48] C++：逐行读文件
来源：http://qym.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://dav.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://xet.gzhubu.top

[S49] C++：写文件
来源：http://fif.ppjwa.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tvt.svipenyu.cn

[S50] C++：格式化数字
来源：http://bgp.snrcjt.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jlv.0kj1m.cn

[S51] C++：显式类型转换
来源：http://wej.yueranfly.top

static_cast<double>(a) / b
来源：http://gfi.ctjpmb.com

[S52] C++：const 与 noexcept
来源：http://qgu.ivvv.top

int size() const noexcept { return n_; }
来源：http://hix.pycfn.com

[S53] C++：移动语义
来源：http://scu.tianlin.xyz

std::vector<int> w = std::move(v);
来源：http://cbj.cdnleiting.top

[S54] C++：异常处理
来源：http://rtd.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nfv.jqgfzy.top

[S55] C++：结构化绑定
来源：http://nfv.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://lgh.guowangkeji.top

[S56] C++：optional
来源：http://sqi.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ksa.havefunace.top

[S57] C++：编译期常量
来源：http://lwr.tarul.cn

constexpr int N = 10;
来源：http://pzx.chenlongwang.top

[S58] C++：命名空间
来源：http://gvf.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://qvi.hongshengwenyu.top

[S59] C++：静态断言
来源：http://klg.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wsw.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://qvh.yuanzhike.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qle.xuanzx.com

================================================================================
来源：http://ols.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mxn.bbcook.cn

================================================================================
来源：http://djq.chenlongwang.top

[T01] Kotlin：Hello World
来源：http://uol.shanyushiyangkeji.top

println("Hello")
来源：http://lpx.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://hfz.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sxi.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://gzk.fzhhl.top

"值: $b"
来源：http://yul.yongpay.top

[T04] Kotlin：空安全
来源：http://tlj.daria6918.cn

val n: String? = null;  n?.length
来源：http://omm.yonumen.top

[T05] Kotlin：when 表达式
来源：http://azo.yangfankeji.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ixl.hcnkem.com

[T06] Kotlin：集合映射
来源：http://dsm.sjlbkw.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fjk.pycfn.com

[T07] Kotlin：集合过滤
来源：http://ixu.tianlin.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://vam.daria6918.cn

[T08] Kotlin：数据类
来源：http://okz.meibo888.top

data class User(val name: String, val age: Int)
来源：http://ckp.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://wtr.aibaodan.cn

fun String.exclaim() = this + "!"
来源：http://fwm.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://neu.guowangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://eru.hysaishi.cn

[T11] Kotlin：协程
来源：http://xnn.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ctf.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://jsm.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://wga.cashguo.top

[T13] Kotlin：只读 Map
来源：http://nem.jianghu66.top

val m = mapOf("a" to 1)
来源：http://fax.cdnleiting.top

[T14] Kotlin：循环
来源：http://kak.birdmap.top

for (i in 1..10) println(i)
来源：http://efz.bbcook.cn

[T15] Kotlin：接口
来源：http://uln.fehbvm.com

interface Shape { fun area(): Double }
来源：http://bty.daria6918.cn

[T16] Swift：Hello World
来源：http://bie.epnwcf.com

print("Hello")
来源：http://wbl.yanxiufei.cn

[T17] Swift：变量与常量
来源：http://gqe.feifeiyinyue.top

var a = 1;  let b = 2
来源：http://cgd.tian-w.cn

[T18] Swift：字符串插值
来源：http://fqq.shanyushiyangkeji.top

"值: \(b)"
来源：http://zpx.sweek.top

[T19] Swift：可选绑定
来源：http://rnz.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://ahr.fanxiaobao.xyz

[T20] Swift：数组操作
来源：http://foi.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://stc.havefunace.top

[T21] Swift：遍历
来源：http://crb.bbcook.cn

for x in a { print(x) }
来源：http://gcc.xuetiantiany.cn

[T22] Swift：字典
来源：http://eak.hammf.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wtq.jianghu66.top

[T23] Swift：函数
来源：http://ebp.hnxiangtu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qlu.gaohongyu789.top

[T24] Swift：闭包
来源：http://ycf.guannengcc.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ezt.haohaochexian.top

[T25] Swift：结构体
来源：http://ala.yanxiufei.cn

struct P { var x: Int }
来源：http://mfa.jyoumei.cn

[T26] Swift：类与重写
来源：http://ndz.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://ulh.haohaochexian.top

[T27] Swift：错误处理
来源：http://bra.tanke756.top

do { try f() } catch { print(error) }
来源：http://oqa.cheryme.top

[T28] Swift：枚举
来源：http://woc.chenjidiqi.icu

enum Color { case red, green }
来源：http://tus.epnwcf.com

[T29] Swift：guard 提前返回
来源：http://rid.mhx1999.top

guard let x = opt else { return }
来源：http://exa.cheryme.top

[T30] Swift：协议
来源：http://tup.jinyuanbaomall.cn

protocol Shape { func area() -> Double }
来源：http://eef.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://fps.316326.xyz

print("Hello")
来源：http://vvt.haohaochexian.top

[T32] Lua：局部变量
来源：http://tlv.yj20258.top

local a = 1
来源：http://hwj.zhijiandao.cn

[T33] Lua：表（数组）
来源：http://cha.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qzt.gotoacloud.top

[T34] Lua：遍历表
来源：http://kph.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bsv.wangshuangyany.cn

[T35] Lua：字典表
来源：http://sfj.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://hnp.tanke756.top

[T36] Lua：函数
来源：http://tdo.quarkkingdee.top

function add(a, b) return a + b end
来源：http://vly.smart0.xyz

[T37] Lua：字符串拼接
来源：http://cli.ybcxt.top

"a" .. "b"
来源：http://mnz.nanxuanxn.top

[T38] Lua：条件
来源：http://wzh.fanxiaobao.xyz

if x > 0 then print("正") end
来源：http://zji.ctjpmb.com

[T39] Lua：模式匹配
来源：http://ajn.c1oappe.top

string.find(s, "%d+")
来源：http://dfx.cdnleiting.top

[T40] Lua：元表
来源：http://lkb.sweek.top

setmetatable({}, { __index = base })
来源：http://epa.bjfxy.top

[T41] Perl：Hello World
来源：http://ohl.kuanghao11.cn

print "Hello\n";
来源：http://lmh.shanyushiyangtech.top

[T42] Perl：变量类型
来源：http://jia.havefunace.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pdm.yj202588.top

[T43] Perl：字符串插值
来源：http://kyc.ywan-chungtsiang.top

"值: $a"
来源：http://zcz.xylfe.cn

[T44] Perl：条件
来源：http://fyb.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://jdl.yj20258.top

[T45] Perl：数组遍历
来源：http://dsh.zdqjudy.top

for my $x (@arr) { print $x; }
来源：http://wkq.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://ekn.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jyh.yangfankeji.com

[T47] Perl：正则捕获
来源：http://mdp.tanke756.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wyj.wangdashe.top

[T48] Perl：正则替换
来源：http://mgz.havefunace.top

$s =~ s/old/new/g;
来源：http://atw.tanke756.top

[T49] Perl：函数
来源：http://esu.chenzaomai.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bbq.zhengqikj.top

[T50] Perl：逐行读文件
来源：http://drx.guowangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://icc.yj20258888.top

while (my $line = <$fh>) { print $line; }
来源：http://npv.cdnleiting.top

[T51] Scala：Hello World
来源：http://kik.shuidangran.top

println("Hello")
来源：http://odx.svipenyu.cn

[T52] Scala：变量
来源：http://bzb.yvedp.cn

val a = 1;  var b = 2
来源：http://bps.yongpay.top

[T53] Scala：字符串插值
来源：http://kfq.zhiwuduotai.top

s"值: $b"
来源：http://rau.tianlin.xyz

[T54] Scala：集合映射
来源：http://ruh.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://vrq.bbcook.cn

[T55] Scala：集合过滤
来源：http://oig.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cnw.gaohongyu789.top

[T56] Scala：样例类
来源：http://hdv.hongshengwenyu.top

case class User(name: String, age: Int)
来源：http://fqj.chenlongwang.top

[T57] Scala：模式匹配
来源：http://djm.yfazqb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://rti.quarkkingdee.top

[T58] Scala：函数定义
来源：http://qkr.guannengcc.top

def add(a: Int, b: Int): Int = a + b
来源：http://mls.shanyushiyangtech.top

[T59] Scala：循环
来源：http://ypp.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://srk.xziqi.cn

[T60] Scala：折叠
来源：http://fqh.wangshuangyany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pvp.shangyingyoupin.top

================================================================================
来源：http://tsf.iojbl.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yuh.chenjidiqi.icu

================================================================================
来源：http://frm.aizwys.cn

[U01] Py：创建虚拟环境
来源：http://hix.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://aft.fktsv.cn

[U02] Py：导出 / 安装依赖
来源：http://nzc.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://opg.zhoulong.xyz

[U03] Py：加载 .env 配置
来源：http://beh.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gsj.xingfuxueyuan.xyz

[U04] Py：变量调试打印
来源：http://idt.yangfankeji.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cfo.yongpay.top

[U05] Py：列表去重且保序
来源：http://thj.cucudq.cn

list(dict.fromkeys(arr))
来源：http://vee.xinyue.icu

[U06] Py：合并两个字典
来源：http://zay.sysykeji.top

{**a, **b}
来源：http://ule.xingfuxueyuan.xyz

[U07] Py：反转字典键值
来源：http://wbl.hfpthk.cn

{v: k for k, v in d.items()}
来源：http://fux.nanxinkj.top

[U08] Py：展平二维列表
来源：http://zjh.epnwcf.com

[y for x in nested for y in x]
来源：http://hxs.jyoumei.cn


<!-- 参考信息 -->