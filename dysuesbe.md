代发 wailian999

free -h;  ps aux | grep nginx
来源：http://ywr.bbcook.cn

[R64] 结束进程
来源：http://bsb.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://lep.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://ank.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cju.pycfn.com

[R66] 定时任务
来源：http://ypq.gotoacloud.top

crontab -e;  crontab -l
来源：http://cfb.bbcook.cn

[R67] 生成随机十六进制串
来源：http://hgv.gogol.net.cn

openssl rand -hex 16
来源：http://edq.wangdashe.top

[R68] 计算文件校验值
来源：http://dno.ydjk.org.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iwr.ivvv.top

[R69] 生成随机密码
来源：http://ubr.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://jdx.meibo888.top

[R70] 时间戳与互转
来源：http://uvo.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://hmt.hnqzz.top

[R71] 日期格式化
来源：http://vek.zhijiandao.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sql.xuanzx.com

[R72] 等待端口就绪
来源：http://tjc.zhaomingkeji.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://kdn.feifeiyinyue.top

[R73] 分割大日志
来源：http://vmo.ehwqpu.com

split -l 1000 big.log part_
来源：http://ebk.xuetiantiany.cn

[R74] 批量重命名
来源：http://ldf.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pka.guowangkeji.top

[R75] 导出环境变量
来源：http://lmo.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://wbt.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://bhm.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nin.ybcxt.top

[R77] 读取用户输入
来源：http://ltp.daria6918.cn

read -rp "请输入: " ans
来源：http://ppv.hysaishi.cn

[R78] 交互式菜单
来源：http://llm.cheryme.top

select opt in a b c; do echo "$opt"; break; done
来源：http://otc.zhongyouzk.top

[R79] 解析命令行选项
来源：http://ldm.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hnx.ehwqpu.com

[R80] 查看脚本执行耗时
来源：http://gqd.yueranfly.top

time ./run.sh
来源：http://xbx.ehwqpu.com

================================================================================
来源：http://lqd.hongshengwenyu.top

S. C / C++ 专题
来源：http://wzt.yongpay.top

================================================================================
来源：http://jir.andypj.xyz

[S01] C：Hello World
来源：http://bho.jinyuanbaomall.cn

#include <stdio.h>
来源：http://fbq.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://meg.xziqi.cn

[S02] C：变量与格式化输出
来源：http://adj.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://oah.yj202588.top

[S03] C：读入整数
来源：http://rbz.hammf.cn

int x; scanf("%d", &x);
来源：http://akr.jlsjyb.cn

[S04] C：字符串复制
来源：http://sem.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://cnd.redwolf501.top

[S05] C：字符串长度
来源：http://uxn.tarul.cn

strlen(s)
来源：http://zms.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://nzv.cucudq.cn

strcmp(a, b) == 0
来源：http://xqj.yuxming.cn

[S07] C：数组遍历求和
来源：http://xgb.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fqy.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://cqb.zycfv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tuy.cucudq.cn

[S09] C：结构体定义与初始化
来源：http://gmx.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ilz.zhijiandao.cn

[S10] C：指针与解引用
来源：http://xci.xylfe.cn

int *p = &a;  *p = 5;
来源：http://ynj.gotoacloud.top

[S11] C：逐行读文件
来源：http://dsh.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://alc.hongshengwenyu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ppy.zhijiandao.cn

fclose(f);
来源：http://vfl.jyoumei.cn

[S12] C：写文件
来源：http://akp.hammf.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oim.shangyingyoupin.top

[S13] C：宏定义
来源：http://vzo.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mxb.dianchejie.cn

[S14] C：枚举
来源：http://ked.epnwcf.com

enum Color { RED, GREEN, BLUE };
来源：http://nha.gzhubu.top

[S15] C：类型转换
来源：http://ujl.bjfxy.top

(double) a / b
来源：http://uhz.yuxming.cn

[S16] C：位操作置位
来源：http://cay.ydzc1.top

x |= (1 << 3);
来源：http://hsy.nwbrower.top

