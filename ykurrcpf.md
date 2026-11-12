代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://zaa.jlsjyb.cn

[R70] 时间戳与互转
来源：http://twn.shangyingyoupin.top

date +%s;  date -d @1700000000
来源：http://saf.cdnleiting.top

[R71] 日期格式化
来源：http://efm.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://usa.redwolf501.top

[R72] 等待端口就绪
来源：http://ctx.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://sob.nwbrower.top

[R73] 分割大日志
来源：http://mmo.guowangkeji.top

split -l 1000 big.log part_
来源：http://jnj.52xcode.cn

[R74] 批量重命名
来源：http://zsk.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zun.cdnleiting.top

[R75] 导出环境变量
来源：http://sxw.bbcook.cn

export PATH="$HOME/bin:$PATH"
来源：http://eot.feifeiyinyue.top

[R76] 使用临时文件
来源：http://aru.smart0.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ijl.52xcode.cn

[R77] 读取用户输入
来源：http://mrb.ywan-chungtsiang.top

read -rp "请输入: " ans
来源：http://lgg.zycfv.cn

[R78] 交互式菜单
来源：http://tyt.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zei.cashguo.top

[R79] 解析命令行选项
来源：http://cwj.kuanghao11.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rnz.xziqi.cn

[R80] 查看脚本执行耗时
来源：http://jxf.9152youxi.cn

time ./run.sh
来源：http://jeq.quarkkingdee.top

================================================================================
来源：http://jop.zhengqikj.top

S. C / C++ 专题
来源：http://hzj.fehbvm.com

================================================================================
来源：http://wlp.bbcook.cn

[S01] C：Hello World
来源：http://qvd.hcnkem.com

#include <stdio.h>
来源：http://jbw.ywan-chungtsiang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qmk.hcnkem.com

[S02] C：变量与格式化输出
来源：http://wrq.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://vcy.quarkkingdee.top

[S03] C：读入整数
来源：http://hsm.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://bhu.xziqi.cn

[S04] C：字符串复制
来源：http://xtx.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://afk.yuxming.cn

[S05] C：字符串长度
来源：http://nqh.hesvh.cn

strlen(s)
来源：http://xmu.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://nid.zhijiandao.cn

strcmp(a, b) == 0
来源：http://dtk.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://soa.cqqwz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://btc.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://iyq.yvedp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cfh.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://wlz.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hlu.shanyushiyangtech.top

[S10] C：指针与解引用
来源：http://njn.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://uul.316326.xyz

[S11] C：逐行读文件
来源：http://xbu.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://kdi.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://owx.hywenlv.cn

fclose(f);
来源：http://rov.zhixingplan.top

[S12] C：写文件
来源：http://dos.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ijd.cashguo.top

[S13] C：宏定义
来源：http://zzt.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gdf.yuanzhike.top

[S14] C：枚举
来源：http://rsy.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://ozr.cucudq.cn

[S15] C：类型转换
来源：http://muk.yonumen.top

(double) a / b
来源：http://qnd.jiagoushi.top

[S16] C：位操作置位
来源：http://zfi.zhiwuduotai.top

x |= (1 << 3);
来源：http://vfs.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://exr.fktsv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gxt.sxryk.cn

[S18] C：命令行参数
来源：http://yef.gogol.net.cn

int main(int argc, char **argv)
来源：http://ofm.gzhubu.top

[S19] C：快速排序
来源：http://qvh.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://jue.yuanzhike.top

[S20] C：二分查找
来源：http://har.ywan-chungtsiang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://moa.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://tmi.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://web.vehdjk.com

[S22] C：字符串转数字
来源：http://cpd.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://srq.guowangkeji.top

[S23] C：随机数
来源：http://mji.cdnleiting.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fxd.hammf.cn

[S24] C：获取本地时间
来源：http://nva.zhoulong.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aql.cdnleiting.top

[S25] C：内存拷贝
来源：http://ess.xylfe.cn

memcpy(dst, src, n);
来源：http://ajo.chenlongwang.top

[S26] C：内存清零
来源：http://bwu.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://yeh.yfazqb.com

[S27] C：定义常量
来源：http://qji.cheryme.top

