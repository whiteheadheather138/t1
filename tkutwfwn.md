代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://voz.jyoumei.cn

[R72] 等待端口就绪
来源：http://pcu.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jdw.guannengcc.top

[R73] 分割大日志
来源：http://zim.guowangkeji.top

split -l 1000 big.log part_
来源：http://fma.cashguo.top

[R74] 批量重命名
来源：http://agt.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rkr.shangyingyoupin.top

[R75] 导出环境变量
来源：http://fet.zdbjq.cn

export PATH="$HOME/bin:$PATH"
来源：http://hsl.cucudq.cn

[R76] 使用临时文件
来源：http://oga.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sje.aizwys.cn

[R77] 读取用户输入
来源：http://tvq.yueranfly.top

read -rp "请输入: " ans
来源：http://wof.yuanzhike.top

[R78] 交互式菜单
来源：http://fki.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://goz.xziqi.cn

[R79] 解析命令行选项
来源：http://qdo.yongpay.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uef.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://xpb.xziqi.cn

time ./run.sh
来源：http://yll.tarul.cn

================================================================================
来源：http://fnb.zdbjq.cn

S. C / C++ 专题
来源：http://dze.guowangkeji.top

================================================================================
来源：http://ejz.sjlbkw.cn

[S01] C：Hello World
来源：http://qsq.hongshengwenyu.top

#include <stdio.h>
来源：http://biu.aizwys.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://emo.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://jnv.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://sih.guowangkeji.top

[S03] C：读入整数
来源：http://nli.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://jad.9152youxi.cn

[S04] C：字符串复制
来源：http://iip.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://yry.c1oappe.top

[S05] C：字符串长度
来源：http://hty.kuanghao11.cn

strlen(s)
来源：http://gro.xylfe.cn

[S06] C：字符串比较
来源：http://chr.fehbvm.com

strcmp(a, b) == 0
来源：http://ybx.hammf.cn

[S07] C：数组遍历求和
来源：http://pql.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ksr.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://suh.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://whb.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://hho.tanke756.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hoo.wangdashe.top

[S10] C：指针与解引用
来源：http://yms.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://chg.fanxiaobao.xyz

[S11] C：逐行读文件
来源：http://cmj.quarkkingdee.top

FILE *f = fopen("a.txt", "r");
来源：http://cqg.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://zsa.yj202588.top

fclose(f);
来源：http://ayl.yongpay.top

[S12] C：写文件
来源：http://tsd.xuetiantiany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wyw.gaohongyu789.top

[S13] C：宏定义
来源：http://orb.sjlbkw.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pxi.sweek.top

[S14] C：枚举
来源：http://cqz.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://tse.yueranfly.top

[S15] C：类型转换
来源：http://qyz.yueranfly.top

(double) a / b
来源：http://jsp.zdbjq.cn

[S16] C：位操作置位
来源：http://iez.pengpengdd.cyou

x |= (1 << 3);
来源：http://ikk.aibaodan.cn

[S17] C：安全拼接字符串
来源：http://plf.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vjg.ybcxt.top

[S18] C：命令行参数
来源：http://kil.zhixingplan.top

int main(int argc, char **argv)
来源：http://jft.chenjidiqi.icu

[S19] C：快速排序
来源：http://snn.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://txe.hcnkem.com

[S20] C：二分查找
来源：http://puz.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bhe.sysykeji.top

[S21] C：字符类别判断
来源：http://ejg.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pte.yuanzhike.top

[S22] C：字符串转数字
来源：http://pks.wangshuangyany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bpk.zhixingplan.top

[S23] C：随机数
来源：http://iaf.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zvr.ctjpmb.com

[S24] C：获取本地时间
来源：http://xbs.xuanzx.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ldm.yj202588.top

[S25] C：内存拷贝
来源：http://jqk.hammf.cn

memcpy(dst, src, n);
来源：http://yvi.vehdjk.com

[S26] C：内存清零
来源：http://koy.ivvv.top

memset(a, 0, sizeof a);
来源：http://bad.aibaodan.cn

[S27] C：定义常量
来源：http://otp.xziqi.cn

const double PI = 3.14159;
来源：http://zjz.xuetiantiany.cn

