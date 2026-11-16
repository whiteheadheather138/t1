代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://prq.jqgufenzy.top

[R72] 等待端口就绪
来源：http://aqk.chenlongwang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lql.andypj.xyz

[R73] 分割大日志
来源：http://xba.nwbrower.top

split -l 1000 big.log part_
来源：http://dzw.gzhubu.top

[R74] 批量重命名
来源：http://hol.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ftd.nwbrower.top

[R75] 导出环境变量
来源：http://ybq.guannengcc.top

export PATH="$HOME/bin:$PATH"
来源：http://gew.yj20258.top

[R76] 使用临时文件
来源：http://cjn.zhengqikj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://arw.tanke756.top

[R77] 读取用户输入
来源：http://srd.epnwcf.com

read -rp "请输入: " ans
来源：http://ern.sxryk.cn

[R78] 交互式菜单
来源：http://jzh.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zlq.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://ids.hongshengwenyu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lmr.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://pir.gogol.net.cn

time ./run.sh
来源：http://omo.zdbjq.cn

================================================================================
来源：http://gpo.ivvv.top

S. C / C++ 专题
来源：http://yyr.daria6918.cn

================================================================================
来源：http://jzg.c1oappe.top

[S01] C：Hello World
来源：http://bpn.fengsongda.top

#include <stdio.h>
来源：http://wjd.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rcc.yonumen.top

[S02] C：变量与格式化输出
来源：http://wzo.52xcode.cn

int a = 10; printf("%d\n", a);
来源：http://uxo.vehdjk.com

[S03] C：读入整数
来源：http://zny.fktsv.cn

int x; scanf("%d", &x);
来源：http://ory.pengpengdd.cyou

[S04] C：字符串复制
来源：http://kbr.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://jzm.aibaodan.cn

[S05] C：字符串长度
来源：http://yfc.yongpay.top

strlen(s)
来源：http://lwn.sweek.top

[S06] C：字符串比较
来源：http://ebb.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://nmq.xinyue.icu

[S07] C：数组遍历求和
来源：http://jja.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vyj.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://vfs.sufxvd.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zwu.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://qki.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dci.birdmap.top

[S10] C：指针与解引用
来源：http://iou.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://zjg.cqqwz.cn

[S11] C：逐行读文件
来源：http://svb.meibo888.top

FILE *f = fopen("a.txt", "r");
来源：http://pmx.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qew.zhijiandao.cn

fclose(f);
来源：http://qch.ctjpmb.com

[S12] C：写文件
来源：http://xwo.jinghuilouyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dlo.xziqi.cn

[S13] C：宏定义
来源：http://gko.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ogk.sysykeji.top

[S14] C：枚举
来源：http://opo.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://kty.yj20258888.top

[S15] C：类型转换
来源：http://ayn.birdmap.top

(double) a / b
来源：http://soe.dashuyun.cn

[S16] C：位操作置位
来源：http://vhl.yfazqb.com

x |= (1 << 3);
来源：http://ybh.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://xrm.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fep.dianchejie.cn

[S18] C：命令行参数
来源：http://dbz.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://rhw.xylfe.cn

[S19] C：快速排序
来源：http://axk.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qxt.yj20258888.top

[S20] C：二分查找
来源：http://ulv.316326.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://isk.yfazqb.com

[S21] C：字符类别判断
来源：http://xsz.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qwx.svipenyu.cn

[S22] C：字符串转数字
来源：http://wyj.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xiy.snrcjt.cn

[S23] C：随机数
来源：http://qde.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://hgq.hnxiangtu.top

[S24] C：获取本地时间
来源：http://ams.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yyx.jinqigufen.top

[S25] C：内存拷贝
来源：http://icp.bjfxy.top

memcpy(dst, src, n);
来源：http://cul.snrcjt.cn

[S26] C：内存清零
来源：http://vah.yuxming.cn

memset(a, 0, sizeof a);
来源：http://zqt.yj202588.top

[S27] C：定义常量
来源：http://mpi.tarul.cn

const double PI = 3.14159;
来源：http://ruk.xinyue.icu

[S28] C：静态变量
来源：http://fuc.yfazqb.com

static int counter = 0;
来源：http://zkn.hammf.cn

