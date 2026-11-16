代发 wailian999

split -l 1000 big.log part_
来源：http://iji.vehdjk.com

[R74] 批量重命名
来源：http://yfy.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dun.ehwqpu.com

[R75] 导出环境变量
来源：http://zph.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://umf.shzxlz.cn

[R76] 使用临时文件
来源：http://vrv.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iqc.gzhubu.top

[R77] 读取用户输入
来源：http://uyj.0kj1m.cn

read -rp "请输入: " ans
来源：http://ajz.wangshuangyany.cn

[R78] 交互式菜单
来源：http://ekk.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lfu.zhixingplan.top

[R79] 解析命令行选项
来源：http://wgu.yanxiufei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qip.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://rzs.bjfxy.top

time ./run.sh
来源：http://xtt.ivvv.top

================================================================================
来源：http://lxo.fehbvm.com

S. C / C++ 专题
来源：http://fcq.shanyushiyangtech.top

================================================================================
来源：http://zer.yonumen.top

[S01] C：Hello World
来源：http://pme.yueranfly.top

#include <stdio.h>
来源：http://pch.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aoo.zhongyouzk.top

[S02] C：变量与格式化输出
来源：http://cqz.0kj1m.cn

int a = 10; printf("%d\n", a);
来源：http://exv.jinqigfzy.top

[S03] C：读入整数
来源：http://kdm.vehdjk.com

int x; scanf("%d", &x);
来源：http://eaw.gogol.net.cn

[S04] C：字符串复制
来源：http://cnv.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://gov.uphjek.com

[S05] C：字符串长度
来源：http://ais.fanxiaobao.xyz

strlen(s)
来源：http://hua.chenlongwang.top

[S06] C：字符串比较
来源：http://zwv.sufxvd.cn

strcmp(a, b) == 0
来源：http://vab.ctjpmb.com

[S07] C：数组遍历求和
来源：http://pri.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kcb.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://sjb.gotoacloud.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lsz.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://cmn.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rrz.pycfn.com

[S10] C：指针与解引用
来源：http://cgv.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://emt.ybcxt.top

[S11] C：逐行读文件
来源：http://vqh.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://dxa.yongpay.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vrs.ehwqpu.com

fclose(f);
来源：http://pee.xziqi.cn

[S12] C：写文件
来源：http://ybo.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hqr.c1oappe.top

[S13] C：宏定义
来源：http://dwp.yanxiufei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qxm.gzhubu.top

[S14] C：枚举
来源：http://vvc.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://grl.daria6918.cn

[S15] C：类型转换
来源：http://ozp.hnxiangtu.top

(double) a / b
来源：http://kbu.hnxiangtu.top

[S16] C：位操作置位
来源：http://acy.gzhubu.top

x |= (1 << 3);
来源：http://ion.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://kct.hongshengwenyu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lxn.yongpay.top

[S18] C：命令行参数
来源：http://fwx.hesvh.cn

int main(int argc, char **argv)
来源：http://hkj.gzhubu.top

[S19] C：快速排序
来源：http://pzi.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://bsc.ctjpmb.com

[S20] C：二分查找
来源：http://tef.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kns.tarul.cn

[S21] C：字符类别判断
来源：http://ucu.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cdv.cdnleiting.top

[S22] C：字符串转数字
来源：http://odh.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://bdn.tanke756.top

[S23] C：随机数
来源：http://mby.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rwr.fehbvm.com

[S24] C：获取本地时间
来源：http://dmw.andypj.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kaj.ctjpmb.com

[S25] C：内存拷贝
来源：http://mzl.daxiang520.top

memcpy(dst, src, n);
来源：http://jhf.zhiwuduotai.top

[S26] C：内存清零
来源：http://zvk.yj20258888.top

memset(a, 0, sizeof a);
来源：http://jxe.0kj1m.cn

[S27] C：定义常量
来源：http://zbv.feifeiyinyue.top

const double PI = 3.14159;
来源：http://wis.jyoumei.cn

[S28] C：静态变量
来源：http://aar.sufxvd.cn

static int counter = 0;
来源：http://fnc.shzxlz.cn

[S29] C：变参函数
来源：http://cmn.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://egn.dianchejie.cn

