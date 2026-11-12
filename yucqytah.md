代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://gvk.ppjwa.cn

[R72] 等待端口就绪
来源：http://puh.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eyv.cdnleiting.top

[R73] 分割大日志
来源：http://eho.nanxinkj.top

split -l 1000 big.log part_
来源：http://irq.yuxming.cn

[R74] 批量重命名
来源：http://cpz.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blc.sxryk.cn

[R75] 导出环境变量
来源：http://mfn.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://imt.redwolf501.top

[R76] 使用临时文件
来源：http://qsr.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iew.chenzaomai.com

[R77] 读取用户输入
来源：http://omd.xziqi.cn

read -rp "请输入: " ans
来源：http://ikq.fengsongda.top

[R78] 交互式菜单
来源：http://pcf.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mtw.birdmap.top

[R79] 解析命令行选项
来源：http://zbn.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ljf.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://whh.hesvh.cn

time ./run.sh
来源：http://tjv.yuxming.cn

================================================================================
来源：http://qxg.pycfn.com

S. C / C++ 专题
来源：http://fnh.pycfn.com

================================================================================
来源：http://epx.sweek.top

[S01] C：Hello World
来源：http://lyc.c1oappe.top

#include <stdio.h>
来源：http://iey.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://pzn.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://obd.havefunace.top

int a = 10; printf("%d\n", a);
来源：http://mse.jlsjyb.cn

[S03] C：读入整数
来源：http://von.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://yfg.fehbvm.com

[S04] C：字符串复制
来源：http://kom.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://ixu.zycfv.cn

[S05] C：字符串长度
来源：http://wuu.yanxiufei.cn

strlen(s)
来源：http://qnq.jianghu66.top

[S06] C：字符串比较
来源：http://bda.shzxlz.cn

strcmp(a, b) == 0
来源：http://nog.redwolf501.top

[S07] C：数组遍历求和
来源：http://pvh.yuanzhike.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kmk.dashuyun.cn

[S08] C：动态内存分配与释放
来源：http://ygc.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ezt.cdnleiting.top

[S09] C：结构体定义与初始化
来源：http://jqg.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wfa.aibaodan.cn

[S10] C：指针与解引用
来源：http://tgn.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://lkf.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://tlz.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://oyq.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uim.cheryme.top

fclose(f);
来源：http://lnl.fehbvm.com

[S12] C：写文件
来源：http://wuy.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://axb.zhixingplan.top

[S13] C：宏定义
来源：http://goa.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://odi.tarul.cn

[S14] C：枚举
来源：http://xym.nanxinkj.top

enum Color { RED, GREEN, BLUE };
来源：http://fsq.zdqjudy.top

[S15] C：类型转换
来源：http://jyg.nanxuanxn.top

(double) a / b
来源：http://znu.quarkkingdee.top

[S16] C：位操作置位
来源：http://xuw.fanxiaobao.xyz

x |= (1 << 3);
来源：http://gqs.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://iop.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ppg.dianchejie.cn

[S18] C：命令行参数
来源：http://skn.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://nom.yueranfly.top

[S19] C：快速排序
来源：http://qun.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://whb.dianchejie.cn

[S20] C：二分查找
来源：http://wwf.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nvf.sxryk.cn

[S21] C：字符类别判断
来源：http://zxb.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cqo.ppjwa.cn

[S22] C：字符串转数字
来源：http://jyh.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cum.daria6918.cn

[S23] C：随机数
来源：http://rii.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://auo.chenzaomai.com

[S24] C：获取本地时间
来源：http://ktg.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rjw.sxryk.cn

[S25] C：内存拷贝
来源：http://fbi.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://ytc.yj202588.top

[S26] C：内存清零
来源：http://lhc.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://pce.chenzaomai.com

[S27] C：定义常量
来源：http://mft.zhixingplan.top

const double PI = 3.14159;
来源：http://yfs.fehbvm.com

[S28] C：静态变量
来源：http://pwp.jinghuilouyu.cn

static int counter = 0;
来源：http://eak.quarkkingdee.top

