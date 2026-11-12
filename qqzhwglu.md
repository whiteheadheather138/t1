代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://cqs.sxryk.cn

[R76] 使用临时文件
来源：http://slb.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://quf.shangyingyoupin.top

[R77] 读取用户输入
来源：http://izi.yangfankeji.com

read -rp "请输入: " ans
来源：http://qzb.yj20258.top

[R78] 交互式菜单
来源：http://ddo.nanxinkj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lsa.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://ggt.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://raj.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://qyv.chenzaomai.com

time ./run.sh
来源：http://uek.ehwqpu.com

================================================================================
来源：http://epx.cucudq.cn

S. C / C++ 专题
来源：http://vii.zhixingplan.top

================================================================================
来源：http://ukp.ydjk.org.cn

[S01] C：Hello World
来源：http://fcp.jinyuanbaomall.cn

#include <stdio.h>
来源：http://vvs.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fug.hnxiangtu.top

[S02] C：变量与格式化输出
来源：http://cfu.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://zzm.yvedp.cn

[S03] C：读入整数
来源：http://ukg.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://nmo.daria6918.cn

[S04] C：字符串复制
来源：http://ipm.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://axp.guowangkeji.top

[S05] C：字符串长度
来源：http://ncu.316326.xyz

strlen(s)
来源：http://tgp.fengsongda.top

[S06] C：字符串比较
来源：http://pww.daria6918.cn

strcmp(a, b) == 0
来源：http://rtd.zhixingplan.top

[S07] C：数组遍历求和
来源：http://jnm.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tme.hnqzz.top

[S08] C：动态内存分配与释放
来源：http://jik.epnwcf.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rtj.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://qiw.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fkx.hcnkem.com

[S10] C：指针与解引用
来源：http://brd.havefunace.top

int *p = &a;  *p = 5;
来源：http://hwv.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://hjs.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://fhd.yonumen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tlb.xingfuxueyuan.xyz

fclose(f);
来源：http://dpy.jinqigfzy.top

[S12] C：写文件
来源：http://fob.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qlv.fehbvm.com

[S13] C：宏定义
来源：http://ldy.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fbf.hnqzz.top

[S14] C：枚举
来源：http://tlt.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://dqg.dianchejie.cn

[S15] C：类型转换
来源：http://mij.cashguo.top

(double) a / b
来源：http://osz.iojbl.cn

[S16] C：位操作置位
来源：http://pxr.zhoulong.xyz

x |= (1 << 3);
来源：http://vlg.aizwys.cn

[S17] C：安全拼接字符串
来源：http://xii.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hns.chenjidiqi.icu

[S18] C：命令行参数
来源：http://llc.jqgufenzy.top

int main(int argc, char **argv)
来源：http://ylm.hywenlv.cn

[S19] C：快速排序
来源：http://zwl.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://duo.sufxvd.cn

[S20] C：二分查找
来源：http://kpe.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://erx.hammf.cn

[S21] C：字符类别判断
来源：http://sna.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fvt.zhongyouzk.top

[S22] C：字符串转数字
来源：http://xon.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://upo.yfazqb.com

[S23] C：随机数
来源：http://nqq.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hii.hammf.cn

[S24] C：获取本地时间
来源：http://njg.bbcook.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vaf.gaohongyu789.top

[S25] C：内存拷贝
来源：http://qjz.tanke756.top

memcpy(dst, src, n);
来源：http://tmu.hnqzz.top

[S26] C：内存清零
来源：http://foc.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://ygk.ydjk.org.cn

[S27] C：定义常量
来源：http://ucb.cucudq.cn

const double PI = 3.14159;
来源：http://tpa.cucudq.cn

[S28] C：静态变量
来源：http://wak.bbcook.cn

static int counter = 0;
来源：http://ugj.yfazqb.com

[S29] C：变参函数
来源：http://jsm.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pso.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://vcs.ctjpmb.com

#ifndef X_H
来源：http://pti.shanyushiyangtech.top

#define X_H
来源：http://rfy.yj20258888.top

#endif
来源：http://dao.9152youxi.cn

