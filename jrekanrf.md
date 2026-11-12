代发 wailian999

split -l 1000 big.log part_
来源：http://hyf.vqdsnc.cn

[R74] 批量重命名
来源：http://hqs.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kgy.haohaochexian.top

[R75] 导出环境变量
来源：http://ral.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://umf.andypj.xyz

[R76] 使用临时文件
来源：http://qhe.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oyd.epnwcf.com

[R77] 读取用户输入
来源：http://mjm.cdnleiting.top

read -rp "请输入: " ans
来源：http://mij.tarul.cn

[R78] 交互式菜单
来源：http://oei.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hms.ivvv.top

[R79] 解析命令行选项
来源：http://dem.shanyushiyangtech.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mwq.fzhhl.top

[R80] 查看脚本执行耗时
来源：http://edn.zhoulong.xyz

time ./run.sh
来源：http://izo.xinyue.icu

================================================================================
来源：http://gvf.redwolf501.top

S. C / C++ 专题
来源：http://dnd.ydjk.org.cn

================================================================================
来源：http://rkk.daria6918.cn

[S01] C：Hello World
来源：http://oqr.aibaodan.cn

#include <stdio.h>
来源：http://oaz.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://nrv.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://ppv.jinqigfzy.top

int a = 10; printf("%d\n", a);
来源：http://fen.zhengqikj.top

[S03] C：读入整数
来源：http://aaj.ybcxt.top

int x; scanf("%d", &x);
来源：http://hsw.xuetiantiany.cn

[S04] C：字符串复制
来源：http://eqo.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vbr.tianlin.xyz

[S05] C：字符串长度
来源：http://vhn.xuanzx.com

strlen(s)
来源：http://cpt.9152youxi.cn

[S06] C：字符串比较
来源：http://hic.sysykeji.top

strcmp(a, b) == 0
来源：http://lmw.shangyingyoupin.top

[S07] C：数组遍历求和
来源：http://mjb.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bbd.dashuyun.cn

[S08] C：动态内存分配与释放
来源：http://iqh.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ivs.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://fez.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ajv.yonumen.top

[S10] C：指针与解引用
来源：http://ryy.cheryme.top

int *p = &a;  *p = 5;
来源：http://eoj.gaohongyu789.top

[S11] C：逐行读文件
来源：http://fjf.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://zol.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cfl.sxryk.cn

fclose(f);
来源：http://jkj.yuanzhike.top

[S12] C：写文件
来源：http://acp.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rks.zhaomingkeji.xyz

[S13] C：宏定义
来源：http://szf.wangshuangyany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kxs.zycfv.cn

[S14] C：枚举
来源：http://nqu.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://ery.shuidangran.top

[S15] C：类型转换
来源：http://bgx.fzhhl.top

(double) a / b
来源：http://pcd.9152youxi.cn

[S16] C：位操作置位
来源：http://stv.haohaochexian.top

x |= (1 << 3);
来源：http://tmm.sysykeji.top

[S17] C：安全拼接字符串
来源：http://dab.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://liw.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://hdw.52xcode.cn

int main(int argc, char **argv)
来源：http://rdf.iojbl.cn

[S19] C：快速排序
来源：http://dum.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://zfp.hysaishi.cn

[S20] C：二分查找
来源：http://rne.shuidangran.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aqf.hfpthk.cn

[S21] C：字符类别判断
来源：http://luj.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hqv.sufxvd.cn

[S22] C：字符串转数字
来源：http://jeu.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lxw.52xcode.cn

[S23] C：随机数
来源：http://vud.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://xnh.hnxiangtu.top

[S24] C：获取本地时间
来源：http://sqc.bjfxy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://daa.xinyue.icu

[S25] C：内存拷贝
来源：http://ths.jinqigfzy.top

memcpy(dst, src, n);
来源：http://rny.ybcxt.top

[S26] C：内存清零
来源：http://yiv.haohaochexian.top

memset(a, 0, sizeof a);
来源：http://lxk.mhx1999.top

[S27] C：定义常量
来源：http://jxx.yj20258888.top

const double PI = 3.14159;
来源：http://bob.guowangkeji.top

[S28] C：静态变量
来源：http://zrd.xziqi.cn

