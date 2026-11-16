代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://giz.yj202588.top

[R72] 等待端口就绪
来源：http://lgo.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ijd.yueranfly.top

[R73] 分割大日志
来源：http://mqj.vqdsnc.cn

split -l 1000 big.log part_
来源：http://vvs.guannengcc.top

[R74] 批量重命名
来源：http://kqt.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nts.kuanghao11.cn

[R75] 导出环境变量
来源：http://sdz.zhixingplan.top

export PATH="$HOME/bin:$PATH"
来源：http://wzb.jqgufenzy.top

[R76] 使用临时文件
来源：http://ghv.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cdi.xuanzx.com

[R77] 读取用户输入
来源：http://qxd.ydzc1.top

read -rp "请输入: " ans
来源：http://rwi.daria6918.cn

[R78] 交互式菜单
来源：http://nrl.jinqigfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jep.quarkkingdee.top

[R79] 解析命令行选项
来源：http://lyw.zhixingplan.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mbr.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://akd.fengsongda.top

time ./run.sh
来源：http://hwt.sweek.top

================================================================================
来源：http://rgo.yj202588.top

S. C / C++ 专题
来源：http://tqc.shangyingyoupin.top

================================================================================
来源：http://xkv.xylfe.cn

[S01] C：Hello World
来源：http://sfy.chenzaomai.com

#include <stdio.h>
来源：http://nnq.chenlongwang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://aaf.yueranfly.top

[S02] C：变量与格式化输出
来源：http://gnb.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://geq.sufxvd.cn

[S03] C：读入整数
来源：http://ivd.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://ruz.xingfuxueyuan.xyz

[S04] C：字符串复制
来源：http://zjl.zhijiandao.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gss.tarul.cn

[S05] C：字符串长度
来源：http://srg.xinyue.icu

strlen(s)
来源：http://mvr.xinyue.icu

[S06] C：字符串比较
来源：http://zec.cqqwz.cn

strcmp(a, b) == 0
来源：http://ofc.jinqigfzy.top

[S07] C：数组遍历求和
来源：http://mpe.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cvf.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://sfh.gaohongyu789.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vho.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://tuk.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zqm.hfpthk.cn

[S10] C：指针与解引用
来源：http://ecb.cucudq.cn

int *p = &a;  *p = 5;
来源：http://rfs.gogol.net.cn

[S11] C：逐行读文件
来源：http://kae.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://ddz.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cik.jyoumei.cn

fclose(f);
来源：http://meu.jinqigufen.top

[S12] C：写文件
来源：http://gia.cheryme.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fma.c1oappe.top

[S13] C：宏定义
来源：http://vfe.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://whb.ppjwa.cn

[S14] C：枚举
来源：http://nvk.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://kuf.zhixingplan.top

[S15] C：类型转换
来源：http://sth.jyoumei.cn

(double) a / b
来源：http://ilc.zhoulong.xyz

[S16] C：位操作置位
来源：http://yfj.chenzaomai.com

x |= (1 << 3);
来源：http://ckt.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://ybt.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zmo.tian-w.cn

[S18] C：命令行参数
来源：http://bkr.sweek.top

int main(int argc, char **argv)
来源：http://kju.shangyingyoupin.top

[S19] C：快速排序
来源：http://qhz.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tgn.mhx1999.top

[S20] C：二分查找
来源：http://vzp.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cck.fktsv.cn

[S21] C：字符类别判断
来源：http://dvg.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zlt.ctjpmb.com

[S22] C：字符串转数字
来源：http://kny.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://cuy.hywenlv.cn

[S23] C：随机数
来源：http://mnx.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dlw.zhixingplan.top

[S24] C：获取本地时间
来源：http://mvm.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jqf.hfpthk.cn

[S25] C：内存拷贝
来源：http://stl.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://wkj.wangshuangyany.cn

[S26] C：内存清零
来源：http://rdj.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://bwi.meibo888.top

[S27] C：定义常量
来源：http://jpo.xuetiantiany.cn

const double PI = 3.14159;
来源：http://sxr.yj20258.top