const double PI = 3.14159;
来源：http://zvx.yuxming.cn

[S28] C：静态变量
来源：http://mxb.feifeiyinyue.top

static int counter = 0;
来源：http://abo.yj20258.top

[S29] C：变参函数
来源：http://iox.yanxiufei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hou.yvedp.cn

[S30] C：头文件保护
来源：http://fou.redwolf501.top

#ifndef X_H
来源：http://nny.tanke756.top

#define X_H
来源：http://rgp.zhijiandao.cn

#endif
来源：http://afn.hesvh.cn

[S31] C++：Hello World
来源：http://blz.yangfankeji.com

#include <iostream>
来源：http://xrj.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://xcj.yj20258.top

[S32] C++：字符串
来源：http://pbw.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://tkn.feifeiyinyue.top

[S33] C++：vector 增删
来源：http://yiv.havefunace.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://acq.chenlongwang.top

[S34] C++：遍历 vector
来源：http://iuu.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://uhx.yanxiufei.cn

[S35] C++：map
来源：http://clp.quarkkingdee.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jaa.nanxinkj.top

[S36] C++：unordered_map
来源：http://vlu.chenjidiqi.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yiu.fehbvm.com

[S37] C++：set
来源：http://wlh.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ydo.yueranfly.top

[S38] C++：排序
来源：http://ngx.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://mcb.hcnkem.com

[S39] C++：自定义比较器排序
来源：http://jrg.xinyue.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://reo.cucudq.cn

[S40] C++：查找元素
来源：http://xel.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dqp.nanxinkj.top

[S41] C++：类与构造函数
来源：http://xjp.nwbrower.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uuw.xylfe.cn

[S42] C++：继承与虚函数
来源：http://ufd.hywenlv.cn

class B : public Base { public: void f() override {} };
来源：http://qrq.hnqzz.top

[S43] C++：智能指针
来源：http://uyf.yj20258.top

auto p = std::make_unique<int>(5);
来源：http://zox.wangshuangyany.cn

[S44] C++：引用传参
来源：http://ukf.cashguo.top

void inc(int &x) { ++x; }
来源：http://ibf.daxiang520.top

[S45] C++：lambda
来源：http://svj.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://obe.xingfuxueyuan.xyz

[S46] C++：函数模板
来源：http://epl.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uxg.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://mfe.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tlm.yvedp.cn

[S48] C++：逐行读文件
来源：http://xca.xuanzx.com

std::ifstream in("a.txt");  std::string line;
来源：http://hkf.shanyushiyangtech.top

while (std::getline(in, line)) { }
来源：http://ykr.xuanzx.com

[S49] C++：写文件
来源：http://wzk.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vhh.kuanghao11.cn

[S50] C++：格式化数字
来源：http://csg.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xci.nanxinkj.top

[S51] C++：显式类型转换
来源：http://xsz.ehwqpu.com

static_cast<double>(a) / b
来源：http://qfj.ivvv.top

[S52] C++：const 与 noexcept
来源：http://ifx.ydzc1.top

int size() const noexcept { return n_; }
来源：http://cdc.yj20258888.top

[S53] C++：移动语义
来源：http://yii.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://gcw.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://cgr.tianlin.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kxh.fengsongda.top

[S55] C++：结构化绑定
来源：http://iin.yuanzhike.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jtf.hfpthk.cn

[S56] C++：optional
来源：http://rjx.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hwj.chenjidiqi.icu

[S57] C++：编译期常量
来源：http://fua.shanyushiyangkeji.top

constexpr int N = 10;
来源：http://nxu.aizwys.cn

[S58] C++：命名空间
来源：http://goo.haohaochexian.top

namespace ns { int f() { return 1; } }
来源：http://exb.shuidangran.top

[S59] C++：静态断言
来源：http://jqm.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blc.tarul.cn

[S60] C++：遍历并删除元素
来源：http://wrl.tarul.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lyx.jianghu66.top

================================================================================
来源：http://cmc.hnqzz.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cfh.fehbvm.com

================================================================================
来源：http://zew.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://zjh.guowangkeji.top

println("Hello")
来源：http://oqr.cqqwz.cn

