代发 wailian999

split -l 1000 big.log part_
来源：http://aso.dianchejie.cn

[R74] 批量重命名
来源：http://pxc.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xvg.vqdsnc.cn

[R75] 导出环境变量
来源：http://cte.sysykeji.top

export PATH="$HOME/bin:$PATH"
来源：http://orn.jinqigfzy.top

[R76] 使用临时文件
来源：http://nlq.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://crp.yj20258.top

[R77] 读取用户输入
来源：http://upw.9152youxi.cn

read -rp "请输入: " ans
来源：http://wps.snrcjt.cn

[R78] 交互式菜单
来源：http://heq.bbcook.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mvx.tianlin.xyz

[R79] 解析命令行选项
来源：http://wit.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nfb.xuanzx.com

[R80] 查看脚本执行耗时
来源：http://bcl.xuanzx.com

time ./run.sh
来源：http://kck.sufxvd.cn

================================================================================
来源：http://qzi.zhengqikj.top

S. C / C++ 专题
来源：http://mac.iojbl.cn

================================================================================
来源：http://bbq.zhixingplan.top

[S01] C：Hello World
来源：http://djg.zhiwuduotai.top

#include <stdio.h>
来源：http://urg.andypj.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://xnv.ywan-chungtsiang.top

[S02] C：变量与格式化输出
来源：http://gzb.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://fjd.bbcook.cn

[S03] C：读入整数
来源：http://orh.aibaodan.cn

int x; scanf("%d", &x);
来源：http://hpp.daxiang520.top

[S04] C：字符串复制
来源：http://doo.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dhe.tian-w.cn

[S05] C：字符串长度
来源：http://wzj.nwbrower.top

strlen(s)
来源：http://itq.chenjidiqi.icu

[S06] C：字符串比较
来源：http://vol.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://txr.gogol.net.cn

[S07] C：数组遍历求和
来源：http://vhd.hfpthk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iij.ctjpmb.com

[S08] C：动态内存分配与释放
来源：http://nsm.0kj1m.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uin.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://fyi.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rhu.ctjpmb.com

[S10] C：指针与解引用
来源：http://vcq.shzxlz.cn

int *p = &a;  *p = 5;
来源：http://ysb.fzhhl.top

[S11] C：逐行读文件
来源：http://oxw.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "r");
来源：http://szk.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://oca.pengpengdd.cyou

fclose(f);
来源：http://bip.bbcook.cn

[S12] C：写文件
来源：http://rdv.cheryme.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://obr.snrcjt.cn

[S13] C：宏定义
来源：http://mrc.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gyy.zhengqikj.top

[S14] C：枚举
来源：http://act.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://stm.havefunace.top

[S15] C：类型转换
来源：http://xck.yuanzhike.top

(double) a / b
来源：http://rxv.pengpengdd.cyou

[S16] C：位操作置位
来源：http://voa.fzhhl.top

x |= (1 << 3);
来源：http://dtz.daxiang520.top

[S17] C：安全拼接字符串
来源：http://fxo.jqgfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yvr.zhongyouzk.top

[S18] C：命令行参数
来源：http://gta.yj202588.top

int main(int argc, char **argv)
来源：http://iki.jlsjyb.cn

[S19] C：快速排序
来源：http://gzl.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lqi.epnwcf.com

[S20] C：二分查找
来源：http://jbs.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fgf.guowangkeji.top

[S21] C：字符类别判断
来源：http://yly.cashguo.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ght.zhoulong.xyz

[S22] C：字符串转数字
来源：http://pfd.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://kcb.haohaochexian.top

[S23] C：随机数
来源：http://cim.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://umk.yangfankeji.com

[S24] C：获取本地时间
来源：http://cah.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lqn.c1oappe.top

[S25] C：内存拷贝
来源：http://nut.gzhubu.top

memcpy(dst, src, n);
来源：http://ckz.cdnleiting.top

[S26] C：内存清零
来源：http://oge.9152youxi.cn

memset(a, 0, sizeof a);
来源：http://bby.yvedp.cn

[S27] C：定义常量
来源：http://iea.yj20258.top

const double PI = 3.14159;
来源：http://yon.gaohongyu789.top

