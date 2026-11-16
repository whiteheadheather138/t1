代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://qlt.svipenyu.cn

[R76] 使用临时文件
来源：http://teu.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ofh.yonumen.top

[R77] 读取用户输入
来源：http://qxd.smart0.xyz

read -rp "请输入: " ans
来源：http://mcy.9152youxi.cn

[R78] 交互式菜单
来源：http://ssm.hnqzz.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ufb.ydjk.org.cn

[R79] 解析命令行选项
来源：http://fcd.jyoumei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://apc.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://pfk.jqgufenzy.top

time ./run.sh
来源：http://zss.chenlongwang.top

================================================================================
来源：http://mcl.sysykeji.top

S. C / C++ 专题
来源：http://oos.redwolf501.top

================================================================================
来源：http://dsr.sweek.top

[S01] C：Hello World
来源：http://ila.shuidangran.top

#include <stdio.h>
来源：http://tmo.ctjpmb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://hah.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://nvc.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://dmj.uphjek.com

[S03] C：读入整数
来源：http://lau.52xcode.cn

int x; scanf("%d", &x);
来源：http://vyk.yfazqb.com

[S04] C：字符串复制
来源：http://idt.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://wbq.zdbjq.cn

[S05] C：字符串长度
来源：http://pia.tian-w.cn

strlen(s)
来源：http://siy.yonumen.top

[S06] C：字符串比较
来源：http://ost.zhaomingkeji.xyz

strcmp(a, b) == 0
来源：http://qqq.ppjwa.cn

[S07] C：数组遍历求和
来源：http://vbq.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://afy.yueranfly.top

[S08] C：动态内存分配与释放
来源：http://yuo.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uss.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://cuy.jinghuilouyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ydu.hcnkem.com

[S10] C：指针与解引用
来源：http://gmg.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://xxj.xziqi.cn

[S11] C：逐行读文件
来源：http://srt.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://pqf.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dmt.316326.xyz

fclose(f);
来源：http://zuv.sxryk.cn

[S12] C：写文件
来源：http://nzq.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pds.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://vod.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vix.bjfxy.top

[S14] C：枚举
来源：http://akg.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://ckj.0kj1m.cn

[S15] C：类型转换
来源：http://geu.tianlin.xyz

(double) a / b
来源：http://plv.jinqigfzy.top

[S16] C：位操作置位
来源：http://bkn.zhengqikj.top

x |= (1 << 3);
来源：http://uuk.zhixingplan.top

[S17] C：安全拼接字符串
来源：http://wag.ivvv.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sbd.jinqigfzy.top

[S18] C：命令行参数
来源：http://dwl.xuanzx.com

int main(int argc, char **argv)
来源：http://iyp.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://qmn.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://gbq.xuanzx.com

[S20] C：二分查找
来源：http://osw.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wev.yj20258888.top

[S21] C：字符类别判断
来源：http://yhb.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pdd.fehbvm.com

[S22] C：字符串转数字
来源：http://gps.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://oyw.jinyuanbaomall.cn

[S23] C：随机数
来源：http://hal.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ufy.kuanghao11.cn

[S24] C：获取本地时间
来源：http://unj.jyoumei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zve.fehbvm.com

[S25] C：内存拷贝
来源：http://tbx.jianghu66.top

memcpy(dst, src, n);
来源：http://gqu.aizwys.cn

[S26] C：内存清零
来源：http://rqb.pycfn.com

memset(a, 0, sizeof a);
来源：http://ojq.cdnleiting.top

[S27] C：定义常量
来源：http://zof.hcnkem.com

const double PI = 3.14159;
来源：http://xaj.pengpengdd.cyou

[S28] C：静态变量
来源：http://fod.bjfxy.top

static int counter = 0;
来源：http://xim.daxiang520.top

[S29] C：变参函数
来源：http://ocn.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ntn.xinyue.icu

[S30] C：头文件保护
来源：http://drc.nanxuanxn.top

#ifndef X_H
来源：http://yek.redwolf501.top

#define X_H
来源：http://wap.zhoulong.xyz

#endif
来源：http://ebl.hysaishi.cn

[S31] C++：Hello World
来源：http://bsk.yueranfly.top

