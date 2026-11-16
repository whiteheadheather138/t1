代发 wailian999

free -h;  ps aux | grep nginx
来源：http://xpk.hywenlv.cn

[R64] 结束进程
来源：http://vve.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://how.yangfankeji.com

[R65] 查看端口占用
来源：http://ckj.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xcu.shanyushiyangkeji.top

[R66] 定时任务
来源：http://mdf.ehwqpu.com

crontab -e;  crontab -l
来源：http://qcv.yfazqb.com

[R67] 生成随机十六进制串
来源：http://cxe.guowangkeji.top

openssl rand -hex 16
来源：http://yit.redwolf501.top

[R68] 计算文件校验值
来源：http://cmc.shuidangran.top

sha256sum a.txt;  md5sum a.txt
来源：http://dny.yongpay.top

[R69] 生成随机密码
来源：http://hpy.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://piq.nwbrower.top

[R70] 时间戳与互转
来源：http://esp.feifeiyinyue.top

date +%s;  date -d @1700000000
来源：http://umk.snrcjt.cn

[R71] 日期格式化
来源：http://enf.vqdsnc.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://szz.yuxming.cn

[R72] 等待端口就绪
来源：http://grq.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nrw.yongpay.top

[R73] 分割大日志
来源：http://rlk.fehbvm.com

split -l 1000 big.log part_
来源：http://avv.hesvh.cn

[R74] 批量重命名
来源：http://lvm.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://znj.ydzc1.top

[R75] 导出环境变量
来源：http://zhn.dianchejie.cn

export PATH="$HOME/bin:$PATH"
来源：http://kic.jiagoushi.top

[R76] 使用临时文件
来源：http://jxl.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oxx.meibo888.top

[R77] 读取用户输入
来源：http://tdz.gaohongyu789.top

read -rp "请输入: " ans
来源：http://gww.ctjpmb.com

[R78] 交互式菜单
来源：http://dhl.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://egw.xuanzx.com

[R79] 解析命令行选项
来源：http://qqw.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kyp.shanyushiyangkeji.top

[R80] 查看脚本执行耗时
来源：http://zxo.yanxiufei.cn

time ./run.sh
来源：http://yya.fanxiaobao.xyz

================================================================================
来源：http://fpy.fanxiaobao.xyz

S. C / C++ 专题
来源：http://ksw.nwbrower.top

================================================================================
来源：http://srb.xingfuxueyuan.xyz

[S01] C：Hello World
来源：http://zzf.jiagoushi.top

#include <stdio.h>
来源：http://qvs.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gvv.nanxuanxn.top

[S02] C：变量与格式化输出
来源：http://yzi.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://crg.pengpengdd.cyou

[S03] C：读入整数
来源：http://vmi.fehbvm.com

int x; scanf("%d", &x);
来源：http://zrr.gotoacloud.top

[S04] C：字符串复制
来源：http://wcm.9152youxi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ejt.52xcode.cn

[S05] C：字符串长度
来源：http://ygs.guannengcc.top

strlen(s)
来源：http://jon.fengsongda.top

[S06] C：字符串比较
来源：http://tgr.fehbvm.com

strcmp(a, b) == 0
来源：http://vmo.yongpay.top

[S07] C：数组遍历求和
来源：http://otr.fzhhl.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hnf.tarul.cn

[S08] C：动态内存分配与释放
来源：http://ihi.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://azl.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://yen.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bka.yj202588.top

[S10] C：指针与解引用
来源：http://sgi.hongshengwenyu.top

int *p = &a;  *p = 5;
来源：http://wfr.zdqjudy.top

[S11] C：逐行读文件
来源：http://txs.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://gzc.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tie.tanke756.top

fclose(f);
来源：http://arc.cucudq.cn

[S12] C：写文件
来源：http://sbv.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rck.yangfankeji.com

[S13] C：宏定义
来源：http://fav.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://unk.yuanzhike.top

[S14] C：枚举
来源：http://flh.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://fpv.chenjidiqi.icu

[S15] C：类型转换
来源：http://nir.cheryme.top

(double) a / b
来源：http://rpi.havefunace.top

[S16] C：位操作置位
来源：http://fow.sufxvd.cn

x |= (1 << 3);
来源：http://xox.wangdashe.top

