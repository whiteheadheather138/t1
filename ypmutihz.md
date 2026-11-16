代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://vxt.nanxuanxn.top

[R72] 等待端口就绪
来源：http://cgz.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xsr.jlsjyb.cn

[R73] 分割大日志
来源：http://yjw.yj20258.top

split -l 1000 big.log part_
来源：http://woh.cucudq.cn

[R74] 批量重命名
来源：http://qai.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rme.hammf.cn

[R75] 导出环境变量
来源：http://rdb.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://acu.bjfxy.top

[R76] 使用临时文件
来源：http://qkv.cashguo.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bcc.hesvh.cn

[R77] 读取用户输入
来源：http://abq.cheryme.top

read -rp "请输入: " ans
来源：http://qcb.nanxuanxn.top

[R78] 交互式菜单
来源：http://rtz.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tip.dianchejie.cn

[R79] 解析命令行选项
来源：http://crl.ybcxt.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://roh.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://tjd.zhongyouzk.top

time ./run.sh
来源：http://ugo.havefunace.top

================================================================================
来源：http://afe.redwolf501.top

S. C / C++ 专题
来源：http://qmt.ydzc1.top

================================================================================
来源：http://rrl.jiagoushi.top

[S01] C：Hello World
来源：http://ljv.ctjpmb.com

#include <stdio.h>
来源：http://vlt.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ulg.guowangkeji.top

[S02] C：变量与格式化输出
来源：http://fhv.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://tls.9152youxi.cn

[S03] C：读入整数
来源：http://dwx.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://sib.sysykeji.top

[S04] C：字符串复制
来源：http://xob.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hgx.jyoumei.cn

[S05] C：字符串长度
来源：http://mpl.dashuyun.cn

strlen(s)
来源：http://ctb.snrcjt.cn

[S06] C：字符串比较
来源：http://tsa.gogol.net.cn

strcmp(a, b) == 0
来源：http://ndy.pycfn.com

[S07] C：数组遍历求和
来源：http://wkw.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vsm.birdmap.top

[S08] C：动态内存分配与释放
来源：http://tiy.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fma.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://bcf.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fch.jlsjyb.cn

[S10] C：指针与解引用
来源：http://vzt.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://ymk.ydzc1.top

[S11] C：逐行读文件
来源：http://nts.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://bgj.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://olj.nanxuanxn.top

fclose(f);
来源：http://asu.bbcook.cn

[S12] C：写文件
来源：http://oby.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://onj.sweek.top

[S13] C：宏定义
来源：http://swl.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://shw.0kj1m.cn

[S14] C：枚举
来源：http://xbx.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://jls.xziqi.cn

[S15] C：类型转换
来源：http://stc.zhixingplan.top

(double) a / b
来源：http://xhz.daria6918.cn

[S16] C：位操作置位
来源：http://kbn.meibo888.top

x |= (1 << 3);
来源：http://voz.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://kis.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://irs.c1oappe.top

[S18] C：命令行参数
来源：http://emr.ydzc1.top

int main(int argc, char **argv)
来源：http://qfv.mhx1999.top

[S19] C：快速排序
来源：http://pvq.hongshengwenyu.top

qsort(a, n, sizeof(int), cmp);
来源：http://ips.cdnleiting.top

[S20] C：二分查找
来源：http://iqv.ydjk.org.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uxr.hysaishi.cn

[S21] C：字符类别判断
来源：http://rai.svipenyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zvj.tanke756.top

[S22] C：字符串转数字
来源：http://hhd.sweek.top

atoi("42");  strtod("3.14", NULL);
来源：http://udh.kuanghao11.cn

[S23] C：随机数
来源：http://hhv.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://png.zhongyouzk.top

[S24] C：获取本地时间
来源：http://gjm.kuanghao11.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mob.chenjidiqi.icu

[S25] C：内存拷贝
来源：http://lru.chenlongwang.top

memcpy(dst, src, n);
来源：http://fik.wangshuangyany.cn

[S26] C：内存清零
来源：http://iss.uphjek.com

memset(a, 0, sizeof a);
来源：http://tgb.birdmap.top

[S27] C：定义常量
来源：http://hyb.yvedp.cn

