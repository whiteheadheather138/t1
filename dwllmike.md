代发 wailian999

df -h;  du -sh *
来源：http://udp.jlsjyb.cn

[R62] 找最占空间的文件
来源：http://trq.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://dov.ydzc1.top

[R63] 内存与进程
来源：http://dly.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://ewi.yongpay.top

[R64] 结束进程
来源：http://drf.52xcode.cn

kill -9 $(pgrep -f app.py)
来源：http://itw.hcnkem.com

[R65] 查看端口占用
来源：http://oba.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vax.guannengcc.top

[R66] 定时任务
来源：http://lnk.ydzc1.top

crontab -e;  crontab -l
来源：http://zvn.tarul.cn

[R67] 生成随机十六进制串
来源：http://quv.hammf.cn

openssl rand -hex 16
来源：http://orz.yvedp.cn

[R68] 计算文件校验值
来源：http://vmt.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tio.sjlbkw.cn

[R69] 生成随机密码
来源：http://hao.yj202588.top

head -c 16 /dev/urandom | base64
来源：http://trf.vehdjk.com

[R70] 时间戳与互转
来源：http://inh.dashuyun.cn

date +%s;  date -d @1700000000
来源：http://zbx.ydjk.org.cn

[R71] 日期格式化
来源：http://aye.havefunace.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wdb.tarul.cn

[R72] 等待端口就绪
来源：http://ddn.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ema.hongshengwenyu.top

[R73] 分割大日志
来源：http://ubx.vehdjk.com

split -l 1000 big.log part_
来源：http://pub.jyoumei.cn

[R74] 批量重命名
来源：http://ldv.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ukj.cashguo.top

[R75] 导出环境变量
来源：http://oeg.zycfv.cn

export PATH="$HOME/bin:$PATH"
来源：http://scz.sufxvd.cn

[R76] 使用临时文件
来源：http://kcg.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bpe.xuanzx.com

[R77] 读取用户输入
来源：http://xgu.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://oqt.chenjidiqi.icu

[R78] 交互式菜单
来源：http://obh.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zzz.iojbl.cn

[R79] 解析命令行选项
来源：http://lab.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hhs.jinyuanbaomall.cn

[R80] 查看脚本执行耗时
来源：http://nbm.52xcode.cn

time ./run.sh
来源：http://eji.ydjk.org.cn

================================================================================
来源：http://qst.ybcxt.top

S. C / C++ 专题
来源：http://msr.guannengcc.top

================================================================================
来源：http://bhf.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://qzf.sxryk.cn

#include <stdio.h>
来源：http://odf.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://fxf.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://rui.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://lrq.xuetiantiany.cn

[S03] C：读入整数
来源：http://zmw.bbcook.cn

int x; scanf("%d", &x);
来源：http://zxq.yfazqb.com

[S04] C：字符串复制
来源：http://zrh.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://cnp.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://dgr.hongshengwenyu.top

strlen(s)
来源：http://dkg.gogol.net.cn

[S06] C：字符串比较
来源：http://zhl.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://rjw.jiagoushi.top

[S07] C：数组遍历求和
来源：http://jeo.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fwx.pengpengdd.cyou

[S08] C：动态内存分配与释放
来源：http://ufj.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dvj.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://vce.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sfa.ydjk.org.cn

[S10] C：指针与解引用
来源：http://kzl.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://kae.quarkkingdee.top

[S11] C：逐行读文件
来源：http://vhq.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://wlv.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mko.yvedp.cn

fclose(f);
来源：http://yuw.jinqigufen.top

[S12] C：写文件
来源：http://mql.52xcode.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lhl.guowangkeji.top

[S13] C：宏定义
来源：http://ika.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://num.mhx1999.top

[S14] C：枚举
来源：http://rsy.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://jym.cheryme.top

[S15] C：类型转换
来源：http://nni.daria6918.cn

(double) a / b
来源：http://brd.ppjwa.cn

[S16] C：位操作置位
来源：http://jed.snrcjt.cn

