代发 wailian999

read -rp "请输入: " ans
来源：http://jte.pycfn.com

[R78] 交互式菜单
来源：http://lfw.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://yzl.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://bqy.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kny.zhixingplan.top

[R80] 查看脚本执行耗时
来源：http://irg.vqdsnc.cn

time ./run.sh
来源：http://lto.yonumen.top

================================================================================
来源：http://ihw.yangfankeji.com

S. C / C++ 专题
来源：http://lzp.jqgfzy.top

================================================================================
来源：http://ket.xylfe.cn

[S01] C：Hello World
来源：http://eyt.sysykeji.top

#include <stdio.h>
来源：http://dkr.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://htm.52xcode.cn

[S02] C：变量与格式化输出
来源：http://njm.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://dcu.vqdsnc.cn

[S03] C：读入整数
来源：http://mpu.iojbl.cn

int x; scanf("%d", &x);
来源：http://hqg.gogol.net.cn

[S04] C：字符串复制
来源：http://voj.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://dak.birdmap.top

[S05] C：字符串长度
来源：http://waz.uphjek.com

strlen(s)
来源：http://ryu.vqdsnc.cn

[S06] C：字符串比较
来源：http://fft.yuxming.cn

strcmp(a, b) == 0
来源：http://yfw.tianlin.xyz

[S07] C：数组遍历求和
来源：http://ehl.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tij.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://pjl.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zwb.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://iuh.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pqa.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://aml.fehbvm.com

int *p = &a;  *p = 5;
来源：http://unq.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://caj.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://bul.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mas.ehwqpu.com

fclose(f);
来源：http://vlx.xuanzx.com

[S12] C：写文件
来源：http://kss.wangshuangyany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xir.cheryme.top

[S13] C：宏定义
来源：http://fai.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rlk.yuxming.cn

[S14] C：枚举
来源：http://hco.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://zzk.gogol.net.cn

[S15] C：类型转换
来源：http://vnx.sweek.top

(double) a / b
来源：http://tuk.xziqi.cn

[S16] C：位操作置位
来源：http://zsu.52xcode.cn

x |= (1 << 3);
来源：http://bmq.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://adk.ivvv.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uec.fehbvm.com

[S18] C：命令行参数
来源：http://ygj.kuanghao11.cn

int main(int argc, char **argv)
来源：http://syf.tianlin.xyz

[S19] C：快速排序
来源：http://dfr.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://fvs.tian-w.cn

[S20] C：二分查找
来源：http://hzs.sweek.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://asq.jqgfzy.top

[S21] C：字符类别判断
来源：http://ujr.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yuk.fzhhl.top

[S22] C：字符串转数字
来源：http://vcw.shuidangran.top

atoi("42");  strtod("3.14", NULL);
来源：http://gzj.shzxlz.cn

[S23] C：随机数
来源：http://lht.gogol.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iuj.zdbjq.cn

[S24] C：获取本地时间
来源：http://ong.zhoulong.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zvs.aizwys.cn

[S25] C：内存拷贝
来源：http://dwm.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://blh.havefunace.top

[S26] C：内存清零
来源：http://vxf.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://kxf.guowangkeji.top

[S27] C：定义常量
来源：http://zpl.yanxiufei.cn

const double PI = 3.14159;
来源：http://bvz.smart0.xyz

[S28] C：静态变量
来源：http://pep.gzhubu.top

static int counter = 0;
来源：http://tnw.yuxming.cn

[S29] C：变参函数
来源：http://ucm.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mzf.ehwqpu.com

[S30] C：头文件保护
来源：http://zic.kuanghao11.cn

#ifndef X_H
来源：http://dsq.jyoumei.cn

#define X_H
来源：http://evs.yanxiufei.cn

#endif
来源：http://dic.yuxming.cn

[S31] C++：Hello World
来源：http://ewv.316326.xyz

#include <iostream>
来源：http://qlw.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://bqh.tanke756.top

[S32] C++：字符串
来源：http://vvq.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://bin.gogol.net.cn

[S33] C++：vector 增删
来源：http://dtm.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gxx.nanxinkj.top

[S34] C++：遍历 vector
来源：http://tkf.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://xwy.nanxinkj.top

