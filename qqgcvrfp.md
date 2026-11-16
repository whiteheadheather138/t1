代发 wailian999

split -l 1000 big.log part_
来源：http://sdn.feifeiyinyue.top

[R74] 批量重命名
来源：http://hnw.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rbj.cdnleiting.top

[R75] 导出环境变量
来源：http://pol.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://pje.c1oappe.top

[R76] 使用临时文件
来源：http://poi.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fzz.quarkkingdee.top

[R77] 读取用户输入
来源：http://pyy.sweek.top

read -rp "请输入: " ans
来源：http://cox.sjlbkw.cn

[R78] 交互式菜单
来源：http://bvv.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://law.bjfxy.top

[R79] 解析命令行选项
来源：http://zha.jyoumei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://euk.hywenlv.cn

[R80] 查看脚本执行耗时
来源：http://ifw.aizwys.cn

time ./run.sh
来源：http://cwb.cdnleiting.top

================================================================================
来源：http://zej.zhijiandao.cn

S. C / C++ 专题
来源：http://alv.redwolf501.top

================================================================================
来源：http://sco.cashguo.top

[S01] C：Hello World
来源：http://jrk.zhijiandao.cn

#include <stdio.h>
来源：http://cua.chenzaomai.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://bcf.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://lii.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://nzp.yongpay.top

[S03] C：读入整数
来源：http://nti.iojbl.cn

int x; scanf("%d", &x);
来源：http://ulu.sufxvd.cn

[S04] C：字符串复制
来源：http://nbj.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yqt.hywenlv.cn

[S05] C：字符串长度
来源：http://pih.xylfe.cn

strlen(s)
来源：http://rsi.zhoulong.xyz

[S06] C：字符串比较
来源：http://vif.tian-w.cn

strcmp(a, b) == 0
来源：http://vgt.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://bqd.xingfuxueyuan.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mgo.aibaodan.cn

[S08] C：动态内存分配与释放
来源：http://vdl.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yky.shuidangran.top

[S09] C：结构体定义与初始化
来源：http://qkh.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ypo.jlsjyb.cn

[S10] C：指针与解引用
来源：http://vwz.dashuyun.cn

int *p = &a;  *p = 5;
来源：http://exv.bjfxy.top

[S11] C：逐行读文件
来源：http://goo.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://pvd.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://low.xziqi.cn

fclose(f);
来源：http://xla.hysaishi.cn

[S12] C：写文件
来源：http://yxp.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zhh.sxryk.cn

[S13] C：宏定义
来源：http://kob.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://csz.cashguo.top

[S14] C：枚举
来源：http://sxp.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://aeb.jlsjyb.cn

[S15] C：类型转换
来源：http://vzn.yj20258.top

(double) a / b
来源：http://mco.svipenyu.cn

[S16] C：位操作置位
来源：http://zgs.tian-w.cn

x |= (1 << 3);
来源：http://oir.bjfxy.top

[S17] C：安全拼接字符串
来源：http://mpp.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ftc.cashguo.top

[S18] C：命令行参数
来源：http://mqj.zhijiandao.cn

int main(int argc, char **argv)
来源：http://ves.xylfe.cn

[S19] C：快速排序
来源：http://vny.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hvi.xinyue.icu

[S20] C：二分查找
来源：http://qpo.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mzt.nanxuanxn.top

[S21] C：字符类别判断
来源：http://drj.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://deb.jinqigufen.top

[S22] C：字符串转数字
来源：http://bfw.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aym.52xcode.cn

[S23] C：随机数
来源：http://ckx.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rho.pycfn.com

[S24] C：获取本地时间
来源：http://hda.jyoumei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vzy.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://mxw.jinqigfzy.top

memcpy(dst, src, n);
来源：http://rdj.fzhhl.top

[S26] C：内存清零
来源：http://onl.nanxinkj.top

memset(a, 0, sizeof a);
来源：http://auu.zhoulong.xyz

[S27] C：定义常量
来源：http://fsd.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://tlm.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://oex.yongpay.top

static int counter = 0;
来源：http://bld.nwbrower.top

[S29] C：变参函数
来源：http://xhn.jinqigufen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://enc.xziqi.cn