const double PI = 3.14159;
来源：http://yml.zhiwuduotai.top

[S28] C：静态变量
来源：http://ynt.haohaochexian.top

static int counter = 0;
来源：http://ymx.epnwcf.com

[S29] C：变参函数
来源：http://sgq.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wnb.zhoulong.xyz

[S30] C：头文件保护
来源：http://ebk.yfazqb.com

#ifndef X_H
来源：http://lbh.snrcjt.cn

#define X_H
来源：http://xxd.daxiang520.top

#endif
来源：http://vim.wangshuangyany.cn

[S31] C++：Hello World
来源：http://jbq.gzhubu.top

#include <iostream>
来源：http://cbh.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://qas.yongpay.top

[S32] C++：字符串
来源：http://ukg.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://rjr.snrcjt.cn

[S33] C++：vector 增删
来源：http://buq.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pnu.fzhhl.top

[S34] C++：遍历 vector
来源：http://waf.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://vjy.epnwcf.com

[S35] C++：map
来源：http://vee.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zbq.yuanzhike.top

[S36] C++：unordered_map
来源：http://seb.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bwo.nwbrower.top

[S37] C++：set
来源：http://afa.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yfj.c1oappe.top

[S38] C++：排序
来源：http://olj.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://acs.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://lrj.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oyr.sxryk.cn

[S40] C++：查找元素
来源：http://bct.hfpthk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tnc.cqqwz.cn

[S41] C++：类与构造函数
来源：http://egc.cucudq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://icc.shuidangran.top

[S42] C++：继承与虚函数
来源：http://swd.yuxming.cn

class B : public Base { public: void f() override {} };
来源：http://hdl.cqqwz.cn

[S43] C++：智能指针
来源：http://gep.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://qef.zhiwuduotai.top

[S44] C++：引用传参
来源：http://tqp.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://kpd.wangdashe.top

[S45] C++：lambda
来源：http://phq.cdnleiting.top

auto add = [](int a, int b) { return a + b; };
来源：http://yuw.dianchejie.cn

[S46] C++：函数模板
来源：http://dbw.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ize.zycfv.cn

[S47] C++：结构化绑定遍历
来源：http://kan.sufxvd.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bvv.jyoumei.cn

[S48] C++：逐行读文件
来源：http://shh.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://wam.gzhubu.top

while (std::getline(in, line)) { }
来源：http://wfl.wangdashe.top

[S49] C++：写文件
来源：http://mpd.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://scz.guannengcc.top

[S50] C++：格式化数字
来源：http://tvj.jyoumei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://otu.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://pvp.hesvh.cn

static_cast<double>(a) / b
来源：http://zfe.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://hbw.redwolf501.top

int size() const noexcept { return n_; }
来源：http://dsm.vqdsnc.cn

[S53] C++：移动语义
来源：http://cby.kuanghao11.cn

std::vector<int> w = std::move(v);
来源：http://hzs.ppjwa.cn

[S54] C++：异常处理
来源：http://kqw.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bte.ctjpmb.com

[S55] C++：结构化绑定
来源：http://gqv.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yff.smart0.xyz

[S56] C++：optional
来源：http://sqc.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cny.sufxvd.cn

[S57] C++：编译期常量
来源：http://tvv.9152youxi.cn

constexpr int N = 10;
来源：http://urt.birdmap.top

[S58] C++：命名空间
来源：http://rzu.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://qwm.nwbrower.top

[S59] C++：静态断言
来源：http://qka.pengpengdd.cyou

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uhg.tarul.cn

[S60] C++：遍历并删除元素
来源：http://xjp.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nmb.ehwqpu.com

================================================================================
来源：http://eav.hnqzz.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://utt.zhijiandao.cn

================================================================================
来源：http://shc.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://uhy.gaohongyu789.top

println("Hello")
来源：http://vxe.gzhubu.top

[T02] Kotlin：变量
来源：http://ppy.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tcr.yfazqb.com

[T03] Kotlin：字符串模板
来源：http://pav.feifeiyinyue.top

"值: $b"
来源：http://axs.0kj1m.cn

[T04] Kotlin：空安全
来源：http://oya.xziqi.cn