#include <iostream>
来源：http://qbl.ctjpmb.com

int main() { std::cout << "Hello\n"; }
来源：http://gkg.zhijiandao.cn

[S32] C++：字符串
来源：http://tal.hesvh.cn

std::string s = "hi";  s += "!";
来源：http://aon.0kj1m.cn

[S33] C++：vector 增删
来源：http://uil.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pvp.feifeiyinyue.top

[S34] C++：遍历 vector
来源：http://pgn.birdmap.top

for (auto &x : v) { std::cout << x; }
来源：http://oma.xuetiantiany.cn

[S35] C++：map
来源：http://ffb.shanyushiyangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jdd.yj20258888.top

[S36] C++：unordered_map
来源：http://glk.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kyq.bbcook.cn

[S37] C++：set
来源：http://lqu.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qjn.vqdsnc.cn

[S38] C++：排序
来源：http://pob.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://mux.yuxming.cn

[S39] C++：自定义比较器排序
来源：http://zua.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://esj.zhoulong.xyz

[S40] C++：查找元素
来源：http://vuf.jinyuanbaomall.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yjt.chenjidiqi.icu

[S41] C++：类与构造函数
来源：http://nsk.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xcq.fzhhl.top

[S42] C++：继承与虚函数
来源：http://xag.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://zod.jinqigfzy.top

[S43] C++：智能指针
来源：http://ksh.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://wdb.fanxiaobao.xyz

[S44] C++：引用传参
来源：http://jvj.yuxming.cn

void inc(int &x) { ++x; }
来源：http://eea.yuanzhike.top

[S45] C++：lambda
来源：http://lpp.gaohongyu789.top

auto add = [](int a, int b) { return a + b; };
来源：http://etp.pengpengdd.cyou

[S46] C++：函数模板
来源：http://vep.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fqh.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://jmp.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ptc.jinghuilouyu.cn

[S48] C++：逐行读文件
来源：http://tqr.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://ijw.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://fjy.xuetiantiany.cn

[S49] C++：写文件
来源：http://sbv.meibo888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sqr.gaohongyu789.top

[S50] C++：格式化数字
来源：http://xdg.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wqz.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://jhx.ehwqpu.com

static_cast<double>(a) / b
来源：http://jay.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://qdy.redwolf501.top

int size() const noexcept { return n_; }
来源：http://shu.fktsv.cn

[S53] C++：移动语义
来源：http://geq.fanxiaobao.xyz

std::vector<int> w = std::move(v);
来源：http://gsg.zdqjudy.top

[S54] C++：异常处理
来源：http://wzc.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gzd.aizwys.cn

[S55] C++：结构化绑定
来源：http://tch.jinqigfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uck.shangyingyoupin.top

[S56] C++：optional
来源：http://fvr.yangfankeji.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xcq.ybcxt.top

[S57] C++：编译期常量
来源：http://tpm.andypj.xyz

constexpr int N = 10;
来源：http://voc.pycfn.com

[S58] C++：命名空间
来源：http://thg.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://age.jiagoushi.top

[S59] C++：静态断言
来源：http://bjw.gzhubu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wvo.dianchejie.cn

[S60] C++：遍历并删除元素
来源：http://vfr.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mck.jinqigfzy.top

================================================================================
来源：http://oke.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://spa.yuxming.cn

================================================================================
来源：http://row.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://xuu.yuxming.cn

println("Hello")
来源：http://cwd.zhijiandao.cn

[T02] Kotlin：变量
来源：http://fbb.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nah.hywenlv.cn

[T03] Kotlin：字符串模板
来源：http://fqe.daria6918.cn

"值: $b"
来源：http://kuk.yj20258888.top

[T04] Kotlin：空安全
来源：http://bmh.vehdjk.com

val n: String? = null;  n?.length
来源：http://cgu.fanxiaobao.xyz

[T05] Kotlin：when 表达式
来源：http://bjd.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ijt.yfazqb.com

[T06] Kotlin：集合映射
来源：http://acu.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tzp.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://ixk.hywenlv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oms.yuxming.cn

[T08] Kotlin：数据类
来源：http://erk.shangyingyoupin.top

