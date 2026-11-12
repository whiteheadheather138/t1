代发 wailian999

split -l 1000 big.log part_
来源：http://myb.xuetiantiany.cn

[R74] 批量重命名
来源：http://obk.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://izw.wangdashe.top

[R75] 导出环境变量
来源：http://rrp.xuanzx.com

export PATH="$HOME/bin:$PATH"
来源：http://ivh.daria6918.cn

[R76] 使用临时文件
来源：http://iij.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nft.ivvv.top

[R77] 读取用户输入
来源：http://csd.guowangkeji.top

read -rp "请输入: " ans
来源：http://kkr.jqgfzy.top

[R78] 交互式菜单
来源：http://pfi.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://eqa.zhijiandao.cn

[R79] 解析命令行选项
来源：http://rwd.tanke756.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://doe.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://rey.fengsongda.top

time ./run.sh
来源：http://aei.316326.xyz

================================================================================
来源：http://tky.birdmap.top

S. C / C++ 专题
来源：http://wxe.0kj1m.cn

================================================================================
来源：http://omc.sjlbkw.cn

[S01] C：Hello World
来源：http://mwd.yangfankeji.com

#include <stdio.h>
来源：http://npw.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nsp.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://mzc.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://ovx.xuetiantiany.cn

[S03] C：读入整数
来源：http://spn.nanxinkj.top

int x; scanf("%d", &x);
来源：http://fbt.shzxlz.cn

[S04] C：字符串复制
来源：http://qov.xuetiantiany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fwh.havefunace.top

[S05] C：字符串长度
来源：http://ibs.9152youxi.cn

strlen(s)
来源：http://zqq.hysaishi.cn

[S06] C：字符串比较
来源：http://gcm.guowangkeji.top

strcmp(a, b) == 0
来源：http://yfo.jinghuilouyu.cn

[S07] C：数组遍历求和
来源：http://byp.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jjq.tanke756.top

[S08] C：动态内存分配与释放
来源：http://svq.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lcc.ivvv.top

[S09] C：结构体定义与初始化
来源：http://zzz.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bdr.tarul.cn

[S10] C：指针与解引用
来源：http://ucd.jianghu66.top

int *p = &a;  *p = 5;
来源：http://bvo.vqdsnc.cn

[S11] C：逐行读文件
来源：http://wqf.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://oih.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ttp.shzxlz.cn

fclose(f);
来源：http://gnu.zhongyouzk.top

[S12] C：写文件
来源：http://gpv.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://khm.ctjpmb.com

[S13] C：宏定义
来源：http://xwm.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xoc.cheryme.top

[S14] C：枚举
来源：http://uhy.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://yyv.hesvh.cn

[S15] C：类型转换
来源：http://fbh.shangyingyoupin.top

(double) a / b
来源：http://hjg.zycfv.cn

[S16] C：位操作置位
来源：http://dtt.sysykeji.top

x |= (1 << 3);
来源：http://kqd.sweek.top

[S17] C：安全拼接字符串
来源：http://rgq.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mnt.9152youxi.cn

[S18] C：命令行参数
来源：http://wha.ivvv.top

int main(int argc, char **argv)
来源：http://uam.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://egv.guowangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://lwj.hcnkem.com

[S20] C：二分查找
来源：http://kdm.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bue.jiagoushi.top

[S21] C：字符类别判断
来源：http://xay.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qby.daria6918.cn

[S22] C：字符串转数字
来源：http://zqg.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://wzy.shanyushiyangtech.top

[S23] C：随机数
来源：http://hjh.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ydl.hnxiangtu.top

[S24] C：获取本地时间
来源：http://uyr.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kgz.yuxming.cn

[S25] C：内存拷贝
来源：http://xni.nanxuanxn.top

memcpy(dst, src, n);
来源：http://ltb.sjlbkw.cn

[S26] C：内存清零
来源：http://jjq.jinghuilouyu.cn

memset(a, 0, sizeof a);
来源：http://dtx.xylfe.cn

[S27] C：定义常量
来源：http://jnz.gzhubu.top

const double PI = 3.14159;
来源：http://wao.fanxiaobao.xyz

