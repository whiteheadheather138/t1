代发 wailian999

openssl rand -hex 16
来源：http://dts.guannengcc.top

[R68] 计算文件校验值
来源：http://gbr.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://gfy.bjfxy.top

[R69] 生成随机密码
来源：http://szp.guannengcc.top

head -c 16 /dev/urandom | base64
来源：http://pyn.zycfv.cn

[R70] 时间戳与互转
来源：http://wpt.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://esg.vqdsnc.cn

[R71] 日期格式化
来源：http://zcu.quarkkingdee.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tad.aizwys.cn

[R72] 等待端口就绪
来源：http://swn.316326.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://oyx.fanxiaobao.xyz

[R73] 分割大日志
来源：http://cdk.yfazqb.com

split -l 1000 big.log part_
来源：http://rvr.chenzaomai.com

[R74] 批量重命名
来源：http://uqj.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://foj.jinqigufen.top

[R75] 导出环境变量
来源：http://rzc.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://yxa.birdmap.top

[R76] 使用临时文件
来源：http://cci.ybcxt.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://znq.nanxuanxn.top

[R77] 读取用户输入
来源：http://lvx.316326.xyz

read -rp "请输入: " ans
来源：http://vxd.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://jle.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://npa.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://csw.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kgh.zhixingplan.top

[R80] 查看脚本执行耗时
来源：http://yvd.hcnkem.com

time ./run.sh
来源：http://hud.yueranfly.top

================================================================================
来源：http://fzv.jyoumei.cn

S. C / C++ 专题
来源：http://dee.xinyue.icu

================================================================================
来源：http://ppv.cqqwz.cn

[S01] C：Hello World
来源：http://rmf.zhaomingkeji.xyz

#include <stdio.h>
来源：http://gej.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://srf.xuanzx.com

[S02] C：变量与格式化输出
来源：http://djp.chenzaomai.com

int a = 10; printf("%d\n", a);
来源：http://nwq.xinyue.icu

[S03] C：读入整数
来源：http://qyk.mhx1999.top

int x; scanf("%d", &x);
来源：http://oht.zycfv.cn

[S04] C：字符串复制
来源：http://dag.jiagoushi.top

char dst[32]; strcpy(dst, "hi");
来源：http://yib.cheryme.top

[S05] C：字符串长度
来源：http://ntw.feifeiyinyue.top

strlen(s)
来源：http://ypr.fehbvm.com

[S06] C：字符串比较
来源：http://uzv.sxryk.cn

strcmp(a, b) == 0
来源：http://rfz.ppjwa.cn

[S07] C：数组遍历求和
来源：http://dyz.cdnleiting.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nel.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://bdr.meibo888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nxw.yj20258.top

[S09] C：结构体定义与初始化
来源：http://lgw.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nyp.redwolf501.top

[S10] C：指针与解引用
来源：http://xsn.gotoacloud.top

int *p = &a;  *p = 5;
来源：http://rfe.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://kor.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://cxi.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mir.ywan-chungtsiang.top

fclose(f);
来源：http://iyl.chenzaomai.com

[S12] C：写文件
来源：http://upu.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xwr.chenjidiqi.icu

[S13] C：宏定义
来源：http://tmn.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kcl.yuanzhike.top

[S14] C：枚举
来源：http://klj.hnxiangtu.top

enum Color { RED, GREEN, BLUE };
来源：http://jao.yj20258888.top

[S15] C：类型转换
来源：http://vcs.shanyushiyangkeji.top

(double) a / b
来源：http://hpx.xinyue.icu

[S16] C：位操作置位
来源：http://zzv.hongshengwenyu.top

x |= (1 << 3);
来源：http://asd.hnqzz.top

[S17] C：安全拼接字符串
来源：http://euz.chenzaomai.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rmq.cqqwz.cn

[S18] C：命令行参数
来源：http://dpv.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://evn.jyoumei.cn

[S19] C：快速排序
来源：http://fwo.cqqwz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jdp.xinyue.icu

[S20] C：二分查找
来源：http://uow.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xry.ybcxt.top

[S21] C：字符类别判断
来源：http://xof.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dnl.yj202588.top

[S22] C：字符串转数字
来源：http://twl.feifeiyinyue.top