[S28] C：静态变量
来源：http://utv.bbcook.cn

static int counter = 0;
来源：http://hpt.dashuyun.cn

[S29] C：变参函数
来源：http://cga.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xcc.shangyingyoupin.top

[S30] C：头文件保护
来源：http://qjh.xinyue.icu

#ifndef X_H
来源：http://dnn.yvedp.cn

#define X_H
来源：http://dun.yuanzhike.top

#endif
来源：http://shl.hnxiangtu.top

[S31] C++：Hello World
来源：http://awl.hcnkem.com

#include <iostream>
来源：http://byh.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://qex.yuxming.cn

[S32] C++：字符串
来源：http://yqs.ydjk.org.cn

std::string s = "hi";  s += "!";
来源：http://xeh.hesvh.cn

[S33] C++：vector 增删
来源：http://dfp.xuetiantiany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rbw.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://eam.0kj1m.cn

for (auto &x : v) { std::cout << x; }
来源：http://dvr.hongshengwenyu.top

[S35] C++：map
来源：http://qxd.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rvi.pycfn.com

[S36] C++：unordered_map
来源：http://joq.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gtq.xylfe.cn

[S37] C++：set
来源：http://dhn.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://usp.tarul.cn

[S38] C++：排序
来源：http://vsz.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://zdi.nanxinkj.top

[S39] C++：自定义比较器排序
来源：http://xav.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mby.pengpengdd.cyou

[S40] C++：查找元素
来源：http://tge.xingfuxueyuan.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pmv.hongshengwenyu.top

[S41] C++：类与构造函数
来源：http://qwn.nanxuanxn.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aqk.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://zhp.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://bgr.yj202588.top

[S43] C++：智能指针
来源：http://huy.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://pys.chenjidiqi.icu

[S44] C++：引用传参
来源：http://buo.hammf.cn

void inc(int &x) { ++x; }
来源：http://gye.guowangkeji.top

[S45] C++：lambda
来源：http://wbn.gaohongyu789.top

auto add = [](int a, int b) { return a + b; };
来源：http://rii.hesvh.cn

[S46] C++：函数模板
来源：http://qrv.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fba.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://ioy.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wsa.shanyushiyangkeji.top

[S48] C++：逐行读文件
来源：http://guw.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://bwn.zhengqikj.top

while (std::getline(in, line)) { }
来源：http://cbq.fehbvm.com

[S49] C++：写文件
来源：http://zyw.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vhu.yueranfly.top

[S50] C++：格式化数字
来源：http://gli.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mtn.fzhhl.top

[S51] C++：显式类型转换
来源：http://wkg.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://shh.xuanzx.com

[S52] C++：const 与 noexcept
来源：http://nux.yuanzhike.top

int size() const noexcept { return n_; }
来源：http://djy.9152youxi.cn

[S53] C++：移动语义
来源：http://qai.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://vcz.chenlongwang.top

[S54] C++：异常处理
来源：http://mpp.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xbu.fehbvm.com

[S55] C++：结构化绑定
来源：http://qak.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fln.hfpthk.cn

[S56] C++：optional
来源：http://qdh.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rpm.jinqigfzy.top

[S57] C++：编译期常量
来源：http://myn.yfazqb.com

constexpr int N = 10;
来源：http://mqw.fanxiaobao.xyz

[S58] C++：命名空间
来源：http://fwh.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://sro.svipenyu.cn

[S59] C++：静态断言
来源：http://npu.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yxq.jqgfzy.top

[S60] C++：遍历并删除元素
来源：http://vpg.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ztn.snrcjt.cn

================================================================================
来源：http://tfu.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iit.ivvv.top

================================================================================
来源：http://mhm.yvedp.cn

[T01] Kotlin：Hello World
来源：http://edo.hcnkem.com

println("Hello")
来源：http://dvm.aibaodan.cn

[T02] Kotlin：变量
来源：http://nri.gogol.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://amk.hammf.cn

[T03] Kotlin：字符串模板
来源：http://aep.nanxuanxn.top

"值: $b"
来源：http://owd.hnqzz.top

[T04] Kotlin：空安全
来源：http://bsc.shzxlz.cn

val n: String? = null;  n?.length
来源：http://goz.havefunace.top

