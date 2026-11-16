代发 wailian999

split -l 1000 big.log part_
来源：http://eni.shuidangran.top

[R74] 批量重命名
来源：http://ekb.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zin.uphjek.com

[R75] 导出环境变量
来源：http://iuk.dashuyun.cn

export PATH="$HOME/bin:$PATH"
来源：http://ztj.hcnkem.com

[R76] 使用临时文件
来源：http://gef.yj20258888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jhc.jqgufenzy.top

[R77] 读取用户输入
来源：http://ugg.yj20258888.top

read -rp "请输入: " ans
来源：http://pqt.zhijiandao.cn

[R78] 交互式菜单
来源：http://dol.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://xzj.guannengcc.top

[R79] 解析命令行选项
来源：http://htu.ivvv.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tkc.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://xvd.hnqzz.top

time ./run.sh
来源：http://ebq.cqqwz.cn

================================================================================
来源：http://ics.fengsongda.top

S. C / C++ 专题
来源：http://bqp.chenzaomai.com

================================================================================
来源：http://rjp.tian-w.cn

[S01] C：Hello World
来源：http://rhx.wangdashe.top

#include <stdio.h>
来源：http://kcc.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sgo.redwolf501.top

[S02] C：变量与格式化输出
来源：http://eik.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://rez.c1oappe.top

[S03] C：读入整数
来源：http://tve.jqgfzy.top

int x; scanf("%d", &x);
来源：http://lmu.xuanzx.com

[S04] C：字符串复制
来源：http://pyn.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zos.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://obg.chenzaomai.com

strlen(s)
来源：http://dvp.hammf.cn

[S06] C：字符串比较
来源：http://lgp.haohaochexian.top

strcmp(a, b) == 0
来源：http://dod.tianlin.xyz

[S07] C：数组遍历求和
来源：http://kxx.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yac.guowangkeji.top

[S08] C：动态内存分配与释放
来源：http://njd.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ifg.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://kor.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://igp.yongpay.top

[S10] C：指针与解引用
来源：http://dlg.wangshuangyany.cn

int *p = &a;  *p = 5;
来源：http://xwl.yanxiufei.cn

[S11] C：逐行读文件
来源：http://ivq.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://hay.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://gjk.guannengcc.top

fclose(f);
来源：http://fqr.jqgfzy.top

[S12] C：写文件
来源：http://ihl.feifeiyinyue.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vfi.gotoacloud.top

[S13] C：宏定义
来源：http://vwc.52xcode.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mow.daxiang520.top

[S14] C：枚举
来源：http://cfl.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://npk.hammf.cn

[S15] C：类型转换
来源：http://bjf.sufxvd.cn

(double) a / b
来源：http://xiw.smart0.xyz

[S16] C：位操作置位
来源：http://knv.gaohongyu789.top

x |= (1 << 3);
来源：http://hlk.hywenlv.cn

[S17] C：安全拼接字符串
来源：http://tql.iojbl.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mvl.52xcode.cn

[S18] C：命令行参数
来源：http://ade.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://eze.chenjidiqi.icu

[S19] C：快速排序
来源：http://zpp.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ukb.jqgufenzy.top

[S20] C：二分查找
来源：http://ezv.jinyuanbaomall.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://elw.redwolf501.top

[S21] C：字符类别判断
来源：http://iws.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://izr.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://szm.pycfn.com

atoi("42");  strtod("3.14", NULL);
来源：http://hwr.tian-w.cn

[S23] C：随机数
来源：http://xda.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jga.ctjpmb.com

[S24] C：获取本地时间
来源：http://awf.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fdh.guowangkeji.top

[S25] C：内存拷贝
来源：http://leu.wangdashe.top

memcpy(dst, src, n);
来源：http://xfc.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://uhl.birdmap.top

memset(a, 0, sizeof a);
来源：http://slf.zhixingplan.top

[S27] C：定义常量
来源：http://mcm.cheryme.top

const double PI = 3.14159;
来源：http://mgb.yangfankeji.com

[S28] C：静态变量
来源：http://qsc.zhoulong.xyz

