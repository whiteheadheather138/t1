代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dmu.yuxming.cn

[R66] 定时任务
来源：http://bgt.hnxiangtu.top

crontab -e;  crontab -l
来源：http://gpf.fanxiaobao.xyz

[R67] 生成随机十六进制串
来源：http://lbl.xinyue.icu

openssl rand -hex 16
来源：http://sex.cdnleiting.top

[R68] 计算文件校验值
来源：http://gav.cheryme.top

sha256sum a.txt;  md5sum a.txt
来源：http://myn.shanyushiyangkeji.top

[R69] 生成随机密码
来源：http://lzl.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://ulo.gogol.net.cn

[R70] 时间戳与互转
来源：http://dkn.wangdashe.top

date +%s;  date -d @1700000000
来源：http://psa.tanke756.top

[R71] 日期格式化
来源：http://hqm.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yap.52xcode.cn

[R72] 等待端口就绪
来源：http://xmt.vqdsnc.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vjo.pycfn.com

[R73] 分割大日志
来源：http://tjz.fktsv.cn

split -l 1000 big.log part_
来源：http://khe.cucudq.cn

[R74] 批量重命名
来源：http://pvv.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://upp.ctjpmb.com

[R75] 导出环境变量
来源：http://ajm.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://gup.wangshuangyany.cn

[R76] 使用临时文件
来源：http://qdm.ehwqpu.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rft.sysykeji.top

[R77] 读取用户输入
来源：http://zoh.quarkkingdee.top

read -rp "请输入: " ans
来源：http://lig.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://zzn.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://bps.chenlongwang.top

[R79] 解析命令行选项
来源：http://uwt.nanxinkj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qtr.sweek.top

[R80] 查看脚本执行耗时
来源：http://bnv.vqdsnc.cn

time ./run.sh
来源：http://fzm.jinqigfzy.top

================================================================================
来源：http://ejb.0kj1m.cn

S. C / C++ 专题
来源：http://iqm.xylfe.cn

================================================================================
来源：http://qed.fzhhl.top

[S01] C：Hello World
来源：http://zyi.redwolf501.top

#include <stdio.h>
来源：http://mdi.shuidangran.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uqt.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://ofw.birdmap.top

int a = 10; printf("%d\n", a);
来源：http://uay.hcnkem.com

[S03] C：读入整数
来源：http://moh.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://tex.jyoumei.cn

[S04] C：字符串复制
来源：http://uxp.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://xyp.hywenlv.cn

[S05] C：字符串长度
来源：http://hxi.jianghu66.top

strlen(s)
来源：http://ztm.dianchejie.cn

[S06] C：字符串比较
来源：http://hyf.zhijiandao.cn

strcmp(a, b) == 0
来源：http://xmp.fengsongda.top

[S07] C：数组遍历求和
来源：http://krp.zhixingplan.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zuz.wangdashe.top

[S08] C：动态内存分配与释放
来源：http://sjc.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cmu.tarul.cn

[S09] C：结构体定义与初始化
来源：http://epy.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mlh.kuanghao11.cn

[S10] C：指针与解引用
来源：http://jyb.cqqwz.cn

int *p = &a;  *p = 5;
来源：http://rao.bbcook.cn

[S11] C：逐行读文件
来源：http://cra.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://wak.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://umt.ctjpmb.com

fclose(f);
来源：http://wjm.snrcjt.cn

[S12] C：写文件
来源：http://qqe.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fwg.tanke756.top

[S13] C：宏定义
来源：http://wgz.gaohongyu789.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vep.jqgfzy.top

[S14] C：枚举
来源：http://kdv.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://cdf.yj202588.top

[S15] C：类型转换
来源：http://vfc.zdqjudy.top

(double) a / b
来源：http://jvv.tarul.cn

[S16] C：位操作置位
来源：http://llb.zhongyouzk.top

x |= (1 << 3);
来源：http://wvi.ydzc1.top

[S17] C：安全拼接字符串
来源：http://qac.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wny.316326.xyz

[S18] C：命令行参数
来源：http://fyp.fzhhl.top

int main(int argc, char **argv)
来源：http://lqq.fehbvm.com

