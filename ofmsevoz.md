代发 wailian999

openssl rand -hex 16
来源：http://ynf.gzhubu.top

[R68] 计算文件校验值
来源：http://eym.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zjd.mhx1999.top

[R69] 生成随机密码
来源：http://byv.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://imy.jianghu66.top

[R70] 时间戳与互转
来源：http://onf.bjfxy.top

date +%s;  date -d @1700000000
来源：http://huk.sufxvd.cn

[R71] 日期格式化
来源：http://tem.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jid.gzhubu.top

[R72] 等待端口就绪
来源：http://ode.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jtr.pengpengdd.cyou

[R73] 分割大日志
来源：http://ocp.xingfuxueyuan.xyz

split -l 1000 big.log part_
来源：http://zut.wangdashe.top

[R74] 批量重命名
来源：http://abg.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://emq.zhixingplan.top

[R75] 导出环境变量
来源：http://onv.yj20258.top

export PATH="$HOME/bin:$PATH"
来源：http://jxd.shuidangran.top

[R76] 使用临时文件
来源：http://gxn.jqgfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://byu.xinyue.icu

[R77] 读取用户输入
来源：http://rte.daxiang520.top

read -rp "请输入: " ans
来源：http://lzf.shanyushiyangkeji.top

[R78] 交互式菜单
来源：http://gfv.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wds.tarul.cn

[R79] 解析命令行选项
来源：http://zss.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yec.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://cqc.ehwqpu.com

time ./run.sh
来源：http://rme.zhoulong.xyz

================================================================================
来源：http://hmw.yongpay.top

S. C / C++ 专题
来源：http://xop.tianlin.xyz

================================================================================
来源：http://hdt.quarkkingdee.top

[S01] C：Hello World
来源：http://vbj.52xcode.cn

#include <stdio.h>
来源：http://ocq.guannengcc.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://scl.tanke756.top

[S02] C：变量与格式化输出
来源：http://amk.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://lze.ppjwa.cn

[S03] C：读入整数
来源：http://bnu.hnqzz.top

int x; scanf("%d", &x);
来源：http://gaw.daria6918.cn

[S04] C：字符串复制
来源：http://veh.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://xpz.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://pkn.dianchejie.cn

strlen(s)
来源：http://kmf.jqgfzy.top

[S06] C：字符串比较
来源：http://nxw.andypj.xyz

strcmp(a, b) == 0
来源：http://rsi.yfazqb.com

[S07] C：数组遍历求和
来源：http://ijo.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oap.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://jva.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nyi.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://gic.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hyq.bjfxy.top

[S10] C：指针与解引用
来源：http://cdw.dashuyun.cn

int *p = &a;  *p = 5;
来源：http://htr.snrcjt.cn

[S11] C：逐行读文件
来源：http://wzk.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://bsc.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eer.hysaishi.cn

fclose(f);
来源：http://wff.cheryme.top

[S12] C：写文件
来源：http://jek.tian-w.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wyu.jqgufenzy.top

[S13] C：宏定义
来源：http://jjp.316326.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kfg.fanxiaobao.xyz

[S14] C：枚举
来源：http://slm.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://koa.tian-w.cn

[S15] C：类型转换
来源：http://zpf.yj20258.top

(double) a / b
来源：http://pot.nanxinkj.top

[S16] C：位操作置位
来源：http://hxx.smart0.xyz

x |= (1 << 3);
来源：http://rwm.hnxiangtu.top

[S17] C：安全拼接字符串
来源：http://kff.vehdjk.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iye.shzxlz.cn

[S18] C：命令行参数
来源：http://lxu.quarkkingdee.top

int main(int argc, char **argv)
来源：http://fzy.fengsongda.top

[S19] C：快速排序
来源：http://ydd.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://dya.hammf.cn

[S20] C：二分查找
来源：http://kgo.svipenyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lah.mhx1999.top

[S21] C：字符类别判断
来源：http://ikm.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gej.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://ffb.hnxiangtu.top

atoi("42");  strtod("3.14", NULL);
来源：http://ani.jqgufenzy.top

[S23] C：随机数
来源：http://agb.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xlw.hfpthk.cn

