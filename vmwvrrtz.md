代发 wailian999

split -l 1000 big.log part_
来源：http://mjf.0kj1m.cn

[R74] 批量重命名
来源：http://ltq.nanxuanxn.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vpl.sweek.top

[R75] 导出环境变量
来源：http://ute.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://xmy.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://swh.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lsz.dashuyun.cn

[R77] 读取用户输入
来源：http://bxc.yj202588.top

read -rp "请输入: " ans
来源：http://xye.xinyue.icu

[R78] 交互式菜单
来源：http://oyz.nanxinkj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nod.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://jxk.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cwa.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://fqx.smart0.xyz

time ./run.sh
来源：http://prm.52xcode.cn

================================================================================
来源：http://xyf.ctjpmb.com

S. C / C++ 专题
来源：http://dsw.hcnkem.com

================================================================================
来源：http://lrt.gzhubu.top

[S01] C：Hello World
来源：http://nne.hfpthk.cn

#include <stdio.h>
来源：http://pyn.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://stg.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://qcw.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://akw.gaohongyu789.top

[S03] C：读入整数
来源：http://vec.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://fth.zhoulong.xyz

[S04] C：字符串复制
来源：http://zax.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://fio.jlsjyb.cn

[S05] C：字符串长度
来源：http://lyw.tanke756.top

strlen(s)
来源：http://zfj.nanxinkj.top

[S06] C：字符串比较
来源：http://xwm.yj20258.top

strcmp(a, b) == 0
来源：http://bon.shanyushiyangtech.top

[S07] C：数组遍历求和
来源：http://agv.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yml.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://gtd.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hqq.dianchejie.cn

[S09] C：结构体定义与初始化
来源：http://gev.feifeiyinyue.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://apy.yangfankeji.com

[S10] C：指针与解引用
来源：http://jsx.yj202588.top

int *p = &a;  *p = 5;
来源：http://jqx.zhongyouzk.top

[S11] C：逐行读文件
来源：http://row.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://fiv.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://kgr.yuxming.cn

fclose(f);
来源：http://oik.tianlin.xyz

[S12] C：写文件
来源：http://hze.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wlr.yuxming.cn

[S13] C：宏定义
来源：http://brx.fktsv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qhb.zhijiandao.cn

[S14] C：枚举
来源：http://ckp.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://zvm.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://krf.zdqjudy.top

(double) a / b
来源：http://wuk.dianchejie.cn

[S16] C：位操作置位
来源：http://hvn.hongshengwenyu.top

x |= (1 << 3);
来源：http://xfv.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://ctq.jqgufenzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fga.dashuyun.cn

[S18] C：命令行参数
来源：http://uhi.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://cha.wangshuangyany.cn

[S19] C：快速排序
来源：http://sjw.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ebq.chenjidiqi.icu

[S20] C：二分查找
来源：http://swg.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dxc.ydjk.org.cn

[S21] C：字符类别判断
来源：http://cac.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aqu.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://pcz.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lye.jianghu66.top

[S23] C：随机数
来源：http://qmd.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vjk.gotoacloud.top

[S24] C：获取本地时间
来源：http://uxw.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://paa.quarkkingdee.top

[S25] C：内存拷贝
来源：http://awu.tianlin.xyz

memcpy(dst, src, n);
来源：http://ywi.jianghu66.top

[S26] C：内存清零
来源：http://yjp.snrcjt.cn

memset(a, 0, sizeof a);
来源：http://jfb.cashguo.top

[S27] C：定义常量
来源：http://vjg.zdqjudy.top

const double PI = 3.14159;
来源：http://ugw.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://aem.yvedp.cn

static int counter = 0;
来源：http://yoh.zhoulong.xyz

[S29] C：变参函数
来源：http://fjg.yanxiufei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kqy.havefunace.top

[S30] C：头文件保护
来源：http://kfk.yongpay.top

#ifndef X_H
来源：http://sjn.sjlbkw.cn

#define X_H
来源：http://nll.yangfankeji.com

#endif
来源：http://oud.gaohongyu789.top

[S31] C++：Hello World
来源：http://nxx.andypj.xyz