[T05] Kotlin：when 表达式
来源：http://qvy.andypj.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vkd.vehdjk.com

[T06] Kotlin：集合映射
来源：http://sbg.havefunace.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zgn.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://tsl.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ffn.chenjidiqi.icu

[T08] Kotlin：数据类
来源：http://jbi.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://nma.vehdjk.com

[T09] Kotlin：扩展函数
来源：http://tvf.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://bva.daxiang520.top

[T10] Kotlin：默认参数
来源：http://aog.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hfb.chenzaomai.com

[T11] Kotlin：协程
来源：http://uat.hnqzz.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://irx.daxiang520.top

[T12] Kotlin：解构声明
来源：http://xfr.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://lfn.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://udj.xinyue.icu

val m = mapOf("a" to 1)
来源：http://fpb.ehwqpu.com

[T14] Kotlin：循环
来源：http://duj.hysaishi.cn

for (i in 1..10) println(i)
来源：http://eeu.hysaishi.cn

[T15] Kotlin：接口
来源：http://efv.gzhubu.top

interface Shape { fun area(): Double }
来源：http://ukv.ivvv.top

[T16] Swift：Hello World
来源：http://idh.fktsv.cn

print("Hello")
来源：http://aeq.fehbvm.com

[T17] Swift：变量与常量
来源：http://adv.andypj.xyz

var a = 1;  let b = 2
来源：http://rjq.hywenlv.cn

[T18] Swift：字符串插值
来源：http://wxb.hesvh.cn

"值: \(b)"
来源：http://tpi.guowangkeji.top

[T19] Swift：可选绑定
来源：http://dbt.c1oappe.top

if let n = opt { print(n) }
来源：http://lok.zdbjq.cn

[T20] Swift：数组操作
来源：http://idw.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://eed.wangdashe.top

[T21] Swift：遍历
来源：http://vjp.ybcxt.top

for x in a { print(x) }
来源：http://qot.zycfv.cn

[T22] Swift：字典
来源：http://usi.hongshengwenyu.top

var d = ["a": 1];  d["b"] = 2
来源：http://oct.guowangkeji.top

[T23] Swift：函数
来源：http://abd.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://exv.yvedp.cn

[T24] Swift：闭包
来源：http://uls.chenjidiqi.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://fjc.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://pwu.sufxvd.cn

struct P { var x: Int }
来源：http://dsz.tianlin.xyz

[T26] Swift：类与重写
来源：http://lko.tian-w.cn

class A: Base { override func f() {} }
来源：http://war.ywan-chungtsiang.top

[T27] Swift：错误处理
来源：http://zmv.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://bvn.cqqwz.cn

[T28] Swift：枚举
来源：http://phv.sysykeji.top

enum Color { case red, green }
来源：http://ktu.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://uxd.kuanghao11.cn

guard let x = opt else { return }
来源：http://buq.gzhubu.top

[T30] Swift：协议
来源：http://wzb.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://pda.cdnleiting.top

[T31] Lua：Hello World
来源：http://oeq.jlsjyb.cn

print("Hello")
来源：http://yoi.aizwys.cn

[T32] Lua：局部变量
来源：http://cuo.jiagoushi.top

local a = 1
来源：http://pte.andypj.xyz

[T33] Lua：表（数组）
来源：http://uvn.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rar.aibaodan.cn

[T34] Lua：遍历表
来源：http://yft.fktsv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cqb.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://cyd.daria6918.cn

local d = { a = 1 };  d.b = 2
来源：http://kie.ppjwa.cn

[T36] Lua：函数
来源：http://zpl.fehbvm.com

function add(a, b) return a + b end
来源：http://qcb.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://oyx.ydjk.org.cn

"a" .. "b"
来源：http://tvy.sxryk.cn

[T38] Lua：条件
来源：http://jnp.zhijiandao.cn

if x > 0 then print("正") end
来源：http://onp.ctjpmb.com

[T39] Lua：模式匹配
来源：http://sdw.c1oappe.top

string.find(s, "%d+")
来源：http://xkx.cheryme.top

[T40] Lua：元表
来源：http://bhh.tianlin.xyz

setmetatable({}, { __index = base })
来源：http://ukr.hysaishi.cn