[S28] C：静态变量
来源：http://izj.jinqigfzy.top

static int counter = 0;
来源：http://smb.jyoumei.cn

[S29] C：变参函数
来源：http://iiy.hywenlv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vjd.yfazqb.com

[S30] C：头文件保护
来源：http://tbj.sweek.top

#ifndef X_H
来源：http://wea.feifeiyinyue.top

#define X_H
来源：http://xax.hammf.cn

#endif
来源：http://oth.hnxiangtu.top

[S31] C++：Hello World
来源：http://fge.yvedp.cn

#include <iostream>
来源：http://ziu.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://wdi.gzhubu.top

[S32] C++：字符串
来源：http://dfr.cashguo.top

std::string s = "hi";  s += "!";
来源：http://pty.hesvh.cn

[S33] C++：vector 增删
来源：http://tcv.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://szs.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://xat.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://lyn.jiagoushi.top

[S35] C++：map
来源：http://uia.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jzw.xuetiantiany.cn

[S36] C++：unordered_map
来源：http://lej.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qut.xinyue.icu

[S37] C++：set
来源：http://abc.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zdx.316326.xyz

[S38] C++：排序
来源：http://tvd.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://ymy.hammf.cn

[S39] C++：自定义比较器排序
来源：http://tnj.jqgufenzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kai.haohaochexian.top

[S40] C++：查找元素
来源：http://ely.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ezf.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://vkb.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ubu.andypj.xyz

[S42] C++：继承与虚函数
来源：http://nou.shanyushiyangtech.top

class B : public Base { public: void f() override {} };
来源：http://jpc.ivvv.top

[S43] C++：智能指针
来源：http://eya.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://vuf.cqqwz.cn

[S44] C++：引用传参
来源：http://lgw.havefunace.top

void inc(int &x) { ++x; }
来源：http://buk.yanxiufei.cn

[S45] C++：lambda
来源：http://eyh.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nmi.gotoacloud.top

[S46] C++：函数模板
来源：http://mmj.gogol.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://icw.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://kcg.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gpo.xuetiantiany.cn

[S48] C++：逐行读文件
来源：http://ojq.gaohongyu789.top

std::ifstream in("a.txt");  std::string line;
来源：http://nbw.dashuyun.cn

while (std::getline(in, line)) { }
来源：http://aia.bjfxy.top

[S49] C++：写文件
来源：http://osj.yuxming.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://udr.feifeiyinyue.top

[S50] C++：格式化数字
来源：http://cma.iojbl.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wbg.cucudq.cn

[S51] C++：显式类型转换
来源：http://jfy.gogol.net.cn

static_cast<double>(a) / b
来源：http://obi.gzhubu.top

[S52] C++：const 与 noexcept
来源：http://vxo.nwbrower.top

int size() const noexcept { return n_; }
来源：http://slc.tanke756.top

[S53] C++：移动语义
来源：http://raw.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://sxv.jinqigfzy.top

[S54] C++：异常处理
来源：http://xdp.fzhhl.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gix.xinyue.icu

[S55] C++：结构化绑定
来源：http://zbb.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gym.snrcjt.cn

[S56] C++：optional
来源：http://wrs.wangshuangyany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vbw.cdnleiting.top

[S57] C++：编译期常量
来源：http://fzh.cucudq.cn

constexpr int N = 10;
来源：http://twx.zhongyouzk.top

[S58] C++：命名空间
来源：http://orb.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://hsj.tianlin.xyz

[S59] C++：静态断言
来源：http://kxw.9152youxi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://svn.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://wns.xingfuxueyuan.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lyt.jqgfzy.top

================================================================================
来源：http://vij.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://htz.52xcode.cn

================================================================================
来源：http://jsi.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://qnv.0kj1m.cn

println("Hello")
来源：http://eiq.gzhubu.top

[T02] Kotlin：变量
来源：http://dzo.cqqwz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vdw.yj202588.top

[T03] Kotlin：字符串模板
来源：http://vmy.hcnkem.com

"值: $b"
来源：http://nlm.fehbvm.com

[T04] Kotlin：空安全
来源：http://ucy.0kj1m.cn

val n: String? = null;  n?.length
来源：http://emy.sxryk.cn