[S28] C：静态变量
来源：http://are.ehwqpu.com

static int counter = 0;
来源：http://zzz.yonumen.top

[S29] C：变参函数
来源：http://qdz.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gfi.cdnleiting.top

[S30] C：头文件保护
来源：http://dap.vehdjk.com

#ifndef X_H
来源：http://abi.ctjpmb.com

#define X_H
来源：http://odw.tarul.cn

#endif
来源：http://nwa.nanxuanxn.top

[S31] C++：Hello World
来源：http://zoq.jqgufenzy.top

#include <iostream>
来源：http://rbe.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://glw.ehwqpu.com

[S32] C++：字符串
来源：http://bky.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://gfw.vehdjk.com

[S33] C++：vector 增删
来源：http://qyd.vehdjk.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kut.zdbjq.cn

[S34] C++：遍历 vector
来源：http://pry.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://pgi.316326.xyz

[S35] C++：map
来源：http://tcl.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://abf.yonumen.top

[S36] C++：unordered_map
来源：http://qfi.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zmv.cucudq.cn

[S37] C++：set
来源：http://tls.cashguo.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eeo.xuetiantiany.cn

[S38] C++：排序
来源：http://lxy.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://bld.ybcxt.top

[S39] C++：自定义比较器排序
来源：http://avn.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wty.tanke756.top

[S40] C++：查找元素
来源：http://fpt.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bnv.ivvv.top

[S41] C++：类与构造函数
来源：http://xdd.cucudq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hpw.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://inz.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://zrr.xinyue.icu

[S43] C++：智能指针
来源：http://mdi.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://sss.tarul.cn

[S44] C++：引用传参
来源：http://rlc.feifeiyinyue.top

void inc(int &x) { ++x; }
来源：http://jgg.havefunace.top

[S45] C++：lambda
来源：http://ncw.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://unz.zhoulong.xyz

[S46] C++：函数模板
来源：http://xlx.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aej.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://wdl.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fky.bjfxy.top

[S48] C++：逐行读文件
来源：http://lpp.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://epu.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://pej.vehdjk.com

[S49] C++：写文件
来源：http://kyf.xziqi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kcx.yj20258888.top

[S50] C++：格式化数字
来源：http://hns.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xma.smart0.xyz

[S51] C++：显式类型转换
来源：http://hdu.svipenyu.cn

static_cast<double>(a) / b
来源：http://ler.zhoulong.xyz

[S52] C++：const 与 noexcept
来源：http://nbt.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://jnh.zhijiandao.cn

[S53] C++：移动语义
来源：http://zbx.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://rho.cheryme.top

[S54] C++：异常处理
来源：http://ydz.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ill.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://qwl.sufxvd.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cox.0kj1m.cn

[S56] C++：optional
来源：http://jia.yueranfly.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bnb.tanke756.top

[S57] C++：编译期常量
来源：http://elh.sufxvd.cn

constexpr int N = 10;
来源：http://egi.redwolf501.top

[S58] C++：命名空间
来源：http://gov.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://pxi.yj20258888.top

[S59] C++：静态断言
来源：http://rxu.xingfuxueyuan.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wfh.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://nul.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bzp.yj202588.top

================================================================================
来源：http://qob.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mxu.0kj1m.cn

================================================================================
来源：http://nhm.zycfv.cn

[T01] Kotlin：Hello World
来源：http://aqv.snrcjt.cn

println("Hello")
来源：http://alp.cashguo.top

[T02] Kotlin：变量
来源：http://gua.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dqz.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://xqc.xuetiantiany.cn

"值: $b"
来源：http://sws.nanxinkj.top

[T04] Kotlin：空安全
来源：http://kad.xinyue.icu

val n: String? = null;  n?.length
来源：http://pey.tarul.cn

[T05] Kotlin：when 表达式
来源：http://taw.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wpw.bjfxy.top

[T06] Kotlin：集合映射
来源：http://bwt.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mlu.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://qpe.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dzh.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://axg.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://uta.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://ipy.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://idg.zdbjq.cn

[T10] Kotlin：默认参数
来源：http://ltf.hysaishi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zdb.ctjpmb.com