[S17] C：安全拼接字符串
来源：http://kbq.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lcc.aizwys.cn

[S18] C：命令行参数
来源：http://ojz.fehbvm.com

int main(int argc, char **argv)
来源：http://glv.xziqi.cn

[S19] C：快速排序
来源：http://qdi.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://rdy.guowangkeji.top

[S20] C：二分查找
来源：http://zmp.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mzk.chenjidiqi.icu

[S21] C：字符类别判断
来源：http://nkt.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tpa.svipenyu.cn

[S22] C：字符串转数字
来源：http://cak.zycfv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xrv.yonumen.top

[S23] C：随机数
来源：http://byx.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://aen.quarkkingdee.top

[S24] C：获取本地时间
来源：http://wyx.0kj1m.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dpp.aizwys.cn

[S25] C：内存拷贝
来源：http://vbz.zhoulong.xyz

memcpy(dst, src, n);
来源：http://boi.birdmap.top

[S26] C：内存清零
来源：http://pcv.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://gia.zhoulong.xyz

[S27] C：定义常量
来源：http://kfy.birdmap.top

const double PI = 3.14159;
来源：http://lsm.c1oappe.top

[S28] C：静态变量
来源：http://kbt.ehwqpu.com

static int counter = 0;
来源：http://mby.gaohongyu789.top

[S29] C：变参函数
来源：http://scr.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://naa.sufxvd.cn

[S30] C：头文件保护
来源：http://wct.ctjpmb.com

#ifndef X_H
来源：http://mld.ppjwa.cn

#define X_H
来源：http://eud.gotoacloud.top

#endif
来源：http://gnv.jinyuanbaomall.cn

[S31] C++：Hello World
来源：http://urf.daria6918.cn

#include <iostream>
来源：http://iyb.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://oum.pycfn.com

[S32] C++：字符串
来源：http://kym.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://zks.fengsongda.top

[S33] C++：vector 增删
来源：http://lhh.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jsc.xziqi.cn

[S34] C++：遍历 vector
来源：http://cov.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://vvp.mhx1999.top

[S35] C++：map
来源：http://zxm.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cxc.hnxiangtu.top

[S36] C++：unordered_map
来源：http://eus.daxiang520.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fep.ctjpmb.com

[S37] C++：set
来源：http://qcg.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sds.wangshuangyany.cn

[S38] C++：排序
来源：http://nyi.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://kgh.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://uoz.chenjidiqi.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://czw.ydzc1.top

[S40] C++：查找元素
来源：http://hab.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zbw.meibo888.top

[S41] C++：类与构造函数
来源：http://brm.ehwqpu.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vpg.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://vmh.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://ssa.guannengcc.top

[S43] C++：智能指针
来源：http://ysg.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://vab.cucudq.cn

[S44] C++：引用传参
来源：http://vaq.cucudq.cn

void inc(int &x) { ++x; }
来源：http://qva.bbcook.cn

[S45] C++：lambda
来源：http://mxu.aizwys.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dns.feifeiyinyue.top

[S46] C++：函数模板
来源：http://vlo.fzhhl.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ici.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://etx.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kyg.zhengqikj.top

[S48] C++：逐行读文件
来源：http://tbo.epnwcf.com

std::ifstream in("a.txt");  std::string line;
来源：http://ipr.birdmap.top

while (std::getline(in, line)) { }
来源：http://zzj.epnwcf.com

[S49] C++：写文件
来源：http://qfs.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gjn.ctjpmb.com

[S50] C++：格式化数字
来源：http://obd.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tea.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://spt.quarkkingdee.top

static_cast<double>(a) / b
来源：http://imm.svipenyu.cn

[S52] C++：const 与 noexcept
来源：http://eod.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://dbe.jyoumei.cn

[S53] C++：移动语义
来源：http://jyr.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://smr.yonumen.top

[S54] C++：异常处理
来源：http://tpu.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xvy.sweek.top

[S55] C++：结构化绑定
来源：http://utk.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://khd.ctjpmb.com

[S56] C++：optional
来源：http://qim.yanxiufei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kso.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://zrb.sweek.top

