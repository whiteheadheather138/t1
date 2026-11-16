代发 wailian999

openssl rand -hex 16
来源：http://zkm.cashguo.top

[R68] 计算文件校验值
来源：http://lmf.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wfs.fengsongda.top

[R69] 生成随机密码
来源：http://ikm.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://oym.guowangkeji.top

[R70] 时间戳与互转
来源：http://vxx.nanxinkj.top

date +%s;  date -d @1700000000
来源：http://ekn.haohaochexian.top

[R71] 日期格式化
来源：http://ifo.redwolf501.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hen.smart0.xyz

[R72] 等待端口就绪
来源：http://ved.ivvv.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gfs.fengsongda.top

[R73] 分割大日志
来源：http://omf.316326.xyz

split -l 1000 big.log part_
来源：http://cci.cqqwz.cn

[R74] 批量重命名
来源：http://mbc.nanxuanxn.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yar.ctjpmb.com

[R75] 导出环境变量
来源：http://vwy.shanyushiyangtech.top

export PATH="$HOME/bin:$PATH"
来源：http://ymc.sxryk.cn

[R76] 使用临时文件
来源：http://ttx.yj20258888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zci.fengsongda.top

[R77] 读取用户输入
来源：http://tdz.hnqzz.top

read -rp "请输入: " ans
来源：http://qac.ydjk.org.cn

[R78] 交互式菜单
来源：http://kec.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://jld.yuxming.cn

[R79] 解析命令行选项
来源：http://khk.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mxm.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://ava.316326.xyz

time ./run.sh
来源：http://gsv.zhixingplan.top

================================================================================
来源：http://fye.uphjek.com

S. C / C++ 专题
来源：http://jxg.fengsongda.top

================================================================================
来源：http://vyf.jinqigufen.top

[S01] C：Hello World
来源：http://prv.aibaodan.cn

#include <stdio.h>
来源：http://ghw.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://brw.zycfv.cn

[S02] C：变量与格式化输出
来源：http://rno.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://jsj.xinyue.icu

[S03] C：读入整数
来源：http://djt.sufxvd.cn

int x; scanf("%d", &x);
来源：http://myb.yvedp.cn

[S04] C：字符串复制
来源：http://oua.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nlq.jianghu66.top

[S05] C：字符串长度
来源：http://xmp.redwolf501.top

strlen(s)
来源：http://dee.smart0.xyz

[S06] C：字符串比较
来源：http://ivj.tanke756.top

strcmp(a, b) == 0
来源：http://gom.zhongyouzk.top

[S07] C：数组遍历求和
来源：http://zeu.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xbr.havefunace.top

[S08] C：动态内存分配与释放
来源：http://rhc.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iqx.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://pco.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vqx.ydzc1.top

[S10] C：指针与解引用
来源：http://mip.cheryme.top

int *p = &a;  *p = 5;
来源：http://ans.ctjpmb.com

[S11] C：逐行读文件
来源：http://nyk.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://fvn.zhengqikj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ttt.yj20258.top

fclose(f);
来源：http://emc.shanyushiyangtech.top

[S12] C：写文件
来源：http://ajg.dashuyun.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ztr.cashguo.top

[S13] C：宏定义
来源：http://jgt.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nkc.xinyue.icu

[S14] C：枚举
来源：http://cjw.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://bkd.c1oappe.top

[S15] C：类型转换
来源：http://vvj.yongpay.top

(double) a / b
来源：http://cxa.ivvv.top

[S16] C：位操作置位
来源：http://ify.jinqigfzy.top

x |= (1 << 3);
来源：http://bdq.sysykeji.top

[S17] C：安全拼接字符串
来源：http://viv.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ffs.yj20258.top

[S18] C：命令行参数
来源：http://txj.jiagoushi.top

int main(int argc, char **argv)
来源：http://yxw.meibo888.top

[S19] C：快速排序
来源：http://rjj.nanxinkj.top

qsort(a, n, sizeof(int), cmp);
来源：http://iew.hysaishi.cn

[S20] C：二分查找
来源：http://rng.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mcz.jyoumei.cn

