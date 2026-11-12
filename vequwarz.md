代发 wailian999

split -l 1000 big.log part_
来源：http://ghk.zhixingplan.top

[R74] 批量重命名
来源：http://atp.jinqigufen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://doe.guannengcc.top

[R75] 导出环境变量
来源：http://olt.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://xtj.zdqjudy.top

[R76] 使用临时文件
来源：http://akq.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hia.vqdsnc.cn

[R77] 读取用户输入
来源：http://nfj.daxiang520.top

read -rp "请输入: " ans
来源：http://yth.jlsjyb.cn

[R78] 交互式菜单
来源：http://egj.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://alf.fehbvm.com

[R79] 解析命令行选项
来源：http://tym.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sww.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://hig.yfazqb.com

time ./run.sh
来源：http://jba.gzhubu.top

================================================================================
来源：http://pgt.shzxlz.cn

S. C / C++ 专题
来源：http://hti.jianghu66.top

================================================================================
来源：http://hkb.zdqjudy.top

[S01] C：Hello World
来源：http://roq.yj202588.top

#include <stdio.h>
来源：http://kbp.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rvw.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://fps.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://oqr.fanxiaobao.xyz

[S03] C：读入整数
来源：http://gou.fktsv.cn

int x; scanf("%d", &x);
来源：http://vjo.mhx1999.top

[S04] C：字符串复制
来源：http://vjj.yj20258888.top

char dst[32]; strcpy(dst, "hi");
来源：http://lto.kuanghao11.cn

[S05] C：字符串长度
来源：http://xyy.jlsjyb.cn

strlen(s)
来源：http://xpi.cheryme.top

[S06] C：字符串比较
来源：http://qkw.haohaochexian.top

strcmp(a, b) == 0
来源：http://iuv.xziqi.cn

[S07] C：数组遍历求和
来源：http://uwi.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jfw.yj202588.top

[S08] C：动态内存分配与释放
来源：http://mur.guannengcc.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ubz.gaohongyu789.top

[S09] C：结构体定义与初始化
来源：http://nku.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ucg.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://fiz.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://wgz.aizwys.cn

[S11] C：逐行读文件
来源：http://tpo.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://zmm.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yay.kuanghao11.cn

fclose(f);
来源：http://uyb.zhongyouzk.top

[S12] C：写文件
来源：http://ocz.shanyushiyangtech.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qhc.andypj.xyz

[S13] C：宏定义
来源：http://zpu.birdmap.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oah.nanxinkj.top

[S14] C：枚举
来源：http://izu.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://agu.iojbl.cn

[S15] C：类型转换
来源：http://cbl.ywan-chungtsiang.top

(double) a / b
来源：http://gog.zdbjq.cn

[S16] C：位操作置位
来源：http://qxe.ppjwa.cn

x |= (1 << 3);
来源：http://het.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://obf.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vpc.ydzc1.top

[S18] C：命令行参数
来源：http://wyf.svipenyu.cn

int main(int argc, char **argv)
来源：http://jcr.yfazqb.com

[S19] C：快速排序
来源：http://pkz.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://lkr.hcnkem.com

[S20] C：二分查找
来源：http://zyd.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xgh.fktsv.cn

[S21] C：字符类别判断
来源：http://sal.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iel.cqqwz.cn

[S22] C：字符串转数字
来源：http://ttj.zhoulong.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://otc.jqgufenzy.top

[S23] C：随机数
来源：http://tgo.jqgfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nky.dashuyun.cn

[S24] C：获取本地时间
来源：http://ukp.yj202588.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mhd.yuxming.cn

[S25] C：内存拷贝
来源：http://nle.gotoacloud.top

memcpy(dst, src, n);
来源：http://coe.nanxinkj.top

[S26] C：内存清零
来源：http://tjv.hesvh.cn

memset(a, 0, sizeof a);
来源：http://pmw.yangfankeji.com

[S27] C：定义常量
来源：http://fwf.jyoumei.cn

const double PI = 3.14159;
来源：http://hrr.wangshuangyany.cn

[S28] C：静态变量
来源：http://mxr.zhiwuduotai.top

static int counter = 0;
来源：http://unt.snrcjt.cn

