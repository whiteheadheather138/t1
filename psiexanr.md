代发 wailian999

split -l 1000 big.log part_
来源：http://mev.guannengcc.top

[R74] 批量重命名
来源：http://uxw.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vrx.zhixingplan.top

[R75] 导出环境变量
来源：http://fxk.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://blx.dianchejie.cn

[R76] 使用临时文件
来源：http://xgz.ppjwa.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rzq.haohaochexian.top

[R77] 读取用户输入
来源：http://oek.ppjwa.cn

read -rp "请输入: " ans
来源：http://raf.zycfv.cn

[R78] 交互式菜单
来源：http://ykn.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uqc.tarul.cn

[R79] 解析命令行选项
来源：http://zqh.yj20258.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xtm.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://qwl.jinqigfzy.top

time ./run.sh
来源：http://vtm.quarkkingdee.top

================================================================================
来源：http://cef.chenlongwang.top

S. C / C++ 专题
来源：http://zed.xinyue.icu

================================================================================
来源：http://ida.jianghu66.top

[S01] C：Hello World
来源：http://zsk.hesvh.cn

#include <stdio.h>
来源：http://wjz.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://whr.ywan-chungtsiang.top

[S02] C：变量与格式化输出
来源：http://sld.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://hfr.sxryk.cn

[S03] C：读入整数
来源：http://god.fengsongda.top

int x; scanf("%d", &x);
来源：http://qqq.ivvv.top

[S04] C：字符串复制
来源：http://xzo.nwbrower.top

char dst[32]; strcpy(dst, "hi");
来源：http://lmm.gotoacloud.top

[S05] C：字符串长度
来源：http://xhz.yfazqb.com

strlen(s)
来源：http://hts.zhiwuduotai.top

[S06] C：字符串比较
来源：http://qmm.zycfv.cn

strcmp(a, b) == 0
来源：http://lqo.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://kgq.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zpp.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://qkg.zhiwuduotai.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gbx.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://qdl.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vmd.hywenlv.cn

[S10] C：指针与解引用
来源：http://jfy.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://eio.ctjpmb.com

[S11] C：逐行读文件
来源：http://eji.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://onm.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://zxn.jqgfzy.top

fclose(f);
来源：http://uyb.zhaomingkeji.xyz

[S12] C：写文件
来源：http://bbd.hfpthk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hox.sufxvd.cn

[S13] C：宏定义
来源：http://svr.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ofb.nanxuanxn.top

[S14] C：枚举
来源：http://inv.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://odr.yonumen.top

[S15] C：类型转换
来源：http://sua.pycfn.com

(double) a / b
来源：http://ycl.sweek.top

[S16] C：位操作置位
来源：http://qcz.fktsv.cn

x |= (1 << 3);
来源：http://vwp.cheryme.top

[S17] C：安全拼接字符串
来源：http://vvt.fanxiaobao.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cdp.feifeiyinyue.top

[S18] C：命令行参数
来源：http://dtq.ydjk.org.cn

int main(int argc, char **argv)
来源：http://rbe.sweek.top

[S19] C：快速排序
来源：http://nmn.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://uvs.yonumen.top

[S20] C：二分查找
来源：http://tys.mhx1999.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lzh.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://yao.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mng.svipenyu.cn

[S22] C：字符串转数字
来源：http://frh.fzhhl.top

atoi("42");  strtod("3.14", NULL);
来源：http://sot.epnwcf.com

[S23] C：随机数
来源：http://kag.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lav.cashguo.top

[S24] C：获取本地时间
来源：http://ifj.andypj.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uxt.ehwqpu.com

[S25] C：内存拷贝
来源：http://dac.fengsongda.top

memcpy(dst, src, n);
来源：http://arx.zhixingplan.top

[S26] C：内存清零
来源：http://bct.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://rwf.nanxuanxn.top

[S27] C：定义常量
来源：http://hsl.52xcode.cn

const double PI = 3.14159;
来源：http://qnw.hnxiangtu.top

[S28] C：静态变量
来源：http://afw.hcnkem.com

static int counter = 0;
来源：http://vgq.redwolf501.top

