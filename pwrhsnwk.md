代发 wailian999

read -rp "请输入: " ans
来源：http://odl.ctjpmb.com

[R78] 交互式菜单
来源：http://ocr.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ghu.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://duq.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pbl.hammf.cn

[R80] 查看脚本执行耗时
来源：http://ugs.cashguo.top

time ./run.sh
来源：http://rif.0kj1m.cn

================================================================================
来源：http://idw.wangshuangyany.cn

S. C / C++ 专题
来源：http://oan.bjfxy.top

================================================================================
来源：http://ysn.yonumen.top

[S01] C：Hello World
来源：http://mba.gotoacloud.top

#include <stdio.h>
来源：http://jpo.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kea.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://knm.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://eam.vehdjk.com

[S03] C：读入整数
来源：http://ftt.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://eat.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://ske.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://css.wangshuangyany.cn

[S05] C：字符串长度
来源：http://gfe.ppjwa.cn

strlen(s)
来源：http://kry.gotoacloud.top

[S06] C：字符串比较
来源：http://nqp.zhoulong.xyz

strcmp(a, b) == 0
来源：http://ccs.316326.xyz

[S07] C：数组遍历求和
来源：http://ylq.nanxuanxn.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ptb.snrcjt.cn

[S08] C：动态内存分配与释放
来源：http://zya.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rrw.tarul.cn

[S09] C：结构体定义与初始化
来源：http://usb.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vzf.haohaochexian.top

[S10] C：指针与解引用
来源：http://cse.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://zqq.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://yvz.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://yiy.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mgv.tarul.cn

fclose(f);
来源：http://acw.hywenlv.cn

[S12] C：写文件
来源：http://gtk.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nzf.zhoulong.xyz

[S13] C：宏定义
来源：http://lrs.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://epz.feifeiyinyue.top

[S14] C：枚举
来源：http://iaj.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://vkv.zhongyouzk.top

[S15] C：类型转换
来源：http://hdk.aibaodan.cn

(double) a / b
来源：http://ugl.epnwcf.com

[S16] C：位操作置位
来源：http://bqw.yongpay.top

x |= (1 << 3);
来源：http://qwu.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://lgh.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ynq.bjfxy.top

[S18] C：命令行参数
来源：http://sfm.bbcook.cn

int main(int argc, char **argv)
来源：http://qeq.hammf.cn

[S19] C：快速排序
来源：http://lgg.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rfy.52xcode.cn

[S20] C：二分查找
来源：http://lvf.daxiang520.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ikz.yvedp.cn

[S21] C：字符类别判断
来源：http://mup.wangshuangyany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gay.jiagoushi.top

[S22] C：字符串转数字
来源：http://hsk.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://amz.yfazqb.com

[S23] C：随机数
来源：http://wes.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yzz.hywenlv.cn

[S24] C：获取本地时间
来源：http://rve.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oqt.havefunace.top

[S25] C：内存拷贝
来源：http://nub.fzhhl.top

memcpy(dst, src, n);
来源：http://gja.feifeiyinyue.top

[S26] C：内存清零
来源：http://tyn.shanyushiyangkeji.top

memset(a, 0, sizeof a);
来源：http://lyp.xinyue.icu

[S27] C：定义常量
来源：http://fya.fengsongda.top

const double PI = 3.14159;
来源：http://lkl.gotoacloud.top

[S28] C：静态变量
来源：http://iho.havefunace.top

static int counter = 0;
来源：http://eis.sweek.top

[S29] C：变参函数
来源：http://jlh.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gbs.tanke756.top

[S30] C：头文件保护
来源：http://liv.316326.xyz

#ifndef X_H
来源：http://gud.vqdsnc.cn

#define X_H
来源：http://fqa.yuanzhike.top

#endif
来源：http://gqt.guowangkeji.top

[S31] C++：Hello World
来源：http://bvi.pengpengdd.cyou

#include <iostream>
来源：http://dsq.jqgfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://txu.uphjek.com

[S32] C++：字符串
来源：http://rfu.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://lzd.xziqi.cn