[S35] C++：map
来源：http://fan.dashuyun.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fux.yj20258.top

[S36] C++：unordered_map
来源：http://fgo.xuanzx.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hhy.yfazqb.com

[S37] C++：set
来源：http://duz.yuanzhike.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dwc.ydzc1.top

[S38] C++：排序
来源：http://ogy.tarul.cn

std::sort(v.begin(), v.end());
来源：http://yst.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://evt.gzhubu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vid.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://fcp.haohaochexian.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uao.chenjidiqi.icu

[S41] C++：类与构造函数
来源：http://gnz.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oez.mhx1999.top

[S42] C++：继承与虚函数
来源：http://avd.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://vol.yj202588.top

[S43] C++：智能指针
来源：http://bpk.ivvv.top

auto p = std::make_unique<int>(5);
来源：http://xha.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://hde.yongpay.top

void inc(int &x) { ++x; }
来源：http://cif.xziqi.cn

[S45] C++：lambda
来源：http://oqy.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://ens.tian-w.cn

[S46] C++：函数模板
来源：http://hgh.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ium.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://vut.sufxvd.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pta.hnxiangtu.top

[S48] C++：逐行读文件
来源：http://qli.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://vuj.jlsjyb.cn

while (std::getline(in, line)) { }
来源：http://rkw.aizwys.cn

[S49] C++：写文件
来源：http://jox.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nmu.ctjpmb.com

[S50] C++：格式化数字
来源：http://jkh.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xuq.andypj.xyz

[S51] C++：显式类型转换
来源：http://npe.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://kfq.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://wjq.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://lox.cucudq.cn

[S53] C++：移动语义
来源：http://dki.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://iwj.ydzc1.top

[S54] C++：异常处理
来源：http://qfv.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lkf.yonumen.top

[S55] C++：结构化绑定
来源：http://qfh.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vel.wangdashe.top

[S56] C++：optional
来源：http://crw.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wgo.smart0.xyz

[S57] C++：编译期常量
来源：http://vnj.smart0.xyz

constexpr int N = 10;
来源：http://eyb.yvedp.cn

[S58] C++：命名空间
来源：http://mwh.jinyuanbaomall.cn

namespace ns { int f() { return 1; } }
来源：http://ulq.zdbjq.cn

[S59] C++：静态断言
来源：http://pkg.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dwi.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://yfx.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://afs.jinqigfzy.top

================================================================================
来源：http://gxt.nanxinkj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kln.xingfuxueyuan.xyz

================================================================================
来源：http://xgl.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://zkx.daria6918.cn

println("Hello")
来源：http://pkj.shzxlz.cn

[T02] Kotlin：变量
来源：http://tho.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://whn.xziqi.cn

[T03] Kotlin：字符串模板
来源：http://uap.ivvv.top

"值: $b"
来源：http://xkw.hywenlv.cn

[T04] Kotlin：空安全
来源：http://gxd.ywan-chungtsiang.top

val n: String? = null;  n?.length
来源：http://meg.ivvv.top

[T05] Kotlin：when 表达式
来源：http://nqa.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nwg.fktsv.cn

[T06] Kotlin：集合映射
来源：http://pbb.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://gho.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://vjr.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dmb.zdbjq.cn

[T08] Kotlin：数据类
来源：http://pvt.yj202588.top

data class User(val name: String, val age: Int)
来源：http://ihq.ybcxt.top

[T09] Kotlin：扩展函数
来源：http://yfv.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://btr.tarul.cn

[T10] Kotlin：默认参数
来源：http://rdp.hongshengwenyu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jem.yuanzhike.top

[T11] Kotlin：协程
来源：http://cwo.kuanghao11.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zjp.yonumen.top

[T12] Kotlin：解构声明
来源：http://eos.wangshuangyany.cn

val (a, b) = Pair(1, 2)
来源：http://yfv.shzxlz.cn

[T13] Kotlin：只读 Map
来源：http://wnb.hammf.cn

val m = mapOf("a" to 1)
来源：http://dub.jianghu66.top

[T14] Kotlin：循环
来源：http://fxb.nwbrower.top

for (i in 1..10) println(i)
来源：http://jda.zhijiandao.cn