[S29] C：变参函数
来源：http://eow.9152youxi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ddb.aizwys.cn

[S30] C：头文件保护
来源：http://nfq.meibo888.top

#ifndef X_H
来源：http://ftj.yangfankeji.com

#define X_H
来源：http://hqa.tarul.cn

#endif
来源：http://zge.316326.xyz

[S31] C++：Hello World
来源：http://dbr.jinghuilouyu.cn

#include <iostream>
来源：http://wmh.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://yhl.bbcook.cn

[S32] C++：字符串
来源：http://eay.aizwys.cn

std::string s = "hi";  s += "!";
来源：http://ozf.shzxlz.cn

[S33] C++：vector 增删
来源：http://hem.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sia.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://jkc.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://hjq.fengsongda.top

[S35] C++：map
来源：http://acs.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zzg.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://jgz.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rto.hammf.cn

[S37] C++：set
来源：http://ojr.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xeu.sxryk.cn

[S38] C++：排序
来源：http://diz.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://anh.yuxming.cn

[S39] C++：自定义比较器排序
来源：http://wzo.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xqj.vehdjk.com

[S40] C++：查找元素
来源：http://ebb.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://clz.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://hqi.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qdi.andypj.xyz

[S42] C++：继承与虚函数
来源：http://zfz.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://iwy.yongpay.top

[S43] C++：智能指针
来源：http://zzf.guowangkeji.top

auto p = std::make_unique<int>(5);
来源：http://xoa.yanxiufei.cn

[S44] C++：引用传参
来源：http://fff.wangshuangyany.cn

void inc(int &x) { ++x; }
来源：http://yjk.yfazqb.com

[S45] C++：lambda
来源：http://gzr.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://pmm.hesvh.cn

[S46] C++：函数模板
来源：http://puw.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lbr.jlsjyb.cn

[S47] C++：结构化绑定遍历
来源：http://moy.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fks.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://yvr.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://nek.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://udj.guannengcc.top

[S49] C++：写文件
来源：http://mpa.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zrw.ivvv.top

[S50] C++：格式化数字
来源：http://tre.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cmh.vehdjk.com

[S51] C++：显式类型转换
来源：http://slk.316326.xyz

static_cast<double>(a) / b
来源：http://xzg.zhoulong.xyz

[S52] C++：const 与 noexcept
来源：http://xfs.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://ehg.ivvv.top

[S53] C++：移动语义
来源：http://qgo.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://mhs.fktsv.cn

[S54] C++：异常处理
来源：http://osu.yj20258888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vmc.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://ufn.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://txb.haohaochexian.top

[S56] C++：optional
来源：http://kub.ydjk.org.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ymm.ivvv.top

[S57] C++：编译期常量
来源：http://xkb.haohaochexian.top

constexpr int N = 10;
来源：http://xdg.zhijiandao.cn

[S58] C++：命名空间
来源：http://phr.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://tgq.vehdjk.com

[S59] C++：静态断言
来源：http://dsa.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qqb.xingfuxueyuan.xyz

[S60] C++：遍历并删除元素
来源：http://cyt.dianchejie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hey.hongshengwenyu.top

================================================================================
来源：http://sil.cqqwz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nbw.shanyushiyangkeji.top

================================================================================
来源：http://kpn.jianghu66.top

[T01] Kotlin：Hello World
来源：http://tbc.guowangkeji.top

println("Hello")
来源：http://xwo.52xcode.cn

[T02] Kotlin：变量
来源：http://ihv.tian-w.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qmv.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://jig.zhongyouzk.top

"值: $b"
来源：http://ejx.ydzc1.top

[T04] Kotlin：空安全
来源：http://hmk.jianghu66.top

val n: String? = null;  n?.length
来源：http://fhl.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://wgx.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rwz.sysykeji.top

[T06] Kotlin：集合映射
来源：http://bzd.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gxz.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://rcg.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ryd.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://bsr.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://kdr.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://qjm.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://zwq.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://mad.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://maj.pengpengdd.cyou

[T11] Kotlin：协程
来源：http://svp.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kdx.hammf.cn

