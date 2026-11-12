代发 wailian999

read -rp "请输入: " ans
来源：http://mqx.smart0.xyz

[R78] 交互式菜单
来源：http://fuh.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dua.chenzaomai.com

[R79] 解析命令行选项
来源：http://wxe.xziqi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sgt.hnxiangtu.top

[R80] 查看脚本执行耗时
来源：http://oca.sysykeji.top

time ./run.sh
来源：http://nct.zhaomingkeji.xyz

================================================================================
来源：http://pfu.hcnkem.com

S. C / C++ 专题
来源：http://yez.yuxming.cn

================================================================================
来源：http://vwe.ctjpmb.com

[S01] C：Hello World
来源：http://oma.nanxuanxn.top

#include <stdio.h>
来源：http://ijx.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vlw.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://gwu.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://drc.xinyue.icu

[S03] C：读入整数
来源：http://mco.shzxlz.cn

int x; scanf("%d", &x);
来源：http://snl.ivvv.top

[S04] C：字符串复制
来源：http://wth.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://wfj.zhoulong.xyz

[S05] C：字符串长度
来源：http://cmw.pycfn.com

strlen(s)
来源：http://sxw.0kj1m.cn

[S06] C：字符串比较
来源：http://kld.hfpthk.cn

strcmp(a, b) == 0
来源：http://erg.zhixingplan.top

[S07] C：数组遍历求和
来源：http://tty.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bkn.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://ukd.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ncd.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://ior.cashguo.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xbc.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://bor.yangfankeji.com

int *p = &a;  *p = 5;
来源：http://twd.vehdjk.com

[S11] C：逐行读文件
来源：http://otz.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://ibo.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://iqf.zhengqikj.top

fclose(f);
来源：http://nkt.xylfe.cn

[S12] C：写文件
来源：http://czp.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wme.sysykeji.top

[S13] C：宏定义
来源：http://prz.cashguo.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jte.wangshuangyany.cn

[S14] C：枚举
来源：http://kvx.snrcjt.cn

enum Color { RED, GREEN, BLUE };
来源：http://ezi.aibaodan.cn

[S15] C：类型转换
来源：http://yok.hysaishi.cn

(double) a / b
来源：http://ffb.nanxinkj.top

[S16] C：位操作置位
来源：http://plc.haohaochexian.top

x |= (1 << 3);
来源：http://qfj.316326.xyz

[S17] C：安全拼接字符串
来源：http://hfo.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sse.redwolf501.top

[S18] C：命令行参数
来源：http://oip.zhoulong.xyz

int main(int argc, char **argv)
来源：http://emr.fengsongda.top

[S19] C：快速排序
来源：http://ttu.sjlbkw.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yug.quarkkingdee.top

[S20] C：二分查找
来源：http://mwa.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vru.haohaochexian.top

[S21] C：字符类别判断
来源：http://jse.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lym.zycfv.cn

[S22] C：字符串转数字
来源：http://edf.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qjj.tianlin.xyz

[S23] C：随机数
来源：http://fyy.shanyushiyangtech.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tfa.jinqigfzy.top

[S24] C：获取本地时间
来源：http://nqm.tianlin.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qej.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://huc.aibaodan.cn

memcpy(dst, src, n);
来源：http://ddw.havefunace.top

[S26] C：内存清零
来源：http://ryb.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://yaj.wangshuangyany.cn

[S27] C：定义常量
来源：http://ghe.zdqjudy.top

const double PI = 3.14159;
来源：http://xqx.daria6918.cn

[S28] C：静态变量
来源：http://hfp.ydzc1.top

static int counter = 0;
来源：http://qut.xuanzx.com

[S29] C：变参函数
来源：http://yrh.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mri.fehbvm.com

[S30] C：头文件保护
来源：http://hje.yfazqb.com

#ifndef X_H
来源：http://epo.epnwcf.com

#define X_H
来源：http://twh.dianchejie.cn

#endif
来源：http://zyo.hysaishi.cn

[S31] C++：Hello World
来源：http://jlr.fehbvm.com

#include <iostream>
来源：http://lih.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://sag.guowangkeji.top

[S32] C++：字符串
来源：http://tdl.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://bmi.9152youxi.cn

[S33] C++：vector 增删
来源：http://fae.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kef.tianlin.xyz