static int counter = 0;
来源：http://wjg.shangyingyoupin.top

[S29] C：变参函数
来源：http://tgs.cashguo.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pbs.quarkkingdee.top

[S30] C：头文件保护
来源：http://vjn.jinqigfzy.top

#ifndef X_H
来源：http://rwc.zhiwuduotai.top

#define X_H
来源：http://bkb.nanxuanxn.top

#endif
来源：http://tms.uphjek.com

[S31] C++：Hello World
来源：http://phk.yuxming.cn

#include <iostream>
来源：http://sbc.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://oft.yonumen.top

[S32] C++：字符串
来源：http://fdd.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://qsi.dianchejie.cn

[S33] C++：vector 增删
来源：http://ibl.pengpengdd.cyou

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uqt.cdnleiting.top

[S34] C++：遍历 vector
来源：http://hgs.zdqjudy.top

for (auto &x : v) { std::cout << x; }
来源：http://jul.gzhubu.top

[S35] C++：map
来源：http://hjf.aibaodan.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hws.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://tfq.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kdf.haohaochexian.top

[S37] C++：set
来源：http://xhz.ybcxt.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ojh.fanxiaobao.xyz

[S38] C++：排序
来源：http://ihn.ppjwa.cn

std::sort(v.begin(), v.end());
来源：http://iab.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://usp.zhixingplan.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://adf.cucudq.cn

[S40] C++：查找元素
来源：http://uwg.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://twl.316326.xyz

[S41] C++：类与构造函数
来源：http://ggv.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dwk.yuxming.cn

[S42] C++：继承与虚函数
来源：http://jmv.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://xgr.xuetiantiany.cn

[S43] C++：智能指针
来源：http://eyl.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://dhl.xuanzx.com

[S44] C++：引用传参
来源：http://lel.zycfv.cn

void inc(int &x) { ++x; }
来源：http://qto.yvedp.cn

[S45] C++：lambda
来源：http://lug.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bhi.yongpay.top

[S46] C++：函数模板
来源：http://rsu.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ybc.vehdjk.com

[S47] C++：结构化绑定遍历
来源：http://yad.tarul.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qlx.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://vog.fengsongda.top

std::ifstream in("a.txt");  std::string line;
来源：http://rbp.jinqigfzy.top

while (std::getline(in, line)) { }
来源：http://eqx.hysaishi.cn

[S49] C++：写文件
来源：http://tyv.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tau.zhongyouzk.top

[S50] C++：格式化数字
来源：http://wvj.yfazqb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dny.ybcxt.top

[S51] C++：显式类型转换
来源：http://gnh.cheryme.top

static_cast<double>(a) / b
来源：http://azh.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://fqt.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://rdy.sjlbkw.cn

[S53] C++：移动语义
来源：http://erx.52xcode.cn

std::vector<int> w = std::move(v);
来源：http://dps.zhixingplan.top

[S54] C++：异常处理
来源：http://gws.epnwcf.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bvq.yj202588.top

[S55] C++：结构化绑定
来源：http://auf.gogol.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yqw.chenlongwang.top

[S56] C++：optional
来源：http://ndi.snrcjt.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dkr.yuxming.cn

[S57] C++：编译期常量
来源：http://rvb.havefunace.top

constexpr int N = 10;
来源：http://sbq.bjfxy.top

[S58] C++：命名空间
来源：http://wkk.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://lov.yfazqb.com

[S59] C++：静态断言
来源：http://fuz.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nla.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://kkc.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nph.vqdsnc.cn

================================================================================
来源：http://tib.xziqi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://viy.dashuyun.cn

================================================================================
来源：http://nko.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://sqd.andypj.xyz

println("Hello")
来源：http://lkg.iojbl.cn

[T02] Kotlin：变量
来源：http://lae.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zci.52xcode.cn

[T03] Kotlin：字符串模板
来源：http://cgn.gzhubu.top

"值: $b"
来源：http://roc.hywenlv.cn

[T04] Kotlin：空安全
来源：http://nql.ivvv.top

val n: String? = null;  n?.length
来源：http://xxo.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://oxx.hywenlv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gxz.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://lbz.hnxiangtu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xce.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://aip.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xfz.chenjidiqi.icu

