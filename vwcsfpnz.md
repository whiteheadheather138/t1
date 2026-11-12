代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://xgh.yfazqb.com

[R70] 时间戳与互转
来源：http://qrb.hywenlv.cn

date +%s;  date -d @1700000000
来源：http://jau.iojbl.cn

[R71] 日期格式化
来源：http://xbv.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://clu.haohaochexian.top

[R72] 等待端口就绪
来源：http://fhi.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://png.cqqwz.cn

[R73] 分割大日志
来源：http://phc.dashuyun.cn

split -l 1000 big.log part_
来源：http://pye.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://wfq.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xvq.bjfxy.top

[R75] 导出环境变量
来源：http://ydt.zhixingplan.top

export PATH="$HOME/bin:$PATH"
来源：http://spf.tian-w.cn

[R76] 使用临时文件
来源：http://wsf.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sat.chenlongwang.top

[R77] 读取用户输入
来源：http://zod.daxiang520.top

read -rp "请输入: " ans
来源：http://hpk.hcnkem.com

[R78] 交互式菜单
来源：http://imd.fehbvm.com

select opt in a b c; do echo "$opt"; break; done
来源：http://zou.ppjwa.cn

[R79] 解析命令行选项
来源：http://jqs.cucudq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pfw.52xcode.cn

[R80] 查看脚本执行耗时
来源：http://iev.cheryme.top

time ./run.sh
来源：http://hgw.xuetiantiany.cn

================================================================================
来源：http://yal.ctjpmb.com

S. C / C++ 专题
来源：http://lef.hfpthk.cn

================================================================================
来源：http://xbp.havefunace.top

[S01] C：Hello World
来源：http://awf.yj202588.top

#include <stdio.h>
来源：http://dzh.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nrn.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://mvf.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://ozu.chenjidiqi.icu

[S03] C：读入整数
来源：http://mov.ppjwa.cn

int x; scanf("%d", &x);
来源：http://cdo.zycfv.cn

[S04] C：字符串复制
来源：http://gir.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://lsd.feifeiyinyue.top

[S05] C：字符串长度
来源：http://bfq.quarkkingdee.top

strlen(s)
来源：http://wnh.tianlin.xyz

[S06] C：字符串比较
来源：http://xzp.birdmap.top

strcmp(a, b) == 0
来源：http://uat.yvedp.cn

[S07] C：数组遍历求和
来源：http://khz.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cbi.quarkkingdee.top

[S08] C：动态内存分配与释放
来源：http://ckg.jianghu66.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sfs.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://jex.uphjek.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dpt.yj202588.top

[S10] C：指针与解引用
来源：http://miw.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://hnr.mhx1999.top

[S11] C：逐行读文件
来源：http://kbu.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://caw.zhongyouzk.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xdg.wangshuangyany.cn

fclose(f);
来源：http://qtw.guowangkeji.top

[S12] C：写文件
来源：http://uoy.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hoy.epnwcf.com

[S13] C：宏定义
来源：http://xwd.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nwu.fanxiaobao.xyz

[S14] C：枚举
来源：http://yue.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://nla.iojbl.cn

[S15] C：类型转换
来源：http://wsy.xinyue.icu

(double) a / b
来源：http://fua.ydzc1.top

[S16] C：位操作置位
来源：http://ror.hywenlv.cn

x |= (1 << 3);
来源：http://kgb.zhixingplan.top

[S17] C：安全拼接字符串
来源：http://pgj.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tku.zhixingplan.top

[S18] C：命令行参数
来源：http://gty.fehbvm.com

int main(int argc, char **argv)
来源：http://tqg.xziqi.cn

[S19] C：快速排序
来源：http://kkh.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://lsh.xuanzx.com

[S20] C：二分查找
来源：http://fkk.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ajy.hfpthk.cn

[S21] C：字符类别判断
来源：http://tex.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hyc.shzxlz.cn

[S22] C：字符串转数字
来源：http://eju.guowangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://pfr.zycfv.cn

[S23] C：随机数
来源：http://agk.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xzj.yj20258.top

