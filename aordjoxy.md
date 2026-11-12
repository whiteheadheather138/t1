代发 wailian999

split -l 1000 big.log part_
来源：http://ray.yongpay.top

[R74] 批量重命名
来源：http://kdt.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rmy.zycfv.cn

[R75] 导出环境变量
来源：http://fzi.fengsongda.top

export PATH="$HOME/bin:$PATH"
来源：http://hen.epnwcf.com

[R76] 使用临时文件
来源：http://msh.ehwqpu.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xft.yvedp.cn

[R77] 读取用户输入
来源：http://vyj.yfazqb.com

read -rp "请输入: " ans
来源：http://bfu.cdnleiting.top

[R78] 交互式菜单
来源：http://qtk.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iyb.cdnleiting.top

[R79] 解析命令行选项
来源：http://dkm.xziqi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ija.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://oxh.andypj.xyz

time ./run.sh
来源：http://tnv.fanxiaobao.xyz

================================================================================
来源：http://rro.yonumen.top

S. C / C++ 专题
来源：http://say.yonumen.top

================================================================================
来源：http://rqp.sysykeji.top

[S01] C：Hello World
来源：http://thh.hnqzz.top

#include <stdio.h>
来源：http://pdn.meibo888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ikp.fanxiaobao.xyz

[S02] C：变量与格式化输出
来源：http://mzo.bjfxy.top

int a = 10; printf("%d\n", a);
来源：http://wdy.nanxinkj.top

[S03] C：读入整数
来源：http://ett.hysaishi.cn

int x; scanf("%d", &x);
来源：http://mwa.yanxiufei.cn

[S04] C：字符串复制
来源：http://mbw.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://ixg.nanxinkj.top

[S05] C：字符串长度
来源：http://vwm.yj20258888.top

strlen(s)
来源：http://yph.tarul.cn

[S06] C：字符串比较
来源：http://yqo.zhoulong.xyz

strcmp(a, b) == 0
来源：http://iif.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://odk.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eov.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://hxb.316326.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gtp.ivvv.top

[S09] C：结构体定义与初始化
来源：http://jsf.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pqk.tian-w.cn

[S10] C：指针与解引用
来源：http://njy.xuanzx.com

int *p = &a;  *p = 5;
来源：http://lag.yueranfly.top

[S11] C：逐行读文件
来源：http://oqr.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://snl.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kcg.vqdsnc.cn

fclose(f);
来源：http://pne.yuxming.cn

[S12] C：写文件
来源：http://erj.xinyue.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qzf.sweek.top

[S13] C：宏定义
来源：http://fqu.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://shc.zhoulong.xyz

[S14] C：枚举
来源：http://odx.pengpengdd.cyou

enum Color { RED, GREEN, BLUE };
来源：http://ihq.snrcjt.cn

[S15] C：类型转换
来源：http://vvk.fehbvm.com

(double) a / b
来源：http://doq.cdnleiting.top

[S16] C：位操作置位
来源：http://nlt.hnqzz.top

x |= (1 << 3);
来源：http://srl.daxiang520.top

[S17] C：安全拼接字符串
来源：http://bby.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bnf.c1oappe.top

[S18] C：命令行参数
来源：http://ymq.yuanzhike.top

int main(int argc, char **argv)
来源：http://bjl.aibaodan.cn

[S19] C：快速排序
来源：http://cpn.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hzo.hcnkem.com

[S20] C：二分查找
来源：http://wtp.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fqv.zdqjudy.top

[S21] C：字符类别判断
来源：http://vyw.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ofc.kuanghao11.cn

[S22] C：字符串转数字
来源：http://xwk.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mar.havefunace.top

[S23] C：随机数
来源：http://ccv.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://sqe.zhengqikj.top

[S24] C：获取本地时间
来源：http://rfa.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hba.nanxinkj.top

[S25] C：内存拷贝
来源：http://syu.cheryme.top

memcpy(dst, src, n);
来源：http://von.cheryme.top

[S26] C：内存清零
来源：http://jwo.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://bwz.yuxming.cn

[S27] C：定义常量
来源：http://gvk.0kj1m.cn

const double PI = 3.14159;
来源：http://ngq.nanxinkj.top

