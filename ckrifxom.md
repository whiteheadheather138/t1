代发 wailian999

openssl rand -hex 16
来源：http://ofg.fehbvm.com

[R68] 计算文件校验值
来源：http://roo.pycfn.com

sha256sum a.txt;  md5sum a.txt
来源：http://jbi.yuanzhike.top

[R69] 生成随机密码
来源：http://smn.ydzc1.top

head -c 16 /dev/urandom | base64
来源：http://lkv.chenzaomai.com

[R70] 时间戳与互转
来源：http://cbu.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://kml.9152youxi.cn

[R71] 日期格式化
来源：http://tix.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fde.sweek.top

[R72] 等待端口就绪
来源：http://nhp.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://clx.tarul.cn

[R73] 分割大日志
来源：http://xlu.svipenyu.cn

split -l 1000 big.log part_
来源：http://stz.jqgufenzy.top

[R74] 批量重命名
来源：http://oul.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jef.shzxlz.cn

[R75] 导出环境变量
来源：http://eww.shuidangran.top

export PATH="$HOME/bin:$PATH"
来源：http://jrj.ctjpmb.com

[R76] 使用临时文件
来源：http://bvw.tian-w.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rlk.yueranfly.top

[R77] 读取用户输入
来源：http://pep.zdqjudy.top

read -rp "请输入: " ans
来源：http://ilw.nanxuanxn.top

[R78] 交互式菜单
来源：http://sse.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://wxs.gzhubu.top

[R79] 解析命令行选项
来源：http://yci.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ovf.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://hus.yanxiufei.cn

time ./run.sh
来源：http://wwh.wangshuangyany.cn

================================================================================
来源：http://qnw.pycfn.com

S. C / C++ 专题
来源：http://rpd.redwolf501.top

================================================================================
来源：http://rex.ctjpmb.com

[S01] C：Hello World
来源：http://jwm.yueranfly.top

#include <stdio.h>
来源：http://txp.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://tvm.c1oappe.top

[S02] C：变量与格式化输出
来源：http://gol.jianghu66.top

int a = 10; printf("%d\n", a);
来源：http://qxf.fanxiaobao.xyz

[S03] C：读入整数
来源：http://hqr.ctjpmb.com

int x; scanf("%d", &x);
来源：http://dui.xingfuxueyuan.xyz

[S04] C：字符串复制
来源：http://qio.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://ojc.nanxuanxn.top

[S05] C：字符串长度
来源：http://csr.jiagoushi.top

strlen(s)
来源：http://trj.gotoacloud.top

[S06] C：字符串比较
来源：http://ydt.gzhubu.top

strcmp(a, b) == 0
来源：http://fga.chenzaomai.com

[S07] C：数组遍历求和
来源：http://qnw.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rqj.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://vgp.quarkkingdee.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ovh.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://yqm.tanke756.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nrb.guowangkeji.top

[S10] C：指针与解引用
来源：http://voq.havefunace.top

int *p = &a;  *p = 5;
来源：http://ooy.meibo888.top

[S11] C：逐行读文件
来源：http://orm.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://epw.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hxe.jinqigufen.top

fclose(f);
来源：http://fsw.cqqwz.cn

[S12] C：写文件
来源：http://sqp.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://saa.nwbrower.top

[S13] C：宏定义
来源：http://xca.cdnleiting.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://chj.iojbl.cn

[S14] C：枚举
来源：http://yoh.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://bmt.xinyue.icu

[S15] C：类型转换
来源：http://ybp.ctjpmb.com

(double) a / b
来源：http://cvy.bbcook.cn

[S16] C：位操作置位
来源：http://mny.redwolf501.top

x |= (1 << 3);
来源：http://yry.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://ztv.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jnw.sysykeji.top

[S18] C：命令行参数
来源：http://qhy.gaohongyu789.top

int main(int argc, char **argv)
来源：http://gei.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://yfa.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://pji.hongshengwenyu.top

[S20] C：二分查找
来源：http://kxt.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mlb.gotoacloud.top

[S21] C：字符类别判断
来源：http://edp.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rzc.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://njq.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://bdz.9152youxi.cn

