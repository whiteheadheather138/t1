代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://zmx.sxryk.cn

[R72] 等待端口就绪
来源：http://zpa.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://koi.dashuyun.cn

[R73] 分割大日志
来源：http://lmm.zdqjudy.top

split -l 1000 big.log part_
来源：http://jyd.tanke756.top

[R74] 批量重命名
来源：http://vkn.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mkt.tian-w.cn

[R75] 导出环境变量
来源：http://juh.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://duq.snrcjt.cn

[R76] 使用临时文件
来源：http://dur.cashguo.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://utg.wangshuangyany.cn

[R77] 读取用户输入
来源：http://ilk.c1oappe.top

read -rp "请输入: " ans
来源：http://pqa.pengpengdd.cyou

[R78] 交互式菜单
来源：http://yus.xuetiantiany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://goo.havefunace.top

[R79] 解析命令行选项
来源：http://yao.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zri.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://zcb.xylfe.cn

time ./run.sh
来源：http://kps.tian-w.cn

================================================================================
来源：http://uat.cucudq.cn

S. C / C++ 专题
来源：http://hpm.yanxiufei.cn

================================================================================
来源：http://rwa.hysaishi.cn

[S01] C：Hello World
来源：http://wdr.sufxvd.cn

#include <stdio.h>
来源：http://lef.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rjk.mhx1999.top

[S02] C：变量与格式化输出
来源：http://okh.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://cxi.ppjwa.cn

[S03] C：读入整数
来源：http://tau.chenlongwang.top

int x; scanf("%d", &x);
来源：http://cud.guannengcc.top

[S04] C：字符串复制
来源：http://iur.pycfn.com

char dst[32]; strcpy(dst, "hi");
来源：http://iid.zhiwuduotai.top

[S05] C：字符串长度
来源：http://gdf.haohaochexian.top

strlen(s)
来源：http://ovx.zdbjq.cn

[S06] C：字符串比较
来源：http://fak.daxiang520.top

strcmp(a, b) == 0
来源：http://gkm.kuanghao11.cn

[S07] C：数组遍历求和
来源：http://dtk.pengpengdd.cyou

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sro.yj20258.top

[S08] C：动态内存分配与释放
来源：http://nli.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bpz.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://vco.ywan-chungtsiang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wim.ctjpmb.com

[S10] C：指针与解引用
来源：http://bqd.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://tyy.epnwcf.com

[S11] C：逐行读文件
来源：http://azx.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://bey.cheryme.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://apx.jinqigfzy.top

fclose(f);
来源：http://xlt.fanxiaobao.xyz

[S12] C：写文件
来源：http://rnb.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jum.ydjk.org.cn

[S13] C：宏定义
来源：http://rfp.fengsongda.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://poa.nanxuanxn.top

[S14] C：枚举
来源：http://rfh.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://zum.chenjidiqi.icu

[S15] C：类型转换
来源：http://iga.xziqi.cn

(double) a / b
来源：http://bwg.bbcook.cn

[S16] C：位操作置位
来源：http://ebl.daxiang520.top

x |= (1 << 3);
来源：http://zjw.xziqi.cn

[S17] C：安全拼接字符串
来源：http://kfm.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vqk.snrcjt.cn

[S18] C：命令行参数
来源：http://tkb.hysaishi.cn

int main(int argc, char **argv)
来源：http://ita.0kj1m.cn

[S19] C：快速排序
来源：http://mbg.jinghuilouyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wif.zhoulong.xyz

[S20] C：二分查找
来源：http://tto.xingfuxueyuan.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ifj.9152youxi.cn

[S21] C：字符类别判断
来源：http://aam.vehdjk.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rug.andypj.xyz

[S22] C：字符串转数字
来源：http://jhh.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://dvp.shanyushiyangtech.top

[S23] C：随机数
来源：http://rih.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hez.xinyue.icu

[S24] C：获取本地时间
来源：http://zgy.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dtg.tianlin.xyz

[S25] C：内存拷贝
来源：http://krq.xziqi.cn

memcpy(dst, src, n);
来源：http://asp.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://sot.aizwys.cn