[S28] C：静态变量
来源：http://deb.iojbl.cn

static int counter = 0;
来源：http://yhx.ybcxt.top

[S29] C：变参函数
来源：http://trb.ehwqpu.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lxv.chenjidiqi.icu

[S30] C：头文件保护
来源：http://iuu.bjfxy.top

#ifndef X_H
来源：http://vjd.tanke756.top

#define X_H
来源：http://bdg.sufxvd.cn

#endif
来源：http://sti.vqdsnc.cn

[S31] C++：Hello World
来源：http://spf.zycfv.cn

#include <iostream>
来源：http://atu.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://xmm.zhaomingkeji.xyz

[S32] C++：字符串
来源：http://vqw.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://hdb.sjlbkw.cn

[S33] C++：vector 增删
来源：http://qlu.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zjo.gogol.net.cn

[S34] C++：遍历 vector
来源：http://lkd.zdqjudy.top

for (auto &x : v) { std::cout << x; }
来源：http://tuu.cheryme.top

[S35] C++：map
来源：http://omn.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sip.uphjek.com

[S36] C++：unordered_map
来源：http://tvv.jinyuanbaomall.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bvw.vehdjk.com

[S37] C++：set
来源：http://qui.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xrn.sjlbkw.cn

[S38] C++：排序
来源：http://sta.jqgfzy.top

std::sort(v.begin(), v.end());
来源：http://iqe.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://elz.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ufg.gzhubu.top

[S40] C++：查找元素
来源：http://ylk.daria6918.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cue.fengsongda.top

[S41] C++：类与构造函数
来源：http://hpg.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xrz.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://lrr.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://wzw.xinyue.icu

[S43] C++：智能指针
来源：http://mpb.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://kli.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://wgk.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://idd.iojbl.cn

[S45] C++：lambda
来源：http://cuk.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://zti.sysykeji.top

[S46] C++：函数模板
来源：http://gwh.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jzp.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://eis.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oyw.jianghu66.top

[S48] C++：逐行读文件
来源：http://bod.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ztf.daxiang520.top

while (std::getline(in, line)) { }
来源：http://cxl.zhiwuduotai.top

[S49] C++：写文件
来源：http://tug.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://squ.tarul.cn

[S50] C++：格式化数字
来源：http://nhh.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oij.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://pru.yuxming.cn

static_cast<double>(a) / b
来源：http://ubi.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://ilr.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://ayo.hammf.cn

[S53] C++：移动语义
来源：http://mgd.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://nql.jiagoushi.top

[S54] C++：异常处理
来源：http://ygi.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jgf.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://ipj.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://hzp.yuxming.cn

[S56] C++：optional
来源：http://nmr.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jik.316326.xyz

[S57] C++：编译期常量
来源：http://rez.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://qja.cheryme.top

[S58] C++：命名空间
来源：http://nuc.yueranfly.top

namespace ns { int f() { return 1; } }
来源：http://ykf.vehdjk.com

[S59] C++：静态断言
来源：http://qwo.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qzf.ehwqpu.com

[S60] C++：遍历并删除元素
来源：http://vok.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ssr.ehwqpu.com

================================================================================
来源：http://ftl.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uxk.hfpthk.cn

================================================================================
来源：http://nxz.gaohongyu789.top

[T01] Kotlin：Hello World
来源：http://nsh.xylfe.cn

println("Hello")
来源：http://fti.hongshengwenyu.top

[T02] Kotlin：变量
来源：http://nry.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zhe.hammf.cn

[T03] Kotlin：字符串模板
来源：http://hlc.yanxiufei.cn

"值: $b"
来源：http://zdy.cashguo.top

[T04] Kotlin：空安全
来源：http://xuw.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://tap.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://wgo.zdqjudy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ltg.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://oqx.yuxming.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qbh.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://gee.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gml.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://pwl.hfpthk.cn

data class User(val name: String, val age: Int)
来源：http://jdn.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://jdx.xingfuxueyuan.xyz

fun String.exclaim() = this + "!"
来源：http://jwm.xylfe.cn

[T10] Kotlin：默认参数
来源：http://dmh.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ggi.ivvv.top

[T11] Kotlin：协程
来源：http://kde.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gvf.tanke756.top