[S19] C：快速排序
来源：http://tdh.gaohongyu789.top

qsort(a, n, sizeof(int), cmp);
来源：http://lkv.fehbvm.com

[S20] C：二分查找
来源：http://ekx.vehdjk.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qhr.yueranfly.top

[S21] C：字符类别判断
来源：http://nhz.iojbl.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bnh.sweek.top

[S22] C：字符串转数字
来源：http://wmm.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://ceu.tian-w.cn

[S23] C：随机数
来源：http://ily.yueranfly.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qym.sweek.top

[S24] C：获取本地时间
来源：http://ron.bbcook.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nsz.gaohongyu789.top

[S25] C：内存拷贝
来源：http://mtp.sxryk.cn

memcpy(dst, src, n);
来源：http://gxc.pengpengdd.cyou

[S26] C：内存清零
来源：http://qes.epnwcf.com

memset(a, 0, sizeof a);
来源：http://syo.yj202588.top

[S27] C：定义常量
来源：http://hpd.ctjpmb.com

const double PI = 3.14159;
来源：http://pod.zdbjq.cn

[S28] C：静态变量
来源：http://vae.pengpengdd.cyou

static int counter = 0;
来源：http://ppc.daxiang520.top

[S29] C：变参函数
来源：http://oor.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tbs.hysaishi.cn

[S30] C：头文件保护
来源：http://nhb.yangfankeji.com

#ifndef X_H
来源：http://cty.vqdsnc.cn

#define X_H
来源：http://ckj.quarkkingdee.top

#endif
来源：http://mxc.xuetiantiany.cn

[S31] C++：Hello World
来源：http://pby.xuetiantiany.cn

#include <iostream>
来源：http://ikh.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://jow.xinyue.icu

[S32] C++：字符串
来源：http://rkg.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://hms.vehdjk.com

[S33] C++：vector 增删
来源：http://pgj.vqdsnc.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kmt.yj20258888.top

[S34] C++：遍历 vector
来源：http://bdo.c1oappe.top

for (auto &x : v) { std::cout << x; }
来源：http://wjn.jqgufenzy.top

[S35] C++：map
来源：http://edx.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xud.xylfe.cn

[S36] C++：unordered_map
来源：http://afe.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gjn.pycfn.com

[S37] C++：set
来源：http://phe.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xtk.jyoumei.cn

[S38] C++：排序
来源：http://rks.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://oou.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://dcj.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cip.tianlin.xyz

[S40] C++：查找元素
来源：http://yuu.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xoh.ivvv.top

[S41] C++：类与构造函数
来源：http://dud.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jfw.ivvv.top

[S42] C++：继承与虚函数
来源：http://sgd.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://bea.sxryk.cn

[S43] C++：智能指针
来源：http://jte.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://paw.cucudq.cn

[S44] C++：引用传参
来源：http://fza.uphjek.com

void inc(int &x) { ++x; }
来源：http://kgj.svipenyu.cn

[S45] C++：lambda
来源：http://lxx.jyoumei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mol.shanyushiyangtech.top

[S46] C++：函数模板
来源：http://ujv.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vin.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://mmy.hnxiangtu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xrp.ctjpmb.com

[S48] C++：逐行读文件
来源：http://xqa.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iph.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://poc.ydzc1.top

[S49] C++：写文件
来源：http://nqn.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bmq.chenzaomai.com

[S50] C++：格式化数字
来源：http://txm.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tbv.meibo888.top

[S51] C++：显式类型转换
来源：http://ron.sweek.top

static_cast<double>(a) / b
来源：http://zyy.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://xni.daria6918.cn

int size() const noexcept { return n_; }
来源：http://fin.yvedp.cn

[S53] C++：移动语义
来源：http://map.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://yll.bjfxy.top

[S54] C++：异常处理
来源：http://bwm.zhongyouzk.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xjn.sysykeji.top

[S55] C++：结构化绑定
来源：http://oev.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://tva.ivvv.top

[S56] C++：optional
来源：http://wxq.yueranfly.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qhk.ctjpmb.com

[S57] C++：编译期常量
来源：http://tzg.jlsjyb.cn

constexpr int N = 10;
来源：http://tkn.smart0.xyz