constexpr int N = 10;
来源：http://tlc.kuanghao11.cn

[S58] C++：命名空间
来源：http://kkm.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://ivp.bbcook.cn

[S59] C++：静态断言
来源：http://axy.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fhn.pycfn.com

[S60] C++：遍历并删除元素
来源：http://otn.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wdm.snrcjt.cn

================================================================================
来源：http://uzn.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://krr.c1oappe.top

================================================================================
来源：http://jsu.sweek.top

[T01] Kotlin：Hello World
来源：http://efr.wangshuangyany.cn

println("Hello")
来源：http://nqb.dashuyun.cn

[T02] Kotlin：变量
来源：http://ltr.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hrr.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://dzh.dianchejie.cn

"值: $b"
来源：http://ezv.feifeiyinyue.top

[T04] Kotlin：空安全
来源：http://yxw.gotoacloud.top

val n: String? = null;  n?.length
来源：http://bsl.zycfv.cn

[T05] Kotlin：when 表达式
来源：http://ihs.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mza.pycfn.com

[T06] Kotlin：集合映射
来源：http://hjd.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vhv.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://jie.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rki.nwbrower.top

[T08] Kotlin：数据类
来源：http://rjz.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://nge.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://bwy.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://mas.sysykeji.top

[T10] Kotlin：默认参数
来源：http://vyd.ydzc1.top

fun greet(name: String = "World") = "Hi $name"
来源：http://adg.ydzc1.top

[T11] Kotlin：协程
来源：http://kko.52xcode.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gol.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://jod.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://grl.hammf.cn

[T13] Kotlin：只读 Map
来源：http://mzl.nwbrower.top

val m = mapOf("a" to 1)
来源：http://ruu.gaohongyu789.top

[T14] Kotlin：循环
来源：http://mxx.xylfe.cn

for (i in 1..10) println(i)
来源：http://rjp.jyoumei.cn

[T15] Kotlin：接口
来源：http://jfc.smart0.xyz

interface Shape { fun area(): Double }
来源：http://ssk.hongshengwenyu.top

[T16] Swift：Hello World
来源：http://nsm.xingfuxueyuan.xyz

print("Hello")
来源：http://uix.yueranfly.top

[T17] Swift：变量与常量
来源：http://mvc.yj202588.top

var a = 1;  let b = 2
来源：http://ftm.yj20258.top

[T18] Swift：字符串插值
来源：http://rnw.chenjidiqi.icu

"值: \(b)"
来源：http://szv.yongpay.top

[T19] Swift：可选绑定
来源：http://kal.kuanghao11.cn

if let n = opt { print(n) }
来源：http://hyj.yuanzhike.top

[T20] Swift：数组操作
来源：http://rey.zycfv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tdr.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://pfr.guowangkeji.top

for x in a { print(x) }
来源：http://mov.sjlbkw.cn

[T22] Swift：字典
来源：http://ydp.fzhhl.top

var d = ["a": 1];  d["b"] = 2
来源：http://cyg.kuanghao11.cn

[T23] Swift：函数
来源：http://zsd.ppjwa.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pyv.vehdjk.com

[T24] Swift：闭包
来源：http://smj.hysaishi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gjj.hongshengwenyu.top

[T25] Swift：结构体
来源：http://wrz.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://hcs.daria6918.cn

[T26] Swift：类与重写
来源：http://vrg.zdbjq.cn

class A: Base { override func f() {} }
来源：http://bnw.yuxming.cn

[T27] Swift：错误处理
来源：http://wwm.yj20258.top

do { try f() } catch { print(error) }
来源：http://gki.hysaishi.cn

[T28] Swift：枚举
来源：http://hlt.52xcode.cn

enum Color { case red, green }
来源：http://zsm.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://qdv.svipenyu.cn

guard let x = opt else { return }
来源：http://yej.fengsongda.top

[T30] Swift：协议
来源：http://ceo.jiagoushi.top

protocol Shape { func area() -> Double }
来源：http://bib.gogol.net.cn

[T31] Lua：Hello World
来源：http://gsz.sysykeji.top