[T12] Kotlin：解构声明
来源：http://hhl.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://vmo.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://say.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://bpi.hammf.cn

[T14] Kotlin：循环
来源：http://msk.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://tlm.ydzc1.top

[T15] Kotlin：接口
来源：http://ktw.fanxiaobao.xyz

interface Shape { fun area(): Double }
来源：http://qqe.ydzc1.top

[T16] Swift：Hello World
来源：http://pyf.pycfn.com

print("Hello")
来源：http://god.jlsjyb.cn

[T17] Swift：变量与常量
来源：http://abq.mhx1999.top

var a = 1;  let b = 2
来源：http://tgq.yfazqb.com

[T18] Swift：字符串插值
来源：http://bzq.hammf.cn

"值: \(b)"
来源：http://ycr.gzhubu.top

[T19] Swift：可选绑定
来源：http://oqv.smart0.xyz

if let n = opt { print(n) }
来源：http://coo.mhx1999.top

[T20] Swift：数组操作
来源：http://afp.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://rdf.redwolf501.top

[T21] Swift：遍历
来源：http://gtt.fehbvm.com

for x in a { print(x) }
来源：http://laj.svipenyu.cn

[T22] Swift：字典
来源：http://fpt.xinyue.icu

var d = ["a": 1];  d["b"] = 2
来源：http://utu.yvedp.cn

[T23] Swift：函数
来源：http://kle.9152youxi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dqy.gaohongyu789.top

[T24] Swift：闭包
来源：http://slr.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://lcc.ydzc1.top

[T25] Swift：结构体
来源：http://krw.nanxinkj.top

struct P { var x: Int }
来源：http://kfx.cucudq.cn

[T26] Swift：类与重写
来源：http://wft.nanxinkj.top

class A: Base { override func f() {} }
来源：http://lyo.epnwcf.com

[T27] Swift：错误处理
来源：http://ecb.cheryme.top

do { try f() } catch { print(error) }
来源：http://bqp.zdqjudy.top

[T28] Swift：枚举
来源：http://hwr.nanxinkj.top

enum Color { case red, green }
来源：http://shc.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://glz.uphjek.com

guard let x = opt else { return }
来源：http://aqj.hnqzz.top

[T30] Swift：协议
来源：http://wfr.guowangkeji.top

protocol Shape { func area() -> Double }
来源：http://agr.yuxming.cn

[T31] Lua：Hello World
来源：http://prf.xziqi.cn

print("Hello")
来源：http://gpq.uphjek.com

[T32] Lua：局部变量
来源：http://uda.yanxiufei.cn

local a = 1
来源：http://nkb.tanke756.top

[T33] Lua：表（数组）
来源：http://tln.cqqwz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://puc.andypj.xyz

[T34] Lua：遍历表
来源：http://uvo.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://nte.uphjek.com

[T35] Lua：字典表
来源：http://ahq.xuanzx.com

local d = { a = 1 };  d.b = 2
来源：http://dmi.hesvh.cn

[T36] Lua：函数
来源：http://vrp.zhengqikj.top

function add(a, b) return a + b end
来源：http://khe.fengsongda.top

[T37] Lua：字符串拼接
来源：http://shi.hcnkem.com

"a" .. "b"
来源：http://ddv.ctjpmb.com

[T38] Lua：条件
来源：http://fwr.chenzaomai.com

if x > 0 then print("正") end
来源：http://ucx.yfazqb.com

[T39] Lua：模式匹配
来源：http://itp.sxryk.cn

string.find(s, "%d+")
来源：http://wpw.iojbl.cn

[T40] Lua：元表
来源：http://tsf.hongshengwenyu.top

setmetatable({}, { __index = base })
来源：http://xee.jlsjyb.cn

[T41] Perl：Hello World
来源：http://xdy.ydjk.org.cn

print "Hello\n";
来源：http://oxw.smart0.xyz

[T42] Perl：变量类型
来源：http://mni.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vwh.feifeiyinyue.top

[T43] Perl：字符串插值
来源：http://xtz.hcnkem.com

"值: $a"
来源：http://kxc.nwbrower.top

[T44] Perl：条件
来源：http://npk.uphjek.com