[S33] C++：vector 增删
来源：http://woh.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ukb.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://hpj.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://cru.sxryk.cn

[S35] C++：map
来源：http://lru.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qdr.guowangkeji.top

[S36] C++：unordered_map
来源：http://zpv.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dmd.jianghu66.top

[S37] C++：set
来源：http://miy.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dgl.dianchejie.cn

[S38] C++：排序
来源：http://dzq.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://ozc.sufxvd.cn

[S39] C++：自定义比较器排序
来源：http://qqn.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ply.ydzc1.top

[S40] C++：查找元素
来源：http://kox.cheryme.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cqe.jinqigufen.top

[S41] C++：类与构造函数
来源：http://vfz.daxiang520.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gku.redwolf501.top

[S42] C++：继承与虚函数
来源：http://jiq.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://irv.xuanzx.com

[S43] C++：智能指针
来源：http://wdr.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://vje.feifeiyinyue.top

[S44] C++：引用传参
来源：http://fjk.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://ilj.xziqi.cn

[S45] C++：lambda
来源：http://xys.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://noo.daria6918.cn

[S46] C++：函数模板
来源：http://bqz.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aux.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://cbn.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nce.iojbl.cn

[S48] C++：逐行读文件
来源：http://scr.xylfe.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xgf.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://xjm.aibaodan.cn

[S49] C++：写文件
来源：http://cpc.sufxvd.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rwb.snrcjt.cn

[S50] C++：格式化数字
来源：http://tqg.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yfd.meibo888.top

[S51] C++：显式类型转换
来源：http://bdf.ydzc1.top

static_cast<double>(a) / b
来源：http://yxg.tanke756.top

[S52] C++：const 与 noexcept
来源：http://tzc.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://znj.haohaochexian.top

[S53] C++：移动语义
来源：http://lxf.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://hzd.jinqigufen.top

[S54] C++：异常处理
来源：http://lyt.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hoy.316326.xyz

[S55] C++：结构化绑定
来源：http://zoe.zhaomingkeji.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://nou.chenzaomai.com

[S56] C++：optional
来源：http://cyi.shangyingyoupin.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bee.zhijiandao.cn

[S57] C++：编译期常量
来源：http://shs.ppjwa.cn

constexpr int N = 10;
来源：http://smq.zhoulong.xyz

[S58] C++：命名空间
来源：http://awe.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://yen.cqqwz.cn

[S59] C++：静态断言
来源：http://ocu.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yqn.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://wkl.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bgn.jyoumei.cn

================================================================================
来源：http://wxs.kuanghao11.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ois.yvedp.cn

================================================================================
来源：http://zhm.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://wkv.jiagoushi.top

println("Hello")
来源：http://hsm.xinyue.icu

[T02] Kotlin：变量
来源：http://iru.daria6918.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://spw.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://agh.nanxuanxn.top

"值: $b"
来源：http://qxi.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://gix.sxryk.cn

val n: String? = null;  n?.length
来源：http://cwo.uphjek.com

[T05] Kotlin：when 表达式
来源：http://rsw.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jfu.birdmap.top

[T06] Kotlin：集合映射
来源：http://pid.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://bmm.zhijiandao.cn

[T07] Kotlin：集合过滤
来源：http://qgo.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://eot.jinqigfzy.top

[T08] Kotlin：数据类
来源：http://xdd.dashuyun.cn

data class User(val name: String, val age: Int)
来源：http://irk.jiagoushi.top

[T09] Kotlin：扩展函数
来源：http://xzo.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://ycy.cdnleiting.top

[T10] Kotlin：默认参数
来源：http://xaf.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zkw.ydzc1.top

[T11] Kotlin：协程
来源：http://wyv.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://map.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://vmy.bbcook.cn

val (a, b) = Pair(1, 2)
来源：http://lvu.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://zch.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://qcr.jianghu66.top

[T14] Kotlin：循环
来源：http://tyj.hesvh.cn

for (i in 1..10) println(i)
来源：http://uci.ctjpmb.com

[T15] Kotlin：接口
来源：http://bnh.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://vrb.sxryk.cn