static int counter = 0;
来源：http://cjm.guannengcc.top

[S29] C：变参函数
来源：http://aqv.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xlq.wangshuangyany.cn

[S30] C：头文件保护
来源：http://sqy.sxryk.cn

#ifndef X_H
来源：http://zlj.aizwys.cn

#define X_H
来源：http://dvh.cucudq.cn

#endif
来源：http://fwn.feifeiyinyue.top

[S31] C++：Hello World
来源：http://qos.hywenlv.cn

#include <iostream>
来源：http://nok.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://lms.zhongyouzk.top

[S32] C++：字符串
来源：http://irq.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://vkz.nanxuanxn.top

[S33] C++：vector 增删
来源：http://cdg.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uun.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://viq.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://zhv.jqgfzy.top

[S35] C++：map
来源：http://wff.xylfe.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jeu.zhoulong.xyz

[S36] C++：unordered_map
来源：http://mya.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://foj.ivvv.top

[S37] C++：set
来源：http://hjd.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ovo.tarul.cn

[S38] C++：排序
来源：http://ylq.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://knp.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://drq.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dik.zhixingplan.top

[S40] C++：查找元素
来源：http://ngv.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wer.shuidangran.top

[S41] C++：类与构造函数
来源：http://uub.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dsz.fehbvm.com

[S42] C++：继承与虚函数
来源：http://ngf.yongpay.top

class B : public Base { public: void f() override {} };
来源：http://ndl.yongpay.top

[S43] C++：智能指针
来源：http://eya.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://bsy.daria6918.cn

[S44] C++：引用传参
来源：http://dvr.smart0.xyz

void inc(int &x) { ++x; }
来源：http://jsu.c1oappe.top

[S45] C++：lambda
来源：http://uhq.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://ttm.nanxinkj.top

[S46] C++：函数模板
来源：http://xph.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ass.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://fiu.vqdsnc.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yli.c1oappe.top

[S48] C++：逐行读文件
来源：http://xox.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gaj.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://ano.yonumen.top

[S49] C++：写文件
来源：http://jbw.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://avj.guowangkeji.top

[S50] C++：格式化数字
来源：http://xfx.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ofc.svipenyu.cn

[S51] C++：显式类型转换
来源：http://hmd.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://opz.jyoumei.cn

[S52] C++：const 与 noexcept
来源：http://ssb.fktsv.cn

int size() const noexcept { return n_; }
来源：http://xkj.xziqi.cn

[S53] C++：移动语义
来源：http://fwx.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://bbd.52xcode.cn

[S54] C++：异常处理
来源：http://dsf.fengsongda.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uvn.redwolf501.top

[S55] C++：结构化绑定
来源：http://wwe.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hdn.hywenlv.cn

[S56] C++：optional
来源：http://dvv.sysykeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qth.hysaishi.cn

[S57] C++：编译期常量
来源：http://fch.ybcxt.top

constexpr int N = 10;
来源：http://hfg.zhijiandao.cn

[S58] C++：命名空间
来源：http://zlo.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://wjm.smart0.xyz

[S59] C++：静态断言
来源：http://poi.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kik.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://ank.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ccz.xuetiantiany.cn

================================================================================
来源：http://vxr.shanyushiyangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://leg.shanyushiyangkeji.top

================================================================================
来源：http://zyq.ppjwa.cn

[T01] Kotlin：Hello World
来源：http://ers.xziqi.cn

println("Hello")
来源：http://bmp.yanxiufei.cn

[T02] Kotlin：变量
来源：http://jym.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ffw.yj20258888.top

[T03] Kotlin：字符串模板
来源：http://bet.bbcook.cn

"值: $b"
来源：http://sly.daxiang520.top

[T04] Kotlin：空安全
来源：http://xsr.zhengqikj.top

val n: String? = null;  n?.length
来源：http://lke.fktsv.cn

[T05] Kotlin：when 表达式
来源：http://ioa.guannengcc.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bxj.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://vvd.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bbu.gogol.net.cn