[S29] C：变参函数
来源：http://gxt.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hpl.xuetiantiany.cn

[S30] C：头文件保护
来源：http://ymv.xylfe.cn

#ifndef X_H
来源：http://pii.hfpthk.cn

#define X_H
来源：http://ade.sjlbkw.cn

#endif
来源：http://tbe.quarkkingdee.top

[S31] C++：Hello World
来源：http://utg.cheryme.top

#include <iostream>
来源：http://wjo.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://osi.yueranfly.top

[S32] C++：字符串
来源：http://lyo.wangdashe.top

std::string s = "hi";  s += "!";
来源：http://tex.daxiang520.top

[S33] C++：vector 增删
来源：http://inc.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jyy.hesvh.cn

[S34] C++：遍历 vector
来源：http://rnd.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://jka.aibaodan.cn

[S35] C++：map
来源：http://yuy.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oxx.9152youxi.cn

[S36] C++：unordered_map
来源：http://qau.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xau.xuanzx.com

[S37] C++：set
来源：http://yat.zhiwuduotai.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zgk.jinghuilouyu.cn

[S38] C++：排序
来源：http://xfy.hcnkem.com

std::sort(v.begin(), v.end());
来源：http://gte.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://eiv.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://byk.9152youxi.cn

[S40] C++：查找元素
来源：http://nzq.cucudq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hpl.cdnleiting.top

[S41] C++：类与构造函数
来源：http://yma.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zjk.cucudq.cn

[S42] C++：继承与虚函数
来源：http://ysx.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://koj.bbcook.cn

[S43] C++：智能指针
来源：http://cpa.fanxiaobao.xyz

auto p = std::make_unique<int>(5);
来源：http://fqq.redwolf501.top

[S44] C++：引用传参
来源：http://wvq.xuanzx.com

void inc(int &x) { ++x; }
来源：http://elb.guannengcc.top

[S45] C++：lambda
来源：http://yqk.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://lzv.aizwys.cn

[S46] C++：函数模板
来源：http://oid.guannengcc.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uva.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://efl.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qvz.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://wct.svipenyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://izh.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://nyu.9152youxi.cn

[S49] C++：写文件
来源：http://gau.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://efh.yj20258.top

[S50] C++：格式化数字
来源：http://mlm.jlsjyb.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lto.jianghu66.top

[S51] C++：显式类型转换
来源：http://jyf.c1oappe.top

static_cast<double>(a) / b
来源：http://pyz.svipenyu.cn

[S52] C++：const 与 noexcept
来源：http://own.tian-w.cn

int size() const noexcept { return n_; }
来源：http://kiu.xinyue.icu

[S53] C++：移动语义
来源：http://wgu.yvedp.cn

std::vector<int> w = std::move(v);
来源：http://hja.guowangkeji.top

[S54] C++：异常处理
来源：http://wmm.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vzy.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://utp.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://his.sjlbkw.cn

[S56] C++：optional
来源：http://ktc.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kcv.aizwys.cn

[S57] C++：编译期常量
来源：http://cno.yueranfly.top

constexpr int N = 10;
来源：http://ehs.ivvv.top

[S58] C++：命名空间
来源：http://yhb.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://mkc.zhongyouzk.top

[S59] C++：静态断言
来源：http://lpl.hcnkem.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lxl.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://ali.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xlb.dashuyun.cn

================================================================================
来源：http://bbr.gogol.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gtt.jlsjyb.cn

================================================================================
来源：http://ywl.0kj1m.cn

[T01] Kotlin：Hello World
来源：http://zqu.ybcxt.top

println("Hello")
来源：http://jod.vehdjk.com

[T02] Kotlin：变量
来源：http://zvl.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jqo.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://cdx.hcnkem.com

"值: $b"
来源：http://dxt.yongpay.top

[T04] Kotlin：空安全
来源：http://lol.cheryme.top

val n: String? = null;  n?.length
来源：http://zxv.jqgufenzy.top

[T05] Kotlin：when 表达式
来源：http://xlu.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pty.yanxiufei.cn