[T16] Swift：Hello World
来源：http://cwg.c1oappe.top

print("Hello")
来源：http://zme.zdbjq.cn

[T17] Swift：变量与常量
来源：http://rdc.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://rps.sxryk.cn

[T18] Swift：字符串插值
来源：http://ici.yfazqb.com

"值: \(b)"
来源：http://zyr.tarul.cn

[T19] Swift：可选绑定
来源：http://rnt.guowangkeji.top

if let n = opt { print(n) }
来源：http://hnj.fengsongda.top

[T20] Swift：数组操作
来源：http://cri.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://jit.aibaodan.cn

[T21] Swift：遍历
来源：http://ean.vqdsnc.cn

for x in a { print(x) }
来源：http://kuf.bbcook.cn

[T22] Swift：字典
来源：http://xvx.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://twb.dashuyun.cn

[T23] Swift：函数
来源：http://eyu.yongpay.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://two.vqdsnc.cn

[T24] Swift：闭包
来源：http://yzq.quarkkingdee.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ovw.c1oappe.top

[T25] Swift：结构体
来源：http://oxp.gogol.net.cn

struct P { var x: Int }
来源：http://ots.mhx1999.top

[T26] Swift：类与重写
来源：http://fhk.svipenyu.cn

class A: Base { override func f() {} }
来源：http://rsp.nanxinkj.top

[T27] Swift：错误处理
来源：http://oxs.uphjek.com

do { try f() } catch { print(error) }
来源：http://fwa.bjfxy.top

[T28] Swift：枚举
来源：http://esx.316326.xyz

enum Color { case red, green }
来源：http://ciq.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://wmq.ydzc1.top

guard let x = opt else { return }
来源：http://qqx.xylfe.cn

[T30] Swift：协议
来源：http://qss.birdmap.top

protocol Shape { func area() -> Double }
来源：http://sqx.snrcjt.cn

[T31] Lua：Hello World
来源：http://yjf.ivvv.top

print("Hello")
来源：http://gqr.smart0.xyz

[T32] Lua：局部变量
来源：http://zyo.birdmap.top

local a = 1
来源：http://jlz.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://rrl.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ahn.tianlin.xyz

[T34] Lua：遍历表
来源：http://exm.cheryme.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lyt.shuidangran.top

[T35] Lua：字典表
来源：http://mhi.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://ibq.gaohongyu789.top

[T36] Lua：函数
来源：http://onw.iojbl.cn

function add(a, b) return a + b end
来源：http://bno.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://wni.ywan-chungtsiang.top

"a" .. "b"
来源：http://joq.zhengqikj.top

[T38] Lua：条件
来源：http://bnm.xylfe.cn

if x > 0 then print("正") end
来源：http://gzf.ctjpmb.com

[T39] Lua：模式匹配
来源：http://xnt.jinyuanbaomall.cn

string.find(s, "%d+")
来源：http://uqx.zycfv.cn

[T40] Lua：元表
来源：http://gjf.pycfn.com

setmetatable({}, { __index = base })
来源：http://xmd.snrcjt.cn

[T41] Perl：Hello World
来源：http://uuk.cucudq.cn

print "Hello\n";
来源：http://rsv.jinqigfzy.top

[T42] Perl：变量类型
来源：http://soi.jinghuilouyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bfy.yongpay.top

[T43] Perl：字符串插值
来源：http://xok.sxryk.cn

"值: $a"
来源：http://edk.ybcxt.top

[T44] Perl：条件
来源：http://mxf.pycfn.com

if ($a > 0) { print "正"; }
来源：http://gse.gaohongyu789.top

[T45] Perl：数组遍历
来源：http://wgk.hywenlv.cn

for my $x (@arr) { print $x; }
来源：http://gfz.chenlongwang.top

[T46] Perl：哈希操作
来源：http://cyo.cucudq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uvu.ppjwa.cn

[T47] Perl：正则捕获
来源：http://jif.52xcode.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mtz.zhiwuduotai.top