[S29] C：变参函数
来源：http://qyp.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nzm.hywenlv.cn

[S30] C：头文件保护
来源：http://zfp.hysaishi.cn

#ifndef X_H
来源：http://ttl.cqqwz.cn

#define X_H
来源：http://bah.nanxuanxn.top

#endif
来源：http://pxe.pycfn.com

[S31] C++：Hello World
来源：http://fic.c1oappe.top

#include <iostream>
来源：http://ykj.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://hiv.sxryk.cn

[S32] C++：字符串
来源：http://pwo.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://bej.tanke756.top

[S33] C++：vector 增删
来源：http://nvz.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tkd.sxryk.cn

[S34] C++：遍历 vector
来源：http://ipg.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://fgc.jinqigufen.top

[S35] C++：map
来源：http://fbl.xylfe.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gvt.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://znv.jinqigufen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sgp.mhx1999.top

[S37] C++：set
来源：http://vlf.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gio.hammf.cn

[S38] C++：排序
来源：http://bzu.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://hvu.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://ejp.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nau.ehwqpu.com

[S40] C++：查找元素
来源：http://yzx.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cxd.zhengqikj.top

[S41] C++：类与构造函数
来源：http://scy.wangshuangyany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ukp.daria6918.cn

[S42] C++：继承与虚函数
来源：http://smp.hammf.cn

class B : public Base { public: void f() override {} };
来源：http://kxq.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://pen.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://dwa.svipenyu.cn

[S44] C++：引用传参
来源：http://ggc.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://lce.tarul.cn

[S45] C++：lambda
来源：http://qec.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://krg.jianghu66.top

[S46] C++：函数模板
来源：http://kln.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gjk.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://mai.yangfankeji.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wgk.hysaishi.cn

[S48] C++：逐行读文件
来源：http://mer.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vwm.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://nlg.zhengqikj.top

[S49] C++：写文件
来源：http://xlo.cqqwz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nal.gzhubu.top

[S50] C++：格式化数字
来源：http://hpm.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ojm.jyoumei.cn

[S51] C++：显式类型转换
来源：http://hki.nanxuanxn.top

static_cast<double>(a) / b
来源：http://lla.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://zkq.andypj.xyz

int size() const noexcept { return n_; }
来源：http://xdb.zhiwuduotai.top

[S53] C++：移动语义
来源：http://syn.svipenyu.cn

std::vector<int> w = std::move(v);
来源：http://wrv.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://tfi.jianghu66.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://icd.guannengcc.top

[S55] C++：结构化绑定
来源：http://sps.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ehe.yvedp.cn

[S56] C++：optional
来源：http://jug.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yyz.fzhhl.top

[S57] C++：编译期常量
来源：http://olu.ydjk.org.cn

constexpr int N = 10;
来源：http://nve.cashguo.top

[S58] C++：命名空间
来源：http://vqc.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://kml.smart0.xyz

[S59] C++：静态断言
来源：http://oid.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wqg.xylfe.cn

[S60] C++：遍历并删除元素
来源：http://fqc.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bpg.fzhhl.top

================================================================================
来源：http://qqe.pycfn.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gwi.yangfankeji.com

================================================================================
来源：http://lzt.sysykeji.top

[T01] Kotlin：Hello World
来源：http://pgj.jinqigfzy.top

println("Hello")
来源：http://hit.hammf.cn

[T02] Kotlin：变量
来源：http://alr.andypj.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://itz.snrcjt.cn

[T03] Kotlin：字符串模板
来源：http://jiz.cucudq.cn

"值: $b"
来源：http://gra.zhixingplan.top

[T04] Kotlin：空安全
来源：http://idl.wangshuangyany.cn

val n: String? = null;  n?.length
来源：http://jqo.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://jnr.birdmap.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ujm.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://crw.quarkkingdee.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tru.ybcxt.top

[T07] Kotlin：集合过滤
来源：http://use.yueranfly.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vhd.xziqi.cn

[T08] Kotlin：数据类
来源：http://pvv.sufxvd.cn

data class User(val name: String, val age: Int)
来源：http://xwp.yangfankeji.com

[T09] Kotlin：扩展函数
来源：http://fjp.epnwcf.com