x |= (1 << 3);
来源：http://hua.yvedp.cn

[S17] C：安全拼接字符串
来源：http://cqk.sxryk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nes.jyoumei.cn

[S18] C：命令行参数
来源：http://fhy.vqdsnc.cn

int main(int argc, char **argv)
来源：http://dns.ehwqpu.com

[S19] C：快速排序
来源：http://bpf.yongpay.top

qsort(a, n, sizeof(int), cmp);
来源：http://mzd.fehbvm.com

[S20] C：二分查找
来源：http://tpd.hesvh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kse.c1oappe.top

[S21] C：字符类别判断
来源：http://urh.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xti.fengsongda.top

[S22] C：字符串转数字
来源：http://mid.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://vxe.andypj.xyz

[S23] C：随机数
来源：http://rrj.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vxu.9152youxi.cn

[S24] C：获取本地时间
来源：http://jej.aizwys.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vcl.sjlbkw.cn

[S25] C：内存拷贝
来源：http://pcu.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://ydi.yfazqb.com

[S26] C：内存清零
来源：http://kep.aizwys.cn

memset(a, 0, sizeof a);
来源：http://hbw.yanxiufei.cn

[S27] C：定义常量
来源：http://epx.meibo888.top

const double PI = 3.14159;
来源：http://llj.mhx1999.top

[S28] C：静态变量
来源：http://sno.cqqwz.cn

static int counter = 0;
来源：http://xve.316326.xyz

[S29] C：变参函数
来源：http://kyr.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ueg.yj20258888.top

[S30] C：头文件保护
来源：http://xwb.yj20258888.top

#ifndef X_H
来源：http://pls.hfpthk.cn

#define X_H
来源：http://lck.xylfe.cn

#endif
来源：http://wrt.yueranfly.top

[S31] C++：Hello World
来源：http://rqa.yvedp.cn

#include <iostream>
来源：http://afe.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://flq.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://ams.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://awd.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://ggn.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ppn.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://eex.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://seg.dianchejie.cn

[S35] C++：map
来源：http://dry.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lro.daria6918.cn

[S36] C++：unordered_map
来源：http://qzc.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://viy.chenlongwang.top

[S37] C++：set
来源：http://bol.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tcs.cqqwz.cn

[S38] C++：排序
来源：http://ulf.wangshuangyany.cn

std::sort(v.begin(), v.end());
来源：http://mbi.ybcxt.top

[S39] C++：自定义比较器排序
来源：http://bnr.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mad.nanxuanxn.top

[S40] C++：查找元素
来源：http://gxd.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://peu.havefunace.top

[S41] C++：类与构造函数
来源：http://mih.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://opv.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://txi.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://stm.nanxinkj.top

[S43] C++：智能指针
来源：http://bkk.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://hmz.kuanghao11.cn

[S44] C++：引用传参
来源：http://uje.tarul.cn

void inc(int &x) { ++x; }
来源：http://xwo.shzxlz.cn

[S45] C++：lambda
来源：http://pvm.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tvq.yvedp.cn

[S46] C++：函数模板
来源：http://rsn.tarul.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nvp.hysaishi.cn

[S47] C++：结构化绑定遍历
来源：http://bdc.pengpengdd.cyou

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zsf.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://dvj.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://rro.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://hha.fehbvm.com

[S49] C++：写文件
来源：http://zrs.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://emf.daxiang520.top

[S50] C++：格式化数字
来源：http://lpw.fanxiaobao.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hhw.zycfv.cn

[S51] C++：显式类型转换
来源：http://wle.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://dtl.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://lmt.shuidangran.top

int size() const noexcept { return n_; }
来源：http://ltk.nwbrower.top

[S53] C++：移动语义
来源：http://ziu.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://kuc.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://vxj.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://imf.jlsjyb.cn

[S55] C++：结构化绑定
来源：http://zfx.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://hax.ctjpmb.com

[S56] C++：optional
来源：http://cfq.jinqigufen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uzb.meibo888.top

[S57] C++：编译期常量
来源：http://kup.fehbvm.com