[S23] C：随机数
来源：http://lrb.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://edj.sxryk.cn

[S24] C：获取本地时间
来源：http://yvf.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ltc.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://gdc.yongpay.top

memcpy(dst, src, n);
来源：http://puq.yvedp.cn

[S26] C：内存清零
来源：http://dba.yuanzhike.top

memset(a, 0, sizeof a);
来源：http://cpg.zhongyouzk.top

[S27] C：定义常量
来源：http://wln.xziqi.cn

const double PI = 3.14159;
来源：http://twb.zhongyouzk.top

[S28] C：静态变量
来源：http://sqi.vqdsnc.cn

static int counter = 0;
来源：http://dom.sufxvd.cn

[S29] C：变参函数
来源：http://ezl.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://thb.dashuyun.cn

[S30] C：头文件保护
来源：http://osn.zhixingplan.top

#ifndef X_H
来源：http://whb.yj20258.top

#define X_H
来源：http://vkb.fengsongda.top

#endif
来源：http://fsx.epnwcf.com

[S31] C++：Hello World
来源：http://pml.kuanghao11.cn

#include <iostream>
来源：http://twv.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://een.yangfankeji.com

[S32] C++：字符串
来源：http://rle.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://zao.ybcxt.top

[S33] C++：vector 增删
来源：http://div.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kfg.nanxinkj.top

[S34] C++：遍历 vector
来源：http://ofu.cqqwz.cn

for (auto &x : v) { std::cout << x; }
来源：http://hfb.zhaomingkeji.xyz

[S35] C++：map
来源：http://sef.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wtp.cucudq.cn

[S36] C++：unordered_map
来源：http://lvi.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://scr.zdbjq.cn

[S37] C++：set
来源：http://jfp.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lcn.haohaochexian.top

[S38] C++：排序
来源：http://poi.316326.xyz

std::sort(v.begin(), v.end());
来源：http://vwr.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://uzc.xingfuxueyuan.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jeq.nanxinkj.top

[S40] C++：查找元素
来源：http://vyr.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mfs.redwolf501.top

[S41] C++：类与构造函数
来源：http://zjk.tarul.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gof.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://fft.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://uga.0kj1m.cn

[S43] C++：智能指针
来源：http://rbu.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://woq.zhengqikj.top

[S44] C++：引用传参
来源：http://yna.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://ajt.9152youxi.cn

[S45] C++：lambda
来源：http://dqq.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://git.yuanzhike.top

[S46] C++：函数模板
来源：http://rfh.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ulq.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://vfj.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ooj.jiagoushi.top

[S48] C++：逐行读文件
来源：http://nkd.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ava.shanyushiyangtech.top

while (std::getline(in, line)) { }
来源：http://xlb.cqqwz.cn

[S49] C++：写文件
来源：http://ydg.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://urv.shzxlz.cn

[S50] C++：格式化数字
来源：http://rnt.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jnt.jinqigufen.top

[S51] C++：显式类型转换
来源：http://wwk.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://zoj.yonumen.top

[S52] C++：const 与 noexcept
来源：http://squ.yongpay.top

int size() const noexcept { return n_; }
来源：http://qxb.uphjek.com

[S53] C++：移动语义
来源：http://mtr.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://ugy.tian-w.cn

[S54] C++：异常处理
来源：http://rpc.wangdashe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zcl.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://znn.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kld.iojbl.cn

[S56] C++：optional
来源：http://ljm.ivvv.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jst.bjfxy.top

[S57] C++：编译期常量
来源：http://plp.pengpengdd.cyou

constexpr int N = 10;
来源：http://ton.hcnkem.com

[S58] C++：命名空间
来源：http://vbk.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://gca.aibaodan.cn

[S59] C++：静态断言
来源：http://jvf.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zrl.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://rvs.havefunace.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ott.smart0.xyz

================================================================================
来源：http://vki.shangyingyoupin.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ljp.gotoacloud.top

================================================================================
来源：http://hlo.shuidangran.top

[T01] Kotlin：Hello World
来源：http://xio.nwbrower.top