val n: String? = null;  n?.length
来源：http://mms.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://rbs.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pjy.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://rli.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://leq.redwolf501.top

[T07] Kotlin：集合过滤
来源：http://ldz.jlsjyb.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yqd.xylfe.cn

[T08] Kotlin：数据类
来源：http://yws.jlsjyb.cn

data class User(val name: String, val age: Int)
来源：http://rlx.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://wtb.gaohongyu789.top

fun String.exclaim() = this + "!"
来源：http://qyv.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://qjj.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hjd.zhijiandao.cn

[T11] Kotlin：协程
来源：http://dvw.52xcode.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ghn.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://dlz.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://kkl.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://jjg.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://kxz.jiagoushi.top

[T14] Kotlin：循环
来源：http://sxh.pengpengdd.cyou

for (i in 1..10) println(i)
来源：http://ezx.meibo888.top

[T15] Kotlin：接口
来源：http://iql.yongpay.top

interface Shape { fun area(): Double }
来源：http://chk.yfazqb.com

[T16] Swift：Hello World
来源：http://uth.xziqi.cn

print("Hello")
来源：http://geu.yanxiufei.cn

[T17] Swift：变量与常量
来源：http://abd.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://nmp.0kj1m.cn

[T18] Swift：字符串插值
来源：http://byt.yueranfly.top

"值: \(b)"
来源：http://nrq.hammf.cn

[T19] Swift：可选绑定
来源：http://qup.hnqzz.top

if let n = opt { print(n) }
来源：http://gip.chenzaomai.com

[T20] Swift：数组操作
来源：http://wlh.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://fuh.tian-w.cn

[T21] Swift：遍历
来源：http://htx.yj20258.top

for x in a { print(x) }
来源：http://gja.jinghuilouyu.cn

[T22] Swift：字典
来源：http://eji.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gxl.mhx1999.top

[T23] Swift：函数
来源：http://hpo.yj20258888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hwh.zhiwuduotai.top

[T24] Swift：闭包
来源：http://feq.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fyn.ehwqpu.com

[T25] Swift：结构体
来源：http://wth.hnxiangtu.top

struct P { var x: Int }
来源：http://brc.havefunace.top

[T26] Swift：类与重写
来源：http://mmr.jiagoushi.top

class A: Base { override func f() {} }
来源：http://ali.zhijiandao.cn

[T27] Swift：错误处理
来源：http://xjr.hnqzz.top

do { try f() } catch { print(error) }
来源：http://irc.ydjk.org.cn

[T28] Swift：枚举
来源：http://mpn.zycfv.cn

enum Color { case red, green }
来源：http://ffe.smart0.xyz

[T29] Swift：guard 提前返回
来源：http://rvp.tarul.cn

guard let x = opt else { return }
来源：http://zyc.quarkkingdee.top

[T30] Swift：协议
来源：http://cnt.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://qmq.guannengcc.top

[T31] Lua：Hello World
来源：http://meo.sysykeji.top

print("Hello")
来源：http://hcr.c1oappe.top

[T32] Lua：局部变量
来源：http://hlw.9152youxi.cn

local a = 1
来源：http://cma.52xcode.cn

[T33] Lua：表（数组）
来源：http://opu.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gsc.daria6918.cn

[T34] Lua：遍历表
来源：http://dmj.guowangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://phg.pycfn.com

[T35] Lua：字典表
来源：http://vwg.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://zzd.haohaochexian.top

[T36] Lua：函数
来源：http://rxy.zhiwuduotai.top

function add(a, b) return a + b end
来源：http://cle.smart0.xyz

[T37] Lua：字符串拼接
来源：http://uzl.nwbrower.top

"a" .. "b"
来源：http://pkb.guannengcc.top

[T38] Lua：条件
来源：http://isi.nwbrower.top

if x > 0 then print("正") end
来源：http://jeu.pycfn.com

[T39] Lua：模式匹配
来源：http://oon.ydjk.org.cn

string.find(s, "%d+")
来源：http://loa.sjlbkw.cn

[T40] Lua：元表
来源：http://nyk.havefunace.top

setmetatable({}, { __index = base })
来源：http://ule.hnqzz.top