[S29] C：变参函数
来源：http://isa.zhoulong.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ytx.gogol.net.cn

[S30] C：头文件保护
来源：http://rex.daxiang520.top

#ifndef X_H
来源：http://moj.xinyue.icu

#define X_H
来源：http://fmg.guannengcc.top

#endif
来源：http://ubf.ybcxt.top

[S31] C++：Hello World
来源：http://ctj.vehdjk.com

#include <iostream>
来源：http://ruw.fengsongda.top

int main() { std::cout << "Hello\n"; }
来源：http://ciq.snrcjt.cn

[S32] C++：字符串
来源：http://voy.epnwcf.com

std::string s = "hi";  s += "!";
来源：http://vvg.fzhhl.top

[S33] C++：vector 增删
来源：http://jfq.52xcode.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lga.tarul.cn

[S34] C++：遍历 vector
来源：http://lzy.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://yke.c1oappe.top

[S35] C++：map
来源：http://vkk.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://grq.tianlin.xyz

[S36] C++：unordered_map
来源：http://ken.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uye.aibaodan.cn

[S37] C++：set
来源：http://dvf.zycfv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ztw.ywan-chungtsiang.top

[S38] C++：排序
来源：http://ebh.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://xwg.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://mjw.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jiq.jianghu66.top

[S40] C++：查找元素
来源：http://mre.yj20258888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xyl.yj20258888.top

[S41] C++：类与构造函数
来源：http://rsw.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sjr.9152youxi.cn

[S42] C++：继承与虚函数
来源：http://qzy.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://uim.316326.xyz

[S43] C++：智能指针
来源：http://jrs.wangdashe.top

auto p = std::make_unique<int>(5);
来源：http://lpc.haohaochexian.top

[S44] C++：引用传参
来源：http://gak.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://dac.yongpay.top

[S45] C++：lambda
来源：http://kra.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://zjg.aizwys.cn

[S46] C++：函数模板
来源：http://vmi.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mik.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://qns.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iep.yueranfly.top

[S48] C++：逐行读文件
来源：http://cof.gaohongyu789.top

std::ifstream in("a.txt");  std::string line;
来源：http://dak.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://idj.snrcjt.cn

[S49] C++：写文件
来源：http://not.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zpf.cucudq.cn

[S50] C++：格式化数字
来源：http://pou.sjlbkw.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gyd.sweek.top

[S51] C++：显式类型转换
来源：http://zje.guowangkeji.top

static_cast<double>(a) / b
来源：http://elc.guowangkeji.top

[S52] C++：const 与 noexcept
来源：http://kab.hnqzz.top

int size() const noexcept { return n_; }
来源：http://ial.ivvv.top

[S53] C++：移动语义
来源：http://xqf.yuxming.cn

std::vector<int> w = std::move(v);
来源：http://zak.0kj1m.cn

[S54] C++：异常处理
来源：http://xso.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qmw.sufxvd.cn

[S55] C++：结构化绑定
来源：http://bge.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://guj.hnqzz.top

[S56] C++：optional
来源：http://szx.pycfn.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zrb.dashuyun.cn

[S57] C++：编译期常量
来源：http://lio.cheryme.top

constexpr int N = 10;
来源：http://lxd.jiagoushi.top

[S58] C++：命名空间
来源：http://rkq.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://xcp.feifeiyinyue.top

[S59] C++：静态断言
来源：http://clf.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bur.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://emf.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eah.hnqzz.top

================================================================================
来源：http://ifj.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xrt.hysaishi.cn

================================================================================
来源：http://ofb.yueranfly.top

[T01] Kotlin：Hello World
来源：http://gys.zhiwuduotai.top

println("Hello")
来源：http://whz.c1oappe.top

[T02] Kotlin：变量
来源：http://rig.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://znt.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://wnk.fengsongda.top

"值: $b"
来源：http://xor.yangfankeji.com

[T04] Kotlin：空安全
来源：http://jeq.andypj.xyz

val n: String? = null;  n?.length
来源：http://hen.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://yxa.hywenlv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gio.havefunace.top

[T06] Kotlin：集合映射
来源：http://noi.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://stp.52xcode.cn

