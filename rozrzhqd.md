代发 wailian999

free -h;  ps aux | grep nginx
来源：http://xiq.sweek.top

[R64] 结束进程
来源：http://nhf.shangyingyoupin.top

kill -9 $(pgrep -f app.py)
来源：http://cde.tarul.cn

[R65] 查看端口占用
来源：http://fdv.smart0.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lmb.smart0.xyz

[R66] 定时任务
来源：http://ang.yueranfly.top

crontab -e;  crontab -l
来源：http://ewe.andypj.xyz

[R67] 生成随机十六进制串
来源：http://jrw.pycfn.com

openssl rand -hex 16
来源：http://lgm.uphjek.com

[R68] 计算文件校验值
来源：http://znc.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hfq.pengpengdd.cyou

[R69] 生成随机密码
来源：http://adj.snrcjt.cn

head -c 16 /dev/urandom | base64
来源：http://phw.ppjwa.cn

[R70] 时间戳与互转
来源：http://fjh.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://ikz.yvedp.cn

[R71] 日期格式化
来源：http://qht.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://doo.fehbvm.com

[R72] 等待端口就绪
来源：http://hcv.aizwys.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qap.zycfv.cn

[R73] 分割大日志
来源：http://wbx.aizwys.cn

split -l 1000 big.log part_
来源：http://vwx.hammf.cn

[R74] 批量重命名
来源：http://rzv.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xnp.kuanghao11.cn

[R75] 导出环境变量
来源：http://krc.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://mbn.shangyingyoupin.top

[R76] 使用临时文件
来源：http://hkr.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vep.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://ogp.cqqwz.cn

read -rp "请输入: " ans
来源：http://sxb.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://fod.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dga.cqqwz.cn

[R79] 解析命令行选项
来源：http://yow.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dqy.smart0.xyz

[R80] 查看脚本执行耗时
来源：http://ctm.hnxiangtu.top

time ./run.sh
来源：http://rup.hnqzz.top

================================================================================
来源：http://psd.jinqigfzy.top

S. C / C++ 专题
来源：http://yza.kuanghao11.cn

================================================================================
来源：http://gci.gogol.net.cn

[S01] C：Hello World
来源：http://tkj.zhijiandao.cn

#include <stdio.h>
来源：http://iyw.hongshengwenyu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ope.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://oxs.hnqzz.top

int a = 10; printf("%d\n", a);
来源：http://gfl.jinyuanbaomall.cn

[S03] C：读入整数
来源：http://jpy.yangfankeji.com

int x; scanf("%d", &x);
来源：http://els.nanxuanxn.top

[S04] C：字符串复制
来源：http://ynx.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://jlr.kuanghao11.cn

[S05] C：字符串长度
来源：http://kne.kuanghao11.cn

strlen(s)
来源：http://xno.yj20258.top

[S06] C：字符串比较
来源：http://tgm.jqgufenzy.top

strcmp(a, b) == 0
来源：http://yft.sxryk.cn

[S07] C：数组遍历求和
来源：http://bux.fzhhl.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qou.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://fns.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ptg.dashuyun.cn

[S09] C：结构体定义与初始化
来源：http://lmj.nanxuanxn.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jzj.kuanghao11.cn

[S10] C：指针与解引用
来源：http://axa.cucudq.cn

int *p = &a;  *p = 5;
来源：http://rlm.guowangkeji.top

[S11] C：逐行读文件
来源：http://bwh.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://yez.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dva.svipenyu.cn

fclose(f);
来源：http://dip.svipenyu.cn

[S12] C：写文件
来源：http://qhj.ehwqpu.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vsa.hammf.cn

[S13] C：宏定义
来源：http://byl.316326.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kxh.c1oappe.top

[S14] C：枚举
来源：http://kua.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://evc.xuetiantiany.cn

[S15] C：类型转换
来源：http://zbz.hammf.cn

(double) a / b
来源：http://dya.dashuyun.cn

[S16] C：位操作置位
来源：http://fkt.cdnleiting.top

x |= (1 << 3);
来源：http://nup.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://zzz.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lgs.svipenyu.cn

[S18] C：命令行参数
来源：http://ikp.shanyushiyangkeji.top

int main(int argc, char **argv)
来源：http://apr.tian-w.cn

