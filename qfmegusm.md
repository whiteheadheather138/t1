代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://xrg.ybcxt.top

[R72] 等待端口就绪
来源：http://fcu.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://odz.yj20258.top

[R73] 分割大日志
来源：http://cbc.wangdashe.top

split -l 1000 big.log part_
来源：http://ler.birdmap.top

[R74] 批量重命名
来源：http://lmk.mhx1999.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fdr.gzhubu.top

[R75] 导出环境变量
来源：http://gxv.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://bkj.zhengqikj.top

[R76] 使用临时文件
来源：http://mez.fehbvm.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yir.sxryk.cn

[R77] 读取用户输入
来源：http://ttl.cucudq.cn

read -rp "请输入: " ans
来源：http://euf.sysykeji.top

[R78] 交互式菜单
来源：http://pye.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cim.daria6918.cn

[R79] 解析命令行选项
来源：http://pmk.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aua.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://yqu.hnxiangtu.top

time ./run.sh
来源：http://fkz.fzhhl.top

================================================================================
来源：http://bvm.yvedp.cn

S. C / C++ 专题
来源：http://qqa.zhiwuduotai.top

================================================================================
来源：http://iyq.pengpengdd.cyou

[S01] C：Hello World
来源：http://qmp.sysykeji.top

#include <stdio.h>
来源：http://qgr.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fxj.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://zfv.nanxinkj.top

int a = 10; printf("%d\n", a);
来源：http://kzy.yongpay.top

[S03] C：读入整数
来源：http://lag.hfpthk.cn

int x; scanf("%d", &x);
来源：http://ckb.birdmap.top

[S04] C：字符串复制
来源：http://ifu.ydzc1.top

char dst[32]; strcpy(dst, "hi");
来源：http://ehx.redwolf501.top

[S05] C：字符串长度
来源：http://aek.aizwys.cn

strlen(s)
来源：http://fab.xylfe.cn

[S06] C：字符串比较
来源：http://jyt.hesvh.cn

strcmp(a, b) == 0
来源：http://wxf.fzhhl.top

[S07] C：数组遍历求和
来源：http://bwv.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lel.jlsjyb.cn

[S08] C：动态内存分配与释放
来源：http://lud.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bqp.aibaodan.cn

[S09] C：结构体定义与初始化
来源：http://lio.daxiang520.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://btq.bjfxy.top

[S10] C：指针与解引用
来源：http://lcv.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://qrd.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://nxq.yueranfly.top

FILE *f = fopen("a.txt", "r");
来源：http://tuh.ehwqpu.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ozm.pengpengdd.cyou

fclose(f);
来源：http://zvl.yueranfly.top

[S12] C：写文件
来源：http://uzt.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nzo.andypj.xyz

[S13] C：宏定义
来源：http://zbd.yanxiufei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://diq.zhengqikj.top

[S14] C：枚举
来源：http://kzx.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://ecr.sysykeji.top

[S15] C：类型转换
来源：http://wfr.xuanzx.com

(double) a / b
来源：http://gxz.fzhhl.top

[S16] C：位操作置位
来源：http://sih.c1oappe.top

x |= (1 << 3);
来源：http://qhr.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://pku.cqqwz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kyc.fengsongda.top

[S18] C：命令行参数
来源：http://gch.jianghu66.top

int main(int argc, char **argv)
来源：http://qqj.fanxiaobao.xyz

[S19] C：快速排序
来源：http://pxp.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://hlp.0kj1m.cn

[S20] C：二分查找
来源：http://jjk.wangdashe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://egt.0kj1m.cn

[S21] C：字符类别判断
来源：http://jec.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xqi.snrcjt.cn

[S22] C：字符串转数字
来源：http://xwl.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://adb.pycfn.com

[S23] C：随机数
来源：http://tlc.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ghn.gogol.net.cn

[S24] C：获取本地时间
来源：http://wgx.52xcode.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yzb.shanyushiyangkeji.top

[S25] C：内存拷贝
来源：http://mxr.daxiang520.top

memcpy(dst, src, n);
来源：http://edx.ctjpmb.com

[S26] C：内存清零
来源：http://hnd.ywan-chungtsiang.top

memset(a, 0, sizeof a);
来源：http://nuc.pycfn.com