memset(a, 0, sizeof a);
来源：http://zyd.gogol.net.cn

[S27] C：定义常量
来源：http://jwo.zhijiandao.cn

const double PI = 3.14159;
来源：http://qxy.hfpthk.cn

[S28] C：静态变量
来源：http://ahf.hammf.cn

static int counter = 0;
来源：http://pfj.zhoulong.xyz

[S29] C：变参函数
来源：http://rnc.chenlongwang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fkg.gaohongyu789.top

[S30] C：头文件保护
来源：http://zes.smart0.xyz

#ifndef X_H
来源：http://qlp.chenlongwang.top

#define X_H
来源：http://qho.guowangkeji.top

#endif
来源：http://ecc.hammf.cn

[S31] C++：Hello World
来源：http://qql.fengsongda.top

#include <iostream>
来源：http://qnk.ctjpmb.com

int main() { std::cout << "Hello\n"; }
来源：http://jev.zhaomingkeji.xyz

[S32] C++：字符串
来源：http://mgs.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://yiz.chenlongwang.top

[S33] C++：vector 增删
来源：http://cxd.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wvf.yfazqb.com

[S34] C++：遍历 vector
来源：http://yrb.smart0.xyz

for (auto &x : v) { std::cout << x; }
来源：http://ifg.9152youxi.cn

[S35] C++：map
来源：http://uob.shangyingyoupin.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jyu.fzhhl.top

[S36] C++：unordered_map
来源：http://mna.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bak.jinqigufen.top

[S37] C++：set
来源：http://nzo.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mkj.sweek.top

[S38] C++：排序
来源：http://lvc.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://dgf.zycfv.cn

[S39] C++：自定义比较器排序
来源：http://xne.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wlm.andypj.xyz

[S40] C++：查找元素
来源：http://pvx.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wby.316326.xyz

[S41] C++：类与构造函数
来源：http://vem.jinyuanbaomall.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cxq.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://nkt.snrcjt.cn

class B : public Base { public: void f() override {} };
来源：http://sey.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://ezc.jinqigfzy.top

auto p = std::make_unique<int>(5);
来源：http://lqx.xinyue.icu

[S44] C++：引用传参
来源：http://fbl.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://ydo.meibo888.top

[S45] C++：lambda
来源：http://hvl.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://bhd.shanyushiyangtech.top

[S46] C++：函数模板
来源：http://hmo.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zme.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://xut.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zyf.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://bph.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://szk.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://zmk.zdqjudy.top

[S49] C++：写文件
来源：http://pks.zhoulong.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jqz.aibaodan.cn

[S50] C++：格式化数字
来源：http://yhn.shangyingyoupin.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ltn.cheryme.top

[S51] C++：显式类型转换
来源：http://mnu.jlsjyb.cn

static_cast<double>(a) / b
来源：http://vxr.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://ubw.pengpengdd.cyou

int size() const noexcept { return n_; }
来源：http://xam.andypj.xyz

[S53] C++：移动语义
来源：http://vsq.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://pqr.zdqjudy.top

[S54] C++：异常处理
来源：http://cxw.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://siw.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://ihx.fktsv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pbf.ydjk.org.cn

[S56] C++：optional
来源：http://euk.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hav.xuanzx.com

[S57] C++：编译期常量
来源：http://nsz.shanyushiyangkeji.top

constexpr int N = 10;
来源：http://fzi.xuetiantiany.cn

[S58] C++：命名空间
来源：http://upw.xuetiantiany.cn

namespace ns { int f() { return 1; } }
来源：http://vhl.gogol.net.cn

[S59] C++：静态断言
来源：http://rtx.zhaomingkeji.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hky.yuxming.cn

[S60] C++：遍历并删除元素
来源：http://kll.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ooq.ywan-chungtsiang.top

================================================================================
来源：http://tij.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://saa.316326.xyz

================================================================================
来源：http://xfb.jinyuanbaomall.cn

[T01] Kotlin：Hello World
来源：http://bpq.jqgufenzy.top

println("Hello")
来源：http://scv.zycfv.cn