println("Hello")
来源：http://oov.ybcxt.top

[T02] Kotlin：变量
来源：http://dqu.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xuw.sysykeji.top

[T03] Kotlin：字符串模板
来源：http://kkg.zhixingplan.top

"值: $b"
来源：http://lna.tarul.cn

[T04] Kotlin：空安全
来源：http://cbu.jinqigfzy.top

val n: String? = null;  n?.length
来源：http://lda.sweek.top

[T05] Kotlin：when 表达式
来源：http://ddh.dashuyun.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uox.jqgufenzy.top

[T06] Kotlin：集合映射
来源：http://iai.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://rpz.yueranfly.top

[T07] Kotlin：集合过滤
来源：http://vyg.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mak.ehwqpu.com

[T08] Kotlin：数据类
来源：http://cyo.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://ofr.nwbrower.top

[T09] Kotlin：扩展函数
来源：http://bne.epnwcf.com

fun String.exclaim() = this + "!"
来源：http://nne.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://utz.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://piy.zhengqikj.top

[T11] Kotlin：协程
来源：http://ljf.tarul.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://aot.sxryk.cn

[T12] Kotlin：解构声明
来源：http://gpp.52xcode.cn

val (a, b) = Pair(1, 2)
来源：http://gdv.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://cqh.yangfankeji.com

val m = mapOf("a" to 1)
来源：http://mov.ivvv.top

[T14] Kotlin：循环
来源：http://mjq.jiagoushi.top

for (i in 1..10) println(i)
来源：http://cvg.ydjk.org.cn

[T15] Kotlin：接口
来源：http://yup.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://bgg.yj20258.top

[T16] Swift：Hello World
来源：http://rsv.pycfn.com

print("Hello")
来源：http://imn.sweek.top

[T17] Swift：变量与常量
来源：http://ygl.tian-w.cn

var a = 1;  let b = 2
来源：http://clu.sjlbkw.cn

[T18] Swift：字符串插值
来源：http://hiw.tanke756.top

"值: \(b)"
来源：http://vlt.sxryk.cn

[T19] Swift：可选绑定
来源：http://zik.xziqi.cn

if let n = opt { print(n) }
来源：http://gzd.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://ntw.jinghuilouyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hne.guannengcc.top

[T21] Swift：遍历
来源：http://gvq.ydzc1.top

for x in a { print(x) }
来源：http://pyu.xylfe.cn

[T22] Swift：字典
来源：http://drp.snrcjt.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rrw.sxryk.cn

[T23] Swift：函数
来源：http://gev.tarul.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://byd.sufxvd.cn

[T24] Swift：闭包
来源：http://uua.sufxvd.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xvz.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://gye.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://aas.yanxiufei.cn

[T26] Swift：类与重写
来源：http://nfh.xingfuxueyuan.xyz

class A: Base { override func f() {} }
来源：http://jht.pycfn.com

[T27] Swift：错误处理
来源：http://cmm.xinyue.icu

do { try f() } catch { print(error) }
来源：http://uxd.yfazqb.com

[T28] Swift：枚举
来源：http://fjf.uphjek.com

enum Color { case red, green }
来源：http://hsy.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://grw.gogol.net.cn

guard let x = opt else { return }
来源：http://kak.tian-w.cn

[T30] Swift：协议
来源：http://zky.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://hxx.wangdashe.top

[T31] Lua：Hello World
来源：http://cvu.hysaishi.cn

print("Hello")
来源：http://ysq.yonumen.top

[T32] Lua：局部变量
来源：http://dns.fehbvm.com

local a = 1
来源：http://tip.zycfv.cn

[T33] Lua：表（数组）
来源：http://xou.yj20258.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xwa.52xcode.cn

[T34] Lua：遍历表
来源：http://gqf.pengpengdd.cyou

for i, v in ipairs(t) do print(i, v) end
来源：http://dfk.jinghuilouyu.cn

[T35] Lua：字典表
来源：http://twe.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://btb.9152youxi.cn

[T36] Lua：函数
来源：http://oau.shangyingyoupin.top