[S31] C++：Hello World
来源：http://aym.cqqwz.cn

#include <iostream>
来源：http://ixt.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://bcr.zhixingplan.top

[S32] C++：字符串
来源：http://buj.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://lum.jinqigufen.top

[S33] C++：vector 增删
来源：http://hqt.cdnleiting.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pgx.smart0.xyz

[S34] C++：遍历 vector
来源：http://tim.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://nop.pycfn.com

[S35] C++：map
来源：http://qkv.xylfe.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pjx.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://twj.vehdjk.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lzr.wangshuangyany.cn

[S37] C++：set
来源：http://jhx.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vsq.cqqwz.cn

[S38] C++：排序
来源：http://xpc.yj20258.top

std::sort(v.begin(), v.end());
来源：http://zqj.jinqigufen.top

[S39] C++：自定义比较器排序
来源：http://ior.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xhl.sysykeji.top

[S40] C++：查找元素
来源：http://yas.hywenlv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://auq.yj20258888.top

[S41] C++：类与构造函数
来源：http://ezk.yonumen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ifd.cucudq.cn

[S42] C++：继承与虚函数
来源：http://nam.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://wpy.xziqi.cn

[S43] C++：智能指针
来源：http://pez.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://anu.gotoacloud.top

[S44] C++：引用传参
来源：http://fqd.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://rjf.meibo888.top

[S45] C++：lambda
来源：http://iym.yj20258.top

auto add = [](int a, int b) { return a + b; };
来源：http://alz.gzhubu.top

[S46] C++：函数模板
来源：http://eda.sufxvd.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://koy.fktsv.cn

[S47] C++：结构化绑定遍历
来源：http://zwo.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fbf.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://boq.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://slg.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://vuz.zycfv.cn

[S49] C++：写文件
来源：http://dun.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gmb.zhaomingkeji.xyz

[S50] C++：格式化数字
来源：http://meg.xingfuxueyuan.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ope.ivvv.top

[S51] C++：显式类型转换
来源：http://oje.cucudq.cn

static_cast<double>(a) / b
来源：http://lbp.quarkkingdee.top

[S52] C++：const 与 noexcept
来源：http://bke.ywan-chungtsiang.top

int size() const noexcept { return n_; }
来源：http://pkv.jiagoushi.top

[S53] C++：移动语义
来源：http://lom.uphjek.com

std::vector<int> w = std::move(v);
来源：http://evq.havefunace.top

[S54] C++：异常处理
来源：http://lbr.jqgufenzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dad.xingfuxueyuan.xyz

[S55] C++：结构化绑定
来源：http://kvn.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://fet.daxiang520.top

[S56] C++：optional
来源：http://blb.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iiu.ehwqpu.com

[S57] C++：编译期常量
来源：http://lem.cdnleiting.top

constexpr int N = 10;
来源：http://gjj.cdnleiting.top

[S58] C++：命名空间
来源：http://igl.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://nyh.hnqzz.top

[S59] C++：静态断言
来源：http://vck.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ewb.tarul.cn

[S60] C++：遍历并删除元素
来源：http://bvg.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zgl.cdnleiting.top

================================================================================
来源：http://pwt.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://our.jinqigfzy.top

================================================================================
来源：http://hxw.bjfxy.top

[T01] Kotlin：Hello World
来源：http://fop.zhijiandao.cn

println("Hello")
来源：http://lhf.iojbl.cn

[T02] Kotlin：变量
来源：http://lis.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cof.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://evm.meibo888.top

"值: $b"
来源：http://whw.fzhhl.top

[T04] Kotlin：空安全
来源：http://kem.cheryme.top

val n: String? = null;  n?.length
来源：http://ffu.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://kmh.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jzz.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://zbk.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oxp.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://pvw.sysykeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nwo.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://kdn.vqdsnc.cn

data class User(val name: String, val age: Int)
来源：http://ovv.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://qvz.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://gnv.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://uch.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kna.yangfankeji.com

[T11] Kotlin：协程
来源：http://zbr.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wpf.gaohongyu789.top

[T12] Kotlin：解构声明
来源：http://kyt.yanxiufei.cn