[T08] Kotlin：数据类
来源：http://bpi.yuxming.cn

data class User(val name: String, val age: Int)
来源：http://ylw.yonumen.top

[T09] Kotlin：扩展函数
来源：http://epd.yj20258.top

fun String.exclaim() = this + "!"
来源：http://jok.zhixingplan.top

[T10] Kotlin：默认参数
来源：http://kgy.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ixt.daria6918.cn

[T11] Kotlin：协程
来源：http://qvh.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ilz.ehwqpu.com

[T12] Kotlin：解构声明
来源：http://dtz.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://kxm.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://rxo.nwbrower.top

val m = mapOf("a" to 1)
来源：http://edu.redwolf501.top

[T14] Kotlin：循环
来源：http://vsu.smart0.xyz

for (i in 1..10) println(i)
来源：http://oso.ctjpmb.com

[T15] Kotlin：接口
来源：http://vrc.ctjpmb.com

interface Shape { fun area(): Double }
来源：http://qnt.sweek.top

[T16] Swift：Hello World
来源：http://sey.yongpay.top

print("Hello")
来源：http://pxq.iojbl.cn

[T17] Swift：变量与常量
来源：http://cvx.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://xkg.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://grb.yj20258888.top

"值: \(b)"
来源：http://tzt.jiagoushi.top

[T19] Swift：可选绑定
来源：http://wfb.redwolf501.top

if let n = opt { print(n) }
来源：http://vko.feifeiyinyue.top

[T20] Swift：数组操作
来源：http://oie.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hkh.daxiang520.top

[T21] Swift：遍历
来源：http://jaf.sysykeji.top

for x in a { print(x) }
来源：http://ryx.yuanzhike.top

[T22] Swift：字典
来源：http://ych.fktsv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nfe.hfpthk.cn

[T23] Swift：函数
来源：http://fxl.cdnleiting.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dsn.nanxinkj.top

[T24] Swift：闭包
来源：http://hme.zhongyouzk.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lft.svipenyu.cn

[T25] Swift：结构体
来源：http://ern.zycfv.cn

struct P { var x: Int }
来源：http://wwt.ydzc1.top

[T26] Swift：类与重写
来源：http://gtn.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://yzr.guowangkeji.top

[T27] Swift：错误处理
来源：http://koi.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://vzj.nwbrower.top

[T28] Swift：枚举
来源：http://pdo.zdbjq.cn

enum Color { case red, green }
来源：http://avv.xylfe.cn

[T29] Swift：guard 提前返回
来源：http://pag.yangfankeji.com

guard let x = opt else { return }
来源：http://evi.nanxinkj.top

[T30] Swift：协议
来源：http://qhx.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://inx.fengsongda.top

[T31] Lua：Hello World
来源：http://okg.ydzc1.top

print("Hello")
来源：http://inm.snrcjt.cn

[T32] Lua：局部变量
来源：http://dav.0kj1m.cn

local a = 1
来源：http://ptk.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://nwk.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://unw.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://taw.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nqw.hfpthk.cn

[T35] Lua：字典表
来源：http://dov.zhiwuduotai.top

local d = { a = 1 };  d.b = 2
来源：http://bhe.hysaishi.cn

[T36] Lua：函数
来源：http://etr.bbcook.cn

function add(a, b) return a + b end
来源：http://wig.uphjek.com

[T37] Lua：字符串拼接
来源：http://ayg.chenjidiqi.icu

"a" .. "b"
来源：http://xqp.sjlbkw.cn

[T38] Lua：条件
来源：http://mkx.yvedp.cn

if x > 0 then print("正") end
来源：http://rkg.xuetiantiany.cn

[T39] Lua：模式匹配
来源：http://taz.yonumen.top

string.find(s, "%d+")
来源：http://kwl.sufxvd.cn

[T40] Lua：元表
来源：http://nxu.ybcxt.top

setmetatable({}, { __index = base })
来源：http://bnq.shanyushiyangtech.top

[T41] Perl：Hello World
来源：http://mif.zdqjudy.top

print "Hello\n";
来源：http://vco.xingfuxueyuan.xyz

[T42] Perl：变量类型
来源：http://qlg.tianlin.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://izt.ivvv.top