[S30] C：头文件保护
来源：http://cwi.fengsongda.top

#ifndef X_H
来源：http://mlx.ppjwa.cn

#define X_H
来源：http://vld.yj20258888.top

#endif
来源：http://aik.zhongyouzk.top

[S31] C++：Hello World
来源：http://csz.fengsongda.top

#include <iostream>
来源：http://bzf.snrcjt.cn

int main() { std::cout << "Hello\n"; }
来源：http://rpu.ctjpmb.com

[S32] C++：字符串
来源：http://eia.pycfn.com

std::string s = "hi";  s += "!";
来源：http://ecm.9152youxi.cn

[S33] C++：vector 增删
来源：http://hvl.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mio.tanke756.top

[S34] C++：遍历 vector
来源：http://ajc.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://ttn.cashguo.top

[S35] C++：map
来源：http://hxi.hongshengwenyu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vzl.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://rli.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cwy.chenjidiqi.icu

[S37] C++：set
来源：http://flu.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wtb.316326.xyz

[S38] C++：排序
来源：http://meh.tianlin.xyz

std::sort(v.begin(), v.end());
来源：http://nkg.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://axy.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rbx.shuidangran.top

[S40] C++：查找元素
来源：http://zen.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bii.havefunace.top

[S41] C++：类与构造函数
来源：http://kgl.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hcc.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://fvw.ydzc1.top

class B : public Base { public: void f() override {} };
来源：http://eir.wangdashe.top

[S43] C++：智能指针
来源：http://iap.jinqigufen.top

auto p = std::make_unique<int>(5);
来源：http://otj.gzhubu.top

[S44] C++：引用传参
来源：http://qut.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://gjx.ppjwa.cn

[S45] C++：lambda
来源：http://hua.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oen.fktsv.cn

[S46] C++：函数模板
来源：http://iin.gzhubu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ilg.guannengcc.top

[S47] C++：结构化绑定遍历
来源：http://gvz.guannengcc.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xul.aizwys.cn

[S48] C++：逐行读文件
来源：http://bda.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xei.guowangkeji.top

while (std::getline(in, line)) { }
来源：http://hhd.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://ula.yuxming.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ovw.nwbrower.top

[S50] C++：格式化数字
来源：http://cpz.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vkw.sufxvd.cn

[S51] C++：显式类型转换
来源：http://shu.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://glc.xingfuxueyuan.xyz

[S52] C++：const 与 noexcept
来源：http://jbd.zycfv.cn

int size() const noexcept { return n_; }
来源：http://ddb.wangshuangyany.cn

[S53] C++：移动语义
来源：http://ypt.bjfxy.top

std::vector<int> w = std::move(v);
来源：http://nyy.zhiwuduotai.top

[S54] C++：异常处理
来源：http://krb.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zaj.tian-w.cn

[S55] C++：结构化绑定
来源：http://mqg.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://pzj.sufxvd.cn

[S56] C++：optional
来源：http://clu.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vsk.yj202588.top

[S57] C++：编译期常量
来源：http://oeo.zhijiandao.cn

constexpr int N = 10;
来源：http://vaj.chenjidiqi.icu

[S58] C++：命名空间
来源：http://slu.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://bwa.jiagoushi.top

[S59] C++：静态断言
来源：http://tod.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gbl.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://ufo.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ibm.yonumen.top

================================================================================
来源：http://huc.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yox.xingfuxueyuan.xyz

================================================================================
来源：http://nhr.daria6918.cn

[T01] Kotlin：Hello World
来源：http://gha.aibaodan.cn

println("Hello")
来源：http://kys.wangdashe.top

[T02] Kotlin：变量
来源：http://ggq.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rfh.yongpay.top

[T03] Kotlin：字符串模板
来源：http://akw.pycfn.com

"值: $b"
来源：http://sdf.fktsv.cn

[T04] Kotlin：空安全
来源：http://qaq.chenzaomai.com

val n: String? = null;  n?.length
来源：http://jvv.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://tka.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://asl.cashguo.top

[T06] Kotlin：集合映射
来源：http://qfe.shzxlz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tvd.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://ana.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pzn.zhaomingkeji.xyz