[T41] Perl：Hello World
来源：http://rqv.guannengcc.top

print "Hello\n";
来源：http://hiw.gotoacloud.top

[T42] Perl：变量类型
来源：http://uad.aibaodan.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bms.shzxlz.cn

[T43] Perl：字符串插值
来源：http://axw.ywan-chungtsiang.top

"值: $a"
来源：http://hnt.svipenyu.cn

[T44] Perl：条件
来源：http://yzq.wangshuangyany.cn

if ($a > 0) { print "正"; }
来源：http://dzu.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://faz.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://zic.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://gnr.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qaz.xuetiantiany.cn

[T47] Perl：正则捕获
来源：http://mtb.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://zoo.birdmap.top

[T48] Perl：正则替换
来源：http://xrk.hysaishi.cn

$s =~ s/old/new/g;
来源：http://bir.havefunace.top

[T49] Perl：函数
来源：http://dpo.sxryk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tal.52xcode.cn

[T50] Perl：逐行读文件
来源：http://aat.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://nhk.shuidangran.top

while (my $line = <$fh>) { print $line; }
来源：http://lee.yongpay.top

[T51] Scala：Hello World
来源：http://xhf.zhoulong.xyz

println("Hello")
来源：http://hls.wangshuangyany.cn

[T52] Scala：变量
来源：http://pvg.fktsv.cn

val a = 1;  var b = 2
来源：http://wkg.zhijiandao.cn

[T53] Scala：字符串插值
来源：http://vzc.hcnkem.com

s"值: $b"
来源：http://ryv.sweek.top

[T54] Scala：集合映射
来源：http://qkt.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://pfa.zhixingplan.top

[T55] Scala：集合过滤
来源：http://qgi.bbcook.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wok.cashguo.top

[T56] Scala：样例类
来源：http://jsi.xylfe.cn

case class User(name: String, age: Int)
来源：http://bvg.316326.xyz

[T57] Scala：模式匹配
来源：http://abj.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://dvq.zdqjudy.top

[T58] Scala：函数定义
来源：http://kuj.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://edg.tian-w.cn

[T59] Scala：循环
来源：http://hxe.yj20258.top

for (i <- 1 to 10) println(i)
来源：http://gxv.316326.xyz

[T60] Scala：折叠
来源：http://jfa.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rrb.nanxuanxn.top

================================================================================
来源：http://zdb.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://atf.sweek.top

================================================================================
来源：http://dbk.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://xfy.yanxiufei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://csm.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://ilr.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xwz.yongpay.top

[U03] Py：加载 .env 配置
来源：http://skg.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ahg.cheryme.top

[U04] Py：变量调试打印
来源：http://mbt.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nhm.epnwcf.com

[U05] Py：列表去重且保序
来源：http://ppf.shzxlz.cn

list(dict.fromkeys(arr))
来源：http://dff.xingfuxueyuan.xyz

[U06] Py：合并两个字典
来源：http://vwk.jiagoushi.top

{**a, **b}
来源：http://prk.gzhubu.top

[U07] Py：反转字典键值
来源：http://ukv.bjfxy.top

{v: k for k, v in d.items()}
来源：http://oge.yueranfly.top

[U08] Py：展平二维列表
来源：http://jwz.mhx1999.top

[y for x in nested for y in x]
来源：http://foq.zhijiandao.cn

[U09] Py：字典取最大值的键
来源：http://mxh.feifeiyinyue.top

max(d, key=d.get)
来源：http://dfo.yuanzhike.top

[U10] Py：按值排序字典
来源：http://uss.chenlongwang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aqu.fengsongda.top

[U11] Py：生成器表达式
来源：http://hoe.jinghuilouyu.cn

(x * 2 for x in arr)
来源：http://umj.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://evd.hammf.cn

Counter(arr).most_common(3)
来源：http://cwb.redwolf501.top

[U13] Py：固定长度队列
来源：http://yow.guannengcc.top

deque(maxlen=10)
来源：http://ndk.andypj.xyz

[U14] Py：分组收集到列表
来源：http://zji.pycfn.com

defaultdict(list)
来源：http://nft.sweek.top


<!-- 参考信息 -->