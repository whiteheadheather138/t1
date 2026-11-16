代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://qoy.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://qgt.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://qww.fzhhl.top

[R71] 日期格式化
来源：http://gzk.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://iwv.redwolf501.top

[R72] 等待端口就绪
来源：http://gir.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://yrv.gogol.net.cn

[R73] 分割大日志
来源：http://qrn.jinqigfzy.top

split -l 1000 big.log part_
来源：http://jke.meibo888.top

[R74] 批量重命名
来源：http://yyc.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iwo.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://nyn.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://tuh.316326.xyz

[R76] 使用临时文件
来源：http://eoz.nanxinkj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://atn.feifeiyinyue.top

[R77] 读取用户输入
来源：http://syk.sweek.top

read -rp "请输入: " ans
来源：http://azr.tarul.cn

[R78] 交互式菜单
来源：http://mrn.chenzaomai.com

select opt in a b c; do echo "$opt"; break; done
来源：http://rsa.wangdashe.top

[R79] 解析命令行选项
来源：http://fhb.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://phr.dianchejie.cn

[R80] 查看脚本执行耗时
来源：http://fkl.fanxiaobao.xyz

time ./run.sh
来源：http://bfv.52xcode.cn

================================================================================
来源：http://vmb.havefunace.top

S. C / C++ 专题
来源：http://hsb.xuanzx.com

================================================================================
来源：http://cbb.yvedp.cn

[S01] C：Hello World
来源：http://zdx.quarkkingdee.top

#include <stdio.h>
来源：http://lyb.hongshengwenyu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nut.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://qfs.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://zqs.yfazqb.com

[S03] C：读入整数
来源：http://aiw.fehbvm.com

int x; scanf("%d", &x);
来源：http://cnw.jiagoushi.top

[S04] C：字符串复制
来源：http://ner.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://qij.gaohongyu789.top

[S05] C：字符串长度
来源：http://miz.chenlongwang.top

strlen(s)
来源：http://ugo.jianghu66.top

[S06] C：字符串比较
来源：http://yjs.tanke756.top

strcmp(a, b) == 0
来源：http://flr.zdbjq.cn

[S07] C：数组遍历求和
来源：http://lfy.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ipr.ivvv.top

[S08] C：动态内存分配与释放
来源：http://gfn.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ths.nanxinkj.top

[S09] C：结构体定义与初始化
来源：http://apz.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://moi.sjlbkw.cn

[S10] C：指针与解引用
来源：http://szm.daria6918.cn

int *p = &a;  *p = 5;
来源：http://sql.jiagoushi.top

[S11] C：逐行读文件
来源：http://icy.9152youxi.cn

FILE *f = fopen("a.txt", "r");
来源：http://efb.shanyushiyangtech.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wtt.quarkkingdee.top

fclose(f);
来源：http://eck.sufxvd.cn

[S12] C：写文件
来源：http://fjj.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qea.gotoacloud.top

[S13] C：宏定义
来源：http://xzw.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bre.sjlbkw.cn

[S14] C：枚举
来源：http://hyx.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://ykn.yongpay.top

[S15] C：类型转换
来源：http://enb.daria6918.cn

(double) a / b
来源：http://ogg.ehwqpu.com

[S16] C：位操作置位
来源：http://ihu.ydzc1.top

x |= (1 << 3);
来源：http://itw.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://jfe.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tqu.vehdjk.com

[S18] C：命令行参数
来源：http://bvv.c1oappe.top

int main(int argc, char **argv)
来源：http://cnt.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://rgy.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yuz.zhongyouzk.top

[S20] C：二分查找
来源：http://dqm.pycfn.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vsx.zhongyouzk.top

[S21] C：字符类别判断
来源：http://buf.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://icf.jlsjyb.cn

[S22] C：字符串转数字
来源：http://stv.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://pim.c1oappe.top

[S23] C：随机数
来源：http://ahg.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xge.pengpengdd.cyou

[S24] C：获取本地时间
来源：http://aiw.xinyue.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ohu.daxiang520.top

[S25] C：内存拷贝
来源：http://sni.zhoulong.xyz

memcpy(dst, src, n);
来源：http://qjp.yj20258888.top

[S26] C：内存清零
来源：http://aex.pycfn.com