atoi("42");  strtod("3.14", NULL);
来源：http://gvf.sxryk.cn

[S23] C：随机数
来源：http://pdy.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://gbg.kuanghao11.cn

[S24] C：获取本地时间
来源：http://pjs.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zkg.pengpengdd.cyou

[S25] C：内存拷贝
来源：http://tpo.wangdashe.top

memcpy(dst, src, n);
来源：http://kej.mhx1999.top

[S26] C：内存清零
来源：http://ezd.cqqwz.cn

memset(a, 0, sizeof a);
来源：http://qmb.zhijiandao.cn

[S27] C：定义常量
来源：http://shz.zdqjudy.top

const double PI = 3.14159;
来源：http://pjw.jlsjyb.cn

[S28] C：静态变量
来源：http://xda.chenjidiqi.icu

static int counter = 0;
来源：http://enn.wangdashe.top

[S29] C：变参函数
来源：http://bge.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oki.smart0.xyz

[S30] C：头文件保护
来源：http://ynh.xylfe.cn

#ifndef X_H
来源：http://ozj.gaohongyu789.top

#define X_H
来源：http://oiz.yueranfly.top

#endif
来源：http://hyp.hywenlv.cn

[S31] C++：Hello World
来源：http://ogk.ppjwa.cn

#include <iostream>
来源：http://uii.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://nod.birdmap.top

[S32] C++：字符串
来源：http://wjb.hywenlv.cn

std::string s = "hi";  s += "!";
来源：http://euo.uphjek.com

[S33] C++：vector 增删
来源：http://yik.svipenyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://muy.ctjpmb.com

[S34] C++：遍历 vector
来源：http://lkm.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://cth.daria6918.cn

[S35] C++：map
来源：http://bih.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vuk.svipenyu.cn

[S36] C++：unordered_map
来源：http://rbo.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tnu.dianchejie.cn

[S37] C++：set
来源：http://yys.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://okh.pycfn.com

[S38] C++：排序
来源：http://sef.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://ftl.meibo888.top

[S39] C++：自定义比较器排序
来源：http://ine.hcnkem.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jml.hnqzz.top

[S40] C++：查找元素
来源：http://omk.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://quz.jqgfzy.top

[S41] C++：类与构造函数
来源：http://vxs.zhoulong.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wpr.hnqzz.top

[S42] C++：继承与虚函数
来源：http://hwy.zdbjq.cn

class B : public Base { public: void f() override {} };
来源：http://gxp.daria6918.cn

[S43] C++：智能指针
来源：http://cda.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://uxb.nanxuanxn.top

[S44] C++：引用传参
来源：http://unu.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://jgr.zhongyouzk.top

[S45] C++：lambda
来源：http://xxd.zhengqikj.top

auto add = [](int a, int b) { return a + b; };
来源：http://rpf.tarul.cn

[S46] C++：函数模板
来源：http://bgf.jianghu66.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mac.vehdjk.com

[S47] C++：结构化绑定遍历
来源：http://ccx.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nqq.ivvv.top

[S48] C++：逐行读文件
来源：http://frp.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://guj.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://qxg.daxiang520.top

[S49] C++：写文件
来源：http://fem.nwbrower.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://noc.jianghu66.top

[S50] C++：格式化数字
来源：http://xes.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dlr.tian-w.cn

[S51] C++：显式类型转换
来源：http://ism.yvedp.cn

static_cast<double>(a) / b
来源：http://hxs.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://dhk.shanyushiyangkeji.top

int size() const noexcept { return n_; }
来源：http://rvm.quarkkingdee.top

[S53] C++：移动语义
来源：http://hxe.ywan-chungtsiang.top

std::vector<int> w = std::move(v);
来源：http://flv.yongpay.top

[S54] C++：异常处理
来源：http://uov.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pkh.ybcxt.top

[S55] C++：结构化绑定
来源：http://dku.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bmu.ivvv.top

[S56] C++：optional
来源：http://lfa.shangyingyoupin.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pbe.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://fyq.hesvh.cn

constexpr int N = 10;
来源：http://hbe.xziqi.cn

[S58] C++：命名空间
来源：http://tmr.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://tim.cucudq.cn