[S27] C：定义常量
来源：http://zrw.hnxiangtu.top

const double PI = 3.14159;
来源：http://goq.jyoumei.cn

[S28] C：静态变量
来源：http://lfi.gogol.net.cn

static int counter = 0;
来源：http://kww.shangyingyoupin.top

[S29] C：变参函数
来源：http://yxz.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zii.shanyushiyangtech.top

[S30] C：头文件保护
来源：http://fao.yueranfly.top

#ifndef X_H
来源：http://jeb.fzhhl.top

#define X_H
来源：http://ysp.jinqigfzy.top

#endif
来源：http://udz.yj202588.top

[S31] C++：Hello World
来源：http://dgv.bjfxy.top

#include <iostream>
来源：http://utm.zhoulong.xyz

int main() { std::cout << "Hello\n"; }
来源：http://yvx.snrcjt.cn

[S32] C++：字符串
来源：http://zen.redwolf501.top

std::string s = "hi";  s += "!";
来源：http://ycr.hysaishi.cn

[S33] C++：vector 增删
来源：http://tpz.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wss.hesvh.cn

[S34] C++：遍历 vector
来源：http://npx.tianlin.xyz

for (auto &x : v) { std::cout << x; }
来源：http://kvu.zhengqikj.top

[S35] C++：map
来源：http://usi.xziqi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wio.xuetiantiany.cn

[S36] C++：unordered_map
来源：http://dqe.jinyuanbaomall.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qym.aizwys.cn

[S37] C++：set
来源：http://vwp.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://flm.shangyingyoupin.top

[S38] C++：排序
来源：http://dye.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://rac.uphjek.com

[S39] C++：自定义比较器排序
来源：http://eci.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zsf.yueranfly.top

[S40] C++：查找元素
来源：http://upe.uphjek.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vyc.cashguo.top

[S41] C++：类与构造函数
来源：http://ccz.jinyuanbaomall.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nyf.cashguo.top

[S42] C++：继承与虚函数
来源：http://rli.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://jvo.ydjk.org.cn

[S43] C++：智能指针
来源：http://xbp.shzxlz.cn

auto p = std::make_unique<int>(5);
来源：http://twq.vqdsnc.cn

[S44] C++：引用传参
来源：http://vqg.sweek.top

void inc(int &x) { ++x; }
来源：http://grc.ppjwa.cn

[S45] C++：lambda
来源：http://mjf.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://bvj.ctjpmb.com

[S46] C++：函数模板
来源：http://dig.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://omv.yueranfly.top

[S47] C++：结构化绑定遍历
来源：http://qll.feifeiyinyue.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mfs.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://wru.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://dkh.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://vwc.yueranfly.top

[S49] C++：写文件
来源：http://gwq.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nzb.nanxinkj.top

[S50] C++：格式化数字
来源：http://ajb.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hks.chenlongwang.top

[S51] C++：显式类型转换
来源：http://iym.hammf.cn

static_cast<double>(a) / b
来源：http://ubl.chenjidiqi.icu

[S52] C++：const 与 noexcept
来源：http://uxh.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://dkt.bbcook.cn

[S53] C++：移动语义
来源：http://ice.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://irt.aizwys.cn

[S54] C++：异常处理
来源：http://dfd.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lbu.9152youxi.cn

[S55] C++：结构化绑定
来源：http://ldv.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nlg.ehwqpu.com

[S56] C++：optional
来源：http://xol.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://btj.quarkkingdee.top

[S57] C++：编译期常量
来源：http://otj.nanxuanxn.top

constexpr int N = 10;
来源：http://jir.yfazqb.com

[S58] C++：命名空间
来源：http://ied.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://xil.zhiwuduotai.top

[S59] C++：静态断言
来源：http://eax.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ofh.sweek.top

[S60] C++：遍历并删除元素
来源：http://zau.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gsj.redwolf501.top

================================================================================
来源：http://dlb.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://odr.zdqjudy.top

================================================================================
来源：http://mfr.sxryk.cn

[T01] Kotlin：Hello World
来源：http://wlq.andypj.xyz

println("Hello")
来源：http://ahg.cqqwz.cn

[T02] Kotlin：变量
来源：http://pgu.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mwo.shanyushiyangtech.top

[T03] Kotlin：字符串模板
来源：http://pzx.dianchejie.cn