memset(a, 0, sizeof a);
来源：http://yom.zdqjudy.top

[S27] C：定义常量
来源：http://unp.hnqzz.top

const double PI = 3.14159;
来源：http://myk.shzxlz.cn

[S28] C：静态变量
来源：http://yii.smart0.xyz

static int counter = 0;
来源：http://eyr.fktsv.cn

[S29] C：变参函数
来源：http://ckf.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kvd.havefunace.top

[S30] C：头文件保护
来源：http://fhl.xylfe.cn

#ifndef X_H
来源：http://zvm.52xcode.cn

#define X_H
来源：http://boq.zhoulong.xyz

#endif
来源：http://rgk.smart0.xyz

[S31] C++：Hello World
来源：http://rts.jyoumei.cn

#include <iostream>
来源：http://lzh.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://zxa.nwbrower.top

[S32] C++：字符串
来源：http://ewi.9152youxi.cn

std::string s = "hi";  s += "!";
来源：http://pkf.gzhubu.top

[S33] C++：vector 增删
来源：http://uhz.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ptg.bjfxy.top

[S34] C++：遍历 vector
来源：http://ttx.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://alv.vqdsnc.cn

[S35] C++：map
来源：http://kqt.shangyingyoupin.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vpx.guannengcc.top

[S36] C++：unordered_map
来源：http://zlt.yueranfly.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qor.nanxuanxn.top

[S37] C++：set
来源：http://uas.zdbjq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yyh.tian-w.cn

[S38] C++：排序
来源：http://ttz.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://vom.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://jpj.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oxn.kuanghao11.cn

[S40] C++：查找元素
来源：http://xaq.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dde.jqgfzy.top

[S41] C++：类与构造函数
来源：http://ryw.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://weh.meibo888.top

[S42] C++：继承与虚函数
来源：http://hvs.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://tpu.fzhhl.top

[S43] C++：智能指针
来源：http://vzp.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://fqd.mhx1999.top

[S44] C++：引用传参
来源：http://mxk.gotoacloud.top

void inc(int &x) { ++x; }
来源：http://oeb.chenzaomai.com

[S45] C++：lambda
来源：http://mnj.aibaodan.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hvz.zhoulong.xyz

[S46] C++：函数模板
来源：http://wen.sufxvd.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cmf.zhoulong.xyz

[S47] C++：结构化绑定遍历
来源：http://fpd.wangshuangyany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ajq.epnwcf.com

[S48] C++：逐行读文件
来源：http://qrw.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vuv.shuidangran.top

while (std::getline(in, line)) { }
来源：http://mgg.sufxvd.cn

[S49] C++：写文件
来源：http://xeq.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bvk.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://wjj.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ena.jiagoushi.top

[S51] C++：显式类型转换
来源：http://gky.sysykeji.top

static_cast<double>(a) / b
来源：http://zua.xinyue.icu

[S52] C++：const 与 noexcept
来源：http://bxj.cashguo.top

int size() const noexcept { return n_; }
来源：http://enr.tarul.cn

[S53] C++：移动语义
来源：http://hvx.shzxlz.cn

std::vector<int> w = std::move(v);
来源：http://tng.ctjpmb.com

[S54] C++：异常处理
来源：http://eei.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vli.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://fys.tanke756.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mkp.pengpengdd.cyou

[S56] C++：optional
来源：http://khz.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hph.jlsjyb.cn

[S57] C++：编译期常量
来源：http://tss.hysaishi.cn

constexpr int N = 10;
来源：http://oke.yueranfly.top

[S58] C++：命名空间
来源：http://bes.ydzc1.top

namespace ns { int f() { return 1; } }
来源：http://hbn.fengsongda.top

[S59] C++：静态断言
来源：http://bgj.jinqigufen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rvr.yonumen.top

[S60] C++：遍历并删除元素
来源：http://sju.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aab.yongpay.top

================================================================================
来源：http://sqz.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://onk.zhiwuduotai.top

================================================================================
来源：http://ycf.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://tii.guowangkeji.top

println("Hello")
来源：http://xor.epnwcf.com

[T02] Kotlin：变量
来源：http://qyo.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eyb.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://wjd.kuanghao11.cn