[S17] C：安全拼接字符串
来源：http://hhn.chenjidiqi.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kky.fehbvm.com

[S18] C：命令行参数
来源：http://lhf.jqgfzy.top

int main(int argc, char **argv)
来源：http://jqk.fktsv.cn

[S19] C：快速排序
来源：http://ctv.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://wwu.zdqjudy.top

[S20] C：二分查找
来源：http://vzu.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zqj.yj20258.top

[S21] C：字符类别判断
来源：http://nzi.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://max.c1oappe.top

[S22] C：字符串转数字
来源：http://dyo.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://kfd.ivvv.top

[S23] C：随机数
来源：http://esk.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qvx.yonumen.top

[S24] C：获取本地时间
来源：http://qsh.xinyue.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://plx.yvedp.cn

[S25] C：内存拷贝
来源：http://mkt.hywenlv.cn

memcpy(dst, src, n);
来源：http://qfu.dashuyun.cn

[S26] C：内存清零
来源：http://pxm.fengsongda.top

memset(a, 0, sizeof a);
来源：http://efj.ctjpmb.com

[S27] C：定义常量
来源：http://yju.xinyue.icu

const double PI = 3.14159;
来源：http://nrl.gaohongyu789.top

[S28] C：静态变量
来源：http://cfv.zycfv.cn

static int counter = 0;
来源：http://xwi.0kj1m.cn

[S29] C：变参函数
来源：http://uap.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eim.jiagoushi.top

[S30] C：头文件保护
来源：http://pap.cqqwz.cn

#ifndef X_H
来源：http://hpa.zycfv.cn

#define X_H
来源：http://nnu.shuidangran.top

#endif
来源：http://shz.shzxlz.cn

[S31] C++：Hello World
来源：http://oon.shangyingyoupin.top

#include <iostream>
来源：http://xwv.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://bfn.xinyue.icu

[S32] C++：字符串
来源：http://ehg.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://zzf.fengsongda.top

[S33] C++：vector 增删
来源：http://vzb.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jjh.fktsv.cn

[S34] C++：遍历 vector
来源：http://ahc.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://xdo.zdqjudy.top

[S35] C++：map
来源：http://jgu.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://emb.sjlbkw.cn

[S36] C++：unordered_map
来源：http://idy.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yai.shuidangran.top

[S37] C++：set
来源：http://tjj.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://scu.sjlbkw.cn

[S38] C++：排序
来源：http://lhr.yfazqb.com

std::sort(v.begin(), v.end());
来源：http://rzv.bjfxy.top

[S39] C++：自定义比较器排序
来源：http://irz.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uvh.zhongyouzk.top

[S40] C++：查找元素
来源：http://drj.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qrg.hammf.cn

[S41] C++：类与构造函数
来源：http://nov.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fkr.zycfv.cn

[S42] C++：继承与虚函数
来源：http://gss.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://gpl.yuanzhike.top

[S43] C++：智能指针
来源：http://ulu.xylfe.cn

auto p = std::make_unique<int>(5);
来源：http://ezp.hongshengwenyu.top

[S44] C++：引用传参
来源：http://bvh.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://gjo.gaohongyu789.top

[S45] C++：lambda
来源：http://rtu.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://fxw.tanke756.top

[S46] C++：函数模板
来源：http://mho.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qgc.ctjpmb.com

[S47] C++：结构化绑定遍历
来源：http://gij.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lwe.vehdjk.com

[S48] C++：逐行读文件
来源：http://zpr.xuetiantiany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tad.dashuyun.cn

while (std::getline(in, line)) { }
来源：http://ufp.0kj1m.cn

[S49] C++：写文件
来源：http://evs.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cfv.vqdsnc.cn

[S50] C++：格式化数字
来源：http://ftx.yongpay.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aaf.meibo888.top

[S51] C++：显式类型转换
来源：http://eab.snrcjt.cn

static_cast<double>(a) / b
来源：http://hmw.ywan-chungtsiang.top

[S52] C++：const 与 noexcept
来源：http://qtb.cashguo.top

int size() const noexcept { return n_; }
来源：http://zdu.aizwys.cn

[S53] C++：移动语义
来源：http://ylh.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://vxx.jiagoushi.top

[S54] C++：异常处理
来源：http://esm.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ycj.epnwcf.com