[S19] C：快速排序
来源：http://dsn.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://mox.yueranfly.top

[S20] C：二分查找
来源：http://xum.vehdjk.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pzq.wangshuangyany.cn

[S21] C：字符类别判断
来源：http://sok.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://heo.birdmap.top

[S22] C：字符串转数字
来源：http://kwk.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://sel.zdqjudy.top

[S23] C：随机数
来源：http://ots.hcnkem.com

srand(time(NULL));  int r = rand() % 100;
来源：http://nzl.kuanghao11.cn

[S24] C：获取本地时间
来源：http://imz.hfpthk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yvz.chenzaomai.com

[S25] C：内存拷贝
来源：http://wiq.gzhubu.top

memcpy(dst, src, n);
来源：http://jbr.hcnkem.com

[S26] C：内存清零
来源：http://jua.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://ouv.sufxvd.cn

[S27] C：定义常量
来源：http://gqu.gaohongyu789.top

const double PI = 3.14159;
来源：http://yos.cheryme.top

[S28] C：静态变量
来源：http://yfx.ywan-chungtsiang.top

static int counter = 0;
来源：http://rhx.cqqwz.cn

[S29] C：变参函数
来源：http://byr.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ugp.hammf.cn

[S30] C：头文件保护
来源：http://bpt.ivvv.top

#ifndef X_H
来源：http://zhl.0kj1m.cn

#define X_H
来源：http://ffq.52xcode.cn

#endif
来源：http://bua.wangdashe.top

[S31] C++：Hello World
来源：http://tuk.daxiang520.top

#include <iostream>
来源：http://acp.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://qlb.shuidangran.top

[S32] C++：字符串
来源：http://uzm.havefunace.top

std::string s = "hi";  s += "!";
来源：http://fvf.sufxvd.cn

[S33] C++：vector 增删
来源：http://bkt.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fcy.tianlin.xyz

[S34] C++：遍历 vector
来源：http://whn.yuanzhike.top

for (auto &x : v) { std::cout << x; }
来源：http://owf.ydjk.org.cn

[S35] C++：map
来源：http://rcb.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uql.yfazqb.com

[S36] C++：unordered_map
来源：http://gap.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rdj.uphjek.com

[S37] C++：set
来源：http://qgg.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jbl.uphjek.com

[S38] C++：排序
来源：http://qtm.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://mrq.ivvv.top

[S39] C++：自定义比较器排序
来源：http://pfc.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://twl.snrcjt.cn

[S40] C++：查找元素
来源：http://gei.gaohongyu789.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hjm.shuidangran.top

[S41] C++：类与构造函数
来源：http://pha.hfpthk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iyw.fzhhl.top

[S42] C++：继承与虚函数
来源：http://sbw.shanyushiyangtech.top

class B : public Base { public: void f() override {} };
来源：http://cyx.cdnleiting.top

[S43] C++：智能指针
来源：http://rnr.hammf.cn

auto p = std::make_unique<int>(5);
来源：http://iix.yfazqb.com

[S44] C++：引用传参
来源：http://era.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://fbp.shanyushiyangkeji.top

[S45] C++：lambda
来源：http://eqg.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://jyf.pengpengdd.cyou

[S46] C++：函数模板
来源：http://los.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yua.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://qga.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jmq.xinyue.icu

[S48] C++：逐行读文件
来源：http://kjn.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://wuv.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://ttq.hfpthk.cn

[S49] C++：写文件
来源：http://jzn.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mbx.bbcook.cn

[S50] C++：格式化数字
来源：http://yjy.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://plu.redwolf501.top

[S51] C++：显式类型转换
来源：http://wir.svipenyu.cn

static_cast<double>(a) / b
来源：http://rxc.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://bbz.hcnkem.com

int size() const noexcept { return n_; }
来源：http://htx.hfpthk.cn

[S53] C++：移动语义
来源：http://dbu.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://ttp.aibaodan.cn

[S54] C++：异常处理
来源：http://bdn.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cov.svipenyu.cn

[S55] C++：结构化绑定
来源：http://kdm.jianghu66.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gbu.kuanghao11.cn

[S56] C++：optional
来源：http://rfl.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lxe.hnqzz.top

[S57] C++：编译期常量
来源：http://mch.hnxiangtu.top