[S34] C++：遍历 vector
来源：http://ojo.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://ouq.dashuyun.cn

[S35] C++：map
来源：http://qnb.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ojn.ydjk.org.cn

[S36] C++：unordered_map
来源：http://fhw.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mfv.zhixingplan.top

[S37] C++：set
来源：http://vsf.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://szg.guannengcc.top

[S38] C++：排序
来源：http://fuc.xinyue.icu

std::sort(v.begin(), v.end());
来源：http://god.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://mjd.xinyue.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ron.hnqzz.top

[S40] C++：查找元素
来源：http://rtn.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ilt.guowangkeji.top

[S41] C++：类与构造函数
来源：http://jho.ppjwa.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xvf.havefunace.top

[S42] C++：继承与虚函数
来源：http://smb.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://pvz.jinqigufen.top

[S43] C++：智能指针
来源：http://yjy.svipenyu.cn

auto p = std::make_unique<int>(5);
来源：http://hed.yvedp.cn

[S44] C++：引用传参
来源：http://yqm.hesvh.cn

void inc(int &x) { ++x; }
来源：http://xad.jyoumei.cn

[S45] C++：lambda
来源：http://xcl.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://qyq.dashuyun.cn

[S46] C++：函数模板
来源：http://ltr.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fux.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://sxo.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zub.xingfuxueyuan.xyz

[S48] C++：逐行读文件
来源：http://bhv.nanxinkj.top

std::ifstream in("a.txt");  std::string line;
来源：http://bxp.hammf.cn

while (std::getline(in, line)) { }
来源：http://bif.xinyue.icu

[S49] C++：写文件
来源：http://epv.meibo888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dyw.vehdjk.com

[S50] C++：格式化数字
来源：http://nes.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://die.cdnleiting.top

[S51] C++：显式类型转换
来源：http://mkh.sweek.top

static_cast<double>(a) / b
来源：http://qup.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://sti.ydzc1.top

int size() const noexcept { return n_; }
来源：http://rgo.zhiwuduotai.top

[S53] C++：移动语义
来源：http://xho.aizwys.cn

std::vector<int> w = std::move(v);
来源：http://exz.yvedp.cn

[S54] C++：异常处理
来源：http://oic.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uco.iojbl.cn

[S55] C++：结构化绑定
来源：http://kpq.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hdz.shanyushiyangtech.top

[S56] C++：optional
来源：http://hqg.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dvy.sxryk.cn

[S57] C++：编译期常量
来源：http://gnd.jyoumei.cn

constexpr int N = 10;
来源：http://gaa.gotoacloud.top

[S58] C++：命名空间
来源：http://upm.jinghuilouyu.cn

namespace ns { int f() { return 1; } }
来源：http://qse.c1oappe.top

[S59] C++：静态断言
来源：http://tsq.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://smx.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://erh.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tfg.tarul.cn

================================================================================
来源：http://ncc.nanxinkj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wkr.zhoulong.xyz

================================================================================
来源：http://cqc.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://xks.sxryk.cn

println("Hello")
来源：http://jsk.yuxming.cn

[T02] Kotlin：变量
来源：http://eim.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jxx.gogol.net.cn

[T03] Kotlin：字符串模板
来源：http://vpa.jlsjyb.cn

"值: $b"
来源：http://upu.zdqjudy.top

[T04] Kotlin：空安全
来源：http://fyl.aizwys.cn

val n: String? = null;  n?.length
来源：http://zaw.bbcook.cn

[T05] Kotlin：when 表达式
来源：http://rve.hnqzz.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tmx.xinyue.icu

[T06] Kotlin：集合映射
来源：http://tri.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oob.jianghu66.top

[T07] Kotlin：集合过滤
来源：http://rcq.xylfe.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pkg.nanxuanxn.top

[T08] Kotlin：数据类
来源：http://dfr.jinghuilouyu.cn

data class User(val name: String, val age: Int)
来源：http://lju.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://btb.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://rsw.smart0.xyz

[T10] Kotlin：默认参数
来源：http://wkb.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zhc.jianghu66.top

[T11] Kotlin：协程
来源：http://hcn.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://obn.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://xaz.hongshengwenyu.top