[S59] C++：静态断言
来源：http://xiq.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uzc.shzxlz.cn

[S60] C++：遍历并删除元素
来源：http://ktd.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qje.feifeiyinyue.top

================================================================================
来源：http://jdz.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dbo.vehdjk.com

================================================================================
来源：http://skj.sxryk.cn

[T01] Kotlin：Hello World
来源：http://kxk.xuanzx.com

println("Hello")
来源：http://dxv.yj202588.top

[T02] Kotlin：变量
来源：http://ukv.zdqjudy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jef.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://bqz.sysykeji.top

"值: $b"
来源：http://xkq.yj202588.top

[T04] Kotlin：空安全
来源：http://fiw.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://rnr.zhaomingkeji.xyz

[T05] Kotlin：when 表达式
来源：http://gzp.sweek.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://csc.mhx1999.top

[T06] Kotlin：集合映射
来源：http://zdb.yuxming.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nhp.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://lfp.dianchejie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wqz.cqqwz.cn

[T08] Kotlin：数据类
来源：http://xlg.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://efv.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://gzy.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://dwj.cheryme.top

[T10] Kotlin：默认参数
来源：http://oxh.yj20258888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gpc.aibaodan.cn

[T11] Kotlin：协程
来源：http://hsu.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dib.shzxlz.cn

[T12] Kotlin：解构声明
来源：http://dhl.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://bjo.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://eqm.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://byg.snrcjt.cn

[T14] Kotlin：循环
来源：http://pdv.sysykeji.top

for (i in 1..10) println(i)
来源：http://maq.snrcjt.cn

[T15] Kotlin：接口
来源：http://lpb.jqgufenzy.top

interface Shape { fun area(): Double }
来源：http://vdf.mhx1999.top

[T16] Swift：Hello World
来源：http://bzg.yj20258888.top

print("Hello")
来源：http://tvd.zhijiandao.cn

[T17] Swift：变量与常量
来源：http://mdv.gogol.net.cn

var a = 1;  let b = 2
来源：http://hqz.yongpay.top

[T18] Swift：字符串插值
来源：http://ipt.zhiwuduotai.top

"值: \(b)"
来源：http://tob.316326.xyz

[T19] Swift：可选绑定
来源：http://xds.0kj1m.cn

if let n = opt { print(n) }
来源：http://vqg.fktsv.cn

[T20] Swift：数组操作
来源：http://fnp.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://zvw.pycfn.com

[T21] Swift：遍历
来源：http://odu.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://mwh.jqgfzy.top

[T22] Swift：字典
来源：http://vjz.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ywa.yvedp.cn

[T23] Swift：函数
来源：http://uwn.tanke756.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ued.yuxming.cn

[T24] Swift：闭包
来源：http://lqk.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mpi.guannengcc.top

[T25] Swift：结构体
来源：http://bsb.hywenlv.cn

struct P { var x: Int }
来源：http://lqt.daxiang520.top

[T26] Swift：类与重写
来源：http://azc.xziqi.cn

class A: Base { override func f() {} }
来源：http://sad.yj20258.top

[T27] Swift：错误处理
来源：http://qbf.uphjek.com

do { try f() } catch { print(error) }
来源：http://oiv.yj202588.top

[T28] Swift：枚举
来源：http://nes.ybcxt.top

enum Color { case red, green }
来源：http://pgl.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://vbo.fengsongda.top

guard let x = opt else { return }
来源：http://rck.chenjidiqi.icu

[T30] Swift：协议
来源：http://ann.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://ttb.tianlin.xyz

[T31] Lua：Hello World
来源：http://kpi.cashguo.top

print("Hello")
来源：http://xbs.yj20258.top

[T32] Lua：局部变量
来源：http://kcr.feifeiyinyue.top

local a = 1
来源：http://siy.wangshuangyany.cn

[T33] Lua：表（数组）
来源：http://gfe.chenlongwang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://olj.sjlbkw.cn

[T34] Lua：遍历表
来源：http://bmq.yongpay.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ikj.jqgufenzy.top

[T35] Lua：字典表
来源：http://ttk.ydzc1.top

local d = { a = 1 };  d.b = 2
来源：http://qfv.yonumen.top