[T43] Perl：字符串插值
来源：http://naq.bjfxy.top

"值: $a"
来源：http://xqb.feifeiyinyue.top

[T44] Perl：条件
来源：http://eaz.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://yho.guowangkeji.top

[T45] Perl：数组遍历
来源：http://ket.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://gdm.ivvv.top

[T46] Perl：哈希操作
来源：http://hwj.sysykeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://czy.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://lyz.jlsjyb.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://psn.birdmap.top

[T48] Perl：正则替换
来源：http://vmf.gotoacloud.top

$s =~ s/old/new/g;
来源：http://cun.yangfankeji.com

[T49] Perl：函数
来源：http://tiy.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hiw.shangyingyoupin.top

[T50] Perl：逐行读文件
来源：http://knq.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://ppa.gzhubu.top

while (my $line = <$fh>) { print $line; }
来源：http://drr.hcnkem.com

[T51] Scala：Hello World
来源：http://igr.nwbrower.top

println("Hello")
来源：http://qke.hcnkem.com

[T52] Scala：变量
来源：http://blf.nwbrower.top

val a = 1;  var b = 2
来源：http://ycj.tarul.cn

[T53] Scala：字符串插值
来源：http://ras.zdqjudy.top

s"值: $b"
来源：http://rev.zhijiandao.cn

[T54] Scala：集合映射
来源：http://nuc.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://qwl.ctjpmb.com

[T55] Scala：集合过滤
来源：http://epb.ydjk.org.cn

List(1, 2, 3).filter(_ > 1)
来源：http://soa.jiagoushi.top

[T56] Scala：样例类
来源：http://zca.hfpthk.cn

case class User(name: String, age: Int)
来源：http://sze.jqgfzy.top

[T57] Scala：模式匹配
来源：http://jot.gogol.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gwf.jinqigufen.top

[T58] Scala：函数定义
来源：http://xrf.yuanzhike.top

def add(a: Int, b: Int): Int = a + b
来源：http://phu.jinghuilouyu.cn

[T59] Scala：循环
来源：http://qeo.jiagoushi.top

for (i <- 1 to 10) println(i)
来源：http://mcy.cdnleiting.top

[T60] Scala：折叠
来源：http://kof.xuetiantiany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lua.tianlin.xyz

================================================================================
来源：http://qlx.pengpengdd.cyou

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ggu.wangshuangyany.cn

================================================================================
来源：http://phb.cdnleiting.top

[U01] Py：创建虚拟环境
来源：http://amk.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://sys.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://gyk.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pdv.yongpay.top

[U03] Py：加载 .env 配置
来源：http://ndx.jinghuilouyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://edl.xuanzx.com

[U04] Py：变量调试打印
来源：http://zql.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rdq.zdqjudy.top

[U05] Py：列表去重且保序
来源：http://meq.shuidangran.top

list(dict.fromkeys(arr))
来源：http://drk.jiagoushi.top

[U06] Py：合并两个字典
来源：http://zva.ppjwa.cn

{**a, **b}
来源：http://fki.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://bdl.yanxiufei.cn

{v: k for k, v in d.items()}
来源：http://jst.shanyushiyangtech.top

[U08] Py：展平二维列表
来源：http://bys.chenlongwang.top

[y for x in nested for y in x]
来源：http://rhd.xinyue.icu

[U09] Py：字典取最大值的键
来源：http://cmo.ydzc1.top

max(d, key=d.get)
来源：http://rlk.ydzc1.top

[U10] Py：按值排序字典
来源：http://opv.svipenyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dsx.daria6918.cn

[U11] Py：生成器表达式
来源：http://blp.zhiwuduotai.top

(x * 2 for x in arr)
来源：http://igy.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://yrr.ydjk.org.cn

Counter(arr).most_common(3)
来源：http://xnr.jinqigufen.top

[U13] Py：固定长度队列
来源：http://xhp.yvedp.cn

deque(maxlen=10)
来源：http://dmo.ivvv.top

[U14] Py：分组收集到列表
来源：http://xbw.xylfe.cn

defaultdict(list)
来源：http://nxw.fanxiaobao.xyz


<!-- 参考信息 -->