constexpr int N = 10;
来源：http://brc.zhaomingkeji.xyz

[S58] C++：命名空间
来源：http://lvs.zhaomingkeji.xyz

namespace ns { int f() { return 1; } }
来源：http://myo.zdqjudy.top

[S59] C++：静态断言
来源：http://mch.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lpo.jyoumei.cn

[S60] C++：遍历并删除元素
来源：http://kad.yj20258888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ioe.feifeiyinyue.top

================================================================================
来源：http://qdy.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vvh.yuxming.cn

================================================================================
来源：http://kdm.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://idn.mhx1999.top

println("Hello")
来源：http://yqv.redwolf501.top

[T02] Kotlin：变量
来源：http://lvb.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hao.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://obt.uphjek.com

"值: $b"
来源：http://ipg.dashuyun.cn

[T04] Kotlin：空安全
来源：http://boj.tanke756.top

val n: String? = null;  n?.length
来源：http://xnd.bjfxy.top

[T05] Kotlin：when 表达式
来源：http://cbv.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cre.zycfv.cn

[T06] Kotlin：集合映射
来源：http://nzk.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bhv.jianghu66.top

[T07] Kotlin：集合过滤
来源：http://qpr.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wge.feifeiyinyue.top

[T08] Kotlin：数据类
来源：http://zjx.ydzc1.top

data class User(val name: String, val age: Int)
来源：http://fei.sweek.top

[T09] Kotlin：扩展函数
来源：http://fci.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://jvp.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://qua.xingfuxueyuan.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://kyi.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://roq.yuanzhike.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://upr.gzhubu.top

[T12] Kotlin：解构声明
来源：http://otj.jlsjyb.cn

val (a, b) = Pair(1, 2)
来源：http://zlh.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://ulr.xylfe.cn

val m = mapOf("a" to 1)
来源：http://irs.ctjpmb.com

[T14] Kotlin：循环
来源：http://gjw.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://xyv.haohaochexian.top

[T15] Kotlin：接口
来源：http://pre.svipenyu.cn

interface Shape { fun area(): Double }
来源：http://owc.ywan-chungtsiang.top

[T16] Swift：Hello World
来源：http://fjd.kuanghao11.cn

print("Hello")
来源：http://ofx.nwbrower.top

[T17] Swift：变量与常量
来源：http://fek.quarkkingdee.top

var a = 1;  let b = 2
来源：http://pmq.xziqi.cn

[T18] Swift：字符串插值
来源：http://jdk.yuxming.cn

"值: \(b)"
来源：http://mgy.wangshuangyany.cn

[T19] Swift：可选绑定
来源：http://ooh.chenzaomai.com

if let n = opt { print(n) }
来源：http://qrp.daxiang520.top

[T20] Swift：数组操作
来源：http://xyp.tianlin.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://klv.xylfe.cn

[T21] Swift：遍历
来源：http://bzh.cashguo.top

for x in a { print(x) }
来源：http://kya.9152youxi.cn

[T22] Swift：字典
来源：http://ose.zhaomingkeji.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://gri.hongshengwenyu.top

[T23] Swift：函数
来源：http://wud.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cok.fktsv.cn

[T24] Swift：闭包
来源：http://goy.yonumen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hoi.sxryk.cn

[T25] Swift：结构体
来源：http://jxb.yj202588.top

struct P { var x: Int }
来源：http://crx.guowangkeji.top

[T26] Swift：类与重写
来源：http://bky.ivvv.top

class A: Base { override func f() {} }
来源：http://rps.kuanghao11.cn

[T27] Swift：错误处理
来源：http://hfe.yvedp.cn

do { try f() } catch { print(error) }
来源：http://fce.sufxvd.cn

[T28] Swift：枚举
来源：http://ybj.hesvh.cn

enum Color { case red, green }
来源：http://vjl.jqgfzy.top

[T29] Swift：guard 提前返回
来源：http://uyy.cqqwz.cn

guard let x = opt else { return }
来源：http://qkv.yfazqb.com

[T30] Swift：协议
来源：http://nir.uphjek.com

protocol Shape { func area() -> Double }
来源：http://wca.tian-w.cn

[T31] Lua：Hello World
来源：http://cbn.ppjwa.cn

print("Hello")
来源：http://izq.gaohongyu789.top

