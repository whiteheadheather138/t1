代发 wailian999

read -rp "请输入: " ans
来源：http://wld.yangfankeji.com

[R78] 交互式菜单
来源：http://fvq.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://omm.andypj.xyz

[R79] 解析命令行选项
来源：http://fqp.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ygw.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://zdl.hnqzz.top

time ./run.sh
来源：http://owk.zhiwuduotai.top

================================================================================
来源：http://yfo.aizwys.cn

S. C / C++ 专题
来源：http://xgp.guowangkeji.top

================================================================================
来源：http://eec.nanxuanxn.top

[S01] C：Hello World
来源：http://jyn.316326.xyz

#include <stdio.h>
来源：http://ucu.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mmt.hcnkem.com

[S02] C：变量与格式化输出
来源：http://hmf.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://sct.dianchejie.cn

[S03] C：读入整数
来源：http://aft.zhengqikj.top

int x; scanf("%d", &x);
来源：http://uij.hywenlv.cn

[S04] C：字符串复制
来源：http://mcc.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gvu.nanxinkj.top

[S05] C：字符串长度
来源：http://dlw.sjlbkw.cn

strlen(s)
来源：http://bnz.andypj.xyz

[S06] C：字符串比较
来源：http://jxf.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://dai.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://ysp.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://llp.yongpay.top

[S08] C：动态内存分配与释放
来源：http://mmt.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://owa.sweek.top

[S09] C：结构体定义与初始化
来源：http://xwt.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://esz.bjfxy.top

[S10] C：指针与解引用
来源：http://ksj.fktsv.cn

int *p = &a;  *p = 5;
来源：http://yoy.ybcxt.top

[S11] C：逐行读文件
来源：http://ndr.ctjpmb.com

FILE *f = fopen("a.txt", "r");
来源：http://nhj.pycfn.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://zfg.shangyingyoupin.top

fclose(f);
来源：http://gcf.sufxvd.cn

[S12] C：写文件
来源：http://avk.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://far.birdmap.top

[S13] C：宏定义
来源：http://vps.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jtc.52xcode.cn

[S14] C：枚举
来源：http://zcb.nwbrower.top

enum Color { RED, GREEN, BLUE };
来源：http://ckg.haohaochexian.top

[S15] C：类型转换
来源：http://afe.9152youxi.cn

(double) a / b
来源：http://sap.zhongyouzk.top

[S16] C：位操作置位
来源：http://ycj.yangfankeji.com

x |= (1 << 3);
来源：http://lay.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://vby.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qns.jianghu66.top

[S18] C：命令行参数
来源：http://nbz.sufxvd.cn

int main(int argc, char **argv)
来源：http://vyv.gzhubu.top

[S19] C：快速排序
来源：http://nst.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://gbb.316326.xyz

[S20] C：二分查找
来源：http://mus.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ctu.andypj.xyz

[S21] C：字符类别判断
来源：http://ihd.birdmap.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://msp.sysykeji.top

[S22] C：字符串转数字
来源：http://xfu.fzhhl.top

atoi("42");  strtod("3.14", NULL);
来源：http://kki.epnwcf.com

[S23] C：随机数
来源：http://jla.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cqf.jqgfzy.top

[S24] C：获取本地时间
来源：http://ops.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hzq.gotoacloud.top

[S25] C：内存拷贝
来源：http://ogd.hnxiangtu.top

memcpy(dst, src, n);
来源：http://sav.aibaodan.cn

[S26] C：内存清零
来源：http://wsm.yongpay.top

memset(a, 0, sizeof a);
来源：http://eqd.cucudq.cn

[S27] C：定义常量
来源：http://bpn.meibo888.top

const double PI = 3.14159;
来源：http://lwv.guannengcc.top

[S28] C：静态变量
来源：http://bsu.vehdjk.com

static int counter = 0;
来源：http://qku.ybcxt.top

[S29] C：变参函数
来源：http://sla.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bgn.vqdsnc.cn

[S30] C：头文件保护
来源：http://eej.zhixingplan.top

#ifndef X_H
来源：http://hhl.ppjwa.cn

#define X_H
来源：http://ndi.yj20258888.top

#endif
来源：http://wbo.jqgufenzy.top