val (a, b) = Pair(1, 2)
来源：http://hae.ivvv.top

[T13] Kotlin：只读 Map
来源：http://ogw.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://pwy.zdqjudy.top

[T14] Kotlin：循环
来源：http://sna.tarul.cn

for (i in 1..10) println(i)
来源：http://yib.zhongyouzk.top

[T15] Kotlin：接口
来源：http://vjl.shanyushiyangkeji.top

interface Shape { fun area(): Double }
来源：http://rmf.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://yql.ywan-chungtsiang.top

print("Hello")
来源：http://ofu.cucudq.cn

[T17] Swift：变量与常量
来源：http://tun.0kj1m.cn

var a = 1;  let b = 2
来源：http://uei.jiagoushi.top

[T18] Swift：字符串插值
来源：http://bbm.zhijiandao.cn

"值: \(b)"
来源：http://olb.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://gth.nwbrower.top

if let n = opt { print(n) }
来源：http://hdu.sufxvd.cn

[T20] Swift：数组操作
来源：http://agr.jinqigufen.top

var a = [1, 2, 3];  a.append(4)
来源：http://tbz.zycfv.cn

[T21] Swift：遍历
来源：http://ntm.dianchejie.cn

for x in a { print(x) }
来源：http://rxr.tanke756.top

[T22] Swift：字典
来源：http://nsa.sxryk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nwk.chenjidiqi.icu

[T23] Swift：函数
来源：http://nmv.uphjek.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lrp.wangdashe.top

[T24] Swift：闭包
来源：http://ssf.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xte.tarul.cn

[T25] Swift：结构体
来源：http://orz.yanxiufei.cn

struct P { var x: Int }
来源：http://twa.hywenlv.cn

[T26] Swift：类与重写
来源：http://non.uphjek.com

class A: Base { override func f() {} }
来源：http://xsg.chenzaomai.com

[T27] Swift：错误处理
来源：http://xql.zhiwuduotai.top

do { try f() } catch { print(error) }
来源：http://waq.xziqi.cn

[T28] Swift：枚举
来源：http://akq.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://wkn.havefunace.top

[T29] Swift：guard 提前返回
来源：http://hnd.ivvv.top

guard let x = opt else { return }
来源：http://ovt.jianghu66.top

[T30] Swift：协议
来源：http://abx.hywenlv.cn

protocol Shape { func area() -> Double }
来源：http://udm.yuanzhike.top

[T31] Lua：Hello World
来源：http://oog.yuanzhike.top

print("Hello")
来源：http://rtw.nwbrower.top

[T32] Lua：局部变量
来源：http://tbl.gaohongyu789.top

local a = 1
来源：http://hxs.sysykeji.top

[T33] Lua：表（数组）
来源：http://brw.xingfuxueyuan.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://fpw.havefunace.top

[T34] Lua：遍历表
来源：http://hzq.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gos.wangshuangyany.cn

[T35] Lua：字典表
来源：http://csz.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://bql.pycfn.com

[T36] Lua：函数
来源：http://acs.zycfv.cn

function add(a, b) return a + b end
来源：http://nvr.316326.xyz

[T37] Lua：字符串拼接
来源：http://thu.316326.xyz

"a" .. "b"
来源：http://frm.hcnkem.com

[T38] Lua：条件
来源：http://kmy.meibo888.top

if x > 0 then print("正") end
来源：http://jly.yfazqb.com

[T39] Lua：模式匹配
来源：http://fnx.sysykeji.top

string.find(s, "%d+")
来源：http://rgq.yuanzhike.top

[T40] Lua：元表
来源：http://wmx.hesvh.cn

setmetatable({}, { __index = base })
来源：http://yde.daria6918.cn

[T41] Perl：Hello World
来源：http://pma.52xcode.cn

print "Hello\n";
来源：http://nmd.gzhubu.top

[T42] Perl：变量类型
来源：http://dbo.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rge.nwbrower.top

[T43] Perl：字符串插值
来源：http://wri.jinghuilouyu.cn

"值: $a"
来源：http://nqb.hnxiangtu.top

[T44] Perl：条件
来源：http://aza.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://uco.hnxiangtu.top

[T45] Perl：数组遍历
来源：http://few.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://mxl.jinghuilouyu.cn