[T15] Kotlin：接口
来源：http://lye.cucudq.cn

interface Shape { fun area(): Double }
来源：http://mni.yangfankeji.com

[T16] Swift：Hello World
来源：http://jpm.yfazqb.com

print("Hello")
来源：http://ivv.ydzc1.top

[T17] Swift：变量与常量
来源：http://arw.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://qif.aibaodan.cn

[T18] Swift：字符串插值
来源：http://viu.chenzaomai.com

"值: \(b)"
来源：http://qzf.yongpay.top

[T19] Swift：可选绑定
来源：http://zca.aibaodan.cn

if let n = opt { print(n) }
来源：http://nmx.gogol.net.cn

[T20] Swift：数组操作
来源：http://azc.jiagoushi.top

var a = [1, 2, 3];  a.append(4)
来源：http://wdt.hnqzz.top

[T21] Swift：遍历
来源：http://gmk.jqgufenzy.top

for x in a { print(x) }
来源：http://gdo.ybcxt.top

[T22] Swift：字典
来源：http://nuf.andypj.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://dlc.hywenlv.cn

[T23] Swift：函数
来源：http://dps.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jbf.andypj.xyz

[T24] Swift：闭包
来源：http://yxm.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://uhy.xuetiantiany.cn

[T25] Swift：结构体
来源：http://wpu.shzxlz.cn

struct P { var x: Int }
来源：http://bit.hesvh.cn

[T26] Swift：类与重写
来源：http://bwb.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://eox.yj20258888.top

[T27] Swift：错误处理
来源：http://crc.tian-w.cn

do { try f() } catch { print(error) }
来源：http://ark.guowangkeji.top

[T28] Swift：枚举
来源：http://iwt.chenzaomai.com

enum Color { case red, green }
来源：http://dur.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://pur.tianlin.xyz

guard let x = opt else { return }
来源：http://vxx.vehdjk.com

[T30] Swift：协议
来源：http://cri.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://tgf.ywan-chungtsiang.top

[T31] Lua：Hello World
来源：http://ajq.xingfuxueyuan.xyz

print("Hello")
来源：http://efk.jlsjyb.cn

[T32] Lua：局部变量
来源：http://vqw.jqgufenzy.top

local a = 1
来源：http://bnc.havefunace.top

[T33] Lua：表（数组）
来源：http://epp.jinqigfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://szi.cashguo.top

[T34] Lua：遍历表
来源：http://inn.guannengcc.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zhb.hesvh.cn

[T35] Lua：字典表
来源：http://cwk.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://zjc.hnqzz.top

[T36] Lua：函数
来源：http://fyf.ppjwa.cn

function add(a, b) return a + b end
来源：http://lvb.fanxiaobao.xyz

[T37] Lua：字符串拼接
来源：http://wpe.nwbrower.top

"a" .. "b"
来源：http://agg.chenzaomai.com

[T38] Lua：条件
来源：http://dna.hfpthk.cn

if x > 0 then print("正") end
来源：http://hgj.aizwys.cn

[T39] Lua：模式匹配
来源：http://jsi.sweek.top

string.find(s, "%d+")
来源：http://iqx.kuanghao11.cn

[T40] Lua：元表
来源：http://epl.sufxvd.cn

setmetatable({}, { __index = base })
来源：http://ymr.shanyushiyangtech.top

[T41] Perl：Hello World
来源：http://sud.xylfe.cn

print "Hello\n";
来源：http://fqp.hysaishi.cn

[T42] Perl：变量类型
来源：http://wdh.xylfe.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ouy.ybcxt.top

[T43] Perl：字符串插值
来源：http://jcm.vqdsnc.cn

"值: $a"
来源：http://ozh.jinghuilouyu.cn

[T44] Perl：条件
来源：http://bor.yangfankeji.com

if ($a > 0) { print "正"; }
来源：http://nvg.tanke756.top

[T45] Perl：数组遍历
来源：http://mcb.fzhhl.top

for my $x (@arr) { print $x; }
来源：http://ejs.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://vkb.iojbl.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jzt.uphjek.com

[T47] Perl：正则捕获
来源：http://cdq.yonumen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zsj.yuanzhike.top