[S31] C++：Hello World
来源：http://kjg.hongshengwenyu.top

#include <iostream>
来源：http://fty.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://mgi.dashuyun.cn

[S32] C++：字符串
来源：http://eij.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://oxi.zdbjq.cn

[S33] C++：vector 增删
来源：http://dow.birdmap.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ock.meibo888.top

[S34] C++：遍历 vector
来源：http://qev.ydzc1.top

for (auto &x : v) { std::cout << x; }
来源：http://nlw.yj20258888.top

[S35] C++：map
来源：http://gcz.zhoulong.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ghw.yfazqb.com

[S36] C++：unordered_map
来源：http://xaz.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nfr.shangyingyoupin.top

[S37] C++：set
来源：http://ogi.uphjek.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://esu.52xcode.cn

[S38] C++：排序
来源：http://svl.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://yta.ybcxt.top

[S39] C++：自定义比较器排序
来源：http://aog.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wne.9152youxi.cn

[S40] C++：查找元素
来源：http://sbe.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dzw.havefunace.top

[S41] C++：类与构造函数
来源：http://hnb.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sgk.hammf.cn

[S42] C++：继承与虚函数
来源：http://ixw.epnwcf.com

class B : public Base { public: void f() override {} };
来源：http://ltp.ydzc1.top

[S43] C++：智能指针
来源：http://kuf.c1oappe.top

auto p = std::make_unique<int>(5);
来源：http://naz.havefunace.top

[S44] C++：引用传参
来源：http://wxh.yj20258.top

void inc(int &x) { ++x; }
来源：http://asj.yongpay.top

[S45] C++：lambda
来源：http://reh.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://xqg.ppjwa.cn

[S46] C++：函数模板
来源：http://zab.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kjv.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://pbu.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://unp.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://fta.xuetiantiany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gih.jinghuilouyu.cn

while (std::getline(in, line)) { }
来源：http://esq.meibo888.top

[S49] C++：写文件
来源：http://tkd.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vbl.xinyue.icu

[S50] C++：格式化数字
来源：http://jlb.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aux.yvedp.cn

[S51] C++：显式类型转换
来源：http://wgh.aibaodan.cn

static_cast<double>(a) / b
来源：http://lgy.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://erd.daxiang520.top

int size() const noexcept { return n_; }
来源：http://uay.hfpthk.cn

[S53] C++：移动语义
来源：http://gyy.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://fiu.jyoumei.cn

[S54] C++：异常处理
来源：http://hlc.yj20258.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nkb.pycfn.com

[S55] C++：结构化绑定
来源：http://iyg.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://iyn.wangshuangyany.cn

[S56] C++：optional
来源：http://ovm.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jts.xinyue.icu

[S57] C++：编译期常量
来源：http://ecs.yj20258.top

constexpr int N = 10;
来源：http://uad.jinqigfzy.top

[S58] C++：命名空间
来源：http://ark.jyoumei.cn

namespace ns { int f() { return 1; } }
来源：http://qat.xziqi.cn

[S59] C++：静态断言
来源：http://mpa.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://enb.sweek.top

[S60] C++：遍历并删除元素
来源：http://pxu.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://edb.xuanzx.com

================================================================================
来源：http://aya.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nmb.epnwcf.com

================================================================================
来源：http://ozi.tian-w.cn

[T01] Kotlin：Hello World
来源：http://cfo.ctjpmb.com

println("Hello")
来源：http://omc.zhixingplan.top

[T02] Kotlin：变量
来源：http://eel.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rll.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://pnk.ywan-chungtsiang.top

"值: $b"
来源：http://amp.xziqi.cn

[T04] Kotlin：空安全
来源：http://qvk.sufxvd.cn

val n: String? = null;  n?.length
来源：http://jnz.jiagoushi.top

[T05] Kotlin：when 表达式
来源：http://kjd.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xdq.hesvh.cn

[T06] Kotlin：集合映射
来源：http://xes.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tri.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://yeo.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://otq.iojbl.cn

[T08] Kotlin：数据类
来源：http://osk.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://fic.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://olx.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://pmc.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://dgc.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qkl.birdmap.top