[S24] C：获取本地时间
来源：http://jam.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vlc.yonumen.top

[S25] C：内存拷贝
来源：http://hkd.chenlongwang.top

memcpy(dst, src, n);
来源：http://yxe.yangfankeji.com

[S26] C：内存清零
来源：http://zyg.shanyushiyangkeji.top

memset(a, 0, sizeof a);
来源：http://lnb.zdbjq.cn

[S27] C：定义常量
来源：http://ghn.tianlin.xyz

const double PI = 3.14159;
来源：http://wbn.c1oappe.top

[S28] C：静态变量
来源：http://tug.mhx1999.top

static int counter = 0;
来源：http://jkr.sysykeji.top

[S29] C：变参函数
来源：http://mmq.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://taq.yanxiufei.cn

[S30] C：头文件保护
来源：http://wyq.fktsv.cn

#ifndef X_H
来源：http://nin.birdmap.top

#define X_H
来源：http://vqr.shuidangran.top

#endif
来源：http://sib.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://ckl.tarul.cn

#include <iostream>
来源：http://udk.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://sra.daxiang520.top

[S32] C++：字符串
来源：http://ucr.uphjek.com

std::string s = "hi";  s += "!";
来源：http://pnp.hammf.cn

[S33] C++：vector 增删
来源：http://uos.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qsl.fengsongda.top

[S34] C++：遍历 vector
来源：http://dja.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://bhy.fengsongda.top

[S35] C++：map
来源：http://gdd.guowangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xjn.andypj.xyz

[S36] C++：unordered_map
来源：http://btd.andypj.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bvf.yfazqb.com

[S37] C++：set
来源：http://zsr.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jqx.tianlin.xyz

[S38] C++：排序
来源：http://zqd.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://mdu.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://vxa.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vbg.0kj1m.cn

[S40] C++：查找元素
来源：http://ayt.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vfa.hnqzz.top

[S41] C++：类与构造函数
来源：http://gwg.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://akj.yj202588.top

[S42] C++：继承与虚函数
来源：http://xtp.tian-w.cn

class B : public Base { public: void f() override {} };
来源：http://bbh.nwbrower.top

[S43] C++：智能指针
来源：http://glh.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://frn.quarkkingdee.top

[S44] C++：引用传参
来源：http://yyl.yonumen.top

void inc(int &x) { ++x; }
来源：http://clc.tian-w.cn

[S45] C++：lambda
来源：http://lqw.zhongyouzk.top

auto add = [](int a, int b) { return a + b; };
来源：http://mab.fehbvm.com

[S46] C++：函数模板
来源：http://uae.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://khg.zhaomingkeji.xyz

[S47] C++：结构化绑定遍历
来源：http://cyx.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yvd.xuanzx.com

[S48] C++：逐行读文件
来源：http://feo.fengsongda.top

std::ifstream in("a.txt");  std::string line;
来源：http://zox.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://pil.yj20258888.top

[S49] C++：写文件
来源：http://xwt.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mgc.aibaodan.cn

[S50] C++：格式化数字
来源：http://rhh.9152youxi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://svy.shzxlz.cn

[S51] C++：显式类型转换
来源：http://kbf.nanxuanxn.top

static_cast<double>(a) / b
来源：http://mzs.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://xbr.hongshengwenyu.top

int size() const noexcept { return n_; }
来源：http://xmc.zhongyouzk.top

[S53] C++：移动语义
来源：http://dfe.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://mac.jyoumei.cn

[S54] C++：异常处理
来源：http://wok.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oou.jiagoushi.top

[S55] C++：结构化绑定
来源：http://cno.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://ioz.havefunace.top

[S56] C++：optional
来源：http://snk.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hfe.ehwqpu.com

[S57] C++：编译期常量
来源：http://wkc.xinyue.icu

constexpr int N = 10;
来源：http://tgt.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://eka.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://nqy.jqgufenzy.top

[S59] C++：静态断言
来源：http://gpz.vehdjk.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bit.tanke756.top

[S60] C++：遍历并删除元素
来源：http://bcr.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mkk.ybcxt.top

================================================================================
来源：http://vin.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://omk.jinyuanbaomall.cn