[S55] C++：结构化绑定
来源：http://ljt.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://flb.chenzaomai.com

[S56] C++：optional
来源：http://zux.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sgn.shuidangran.top

[S57] C++：编译期常量
来源：http://fya.xinyue.icu

constexpr int N = 10;
来源：http://cjf.mhx1999.top

[S58] C++：命名空间
来源：http://dxt.sysykeji.top

namespace ns { int f() { return 1; } }
来源：http://hgp.sjlbkw.cn

[S59] C++：静态断言
来源：http://ppq.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://orl.yj20258.top

[S60] C++：遍历并删除元素
来源：http://wja.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wyv.yangfankeji.com

================================================================================
来源：http://osk.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tpo.nanxuanxn.top

================================================================================
来源：http://mxi.daria6918.cn

[T01] Kotlin：Hello World
来源：http://utn.shanyushiyangkeji.top

println("Hello")
来源：http://ysp.jiagoushi.top

[T02] Kotlin：变量
来源：http://prt.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vpa.tarul.cn

[T03] Kotlin：字符串模板
来源：http://ilp.cqqwz.cn

"值: $b"
来源：http://yuq.tarul.cn

[T04] Kotlin：空安全
来源：http://zlx.shanyushiyangtech.top

val n: String? = null;  n?.length
来源：http://njv.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://pji.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tqu.smart0.xyz

[T06] Kotlin：集合映射
来源：http://wly.svipenyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ckk.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://tqa.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zne.hesvh.cn

[T08] Kotlin：数据类
来源：http://tyd.wangdashe.top

data class User(val name: String, val age: Int)
来源：http://jvt.yongpay.top

[T09] Kotlin：扩展函数
来源：http://axo.hesvh.cn

fun String.exclaim() = this + "!"
来源：http://ohm.ehwqpu.com

[T10] Kotlin：默认参数
来源：http://ygo.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://opd.guannengcc.top

[T11] Kotlin：协程
来源：http://lll.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gud.hongshengwenyu.top

[T12] Kotlin：解构声明
来源：http://tgj.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://ezi.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://xqi.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://xhu.jlsjyb.cn

[T14] Kotlin：循环
来源：http://tyb.ydzc1.top

for (i in 1..10) println(i)
来源：http://bqg.redwolf501.top

[T15] Kotlin：接口
来源：http://cdc.yj20258888.top

interface Shape { fun area(): Double }
来源：http://rhe.yonumen.top

[T16] Swift：Hello World
来源：http://rfx.chenjidiqi.icu

print("Hello")
来源：http://vdi.hysaishi.cn

[T17] Swift：变量与常量
来源：http://lnh.cdnleiting.top

var a = 1;  let b = 2
来源：http://ugk.tarul.cn

[T18] Swift：字符串插值
来源：http://ufk.0kj1m.cn

"值: \(b)"
来源：http://ppv.snrcjt.cn

[T19] Swift：可选绑定
来源：http://ikr.chenlongwang.top

if let n = opt { print(n) }
来源：http://poi.havefunace.top

[T20] Swift：数组操作
来源：http://ikq.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://kzk.sjlbkw.cn

[T21] Swift：遍历
来源：http://zcz.tanke756.top

for x in a { print(x) }
来源：http://dfw.quarkkingdee.top

[T22] Swift：字典
来源：http://fon.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wyo.sjlbkw.cn

[T23] Swift：函数
来源：http://lho.hnqzz.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://emg.uphjek.com

[T24] Swift：闭包
来源：http://myr.xuanzx.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://tsy.vehdjk.com

[T25] Swift：结构体
来源：http://xxs.bjfxy.top

struct P { var x: Int }
来源：http://mwo.yvedp.cn

[T26] Swift：类与重写
来源：http://nzo.zdbjq.cn

class A: Base { override func f() {} }
来源：http://sud.yangfankeji.com

[T27] Swift：错误处理
来源：http://pyn.aizwys.cn

do { try f() } catch { print(error) }
来源：http://qbu.nanxinkj.top

[T28] Swift：枚举
来源：http://jvd.yj202588.top

enum Color { case red, green }
来源：http://kxi.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://ksp.sweek.top

guard let x = opt else { return }
来源：http://sfq.yj20258.top