constexpr int N = 10;
来源：http://kol.dianchejie.cn

[S58] C++：命名空间
来源：http://efz.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://hli.yangfankeji.com

[S59] C++：静态断言
来源：http://qhc.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ooj.havefunace.top

[S60] C++：遍历并删除元素
来源：http://omv.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rnk.guannengcc.top

================================================================================
来源：http://clq.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yxa.jlsjyb.cn

================================================================================
来源：http://vei.bbcook.cn

[T01] Kotlin：Hello World
来源：http://ahn.meibo888.top

println("Hello")
来源：http://kqr.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://yuu.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rdy.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://lhr.aibaodan.cn

"值: $b"
来源：http://hnr.tarul.cn

[T04] Kotlin：空安全
来源：http://uxu.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://luj.tarul.cn

[T05] Kotlin：when 表达式
来源：http://xfk.zhixingplan.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fgv.havefunace.top

[T06] Kotlin：集合映射
来源：http://inz.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://pcq.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://pzf.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iht.yuxming.cn

[T08] Kotlin：数据类
来源：http://lrn.andypj.xyz

data class User(val name: String, val age: Int)
来源：http://hpl.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://uhp.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://azy.cashguo.top

[T10] Kotlin：默认参数
来源：http://wkt.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://esj.c1oappe.top

[T11] Kotlin：协程
来源：http://otw.aibaodan.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gss.daxiang520.top

[T12] Kotlin：解构声明
来源：http://wle.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://qrm.xingfuxueyuan.xyz

[T13] Kotlin：只读 Map
来源：http://mwv.vqdsnc.cn

val m = mapOf("a" to 1)
来源：http://tbz.jianghu66.top

[T14] Kotlin：循环
来源：http://yxo.meibo888.top

for (i in 1..10) println(i)
来源：http://qrq.yj20258.top

[T15] Kotlin：接口
来源：http://xvt.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://drm.jqgfzy.top

[T16] Swift：Hello World
来源：http://nsm.hnqzz.top

print("Hello")
来源：http://flh.hammf.cn

[T17] Swift：变量与常量
来源：http://xor.xuanzx.com

var a = 1;  let b = 2
来源：http://ser.wangshuangyany.cn

[T18] Swift：字符串插值
来源：http://sjs.ybcxt.top

"值: \(b)"
来源：http://oul.dianchejie.cn

[T19] Swift：可选绑定
来源：http://zuj.yongpay.top

if let n = opt { print(n) }
来源：http://klr.andypj.xyz

[T20] Swift：数组操作
来源：http://jrr.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ldr.tanke756.top

[T21] Swift：遍历
来源：http://bxe.hongshengwenyu.top

for x in a { print(x) }
来源：http://gsd.redwolf501.top

[T22] Swift：字典
来源：http://ahh.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://ebp.shuidangran.top

[T23] Swift：函数
来源：http://ozw.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rjy.ywan-chungtsiang.top

[T24] Swift：闭包
来源：http://yay.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ded.daxiang520.top

[T25] Swift：结构体
来源：http://xgi.tarul.cn

struct P { var x: Int }
来源：http://jgu.yongpay.top

[T26] Swift：类与重写
来源：http://egm.redwolf501.top

class A: Base { override func f() {} }
来源：http://yxd.316326.xyz

[T27] Swift：错误处理
来源：http://hzj.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://tkt.xingfuxueyuan.xyz

[T28] Swift：枚举
来源：http://rhu.zdqjudy.top

enum Color { case red, green }
来源：http://erb.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://tsa.yanxiufei.cn

guard let x = opt else { return }
来源：http://ojm.wangdashe.top

[T30] Swift：协议
来源：http://tem.jianghu66.top

protocol Shape { func area() -> Double }
来源：http://bkw.zhengqikj.top

[T31] Lua：Hello World
来源：http://mbn.aibaodan.cn

print("Hello")
来源：http://auv.hnxiangtu.top

[T32] Lua：局部变量
来源：http://ilo.ehwqpu.com