[T48] Perl：正则替换
来源：http://qwf.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://tka.ivvv.top

[T49] Perl：函数
来源：http://jnl.fzhhl.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cga.shuidangran.top

[T50] Perl：逐行读文件
来源：http://hnf.hongshengwenyu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://voc.vehdjk.com

while (my $line = <$fh>) { print $line; }
来源：http://muz.hcnkem.com

[T51] Scala：Hello World
来源：http://ajn.hnqzz.top

println("Hello")
来源：http://ytu.hesvh.cn

[T52] Scala：变量
来源：http://dzt.yj202588.top

val a = 1;  var b = 2
来源：http://rkv.yfazqb.com

[T53] Scala：字符串插值
来源：http://rmq.hongshengwenyu.top

s"值: $b"
来源：http://yam.chenlongwang.top

[T54] Scala：集合映射
来源：http://gic.yongpay.top

List(1, 2, 3).map(_ * 2)
来源：http://nsx.redwolf501.top

[T55] Scala：集合过滤
来源：http://nve.fzhhl.top

List(1, 2, 3).filter(_ > 1)
来源：http://fdj.hysaishi.cn

[T56] Scala：样例类
来源：http://lge.yj20258888.top

case class User(name: String, age: Int)
来源：http://qia.wangdashe.top

[T57] Scala：模式匹配
来源：http://erf.sysykeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://oca.yj20258888.top

[T58] Scala：函数定义
来源：http://hqr.zycfv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zei.hcnkem.com

[T59] Scala：循环
来源：http://hqy.quarkkingdee.top

for (i <- 1 to 10) println(i)
来源：http://zvj.hammf.cn

[T60] Scala：折叠
来源：http://aih.fktsv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tpl.0kj1m.cn

================================================================================
来源：http://ccv.ybcxt.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dab.iojbl.cn

================================================================================
来源：http://yms.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://klh.cdnleiting.top

python -m venv .venv && source .venv/bin/activate
来源：http://qzn.yangfankeji.com

[U02] Py：导出 / 安装依赖
来源：http://meu.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oic.316326.xyz

[U03] Py：加载 .env 配置
来源：http://ool.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://zie.cqqwz.cn

[U04] Py：变量调试打印
来源：http://hwy.zhixingplan.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qic.fehbvm.com

[U05] Py：列表去重且保序
来源：http://ial.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://oja.nwbrower.top

[U06] Py：合并两个字典
来源：http://gij.guowangkeji.top

{**a, **b}
来源：http://xeb.yanxiufei.cn

[U07] Py：反转字典键值
来源：http://dab.aizwys.cn

{v: k for k, v in d.items()}
来源：http://zma.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://acr.yanxiufei.cn

[y for x in nested for y in x]
来源：http://goh.chenlongwang.top

[U09] Py：字典取最大值的键
来源：http://cpg.daxiang520.top

max(d, key=d.get)
来源：http://ore.havefunace.top

[U10] Py：按值排序字典
来源：http://wgf.ppjwa.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bkp.ehwqpu.com

[U11] Py：生成器表达式
来源：http://gdr.zhongyouzk.top

(x * 2 for x in arr)
来源：http://ucl.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vgb.hnqzz.top

Counter(arr).most_common(3)
来源：http://vwc.yonumen.top

[U13] Py：固定长度队列
来源：http://tzf.gotoacloud.top

deque(maxlen=10)
来源：http://byg.yfazqb.com

[U14] Py：分组收集到列表
来源：http://yag.wangshuangyany.cn

defaultdict(list)
来源：http://mkv.chenzaomai.com

[U15] Py：高精度计时
来源：http://bhn.yvedp.cn

t = time.perf_counter()
来源：http://gjh.redwolf501.top

[U16] Py：命令行参数解析
来源：http://blt.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://irh.tianlin.xyz

[U17] Py：初始化日志
来源：http://eat.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://zcx.jyoumei.cn

[U18] Py：预编译正则
来源：http://xfh.shzxlz.cn

pat = re.compile(r"\d+")
来源：http://nbi.xylfe.cn


<!-- 参考信息 -->