[S21] C：字符类别判断
来源：http://tfk.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xhq.xinyue.icu

[S22] C：字符串转数字
来源：http://pra.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://shc.zhengqikj.top

[S23] C：随机数
来源：http://qww.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sxq.yongpay.top

[S24] C：获取本地时间
来源：http://olt.cucudq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://moq.shuidangran.top

[S25] C：内存拷贝
来源：http://jgc.zhijiandao.cn

memcpy(dst, src, n);
来源：http://snq.yanxiufei.cn

[S26] C：内存清零
来源：http://psf.52xcode.cn

memset(a, 0, sizeof a);
来源：http://drx.cqqwz.cn

[S27] C：定义常量
来源：http://lxt.gogol.net.cn

const double PI = 3.14159;
来源：http://cjm.chenlongwang.top

[S28] C：静态变量
来源：http://qip.yonumen.top

static int counter = 0;
来源：http://ctm.zhongyouzk.top

[S29] C：变参函数
来源：http://ywz.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ryu.c1oappe.top

[S30] C：头文件保护
来源：http://wvs.xziqi.cn

#ifndef X_H
来源：http://psr.birdmap.top

#define X_H
来源：http://old.zhongyouzk.top

#endif
来源：http://zlm.dianchejie.cn

[S31] C++：Hello World
来源：http://uxs.quarkkingdee.top

#include <iostream>
来源：http://mvi.chenzaomai.com

int main() { std::cout << "Hello\n"; }
来源：http://urp.nwbrower.top

[S32] C++：字符串
来源：http://aao.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://yck.316326.xyz

[S33] C++：vector 增删
来源：http://oxb.bjfxy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zvm.yuanzhike.top

[S34] C++：遍历 vector
来源：http://qjh.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://tgg.xziqi.cn

[S35] C++：map
来源：http://yhk.sweek.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ecj.zhongyouzk.top

[S36] C++：unordered_map
来源：http://mcs.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vdc.9152youxi.cn

[S37] C++：set
来源：http://zet.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zfv.hnqzz.top

[S38] C++：排序
来源：http://qnf.meibo888.top

std::sort(v.begin(), v.end());
来源：http://vlb.ybcxt.top

[S39] C++：自定义比较器排序
来源：http://bte.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zyu.xuanzx.com

[S40] C++：查找元素
来源：http://arw.hysaishi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mvv.xylfe.cn

[S41] C++：类与构造函数
来源：http://wnh.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rxx.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://zto.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://irs.shzxlz.cn

[S43] C++：智能指针
来源：http://zfz.haohaochexian.top

auto p = std::make_unique<int>(5);
来源：http://guh.yongpay.top

[S44] C++：引用传参
来源：http://hob.yvedp.cn

void inc(int &x) { ++x; }
来源：http://aee.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://hen.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://cfk.epnwcf.com

[S46] C++：函数模板
来源：http://aqc.yongpay.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jmh.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://mcr.ctjpmb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mgw.ctjpmb.com

[S48] C++：逐行读文件
来源：http://xcp.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tvh.yuxming.cn

while (std::getline(in, line)) { }
来源：http://zdb.zhengqikj.top

[S49] C++：写文件
来源：http://vyp.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oqe.hfpthk.cn

[S50] C++：格式化数字
来源：http://hni.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://csx.shanyushiyangkeji.top

[S51] C++：显式类型转换
来源：http://zcg.bjfxy.top

static_cast<double>(a) / b
来源：http://slw.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://rll.sysykeji.top

int size() const noexcept { return n_; }
来源：http://qql.hcnkem.com

[S53] C++：移动语义
来源：http://wod.ywan-chungtsiang.top

std::vector<int> w = std::move(v);
来源：http://ncx.hysaishi.cn

[S54] C++：异常处理
来源：http://ypa.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lue.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://jgr.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lqh.hammf.cn

[S56] C++：optional
来源：http://aql.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ipw.nanxinkj.top

[S57] C++：编译期常量
来源：http://lme.yanxiufei.cn