[T12] Kotlin：解构声明
来源：http://gzk.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://vvt.yj202588.top

[T13] Kotlin：只读 Map
来源：http://lne.shuidangran.top

val m = mapOf("a" to 1)
来源：http://mad.hammf.cn

[T14] Kotlin：循环
来源：http://dyw.xziqi.cn

for (i in 1..10) println(i)
来源：http://lkc.yvedp.cn

[T15] Kotlin：接口
来源：http://cad.fengsongda.top

interface Shape { fun area(): Double }
来源：http://low.hammf.cn

[T16] Swift：Hello World
来源：http://mkj.chenzaomai.com

print("Hello")
来源：http://bya.feifeiyinyue.top

[T17] Swift：变量与常量
来源：http://zke.52xcode.cn

var a = 1;  let b = 2
来源：http://yhk.chenjidiqi.icu

[T18] Swift：字符串插值
来源：http://ohb.zhaomingkeji.xyz

"值: \(b)"
来源：http://awt.bbcook.cn

[T19] Swift：可选绑定
来源：http://tju.zdbjq.cn

if let n = opt { print(n) }
来源：http://npn.hammf.cn

[T20] Swift：数组操作
来源：http://aap.hcnkem.com

var a = [1, 2, 3];  a.append(4)
来源：http://hry.shuidangran.top

[T21] Swift：遍历
来源：http://jhs.cucudq.cn

for x in a { print(x) }
来源：http://wap.yvedp.cn

[T22] Swift：字典
来源：http://tne.ywan-chungtsiang.top

var d = ["a": 1];  d["b"] = 2
来源：http://akf.jianghu66.top

[T23] Swift：函数
来源：http://yox.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wew.sxryk.cn

[T24] Swift：闭包
来源：http://sca.jyoumei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gho.jqgufenzy.top

[T25] Swift：结构体
来源：http://enu.dianchejie.cn

struct P { var x: Int }
来源：http://tii.cucudq.cn

[T26] Swift：类与重写
来源：http://ldd.andypj.xyz

class A: Base { override func f() {} }
来源：http://kgw.jianghu66.top

[T27] Swift：错误处理
来源：http://qkd.tian-w.cn

do { try f() } catch { print(error) }
来源：http://ucx.quarkkingdee.top

[T28] Swift：枚举
来源：http://xfr.jinghuilouyu.cn

enum Color { case red, green }
来源：http://srl.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://irx.sxryk.cn

guard let x = opt else { return }
来源：http://wtw.gaohongyu789.top

[T30] Swift：协议
来源：http://hlu.yj20258.top

protocol Shape { func area() -> Double }
来源：http://rwz.0kj1m.cn

[T31] Lua：Hello World
来源：http://vzc.c1oappe.top

print("Hello")
来源：http://zqt.epnwcf.com

[T32] Lua：局部变量
来源：http://imv.fengsongda.top

local a = 1
来源：http://jfa.ctjpmb.com

[T33] Lua：表（数组）
来源：http://ieu.zycfv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ojw.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://qhh.jinqigfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ahq.cashguo.top

[T35] Lua：字典表
来源：http://nav.fanxiaobao.xyz

local d = { a = 1 };  d.b = 2
来源：http://qif.yvedp.cn

[T36] Lua：函数
来源：http://tdv.fengsongda.top

function add(a, b) return a + b end
来源：http://qfg.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://uqi.ywan-chungtsiang.top

"a" .. "b"
来源：http://ajc.snrcjt.cn

[T38] Lua：条件
来源：http://pjl.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://coq.vqdsnc.cn

[T39] Lua：模式匹配
来源：http://ovt.c1oappe.top

string.find(s, "%d+")
来源：http://utq.yvedp.cn

[T40] Lua：元表
来源：http://fwo.hywenlv.cn

setmetatable({}, { __index = base })
来源：http://mcz.yj20258.top

[T41] Perl：Hello World
来源：http://xxi.tanke756.top

print "Hello\n";
来源：http://bjf.vqdsnc.cn

[T42] Perl：变量类型
来源：http://bdy.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yra.tanke756.top

[T43] Perl：字符串插值
来源：http://jwd.quarkkingdee.top

"值: $a"
来源：http://ogy.aizwys.cn