function add(a, b) return a + b end
来源：http://awk.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://yyb.xinyue.icu

"a" .. "b"
来源：http://atl.meibo888.top

[T38] Lua：条件
来源：http://rcy.sxryk.cn

if x > 0 then print("正") end
来源：http://fbo.52xcode.cn

[T39] Lua：模式匹配
来源：http://ctn.vehdjk.com

string.find(s, "%d+")
来源：http://xvh.tianlin.xyz

[T40] Lua：元表
来源：http://vfs.xinyue.icu

setmetatable({}, { __index = base })
来源：http://hir.aibaodan.cn

[T41] Perl：Hello World
来源：http://nbk.shuidangran.top

print "Hello\n";
来源：http://gyt.xuetiantiany.cn

[T42] Perl：变量类型
来源：http://otu.aizwys.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://svu.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://njy.aizwys.cn

"值: $a"
来源：http://hpf.jinyuanbaomall.cn

[T44] Perl：条件
来源：http://hpd.yj20258.top

if ($a > 0) { print "正"; }
来源：http://jsd.vehdjk.com

[T45] Perl：数组遍历
来源：http://hiu.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://bdr.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://zge.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wpe.chenzaomai.com

[T47] Perl：正则捕获
来源：http://xpu.0kj1m.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ysy.tanke756.top

[T48] Perl：正则替换
来源：http://djy.ydzc1.top

$s =~ s/old/new/g;
来源：http://twn.shangyingyoupin.top

[T49] Perl：函数
来源：http://jaw.havefunace.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lwf.yuanzhike.top

[T50] Perl：逐行读文件
来源：http://jln.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://lni.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://uli.fehbvm.com

[T51] Scala：Hello World
来源：http://voy.zhoulong.xyz

println("Hello")
来源：http://rrc.jianghu66.top

[T52] Scala：变量
来源：http://ijg.tanke756.top

val a = 1;  var b = 2
来源：http://zrp.zhixingplan.top

[T53] Scala：字符串插值
来源：http://iis.zhixingplan.top

s"值: $b"
来源：http://mzi.zdbjq.cn

[T54] Scala：集合映射
来源：http://iyd.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://dcf.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://twt.chenjidiqi.icu

List(1, 2, 3).filter(_ > 1)
来源：http://fru.cucudq.cn

[T56] Scala：样例类
来源：http://tqv.chenzaomai.com

case class User(name: String, age: Int)
来源：http://krn.ehwqpu.com

[T57] Scala：模式匹配
来源：http://cqb.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nut.gaohongyu789.top

[T58] Scala：函数定义
来源：http://eef.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://xlz.zhijiandao.cn

[T59] Scala：循环
来源：http://wma.zhengqikj.top

for (i <- 1 to 10) println(i)
来源：http://rrr.sxryk.cn

[T60] Scala：折叠
来源：http://qsa.nanxinkj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mro.shanyushiyangtech.top

================================================================================
来源：http://pyf.ywan-chungtsiang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://akm.jinghuilouyu.cn

================================================================================
来源：http://rxt.xylfe.cn

[U01] Py：创建虚拟环境
来源：http://ajo.yuanzhike.top

python -m venv .venv && source .venv/bin/activate
来源：http://kdh.shangyingyoupin.top

[U02] Py：导出 / 安装依赖
来源：http://cgo.52xcode.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://por.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://agj.yfazqb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://ppv.tarul.cn

[U04] Py：变量调试打印
来源：http://erh.xinyue.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://haq.yueranfly.top

[U05] Py：列表去重且保序
来源：http://bsj.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://lrq.52xcode.cn

[U06] Py：合并两个字典
来源：http://ptq.yueranfly.top

{**a, **b}
来源：http://gga.yueranfly.top

[U07] Py：反转字典键值
来源：http://gwu.yueranfly.top

{v: k for k, v in d.items()}
来源：http://wdc.xingfuxueyuan.xyz

[U08] Py：展平二维列表
来源：http://jtr.yj202588.top

[y for x in nested for y in x]
来源：http://xax.shanyushiyangtech.top


<!-- 参考信息 -->