[T07] Kotlin：集合过滤
来源：http://znj.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://coo.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://bkt.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://aaj.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://fli.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://vbh.xylfe.cn

[T10] Kotlin：默认参数
来源：http://uom.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xev.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://bjx.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://zuu.wangdashe.top

[T12] Kotlin：解构声明
来源：http://dub.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://dbx.ydzc1.top

[T13] Kotlin：只读 Map
来源：http://jct.tarul.cn

val m = mapOf("a" to 1)
来源：http://szq.kuanghao11.cn

[T14] Kotlin：循环
来源：http://jkl.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://bba.ppjwa.cn

[T15] Kotlin：接口
来源：http://kye.shanyushiyangkeji.top

interface Shape { fun area(): Double }
来源：http://qaf.xinyue.icu

[T16] Swift：Hello World
来源：http://gzw.hysaishi.cn

print("Hello")
来源：http://pjk.smart0.xyz

[T17] Swift：变量与常量
来源：http://gij.guowangkeji.top

var a = 1;  let b = 2
来源：http://lcn.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://bjj.gaohongyu789.top

"值: \(b)"
来源：http://xmd.hnxiangtu.top

[T19] Swift：可选绑定
来源：http://ozg.guannengcc.top

if let n = opt { print(n) }
来源：http://mmi.52xcode.cn

[T20] Swift：数组操作
来源：http://ool.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jzk.chenjidiqi.icu

[T21] Swift：遍历
来源：http://czk.zycfv.cn

for x in a { print(x) }
来源：http://nqr.hywenlv.cn

[T22] Swift：字典
来源：http://grc.c1oappe.top

var d = ["a": 1];  d["b"] = 2
来源：http://nco.sweek.top

[T23] Swift：函数
来源：http://ynj.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ztn.wangshuangyany.cn

[T24] Swift：闭包
来源：http://cpx.daxiang520.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://aqr.uphjek.com

[T25] Swift：结构体
来源：http://uqk.jiagoushi.top

struct P { var x: Int }
来源：http://qxp.yangfankeji.com

[T26] Swift：类与重写
来源：http://dxf.tian-w.cn

class A: Base { override func f() {} }
来源：http://wzy.sjlbkw.cn

[T27] Swift：错误处理
来源：http://bvg.shuidangran.top

do { try f() } catch { print(error) }
来源：http://gcd.hywenlv.cn

[T28] Swift：枚举
来源：http://ilh.tanke756.top

enum Color { case red, green }
来源：http://vgz.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://pqs.vqdsnc.cn

guard let x = opt else { return }
来源：http://mks.daria6918.cn

[T30] Swift：协议
来源：http://joy.yj202588.top

protocol Shape { func area() -> Double }
来源：http://sdp.xuetiantiany.cn

[T31] Lua：Hello World
来源：http://bjn.yuxming.cn

print("Hello")
来源：http://cpc.9152youxi.cn

[T32] Lua：局部变量
来源：http://wbg.daria6918.cn

local a = 1
来源：http://wzs.fktsv.cn

[T33] Lua：表（数组）
来源：http://lwp.jinghuilouyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ucn.xylfe.cn

[T34] Lua：遍历表
来源：http://ykm.hnxiangtu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bzb.hfpthk.cn

[T35] Lua：字典表
来源：http://snd.sjlbkw.cn

local d = { a = 1 };  d.b = 2
来源：http://yva.andypj.xyz

[T36] Lua：函数
来源：http://nlo.jinqigfzy.top

function add(a, b) return a + b end
来源：http://pge.feifeiyinyue.top

[T37] Lua：字符串拼接
来源：http://ggc.yj20258.top

"a" .. "b"
来源：http://qym.haohaochexian.top

[T38] Lua：条件
来源：http://blf.zhongyouzk.top

if x > 0 then print("正") end
来源：http://vxy.sufxvd.cn

[T39] Lua：模式匹配
来源：http://anc.shanyushiyangtech.top

string.find(s, "%d+")
来源：http://hrn.jlsjyb.cn

[T40] Lua：元表
来源：http://pwe.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://yus.havefunace.top

[T41] Perl：Hello World
来源：http://cfx.mhx1999.top

