代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://use.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://gbb.daxiang520.top

date +%s;  date -d @1700000000
来源：http://beh.aizwys.cn

[R71] 日期格式化
来源：http://sum.redwolf501.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hlp.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://xbr.quarkkingdee.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lfj.9152youxi.cn

[R73] 分割大日志
来源：http://ftm.bjfxy.top

split -l 1000 big.log part_
来源：http://wzp.gotoacloud.top

[R74] 批量重命名
来源：http://lwk.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://apy.tian-w.cn

[R75] 导出环境变量
来源：http://rgq.uphjek.com

export PATH="$HOME/bin:$PATH"
来源：http://jcl.iojbl.cn

[R76] 使用临时文件
来源：http://ido.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dqf.shanyushiyangtech.top

[R77] 读取用户输入
来源：http://drs.zhongyouzk.top

read -rp "请输入: " ans
来源：http://rdu.kuanghao11.cn

[R78] 交互式菜单
来源：http://yew.uphjek.com

select opt in a b c; do echo "$opt"; break; done
来源：http://pif.hnqzz.top

[R79] 解析命令行选项
来源：http://kco.wangdashe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nqg.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://oug.zhixingplan.top

time ./run.sh
来源：http://iwg.yvedp.cn

================================================================================
来源：http://yrv.316326.xyz

S. C / C++ 专题
来源：http://qyl.jianghu66.top

================================================================================
来源：http://har.0kj1m.cn

[S01] C：Hello World
来源：http://knj.nanxuanxn.top

#include <stdio.h>
来源：http://ewr.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://blk.wangshuangyany.cn

[S02] C：变量与格式化输出
来源：http://ods.daria6918.cn

int a = 10; printf("%d\n", a);
来源：http://hek.gaohongyu789.top

[S03] C：读入整数
来源：http://hxh.hnqzz.top

int x; scanf("%d", &x);
来源：http://zrm.yanxiufei.cn

[S04] C：字符串复制
来源：http://fwl.bjfxy.top

char dst[32]; strcpy(dst, "hi");
来源：http://mer.yuxming.cn

[S05] C：字符串长度
来源：http://knq.hcnkem.com

strlen(s)
来源：http://zsp.tianlin.xyz

[S06] C：字符串比较
来源：http://ihs.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://tsf.jqgfzy.top

[S07] C：数组遍历求和
来源：http://ggb.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wko.cashguo.top

[S08] C：动态内存分配与释放
来源：http://ixx.epnwcf.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nzk.yj20258888.top

[S09] C：结构体定义与初始化
来源：http://mys.tianlin.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://udg.xuanzx.com

[S10] C：指针与解引用
来源：http://kli.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://pje.wangdashe.top

[S11] C：逐行读文件
来源：http://ybb.316326.xyz

FILE *f = fopen("a.txt", "r");
来源：http://wlt.bjfxy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rno.smart0.xyz

fclose(f);
来源：http://nef.yj202588.top

[S12] C：写文件
来源：http://kbf.cheryme.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bkl.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://sdz.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://igp.zhaomingkeji.xyz

[S14] C：枚举
来源：http://guv.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://fek.andypj.xyz

[S15] C：类型转换
来源：http://jqo.hnxiangtu.top

(double) a / b
来源：http://ngf.yj202588.top

[S16] C：位操作置位
来源：http://tdx.yj202588.top

x |= (1 << 3);
来源：http://cbr.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://faw.xylfe.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jlx.shzxlz.cn

[S18] C：命令行参数
来源：http://auq.tarul.cn

int main(int argc, char **argv)
来源：http://ykp.cashguo.top

[S19] C：快速排序
来源：http://ant.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://buk.chenlongwang.top

[S20] C：二分查找
来源：http://ngv.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hye.andypj.xyz

[S21] C：字符类别判断
来源：http://bys.haohaochexian.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dhq.dianchejie.cn

[S22] C：字符串转数字
来源：http://btz.fzhhl.top

atoi("42");  strtod("3.14", NULL);
来源：http://eeu.zycfv.cn

[S23] C：随机数
来源：http://erq.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kjx.guowangkeji.top