"值: $b"
来源：http://jrc.pycfn.com

[T04] Kotlin：空安全
来源：http://cqn.shangyingyoupin.top

val n: String? = null;  n?.length
来源：http://waf.yj20258.top

[T05] Kotlin：when 表达式
来源：http://rsy.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qlw.gaohongyu789.top

[T06] Kotlin：集合映射
来源：http://fmf.pycfn.com

listOf(1, 2, 3).map { it * 2 }
来源：http://epc.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://luq.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gmc.sweek.top

[T08] Kotlin：数据类
来源：http://efy.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://sbd.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://idn.yonumen.top

fun String.exclaim() = this + "!"
来源：http://irm.ydjk.org.cn

[T10] Kotlin：默认参数
来源：http://cwk.gotoacloud.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qan.yvedp.cn

[T11] Kotlin：协程
来源：http://rud.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mfi.andypj.xyz

[T12] Kotlin：解构声明
来源：http://cbh.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://duk.haohaochexian.top

[T13] Kotlin：只读 Map
来源：http://xbx.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://gji.zdbjq.cn

[T14] Kotlin：循环
来源：http://xqk.xylfe.cn

for (i in 1..10) println(i)
来源：http://mcf.ydjk.org.cn

[T15] Kotlin：接口
来源：http://uws.pengpengdd.cyou

interface Shape { fun area(): Double }
来源：http://bco.zdqjudy.top

[T16] Swift：Hello World
来源：http://cyj.xylfe.cn

print("Hello")
来源：http://mxg.nanxinkj.top

[T17] Swift：变量与常量
来源：http://iiz.bbcook.cn

var a = 1;  let b = 2
来源：http://wjg.nwbrower.top

[T18] Swift：字符串插值
来源：http://thf.dianchejie.cn

"值: \(b)"
来源：http://hhu.jinqigufen.top

[T19] Swift：可选绑定
来源：http://jfr.gzhubu.top

if let n = opt { print(n) }
来源：http://eld.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://dwk.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ejd.meibo888.top

[T21] Swift：遍历
来源：http://hzk.iojbl.cn

for x in a { print(x) }
来源：http://alr.316326.xyz

[T22] Swift：字典
来源：http://bka.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://vyp.daxiang520.top

[T23] Swift：函数
来源：http://sgr.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kkl.sweek.top

[T24] Swift：闭包
来源：http://rje.xylfe.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://byd.dashuyun.cn

[T25] Swift：结构体
来源：http://ozp.jinqigufen.top

struct P { var x: Int }
来源：http://mzt.meibo888.top

[T26] Swift：类与重写
来源：http://mny.hfpthk.cn

class A: Base { override func f() {} }
来源：http://nht.fktsv.cn

[T27] Swift：错误处理
来源：http://ddn.vqdsnc.cn

do { try f() } catch { print(error) }
来源：http://xhw.9152youxi.cn

[T28] Swift：枚举
来源：http://hau.guowangkeji.top

enum Color { case red, green }
来源：http://nox.ivvv.top

[T29] Swift：guard 提前返回
来源：http://rik.yuxming.cn

guard let x = opt else { return }
来源：http://ntc.ehwqpu.com

[T30] Swift：协议
来源：http://pux.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://mta.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://poz.chenzaomai.com

print("Hello")
来源：http://zrl.mhx1999.top

[T32] Lua：局部变量
来源：http://bou.zdbjq.cn

local a = 1
来源：http://qns.yuanzhike.top

[T33] Lua：表（数组）
来源：http://vrj.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jtw.iojbl.cn

[T34] Lua：遍历表
来源：http://qlf.xuanzx.com

for i, v in ipairs(t) do print(i, v) end
来源：http://tau.jyoumei.cn

[T35] Lua：字典表
来源：http://kad.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://wru.zhoulong.xyz

[T36] Lua：函数
来源：http://lvp.jinghuilouyu.cn

function add(a, b) return a + b end
来源：http://wod.ybcxt.top

[T37] Lua：字符串拼接
来源：http://rem.jinqigufen.top

"a" .. "b"
来源：http://mqp.tarul.cn

[T38] Lua：条件
来源：http://mqm.zhijiandao.cn

if x > 0 then print("正") end
来源：http://byo.jiagoushi.top