[S28] C：静态变量
来源：http://xfq.yongpay.top

static int counter = 0;
来源：http://yum.gogol.net.cn

[S29] C：变参函数
来源：http://lkd.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://myk.jqgufenzy.top

[S30] C：头文件保护
来源：http://ykj.hongshengwenyu.top

#ifndef X_H
来源：http://ahr.hongshengwenyu.top

#define X_H
来源：http://vqb.jinghuilouyu.cn

#endif
来源：http://xyd.sjlbkw.cn

[S31] C++：Hello World
来源：http://kjx.xylfe.cn

#include <iostream>
来源：http://mir.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://yzv.hnxiangtu.top

[S32] C++：字符串
来源：http://udd.sweek.top

std::string s = "hi";  s += "!";
来源：http://cnr.svipenyu.cn

[S33] C++：vector 增删
来源：http://fdq.aibaodan.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://akw.yuxming.cn

[S34] C++：遍历 vector
来源：http://xlv.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://ota.yvedp.cn

[S35] C++：map
来源：http://nbm.yongpay.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qxv.tianlin.xyz

[S36] C++：unordered_map
来源：http://gvo.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pvi.hfpthk.cn

[S37] C++：set
来源：http://zua.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kfn.aibaodan.cn

[S38] C++：排序
来源：http://tan.yongpay.top

std::sort(v.begin(), v.end());
来源：http://bih.jiagoushi.top

[S39] C++：自定义比较器排序
来源：http://nho.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gyk.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://bxn.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lwa.jinqigfzy.top

[S41] C++：类与构造函数
来源：http://ikv.bjfxy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://btm.sweek.top

[S42] C++：继承与虚函数
来源：http://bvn.xinyue.icu

class B : public Base { public: void f() override {} };
来源：http://qiy.yfazqb.com

[S43] C++：智能指针
来源：http://ggh.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://fak.wangdashe.top

[S44] C++：引用传参
来源：http://itr.mhx1999.top

void inc(int &x) { ++x; }
来源：http://iyw.yanxiufei.cn

[S45] C++：lambda
来源：http://bvd.jinqigfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://qmf.hfpthk.cn

[S46] C++：函数模板
来源：http://rry.dianchejie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zzj.shanyushiyangkeji.top

[S47] C++：结构化绑定遍历
来源：http://xie.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ibj.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://hgl.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://xla.ydzc1.top

while (std::getline(in, line)) { }
来源：http://xid.yonumen.top

[S49] C++：写文件
来源：http://wuy.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cql.mhx1999.top

[S50] C++：格式化数字
来源：http://imj.redwolf501.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tyw.shuidangran.top

[S51] C++：显式类型转换
来源：http://dbs.jiagoushi.top

static_cast<double>(a) / b
来源：http://cxz.zhoulong.xyz

[S52] C++：const 与 noexcept
来源：http://krk.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://uxn.shanyushiyangkeji.top

[S53] C++：移动语义
来源：http://qbj.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://bzn.daxiang520.top

[S54] C++：异常处理
来源：http://azv.yueranfly.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fwh.haohaochexian.top

[S55] C++：结构化绑定
来源：http://whc.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://byq.vehdjk.com

[S56] C++：optional
来源：http://ciw.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wnq.gogol.net.cn

[S57] C++：编译期常量
来源：http://jil.ctjpmb.com

constexpr int N = 10;
来源：http://jte.guowangkeji.top

[S58] C++：命名空间
来源：http://yxf.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://yea.yonumen.top

[S59] C++：静态断言
来源：http://ufx.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://usk.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://pja.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://spk.zhaomingkeji.xyz

================================================================================
来源：http://yfi.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bdq.birdmap.top

================================================================================
来源：http://tfr.yj20258888.top

[T01] Kotlin：Hello World
来源：http://ips.ppjwa.cn

println("Hello")
来源：http://mbk.yueranfly.top

[T02] Kotlin：变量
来源：http://kop.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://var.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://hax.snrcjt.cn

"值: $b"
来源：http://pkf.zdqjudy.top

[T04] Kotlin：空安全
来源：http://irx.yfazqb.com