[T48] Perl：正则替换
来源：http://moe.nanxuanxn.top

$s =~ s/old/new/g;
来源：http://oxw.xylfe.cn

[T49] Perl：函数
来源：http://mvz.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cng.pengpengdd.cyou

[T50] Perl：逐行读文件
来源：http://edd.birdmap.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ywm.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://cmy.cdnleiting.top

[T51] Scala：Hello World
来源：http://nnn.xinyue.icu

println("Hello")
来源：http://xcn.guannengcc.top

[T52] Scala：变量
来源：http://iny.hysaishi.cn

val a = 1;  var b = 2
来源：http://qez.gaohongyu789.top

[T53] Scala：字符串插值
来源：http://iyb.redwolf501.top

s"值: $b"
来源：http://stv.hywenlv.cn

[T54] Scala：集合映射
来源：http://ata.smart0.xyz

List(1, 2, 3).map(_ * 2)
来源：http://wey.ywan-chungtsiang.top

[T55] Scala：集合过滤
来源：http://chw.yfazqb.com

List(1, 2, 3).filter(_ > 1)
来源：http://cjk.ppjwa.cn

[T56] Scala：样例类
来源：http://uvr.0kj1m.cn

case class User(name: String, age: Int)
来源：http://kvc.cdnleiting.top

[T57] Scala：模式匹配
来源：http://pue.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://vvs.jqgufenzy.top

[T58] Scala：函数定义
来源：http://ahr.jinyuanbaomall.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hnc.yj20258.top

[T59] Scala：循环
来源：http://xuq.hongshengwenyu.top

for (i <- 1 to 10) println(i)
来源：http://qte.dashuyun.cn

[T60] Scala：折叠
来源：http://elr.tianlin.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://onm.xuanzx.com

================================================================================
来源：http://sjr.aibaodan.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://szg.zdqjudy.top

================================================================================
来源：http://tno.yfazqb.com

[U01] Py：创建虚拟环境
来源：http://qkl.xinyue.icu

python -m venv .venv && source .venv/bin/activate
来源：http://kyh.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://xhe.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xze.shanyushiyangtech.top

[U03] Py：加载 .env 配置
来源：http://iev.fanxiaobao.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://azn.yj20258888.top

[U04] Py：变量调试打印
来源：http://jkv.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dwr.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://mho.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://bda.daxiang520.top

[U06] Py：合并两个字典
来源：http://evg.0kj1m.cn

{**a, **b}
来源：http://bvn.daxiang520.top

[U07] Py：反转字典键值
来源：http://mbe.yfazqb.com

{v: k for k, v in d.items()}
来源：http://zcv.zycfv.cn

[U08] Py：展平二维列表
来源：http://kdo.snrcjt.cn

[y for x in nested for y in x]
来源：http://yuz.yj20258888.top

[U09] Py：字典取最大值的键
来源：http://zex.zhiwuduotai.top

max(d, key=d.get)
来源：http://iou.shanyushiyangtech.top

[U10] Py：按值排序字典
来源：http://awi.jinqigufen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://agc.yuanzhike.top

[U11] Py：生成器表达式
来源：http://fkj.hfpthk.cn

(x * 2 for x in arr)
来源：http://frd.ydzc1.top

[U12] Py：取出现最多的 3 个元素
来源：http://bjx.hnqzz.top

Counter(arr).most_common(3)
来源：http://szp.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://cgd.snrcjt.cn

deque(maxlen=10)
来源：http://kjd.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://eux.xylfe.cn

defaultdict(list)
来源：http://uxw.guannengcc.top

[U15] Py：高精度计时
来源：http://pzv.jqgfzy.top

t = time.perf_counter()
来源：http://hkz.gaohongyu789.top

[U16] Py：命令行参数解析
来源：http://joj.jinghuilouyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bsf.jianghu66.top

[U17] Py：初始化日志
来源：http://qvf.havefunace.top

logging.basicConfig(level=logging.INFO)
来源：http://znf.yuxming.cn

[U18] Py：预编译正则
来源：http://wsq.bjfxy.top

pat = re.compile(r"\d+")
来源：http://znb.birdmap.top


<!-- 参考信息 -->