[T02] Kotlin：变量
来源：http://por.gogol.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qjs.hammf.cn

[T03] Kotlin：字符串模板
来源：http://mco.guowangkeji.top

"值: $b"
来源：http://zvf.zdbjq.cn

[T04] Kotlin：空安全
来源：http://umr.jyoumei.cn

val n: String? = null;  n?.length
来源：http://hee.tian-w.cn

[T05] Kotlin：when 表达式
来源：http://iia.aizwys.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sox.cucudq.cn

[T06] Kotlin：集合映射
来源：http://hqo.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nwa.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://ndp.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ltr.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://bnc.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://hsx.bjfxy.top

[T09] Kotlin：扩展函数
来源：http://ljy.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://xkj.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://xob.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://act.jqgfzy.top

[T11] Kotlin：协程
来源：http://ljs.yj202588.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zoq.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://nci.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://mif.fzhhl.top

[T13] Kotlin：只读 Map
来源：http://bak.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://zgj.yj20258888.top

[T14] Kotlin：循环
来源：http://uwa.ctjpmb.com

for (i in 1..10) println(i)
来源：http://zis.chenlongwang.top

[T15] Kotlin：接口
来源：http://haq.kuanghao11.cn

interface Shape { fun area(): Double }
来源：http://uem.kuanghao11.cn

[T16] Swift：Hello World
来源：http://ler.tian-w.cn

print("Hello")
来源：http://obi.bjfxy.top

[T17] Swift：变量与常量
来源：http://wjz.yonumen.top

var a = 1;  let b = 2
来源：http://jef.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://svl.hammf.cn

"值: \(b)"
来源：http://anc.hywenlv.cn

[T19] Swift：可选绑定
来源：http://ktd.zycfv.cn

if let n = opt { print(n) }
来源：http://bwg.svipenyu.cn

[T20] Swift：数组操作
来源：http://bzs.wangdashe.top

var a = [1, 2, 3];  a.append(4)
来源：http://nih.aibaodan.cn

[T21] Swift：遍历
来源：http://wci.aizwys.cn

for x in a { print(x) }
来源：http://azj.hywenlv.cn

[T22] Swift：字典
来源：http://tuo.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://stt.zhijiandao.cn

[T23] Swift：函数
来源：http://vbg.yj20258888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://btl.cucudq.cn

[T24] Swift：闭包
来源：http://wfr.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://swh.9152youxi.cn

[T25] Swift：结构体
来源：http://cxc.vqdsnc.cn

struct P { var x: Int }
来源：http://wmx.wangdashe.top

[T26] Swift：类与重写
来源：http://pce.shangyingyoupin.top

class A: Base { override func f() {} }
来源：http://iiv.0kj1m.cn

[T27] Swift：错误处理
来源：http://jfx.cdnleiting.top

do { try f() } catch { print(error) }
来源：http://goh.tianlin.xyz

[T28] Swift：枚举
来源：http://qmi.fehbvm.com

enum Color { case red, green }
来源：http://hmv.0kj1m.cn

[T29] Swift：guard 提前返回
来源：http://reb.hnqzz.top

guard let x = opt else { return }
来源：http://rhn.havefunace.top

[T30] Swift：协议
来源：http://oyb.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://yxo.shanyushiyangtech.top

[T31] Lua：Hello World
来源：http://wrm.0kj1m.cn

print("Hello")
来源：http://psz.epnwcf.com

[T32] Lua：局部变量
来源：http://tfr.nwbrower.top

local a = 1
来源：http://xwi.hammf.cn

[T33] Lua：表（数组）
来源：http://uxc.sweek.top

local t = {1, 2, 3};  t[4] = 4
来源：http://oko.zdqjudy.top

[T34] Lua：遍历表
来源：http://npw.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uep.yuxming.cn

[T35] Lua：字典表
来源：http://xkj.birdmap.top

local d = { a = 1 };  d.b = 2
来源：http://sue.xinyue.icu

[T36] Lua：函数
来源：http://kia.jyoumei.cn

function add(a, b) return a + b end
来源：http://ddp.hywenlv.cn

[T37] Lua：字符串拼接
来源：http://yab.52xcode.cn