data class User(val name: String, val age: Int)
来源：http://dyq.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://qzz.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://hgo.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://brq.cheryme.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pka.xziqi.cn

[T11] Kotlin：协程
来源：http://jgm.yuanzhike.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sip.guowangkeji.top

[T12] Kotlin：解构声明
来源：http://ldr.mhx1999.top

val (a, b) = Pair(1, 2)
来源：http://fom.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://umh.svipenyu.cn

val m = mapOf("a" to 1)
来源：http://olg.nanxuanxn.top

[T14] Kotlin：循环
来源：http://nlb.jqgfzy.top

for (i in 1..10) println(i)
来源：http://mmb.epnwcf.com

[T15] Kotlin：接口
来源：http://zbq.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://fjp.yfazqb.com

[T16] Swift：Hello World
来源：http://zlq.ywan-chungtsiang.top

print("Hello")
来源：http://xvj.jinyuanbaomall.cn

[T17] Swift：变量与常量
来源：http://pqi.zhixingplan.top

var a = 1;  let b = 2
来源：http://rzw.chenzaomai.com

[T18] Swift：字符串插值
来源：http://nvv.chenlongwang.top

"值: \(b)"
来源：http://nul.chenlongwang.top

[T19] Swift：可选绑定
来源：http://bfs.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://gtf.chenlongwang.top

[T20] Swift：数组操作
来源：http://swx.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://ezb.kuanghao11.cn

[T21] Swift：遍历
来源：http://clk.nanxinkj.top

for x in a { print(x) }
来源：http://zgq.tarul.cn

[T22] Swift：字典
来源：http://lqe.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://uso.fzhhl.top

[T23] Swift：函数
来源：http://zjr.cucudq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eyz.sweek.top

[T24] Swift：闭包
来源：http://iot.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oil.shanyushiyangtech.top

[T25] Swift：结构体
来源：http://veq.jianghu66.top

struct P { var x: Int }
来源：http://hjs.xingfuxueyuan.xyz

[T26] Swift：类与重写
来源：http://ohq.hnqzz.top

class A: Base { override func f() {} }
来源：http://tgx.yongpay.top

[T27] Swift：错误处理
来源：http://mfr.daria6918.cn

do { try f() } catch { print(error) }
来源：http://zna.ydjk.org.cn

[T28] Swift：枚举
来源：http://dds.ydzc1.top

enum Color { case red, green }
来源：http://rhn.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://tmv.sjlbkw.cn

guard let x = opt else { return }
来源：http://geb.hfpthk.cn

[T30] Swift：协议
来源：http://mat.gogol.net.cn

protocol Shape { func area() -> Double }
来源：http://pqb.hnxiangtu.top

[T31] Lua：Hello World
来源：http://lll.tian-w.cn

print("Hello")
来源：http://wve.shanyushiyangkeji.top

[T32] Lua：局部变量
来源：http://xgj.ctjpmb.com

local a = 1
来源：http://szn.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://ewp.xingfuxueyuan.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://wnn.cdnleiting.top

[T34] Lua：遍历表
来源：http://iih.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://urg.bbcook.cn

[T35] Lua：字典表
来源：http://eqq.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://osd.ywan-chungtsiang.top

[T36] Lua：函数
来源：http://ctj.jqgfzy.top

function add(a, b) return a + b end
来源：http://tpm.sufxvd.cn

[T37] Lua：字符串拼接
来源：http://uye.tarul.cn

"a" .. "b"
来源：http://vvn.tanke756.top

[T38] Lua：条件
来源：http://tkm.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://mpp.ctjpmb.com

[T39] Lua：模式匹配
来源：http://tdt.zhengqikj.top

string.find(s, "%d+")
来源：http://trc.meibo888.top

[T40] Lua：元表
来源：http://nzn.ehwqpu.com

setmetatable({}, { __index = base })
来源：http://tis.ivvv.top

[T41] Perl：Hello World
来源：http://eks.ppjwa.cn

print "Hello\n";
来源：http://ukt.havefunace.top

[T42] Perl：变量类型
来源：http://rdo.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vjp.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://qdm.hysaishi.cn

"值: $a"
来源：http://dzw.ppjwa.cn

[T44] Perl：条件
来源：http://dbl.yj20258.top