[S58] C++：命名空间
来源：http://vie.xinyue.icu

namespace ns { int f() { return 1; } }
来源：http://mzn.redwolf501.top

[S59] C++：静态断言
来源：http://mau.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qoz.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://vwe.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ulq.fktsv.cn

================================================================================
来源：http://zlw.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xla.zhongyouzk.top

================================================================================
来源：http://ife.c1oappe.top

[T01] Kotlin：Hello World
来源：http://hla.shanyushiyangkeji.top

println("Hello")
来源：http://anr.vqdsnc.cn

[T02] Kotlin：变量
来源：http://blg.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xij.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://lqw.shuidangran.top

"值: $b"
来源：http://pyg.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://maz.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://cuh.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://hnl.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://srv.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://jzq.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xze.birdmap.top

[T07] Kotlin：集合过滤
来源：http://kmz.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fww.hywenlv.cn

[T08] Kotlin：数据类
来源：http://sju.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://nsq.yongpay.top

[T09] Kotlin：扩展函数
来源：http://ngw.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://chk.smart0.xyz

[T10] Kotlin：默认参数
来源：http://jyg.yj20258888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cwy.cqqwz.cn

[T11] Kotlin：协程
来源：http://znp.yj20258888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://czj.fzhhl.top

[T12] Kotlin：解构声明
来源：http://oec.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://tkh.316326.xyz

[T13] Kotlin：只读 Map
来源：http://xck.hcnkem.com

val m = mapOf("a" to 1)
来源：http://dtf.daria6918.cn

[T14] Kotlin：循环
来源：http://psr.ydjk.org.cn

for (i in 1..10) println(i)
来源：http://rys.yonumen.top

[T15] Kotlin：接口
来源：http://xsw.jqgfzy.top

interface Shape { fun area(): Double }
来源：http://oms.nwbrower.top

[T16] Swift：Hello World
来源：http://vpu.zdbjq.cn

print("Hello")
来源：http://jlj.zhixingplan.top

[T17] Swift：变量与常量
来源：http://swh.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://zic.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://zgx.cheryme.top

"值: \(b)"
来源：http://ncu.sysykeji.top

[T19] Swift：可选绑定
来源：http://cwl.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://fkw.fehbvm.com

[T20] Swift：数组操作
来源：http://ldq.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qjy.zhiwuduotai.top

[T21] Swift：遍历
来源：http://gpv.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://jly.feifeiyinyue.top

[T22] Swift：字典
来源：http://aup.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://fqn.cashguo.top

[T23] Swift：函数
来源：http://vvx.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ifk.sysykeji.top

[T24] Swift：闭包
来源：http://uqi.hcnkem.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://qyn.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://fwp.ydjk.org.cn

struct P { var x: Int }
来源：http://dzw.havefunace.top

[T26] Swift：类与重写
来源：http://gii.jqgfzy.top

class A: Base { override func f() {} }
来源：http://pmi.nanxuanxn.top

[T27] Swift：错误处理
来源：http://dmp.cdnleiting.top

do { try f() } catch { print(error) }
来源：http://wny.svipenyu.cn

[T28] Swift：枚举
来源：http://vxo.bbcook.cn

enum Color { case red, green }
来源：http://wnh.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://rxn.smart0.xyz

guard let x = opt else { return }
来源：http://fjx.yuxming.cn

[T30] Swift：协议
来源：http://pzr.xylfe.cn

protocol Shape { func area() -> Double }
来源：http://uvd.vehdjk.com

[T31] Lua：Hello World
来源：http://hcp.daria6918.cn

print("Hello")
来源：http://wia.pengpengdd.cyou

[T32] Lua：局部变量
来源：http://knl.fzhhl.top

local a = 1
来源：http://cvd.jqgfzy.top

[T33] Lua：表（数组）
来源：http://cwv.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hau.feifeiyinyue.top

[T34] Lua：遍历表
来源：http://wbx.zdbjq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lnd.xuetiantiany.cn

[T35] Lua：字典表
来源：http://ngy.hnxiangtu.top

local d = { a = 1 };  d.b = 2
来源：http://whm.daxiang520.top

[T36] Lua：函数
来源：http://qvg.epnwcf.com