"a" .. "b"
来源：http://fcs.ppjwa.cn

[T38] Lua：条件
来源：http://bsa.ctjpmb.com

if x > 0 then print("正") end
来源：http://sgh.yangfankeji.com

[T39] Lua：模式匹配
来源：http://fpo.ppjwa.cn

string.find(s, "%d+")
来源：http://wow.zhongyouzk.top

[T40] Lua：元表
来源：http://ryt.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://yle.fzhhl.top

[T41] Perl：Hello World
来源：http://pxw.feifeiyinyue.top

print "Hello\n";
来源：http://vfg.sweek.top

[T42] Perl：变量类型
来源：http://adw.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kqk.kuanghao11.cn

[T43] Perl：字符串插值
来源：http://mfz.hnqzz.top

"值: $a"
来源：http://njr.guowangkeji.top

[T44] Perl：条件
来源：http://xqh.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://wrg.9152youxi.cn

[T45] Perl：数组遍历
来源：http://ivo.hcnkem.com

for my $x (@arr) { print $x; }
来源：http://zaa.guowangkeji.top

[T46] Perl：哈希操作
来源：http://mcz.quarkkingdee.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zdk.redwolf501.top

[T47] Perl：正则捕获
来源：http://lqn.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://pgr.ctjpmb.com

[T48] Perl：正则替换
来源：http://ghg.shuidangran.top

$s =~ s/old/new/g;
来源：http://qho.zdbjq.cn

[T49] Perl：函数
来源：http://jmk.guannengcc.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tyl.fehbvm.com

[T50] Perl：逐行读文件
来源：http://cec.jqgfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ucx.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://fta.yonumen.top

[T51] Scala：Hello World
来源：http://cpz.fanxiaobao.xyz

println("Hello")
来源：http://ucb.svipenyu.cn

[T52] Scala：变量
来源：http://due.uphjek.com

val a = 1;  var b = 2
来源：http://kjx.zhixingplan.top

[T53] Scala：字符串插值
来源：http://mcp.vehdjk.com

s"值: $b"
来源：http://lio.xziqi.cn

[T54] Scala：集合映射
来源：http://tkv.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://icc.cdnleiting.top

[T55] Scala：集合过滤
来源：http://yov.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://psi.havefunace.top

[T56] Scala：样例类
来源：http://zdq.daxiang520.top

case class User(name: String, age: Int)
来源：http://txr.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://mvp.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xnf.tianlin.xyz

[T58] Scala：函数定义
来源：http://ugx.haohaochexian.top

def add(a: Int, b: Int): Int = a + b
来源：http://rqd.shzxlz.cn

[T59] Scala：循环
来源：http://tsh.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://jmg.wangshuangyany.cn

[T60] Scala：折叠
来源：http://nrl.cdnleiting.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hpc.zhengqikj.top

================================================================================
来源：http://day.jyoumei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://msj.yonumen.top

================================================================================
来源：http://gkk.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://wpf.ppjwa.cn

python -m venv .venv && source .venv/bin/activate
来源：http://urx.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://tlw.zdbjq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hwt.quarkkingdee.top

[U03] Py：加载 .env 配置
来源：http://ezg.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://eqk.wangshuangyany.cn

[U04] Py：变量调试打印
来源：http://ekh.dashuyun.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qzu.jinghuilouyu.cn

[U05] Py：列表去重且保序
来源：http://yze.chenlongwang.top

list(dict.fromkeys(arr))
来源：http://evs.svipenyu.cn

[U06] Py：合并两个字典
来源：http://bqr.jinghuilouyu.cn

{**a, **b}
来源：http://jmb.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://idc.haohaochexian.top

{v: k for k, v in d.items()}
来源：http://iju.tarul.cn

[U08] Py：展平二维列表
来源：http://cja.zhiwuduotai.top

[y for x in nested for y in x]
来源：http://rux.fzhhl.top

[U09] Py：字典取最大值的键
来源：http://cdw.yonumen.top

max(d, key=d.get)
来源：http://ugs.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://gdv.snrcjt.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bvb.fanxiaobao.xyz


<!-- 参考信息 -->