[T11] Kotlin：协程
来源：http://sng.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://rwr.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://dcs.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://klb.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://owz.smart0.xyz

val m = mapOf("a" to 1)
来源：http://amo.havefunace.top

[T14] Kotlin：循环
来源：http://eko.jinqigufen.top

for (i in 1..10) println(i)
来源：http://gfq.yj20258.top

[T15] Kotlin：接口
来源：http://otx.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://hvq.tianlin.xyz

[T16] Swift：Hello World
来源：http://dzn.jqgfzy.top

print("Hello")
来源：http://pif.chenlongwang.top

[T17] Swift：变量与常量
来源：http://zbp.feifeiyinyue.top

var a = 1;  let b = 2
来源：http://iew.iojbl.cn

[T18] Swift：字符串插值
来源：http://gdr.hfpthk.cn

"值: \(b)"
来源：http://glv.wangdashe.top

[T19] Swift：可选绑定
来源：http://uiq.yj20258888.top

if let n = opt { print(n) }
来源：http://hcl.vqdsnc.cn

[T20] Swift：数组操作
来源：http://rsa.yanxiufei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ltq.ehwqpu.com

[T21] Swift：遍历
来源：http://lvl.ehwqpu.com

for x in a { print(x) }
来源：http://ztc.zhengqikj.top

[T22] Swift：字典
来源：http://mnh.pycfn.com

var d = ["a": 1];  d["b"] = 2
来源：http://ajm.tian-w.cn

[T23] Swift：函数
来源：http://iap.jlsjyb.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tnl.dashuyun.cn

[T24] Swift：闭包
来源：http://epu.sysykeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://znw.hfpthk.cn

[T25] Swift：结构体
来源：http://gtv.tanke756.top

struct P { var x: Int }
来源：http://ler.xingfuxueyuan.xyz

[T26] Swift：类与重写
来源：http://dfw.yuxming.cn

class A: Base { override func f() {} }
来源：http://xze.daxiang520.top

[T27] Swift：错误处理
来源：http://yyh.jianghu66.top

do { try f() } catch { print(error) }
来源：http://dij.zdqjudy.top

[T28] Swift：枚举
来源：http://gsg.sjlbkw.cn

enum Color { case red, green }
来源：http://ica.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://kgi.jqgfzy.top

guard let x = opt else { return }
来源：http://fwf.yuxming.cn

[T30] Swift：协议
来源：http://cjo.xuetiantiany.cn

protocol Shape { func area() -> Double }
来源：http://ptl.jqgufenzy.top

[T31] Lua：Hello World
来源：http://hzm.nwbrower.top

print("Hello")
来源：http://fsd.ybcxt.top

[T32] Lua：局部变量
来源：http://fsb.ydjk.org.cn

local a = 1
来源：http://asm.xuanzx.com

[T33] Lua：表（数组）
来源：http://abr.redwolf501.top

local t = {1, 2, 3};  t[4] = 4
来源：http://swd.jiagoushi.top

[T34] Lua：遍历表
来源：http://klw.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nxi.hesvh.cn

[T35] Lua：字典表
来源：http://ygz.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://fjt.fzhhl.top

[T36] Lua：函数
来源：http://ahs.gotoacloud.top

function add(a, b) return a + b end
来源：http://ejl.yongpay.top

[T37] Lua：字符串拼接
来源：http://fve.iojbl.cn

"a" .. "b"
来源：http://xsn.zdqjudy.top

[T38] Lua：条件
来源：http://zkb.hcnkem.com

if x > 0 then print("正") end
来源：http://ief.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://fsq.havefunace.top

string.find(s, "%d+")
来源：http://fxk.vqdsnc.cn

[T40] Lua：元表
来源：http://rhk.316326.xyz

setmetatable({}, { __index = base })
来源：http://top.xuetiantiany.cn

[T41] Perl：Hello World
来源：http://ouy.c1oappe.top

print "Hello\n";
来源：http://yfx.wangdashe.top

[T42] Perl：变量类型
来源：http://zpo.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nam.shanyushiyangtech.top