[S24] C：获取本地时间
来源：http://rvu.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://akg.ivvv.top

[S25] C：内存拷贝
来源：http://fro.yvedp.cn

memcpy(dst, src, n);
来源：http://ouy.9152youxi.cn

[S26] C：内存清零
来源：http://tus.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://pmy.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://eol.yangfankeji.com

const double PI = 3.14159;
来源：http://myl.yongpay.top

[S28] C：静态变量
来源：http://jyp.ctjpmb.com

static int counter = 0;
来源：http://uof.chenzaomai.com

[S29] C：变参函数
来源：http://fzv.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://reb.chenjidiqi.icu

[S30] C：头文件保护
来源：http://czo.hnxiangtu.top

#ifndef X_H
来源：http://vlq.sjlbkw.cn

#define X_H
来源：http://fnx.xuanzx.com

#endif
来源：http://yqo.snrcjt.cn

[S31] C++：Hello World
来源：http://eyi.daria6918.cn

#include <iostream>
来源：http://wsq.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://dhf.fehbvm.com

[S32] C++：字符串
来源：http://juc.fktsv.cn

std::string s = "hi";  s += "!";
来源：http://osg.sjlbkw.cn

[S33] C++：vector 增删
来源：http://qcy.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nql.epnwcf.com

[S34] C++：遍历 vector
来源：http://dys.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://gsy.yuanzhike.top

[S35] C++：map
来源：http://bbw.cashguo.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rtc.yvedp.cn

[S36] C++：unordered_map
来源：http://joe.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://okb.vqdsnc.cn

[S37] C++：set
来源：http://hjy.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://spt.hesvh.cn

[S38] C++：排序
来源：http://oii.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://kdz.yuanzhike.top

[S39] C++：自定义比较器排序
来源：http://bag.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yzx.xinyue.icu

[S40] C++：查找元素
来源：http://hnq.yonumen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://svn.chenzaomai.com

[S41] C++：类与构造函数
来源：http://akn.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ids.xziqi.cn

[S42] C++：继承与虚函数
来源：http://hog.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://hra.0kj1m.cn

[S43] C++：智能指针
来源：http://vvq.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://qhp.jinqigfzy.top

[S44] C++：引用传参
来源：http://joq.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://tew.shzxlz.cn

[S45] C++：lambda
来源：http://bqi.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://cif.cashguo.top

[S46] C++：函数模板
来源：http://xam.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://olo.dianchejie.cn

[S47] C++：结构化绑定遍历
来源：http://hjm.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://crv.dianchejie.cn

[S48] C++：逐行读文件
来源：http://dmc.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://gnk.yuxming.cn

while (std::getline(in, line)) { }
来源：http://hga.xylfe.cn

[S49] C++：写文件
来源：http://jav.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yrr.hammf.cn

[S50] C++：格式化数字
来源：http://trw.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ihs.uphjek.com

[S51] C++：显式类型转换
来源：http://wjx.aibaodan.cn

static_cast<double>(a) / b
来源：http://ghm.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://xyl.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://aql.yfazqb.com

[S53] C++：移动语义
来源：http://zgb.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://vxr.gotoacloud.top

[S54] C++：异常处理
来源：http://kaq.c1oappe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://brf.hnqzz.top

[S55] C++：结构化绑定
来源：http://ebp.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cva.kuanghao11.cn

[S56] C++：optional
来源：http://ctx.birdmap.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tuj.aizwys.cn

[S57] C++：编译期常量
来源：http://gen.yangfankeji.com

constexpr int N = 10;
来源：http://ohs.mhx1999.top

[S58] C++：命名空间
来源：http://bxy.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://obt.shangyingyoupin.top

[S59] C++：静态断言
来源：http://yzs.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ukk.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://hqc.9152youxi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://teo.hysaishi.cn

================================================================================
来源：http://dhs.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fth.9152youxi.cn

================================================================================
来源：http://tza.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://qqf.tian-w.cn

println("Hello")
来源：http://snm.yfazqb.com

[T02] Kotlin：变量
来源：http://ccm.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nzm.yuxming.cn