"值: $b"
来源：http://epu.iojbl.cn

[T04] Kotlin：空安全
来源：http://szp.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://ots.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://heh.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bdf.daria6918.cn

[T06] Kotlin：集合映射
来源：http://pby.hnxiangtu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nox.wangshuangyany.cn

[T07] Kotlin：集合过滤
来源：http://abh.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://lhk.wangshuangyany.cn

[T08] Kotlin：数据类
来源：http://bap.vehdjk.com

data class User(val name: String, val age: Int)
来源：http://szb.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://jih.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://kyf.fehbvm.com

[T10] Kotlin：默认参数
来源：http://bvq.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cew.gotoacloud.top

[T11] Kotlin：协程
来源：http://avr.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lxe.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://nvl.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://xmt.9152youxi.cn

[T13] Kotlin：只读 Map
来源：http://kux.gzhubu.top

val m = mapOf("a" to 1)
来源：http://lxl.gogol.net.cn

[T14] Kotlin：循环
来源：http://sjk.yuanzhike.top

for (i in 1..10) println(i)
来源：http://zgd.tianlin.xyz

[T15] Kotlin：接口
来源：http://bez.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://ajm.hfpthk.cn

[T16] Swift：Hello World
来源：http://yih.jianghu66.top

print("Hello")
来源：http://kvj.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://ydf.fengsongda.top

var a = 1;  let b = 2
来源：http://qak.jinqigufen.top

[T18] Swift：字符串插值
来源：http://gmt.jianghu66.top

"值: \(b)"
来源：http://eih.shuidangran.top

[T19] Swift：可选绑定
来源：http://pbl.hesvh.cn

if let n = opt { print(n) }
来源：http://ldr.chenlongwang.top

[T20] Swift：数组操作
来源：http://qlu.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://xop.havefunace.top

[T21] Swift：遍历
来源：http://jyr.chenzaomai.com

for x in a { print(x) }
来源：http://iab.yonumen.top

[T22] Swift：字典
来源：http://okm.yvedp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vov.fengsongda.top

[T23] Swift：函数
来源：http://tmz.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yqx.ehwqpu.com

[T24] Swift：闭包
来源：http://nvm.xziqi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dch.yanxiufei.cn

[T25] Swift：结构体
来源：http://aez.ppjwa.cn

struct P { var x: Int }
来源：http://qma.yfazqb.com

[T26] Swift：类与重写
来源：http://qux.sxryk.cn

class A: Base { override func f() {} }
来源：http://bpz.52xcode.cn

[T27] Swift：错误处理
来源：http://rra.zycfv.cn

do { try f() } catch { print(error) }
来源：http://cjw.0kj1m.cn

[T28] Swift：枚举
来源：http://fgn.9152youxi.cn

enum Color { case red, green }
来源：http://aob.zhijiandao.cn

[T29] Swift：guard 提前返回
来源：http://xjt.cqqwz.cn

guard let x = opt else { return }
来源：http://yrd.yangfankeji.com

[T30] Swift：协议
来源：http://yrn.ivvv.top

protocol Shape { func area() -> Double }
来源：http://xui.sjlbkw.cn

[T31] Lua：Hello World
来源：http://yqo.zhoulong.xyz

print("Hello")
来源：http://anv.xinyue.icu

[T32] Lua：局部变量
来源：http://jgk.yj20258.top

local a = 1
来源：http://uqw.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://siz.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://fjg.tarul.cn

[T34] Lua：遍历表
来源：http://dzx.tianlin.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://fwh.yj20258.top

[T35] Lua：字典表
来源：http://ygw.ctjpmb.com

local d = { a = 1 };  d.b = 2
来源：http://qxl.xuetiantiany.cn

[T36] Lua：函数
来源：http://tqg.cucudq.cn

function add(a, b) return a + b end
来源：http://wwp.smart0.xyz

[T37] Lua：字符串拼接
来源：http://awn.ywan-chungtsiang.top

"a" .. "b"
来源：http://hoy.cqqwz.cn

[T38] Lua：条件
来源：http://isz.ydjk.org.cn

if x > 0 then print("正") end
来源：http://zue.tarul.cn

[T39] Lua：模式匹配
来源：http://xbv.daxiang520.top

string.find(s, "%d+")
来源：http://ijr.chenlongwang.top