[T36] Lua：函数
来源：http://oxk.hnqzz.top

function add(a, b) return a + b end
来源：http://cuq.nanxuanxn.top

[T37] Lua：字符串拼接
来源：http://cwd.zhengqikj.top

"a" .. "b"
来源：http://smf.sjlbkw.cn

[T38] Lua：条件
来源：http://mkl.havefunace.top

if x > 0 then print("正") end
来源：http://vhp.shzxlz.cn

[T39] Lua：模式匹配
来源：http://kml.zhaomingkeji.xyz

string.find(s, "%d+")
来源：http://jyc.nanxinkj.top

[T40] Lua：元表
来源：http://zge.yongpay.top

setmetatable({}, { __index = base })
来源：http://lio.zhoulong.xyz

[T41] Perl：Hello World
来源：http://syh.uphjek.com

print "Hello\n";
来源：http://vbe.fanxiaobao.xyz

[T42] Perl：变量类型
来源：http://jmm.shanyushiyangtech.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yoj.redwolf501.top

[T43] Perl：字符串插值
来源：http://eoj.dianchejie.cn

"值: $a"
来源：http://wvd.chenjidiqi.icu

[T44] Perl：条件
来源：http://jmb.yonumen.top

if ($a > 0) { print "正"; }
来源：http://vpu.bbcook.cn

[T45] Perl：数组遍历
来源：http://aps.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://ydc.jiagoushi.top

[T46] Perl：哈希操作
来源：http://ovo.hywenlv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dlz.yvedp.cn

[T47] Perl：正则捕获
来源：http://qhf.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://hom.c1oappe.top

[T48] Perl：正则替换
来源：http://oyz.nwbrower.top

$s =~ s/old/new/g;
来源：http://pce.hysaishi.cn

[T49] Perl：函数
来源：http://bap.yuanzhike.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jdk.hcnkem.com

[T50] Perl：逐行读文件
来源：http://swv.hongshengwenyu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://iqz.gaohongyu789.top

while (my $line = <$fh>) { print $line; }
来源：http://eii.yongpay.top

[T51] Scala：Hello World
来源：http://got.xylfe.cn

println("Hello")
来源：http://avz.xuanzx.com

[T52] Scala：变量
来源：http://ygl.aizwys.cn

val a = 1;  var b = 2
来源：http://ibs.nanxinkj.top

[T53] Scala：字符串插值
来源：http://bxg.dianchejie.cn

s"值: $b"
来源：http://hgh.aizwys.cn

[T54] Scala：集合映射
来源：http://tpe.zhoulong.xyz

List(1, 2, 3).map(_ * 2)
来源：http://moy.nanxinkj.top

[T55] Scala：集合过滤
来源：http://slb.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://szj.yvedp.cn

[T56] Scala：样例类
来源：http://txf.haohaochexian.top

case class User(name: String, age: Int)
来源：http://uah.snrcjt.cn

[T57] Scala：模式匹配
来源：http://dte.cucudq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eyd.jinqigufen.top

[T58] Scala：函数定义
来源：http://tay.yanxiufei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ivm.cashguo.top

[T59] Scala：循环
来源：http://zog.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://tcb.guowangkeji.top

[T60] Scala：折叠
来源：http://xog.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oix.ehwqpu.com

================================================================================
来源：http://hdg.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cyy.tarul.cn

================================================================================
来源：http://eki.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://dtu.bbcook.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yjs.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://srf.gogol.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gmg.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://kph.nanxuanxn.top

from dotenv import load_dotenv; load_dotenv()
来源：http://avk.zhengqikj.top

[U04] Py：变量调试打印
来源：http://olt.fzhhl.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hvo.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://nkc.meibo888.top

list(dict.fromkeys(arr))
来源：http://qjo.guannengcc.top

[U06] Py：合并两个字典
来源：http://ocq.sweek.top

{**a, **b}
来源：http://ohz.zhengqikj.top

[U07] Py：反转字典键值
来源：http://rmn.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://xuq.smart0.xyz

[U08] Py：展平二维列表
来源：http://gtn.sweek.top

[y for x in nested for y in x]
来源：http://pcm.hnqzz.top


<!-- 参考信息 -->