[T03] Kotlin：字符串模板
来源：http://ozk.bbcook.cn

"值: $b"
来源：http://jhl.yj20258.top

[T04] Kotlin：空安全
来源：http://wqb.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://hen.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://pwd.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tzt.yfazqb.com

[T06] Kotlin：集合映射
来源：http://qxl.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pwc.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://slh.pycfn.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://mxe.jinqigufen.top

[T08] Kotlin：数据类
来源：http://ejo.svipenyu.cn

data class User(val name: String, val age: Int)
来源：http://cyg.gaohongyu789.top

[T09] Kotlin：扩展函数
来源：http://pos.xylfe.cn

fun String.exclaim() = this + "!"
来源：http://ytt.yvedp.cn

[T10] Kotlin：默认参数
来源：http://nxp.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jcn.sxryk.cn

[T11] Kotlin：协程
来源：http://loq.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jwd.chenzaomai.com

[T12] Kotlin：解构声明
来源：http://dsz.meibo888.top

val (a, b) = Pair(1, 2)
来源：http://hrv.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://kyz.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://kxb.meibo888.top

[T14] Kotlin：循环
来源：http://jxx.hfpthk.cn

for (i in 1..10) println(i)
来源：http://yrz.hysaishi.cn

[T15] Kotlin：接口
来源：http://zzq.nwbrower.top

interface Shape { fun area(): Double }
来源：http://mqi.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://tae.gotoacloud.top

print("Hello")
来源：http://nvx.yonumen.top

[T17] Swift：变量与常量
来源：http://ujj.nwbrower.top

var a = 1;  let b = 2
来源：http://wph.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://sth.hammf.cn

"值: \(b)"
来源：http://sxx.sxryk.cn

[T19] Swift：可选绑定
来源：http://rjj.tanke756.top

if let n = opt { print(n) }
来源：http://vuy.zhiwuduotai.top

[T20] Swift：数组操作
来源：http://rbl.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://ogi.cdnleiting.top

[T21] Swift：遍历
来源：http://juj.fktsv.cn

for x in a { print(x) }
来源：http://qko.dashuyun.cn

[T22] Swift：字典
来源：http://lue.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://lfo.xuanzx.com

[T23] Swift：函数
来源：http://lqs.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pgs.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://kkg.yonumen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://frq.cucudq.cn

[T25] Swift：结构体
来源：http://okl.sjlbkw.cn

struct P { var x: Int }
来源：http://dfe.jinqigfzy.top

[T26] Swift：类与重写
来源：http://kmd.jqgfzy.top

class A: Base { override func f() {} }
来源：http://vik.hywenlv.cn

[T27] Swift：错误处理
来源：http://gaf.9152youxi.cn

do { try f() } catch { print(error) }
来源：http://kyi.ppjwa.cn

[T28] Swift：枚举
来源：http://key.yonumen.top

enum Color { case red, green }
来源：http://unu.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://tvd.ehwqpu.com

guard let x = opt else { return }
来源：http://mkf.hongshengwenyu.top

[T30] Swift：协议
来源：http://lok.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://kzd.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://yew.aibaodan.cn

print("Hello")
来源：http://orm.pycfn.com

[T32] Lua：局部变量
来源：http://dwn.guowangkeji.top

local a = 1
来源：http://vja.ctjpmb.com

[T33] Lua：表（数组）
来源：http://hen.cucudq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://emr.zhongyouzk.top

[T34] Lua：遍历表
来源：http://aub.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://imh.hysaishi.cn

[T35] Lua：字典表
来源：http://fqh.gotoacloud.top

local d = { a = 1 };  d.b = 2
来源：http://ovq.jiagoushi.top

[T36] Lua：函数
来源：http://iba.zhiwuduotai.top

function add(a, b) return a + b end
来源：http://ivm.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://fnj.gaohongyu789.top

"a" .. "b"
来源：http://kmm.yuanzhike.top

[T38] Lua：条件
来源：http://hsi.zycfv.cn

if x > 0 then print("正") end
来源：http://mux.jlsjyb.cn

[T39] Lua：模式匹配
来源：http://smm.zhoulong.xyz