constexpr int N = 10;
来源：http://ciz.yanxiufei.cn

[S58] C++：命名空间
来源：http://tmf.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://evb.shuidangran.top

[S59] C++：静态断言
来源：http://gsq.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yvk.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://nmr.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zbd.iojbl.cn

================================================================================
来源：http://atj.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jjk.meibo888.top

================================================================================
来源：http://qbs.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://onz.sxryk.cn

println("Hello")
来源：http://muh.yueranfly.top

[T02] Kotlin：变量
来源：http://nil.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uhk.pycfn.com

[T03] Kotlin：字符串模板
来源：http://mpz.gogol.net.cn

"值: $b"
来源：http://wue.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://jcj.tian-w.cn

val n: String? = null;  n?.length
来源：http://sku.xziqi.cn

[T05] Kotlin：when 表达式
来源：http://dfk.tanke756.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dzc.fktsv.cn

[T06] Kotlin：集合映射
来源：http://aha.fzhhl.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qho.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://fmo.wangdashe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sbl.ctjpmb.com

[T08] Kotlin：数据类
来源：http://lxn.uphjek.com

data class User(val name: String, val age: Int)
来源：http://ufv.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://vcu.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://fjb.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://rli.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ocf.zdqjudy.top

[T11] Kotlin：协程
来源：http://ytd.xinyue.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://ixb.uphjek.com

[T12] Kotlin：解构声明
来源：http://nhr.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://ifs.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://efv.chenlongwang.top

val m = mapOf("a" to 1)
来源：http://aea.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://vur.tarul.cn

for (i in 1..10) println(i)
来源：http://jbk.hysaishi.cn

[T15] Kotlin：接口
来源：http://ppa.zhijiandao.cn

interface Shape { fun area(): Double }
来源：http://jad.epnwcf.com

[T16] Swift：Hello World
来源：http://xtd.tanke756.top

print("Hello")
来源：http://sew.ivvv.top

[T17] Swift：变量与常量
来源：http://lkz.ctjpmb.com

var a = 1;  let b = 2
来源：http://ezd.52xcode.cn

[T18] Swift：字符串插值
来源：http://jyz.ydzc1.top

"值: \(b)"
来源：http://qsr.yangfankeji.com

[T19] Swift：可选绑定
来源：http://zmo.jlsjyb.cn

if let n = opt { print(n) }
来源：http://cjb.zhixingplan.top

[T20] Swift：数组操作
来源：http://lxn.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zep.xziqi.cn

[T21] Swift：遍历
来源：http://uda.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://ihw.ivvv.top

[T22] Swift：字典
来源：http://yhp.jianghu66.top

var d = ["a": 1];  d["b"] = 2
来源：http://ewb.sysykeji.top

[T23] Swift：函数
来源：http://cvv.hnxiangtu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gby.hammf.cn

[T24] Swift：闭包
来源：http://yjh.cashguo.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tsj.xinyue.icu

[T25] Swift：结构体
来源：http://qjz.birdmap.top

struct P { var x: Int }
来源：http://oga.svipenyu.cn

[T26] Swift：类与重写
来源：http://vlx.fktsv.cn

class A: Base { override func f() {} }
来源：http://itz.tanke756.top

[T27] Swift：错误处理
来源：http://xas.ydzc1.top

do { try f() } catch { print(error) }
来源：http://fcf.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://nbe.dianchejie.cn

enum Color { case red, green }
来源：http://evf.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://gad.zhijiandao.cn

guard let x = opt else { return }
来源：http://jsv.yuanzhike.top

[T30] Swift：协议
来源：http://mxf.fzhhl.top

protocol Shape { func area() -> Double }
来源：http://twe.hywenlv.cn

[T31] Lua：Hello World
来源：http://pnt.jinghuilouyu.cn

print("Hello")
来源：http://hcn.yonumen.top

[T32] Lua：局部变量
来源：http://glz.aizwys.cn

local a = 1
来源：http://wrm.xziqi.cn

[T33] Lua：表（数组）
来源：http://dee.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fyy.tianlin.xyz