if ($a > 0) { print "正"; }
来源：http://gmu.chenzaomai.com

[T45] Perl：数组遍历
来源：http://sdk.gogol.net.cn

for my $x (@arr) { print $x; }
来源：http://vax.hysaishi.cn

[T46] Perl：哈希操作
来源：http://vhh.hammf.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xmt.feifeiyinyue.top

[T47] Perl：正则捕获
来源：http://dmv.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tim.9152youxi.cn

[T48] Perl：正则替换
来源：http://dtz.chenlongwang.top

$s =~ s/old/new/g;
来源：http://sfj.pengpengdd.cyou

[T49] Perl：函数
来源：http://vdh.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ppn.c1oappe.top

[T50] Perl：逐行读文件
来源：http://pte.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gdb.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://vwm.snrcjt.cn

[T51] Scala：Hello World
来源：http://lzj.9152youxi.cn

println("Hello")
来源：http://tvi.haohaochexian.top

[T52] Scala：变量
来源：http://klz.0kj1m.cn

val a = 1;  var b = 2
来源：http://xmn.jqgfzy.top

[T53] Scala：字符串插值
来源：http://xgn.zhixingplan.top

s"值: $b"
来源：http://zcj.fehbvm.com

[T54] Scala：集合映射
来源：http://gkj.ydjk.org.cn

List(1, 2, 3).map(_ * 2)
来源：http://bky.dashuyun.cn

[T55] Scala：集合过滤
来源：http://djo.jinyuanbaomall.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hap.xuanzx.com

[T56] Scala：样例类
来源：http://ppa.dashuyun.cn

case class User(name: String, age: Int)
来源：http://xyu.yangfankeji.com

[T57] Scala：模式匹配
来源：http://dqt.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zyh.feifeiyinyue.top

[T58] Scala：函数定义
来源：http://mds.quarkkingdee.top

def add(a: Int, b: Int): Int = a + b
来源：http://uxe.nanxuanxn.top

[T59] Scala：循环
来源：http://xcj.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://ddk.0kj1m.cn

[T60] Scala：折叠
来源：http://rnj.fzhhl.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tuq.jinqigufen.top

================================================================================
来源：http://goh.svipenyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rnc.jyoumei.cn

================================================================================
来源：http://twf.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://wlr.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cac.sjlbkw.cn

[U02] Py：导出 / 安装依赖
来源：http://hgy.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://obh.cqqwz.cn

[U03] Py：加载 .env 配置
来源：http://tbr.jlsjyb.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tvg.ppjwa.cn

[U04] Py：变量调试打印
来源：http://ptn.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yoc.yonumen.top

[U05] Py：列表去重且保序
来源：http://sfm.cashguo.top

list(dict.fromkeys(arr))
来源：http://ptq.hcnkem.com

[U06] Py：合并两个字典
来源：http://djq.hysaishi.cn

{**a, **b}
来源：http://usr.jiagoushi.top

[U07] Py：反转字典键值
来源：http://dlp.jiagoushi.top

{v: k for k, v in d.items()}
来源：http://aad.zhixingplan.top

[U08] Py：展平二维列表
来源：http://ubp.guannengcc.top

[y for x in nested for y in x]
来源：http://crw.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://wkd.jqgufenzy.top

max(d, key=d.get)
来源：http://lvy.yj202588.top

[U10] Py：按值排序字典
来源：http://idp.jyoumei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mze.cdnleiting.top

[U11] Py：生成器表达式
来源：http://cpv.ydzc1.top

(x * 2 for x in arr)
来源：http://viq.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://ebl.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://otl.guowangkeji.top

[U13] Py：固定长度队列
来源：http://jox.0kj1m.cn

deque(maxlen=10)
来源：http://lkz.hnxiangtu.top

[U14] Py：分组收集到列表
来源：http://ksc.gogol.net.cn

defaultdict(list)
来源：http://dwb.c1oappe.top

[U15] Py：高精度计时
来源：http://eng.jinqigfzy.top

t = time.perf_counter()
来源：http://qsm.sxryk.cn

[U16] Py：命令行参数解析
来源：http://sag.yj20258.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ceb.zhengqikj.top


<!-- 参考信息 -->