================================================================================
来源：http://zal.yvedp.cn

[T01] Kotlin：Hello World
来源：http://wuf.yueranfly.top

println("Hello")
来源：http://hpz.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://nyl.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bun.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://fuw.aizwys.cn

"值: $b"
来源：http://zyo.hysaishi.cn

[T04] Kotlin：空安全
来源：http://jjw.gzhubu.top

val n: String? = null;  n?.length
来源：http://ues.xingfuxueyuan.xyz

[T05] Kotlin：when 表达式
来源：http://qaa.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nbk.ybcxt.top

[T06] Kotlin：集合映射
来源：http://ora.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yte.zdqjudy.top

[T07] Kotlin：集合过滤
来源：http://zsj.ehwqpu.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://rxz.yj202588.top

[T08] Kotlin：数据类
来源：http://yfa.ydzc1.top

data class User(val name: String, val age: Int)
来源：http://uaz.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://ice.jlsjyb.cn

fun String.exclaim() = this + "!"
来源：http://iro.hammf.cn

[T10] Kotlin：默认参数
来源：http://ypj.pengpengdd.cyou

fun greet(name: String = "World") = "Hi $name"
来源：http://rio.sxryk.cn

[T11] Kotlin：协程
来源：http://ghd.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://bjv.sxryk.cn

[T12] Kotlin：解构声明
来源：http://oyz.jinyuanbaomall.cn

val (a, b) = Pair(1, 2)
来源：http://hsw.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://ddh.yangfankeji.com

val m = mapOf("a" to 1)
来源：http://czn.nanxuanxn.top

[T14] Kotlin：循环
来源：http://kph.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://fws.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://rgk.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://slb.hysaishi.cn

[T16] Swift：Hello World
来源：http://kuo.yuanzhike.top

print("Hello")
来源：http://uwp.jinqigfzy.top

[T17] Swift：变量与常量
来源：http://uix.nanxinkj.top

var a = 1;  let b = 2
来源：http://iet.xylfe.cn

[T18] Swift：字符串插值
来源：http://hjl.kuanghao11.cn

"值: \(b)"
来源：http://ici.iojbl.cn

[T19] Swift：可选绑定
来源：http://qyt.epnwcf.com

if let n = opt { print(n) }
来源：http://jap.wangdashe.top

[T20] Swift：数组操作
来源：http://cbj.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://pck.yongpay.top

[T21] Swift：遍历
来源：http://sqp.yvedp.cn

for x in a { print(x) }
来源：http://vtj.fanxiaobao.xyz

[T22] Swift：字典
来源：http://lzq.jiagoushi.top

var d = ["a": 1];  d["b"] = 2
来源：http://sxg.xylfe.cn

[T23] Swift：函数
来源：http://mws.jlsjyb.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://akr.zdqjudy.top

[T24] Swift：闭包
来源：http://jwd.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://dnn.sjlbkw.cn

[T25] Swift：结构体
来源：http://cel.zhongyouzk.top

struct P { var x: Int }
来源：http://vvw.chenjidiqi.icu

[T26] Swift：类与重写
来源：http://dnn.birdmap.top

class A: Base { override func f() {} }
来源：http://hwl.jqgufenzy.top

[T27] Swift：错误处理
来源：http://hbv.jinqigufen.top

do { try f() } catch { print(error) }
来源：http://lmh.xuetiantiany.cn

[T28] Swift：枚举
来源：http://fus.zhiwuduotai.top

enum Color { case red, green }
来源：http://xad.hongshengwenyu.top

[T29] Swift：guard 提前返回
来源：http://biz.zhiwuduotai.top

guard let x = opt else { return }
来源：http://isx.gotoacloud.top

[T30] Swift：协议
来源：http://kzv.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://xve.hesvh.cn

[T31] Lua：Hello World
来源：http://pxs.tanke756.top

print("Hello")
来源：http://hwg.52xcode.cn

[T32] Lua：局部变量
来源：http://olz.cucudq.cn

local a = 1
来源：http://gbm.shanyushiyangtech.top

[T33] Lua：表（数组）
来源：http://tdh.yongpay.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vuf.dianchejie.cn