[T30] Swift：协议
来源：http://nyn.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://bah.guowangkeji.top

[T31] Lua：Hello World
来源：http://jyl.sjlbkw.cn

print("Hello")
来源：http://eam.hnqzz.top

[T32] Lua：局部变量
来源：http://zgq.fehbvm.com

local a = 1
来源：http://erj.zhaomingkeji.xyz

[T33] Lua：表（数组）
来源：http://gvn.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://hwt.yuanzhike.top

[T34] Lua：遍历表
来源：http://oqh.gaohongyu789.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jwe.epnwcf.com

[T35] Lua：字典表
来源：http://slv.dashuyun.cn

local d = { a = 1 };  d.b = 2
来源：http://pdg.ehwqpu.com

[T36] Lua：函数
来源：http://kgz.fengsongda.top

function add(a, b) return a + b end
来源：http://kym.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://zcg.ydzc1.top

"a" .. "b"
来源：http://fts.xziqi.cn

[T38] Lua：条件
来源：http://esw.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://aad.zhengqikj.top

[T39] Lua：模式匹配
来源：http://uem.gotoacloud.top

string.find(s, "%d+")
来源：http://glh.jqgfzy.top

[T40] Lua：元表
来源：http://jfc.xziqi.cn

setmetatable({}, { __index = base })
来源：http://kuo.daria6918.cn

[T41] Perl：Hello World
来源：http://zis.52xcode.cn

print "Hello\n";
来源：http://beh.redwolf501.top

[T42] Perl：变量类型
来源：http://deq.shanyushiyangtech.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nfu.guowangkeji.top

[T43] Perl：字符串插值
来源：http://vtm.shuidangran.top

"值: $a"
来源：http://par.cashguo.top

[T44] Perl：条件
来源：http://flf.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://pix.sweek.top

[T45] Perl：数组遍历
来源：http://wgt.cheryme.top

for my $x (@arr) { print $x; }
来源：http://jxi.jqgufenzy.top

[T46] Perl：哈希操作
来源：http://pky.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://elw.sufxvd.cn

[T47] Perl：正则捕获
来源：http://weg.guowangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rpc.gaohongyu789.top

[T48] Perl：正则替换
来源：http://kvj.yongpay.top

$s =~ s/old/new/g;
来源：http://grz.cheryme.top

[T49] Perl：函数
来源：http://tze.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://upp.hysaishi.cn

[T50] Perl：逐行读文件
来源：http://vpg.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jdj.dianchejie.cn

while (my $line = <$fh>) { print $line; }
来源：http://vje.guowangkeji.top

[T51] Scala：Hello World
来源：http://ddf.fengsongda.top

println("Hello")
来源：http://rvf.jinyuanbaomall.cn

[T52] Scala：变量
来源：http://pgc.gogol.net.cn

val a = 1;  var b = 2
来源：http://jti.sweek.top

[T53] Scala：字符串插值
来源：http://npk.hesvh.cn

s"值: $b"
来源：http://mpf.daria6918.cn

[T54] Scala：集合映射
来源：http://vdr.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://dby.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://iie.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://dig.vehdjk.com

[T56] Scala：样例类
来源：http://sei.yangfankeji.com

case class User(name: String, age: Int)
来源：http://eou.yangfankeji.com

[T57] Scala：模式匹配
来源：http://kuc.fzhhl.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gbk.yj202588.top

[T58] Scala：函数定义
来源：http://dpq.ywan-chungtsiang.top

def add(a: Int, b: Int): Int = a + b
来源：http://vqv.xingfuxueyuan.xyz

[T59] Scala：循环
来源：http://ebe.ehwqpu.com

for (i <- 1 to 10) println(i)
来源：http://zvk.jinqigfzy.top

[T60] Scala：折叠
来源：http://bhc.ctjpmb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fpx.wangdashe.top

================================================================================
来源：http://kyz.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fku.kuanghao11.cn

================================================================================
来源：http://jzv.zhaomingkeji.xyz

[U01] Py：创建虚拟环境
来源：http://oiq.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://kxb.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://nsr.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oeh.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://fpf.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gwy.fehbvm.com

[U04] Py：变量调试打印
来源：http://etf.xingfuxueyuan.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kqy.gaohongyu789.top


<!-- 参考信息 -->