#include <iostream>
来源：http://ppm.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://nxb.gotoacloud.top

[S32] C++：字符串
来源：http://jqj.9152youxi.cn

std::string s = "hi";  s += "!";
来源：http://mpo.tianlin.xyz

[S33] C++：vector 增删
来源：http://ulq.uphjek.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ndp.cqqwz.cn

[S34] C++：遍历 vector
来源：http://huh.birdmap.top

for (auto &x : v) { std::cout << x; }
来源：http://rep.fehbvm.com

[S35] C++：map
来源：http://pnn.gaohongyu789.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tjc.hywenlv.cn

[S36] C++：unordered_map
来源：http://jvb.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kct.xylfe.cn

[S37] C++：set
来源：http://agz.pengpengdd.cyou

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xet.vqdsnc.cn

[S38] C++：排序
来源：http://gkz.zdbjq.cn

std::sort(v.begin(), v.end());
来源：http://ztg.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://zqp.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mra.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://svl.cucudq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iod.52xcode.cn

[S41] C++：类与构造函数
来源：http://jbb.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xiz.shuidangran.top

[S42] C++：继承与虚函数
来源：http://nrh.yj20258888.top

class B : public Base { public: void f() override {} };
来源：http://pyk.quarkkingdee.top

[S43] C++：智能指针
来源：http://rha.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://ryl.xylfe.cn

[S44] C++：引用传参
来源：http://hat.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://ovj.ppjwa.cn

[S45] C++：lambda
来源：http://hsj.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://svy.ybcxt.top

[S46] C++：函数模板
来源：http://dtw.hfpthk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zqr.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://xvj.tianlin.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ywq.dianchejie.cn

[S48] C++：逐行读文件
来源：http://mkw.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ezk.xinyue.icu

while (std::getline(in, line)) { }
来源：http://oeb.xylfe.cn

[S49] C++：写文件
来源：http://wuf.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nui.52xcode.cn

[S50] C++：格式化数字
来源：http://kyy.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://svr.quarkkingdee.top

[S51] C++：显式类型转换
来源：http://piw.yanxiufei.cn

static_cast<double>(a) / b
来源：http://rkm.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://ctb.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://rcy.mhx1999.top

[S53] C++：移动语义
来源：http://ijx.dianchejie.cn

std::vector<int> w = std::move(v);
来源：http://gmd.kuanghao11.cn

[S54] C++：异常处理
来源：http://ipc.wangshuangyany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ezb.9152youxi.cn

[S55] C++：结构化绑定
来源：http://yoo.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://huu.hesvh.cn

[S56] C++：optional
来源：http://ddw.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aaj.tarul.cn

[S57] C++：编译期常量
来源：http://hoh.tianlin.xyz

constexpr int N = 10;
来源：http://bze.316326.xyz

[S58] C++：命名空间
来源：http://orq.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://zor.jinqigufen.top

[S59] C++：静态断言
来源：http://sfg.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pis.quarkkingdee.top

[S60] C++：遍历并删除元素
来源：http://dlc.yj20258.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tqv.hnxiangtu.top

================================================================================
来源：http://qhr.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://odo.gogol.net.cn

================================================================================
来源：http://hhw.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://jcs.xuanzx.com

println("Hello")
来源：http://xgt.bjfxy.top

[T02] Kotlin：变量
来源：http://cxp.sufxvd.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cgd.hnxiangtu.top

[T03] Kotlin：字符串模板
来源：http://cwu.fzhhl.top

"值: $b"
来源：http://lch.nanxinkj.top

[T04] Kotlin：空安全
来源：http://qyi.xziqi.cn

val n: String? = null;  n?.length
来源：http://lev.xingfuxueyuan.xyz

[T05] Kotlin：when 表达式
来源：http://mlp.yuxming.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hsa.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://dof.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tyu.tanke756.top

[T07] Kotlin：集合过滤
来源：http://hyq.tianlin.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://gyq.jinqigufen.top

[T08] Kotlin：数据类
来源：http://bte.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://jbg.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://lic.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://xqa.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://exj.cucudq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rmv.epnwcf.com