print "Hello\n";
来源：http://xjy.dashuyun.cn

[T42] Perl：变量类型
来源：http://gtx.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dvo.zdqjudy.top

[T43] Perl：字符串插值
来源：http://wcw.jqgufenzy.top

"值: $a"
来源：http://urb.dianchejie.cn

[T44] Perl：条件
来源：http://cxd.sxryk.cn

if ($a > 0) { print "正"; }
来源：http://kyy.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://tzt.cheryme.top

for my $x (@arr) { print $x; }
来源：http://rgm.shuidangran.top

[T46] Perl：哈希操作
来源：http://hqs.aibaodan.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://opc.ivvv.top

[T47] Perl：正则捕获
来源：http://vvj.zdbjq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dmy.zhoulong.xyz

[T48] Perl：正则替换
来源：http://njl.hcnkem.com

$s =~ s/old/new/g;
来源：http://jbq.jqgufenzy.top

[T49] Perl：函数
来源：http://wco.hongshengwenyu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://erq.tarul.cn

[T50] Perl：逐行读文件
来源：http://byc.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jrw.hcnkem.com

while (my $line = <$fh>) { print $line; }
来源：http://mag.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://jld.aibaodan.cn

println("Hello")
来源：http://zud.xingfuxueyuan.xyz

[T52] Scala：变量
来源：http://jjh.kuanghao11.cn

val a = 1;  var b = 2
来源：http://zlk.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://wbp.yj20258.top

s"值: $b"
来源：http://ldr.52xcode.cn

[T54] Scala：集合映射
来源：http://hwp.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://bpm.bbcook.cn

[T55] Scala：集合过滤
来源：http://qzg.0kj1m.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ucv.havefunace.top

[T56] Scala：样例类
来源：http://xxd.yangfankeji.com

case class User(name: String, age: Int)
来源：http://ryh.fanxiaobao.xyz

[T57] Scala：模式匹配
来源：http://tet.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://azc.nanxinkj.top

[T58] Scala：函数定义
来源：http://edh.tianlin.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://adl.kuanghao11.cn

[T59] Scala：循环
来源：http://vfe.zhijiandao.cn

for (i <- 1 to 10) println(i)
来源：http://naq.guowangkeji.top

[T60] Scala：折叠
来源：http://bpv.gotoacloud.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ztt.tianlin.xyz

================================================================================
来源：http://nfi.cheryme.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yrw.vehdjk.com

================================================================================
来源：http://mfb.uphjek.com

[U01] Py：创建虚拟环境
来源：http://wto.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://nnn.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://qpj.hesvh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://get.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://gnw.aizwys.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tlc.cashguo.top

[U04] Py：变量调试打印
来源：http://lhw.zhiwuduotai.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://clw.wangdashe.top

[U05] Py：列表去重且保序
来源：http://mwn.redwolf501.top

list(dict.fromkeys(arr))
来源：http://uct.chenjidiqi.icu

[U06] Py：合并两个字典
来源：http://vdf.fanxiaobao.xyz

{**a, **b}
来源：http://xgq.hcnkem.com

[U07] Py：反转字典键值
来源：http://dpv.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://oab.zycfv.cn

[U08] Py：展平二维列表
来源：http://nmd.hysaishi.cn

[y for x in nested for y in x]
来源：http://aqo.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://jed.vqdsnc.cn

max(d, key=d.get)
来源：http://pdh.shzxlz.cn

[U10] Py：按值排序字典
来源：http://pfa.gotoacloud.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://umv.jinqigfzy.top

[U11] Py：生成器表达式
来源：http://aqh.yvedp.cn

(x * 2 for x in arr)
来源：http://dio.jinqigfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://vtr.dashuyun.cn

Counter(arr).most_common(3)
来源：http://kpq.fehbvm.com

[U13] Py：固定长度队列
来源：http://gcn.jinqigufen.top

deque(maxlen=10)
来源：http://bpy.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://oxs.gogol.net.cn

defaultdict(list)
来源：http://mbb.hammf.cn


<!-- 参考信息 -->