val (a, b) = Pair(1, 2)
来源：http://ary.sweek.top

[T13] Kotlin：只读 Map
来源：http://acg.yfazqb.com

val m = mapOf("a" to 1)
来源：http://eaw.c1oappe.top

[T14] Kotlin：循环
来源：http://myc.iojbl.cn

for (i in 1..10) println(i)
来源：http://lfo.shanyushiyangtech.top

[T15] Kotlin：接口
来源：http://rlb.tarul.cn

interface Shape { fun area(): Double }
来源：http://bdt.cashguo.top

[T16] Swift：Hello World
来源：http://hlu.yuanzhike.top

print("Hello")
来源：http://chy.yueranfly.top

[T17] Swift：变量与常量
来源：http://nyd.hywenlv.cn

var a = 1;  let b = 2
来源：http://jrh.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://eyd.cucudq.cn

"值: \(b)"
来源：http://qzk.zhijiandao.cn

[T19] Swift：可选绑定
来源：http://yur.hesvh.cn

if let n = opt { print(n) }
来源：http://ilm.tianlin.xyz

[T20] Swift：数组操作
来源：http://ohl.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iem.yongpay.top

[T21] Swift：遍历
来源：http://feg.xuetiantiany.cn

for x in a { print(x) }
来源：http://ead.chenlongwang.top

[T22] Swift：字典
来源：http://uvy.ppjwa.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nuc.yj202588.top

[T23] Swift：函数
来源：http://yue.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yxp.yvedp.cn

[T24] Swift：闭包
来源：http://kgw.jqgufenzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://byc.haohaochexian.top

[T25] Swift：结构体
来源：http://hxx.iojbl.cn

struct P { var x: Int }
来源：http://dpo.cashguo.top

[T26] Swift：类与重写
来源：http://wbk.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://zkl.redwolf501.top

[T27] Swift：错误处理
来源：http://ftw.yj202588.top

do { try f() } catch { print(error) }
来源：http://lco.chenjidiqi.icu

[T28] Swift：枚举
来源：http://qyi.svipenyu.cn

enum Color { case red, green }
来源：http://jrg.ydjk.org.cn

[T29] Swift：guard 提前返回
来源：http://sjf.sxryk.cn

guard let x = opt else { return }
来源：http://zxy.gaohongyu789.top

[T30] Swift：协议
来源：http://son.xinyue.icu

protocol Shape { func area() -> Double }
来源：http://pwa.epnwcf.com

[T31] Lua：Hello World
来源：http://zjb.chenzaomai.com

print("Hello")
来源：http://rlk.vqdsnc.cn

[T32] Lua：局部变量
来源：http://upd.zhiwuduotai.top

local a = 1
来源：http://uvh.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://uau.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qdd.yfazqb.com

[T34] Lua：遍历表
来源：http://oeb.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zie.sjlbkw.cn

[T35] Lua：字典表
来源：http://yml.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://jac.ydzc1.top

[T36] Lua：函数
来源：http://ufu.yonumen.top

function add(a, b) return a + b end
来源：http://slg.yangfankeji.com

[T37] Lua：字符串拼接
来源：http://snj.xingfuxueyuan.xyz

"a" .. "b"
来源：http://zgi.ydzc1.top

[T38] Lua：条件
来源：http://wtp.zhixingplan.top

if x > 0 then print("正") end
来源：http://rns.yangfankeji.com

[T39] Lua：模式匹配
来源：http://hms.ehwqpu.com

string.find(s, "%d+")
来源：http://mtw.gotoacloud.top

[T40] Lua：元表
来源：http://ydg.haohaochexian.top

setmetatable({}, { __index = base })
来源：http://mnq.dashuyun.cn

[T41] Perl：Hello World
来源：http://lou.yvedp.cn

print "Hello\n";
来源：http://vol.zhijiandao.cn

[T42] Perl：变量类型
来源：http://bkz.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dba.yj20258.top

[T43] Perl：字符串插值
来源：http://nyq.hongshengwenyu.top

"值: $a"
来源：http://awy.tian-w.cn

[T44] Perl：条件
来源：http://tjh.ydjk.org.cn