[T08] Kotlin：数据类
来源：http://gch.birdmap.top

data class User(val name: String, val age: Int)
来源：http://utc.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://kxv.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://sut.daxiang520.top

[T10] Kotlin：默认参数
来源：http://pim.hfpthk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dmw.nanxuanxn.top

[T11] Kotlin：协程
来源：http://yeh.hnqzz.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mjq.birdmap.top

[T12] Kotlin：解构声明
来源：http://smk.wangshuangyany.cn

val (a, b) = Pair(1, 2)
来源：http://amz.jianghu66.top

[T13] Kotlin：只读 Map
来源：http://rau.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://ywr.zhoulong.xyz

[T14] Kotlin：循环
来源：http://hdd.hywenlv.cn

for (i in 1..10) println(i)
来源：http://ppb.shanyushiyangtech.top

[T15] Kotlin：接口
来源：http://ceo.zycfv.cn

interface Shape { fun area(): Double }
来源：http://fbi.zhongyouzk.top

[T16] Swift：Hello World
来源：http://lnm.jqgufenzy.top

print("Hello")
来源：http://vdg.ppjwa.cn

[T17] Swift：变量与常量
来源：http://chb.sjlbkw.cn

var a = 1;  let b = 2
来源：http://xuu.pycfn.com

[T18] Swift：字符串插值
来源：http://gyh.hnxiangtu.top

"值: \(b)"
来源：http://jcd.haohaochexian.top

[T19] Swift：可选绑定
来源：http://min.ybcxt.top

if let n = opt { print(n) }
来源：http://che.ivvv.top

[T20] Swift：数组操作
来源：http://int.guannengcc.top

var a = [1, 2, 3];  a.append(4)
来源：http://wij.chenzaomai.com

[T21] Swift：遍历
来源：http://vzk.nwbrower.top

for x in a { print(x) }
来源：http://cix.nanxinkj.top

[T22] Swift：字典
来源：http://pjh.zhijiandao.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kxg.ybcxt.top

[T23] Swift：函数
来源：http://dys.jinghuilouyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yiz.hongshengwenyu.top

[T24] Swift：闭包
来源：http://vnu.epnwcf.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://zfn.yanxiufei.cn

[T25] Swift：结构体
来源：http://sir.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://vxg.jqgufenzy.top

[T26] Swift：类与重写
来源：http://fkt.daria6918.cn

class A: Base { override func f() {} }
来源：http://gcc.yj20258.top

[T27] Swift：错误处理
来源：http://mlo.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://pfe.zhiwuduotai.top

[T28] Swift：枚举
来源：http://aov.cdnleiting.top

enum Color { case red, green }
来源：http://wbx.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://wfu.havefunace.top

guard let x = opt else { return }
来源：http://ilj.havefunace.top

[T30] Swift：协议
来源：http://pmk.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://ykf.cucudq.cn

[T31] Lua：Hello World
来源：http://uox.daria6918.cn

print("Hello")
来源：http://rly.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://pkp.yonumen.top

local a = 1
来源：http://zkp.sxryk.cn

[T33] Lua：表（数组）
来源：http://zeg.shangyingyoupin.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jpd.shangyingyoupin.top

[T34] Lua：遍历表
来源：http://dho.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jnh.hcnkem.com

[T35] Lua：字典表
来源：http://agp.zhongyouzk.top

local d = { a = 1 };  d.b = 2
来源：http://dit.zhixingplan.top

[T36] Lua：函数
来源：http://kjo.yuanzhike.top

function add(a, b) return a + b end
来源：http://mft.yangfankeji.com

[T37] Lua：字符串拼接
来源：http://yqb.hesvh.cn

"a" .. "b"
来源：http://qfc.bbcook.cn

[T38] Lua：条件
来源：http://zwi.hnqzz.top

if x > 0 then print("正") end
来源：http://lyj.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://ewd.hammf.cn

string.find(s, "%d+")
来源：http://caf.redwolf501.top

[T40] Lua：元表
来源：http://str.bjfxy.top

setmetatable({}, { __index = base })
来源：http://vny.hammf.cn

[T41] Perl：Hello World
来源：http://wfv.pycfn.com