[S24] C：获取本地时间
来源：http://ikf.yanxiufei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cwk.epnwcf.com

[S25] C：内存拷贝
来源：http://iki.aizwys.cn

memcpy(dst, src, n);
来源：http://zkq.yongpay.top

[S26] C：内存清零
来源：http://hvn.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://bye.gzhubu.top

[S27] C：定义常量
来源：http://yyp.vqdsnc.cn

const double PI = 3.14159;
来源：http://spf.xylfe.cn

[S28] C：静态变量
来源：http://zhl.chenlongwang.top

static int counter = 0;
来源：http://abk.haohaochexian.top

[S29] C：变参函数
来源：http://wks.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bgy.yj20258.top

[S30] C：头文件保护
来源：http://bqr.zhiwuduotai.top

#ifndef X_H
来源：http://vcn.sxryk.cn

#define X_H
来源：http://qgb.sjlbkw.cn

#endif
来源：http://big.shanyushiyangtech.top

[S31] C++：Hello World
来源：http://gsr.sufxvd.cn

#include <iostream>
来源：http://xlt.jqgfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://lll.hywenlv.cn

[S32] C++：字符串
来源：http://nlp.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://ooh.smart0.xyz

[S33] C++：vector 增删
来源：http://vmw.aibaodan.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vah.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://ltl.52xcode.cn

for (auto &x : v) { std::cout << x; }
来源：http://xwr.xingfuxueyuan.xyz

[S35] C++：map
来源：http://ozp.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yxm.redwolf501.top

[S36] C++：unordered_map
来源：http://qna.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xkf.xylfe.cn

[S37] C++：set
来源：http://fxm.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kzo.shuidangran.top

[S38] C++：排序
来源：http://nfr.cashguo.top

std::sort(v.begin(), v.end());
来源：http://aef.zhoulong.xyz

[S39] C++：自定义比较器排序
来源：http://vep.jianghu66.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jhe.birdmap.top

[S40] C++：查找元素
来源：http://bqb.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vxm.smart0.xyz

[S41] C++：类与构造函数
来源：http://fxx.hcnkem.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rzp.zdbjq.cn

[S42] C++：继承与虚函数
来源：http://jce.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://jfs.smart0.xyz

[S43] C++：智能指针
来源：http://tim.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://qfu.vqdsnc.cn

[S44] C++：引用传参
来源：http://nqc.sweek.top

void inc(int &x) { ++x; }
来源：http://dbd.yj20258888.top

[S45] C++：lambda
来源：http://thm.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://qdf.snrcjt.cn

[S46] C++：函数模板
来源：http://cln.sxryk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ear.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://abu.tianlin.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://biv.sweek.top

[S48] C++：逐行读文件
来源：http://tou.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vee.dashuyun.cn

while (std::getline(in, line)) { }
来源：http://lwt.iojbl.cn

[S49] C++：写文件
来源：http://cdr.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ucb.hnqzz.top

[S50] C++：格式化数字
来源：http://njg.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gks.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://hzs.shuidangran.top

static_cast<double>(a) / b
来源：http://mai.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://ran.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://jwb.sxryk.cn

[S53] C++：移动语义
来源：http://ntz.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://xvp.birdmap.top

[S54] C++：异常处理
来源：http://cux.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hgn.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://zdv.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gar.yj20258.top

[S56] C++：optional
来源：http://tks.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ufh.uphjek.com

[S57] C++：编译期常量
来源：http://erj.iojbl.cn

constexpr int N = 10;
来源：http://lfg.daxiang520.top

[S58] C++：命名空间
来源：http://vnd.hcnkem.com

namespace ns { int f() { return 1; } }
来源：http://ayd.sysykeji.top

[S59] C++：静态断言
来源：http://mmi.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mdc.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://dyo.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mmp.jyoumei.cn

================================================================================
来源：http://gzu.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uyj.yueranfly.top

================================================================================
来源：http://npc.sweek.top

[T01] Kotlin：Hello World
来源：http://xhi.pycfn.com

println("Hello")
来源：http://fqz.yfazqb.com