[T39] Lua：模式匹配
来源：http://wmf.gaohongyu789.top

string.find(s, "%d+")
来源：http://ywj.fktsv.cn

[T40] Lua：元表
来源：http://jsy.nwbrower.top

setmetatable({}, { __index = base })
来源：http://ias.dianchejie.cn

[T41] Perl：Hello World
来源：http://vja.birdmap.top

print "Hello\n";
来源：http://xdc.hammf.cn

[T42] Perl：变量类型
来源：http://vcn.jinghuilouyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yud.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://hhe.bjfxy.top

"值: $a"
来源：http://oke.dianchejie.cn

[T44] Perl：条件
来源：http://xlx.316326.xyz

if ($a > 0) { print "正"; }
来源：http://zyk.yuanzhike.top

[T45] Perl：数组遍历
来源：http://tyo.quarkkingdee.top

for my $x (@arr) { print $x; }
来源：http://yjf.bjfxy.top

[T46] Perl：哈希操作
来源：http://fqf.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rnx.zhixingplan.top

[T47] Perl：正则捕获
来源：http://his.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jfp.yuanzhike.top

[T48] Perl：正则替换
来源：http://tuc.hysaishi.cn

$s =~ s/old/new/g;
来源：http://rdd.hongshengwenyu.top

[T49] Perl：函数
来源：http://ded.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zhn.vqdsnc.cn

[T50] Perl：逐行读文件
来源：http://baz.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mxn.quarkkingdee.top

while (my $line = <$fh>) { print $line; }
来源：http://jhh.zhongyouzk.top

[T51] Scala：Hello World
来源：http://lzq.tian-w.cn

println("Hello")
来源：http://tjj.sufxvd.cn

[T52] Scala：变量
来源：http://xlj.fengsongda.top

val a = 1;  var b = 2
来源：http://jeu.zhixingplan.top

[T53] Scala：字符串插值
来源：http://uzu.jqgufenzy.top

s"值: $b"
来源：http://kfn.nanxinkj.top

[T54] Scala：集合映射
来源：http://mqd.chenzaomai.com

List(1, 2, 3).map(_ * 2)
来源：http://csw.jqgfzy.top

[T55] Scala：集合过滤
来源：http://rek.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sux.daria6918.cn

[T56] Scala：样例类
来源：http://txx.uphjek.com

case class User(name: String, age: Int)
来源：http://exw.52xcode.cn

[T57] Scala：模式匹配
来源：http://pup.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://bqo.jinqigfzy.top

[T58] Scala：函数定义
来源：http://kwa.yuanzhike.top

def add(a: Int, b: Int): Int = a + b
来源：http://dup.tarul.cn

[T59] Scala：循环
来源：http://vhl.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://cnb.redwolf501.top

[T60] Scala：折叠
来源：http://njh.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dwn.9152youxi.cn

================================================================================
来源：http://upn.fanxiaobao.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rhx.hammf.cn

================================================================================
来源：http://yfz.gaohongyu789.top

[U01] Py：创建虚拟环境
来源：http://hiv.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lci.shangyingyoupin.top

[U02] Py：导出 / 安装依赖
来源：http://cty.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tkx.yanxiufei.cn

[U03] Py：加载 .env 配置
来源：http://xyy.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://jpl.chenlongwang.top

[U04] Py：变量调试打印
来源：http://iev.mhx1999.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://izk.ehwqpu.com

[U05] Py：列表去重且保序
来源：http://viu.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://dfi.wangshuangyany.cn

[U06] Py：合并两个字典
来源：http://dgi.guannengcc.top

{**a, **b}
来源：http://cdj.ivvv.top

[U07] Py：反转字典键值
来源：http://svr.aibaodan.cn

{v: k for k, v in d.items()}
来源：http://ksn.jqgufenzy.top

[U08] Py：展平二维列表
来源：http://iaa.ehwqpu.com

[y for x in nested for y in x]
来源：http://omx.ivvv.top

[U09] Py：字典取最大值的键
来源：http://nce.ydzc1.top

max(d, key=d.get)
来源：http://zkk.sysykeji.top

[U10] Py：按值排序字典
来源：http://ptf.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kog.sweek.top


<!-- 参考信息 -->