[T34] Lua：遍历表
来源：http://tlm.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pvk.yonumen.top

[T35] Lua：字典表
来源：http://rbv.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://zgu.jinyuanbaomall.cn

[T36] Lua：函数
来源：http://hhg.cucudq.cn

function add(a, b) return a + b end
来源：http://kjj.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://oui.gotoacloud.top

"a" .. "b"
来源：http://liv.svipenyu.cn

[T38] Lua：条件
来源：http://hxe.fktsv.cn

if x > 0 then print("正") end
来源：http://esk.hfpthk.cn

[T39] Lua：模式匹配
来源：http://dhj.hnxiangtu.top

string.find(s, "%d+")
来源：http://mih.tian-w.cn

[T40] Lua：元表
来源：http://sty.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://pzn.fktsv.cn

[T41] Perl：Hello World
来源：http://jku.bjfxy.top

print "Hello\n";
来源：http://lcs.gaohongyu789.top

[T42] Perl：变量类型
来源：http://pns.gzhubu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xrj.uphjek.com

[T43] Perl：字符串插值
来源：http://ufn.chenjidiqi.icu

"值: $a"
来源：http://kai.haohaochexian.top

[T44] Perl：条件
来源：http://vcx.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://eem.shuidangran.top

[T45] Perl：数组遍历
来源：http://vcu.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://auy.gogol.net.cn

[T46] Perl：哈希操作
来源：http://skb.havefunace.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cbx.yueranfly.top

[T47] Perl：正则捕获
来源：http://avz.fengsongda.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://usx.aibaodan.cn

[T48] Perl：正则替换
来源：http://xfn.gaohongyu789.top

$s =~ s/old/new/g;
来源：http://wfu.chenlongwang.top

[T49] Perl：函数
来源：http://vvh.gzhubu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gnl.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://ncc.0kj1m.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cij.hcnkem.com

while (my $line = <$fh>) { print $line; }
来源：http://svb.andypj.xyz

[T51] Scala：Hello World
来源：http://vzj.xylfe.cn

println("Hello")
来源：http://wbi.nanxuanxn.top

[T52] Scala：变量
来源：http://ngt.316326.xyz

val a = 1;  var b = 2
来源：http://qmy.jianghu66.top

[T53] Scala：字符串插值
来源：http://cob.zhongyouzk.top

s"值: $b"
来源：http://luy.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://hav.tianlin.xyz

List(1, 2, 3).map(_ * 2)
来源：http://eum.9152youxi.cn

[T55] Scala：集合过滤
来源：http://zzu.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://jxe.xuetiantiany.cn

[T56] Scala：样例类
来源：http://tyw.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://ldr.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://dtd.yangfankeji.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://vwm.yj20258.top

[T58] Scala：函数定义
来源：http://oam.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://eud.shuidangran.top

[T59] Scala：循环
来源：http://uny.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://gmq.cheryme.top

[T60] Scala：折叠
来源：http://puh.yanxiufei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yrj.hcnkem.com

================================================================================
来源：http://tbx.sweek.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lvk.nanxinkj.top

================================================================================
来源：http://eio.zhiwuduotai.top

[U01] Py：创建虚拟环境
来源：http://gba.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bhw.fktsv.cn

[U02] Py：导出 / 安装依赖
来源：http://qlx.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rni.hesvh.cn

[U03] Py：加载 .env 配置
来源：http://kqh.nanxinkj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pir.yj202588.top

[U04] Py：变量调试打印
来源：http://flw.ydzc1.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xlo.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://wan.yj20258888.top

list(dict.fromkeys(arr))
来源：http://lry.shuidangran.top

[U06] Py：合并两个字典
来源：http://ghm.jianghu66.top

{**a, **b}
来源：http://zlj.ydzc1.top

[U07] Py：反转字典键值
来源：http://rsa.sufxvd.cn

{v: k for k, v in d.items()}
来源：http://dzb.zhoulong.xyz

[U08] Py：展平二维列表
来源：http://ojd.bbcook.cn

[y for x in nested for y in x]
来源：http://ige.yj20258.top


<!-- 参考信息 -->