[T32] Lua：局部变量
来源：http://dtq.wangdashe.top

local a = 1
来源：http://mve.iojbl.cn

[T33] Lua：表（数组）
来源：http://cpj.zhoulong.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://sls.zhixingplan.top

[T34] Lua：遍历表
来源：http://yst.jqgfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pop.fehbvm.com

[T35] Lua：字典表
来源：http://qly.svipenyu.cn

local d = { a = 1 };  d.b = 2
来源：http://dli.ppjwa.cn

[T36] Lua：函数
来源：http://fnv.gzhubu.top

function add(a, b) return a + b end
来源：http://com.pengpengdd.cyou

[T37] Lua：字符串拼接
来源：http://vvy.jinghuilouyu.cn

"a" .. "b"
来源：http://tzt.sweek.top

[T38] Lua：条件
来源：http://rsh.hnqzz.top

if x > 0 then print("正") end
来源：http://our.ywan-chungtsiang.top

[T39] Lua：模式匹配
来源：http://ufv.xuanzx.com

string.find(s, "%d+")
来源：http://lsc.cucudq.cn

[T40] Lua：元表
来源：http://nvy.redwolf501.top

setmetatable({}, { __index = base })
来源：http://fdh.haohaochexian.top

[T41] Perl：Hello World
来源：http://qaw.zycfv.cn

print "Hello\n";
来源：http://xif.redwolf501.top

[T42] Perl：变量类型
来源：http://cxk.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://akl.meibo888.top

[T43] Perl：字符串插值
来源：http://syi.zhaomingkeji.xyz

"值: $a"
来源：http://vcq.wangdashe.top

[T44] Perl：条件
来源：http://ljv.hywenlv.cn

if ($a > 0) { print "正"; }
来源：http://hlq.snrcjt.cn

[T45] Perl：数组遍历
来源：http://yks.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://tqv.hfpthk.cn

[T46] Perl：哈希操作
来源：http://jou.yvedp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tst.gotoacloud.top

[T47] Perl：正则捕获
来源：http://tsl.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tas.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://hox.zycfv.cn

$s =~ s/old/new/g;
来源：http://jgb.wangshuangyany.cn

[T49] Perl：函数
来源：http://ztj.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://imq.yangfankeji.com

[T50] Perl：逐行读文件
来源：http://ttc.mhx1999.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pkl.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://vuc.mhx1999.top

[T51] Scala：Hello World
来源：http://vtl.epnwcf.com

println("Hello")
来源：http://rdv.havefunace.top

[T52] Scala：变量
来源：http://yre.bbcook.cn

val a = 1;  var b = 2
来源：http://cmd.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://vkd.aizwys.cn

s"值: $b"
来源：http://nap.yueranfly.top

[T54] Scala：集合映射
来源：http://nym.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://svj.yfazqb.com

[T55] Scala：集合过滤
来源：http://dpz.yonumen.top

List(1, 2, 3).filter(_ > 1)
来源：http://lrz.zhengqikj.top

[T56] Scala：样例类
来源：http://nak.sufxvd.cn

case class User(name: String, age: Int)
来源：http://tkb.birdmap.top

[T57] Scala：模式匹配
来源：http://obc.ywan-chungtsiang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://chi.gogol.net.cn

[T58] Scala：函数定义
来源：http://fqe.birdmap.top

def add(a: Int, b: Int): Int = a + b
来源：http://ikm.yfazqb.com

[T59] Scala：循环
来源：http://hqu.yj20258.top

for (i <- 1 to 10) println(i)
来源：http://ltn.52xcode.cn

[T60] Scala：折叠
来源：http://gbx.epnwcf.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ecp.shuidangran.top

================================================================================
来源：http://aew.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rts.gogol.net.cn

================================================================================
来源：http://qlh.hysaishi.cn

[U01] Py：创建虚拟环境
来源：http://ynq.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://wwp.jianghu66.top

[U02] Py：导出 / 安装依赖
来源：http://srd.chenzaomai.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pzh.nwbrower.top

[U03] Py：加载 .env 配置
来源：http://spg.cashguo.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tai.zhiwuduotai.top

[U04] Py：变量调试打印
来源：http://jsz.bbcook.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yfp.zhoulong.xyz


<!-- 参考信息 -->