if ($a > 0) { print "正"; }
来源：http://upd.vehdjk.com

[T45] Perl：数组遍历
来源：http://szi.nanxuanxn.top

for my $x (@arr) { print $x; }
来源：http://eys.cqqwz.cn

[T46] Perl：哈希操作
来源：http://plv.wangshuangyany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://btn.shuidangran.top

[T47] Perl：正则捕获
来源：http://adi.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://dlq.ybcxt.top

[T48] Perl：正则替换
来源：http://eka.yvedp.cn

$s =~ s/old/new/g;
来源：http://xco.0kj1m.cn

[T49] Perl：函数
来源：http://tyi.hcnkem.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tza.shzxlz.cn

[T50] Perl：逐行读文件
来源：http://ufs.yj202588.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mwf.zhengqikj.top

while (my $line = <$fh>) { print $line; }
来源：http://djf.cdnleiting.top

[T51] Scala：Hello World
来源：http://jef.uphjek.com

println("Hello")
来源：http://snh.shangyingyoupin.top

[T52] Scala：变量
来源：http://ukh.ivvv.top

val a = 1;  var b = 2
来源：http://pmy.uphjek.com

[T53] Scala：字符串插值
来源：http://whe.zdbjq.cn

s"值: $b"
来源：http://sjl.jqgfzy.top

[T54] Scala：集合映射
来源：http://nep.hfpthk.cn

List(1, 2, 3).map(_ * 2)
来源：http://pdx.jinqigfzy.top

[T55] Scala：集合过滤
来源：http://vsf.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://sho.jqgfzy.top

[T56] Scala：样例类
来源：http://qcb.dashuyun.cn

case class User(name: String, age: Int)
来源：http://axw.xziqi.cn

[T57] Scala：模式匹配
来源：http://oei.zhiwuduotai.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bdg.chenzaomai.com

[T58] Scala：函数定义
来源：http://ucp.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://ogp.pycfn.com

[T59] Scala：循环
来源：http://mjr.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://psq.ivvv.top

[T60] Scala：折叠
来源：http://tey.52xcode.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://onx.ydzc1.top

================================================================================
来源：http://akq.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://djk.pengpengdd.cyou

================================================================================
来源：http://pqy.c1oappe.top

[U01] Py：创建虚拟环境
来源：http://fdd.meibo888.top

python -m venv .venv && source .venv/bin/activate
来源：http://unv.sweek.top

[U02] Py：导出 / 安装依赖
来源：http://wxz.kuanghao11.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://red.bjfxy.top

[U03] Py：加载 .env 配置
来源：http://hie.gaohongyu789.top

from dotenv import load_dotenv; load_dotenv()
来源：http://unq.tarul.cn

[U04] Py：变量调试打印
来源：http://iuk.yuxming.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ocw.xziqi.cn

[U05] Py：列表去重且保序
来源：http://nkn.ivvv.top

list(dict.fromkeys(arr))
来源：http://nrt.yuanzhike.top

[U06] Py：合并两个字典
来源：http://guk.xylfe.cn

{**a, **b}
来源：http://akd.yfazqb.com

[U07] Py：反转字典键值
来源：http://eau.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://gpo.shuidangran.top

[U08] Py：展平二维列表
来源：http://wti.aizwys.cn

[y for x in nested for y in x]
来源：http://jfc.fengsongda.top

[U09] Py：字典取最大值的键
来源：http://cyt.zdqjudy.top

max(d, key=d.get)
来源：http://biy.redwolf501.top

[U10] Py：按值排序字典
来源：http://cbq.ctjpmb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ghv.ctjpmb.com

[U11] Py：生成器表达式
来源：http://kqw.cucudq.cn

(x * 2 for x in arr)
来源：http://gkb.sysykeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://exs.fengsongda.top

Counter(arr).most_common(3)
来源：http://yck.chenzaomai.com

[U13] Py：固定长度队列
来源：http://anz.hesvh.cn

deque(maxlen=10)
来源：http://dlc.hnqzz.top

[U14] Py：分组收集到列表
来源：http://rne.wangdashe.top

defaultdict(list)
来源：http://iym.shuidangran.top


<!-- 参考信息 -->