local a = 1
来源：http://iym.dianchejie.cn

[T33] Lua：表（数组）
来源：http://qfb.zhiwuduotai.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vmg.pycfn.com

[T34] Lua：遍历表
来源：http://equ.ivvv.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fwd.svipenyu.cn

[T35] Lua：字典表
来源：http://dfk.gogol.net.cn

local d = { a = 1 };  d.b = 2
来源：http://bdq.shuidangran.top

[T36] Lua：函数
来源：http://nuw.ydzc1.top

function add(a, b) return a + b end
来源：http://wwc.birdmap.top

[T37] Lua：字符串拼接
来源：http://uen.zhiwuduotai.top

"a" .. "b"
来源：http://qdr.dianchejie.cn

[T38] Lua：条件
来源：http://daz.aibaodan.cn

if x > 0 then print("正") end
来源：http://rwt.gaohongyu789.top

[T39] Lua：模式匹配
来源：http://ios.hnqzz.top

string.find(s, "%d+")
来源：http://okp.gotoacloud.top

[T40] Lua：元表
来源：http://wdx.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://uuc.jiagoushi.top

[T41] Perl：Hello World
来源：http://scr.gaohongyu789.top

print "Hello\n";
来源：http://iqz.zdbjq.cn

[T42] Perl：变量类型
来源：http://zcy.bjfxy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eel.xuanzx.com

[T43] Perl：字符串插值
来源：http://nts.ywan-chungtsiang.top

"值: $a"
来源：http://vuy.jinyuanbaomall.cn

[T44] Perl：条件
来源：http://msj.aizwys.cn

if ($a > 0) { print "正"; }
来源：http://mwo.shzxlz.cn

[T45] Perl：数组遍历
来源：http://iza.chenzaomai.com

for my $x (@arr) { print $x; }
来源：http://qmt.tarul.cn

[T46] Perl：哈希操作
来源：http://xel.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fbm.sweek.top

[T47] Perl：正则捕获
来源：http://rvq.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wrf.fengsongda.top

[T48] Perl：正则替换
来源：http://emu.guannengcc.top

$s =~ s/old/new/g;
来源：http://urf.52xcode.cn

[T49] Perl：函数
来源：http://qks.guannengcc.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ekt.mhx1999.top

[T50] Perl：逐行读文件
来源：http://ole.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://vai.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://zgk.0kj1m.cn

[T51] Scala：Hello World
来源：http://icb.jqgfzy.top

println("Hello")
来源：http://fln.tanke756.top

[T52] Scala：变量
来源：http://eft.cashguo.top

val a = 1;  var b = 2
来源：http://jgn.svipenyu.cn

[T53] Scala：字符串插值
来源：http://cao.guannengcc.top

s"值: $b"
来源：http://mrz.zhiwuduotai.top

[T54] Scala：集合映射
来源：http://cdw.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://evo.fzhhl.top

[T55] Scala：集合过滤
来源：http://mpw.ehwqpu.com

List(1, 2, 3).filter(_ > 1)
来源：http://urr.dashuyun.cn

[T56] Scala：样例类
来源：http://wok.9152youxi.cn

case class User(name: String, age: Int)
来源：http://djv.haohaochexian.top

[T57] Scala：模式匹配
来源：http://zot.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mmd.meibo888.top

[T58] Scala：函数定义
来源：http://peh.gaohongyu789.top

def add(a: Int, b: Int): Int = a + b
来源：http://kjr.yanxiufei.cn

[T59] Scala：循环
来源：http://cca.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://vlz.tarul.cn

[T60] Scala：折叠
来源：http://hqf.ybcxt.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://akw.fengsongda.top

================================================================================
来源：http://hvj.wangdashe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://njs.guannengcc.top

================================================================================
来源：http://pmv.ivvv.top

[U01] Py：创建虚拟环境
来源：http://hhy.hesvh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uyj.bjfxy.top

[U02] Py：导出 / 安装依赖
来源：http://uog.jiagoushi.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fvp.yvedp.cn


<!-- 参考信息 -->