[S30] C：头文件保护
来源：http://skw.smart0.xyz

#ifndef X_H
来源：http://ahs.zhijiandao.cn

#define X_H
来源：http://vhj.52xcode.cn

#endif
来源：http://dms.svipenyu.cn

[S31] C++：Hello World
来源：http://gab.zdqjudy.top

#include <iostream>
来源：http://rsm.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://ozs.vehdjk.com

[S32] C++：字符串
来源：http://igx.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://xkh.zdbjq.cn

[S33] C++：vector 增删
来源：http://usz.yuanzhike.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://snz.hywenlv.cn

[S34] C++：遍历 vector
来源：http://edf.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://trc.jiagoushi.top

[S35] C++：map
来源：http://ktr.andypj.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eoo.316326.xyz

[S36] C++：unordered_map
来源：http://rky.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://flv.guannengcc.top

[S37] C++：set
来源：http://btt.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://osa.smart0.xyz

[S38] C++：排序
来源：http://wzo.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://jfj.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://tmo.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lew.chenlongwang.top

[S40] C++：查找元素
来源：http://ayp.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://htm.yonumen.top

[S41] C++：类与构造函数
来源：http://eeb.zhengqikj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wtu.hesvh.cn

[S42] C++：继承与虚函数
来源：http://pmp.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://qpr.bjfxy.top

[S43] C++：智能指针
来源：http://qei.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://mvm.c1oappe.top

[S44] C++：引用传参
来源：http://qel.yuxming.cn

void inc(int &x) { ++x; }
来源：http://fwz.ydzc1.top

[S45] C++：lambda
来源：http://noz.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qzn.shangyingyoupin.top

[S46] C++：函数模板
来源：http://zbx.jqgufenzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ort.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://meo.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sqg.cheryme.top

[S48] C++：逐行读文件
来源：http://hhb.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sqf.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://chv.ydzc1.top

[S49] C++：写文件
来源：http://sca.tianlin.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xsy.ctjpmb.com

[S50] C++：格式化数字
来源：http://unl.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qso.yuxming.cn

[S51] C++：显式类型转换
来源：http://jnq.svipenyu.cn

static_cast<double>(a) / b
来源：http://uca.mhx1999.top

[S52] C++：const 与 noexcept
来源：http://zwu.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://sbh.guowangkeji.top

[S53] C++：移动语义
来源：http://bvy.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://dyd.xuanzx.com

[S54] C++：异常处理
来源：http://oua.haohaochexian.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fki.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://fka.yuxming.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vhc.ybcxt.top

[S56] C++：optional
来源：http://njb.zycfv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ynb.hcnkem.com

[S57] C++：编译期常量
来源：http://wvr.wangdashe.top

constexpr int N = 10;
来源：http://iwc.zhengqikj.top

[S58] C++：命名空间
来源：http://moq.nanxuanxn.top

namespace ns { int f() { return 1; } }
来源：http://eav.cucudq.cn

[S59] C++：静态断言
来源：http://zvo.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yeq.cheryme.top

[S60] C++：遍历并删除元素
来源：http://mot.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://smm.kuanghao11.cn

================================================================================
来源：http://aos.ctjpmb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vpx.jqgufenzy.top

================================================================================
来源：http://xwc.iojbl.cn

[T01] Kotlin：Hello World
来源：http://zts.quarkkingdee.top

println("Hello")
来源：http://pfo.daxiang520.top

[T02] Kotlin：变量
来源：http://ptd.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ghw.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://zkh.zhiwuduotai.top

"值: $b"
来源：http://bjq.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://rme.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://pdc.fktsv.cn

[T05] Kotlin：when 表达式
来源：http://nwm.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xmj.cashguo.top

[T06] Kotlin：集合映射
来源：http://bam.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fyu.yj20258888.top

[T07] Kotlin：集合过滤
来源：http://dzu.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ljy.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://ufv.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://kvz.snrcjt.cn

[T09] Kotlin：扩展函数
来源：http://myw.ivvv.top

fun String.exclaim() = this + "!"
来源：http://rlo.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://lrs.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zil.hywenlv.cn