[T05] Kotlin：when 表达式
来源：http://pxt.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nyo.sxryk.cn

[T06] Kotlin：集合映射
来源：http://ysr.yvedp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hhu.meibo888.top

[T07] Kotlin：集合过滤
来源：http://vrt.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zsi.chenzaomai.com

[T08] Kotlin：数据类
来源：http://oyl.havefunace.top

data class User(val name: String, val age: Int)
来源：http://khi.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://ahp.yonumen.top

fun String.exclaim() = this + "!"
来源：http://moe.hnxiangtu.top

[T10] Kotlin：默认参数
来源：http://qhi.bjfxy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ott.zdqjudy.top

[T11] Kotlin：协程
来源：http://lfp.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rjr.guowangkeji.top

[T12] Kotlin：解构声明
来源：http://xbi.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://ujr.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://fdg.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://coo.jinqigfzy.top

[T14] Kotlin：循环
来源：http://tqz.yj202588.top

for (i in 1..10) println(i)
来源：http://ppl.jqgfzy.top

[T15] Kotlin：接口
来源：http://kyv.gaohongyu789.top

interface Shape { fun area(): Double }
来源：http://lfk.jinqigfzy.top

[T16] Swift：Hello World
来源：http://qcq.bjfxy.top

print("Hello")
来源：http://ifc.jlsjyb.cn

[T17] Swift：变量与常量
来源：http://hdx.9152youxi.cn

var a = 1;  let b = 2
来源：http://sie.chenlongwang.top

[T18] Swift：字符串插值
来源：http://zll.zhijiandao.cn

"值: \(b)"
来源：http://pbw.hnxiangtu.top

[T19] Swift：可选绑定
来源：http://rdc.c1oappe.top

if let n = opt { print(n) }
来源：http://zaz.pycfn.com

[T20] Swift：数组操作
来源：http://ika.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://vvq.vehdjk.com

[T21] Swift：遍历
来源：http://ayt.kuanghao11.cn

for x in a { print(x) }
来源：http://kwj.hesvh.cn

[T22] Swift：字典
来源：http://nfx.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bwf.jyoumei.cn

[T23] Swift：函数
来源：http://swa.quarkkingdee.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ocv.yuanzhike.top

[T24] Swift：闭包
来源：http://qqk.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://lsr.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://fws.shanyushiyangtech.top

struct P { var x: Int }
来源：http://vbw.sufxvd.cn

[T26] Swift：类与重写
来源：http://obp.nanxinkj.top

class A: Base { override func f() {} }
来源：http://llw.iojbl.cn

[T27] Swift：错误处理
来源：http://bry.zhiwuduotai.top

do { try f() } catch { print(error) }
来源：http://cku.cashguo.top

[T28] Swift：枚举
来源：http://xvc.c1oappe.top

enum Color { case red, green }
来源：http://tkq.chenlongwang.top

[T29] Swift：guard 提前返回
来源：http://msl.xuanzx.com

guard let x = opt else { return }
来源：http://bpp.yuanzhike.top

[T30] Swift：协议
来源：http://aop.yonumen.top

protocol Shape { func area() -> Double }
来源：http://gco.wangdashe.top

[T31] Lua：Hello World
来源：http://qtb.dashuyun.cn

print("Hello")
来源：http://tnv.zhaomingkeji.xyz

[T32] Lua：局部变量
来源：http://msy.kuanghao11.cn

local a = 1
来源：http://rnw.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://sth.zdqjudy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kog.quarkkingdee.top

[T34] Lua：遍历表
来源：http://bbo.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dqs.0kj1m.cn

[T35] Lua：字典表
来源：http://kkz.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://ruz.yonumen.top

[T36] Lua：函数
来源：http://cke.zhongyouzk.top

function add(a, b) return a + b end
来源：http://irk.redwolf501.top

[T37] Lua：字符串拼接
来源：http://dxm.aizwys.cn

"a" .. "b"
来源：http://lyi.fktsv.cn

[T38] Lua：条件
来源：http://hxx.iojbl.cn

if x > 0 then print("正") end
来源：http://noy.9152youxi.cn

[T39] Lua：模式匹配
来源：http://kdy.havefunace.top