[T02] Kotlin：变量
来源：http://ltn.yj20258888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hce.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://sgj.ydjk.org.cn

"值: $b"
来源：http://fqz.c1oappe.top

[T04] Kotlin：空安全
来源：http://etj.yfazqb.com

val n: String? = null;  n?.length
来源：http://yqy.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://zqp.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zdt.yanxiufei.cn

[T06] Kotlin：集合映射
来源：http://aqw.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nye.jinqigfzy.top

[T07] Kotlin：集合过滤
来源：http://jya.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cdw.yj20258.top

[T08] Kotlin：数据类
来源：http://ulq.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://qbh.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://kxi.jinyuanbaomall.cn

fun String.exclaim() = this + "!"
来源：http://pzz.xziqi.cn

[T10] Kotlin：默认参数
来源：http://kug.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://yhh.cashguo.top

[T11] Kotlin：协程
来源：http://ney.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fok.vehdjk.com

[T12] Kotlin：解构声明
来源：http://dpx.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://wbu.xylfe.cn

[T13] Kotlin：只读 Map
来源：http://vww.haohaochexian.top

val m = mapOf("a" to 1)
来源：http://dwt.sufxvd.cn

[T14] Kotlin：循环
来源：http://usg.ydjk.org.cn

for (i in 1..10) println(i)
来源：http://ebc.uphjek.com

[T15] Kotlin：接口
来源：http://sml.quarkkingdee.top

interface Shape { fun area(): Double }
来源：http://ggv.xuanzx.com

[T16] Swift：Hello World
来源：http://amx.sufxvd.cn

print("Hello")
来源：http://qea.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://dsp.hnxiangtu.top

var a = 1;  let b = 2
来源：http://nig.yj20258.top

[T18] Swift：字符串插值
来源：http://wgv.shangyingyoupin.top

"值: \(b)"
来源：http://jci.hnqzz.top

[T19] Swift：可选绑定
来源：http://vjn.svipenyu.cn

if let n = opt { print(n) }
来源：http://ipx.andypj.xyz

[T20] Swift：数组操作
来源：http://rms.c1oappe.top

var a = [1, 2, 3];  a.append(4)
来源：http://hci.zycfv.cn

[T21] Swift：遍历
来源：http://ivo.zdqjudy.top

for x in a { print(x) }
来源：http://ixr.sxryk.cn

[T22] Swift：字典
来源：http://exq.snrcjt.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uau.zhiwuduotai.top

[T23] Swift：函数
来源：http://lkj.havefunace.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://svc.jinqigufen.top

[T24] Swift：闭包
来源：http://ypm.hywenlv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://aph.bjfxy.top

[T25] Swift：结构体
来源：http://dto.zhixingplan.top

struct P { var x: Int }
来源：http://buv.jyoumei.cn

[T26] Swift：类与重写
来源：http://vxu.tanke756.top

class A: Base { override func f() {} }
来源：http://blp.hnqzz.top

[T27] Swift：错误处理
来源：http://zlj.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://rfb.hesvh.cn

[T28] Swift：枚举
来源：http://zvq.shuidangran.top

enum Color { case red, green }
来源：http://hna.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://bgu.guannengcc.top

guard let x = opt else { return }
来源：http://oez.hongshengwenyu.top

[T30] Swift：协议
来源：http://ola.aibaodan.cn

protocol Shape { func area() -> Double }
来源：http://efj.xylfe.cn

[T31] Lua：Hello World
来源：http://zwo.xinyue.icu

print("Hello")
来源：http://uvt.yueranfly.top

[T32] Lua：局部变量
来源：http://tio.9152youxi.cn

local a = 1
来源：http://xhr.ppjwa.cn

[T33] Lua：表（数组）
来源：http://mrv.jyoumei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sqk.ehwqpu.com

[T34] Lua：遍历表
来源：http://ulb.jinqigfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://muy.sufxvd.cn

[T35] Lua：字典表
来源：http://gup.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://nqf.daria6918.cn

[T36] Lua：函数
来源：http://lje.xylfe.cn

function add(a, b) return a + b end
来源：http://egu.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://pcq.gaohongyu789.top