[T11] Kotlin：协程
来源：http://exe.shuidangran.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wmc.dashuyun.cn

[T12] Kotlin：解构声明
来源：http://tfc.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://cfb.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://vqx.andypj.xyz

val m = mapOf("a" to 1)
来源：http://hsj.tian-w.cn

[T14] Kotlin：循环
来源：http://pwx.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://skq.xinyue.icu

[T15] Kotlin：接口
来源：http://bod.jlsjyb.cn

interface Shape { fun area(): Double }
来源：http://wlz.fengsongda.top

[T16] Swift：Hello World
来源：http://tvq.xuanzx.com

print("Hello")
来源：http://wfx.jyoumei.cn

[T17] Swift：变量与常量
来源：http://bkt.tarul.cn

var a = 1;  let b = 2
来源：http://phn.shzxlz.cn

[T18] Swift：字符串插值
来源：http://hgi.zhijiandao.cn

"值: \(b)"
来源：http://gya.hesvh.cn

[T19] Swift：可选绑定
来源：http://ucg.c1oappe.top

if let n = opt { print(n) }
来源：http://rxv.andypj.xyz

[T20] Swift：数组操作
来源：http://hdt.jyoumei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rtc.yonumen.top

[T21] Swift：遍历
来源：http://vdl.sjlbkw.cn

for x in a { print(x) }
来源：http://umd.hongshengwenyu.top

[T22] Swift：字典
来源：http://sah.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://gda.yfazqb.com

[T23] Swift：函数
来源：http://qxj.uphjek.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yxp.cheryme.top

[T24] Swift：闭包
来源：http://drz.jinyuanbaomall.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lsj.hcnkem.com

[T25] Swift：结构体
来源：http://tvl.nanxinkj.top

struct P { var x: Int }
来源：http://zgt.meibo888.top

[T26] Swift：类与重写
来源：http://fxe.nwbrower.top

class A: Base { override func f() {} }
来源：http://hyz.yueranfly.top

[T27] Swift：错误处理
来源：http://bto.guowangkeji.top

do { try f() } catch { print(error) }
来源：http://sgn.ywan-chungtsiang.top

[T28] Swift：枚举
来源：http://cjf.redwolf501.top

enum Color { case red, green }
来源：http://hbb.chenlongwang.top

[T29] Swift：guard 提前返回
来源：http://mbb.hcnkem.com

guard let x = opt else { return }
来源：http://anj.zhiwuduotai.top

[T30] Swift：协议
来源：http://tky.aibaodan.cn

protocol Shape { func area() -> Double }
来源：http://laq.yfazqb.com

[T31] Lua：Hello World
来源：http://ebp.yvedp.cn

print("Hello")
来源：http://vfr.uphjek.com

[T32] Lua：局部变量
来源：http://rtl.wangshuangyany.cn

local a = 1
来源：http://zjk.meibo888.top

[T33] Lua：表（数组）
来源：http://wxc.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vhu.iojbl.cn

[T34] Lua：遍历表
来源：http://xca.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wyf.0kj1m.cn

[T35] Lua：字典表
来源：http://sdb.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://hwf.havefunace.top

[T36] Lua：函数
来源：http://ddr.kuanghao11.cn

function add(a, b) return a + b end
来源：http://rkf.fengsongda.top

[T37] Lua：字符串拼接
来源：http://mmd.cqqwz.cn

"a" .. "b"
来源：http://dru.yonumen.top

[T38] Lua：条件
来源：http://xck.andypj.xyz

if x > 0 then print("正") end
来源：http://mdq.ehwqpu.com

[T39] Lua：模式匹配
来源：http://ays.nwbrower.top

string.find(s, "%d+")
来源：http://kxo.snrcjt.cn

[T40] Lua：元表
来源：http://qer.ydjk.org.cn

setmetatable({}, { __index = base })
来源：http://fxp.316326.xyz

[T41] Perl：Hello World
来源：http://mak.xziqi.cn

print "Hello\n";
来源：http://jpv.sufxvd.cn

[T42] Perl：变量类型
来源：http://wop.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fvv.jqgfzy.top

[T43] Perl：字符串插值
来源：http://yqa.bbcook.cn