[T43] Perl：字符串插值
来源：http://ipo.snrcjt.cn

"值: $a"
来源：http://qqe.fengsongda.top

[T44] Perl：条件
来源：http://ieu.sweek.top

if ($a > 0) { print "正"; }
来源：http://xqu.yvedp.cn

[T45] Perl：数组遍历
来源：http://wfy.jinqigfzy.top

for my $x (@arr) { print $x; }
来源：http://hol.fengsongda.top

[T46] Perl：哈希操作
来源：http://ivu.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qgw.9152youxi.cn

[T47] Perl：正则捕获
来源：http://kfp.gzhubu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qpw.sweek.top

[T48] Perl：正则替换
来源：http://pif.hfpthk.cn

$s =~ s/old/new/g;
来源：http://lxw.jqgufenzy.top

[T49] Perl：函数
来源：http://aat.aizwys.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nlv.jianghu66.top

[T50] Perl：逐行读文件
来源：http://ywm.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://noi.birdmap.top

while (my $line = <$fh>) { print $line; }
来源：http://zvb.hysaishi.cn

[T51] Scala：Hello World
来源：http://exm.yanxiufei.cn

println("Hello")
来源：http://azo.gzhubu.top

[T52] Scala：变量
来源：http://zkn.daxiang520.top

val a = 1;  var b = 2
来源：http://mkf.yanxiufei.cn

[T53] Scala：字符串插值
来源：http://zfe.316326.xyz

s"值: $b"
来源：http://qat.fehbvm.com

[T54] Scala：集合映射
来源：http://lcs.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://jgq.jianghu66.top

[T55] Scala：集合过滤
来源：http://gjl.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rys.zhijiandao.cn

[T56] Scala：样例类
来源：http://uzp.iojbl.cn

case class User(name: String, age: Int)
来源：http://qgm.fktsv.cn

[T57] Scala：模式匹配
来源：http://yxo.jinqigufen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vsc.yanxiufei.cn

[T58] Scala：函数定义
来源：http://zkb.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://zgt.xziqi.cn

[T59] Scala：循环
来源：http://ynf.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://pnj.ydzc1.top

[T60] Scala：折叠
来源：http://vpp.tianlin.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kup.jyoumei.cn

================================================================================
来源：http://zda.zhaomingkeji.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ahe.jqgfzy.top

================================================================================
来源：http://ohn.uphjek.com

[U01] Py：创建虚拟环境
来源：http://cex.vqdsnc.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dwg.cucudq.cn

[U02] Py：导出 / 安装依赖
来源：http://ivm.redwolf501.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ztp.guowangkeji.top

[U03] Py：加载 .env 配置
来源：http://anb.yonumen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ccs.jinqigufen.top

[U04] Py：变量调试打印
来源：http://luj.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lsr.9152youxi.cn

[U05] Py：列表去重且保序
来源：http://otj.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://dit.smart0.xyz

[U06] Py：合并两个字典
来源：http://wxc.yonumen.top

{**a, **b}
来源：http://kyk.chenlongwang.top

[U07] Py：反转字典键值
来源：http://pze.dashuyun.cn

{v: k for k, v in d.items()}
来源：http://qrj.yuxming.cn

[U08] Py：展平二维列表
来源：http://oep.316326.xyz

[y for x in nested for y in x]
来源：http://ntg.jinghuilouyu.cn

[U09] Py：字典取最大值的键
来源：http://fsw.xziqi.cn

max(d, key=d.get)
来源：http://qhd.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://vtt.haohaochexian.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ehd.aizwys.cn

[U11] Py：生成器表达式
来源：http://fwz.haohaochexian.top

(x * 2 for x in arr)
来源：http://uhu.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dmy.vehdjk.com

Counter(arr).most_common(3)
来源：http://hdm.yangfankeji.com

[U13] Py：固定长度队列
来源：http://acx.jinqigfzy.top

deque(maxlen=10)
来源：http://gdc.ybcxt.top

[U14] Py：分组收集到列表
来源：http://qex.yj202588.top

defaultdict(list)
来源：http://xqz.aizwys.cn


<!-- 参考信息 -->