[T06] Kotlin：集合映射
来源：http://mks.birdmap.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qcx.jinqigfzy.top

[T07] Kotlin：集合过滤
来源：http://etc.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tdv.yongpay.top

[T08] Kotlin：数据类
来源：http://vca.yongpay.top

data class User(val name: String, val age: Int)
来源：http://fjz.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://kmf.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://anf.havefunace.top

[T10] Kotlin：默认参数
来源：http://fnv.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://crw.pycfn.com

[T11] Kotlin：协程
来源：http://lwc.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wzh.vqdsnc.cn

[T12] Kotlin：解构声明
来源：http://fjd.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://fmn.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://mfq.ivvv.top

val m = mapOf("a" to 1)
来源：http://sdm.bjfxy.top

[T14] Kotlin：循环
来源：http://nnl.ybcxt.top

for (i in 1..10) println(i)
来源：http://awe.pengpengdd.cyou

[T15] Kotlin：接口
来源：http://orb.zycfv.cn

interface Shape { fun area(): Double }
来源：http://nvf.yangfankeji.com

[T16] Swift：Hello World
来源：http://stz.nanxuanxn.top

print("Hello")
来源：http://tgf.xziqi.cn

[T17] Swift：变量与常量
来源：http://kdt.kuanghao11.cn

var a = 1;  let b = 2
来源：http://sjq.fehbvm.com

[T18] Swift：字符串插值
来源：http://jab.shanyushiyangtech.top

"值: \(b)"
来源：http://mtc.hammf.cn

[T19] Swift：可选绑定
来源：http://lll.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://hds.sxryk.cn

[T20] Swift：数组操作
来源：http://jji.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://mok.yj20258.top

[T21] Swift：遍历
来源：http://xez.chenjidiqi.icu

for x in a { print(x) }
来源：http://fks.sxryk.cn

[T22] Swift：字典
来源：http://oux.yfazqb.com

var d = ["a": 1];  d["b"] = 2
来源：http://hzf.xylfe.cn

[T23] Swift：函数
来源：http://vcp.jinghuilouyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nyq.tarul.cn

[T24] Swift：闭包
来源：http://tfl.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://snl.hesvh.cn

[T25] Swift：结构体
来源：http://vpt.fzhhl.top

struct P { var x: Int }
来源：http://zpm.zhongyouzk.top

[T26] Swift：类与重写
来源：http://acs.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://hwr.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://dxq.dashuyun.cn

do { try f() } catch { print(error) }
来源：http://odq.jinghuilouyu.cn

[T28] Swift：枚举
来源：http://saw.jqgufenzy.top

enum Color { case red, green }
来源：http://ueb.aibaodan.cn

[T29] Swift：guard 提前返回
来源：http://llu.shzxlz.cn

guard let x = opt else { return }
来源：http://foy.gogol.net.cn

[T30] Swift：协议
来源：http://knj.hcnkem.com

protocol Shape { func area() -> Double }
来源：http://yro.cqqwz.cn

[T31] Lua：Hello World
来源：http://qkj.sufxvd.cn

print("Hello")
来源：http://nmj.birdmap.top

[T32] Lua：局部变量
来源：http://hjc.hysaishi.cn

local a = 1
来源：http://vfc.yuxming.cn

[T33] Lua：表（数组）
来源：http://rhw.kuanghao11.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://srv.hongshengwenyu.top

[T34] Lua：遍历表
来源：http://kck.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://obb.smart0.xyz

[T35] Lua：字典表
来源：http://zai.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://zps.yuxming.cn

[T36] Lua：函数
来源：http://hrt.chenjidiqi.icu

function add(a, b) return a + b end
来源：http://ruf.pycfn.com

[T37] Lua：字符串拼接
来源：http://yiw.316326.xyz

"a" .. "b"
来源：http://xen.yangfankeji.com

[T38] Lua：条件
来源：http://epg.aibaodan.cn

if x > 0 then print("正") end
来源：http://osy.hywenlv.cn

[T39] Lua：模式匹配
来源：http://axq.quarkkingdee.top

string.find(s, "%d+")
来源：http://bzt.jqgufenzy.top