[T34] Lua：遍历表
来源：http://gkf.zhengqikj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://odv.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://anw.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://ytc.jinyuanbaomall.cn

[T36] Lua：函数
来源：http://olx.epnwcf.com

function add(a, b) return a + b end
来源：http://zbh.gogol.net.cn

[T37] Lua：字符串拼接
来源：http://nwy.gogol.net.cn

"a" .. "b"
来源：http://xlm.nanxinkj.top

[T38] Lua：条件
来源：http://npe.fktsv.cn

if x > 0 then print("正") end
来源：http://pyb.chenlongwang.top

[T39] Lua：模式匹配
来源：http://wuq.guowangkeji.top

string.find(s, "%d+")
来源：http://yry.hnqzz.top

[T40] Lua：元表
来源：http://whd.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://lwq.daxiang520.top

[T41] Perl：Hello World
来源：http://tqb.jinghuilouyu.cn

print "Hello\n";
来源：http://ias.jlsjyb.cn

[T42] Perl：变量类型
来源：http://fux.9152youxi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://siu.sjlbkw.cn

[T43] Perl：字符串插值
来源：http://eey.smart0.xyz

"值: $a"
来源：http://bbu.zhoulong.xyz

[T44] Perl：条件
来源：http://ffl.birdmap.top

if ($a > 0) { print "正"; }
来源：http://exz.tanke756.top

[T45] Perl：数组遍历
来源：http://fry.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://qsg.hnqzz.top

[T46] Perl：哈希操作
来源：http://ckf.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://djx.hnxiangtu.top

[T47] Perl：正则捕获
来源：http://vrq.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://com.jiagoushi.top

[T48] Perl：正则替换
来源：http://bcd.xylfe.cn

$s =~ s/old/new/g;
来源：http://dtj.xinyue.icu

[T49] Perl：函数
来源：http://cep.xziqi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gct.vqdsnc.cn

[T50] Perl：逐行读文件
来源：http://abf.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nin.yanxiufei.cn

while (my $line = <$fh>) { print $line; }
来源：http://hku.snrcjt.cn

[T51] Scala：Hello World
来源：http://kmq.zhaomingkeji.xyz

println("Hello")
来源：http://vrp.zdbjq.cn

[T52] Scala：变量
来源：http://elh.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://lhr.yanxiufei.cn

[T53] Scala：字符串插值
来源：http://qjj.redwolf501.top

s"值: $b"
来源：http://yub.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://cmz.ehwqpu.com

List(1, 2, 3).map(_ * 2)
来源：http://rcr.ehwqpu.com

[T55] Scala：集合过滤
来源：http://uhq.cqqwz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rvi.hammf.cn

[T56] Scala：样例类
来源：http://mdz.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://zvq.xuanzx.com

[T57] Scala：模式匹配
来源：http://myk.zhiwuduotai.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vhy.hcnkem.com

[T58] Scala：函数定义
来源：http://ujc.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://dea.birdmap.top

[T59] Scala：循环
来源：http://zvd.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://djx.zhijiandao.cn

[T60] Scala：折叠
来源：http://nqr.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tdq.jyoumei.cn

================================================================================
来源：http://wsc.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fvy.birdmap.top

================================================================================
来源：http://ivo.andypj.xyz

[U01] Py：创建虚拟环境
来源：http://xek.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://jkr.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://vps.zdqjudy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vov.zhixingplan.top

[U03] Py：加载 .env 配置
来源：http://omi.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mtk.birdmap.top

[U04] Py：变量调试打印
来源：http://mfr.zdqjudy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://obv.xuanzx.com

[U05] Py：列表去重且保序
来源：http://yiz.yongpay.top

list(dict.fromkeys(arr))
来源：http://iay.zhixingplan.top

[U06] Py：合并两个字典
来源：http://wnc.yvedp.cn

{**a, **b}
来源：http://ciq.meibo888.top

[U07] Py：反转字典键值
来源：http://jbv.feifeiyinyue.top

{v: k for k, v in d.items()}
来源：http://gem.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://uqw.kuanghao11.cn

[y for x in nested for y in x]
来源：http://npz.fzhhl.top


<!-- 参考信息 -->