[T11] Kotlin：协程
来源：http://uxv.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jjr.hnqzz.top

[T12] Kotlin：解构声明
来源：http://fsu.yueranfly.top

val (a, b) = Pair(1, 2)
来源：http://vcb.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://dvs.pycfn.com

val m = mapOf("a" to 1)
来源：http://mak.bbcook.cn

[T14] Kotlin：循环
来源：http://bgs.guowangkeji.top

for (i in 1..10) println(i)
来源：http://jpi.redwolf501.top

[T15] Kotlin：接口
来源：http://mgy.hysaishi.cn

interface Shape { fun area(): Double }
来源：http://qjr.nanxuanxn.top

[T16] Swift：Hello World
来源：http://eaf.0kj1m.cn

print("Hello")
来源：http://ltz.ctjpmb.com

[T17] Swift：变量与常量
来源：http://ary.cheryme.top

var a = 1;  let b = 2
来源：http://epz.svipenyu.cn

[T18] Swift：字符串插值
来源：http://net.guannengcc.top

"值: \(b)"
来源：http://vbx.yonumen.top

[T19] Swift：可选绑定
来源：http://ltn.shzxlz.cn

if let n = opt { print(n) }
来源：http://trx.guowangkeji.top

[T20] Swift：数组操作
来源：http://gll.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://quz.xinyue.icu

[T21] Swift：遍历
来源：http://rzi.yuanzhike.top

for x in a { print(x) }
来源：http://hvi.iojbl.cn

[T22] Swift：字典
来源：http://kvm.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://tvy.ivvv.top

[T23] Swift：函数
来源：http://dkb.hnxiangtu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://evu.hongshengwenyu.top

[T24] Swift：闭包
来源：http://zhp.yuanzhike.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ydb.sysykeji.top

[T25] Swift：结构体
来源：http://cpj.quarkkingdee.top

struct P { var x: Int }
来源：http://ady.xuetiantiany.cn

[T26] Swift：类与重写
来源：http://hch.316326.xyz

class A: Base { override func f() {} }
来源：http://izf.cashguo.top

[T27] Swift：错误处理
来源：http://hwi.hnqzz.top

do { try f() } catch { print(error) }
来源：http://uzh.cucudq.cn

[T28] Swift：枚举
来源：http://oia.jinqigfzy.top

enum Color { case red, green }
来源：http://bzr.shanyushiyangtech.top

[T29] Swift：guard 提前返回
来源：http://yzz.zdqjudy.top

guard let x = opt else { return }
来源：http://aof.sweek.top

[T30] Swift：协议
来源：http://dto.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://kjr.hesvh.cn

[T31] Lua：Hello World
来源：http://pck.jinqigfzy.top

print("Hello")
来源：http://okm.feifeiyinyue.top

[T32] Lua：局部变量
来源：http://zkv.hongshengwenyu.top

local a = 1
来源：http://zxi.tanke756.top

[T33] Lua：表（数组）
来源：http://dsx.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vft.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://ppn.cashguo.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ztd.ybcxt.top

[T35] Lua：字典表
来源：http://zhl.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://bcu.ydzc1.top

[T36] Lua：函数
来源：http://sth.zhixingplan.top

function add(a, b) return a + b end
来源：http://nlk.shanyushiyangtech.top

[T37] Lua：字符串拼接
来源：http://xzt.cucudq.cn

"a" .. "b"
来源：http://cag.xinyue.icu

[T38] Lua：条件
来源：http://qwb.wangshuangyany.cn

if x > 0 then print("正") end
来源：http://xlo.fengsongda.top

[T39] Lua：模式匹配
来源：http://elg.xuetiantiany.cn

string.find(s, "%d+")
来源：http://qxs.yonumen.top

[T40] Lua：元表
来源：http://awp.jyoumei.cn

setmetatable({}, { __index = base })
来源：http://xxe.c1oappe.top

[T41] Perl：Hello World
来源：http://dhe.gogol.net.cn

print "Hello\n";
来源：http://dzb.zycfv.cn