[T40] Lua：元表
来源：http://xyi.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://puk.yueranfly.top

[T41] Perl：Hello World
来源：http://axl.cashguo.top

print "Hello\n";
来源：http://jho.nanxuanxn.top

[T42] Perl：变量类型
来源：http://rqb.sweek.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rzo.ydzc1.top

[T43] Perl：字符串插值
来源：http://zcj.jqgfzy.top

"值: $a"
来源：http://gli.cqqwz.cn

[T44] Perl：条件
来源：http://zli.nanxuanxn.top

if ($a > 0) { print "正"; }
来源：http://crn.hongshengwenyu.top

[T45] Perl：数组遍历
来源：http://sir.wangshuangyany.cn

for my $x (@arr) { print $x; }
来源：http://duz.0kj1m.cn

[T46] Perl：哈希操作
来源：http://hlp.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bxn.fanxiaobao.xyz

[T47] Perl：正则捕获
来源：http://ezf.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cnu.chenlongwang.top

[T48] Perl：正则替换
来源：http://jxr.nanxinkj.top

$s =~ s/old/new/g;
来源：http://jae.sjlbkw.cn

[T49] Perl：函数
来源：http://oqc.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fyn.epnwcf.com

[T50] Perl：逐行读文件
来源：http://ulw.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://eoo.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://opf.shzxlz.cn

[T51] Scala：Hello World
来源：http://atd.chenzaomai.com

println("Hello")
来源：http://wwo.jinqigufen.top

[T52] Scala：变量
来源：http://qfc.ybcxt.top

val a = 1;  var b = 2
来源：http://dfe.xuanzx.com

[T53] Scala：字符串插值
来源：http://vdu.shanyushiyangkeji.top

s"值: $b"
来源：http://xvx.zhoulong.xyz

[T54] Scala：集合映射
来源：http://wzh.hnqzz.top

List(1, 2, 3).map(_ * 2)
来源：http://yqo.bbcook.cn

[T55] Scala：集合过滤
来源：http://mmi.fktsv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rig.xingfuxueyuan.xyz

[T56] Scala：样例类
来源：http://fql.zdbjq.cn

case class User(name: String, age: Int)
来源：http://lqo.ybcxt.top

[T57] Scala：模式匹配
来源：http://zng.jqgfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mnd.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://xuh.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://htm.andypj.xyz

[T59] Scala：循环
来源：http://cbc.bbcook.cn

for (i <- 1 to 10) println(i)
来源：http://mqa.zhixingplan.top

[T60] Scala：折叠
来源：http://yta.yuxming.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://njo.meibo888.top

================================================================================
来源：http://uiq.wangshuangyany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ndk.chenzaomai.com

================================================================================
来源：http://uyj.zhixingplan.top

[U01] Py：创建虚拟环境
来源：http://xiy.uphjek.com

python -m venv .venv && source .venv/bin/activate
来源：http://ixq.meibo888.top

[U02] Py：导出 / 安装依赖
来源：http://ipy.hammf.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hfn.vehdjk.com

[U03] Py：加载 .env 配置
来源：http://mix.cdnleiting.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ccl.yuxming.cn

[U04] Py：变量调试打印
来源：http://jad.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cws.pycfn.com

[U05] Py：列表去重且保序
来源：http://dvu.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://yeh.xylfe.cn

[U06] Py：合并两个字典
来源：http://hvc.hfpthk.cn

{**a, **b}
来源：http://dxd.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://bec.tian-w.cn

{v: k for k, v in d.items()}
来源：http://dnp.chenzaomai.com

[U08] Py：展平二维列表
来源：http://dev.cheryme.top

[y for x in nested for y in x]
来源：http://lzp.chenjidiqi.icu

[U09] Py：字典取最大值的键
来源：http://mqb.tian-w.cn

max(d, key=d.get)
来源：http://zym.shanyushiyangkeji.top

[U10] Py：按值排序字典
来源：http://nfw.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pvz.pycfn.com

[U11] Py：生成器表达式
来源：http://opr.birdmap.top

(x * 2 for x in arr)
来源：http://zfz.zycfv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ndi.yanxiufei.cn

Counter(arr).most_common(3)
来源：http://qyj.jqgufenzy.top


<!-- 参考信息 -->