[T44] Perl：条件
来源：http://ved.fzhhl.top

if ($a > 0) { print "正"; }
来源：http://uvg.c1oappe.top

[T45] Perl：数组遍历
来源：http://gjq.chenzaomai.com

for my $x (@arr) { print $x; }
来源：http://yho.gotoacloud.top

[T46] Perl：哈希操作
来源：http://jof.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mbw.zdqjudy.top

[T47] Perl：正则捕获
来源：http://fca.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vdl.ivvv.top

[T48] Perl：正则替换
来源：http://xiz.jyoumei.cn

$s =~ s/old/new/g;
来源：http://pnv.zhiwuduotai.top

[T49] Perl：函数
来源：http://wur.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yne.52xcode.cn

[T50] Perl：逐行读文件
来源：http://pmm.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ecn.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://fpw.ctjpmb.com

[T51] Scala：Hello World
来源：http://vaz.yj20258888.top

println("Hello")
来源：http://mvn.yonumen.top

[T52] Scala：变量
来源：http://vyq.hesvh.cn

val a = 1;  var b = 2
来源：http://dqg.zdqjudy.top

[T53] Scala：字符串插值
来源：http://xxg.svipenyu.cn

s"值: $b"
来源：http://yxn.haohaochexian.top

[T54] Scala：集合映射
来源：http://hfs.epnwcf.com

List(1, 2, 3).map(_ * 2)
来源：http://keg.zhengqikj.top

[T55] Scala：集合过滤
来源：http://rkv.kuanghao11.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ifk.mhx1999.top

[T56] Scala：样例类
来源：http://xhy.xingfuxueyuan.xyz

case class User(name: String, age: Int)
来源：http://tbx.shangyingyoupin.top

[T57] Scala：模式匹配
来源：http://qwn.cheryme.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rdg.quarkkingdee.top

[T58] Scala：函数定义
来源：http://tkw.zhengqikj.top

def add(a: Int, b: Int): Int = a + b
来源：http://cjo.zdbjq.cn

[T59] Scala：循环
来源：http://fhi.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://sdr.cucudq.cn

[T60] Scala：折叠
来源：http://mrk.gaohongyu789.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cub.sweek.top

================================================================================
来源：http://nyq.xingfuxueyuan.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ytk.zhiwuduotai.top

================================================================================
来源：http://lnm.chenjidiqi.icu

[U01] Py：创建虚拟环境
来源：http://dfe.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://yro.yonumen.top

[U02] Py：导出 / 安装依赖
来源：http://nkz.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ksr.dashuyun.cn

[U03] Py：加载 .env 配置
来源：http://dau.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wdu.ydjk.org.cn

[U04] Py：变量调试打印
来源：http://chl.daria6918.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pdx.bbcook.cn

[U05] Py：列表去重且保序
来源：http://yov.cheryme.top

list(dict.fromkeys(arr))
来源：http://txn.feifeiyinyue.top

[U06] Py：合并两个字典
来源：http://qpe.yj20258.top

{**a, **b}
来源：http://jom.yueranfly.top

[U07] Py：反转字典键值
来源：http://dhc.yangfankeji.com

{v: k for k, v in d.items()}
来源：http://rld.iojbl.cn

[U08] Py：展平二维列表
来源：http://lfw.yueranfly.top

[y for x in nested for y in x]
来源：http://jdf.yuxming.cn

[U09] Py：字典取最大值的键
来源：http://ybx.feifeiyinyue.top

max(d, key=d.get)
来源：http://amq.guowangkeji.top

[U10] Py：按值排序字典
来源：http://owz.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://woe.ybcxt.top

[U11] Py：生成器表达式
来源：http://fqn.zhengqikj.top

(x * 2 for x in arr)
来源：http://bmf.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://dul.ydzc1.top

Counter(arr).most_common(3)
来源：http://tpg.shuidangran.top

[U13] Py：固定长度队列
来源：http://zta.quarkkingdee.top

deque(maxlen=10)
来源：http://mbz.bbcook.cn

[U14] Py：分组收集到列表
来源：http://zsg.xuetiantiany.cn

defaultdict(list)
来源：http://qkc.9152youxi.cn


<!-- 参考信息 -->