[T46] Perl：哈希操作
来源：http://oya.c1oappe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://myc.zdqjudy.top

[T47] Perl：正则捕获
来源：http://nlk.xingfuxueyuan.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://aam.hywenlv.cn

[T48] Perl：正则替换
来源：http://cqy.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://qet.jianghu66.top

[T49] Perl：函数
来源：http://aqs.fzhhl.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tzy.yj20258.top

[T50] Perl：逐行读文件
来源：http://gbt.andypj.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://qyk.wangdashe.top

while (my $line = <$fh>) { print $line; }
来源：http://mjo.xuanzx.com

[T51] Scala：Hello World
来源：http://njn.xinyue.icu

println("Hello")
来源：http://xbm.ydzc1.top

[T52] Scala：变量
来源：http://zcg.daria6918.cn

val a = 1;  var b = 2
来源：http://zar.andypj.xyz

[T53] Scala：字符串插值
来源：http://gyb.zdqjudy.top

s"值: $b"
来源：http://ihp.jinqigfzy.top

[T54] Scala：集合映射
来源：http://eyo.yj202588.top

List(1, 2, 3).map(_ * 2)
来源：http://qgr.9152youxi.cn

[T55] Scala：集合过滤
来源：http://vdm.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://scr.zhongyouzk.top

[T56] Scala：样例类
来源：http://buc.gzhubu.top

case class User(name: String, age: Int)
来源：http://hry.ybcxt.top

[T57] Scala：模式匹配
来源：http://cta.yuanzhike.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tyu.cucudq.cn

[T58] Scala：函数定义
来源：http://ztn.yj20258.top

def add(a: Int, b: Int): Int = a + b
来源：http://fzn.fktsv.cn

[T59] Scala：循环
来源：http://hot.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://qno.sufxvd.cn

[T60] Scala：折叠
来源：http://glx.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xkn.jinghuilouyu.cn

================================================================================
来源：http://kbt.aizwys.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qwa.jianghu66.top

================================================================================
来源：http://nlg.zhiwuduotai.top

[U01] Py：创建虚拟环境
来源：http://znu.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://grf.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://jdo.vqdsnc.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zbo.sxryk.cn

[U03] Py：加载 .env 配置
来源：http://bxt.yangfankeji.com

from dotenv import load_dotenv; load_dotenv()
来源：http://uok.nwbrower.top

[U04] Py：变量调试打印
来源：http://avc.nanxuanxn.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://trv.bjfxy.top

[U05] Py：列表去重且保序
来源：http://fej.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://ehd.shanyushiyangkeji.top

[U06] Py：合并两个字典
来源：http://sck.52xcode.cn

{**a, **b}
来源：http://hhr.guowangkeji.top

[U07] Py：反转字典键值
来源：http://soz.daria6918.cn

{v: k for k, v in d.items()}
来源：http://sne.hysaishi.cn

[U08] Py：展平二维列表
来源：http://cwr.ydzc1.top

[y for x in nested for y in x]
来源：http://wui.jianghu66.top

[U09] Py：字典取最大值的键
来源：http://bft.xziqi.cn

max(d, key=d.get)
来源：http://fpt.vqdsnc.cn

[U10] Py：按值排序字典
来源：http://www.yuxming.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ijw.sufxvd.cn

[U11] Py：生成器表达式
来源：http://psq.hnqzz.top

(x * 2 for x in arr)
来源：http://vyz.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fah.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://nad.xuetiantiany.cn

[U13] Py：固定长度队列
来源：http://eul.ctjpmb.com

deque(maxlen=10)
来源：http://kpu.jianghu66.top

[U14] Py：分组收集到列表
来源：http://qbo.chenlongwang.top

defaultdict(list)
来源：http://mvf.uphjek.com

[U15] Py：高精度计时
来源：http://gle.birdmap.top

t = time.perf_counter()
来源：http://ykz.feifeiyinyue.top

[U16] Py：命令行参数解析
来源：http://blz.zhengqikj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rsn.tianlin.xyz

[U17] Py：初始化日志
来源：http://ghp.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://jkj.svipenyu.cn

[U18] Py：预编译正则
来源：http://sqn.bbcook.cn

pat = re.compile(r"\d+")
来源：http://uzw.yuxming.cn


<!-- 参考信息 -->