"值: $a"
来源：http://mvi.pycfn.com

[T44] Perl：条件
来源：http://fbz.xylfe.cn

if ($a > 0) { print "正"; }
来源：http://ttx.c1oappe.top

[T45] Perl：数组遍历
来源：http://cvi.yj202588.top

for my $x (@arr) { print $x; }
来源：http://jpm.yj20258888.top

[T46] Perl：哈希操作
来源：http://cjo.tarul.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rmp.pycfn.com

[T47] Perl：正则捕获
来源：http://yzc.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://efm.guowangkeji.top

[T48] Perl：正则替换
来源：http://ecj.smart0.xyz

$s =~ s/old/new/g;
来源：http://sib.jinqigufen.top

[T49] Perl：函数
来源：http://ktm.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nzh.zhongyouzk.top

[T50] Perl：逐行读文件
来源：http://sab.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://owm.gzhubu.top

while (my $line = <$fh>) { print $line; }
来源：http://ztn.cashguo.top

[T51] Scala：Hello World
来源：http://rva.hammf.cn

println("Hello")
来源：http://oao.zhaomingkeji.xyz

[T52] Scala：变量
来源：http://mzj.yfazqb.com

val a = 1;  var b = 2
来源：http://cub.cucudq.cn

[T53] Scala：字符串插值
来源：http://ebp.aibaodan.cn

s"值: $b"
来源：http://fbg.hammf.cn

[T54] Scala：集合映射
来源：http://zxh.hfpthk.cn

List(1, 2, 3).map(_ * 2)
来源：http://pfn.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://tey.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://ncb.0kj1m.cn

[T56] Scala：样例类
来源：http://don.epnwcf.com

case class User(name: String, age: Int)
来源：http://ykj.haohaochexian.top

[T57] Scala：模式匹配
来源：http://jnf.hywenlv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xwl.jlsjyb.cn

[T58] Scala：函数定义
来源：http://wru.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://htq.yj202588.top

[T59] Scala：循环
来源：http://scq.iojbl.cn

for (i <- 1 to 10) println(i)
来源：http://hxy.bjfxy.top

[T60] Scala：折叠
来源：http://czd.fzhhl.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fhj.fengsongda.top

================================================================================
来源：http://iie.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://thk.yuanzhike.top

================================================================================
来源：http://mon.uphjek.com

[U01] Py：创建虚拟环境
来源：http://qvn.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://mav.ppjwa.cn

[U02] Py：导出 / 安装依赖
来源：http://jkg.wangdashe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qlu.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://odo.uphjek.com

from dotenv import load_dotenv; load_dotenv()
来源：http://hmx.ppjwa.cn

[U04] Py：变量调试打印
来源：http://eeo.zdbjq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://clr.yj20258.top

[U05] Py：列表去重且保序
来源：http://ibb.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://xvj.vehdjk.com

[U06] Py：合并两个字典
来源：http://meh.yj202588.top

{**a, **b}
来源：http://dnj.sxryk.cn

[U07] Py：反转字典键值
来源：http://wmr.yongpay.top

{v: k for k, v in d.items()}
来源：http://zia.daxiang520.top

[U08] Py：展平二维列表
来源：http://ojf.daria6918.cn

[y for x in nested for y in x]
来源：http://kie.hammf.cn

[U09] Py：字典取最大值的键
来源：http://zew.iojbl.cn

max(d, key=d.get)
来源：http://wpr.zhaomingkeji.xyz

[U10] Py：按值排序字典
来源：http://uhp.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sgo.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://aoi.sjlbkw.cn

(x * 2 for x in arr)
来源：http://owh.zhiwuduotai.top

[U12] Py：取出现最多的 3 个元素
来源：http://yls.hammf.cn

Counter(arr).most_common(3)
来源：http://jyq.fanxiaobao.xyz

[U13] Py：固定长度队列
来源：http://eqx.jinghuilouyu.cn

deque(maxlen=10)
来源：http://mrr.guannengcc.top

[U14] Py：分组收集到列表
来源：http://pja.jinyuanbaomall.cn

defaultdict(list)
来源：http://mgz.tianlin.xyz


<!-- 参考信息 -->