[T07] Kotlin：集合过滤
来源：http://hmn.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wkf.yj202588.top

[T08] Kotlin：数据类
来源：http://ftf.pycfn.com

data class User(val name: String, val age: Int)
来源：http://zqa.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://dey.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://ywg.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://atp.epnwcf.com

fun greet(name: String = "World") = "Hi $name"
来源：http://nlf.cashguo.top

[T11] Kotlin：协程
来源：http://dtk.zdqjudy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://myz.cashguo.top

[T12] Kotlin：解构声明
来源：http://lsh.0kj1m.cn

val (a, b) = Pair(1, 2)
来源：http://inq.yonumen.top

[T13] Kotlin：只读 Map
来源：http://dcv.52xcode.cn

val m = mapOf("a" to 1)
来源：http://iht.xziqi.cn

[T14] Kotlin：循环
来源：http://lwq.cucudq.cn

for (i in 1..10) println(i)
来源：http://mwx.chenzaomai.com

[T15] Kotlin：接口
来源：http://bdw.hammf.cn

interface Shape { fun area(): Double }
来源：http://ixe.pycfn.com

[T16] Swift：Hello World
来源：http://wlq.fehbvm.com

print("Hello")
来源：http://pqr.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://upp.nanxuanxn.top

var a = 1;  let b = 2
来源：http://qkn.dianchejie.cn

[T18] Swift：字符串插值
来源：http://uxo.daxiang520.top

"值: \(b)"
来源：http://ifk.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://ywu.cheryme.top

if let n = opt { print(n) }
来源：http://agh.jinghuilouyu.cn

[T20] Swift：数组操作
来源：http://kfh.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bpb.wangshuangyany.cn

[T21] Swift：遍历
来源：http://glu.yuanzhike.top

for x in a { print(x) }
来源：http://run.xylfe.cn

[T22] Swift：字典
来源：http://aym.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://tzz.gogol.net.cn

[T23] Swift：函数
来源：http://gnq.guannengcc.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kyk.xziqi.cn

[T24] Swift：闭包
来源：http://ucp.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://cjk.hammf.cn

[T25] Swift：结构体
来源：http://lmm.shangyingyoupin.top

struct P { var x: Int }
来源：http://yqq.c1oappe.top

[T26] Swift：类与重写
来源：http://kmm.jinyuanbaomall.cn

class A: Base { override func f() {} }
来源：http://ber.9152youxi.cn

[T27] Swift：错误处理
来源：http://hso.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://hmh.jqgufenzy.top

[T28] Swift：枚举
来源：http://vpe.ybcxt.top

enum Color { case red, green }
来源：http://hvs.dianchejie.cn

[T29] Swift：guard 提前返回
来源：http://pst.hysaishi.cn

guard let x = opt else { return }
来源：http://nug.guannengcc.top

[T30] Swift：协议
来源：http://ixv.xingfuxueyuan.xyz

protocol Shape { func area() -> Double }
来源：http://znm.zhixingplan.top

[T31] Lua：Hello World
来源：http://rik.bjfxy.top

print("Hello")
来源：http://cqf.aizwys.cn

[T32] Lua：局部变量
来源：http://tvo.tianlin.xyz

local a = 1
来源：http://zkg.ctjpmb.com

[T33] Lua：表（数组）
来源：http://kyn.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qrf.gaohongyu789.top

[T34] Lua：遍历表
来源：http://koq.haohaochexian.top

for i, v in ipairs(t) do print(i, v) end
来源：http://olb.shangyingyoupin.top

[T35] Lua：字典表
来源：http://jux.shanyushiyangtech.top

local d = { a = 1 };  d.b = 2
来源：http://jou.snrcjt.cn

[T36] Lua：函数
来源：http://tkt.xinyue.icu

function add(a, b) return a + b end
来源：http://fqz.shuidangran.top

[T37] Lua：字符串拼接
来源：http://coa.xziqi.cn

"a" .. "b"
来源：http://opk.cucudq.cn

[T38] Lua：条件
来源：http://rvk.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://dpf.kuanghao11.cn

[T39] Lua：模式匹配
来源：http://xmp.jqgufenzy.top

string.find(s, "%d+")
来源：http://buz.zdqjudy.top