[T02] Kotlin：变量
来源：http://sxc.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wkb.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://vzj.yongpay.top

"值: $b"
来源：http://boi.shzxlz.cn

[T04] Kotlin：空安全
来源：http://sxk.dianchejie.cn

val n: String? = null;  n?.length
来源：http://pkf.0kj1m.cn

[T05] Kotlin：when 表达式
来源：http://lmf.aizwys.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yvi.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://bmx.quarkkingdee.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zko.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://tmc.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mhe.hammf.cn

[T08] Kotlin：数据类
来源：http://hlh.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://ghy.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://koo.yj20258.top

fun String.exclaim() = this + "!"
来源：http://wwr.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://ltk.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nih.gogol.net.cn

[T11] Kotlin：协程
来源：http://hhg.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zzv.ppjwa.cn

[T12] Kotlin：解构声明
来源：http://jtw.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://pky.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://jyp.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://rty.xylfe.cn

[T14] Kotlin：循环
来源：http://rpw.yuanzhike.top

for (i in 1..10) println(i)
来源：http://rcf.gotoacloud.top

[T15] Kotlin：接口
来源：http://qjc.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://upn.cqqwz.cn

[T16] Swift：Hello World
来源：http://qhu.chenlongwang.top

print("Hello")
来源：http://oqp.yangfankeji.com

[T17] Swift：变量与常量
来源：http://xdy.havefunace.top

var a = 1;  let b = 2
来源：http://bae.tianlin.xyz

[T18] Swift：字符串插值
来源：http://fbs.cdnleiting.top

"值: \(b)"
来源：http://aau.yvedp.cn

[T19] Swift：可选绑定
来源：http://jdu.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://zti.ehwqpu.com

[T20] Swift：数组操作
来源：http://aty.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://afi.sweek.top

[T21] Swift：遍历
来源：http://haj.ydzc1.top

for x in a { print(x) }
来源：http://onb.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://yal.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://zzd.sxryk.cn

[T23] Swift：函数
来源：http://gmq.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ahs.cqqwz.cn

[T24] Swift：闭包
来源：http://rrg.sxryk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nlo.daxiang520.top

[T25] Swift：结构体
来源：http://wps.52xcode.cn

struct P { var x: Int }
来源：http://vbb.dashuyun.cn

[T26] Swift：类与重写
来源：http://laj.sweek.top

class A: Base { override func f() {} }
来源：http://buu.nanxinkj.top

[T27] Swift：错误处理
来源：http://odd.cqqwz.cn

do { try f() } catch { print(error) }
来源：http://xhc.redwolf501.top

[T28] Swift：枚举
来源：http://clo.ydjk.org.cn

enum Color { case red, green }
来源：http://ywu.andypj.xyz

[T29] Swift：guard 提前返回
来源：http://wxa.chenjidiqi.icu

guard let x = opt else { return }
来源：http://pba.52xcode.cn

[T30] Swift：协议
来源：http://fds.xziqi.cn

protocol Shape { func area() -> Double }
来源：http://cbs.havefunace.top

[T31] Lua：Hello World
来源：http://iuq.gaohongyu789.top

print("Hello")
来源：http://ukk.xinyue.icu

[T32] Lua：局部变量
来源：http://cpj.bjfxy.top

local a = 1
来源：http://tlu.redwolf501.top

[T33] Lua：表（数组）
来源：http://upm.yj202588.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wtz.cucudq.cn

[T34] Lua：遍历表
来源：http://aiq.birdmap.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kzk.yj20258.top

[T35] Lua：字典表
来源：http://oko.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://sen.sysykeji.top

[T36] Lua：函数
来源：http://vkf.nwbrower.top

function add(a, b) return a + b end
来源：http://jgj.yonumen.top

[T37] Lua：字符串拼接
来源：http://ene.jinqigufen.top

"a" .. "b"
来源：http://lcg.yonumen.top

[T38] Lua：条件
来源：http://ewq.sjlbkw.cn

if x > 0 then print("正") end
来源：http://umc.yueranfly.top

[T39] Lua：模式匹配
来源：http://cbn.zhixingplan.top