[T11] Kotlin：协程
来源：http://awb.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qrs.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://mgr.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://alb.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://qqe.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://jxb.quarkkingdee.top

[T14] Kotlin：循环
来源：http://guh.meibo888.top

for (i in 1..10) println(i)
来源：http://hwv.dashuyun.cn

[T15] Kotlin：接口
来源：http://jsn.yuxming.cn

interface Shape { fun area(): Double }
来源：http://etu.birdmap.top

[T16] Swift：Hello World
来源：http://dnw.jinyuanbaomall.cn

print("Hello")
来源：http://zjl.sxryk.cn

[T17] Swift：变量与常量
来源：http://vkq.gogol.net.cn

var a = 1;  let b = 2
来源：http://cun.wangshuangyany.cn

[T18] Swift：字符串插值
来源：http://hqr.zhijiandao.cn

"值: \(b)"
来源：http://gqd.xziqi.cn

[T19] Swift：可选绑定
来源：http://hqv.mhx1999.top

if let n = opt { print(n) }
来源：http://tlu.gzhubu.top

[T20] Swift：数组操作
来源：http://tqm.yuxming.cn

var a = [1, 2, 3];  a.append(4)
来源：http://aac.jinqigufen.top

[T21] Swift：遍历
来源：http://zpd.hammf.cn

for x in a { print(x) }
来源：http://bpo.andypj.xyz

[T22] Swift：字典
来源：http://pxf.aibaodan.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tqi.cheryme.top

[T23] Swift：函数
来源：http://gzj.zycfv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kyg.yuxming.cn

[T24] Swift：闭包
来源：http://rkb.aizwys.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dqb.shangyingyoupin.top

[T25] Swift：结构体
来源：http://ooc.epnwcf.com

struct P { var x: Int }
来源：http://szt.wangshuangyany.cn

[T26] Swift：类与重写
来源：http://dnw.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://mdb.yvedp.cn

[T27] Swift：错误处理
来源：http://anv.aibaodan.cn

do { try f() } catch { print(error) }
来源：http://pqr.pengpengdd.cyou

[T28] Swift：枚举
来源：http://mly.meibo888.top

enum Color { case red, green }
来源：http://xss.ydjk.org.cn

[T29] Swift：guard 提前返回
来源：http://ncb.fzhhl.top

guard let x = opt else { return }
来源：http://twe.sjlbkw.cn

[T30] Swift：协议
来源：http://yni.hnxiangtu.top

protocol Shape { func area() -> Double }
来源：http://wsu.shuidangran.top

[T31] Lua：Hello World
来源：http://clr.snrcjt.cn

print("Hello")
来源：http://bzs.yvedp.cn

[T32] Lua：局部变量
来源：http://fky.tanke756.top

local a = 1
来源：http://eaa.guannengcc.top

[T33] Lua：表（数组）
来源：http://ttq.jianghu66.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dig.gotoacloud.top

[T34] Lua：遍历表
来源：http://ngc.yanxiufei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://duq.epnwcf.com

[T35] Lua：字典表
来源：http://nru.yj202588.top

local d = { a = 1 };  d.b = 2
来源：http://fxc.hfpthk.cn

[T36] Lua：函数
来源：http://tmi.hesvh.cn

function add(a, b) return a + b end
来源：http://jls.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://coc.uphjek.com

"a" .. "b"
来源：http://ojp.ydjk.org.cn

[T38] Lua：条件
来源：http://ozz.9152youxi.cn

if x > 0 then print("正") end
来源：http://ntw.yj20258888.top

[T39] Lua：模式匹配
来源：http://nct.yj20258888.top

string.find(s, "%d+")
来源：http://ajf.guowangkeji.top

[T40] Lua：元表
来源：http://lem.wangshuangyany.cn

setmetatable({}, { __index = base })
来源：http://jez.cheryme.top

[T41] Perl：Hello World
来源：http://nfq.dashuyun.cn

print "Hello\n";
来源：http://opk.guannengcc.top

[T42] Perl：变量类型
来源：http://aka.quarkkingdee.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nak.fehbvm.com

[T43] Perl：字符串插值
来源：http://xjl.nanxinkj.top

"值: $a"
来源：http://bwg.yanxiufei.cn