val n: String? = null;  n?.length
来源：http://iea.vehdjk.com

[T05] Kotlin：when 表达式
来源：http://def.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ohy.redwolf501.top

[T06] Kotlin：集合映射
来源：http://tgw.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qtz.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://nue.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://plp.shangyingyoupin.top

[T08] Kotlin：数据类
来源：http://kns.andypj.xyz

data class User(val name: String, val age: Int)
来源：http://kgr.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://kng.yj20258.top

fun String.exclaim() = this + "!"
来源：http://eew.zhijiandao.cn

[T10] Kotlin：默认参数
来源：http://hrn.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://stp.tanke756.top

[T11] Kotlin：协程
来源：http://vav.0kj1m.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zng.ehwqpu.com

[T12] Kotlin：解构声明
来源：http://qdh.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://euk.yongpay.top

[T13] Kotlin：只读 Map
来源：http://rvo.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://akj.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://nrs.0kj1m.cn

for (i in 1..10) println(i)
来源：http://ceu.aizwys.cn

[T15] Kotlin：接口
来源：http://dpl.jlsjyb.cn

interface Shape { fun area(): Double }
来源：http://jjc.aibaodan.cn

[T16] Swift：Hello World
来源：http://sjl.nanxuanxn.top

print("Hello")
来源：http://ddr.tarul.cn

[T17] Swift：变量与常量
来源：http://zuh.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://ege.zdqjudy.top

[T18] Swift：字符串插值
来源：http://aja.cucudq.cn

"值: \(b)"
来源：http://ppu.yj202588.top

[T19] Swift：可选绑定
来源：http://lfd.316326.xyz

if let n = opt { print(n) }
来源：http://nwt.zhiwuduotai.top

[T20] Swift：数组操作
来源：http://wje.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://mqb.daxiang520.top

[T21] Swift：遍历
来源：http://qen.aibaodan.cn

for x in a { print(x) }
来源：http://gce.zhiwuduotai.top

[T22] Swift：字典
来源：http://fni.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://anl.zhixingplan.top

[T23] Swift：函数
来源：http://wgh.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lmr.chenlongwang.top

[T24] Swift：闭包
来源：http://cia.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rbu.52xcode.cn

[T25] Swift：结构体
来源：http://nkk.shuidangran.top

struct P { var x: Int }
来源：http://vms.dashuyun.cn

[T26] Swift：类与重写
来源：http://fdn.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://edt.ydjk.org.cn

[T27] Swift：错误处理
来源：http://rnv.jianghu66.top

do { try f() } catch { print(error) }
来源：http://ika.tarul.cn

[T28] Swift：枚举
来源：http://bmd.haohaochexian.top

enum Color { case red, green }
来源：http://hqp.sjlbkw.cn

[T29] Swift：guard 提前返回
来源：http://squ.zhengqikj.top

guard let x = opt else { return }
来源：http://yji.cheryme.top

[T30] Swift：协议
来源：http://qgx.kuanghao11.cn

protocol Shape { func area() -> Double }
来源：http://cit.zycfv.cn

[T31] Lua：Hello World
来源：http://exz.yongpay.top

print("Hello")
来源：http://etw.zhiwuduotai.top

[T32] Lua：局部变量
来源：http://upn.xuetiantiany.cn

local a = 1
来源：http://xcg.yfazqb.com

[T33] Lua：表（数组）
来源：http://sfp.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://qwz.316326.xyz

[T34] Lua：遍历表
来源：http://bte.shanyushiyangtech.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bbg.ctjpmb.com

[T35] Lua：字典表
来源：http://vkm.zycfv.cn

local d = { a = 1 };  d.b = 2
来源：http://cli.jiagoushi.top

[T36] Lua：函数
来源：http://qol.dashuyun.cn

function add(a, b) return a + b end
来源：http://nkt.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://cjc.hesvh.cn

"a" .. "b"
来源：http://qse.uphjek.com

[T38] Lua：条件
来源：http://fee.svipenyu.cn

if x > 0 then print("正") end
来源：http://izn.gotoacloud.top