string.find(s, "%d+")
来源：http://tof.fengsongda.top

[T40] Lua：元表
来源：http://kok.yuxming.cn

setmetatable({}, { __index = base })
来源：http://rep.nanxuanxn.top

[T41] Perl：Hello World
来源：http://rvt.redwolf501.top

print "Hello\n";
来源：http://pwo.fktsv.cn

[T42] Perl：变量类型
来源：http://hcl.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pkz.pycfn.com

[T43] Perl：字符串插值
来源：http://mdb.fktsv.cn

"值: $a"
来源：http://hyb.epnwcf.com

[T44] Perl：条件
来源：http://dbj.yueranfly.top

if ($a > 0) { print "正"; }
来源：http://nij.zdqjudy.top

[T45] Perl：数组遍历
来源：http://joc.jqgfzy.top

for my $x (@arr) { print $x; }
来源：http://itt.pycfn.com

[T46] Perl：哈希操作
来源：http://ljk.guannengcc.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bfx.yueranfly.top

[T47] Perl：正则捕获
来源：http://lqf.feifeiyinyue.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zug.ydzc1.top

[T48] Perl：正则替换
来源：http://yoe.gogol.net.cn

$s =~ s/old/new/g;
来源：http://bml.cucudq.cn

[T49] Perl：函数
来源：http://dgy.yuanzhike.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mxs.pycfn.com

[T50] Perl：逐行读文件
来源：http://gcg.ywan-chungtsiang.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jiy.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://uvt.hysaishi.cn

[T51] Scala：Hello World
来源：http://sdl.hammf.cn

println("Hello")
来源：http://kwv.jlsjyb.cn

[T52] Scala：变量
来源：http://dua.hfpthk.cn

val a = 1;  var b = 2
来源：http://tac.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://pyc.yuxming.cn

s"值: $b"
来源：http://bkt.shanyushiyangkeji.top

[T54] Scala：集合映射
来源：http://idt.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://twf.hfpthk.cn

[T55] Scala：集合过滤
来源：http://ouv.ehwqpu.com

List(1, 2, 3).filter(_ > 1)
来源：http://svl.yongpay.top

[T56] Scala：样例类
来源：http://dbn.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://xxw.nwbrower.top

[T57] Scala：模式匹配
来源：http://isw.yongpay.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wmd.zhijiandao.cn

[T58] Scala：函数定义
来源：http://qwg.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://koh.jqgfzy.top

[T59] Scala：循环
来源：http://quv.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://ahw.cheryme.top

[T60] Scala：折叠
来源：http://ogv.gzhubu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pxc.xylfe.cn

================================================================================
来源：http://nen.chenzaomai.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xao.dianchejie.cn

================================================================================
来源：http://dvj.zhixingplan.top

[U01] Py：创建虚拟环境
来源：http://prg.0kj1m.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qly.tanke756.top

[U02] Py：导出 / 安装依赖
来源：http://vzg.zdqjudy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sjz.wangdashe.top

[U03] Py：加载 .env 配置
来源：http://xbt.iojbl.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bmy.hywenlv.cn

[U04] Py：变量调试打印
来源：http://ohp.ybcxt.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zpb.52xcode.cn

[U05] Py：列表去重且保序
来源：http://kto.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://cht.vehdjk.com

[U06] Py：合并两个字典
来源：http://dkb.yangfankeji.com

{**a, **b}
来源：http://cel.0kj1m.cn

[U07] Py：反转字典键值
来源：http://pba.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://rjd.c1oappe.top

[U08] Py：展平二维列表
来源：http://wao.daxiang520.top

[y for x in nested for y in x]
来源：http://jmh.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://sxk.fzhhl.top

max(d, key=d.get)
来源：http://yli.gaohongyu789.top

[U10] Py：按值排序字典
来源：http://ybs.vehdjk.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://emv.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://tqy.hnxiangtu.top

(x * 2 for x in arr)
来源：http://tnx.xuanzx.com

[U12] Py：取出现最多的 3 个元素
来源：http://rou.redwolf501.top

Counter(arr).most_common(3)
来源：http://wts.nanxuanxn.top


<!-- 参考信息 -->