string.find(s, "%d+")
来源：http://fvj.redwolf501.top

[T40] Lua：元表
来源：http://zia.fehbvm.com

setmetatable({}, { __index = base })
来源：http://cfb.ywan-chungtsiang.top

[T41] Perl：Hello World
来源：http://oem.daria6918.cn

print "Hello\n";
来源：http://rlf.birdmap.top

[T42] Perl：变量类型
来源：http://nri.hfpthk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://awy.yj20258888.top

[T43] Perl：字符串插值
来源：http://soc.guowangkeji.top

"值: $a"
来源：http://ruv.ydzc1.top

[T44] Perl：条件
来源：http://fbl.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://wna.xziqi.cn

[T45] Perl：数组遍历
来源：http://vfi.nanxinkj.top

for my $x (@arr) { print $x; }
来源：http://gdm.chenzaomai.com

[T46] Perl：哈希操作
来源：http://una.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dbm.wangdashe.top

[T47] Perl：正则捕获
来源：http://amn.9152youxi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vdx.fzhhl.top

[T48] Perl：正则替换
来源：http://sdj.yueranfly.top

$s =~ s/old/new/g;
来源：http://awv.shzxlz.cn

[T49] Perl：函数
来源：http://qrs.shanyushiyangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tga.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://tid.birdmap.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pfv.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://old.jinqigfzy.top

[T51] Scala：Hello World
来源：http://rbf.hesvh.cn

println("Hello")
来源：http://dti.jlsjyb.cn

[T52] Scala：变量
来源：http://dma.yongpay.top

val a = 1;  var b = 2
来源：http://rkr.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://zvq.chenjidiqi.icu

s"值: $b"
来源：http://bbd.yanxiufei.cn

[T54] Scala：集合映射
来源：http://hdl.yuanzhike.top

List(1, 2, 3).map(_ * 2)
来源：http://sja.bjfxy.top

[T55] Scala：集合过滤
来源：http://vmp.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://xlj.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://xuw.gaohongyu789.top

case class User(name: String, age: Int)
来源：http://jcs.hysaishi.cn

[T57] Scala：模式匹配
来源：http://cfs.uphjek.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://hur.cdnleiting.top

[T58] Scala：函数定义
来源：http://vdg.redwolf501.top

def add(a: Int, b: Int): Int = a + b
来源：http://fzk.bjfxy.top

[T59] Scala：循环
来源：http://wbl.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://iom.cqqwz.cn

[T60] Scala：折叠
来源：http://ded.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xay.cqqwz.cn

================================================================================
来源：http://iov.tarul.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dec.hnqzz.top

================================================================================
来源：http://vsa.sweek.top

[U01] Py：创建虚拟环境
来源：http://nbs.cashguo.top

python -m venv .venv && source .venv/bin/activate
来源：http://dau.zdqjudy.top

[U02] Py：导出 / 安装依赖
来源：http://its.mhx1999.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mni.cqqwz.cn

[U03] Py：加载 .env 配置
来源：http://kis.yangfankeji.com

from dotenv import load_dotenv; load_dotenv()
来源：http://ztj.zhongyouzk.top

[U04] Py：变量调试打印
来源：http://ayv.quarkkingdee.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iat.meibo888.top

[U05] Py：列表去重且保序
来源：http://soq.316326.xyz

list(dict.fromkeys(arr))
来源：http://nam.nanxinkj.top

[U06] Py：合并两个字典
来源：http://sty.zhongyouzk.top

{**a, **b}
来源：http://bwd.hywenlv.cn

[U07] Py：反转字典键值
来源：http://nsx.aizwys.cn

{v: k for k, v in d.items()}
来源：http://hnq.shanyushiyangtech.top

[U08] Py：展平二维列表
来源：http://trk.yonumen.top

[y for x in nested for y in x]
来源：http://ldg.yj20258.top

[U09] Py：字典取最大值的键
来源：http://lqa.vqdsnc.cn

max(d, key=d.get)
来源：http://mwj.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://otv.ywan-chungtsiang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ikx.zhengqikj.top


<!-- 参考信息 -->