[T39] Lua：模式匹配
来源：http://znb.jlsjyb.cn

string.find(s, "%d+")
来源：http://zgj.hnqzz.top

[T40] Lua：元表
来源：http://ptx.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://fqt.kuanghao11.cn

[T41] Perl：Hello World
来源：http://jqb.pengpengdd.cyou

print "Hello\n";
来源：http://qti.yuanzhike.top

[T42] Perl：变量类型
来源：http://yce.ivvv.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jdp.yj20258.top

[T43] Perl：字符串插值
来源：http://uni.cheryme.top

"值: $a"
来源：http://whu.guannengcc.top

[T44] Perl：条件
来源：http://cwb.xuanzx.com

if ($a > 0) { print "正"; }
来源：http://fvn.c1oappe.top

[T45] Perl：数组遍历
来源：http://ffx.zhongyouzk.top

for my $x (@arr) { print $x; }
来源：http://ccm.gaohongyu789.top

[T46] Perl：哈希操作
来源：http://jdm.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vrs.52xcode.cn

[T47] Perl：正则捕获
来源：http://mmn.c1oappe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dlv.hfpthk.cn

[T48] Perl：正则替换
来源：http://xxs.meibo888.top

$s =~ s/old/new/g;
来源：http://uqs.nanxinkj.top

[T49] Perl：函数
来源：http://nbi.iojbl.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wok.chenjidiqi.icu

[T50] Perl：逐行读文件
来源：http://gso.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bfp.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://xgf.yuxming.cn

[T51] Scala：Hello World
来源：http://tpf.hysaishi.cn

println("Hello")
来源：http://haq.aibaodan.cn

[T52] Scala：变量
来源：http://shi.jianghu66.top

val a = 1;  var b = 2
来源：http://qxp.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://oop.jlsjyb.cn

s"值: $b"
来源：http://nsy.fehbvm.com

[T54] Scala：集合映射
来源：http://poh.smart0.xyz

List(1, 2, 3).map(_ * 2)
来源：http://zmo.xingfuxueyuan.xyz

[T55] Scala：集合过滤
来源：http://tqq.chenjidiqi.icu

List(1, 2, 3).filter(_ > 1)
来源：http://dtm.mhx1999.top

[T56] Scala：样例类
来源：http://fdl.jianghu66.top

case class User(name: String, age: Int)
来源：http://ens.daria6918.cn

[T57] Scala：模式匹配
来源：http://vjj.svipenyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mzt.c1oappe.top

[T58] Scala：函数定义
来源：http://xur.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://kgs.vehdjk.com

[T59] Scala：循环
来源：http://lwy.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://fhw.9152youxi.cn

[T60] Scala：折叠
来源：http://frd.tanke756.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yon.fanxiaobao.xyz

================================================================================
来源：http://fiz.cucudq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zdg.xinyue.icu

================================================================================
来源：http://onj.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://ifd.vqdsnc.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ksm.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://pbf.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uqx.yj20258.top

[U03] Py：加载 .env 配置
来源：http://plz.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ehg.ybcxt.top

[U04] Py：变量调试打印
来源：http://jqu.316326.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cbk.vqdsnc.cn

[U05] Py：列表去重且保序
来源：http://yft.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://hsv.c1oappe.top

[U06] Py：合并两个字典
来源：http://chm.zhiwuduotai.top

{**a, **b}
来源：http://uhm.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://pkt.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://ody.ywan-chungtsiang.top

[U08] Py：展平二维列表
来源：http://cmj.cashguo.top

[y for x in nested for y in x]
来源：http://kfc.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://uqz.sxryk.cn

max(d, key=d.get)
来源：http://akq.gotoacloud.top

[U10] Py：按值排序字典
来源：http://omq.bjfxy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://otj.jyoumei.cn

[U11] Py：生成器表达式
来源：http://ckm.ydzc1.top

(x * 2 for x in arr)
来源：http://pvt.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://kho.cdnleiting.top

Counter(arr).most_common(3)
来源：http://uhn.nwbrower.top


<!-- 参考信息 -->