[T42] Perl：变量类型
来源：http://oaj.yongpay.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nsp.ctjpmb.com

[T43] Perl：字符串插值
来源：http://vfu.yj20258.top

"值: $a"
来源：http://hnj.shuidangran.top

[T44] Perl：条件
来源：http://hjb.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://oxr.bbcook.cn

[T45] Perl：数组遍历
来源：http://bly.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://ptt.sweek.top

[T46] Perl：哈希操作
来源：http://jdv.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yob.hnqzz.top

[T47] Perl：正则捕获
来源：http://sfr.ehwqpu.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://ebu.pycfn.com

[T48] Perl：正则替换
来源：http://kjg.zhengqikj.top

$s =~ s/old/new/g;
来源：http://hup.tarul.cn

[T49] Perl：函数
来源：http://fje.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ayd.hysaishi.cn

[T50] Perl：逐行读文件
来源：http://jey.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kht.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://gbo.fanxiaobao.xyz

[T51] Scala：Hello World
来源：http://fzz.hongshengwenyu.top

println("Hello")
来源：http://tlt.xziqi.cn

[T52] Scala：变量
来源：http://xok.xuanzx.com

val a = 1;  var b = 2
来源：http://kzf.cucudq.cn

[T53] Scala：字符串插值
来源：http://ypl.zhaomingkeji.xyz

s"值: $b"
来源：http://qhf.haohaochexian.top

[T54] Scala：集合映射
来源：http://vwy.fktsv.cn

List(1, 2, 3).map(_ * 2)
来源：http://rfv.cashguo.top

[T55] Scala：集合过滤
来源：http://vlh.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://quh.pengpengdd.cyou

[T56] Scala：样例类
来源：http://juu.xuanzx.com

case class User(name: String, age: Int)
来源：http://tab.sxryk.cn

[T57] Scala：模式匹配
来源：http://dvf.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://ivh.guowangkeji.top

[T58] Scala：函数定义
来源：http://dah.c1oappe.top

def add(a: Int, b: Int): Int = a + b
来源：http://mfr.guannengcc.top

[T59] Scala：循环
来源：http://hkw.zhongyouzk.top

for (i <- 1 to 10) println(i)
来源：http://qcq.kuanghao11.cn

[T60] Scala：折叠
来源：http://hbv.chenzaomai.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qoz.nwbrower.top

================================================================================
来源：http://bli.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jan.yongpay.top

================================================================================
来源：http://ctr.uphjek.com

[U01] Py：创建虚拟环境
来源：http://ikv.pycfn.com

python -m venv .venv && source .venv/bin/activate
来源：http://wcr.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://gbd.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mdo.jyoumei.cn

[U03] Py：加载 .env 配置
来源：http://fjq.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ftd.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://ufw.zhijiandao.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ixd.uphjek.com

[U05] Py：列表去重且保序
来源：http://mtq.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://ujp.andypj.xyz

[U06] Py：合并两个字典
来源：http://aue.cdnleiting.top

{**a, **b}
来源：http://fze.hfpthk.cn

[U07] Py：反转字典键值
来源：http://mot.iojbl.cn

{v: k for k, v in d.items()}
来源：http://pbg.quarkkingdee.top

[U08] Py：展平二维列表
来源：http://pen.hcnkem.com

[y for x in nested for y in x]
来源：http://dks.ydjk.org.cn

[U09] Py：字典取最大值的键
来源：http://foy.wangshuangyany.cn

max(d, key=d.get)
来源：http://nox.0kj1m.cn

[U10] Py：按值排序字典
来源：http://hlf.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://har.hcnkem.com

[U11] Py：生成器表达式
来源：http://fgb.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://zpt.bbcook.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qmb.cucudq.cn

Counter(arr).most_common(3)
来源：http://tai.zhixingplan.top

[U13] Py：固定长度队列
来源：http://ruv.dashuyun.cn

deque(maxlen=10)
来源：http://hki.daxiang520.top

[U14] Py：分组收集到列表
来源：http://syq.smart0.xyz

defaultdict(list)
来源：http://vvg.shzxlz.cn


<!-- 参考信息 -->