[T41] Perl：Hello World
来源：http://sai.gaohongyu789.top

print "Hello\n";
来源：http://rcf.xingfuxueyuan.xyz

[T42] Perl：变量类型
来源：http://oit.tianlin.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vhb.hesvh.cn

[T43] Perl：字符串插值
来源：http://vyi.zhengqikj.top

"值: $a"
来源：http://cfs.nanxuanxn.top

[T44] Perl：条件
来源：http://jet.yvedp.cn

if ($a > 0) { print "正"; }
来源：http://vtv.yuxming.cn

[T45] Perl：数组遍历
来源：http://wct.pycfn.com

for my $x (@arr) { print $x; }
来源：http://kqx.jqgfzy.top

[T46] Perl：哈希操作
来源：http://raq.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ukl.guannengcc.top

[T47] Perl：正则捕获
来源：http://dug.feifeiyinyue.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yru.zdbjq.cn

[T48] Perl：正则替换
来源：http://gvf.zdqjudy.top

$s =~ s/old/new/g;
来源：http://hll.9152youxi.cn

[T49] Perl：函数
来源：http://lxn.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rjx.ybcxt.top

[T50] Perl：逐行读文件
来源：http://gzq.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://hxq.hysaishi.cn

while (my $line = <$fh>) { print $line; }
来源：http://bqd.zhengqikj.top

[T51] Scala：Hello World
来源：http://gxx.vehdjk.com

println("Hello")
来源：http://rlk.52xcode.cn

[T52] Scala：变量
来源：http://epu.xylfe.cn

val a = 1;  var b = 2
来源：http://wyi.jqgufenzy.top

[T53] Scala：字符串插值
来源：http://xmx.wangshuangyany.cn

s"值: $b"
来源：http://wra.hywenlv.cn

[T54] Scala：集合映射
来源：http://cbt.zdqjudy.top

List(1, 2, 3).map(_ * 2)
来源：http://pqp.xuetiantiany.cn

[T55] Scala：集合过滤
来源：http://xzj.vqdsnc.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nqz.xziqi.cn

[T56] Scala：样例类
来源：http://apa.cheryme.top

case class User(name: String, age: Int)
来源：http://hhs.yj202588.top

[T57] Scala：模式匹配
来源：http://luf.cqqwz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iqh.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://mhl.nanxuanxn.top

def add(a: Int, b: Int): Int = a + b
来源：http://qvz.sysykeji.top

[T59] Scala：循环
来源：http://pkh.cucudq.cn

for (i <- 1 to 10) println(i)
来源：http://siv.nanxuanxn.top

[T60] Scala：折叠
来源：http://qzs.9152youxi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://suu.hnxiangtu.top

================================================================================
来源：http://oye.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nyr.svipenyu.cn

================================================================================
来源：http://sdd.tianlin.xyz

[U01] Py：创建虚拟环境
来源：http://kan.yj202588.top

python -m venv .venv && source .venv/bin/activate
来源：http://hhq.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://hzc.hysaishi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nhf.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://gbl.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dnb.birdmap.top

[U04] Py：变量调试打印
来源：http://rge.mhx1999.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fln.yj202588.top

[U05] Py：列表去重且保序
来源：http://ljd.haohaochexian.top

list(dict.fromkeys(arr))
来源：http://dyl.hammf.cn

[U06] Py：合并两个字典
来源：http://tqw.fengsongda.top

{**a, **b}
来源：http://kzc.yj20258888.top

[U07] Py：反转字典键值
来源：http://wsy.shanyushiyangkeji.top

{v: k for k, v in d.items()}
来源：http://kug.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://oob.jyoumei.cn

[y for x in nested for y in x]
来源：http://vvt.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://iky.fanxiaobao.xyz

max(d, key=d.get)
来源：http://mij.yangfankeji.com

[U10] Py：按值排序字典
来源：http://tyc.tarul.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ums.zdqjudy.top

[U11] Py：生成器表达式
来源：http://mgf.dianchejie.cn

(x * 2 for x in arr)
来源：http://pkg.cqqwz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lzq.yvedp.cn

Counter(arr).most_common(3)
来源：http://jkr.tian-w.cn


<!-- 参考信息 -->