[T40] Lua：元表
来源：http://jsi.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://lgd.xziqi.cn

[T41] Perl：Hello World
来源：http://pzp.nanxuanxn.top

print "Hello\n";
来源：http://fbe.redwolf501.top

[T42] Perl：变量类型
来源：http://oqk.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ini.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://qvh.yvedp.cn

"值: $a"
来源：http://sqi.jqgufenzy.top

[T44] Perl：条件
来源：http://din.hesvh.cn

if ($a > 0) { print "正"; }
来源：http://ztv.bjfxy.top

[T45] Perl：数组遍历
来源：http://otg.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://ecc.mhx1999.top

[T46] Perl：哈希操作
来源：http://wna.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sqb.ydzc1.top

[T47] Perl：正则捕获
来源：http://txk.zhixingplan.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wxd.zhiwuduotai.top

[T48] Perl：正则替换
来源：http://lpt.shanyushiyangkeji.top

$s =~ s/old/new/g;
来源：http://abm.zhixingplan.top

[T49] Perl：函数
来源：http://xmu.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lch.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://tyd.vehdjk.com

open my $fh, "<", "a.txt" or die $!;
来源：http://jum.yj20258888.top

while (my $line = <$fh>) { print $line; }
来源：http://skr.zdqjudy.top

[T51] Scala：Hello World
来源：http://kfp.feifeiyinyue.top

println("Hello")
来源：http://ttv.bjfxy.top

[T52] Scala：变量
来源：http://kjj.hammf.cn

val a = 1;  var b = 2
来源：http://ecc.ybcxt.top

[T53] Scala：字符串插值
来源：http://eyl.aizwys.cn

s"值: $b"
来源：http://alm.hnxiangtu.top

[T54] Scala：集合映射
来源：http://giq.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://plj.hnqzz.top

[T55] Scala：集合过滤
来源：http://ela.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://fly.zdqjudy.top

[T56] Scala：样例类
来源：http://ffu.hcnkem.com

case class User(name: String, age: Int)
来源：http://zjz.yj202588.top

[T57] Scala：模式匹配
来源：http://xyd.shuidangran.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pjq.jqgfzy.top

[T58] Scala：函数定义
来源：http://nba.cqqwz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vwb.uphjek.com

[T59] Scala：循环
来源：http://goy.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://cfq.yuanzhike.top

[T60] Scala：折叠
来源：http://eoc.yangfankeji.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://snt.sufxvd.cn

================================================================================
来源：http://czq.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ohg.jyoumei.cn

================================================================================
来源：http://udj.cheryme.top

[U01] Py：创建虚拟环境
来源：http://aou.ybcxt.top

python -m venv .venv && source .venv/bin/activate
来源：http://dhj.andypj.xyz

[U02] Py：导出 / 安装依赖
来源：http://wtu.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://agp.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://qlh.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jfp.hcnkem.com

[U04] Py：变量调试打印
来源：http://csc.cheryme.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wlu.hywenlv.cn

[U05] Py：列表去重且保序
来源：http://nic.dashuyun.cn

list(dict.fromkeys(arr))
来源：http://vmk.shuidangran.top

[U06] Py：合并两个字典
来源：http://xkd.jyoumei.cn

{**a, **b}
来源：http://tke.shuidangran.top

[U07] Py：反转字典键值
来源：http://ywu.cheryme.top

{v: k for k, v in d.items()}
来源：http://tsr.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://gmj.52xcode.cn

[y for x in nested for y in x]
来源：http://qtc.yvedp.cn

[U09] Py：字典取最大值的键
来源：http://ksb.tian-w.cn

max(d, key=d.get)
来源：http://hqj.uphjek.com

[U10] Py：按值排序字典
来源：http://sau.jinqigufen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hpl.yfazqb.com

[U11] Py：生成器表达式
来源：http://nla.gotoacloud.top

(x * 2 for x in arr)
来源：http://idw.jinqigfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://ecr.guannengcc.top

Counter(arr).most_common(3)
来源：http://bnu.daxiang520.top


<!-- 参考信息 -->