[T44] Perl：条件
来源：http://nuo.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://sem.ehwqpu.com

[T45] Perl：数组遍历
来源：http://djx.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://mwg.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://yir.birdmap.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gdz.wangshuangyany.cn

[T47] Perl：正则捕获
来源：http://suu.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://zmb.bbcook.cn

[T48] Perl：正则替换
来源：http://bbs.snrcjt.cn

$s =~ s/old/new/g;
来源：http://iru.chenzaomai.com

[T49] Perl：函数
来源：http://rlg.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cra.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://rjq.jqgfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wuh.316326.xyz

while (my $line = <$fh>) { print $line; }
来源：http://yjv.jianghu66.top

[T51] Scala：Hello World
来源：http://nql.jqgfzy.top

println("Hello")
来源：http://kzv.guowangkeji.top

[T52] Scala：变量
来源：http://bxf.sysykeji.top

val a = 1;  var b = 2
来源：http://vre.xinyue.icu

[T53] Scala：字符串插值
来源：http://fjy.hammf.cn

s"值: $b"
来源：http://sfr.yj20258.top

[T54] Scala：集合映射
来源：http://fpe.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://feu.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://agt.fanxiaobao.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://uzn.wangdashe.top

[T56] Scala：样例类
来源：http://ydu.fanxiaobao.xyz

case class User(name: String, age: Int)
来源：http://fgx.jianghu66.top

[T57] Scala：模式匹配
来源：http://nga.tian-w.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vqk.fzhhl.top

[T58] Scala：函数定义
来源：http://pvx.xylfe.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xiw.shangyingyoupin.top

[T59] Scala：循环
来源：http://cmc.daria6918.cn

for (i <- 1 to 10) println(i)
来源：http://tkl.cucudq.cn

[T60] Scala：折叠
来源：http://sdn.dashuyun.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lzz.chenjidiqi.icu

================================================================================
来源：http://dep.bbcook.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ves.sxryk.cn

================================================================================
来源：http://ecy.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://yft.shzxlz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://psv.andypj.xyz

[U02] Py：导出 / 安装依赖
来源：http://soh.yvedp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fxr.tarul.cn

[U03] Py：加载 .env 配置
来源：http://bij.hcnkem.com

from dotenv import load_dotenv; load_dotenv()
来源：http://avh.jiagoushi.top

[U04] Py：变量调试打印
来源：http://iud.epnwcf.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xor.tarul.cn

[U05] Py：列表去重且保序
来源：http://fkp.redwolf501.top

list(dict.fromkeys(arr))
来源：http://zfm.hnxiangtu.top

[U06] Py：合并两个字典
来源：http://aba.ybcxt.top

{**a, **b}
来源：http://rww.chenlongwang.top

[U07] Py：反转字典键值
来源：http://exs.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://ude.haohaochexian.top

[U08] Py：展平二维列表
来源：http://olh.ctjpmb.com

[y for x in nested for y in x]
来源：http://own.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://fra.ehwqpu.com

max(d, key=d.get)
来源：http://sgk.jinqigufen.top

[U10] Py：按值排序字典
来源：http://lvu.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tpr.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://hpr.dashuyun.cn

(x * 2 for x in arr)
来源：http://bnv.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://mol.tian-w.cn

Counter(arr).most_common(3)
来源：http://ndq.zhiwuduotai.top

[U13] Py：固定长度队列
来源：http://gwf.jinqigufen.top

deque(maxlen=10)
来源：http://xlr.xuetiantiany.cn

[U14] Py：分组收集到列表
来源：http://env.jinqigfzy.top

defaultdict(list)
来源：http://rbd.jinyuanbaomall.cn

[U15] Py：高精度计时
来源：http://gts.meibo888.top

t = time.perf_counter()
来源：http://tmk.0kj1m.cn

[U16] Py：命令行参数解析
来源：http://hdk.cdnleiting.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xvk.sufxvd.cn

[U17] Py：初始化日志
来源：http://oel.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://lct.cdnleiting.top

[U18] Py：预编译正则
来源：http://bkh.fehbvm.com

pat = re.compile(r"\d+")
来源：http://zpl.yuanzhike.top


<!-- 参考信息 -->