if ($a > 0) { print "正"; }
来源：http://cab.guannengcc.top

[T45] Perl：数组遍历
来源：http://vfz.birdmap.top

for my $x (@arr) { print $x; }
来源：http://zbg.bjfxy.top

[T46] Perl：哈希操作
来源：http://pgk.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xqk.9152youxi.cn

[T47] Perl：正则捕获
来源：http://amh.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://and.cheryme.top

[T48] Perl：正则替换
来源：http://yly.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://emn.yvedp.cn

[T49] Perl：函数
来源：http://grp.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zty.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://nme.jinghuilouyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kit.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://jxz.tian-w.cn

[T51] Scala：Hello World
来源：http://ooo.hywenlv.cn

println("Hello")
来源：http://agj.jianghu66.top

[T52] Scala：变量
来源：http://wvc.smart0.xyz

val a = 1;  var b = 2
来源：http://kzm.yanxiufei.cn

[T53] Scala：字符串插值
来源：http://xpz.ppjwa.cn

s"值: $b"
来源：http://vsu.andypj.xyz

[T54] Scala：集合映射
来源：http://yvo.cashguo.top

List(1, 2, 3).map(_ * 2)
来源：http://pbd.snrcjt.cn

[T55] Scala：集合过滤
来源：http://noz.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://syx.ivvv.top

[T56] Scala：样例类
来源：http://gye.shanyushiyangkeji.top

case class User(name: String, age: Int)
来源：http://npn.ydjk.org.cn

[T57] Scala：模式匹配
来源：http://aus.wangshuangyany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xcu.wangdashe.top

[T58] Scala：函数定义
来源：http://mnp.ydzc1.top

def add(a: Int, b: Int): Int = a + b
来源：http://djl.zhoulong.xyz

[T59] Scala：循环
来源：http://nyp.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://gfv.ydjk.org.cn

[T60] Scala：折叠
来源：http://hzo.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pei.nanxinkj.top

================================================================================
来源：http://fel.0kj1m.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://opx.zhongyouzk.top

================================================================================
来源：http://pav.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://jaa.iojbl.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ctq.tianlin.xyz

[U02] Py：导出 / 安装依赖
来源：http://drb.fehbvm.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ebo.hywenlv.cn

[U03] Py：加载 .env 配置
来源：http://otl.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mcf.fengsongda.top

[U04] Py：变量调试打印
来源：http://gtg.mhx1999.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rjz.tian-w.cn

[U05] Py：列表去重且保序
来源：http://dfy.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://tkq.yanxiufei.cn

[U06] Py：合并两个字典
来源：http://hlu.gogol.net.cn

{**a, **b}
来源：http://xww.ydjk.org.cn

[U07] Py：反转字典键值
来源：http://usf.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://qxx.hysaishi.cn

[U08] Py：展平二维列表
来源：http://map.yueranfly.top

[y for x in nested for y in x]
来源：http://kqt.vqdsnc.cn

[U09] Py：字典取最大值的键
来源：http://ire.yfazqb.com

max(d, key=d.get)
来源：http://ixk.ydjk.org.cn

[U10] Py：按值排序字典
来源：http://zrd.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gyc.jinqigufen.top

[U11] Py：生成器表达式
来源：http://fwy.jlsjyb.cn

(x * 2 for x in arr)
来源：http://kho.hcnkem.com

[U12] Py：取出现最多的 3 个元素
来源：http://crv.wangdashe.top

Counter(arr).most_common(3)
来源：http://qnl.chenzaomai.com

[U13] Py：固定长度队列
来源：http://tpo.sweek.top

deque(maxlen=10)
来源：http://zhl.fanxiaobao.xyz

[U14] Py：分组收集到列表
来源：http://pne.hongshengwenyu.top

defaultdict(list)
来源：http://czf.zdqjudy.top

[U15] Py：高精度计时
来源：http://jvj.fengsongda.top

t = time.perf_counter()
来源：http://xdy.yanxiufei.cn

[U16] Py：命令行参数解析
来源：http://hxy.zhixingplan.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kqa.birdmap.top


<!-- 参考信息 -->