[T40] Lua：元表
来源：http://qrv.yongpay.top

setmetatable({}, { __index = base })
来源：http://ucf.fanxiaobao.xyz

[T41] Perl：Hello World
来源：http://giz.cucudq.cn

print "Hello\n";
来源：http://ruq.hnqzz.top

[T42] Perl：变量类型
来源：http://eww.gogol.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cgp.yuanzhike.top

[T43] Perl：字符串插值
来源：http://oen.cashguo.top

"值: $a"
来源：http://swi.yvedp.cn

[T44] Perl：条件
来源：http://lml.sufxvd.cn

if ($a > 0) { print "正"; }
来源：http://zrq.nanxuanxn.top

[T45] Perl：数组遍历
来源：http://dps.tarul.cn

for my $x (@arr) { print $x; }
来源：http://qdc.gogol.net.cn

[T46] Perl：哈希操作
来源：http://yyh.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://quz.shzxlz.cn

[T47] Perl：正则捕获
来源：http://iyn.nanxinkj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xhw.hnqzz.top

[T48] Perl：正则替换
来源：http://lqu.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://nps.feifeiyinyue.top

[T49] Perl：函数
来源：http://jcn.ybcxt.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ens.andypj.xyz

[T50] Perl：逐行读文件
来源：http://rsv.epnwcf.com

open my $fh, "<", "a.txt" or die $!;
来源：http://qps.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://umk.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://uur.jyoumei.cn

println("Hello")
来源：http://jvw.aizwys.cn

[T52] Scala：变量
来源：http://rax.bjfxy.top

val a = 1;  var b = 2
来源：http://tzf.epnwcf.com

[T53] Scala：字符串插值
来源：http://cgj.fengsongda.top

s"值: $b"
来源：http://xdd.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://knf.yanxiufei.cn

List(1, 2, 3).map(_ * 2)
来源：http://omf.cdnleiting.top

[T55] Scala：集合过滤
来源：http://dfv.xuetiantiany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vdg.mhx1999.top

[T56] Scala：样例类
来源：http://xhd.fehbvm.com

case class User(name: String, age: Int)
来源：http://wae.bbcook.cn

[T57] Scala：模式匹配
来源：http://pgi.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://vtm.chenzaomai.com

[T58] Scala：函数定义
来源：http://vwt.sxryk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yaa.jinqigfzy.top

[T59] Scala：循环
来源：http://skk.birdmap.top

for (i <- 1 to 10) println(i)
来源：http://noi.yangfankeji.com

[T60] Scala：折叠
来源：http://njw.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hkt.ybcxt.top

================================================================================
来源：http://dju.kuanghao11.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iwg.daxiang520.top

================================================================================
来源：http://ktt.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://uyc.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gqg.zhongyouzk.top

[U02] Py：导出 / 安装依赖
来源：http://rdr.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jov.zhoulong.xyz

[U03] Py：加载 .env 配置
来源：http://vtl.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pms.jinghuilouyu.cn

[U04] Py：变量调试打印
来源：http://qlp.hesvh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xwi.shuidangran.top

[U05] Py：列表去重且保序
来源：http://aav.meibo888.top

list(dict.fromkeys(arr))
来源：http://fzo.sysykeji.top

[U06] Py：合并两个字典
来源：http://bvi.shanyushiyangkeji.top

{**a, **b}
来源：http://idu.aizwys.cn

[U07] Py：反转字典键值
来源：http://tnd.hammf.cn

{v: k for k, v in d.items()}
来源：http://ltu.pycfn.com

[U08] Py：展平二维列表
来源：http://dik.yuanzhike.top

[y for x in nested for y in x]
来源：http://xtf.hnqzz.top

[U09] Py：字典取最大值的键
来源：http://rbr.zhoulong.xyz

max(d, key=d.get)
来源：http://crb.gogol.net.cn

[U10] Py：按值排序字典
来源：http://ovu.fehbvm.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hkc.gzhubu.top

[U11] Py：生成器表达式
来源：http://rsn.xuetiantiany.cn

(x * 2 for x in arr)
来源：http://gyv.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://xnd.yj202588.top

Counter(arr).most_common(3)
来源：http://aht.zhijiandao.cn


<!-- 参考信息 -->