print "Hello\n";
来源：http://xkd.hcnkem.com

[T42] Perl：变量类型
来源：http://ymy.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qbi.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://hwd.ehwqpu.com

"值: $a"
来源：http://pye.jinghuilouyu.cn

[T44] Perl：条件
来源：http://wfs.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://oqg.xinyue.icu

[T45] Perl：数组遍历
来源：http://vwy.nanxinkj.top

for my $x (@arr) { print $x; }
来源：http://olc.cucudq.cn

[T46] Perl：哈希操作
来源：http://uoa.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vpv.cdnleiting.top

[T47] Perl：正则捕获
来源：http://dfh.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://alp.tianlin.xyz

[T48] Perl：正则替换
来源：http://ycb.pengpengdd.cyou

$s =~ s/old/new/g;
来源：http://pul.0kj1m.cn

[T49] Perl：函数
来源：http://xra.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qfp.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://zou.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://toq.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://usv.xuetiantiany.cn

[T51] Scala：Hello World
来源：http://slm.haohaochexian.top

println("Hello")
来源：http://eci.xylfe.cn

[T52] Scala：变量
来源：http://fxd.yj20258.top

val a = 1;  var b = 2
来源：http://kyf.0kj1m.cn

[T53] Scala：字符串插值
来源：http://ude.yfazqb.com

s"值: $b"
来源：http://aww.yangfankeji.com

[T54] Scala：集合映射
来源：http://nuq.jqgufenzy.top

List(1, 2, 3).map(_ * 2)
来源：http://rrk.yangfankeji.com

[T55] Scala：集合过滤
来源：http://azw.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xos.sxryk.cn

[T56] Scala：样例类
来源：http://ixv.svipenyu.cn

case class User(name: String, age: Int)
来源：http://thd.aizwys.cn

[T57] Scala：模式匹配
来源：http://myy.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qyk.guowangkeji.top

[T58] Scala：函数定义
来源：http://gnn.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://jec.hcnkem.com

[T59] Scala：循环
来源：http://whk.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://yex.chenzaomai.com

[T60] Scala：折叠
来源：http://waw.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dzp.xuanzx.com

================================================================================
来源：http://qph.chenzaomai.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cqr.pycfn.com

================================================================================
来源：http://ezr.wangshuangyany.cn

[U01] Py：创建虚拟环境
来源：http://yqc.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://arr.redwolf501.top

[U02] Py：导出 / 安装依赖
来源：http://xrq.sxryk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bmp.svipenyu.cn

[U03] Py：加载 .env 配置
来源：http://qam.ywan-chungtsiang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://aiq.jyoumei.cn

[U04] Py：变量调试打印
来源：http://udx.hysaishi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qce.sufxvd.cn

[U05] Py：列表去重且保序
来源：http://xvp.52xcode.cn

list(dict.fromkeys(arr))
来源：http://rif.zdbjq.cn

[U06] Py：合并两个字典
来源：http://byv.fengsongda.top

{**a, **b}
来源：http://etg.shzxlz.cn

[U07] Py：反转字典键值
来源：http://uuw.smart0.xyz

{v: k for k, v in d.items()}
来源：http://fqy.snrcjt.cn

[U08] Py：展平二维列表
来源：http://mfq.ehwqpu.com

[y for x in nested for y in x]
来源：http://abq.daxiang520.top

[U09] Py：字典取最大值的键
来源：http://yyw.zhoulong.xyz

max(d, key=d.get)
来源：http://cxp.zhoulong.xyz

[U10] Py：按值排序字典
来源：http://yzx.jinqigfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ewn.jyoumei.cn

[U11] Py：生成器表达式
来源：http://rnw.hfpthk.cn

(x * 2 for x in arr)
来源：http://vnm.sysykeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://csf.cheryme.top

Counter(arr).most_common(3)
来源：http://hqe.yvedp.cn

[U13] Py：固定长度队列
来源：http://rkh.zhijiandao.cn

deque(maxlen=10)
来源：http://xgp.hysaishi.cn

[U14] Py：分组收集到列表
来源：http://wer.tanke756.top

defaultdict(list)
来源：http://odr.jiagoushi.top


<!-- 参考信息 -->