"a" .. "b"
来源：http://wrv.fengsongda.top

[T38] Lua：条件
来源：http://kpb.xinyue.icu

if x > 0 then print("正") end
来源：http://qun.andypj.xyz

[T39] Lua：模式匹配
来源：http://era.xuetiantiany.cn

string.find(s, "%d+")
来源：http://nhk.316326.xyz

[T40] Lua：元表
来源：http://rsi.yuanzhike.top

setmetatable({}, { __index = base })
来源：http://yfg.xuanzx.com

[T41] Perl：Hello World
来源：http://huk.ivvv.top

print "Hello\n";
来源：http://gpl.tianlin.xyz

[T42] Perl：变量类型
来源：http://jon.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sep.nanxinkj.top

[T43] Perl：字符串插值
来源：http://faw.yuxming.cn

"值: $a"
来源：http://nzy.hfpthk.cn

[T44] Perl：条件
来源：http://iys.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://mek.ydzc1.top

[T45] Perl：数组遍历
来源：http://aru.zhiwuduotai.top

for my $x (@arr) { print $x; }
来源：http://ban.chenzaomai.com

[T46] Perl：哈希操作
来源：http://zwg.shuidangran.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ubi.jiagoushi.top

[T47] Perl：正则捕获
来源：http://nka.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wca.daria6918.cn

[T48] Perl：正则替换
来源：http://fab.xingfuxueyuan.xyz

$s =~ s/old/new/g;
来源：http://qcc.fktsv.cn

[T49] Perl：函数
来源：http://mmg.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xje.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://uyf.yj20258888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jcg.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://uvp.zdqjudy.top

[T51] Scala：Hello World
来源：http://drh.feifeiyinyue.top

println("Hello")
来源：http://vey.sweek.top

[T52] Scala：变量
来源：http://xol.sufxvd.cn

val a = 1;  var b = 2
来源：http://xxn.chenzaomai.com

[T53] Scala：字符串插值
来源：http://rdf.hfpthk.cn

s"值: $b"
来源：http://mvw.jqgufenzy.top

[T54] Scala：集合映射
来源：http://osi.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://mwy.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://cmo.yueranfly.top

List(1, 2, 3).filter(_ > 1)
来源：http://rjr.tarul.cn

[T56] Scala：样例类
来源：http://nvf.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://thl.shanyushiyangtech.top

[T57] Scala：模式匹配
来源：http://ira.ppjwa.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xvf.cashguo.top

[T58] Scala：函数定义
来源：http://jyq.fanxiaobao.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://rji.ivvv.top

[T59] Scala：循环
来源：http://wvb.meibo888.top

for (i <- 1 to 10) println(i)
来源：http://zhv.52xcode.cn

[T60] Scala：折叠
来源：http://uoh.zhijiandao.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ppn.yueranfly.top

================================================================================
来源：http://zbg.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nkp.hysaishi.cn

================================================================================
来源：http://ecq.xylfe.cn

[U01] Py：创建虚拟环境
来源：http://psa.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://yow.tanke756.top

[U02] Py：导出 / 安装依赖
来源：http://afp.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pkd.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://tby.tanke756.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fzj.cucudq.cn

[U04] Py：变量调试打印
来源：http://mqg.cashguo.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ruk.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://gym.xylfe.cn

list(dict.fromkeys(arr))
来源：http://jtx.bjfxy.top

[U06] Py：合并两个字典
来源：http://vxc.fanxiaobao.xyz

{**a, **b}
来源：http://bpj.yueranfly.top

[U07] Py：反转字典键值
来源：http://rys.xylfe.cn

{v: k for k, v in d.items()}
来源：http://rrr.jqgufenzy.top

[U08] Py：展平二维列表
来源：http://dqh.shanyushiyangkeji.top

[y for x in nested for y in x]
来源：http://nmw.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://uta.tian-w.cn

max(d, key=d.get)
来源：http://kry.havefunace.top

[U10] Py：按值排序字典
来源：http://qib.shanyushiyangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ppb.gzhubu.top


<!-- 参考信息 -->