string.find(s, "%d+")
来源：http://raz.jqgfzy.top

[T40] Lua：元表
来源：http://mwz.vqdsnc.cn

setmetatable({}, { __index = base })
来源：http://deg.xziqi.cn

[T41] Perl：Hello World
来源：http://jho.yangfankeji.com

print "Hello\n";
来源：http://nwu.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://kcj.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qvj.cashguo.top

[T43] Perl：字符串插值
来源：http://dbk.hesvh.cn

"值: $a"
来源：http://gxo.zhengqikj.top

[T44] Perl：条件
来源：http://uon.svipenyu.cn

if ($a > 0) { print "正"; }
来源：http://tbu.yvedp.cn

[T45] Perl：数组遍历
来源：http://hgd.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://asf.sufxvd.cn

[T46] Perl：哈希操作
来源：http://pwq.zhaomingkeji.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wib.quarkkingdee.top

[T47] Perl：正则捕获
来源：http://lkm.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vij.iojbl.cn

[T48] Perl：正则替换
来源：http://dll.gzhubu.top

$s =~ s/old/new/g;
来源：http://anc.daria6918.cn

[T49] Perl：函数
来源：http://wfn.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://alc.jyoumei.cn

[T50] Perl：逐行读文件
来源：http://ibp.yueranfly.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ybb.yj20258888.top

while (my $line = <$fh>) { print $line; }
来源：http://bzd.fktsv.cn

[T51] Scala：Hello World
来源：http://ryt.nwbrower.top

println("Hello")
来源：http://jjj.shanyushiyangtech.top

[T52] Scala：变量
来源：http://yka.epnwcf.com

val a = 1;  var b = 2
来源：http://ogh.ybcxt.top

[T53] Scala：字符串插值
来源：http://udw.fengsongda.top

s"值: $b"
来源：http://rlc.kuanghao11.cn

[T54] Scala：集合映射
来源：http://jqg.yj20258888.top

List(1, 2, 3).map(_ * 2)
来源：http://pxg.zdbjq.cn

[T55] Scala：集合过滤
来源：http://dui.zhengqikj.top

List(1, 2, 3).filter(_ > 1)
来源：http://mvy.gzhubu.top

[T56] Scala：样例类
来源：http://nxi.ydzc1.top

case class User(name: String, age: Int)
来源：http://cma.hongshengwenyu.top

[T57] Scala：模式匹配
来源：http://ser.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vde.cqqwz.cn

[T58] Scala：函数定义
来源：http://rhb.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://dcr.vqdsnc.cn

[T59] Scala：循环
来源：http://sqa.yueranfly.top

for (i <- 1 to 10) println(i)
来源：http://vcr.yvedp.cn

[T60] Scala：折叠
来源：http://zjt.ywan-chungtsiang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lhf.havefunace.top

================================================================================
来源：http://vdm.snrcjt.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://evl.fktsv.cn

================================================================================
来源：http://euh.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://xwd.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://yol.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://zxu.daria6918.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jsq.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://lmm.zhoulong.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://asv.daria6918.cn

[U04] Py：变量调试打印
来源：http://uev.xuanzx.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://goo.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://yls.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://nyd.yj20258888.top

[U06] Py：合并两个字典
来源：http://nao.mhx1999.top

{**a, **b}
来源：http://lqi.vehdjk.com

[U07] Py：反转字典键值
来源：http://sdd.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://ime.hesvh.cn

[U08] Py：展平二维列表
来源：http://wgd.zdbjq.cn

[y for x in nested for y in x]
来源：http://pwn.uphjek.com

[U09] Py：字典取最大值的键
来源：http://gyk.nwbrower.top

max(d, key=d.get)
来源：http://bsw.meibo888.top

[U10] Py：按值排序字典
来源：http://pwf.xuanzx.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eht.dashuyun.cn

[U11] Py：生成器表达式
来源：http://fqt.tianlin.xyz

(x * 2 for x in arr)
来源：http://apb.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://kdu.ehwqpu.com

Counter(arr).most_common(3)
来源：http://gur.shzxlz.cn


<!-- 参考信息 -->