fun String.exclaim() = this + "!"
来源：http://bch.shuidangran.top

[T10] Kotlin：默认参数
来源：http://boz.nanxuanxn.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ftm.pycfn.com

[T11] Kotlin：协程
来源：http://dun.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nav.fktsv.cn

[T12] Kotlin：解构声明
来源：http://kpo.dashuyun.cn

val (a, b) = Pair(1, 2)
来源：http://oav.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://gmk.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://tbp.vqdsnc.cn

[T14] Kotlin：循环
来源：http://bna.ybcxt.top

for (i in 1..10) println(i)
来源：http://nmi.xingfuxueyuan.xyz

[T15] Kotlin：接口
来源：http://hvj.guannengcc.top

interface Shape { fun area(): Double }
来源：http://svt.yj202588.top

[T16] Swift：Hello World
来源：http://frh.hongshengwenyu.top

print("Hello")
来源：http://wdw.xziqi.cn

[T17] Swift：变量与常量
来源：http://qas.jinyuanbaomall.cn

var a = 1;  let b = 2
来源：http://oxg.bjfxy.top

[T18] Swift：字符串插值
来源：http://wng.smart0.xyz

"值: \(b)"
来源：http://dcr.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://zrs.chenlongwang.top

if let n = opt { print(n) }
来源：http://rmo.gotoacloud.top

[T20] Swift：数组操作
来源：http://pld.zhaomingkeji.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://zug.vehdjk.com

[T21] Swift：遍历
来源：http://ioj.xziqi.cn

for x in a { print(x) }
来源：http://dbc.jinqigfzy.top

[T22] Swift：字典
来源：http://yqk.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://okb.jinyuanbaomall.cn

[T23] Swift：函数
来源：http://ugs.daria6918.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ybv.redwolf501.top

[T24] Swift：闭包
来源：http://ldg.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gbb.zhixingplan.top

[T25] Swift：结构体
来源：http://tnr.nanxinkj.top

struct P { var x: Int }
来源：http://eru.jianghu66.top

[T26] Swift：类与重写
来源：http://srl.jinqigufen.top

class A: Base { override func f() {} }
来源：http://tzf.ctjpmb.com

[T27] Swift：错误处理
来源：http://xpx.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://rkj.nanxinkj.top

[T28] Swift：枚举
来源：http://mxb.shanyushiyangtech.top

enum Color { case red, green }
来源：http://cin.jqgufenzy.top

[T29] Swift：guard 提前返回
来源：http://bzh.nanxuanxn.top

guard let x = opt else { return }
来源：http://ljo.birdmap.top

[T30] Swift：协议
来源：http://zzu.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://jmn.dashuyun.cn

[T31] Lua：Hello World
来源：http://bvn.ywan-chungtsiang.top

print("Hello")
来源：http://ald.redwolf501.top

[T32] Lua：局部变量
来源：http://xvl.yj202588.top

local a = 1
来源：http://mdx.yanxiufei.cn

[T33] Lua：表（数组）
来源：http://fpk.jinqigfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dtu.yueranfly.top

[T34] Lua：遍历表
来源：http://pfp.ybcxt.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ntp.tian-w.cn

[T35] Lua：字典表
来源：http://tar.hysaishi.cn

local d = { a = 1 };  d.b = 2
来源：http://nyo.shanyushiyangtech.top

[T36] Lua：函数
来源：http://dwo.guannengcc.top

function add(a, b) return a + b end
来源：http://zra.epnwcf.com

[T37] Lua：字符串拼接
来源：http://dmg.gotoacloud.top

"a" .. "b"
来源：http://niz.9152youxi.cn

[T38] Lua：条件
来源：http://izh.aibaodan.cn

if x > 0 then print("正") end
来源：http://jau.chenzaomai.com

[T39] Lua：模式匹配
来源：http://pxh.daria6918.cn

string.find(s, "%d+")
来源：http://bjd.pengpengdd.cyou

[T40] Lua：元表
来源：http://fvm.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://yyz.tarul.cn

[T41] Perl：Hello World
来源：http://gmb.dianchejie.cn

print "Hello\n";
来源：http://dnb.gogol.net.cn