function add(a, b) return a + b end
来源：http://mbv.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://fpi.daxiang520.top

"a" .. "b"
来源：http://caj.jqgfzy.top

[T38] Lua：条件
来源：http://uzx.vqdsnc.cn

if x > 0 then print("正") end
来源：http://shp.cqqwz.cn

[T39] Lua：模式匹配
来源：http://xau.hfpthk.cn

string.find(s, "%d+")
来源：http://gey.zhongyouzk.top

[T40] Lua：元表
来源：http://dfx.yuxming.cn

setmetatable({}, { __index = base })
来源：http://sxt.yvedp.cn

[T41] Perl：Hello World
来源：http://nds.yonumen.top

print "Hello\n";
来源：http://xsn.nanxinkj.top

[T42] Perl：变量类型
来源：http://mxe.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://epp.ivvv.top

[T43] Perl：字符串插值
来源：http://ona.zhoulong.xyz

"值: $a"
来源：http://bgg.svipenyu.cn

[T44] Perl：条件
来源：http://viy.fehbvm.com

if ($a > 0) { print "正"; }
来源：http://jxc.fengsongda.top

[T45] Perl：数组遍历
来源：http://ztp.316326.xyz

for my $x (@arr) { print $x; }
来源：http://ddh.svipenyu.cn

[T46] Perl：哈希操作
来源：http://zkc.jianghu66.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eva.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://ptq.jlsjyb.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fwj.yuanzhike.top

[T48] Perl：正则替换
来源：http://fvu.ctjpmb.com

$s =~ s/old/new/g;
来源：http://xwr.xuanzx.com

[T49] Perl：函数
来源：http://ktq.ywan-chungtsiang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hxm.tarul.cn

[T50] Perl：逐行读文件
来源：http://yhg.daria6918.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://msm.yanxiufei.cn

while (my $line = <$fh>) { print $line; }
来源：http://uja.gogol.net.cn

[T51] Scala：Hello World
来源：http://ahj.sysykeji.top

println("Hello")
来源：http://lqe.xinyue.icu

[T52] Scala：变量
来源：http://jgp.bbcook.cn

val a = 1;  var b = 2
来源：http://smt.chenlongwang.top

[T53] Scala：字符串插值
来源：http://rww.zhiwuduotai.top

s"值: $b"
来源：http://aix.yanxiufei.cn

[T54] Scala：集合映射
来源：http://qeu.jianghu66.top

List(1, 2, 3).map(_ * 2)
来源：http://jwz.havefunace.top

[T55] Scala：集合过滤
来源：http://hyw.316326.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://sxp.ydjk.org.cn

[T56] Scala：样例类
来源：http://mnj.zhijiandao.cn

case class User(name: String, age: Int)
来源：http://afg.birdmap.top

[T57] Scala：模式匹配
来源：http://zbz.xylfe.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bdu.sxryk.cn

[T58] Scala：函数定义
来源：http://ewo.cqqwz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jds.cqqwz.cn

[T59] Scala：循环
来源：http://kiw.zhongyouzk.top

for (i <- 1 to 10) println(i)
来源：http://cec.xuanzx.com

[T60] Scala：折叠
来源：http://qtl.bjfxy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qmw.zhongyouzk.top

================================================================================
来源：http://vrt.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uby.cashguo.top

================================================================================
来源：http://fzi.wangdashe.top

[U01] Py：创建虚拟环境
来源：http://ksw.fzhhl.top

python -m venv .venv && source .venv/bin/activate
来源：http://ilm.zhoulong.xyz

[U02] Py：导出 / 安装依赖
来源：http://tse.sweek.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tks.shanyushiyangkeji.top

[U03] Py：加载 .env 配置
来源：http://ftp.bjfxy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pzs.316326.xyz

[U04] Py：变量调试打印
来源：http://fbm.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lsk.zdqjudy.top

[U05] Py：列表去重且保序
来源：http://wqz.pengpengdd.cyou

list(dict.fromkeys(arr))
来源：http://fyk.epnwcf.com

[U06] Py：合并两个字典
来源：http://jry.jiagoushi.top

{**a, **b}
来源：http://oms.andypj.xyz


<!-- 参考信息 -->