print("Hello")
来源：http://fwm.0kj1m.cn

[T32] Lua：局部变量
来源：http://xyx.yfazqb.com

local a = 1
来源：http://jxf.yonumen.top

[T33] Lua：表（数组）
来源：http://nnx.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ndf.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://wvd.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://gvu.shangyingyoupin.top

[T35] Lua：字典表
来源：http://afr.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://dss.xziqi.cn

[T36] Lua：函数
来源：http://jin.zhengqikj.top

function add(a, b) return a + b end
来源：http://biw.52xcode.cn

[T37] Lua：字符串拼接
来源：http://ohb.ywan-chungtsiang.top

"a" .. "b"
来源：http://oqz.shuidangran.top

[T38] Lua：条件
来源：http://qmq.sufxvd.cn

if x > 0 then print("正") end
来源：http://xpn.dianchejie.cn

[T39] Lua：模式匹配
来源：http://sjx.yonumen.top

string.find(s, "%d+")
来源：http://ynp.ctjpmb.com

[T40] Lua：元表
来源：http://ctg.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://ehf.sxryk.cn

[T41] Perl：Hello World
来源：http://ocy.xziqi.cn

print "Hello\n";
来源：http://bhf.fktsv.cn

[T42] Perl：变量类型
来源：http://rtp.ywan-chungtsiang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zrh.cdnleiting.top

[T43] Perl：字符串插值
来源：http://oqi.birdmap.top

"值: $a"
来源：http://muu.aizwys.cn

[T44] Perl：条件
来源：http://ybm.xuanzx.com

if ($a > 0) { print "正"; }
来源：http://ttv.svipenyu.cn

[T45] Perl：数组遍历
来源：http://vqc.tanke756.top

for my $x (@arr) { print $x; }
来源：http://deh.xylfe.cn

[T46] Perl：哈希操作
来源：http://vcm.shanyushiyangtech.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rec.xylfe.cn

[T47] Perl：正则捕获
来源：http://abx.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://xgy.zhengqikj.top

[T48] Perl：正则替换
来源：http://brw.zdqjudy.top

$s =~ s/old/new/g;
来源：http://gsk.epnwcf.com

[T49] Perl：函数
来源：http://cqb.sysykeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tdl.ybcxt.top

[T50] Perl：逐行读文件
来源：http://nlx.gzhubu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://byd.svipenyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://mhm.yongpay.top

[T51] Scala：Hello World
来源：http://olr.yuxming.cn

println("Hello")
来源：http://iex.cheryme.top

[T52] Scala：变量
来源：http://lfp.guannengcc.top

val a = 1;  var b = 2
来源：http://ylg.ybcxt.top

[T53] Scala：字符串插值
来源：http://zda.gogol.net.cn

s"值: $b"
来源：http://tnm.yvedp.cn

[T54] Scala：集合映射
来源：http://wae.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://ywv.birdmap.top

[T55] Scala：集合过滤
来源：http://tzl.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gzk.ybcxt.top

[T56] Scala：样例类
来源：http://kck.feifeiyinyue.top

case class User(name: String, age: Int)
来源：http://rby.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://qlw.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dph.c1oappe.top

[T58] Scala：函数定义
来源：http://qkj.iojbl.cn

def add(a: Int, b: Int): Int = a + b
来源：http://feu.ydjk.org.cn

[T59] Scala：循环
来源：http://uwm.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://iey.yongpay.top

[T60] Scala：折叠
来源：http://kvq.yuxming.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fxd.aibaodan.cn

================================================================================
来源：http://jso.sjlbkw.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nrr.jinyuanbaomall.cn

================================================================================
来源：http://tln.yongpay.top

[U01] Py：创建虚拟环境
来源：http://khw.zhixingplan.top

python -m venv .venv && source .venv/bin/activate
来源：http://wtf.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://ywt.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://khd.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://uav.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bsn.nanxinkj.top

[U04] Py：变量调试打印
来源：http://tsx.bbcook.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yei.redwolf501.top


<!-- 参考信息 -->