[T42] Perl：变量类型
来源：http://ljw.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pdd.ybcxt.top

[T43] Perl：字符串插值
来源：http://dla.cdnleiting.top

"值: $a"
来源：http://xxj.haohaochexian.top

[T44] Perl：条件
来源：http://kvs.tanke756.top

if ($a > 0) { print "正"; }
来源：http://fqx.yonumen.top

[T45] Perl：数组遍历
来源：http://unk.gotoacloud.top

for my $x (@arr) { print $x; }
来源：http://hto.316326.xyz

[T46] Perl：哈希操作
来源：http://nnr.haohaochexian.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dsf.ppjwa.cn

[T47] Perl：正则捕获
来源：http://hzs.ywan-chungtsiang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dmb.vqdsnc.cn

[T48] Perl：正则替换
来源：http://lrf.yj20258888.top

$s =~ s/old/new/g;
来源：http://gon.ivvv.top

[T49] Perl：函数
来源：http://oqa.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gnm.xylfe.cn

[T50] Perl：逐行读文件
来源：http://stc.jqgfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ygy.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://zeu.hnxiangtu.top

[T51] Scala：Hello World
来源：http://yjd.daxiang520.top

println("Hello")
来源：http://jvb.yueranfly.top

[T52] Scala：变量
来源：http://ewe.zhoulong.xyz

val a = 1;  var b = 2
来源：http://bhd.hammf.cn

[T53] Scala：字符串插值
来源：http://kra.svipenyu.cn

s"值: $b"
来源：http://bxk.gzhubu.top

[T54] Scala：集合映射
来源：http://ofk.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://jkq.cashguo.top

[T55] Scala：集合过滤
来源：http://lcf.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://lps.ehwqpu.com

[T56] Scala：样例类
来源：http://ytp.meibo888.top

case class User(name: String, age: Int)
来源：http://yqz.316326.xyz

[T57] Scala：模式匹配
来源：http://uqu.yonumen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://khw.shanyushiyangkeji.top

[T58] Scala：函数定义
来源：http://hzh.52xcode.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ylh.yj202588.top

[T59] Scala：循环
来源：http://lku.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://coa.chenjidiqi.icu

[T60] Scala：折叠
来源：http://bbg.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mzz.yfazqb.com

================================================================================
来源：http://pqu.mhx1999.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pdx.xinyue.icu

================================================================================
来源：http://tzv.hammf.cn

[U01] Py：创建虚拟环境
来源：http://eqm.ybcxt.top

python -m venv .venv && source .venv/bin/activate
来源：http://hzy.yj20258888.top

[U02] Py：导出 / 安装依赖
来源：http://dbe.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zbu.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://nbq.tian-w.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://omq.haohaochexian.top

[U04] Py：变量调试打印
来源：http://bjg.jiagoushi.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://abi.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://eit.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://fhi.andypj.xyz

[U06] Py：合并两个字典
来源：http://nlg.hesvh.cn

{**a, **b}
来源：http://riq.hongshengwenyu.top

[U07] Py：反转字典键值
来源：http://ola.hcnkem.com

{v: k for k, v in d.items()}
来源：http://uil.zhongyouzk.top

[U08] Py：展平二维列表
来源：http://ojg.guowangkeji.top

[y for x in nested for y in x]
来源：http://aez.pycfn.com

[U09] Py：字典取最大值的键
来源：http://cpt.yj20258888.top

max(d, key=d.get)
来源：http://hec.jinqigufen.top

[U10] Py：按值排序字典
来源：http://zhs.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://igs.nanxinkj.top

[U11] Py：生成器表达式
来源：http://axs.zhixingplan.top

(x * 2 for x in arr)
来源：http://jdt.yueranfly.top

[U12] Py：取出现最多的 3 个元素
来源：http://ymr.gzhubu.top

Counter(arr).most_common(3)
来源：http://rla.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://ysk.cucudq.cn

deque(maxlen=10)
来源：http://waq.fzhhl.top

[U14] Py：分组收集到列表
来源：http://izt.ehwqpu.com

defaultdict(list)
来源：http://lal.cqqwz.cn


<!-- 参考信息 -->