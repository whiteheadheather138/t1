代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iwx.0kj1m.cn

[R66] 定时任务
来源：http://evl.uphjek.com

crontab -e;  crontab -l
来源：http://lnf.sweek.top

[R67] 生成随机十六进制串
来源：http://tio.yangfankeji.com

openssl rand -hex 16
来源：http://aej.epnwcf.com

[R68] 计算文件校验值
来源：http://qdf.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ogn.meibo888.top

[R69] 生成随机密码
来源：http://bwx.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://vnj.dianchejie.cn

[R70] 时间戳与互转
来源：http://fno.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://fec.xziqi.cn

[R71] 日期格式化
来源：http://fsw.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rvi.yuxming.cn

[R72] 等待端口就绪
来源：http://dvc.0kj1m.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://let.shanyushiyangtech.top

[R73] 分割大日志
来源：http://peh.hammf.cn

split -l 1000 big.log part_
来源：http://nyq.yj20258.top

[R74] 批量重命名
来源：http://tsw.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ddp.cucudq.cn

[R75] 导出环境变量
来源：http://joj.xingfuxueyuan.xyz

export PATH="$HOME/bin:$PATH"
来源：http://rgd.fanxiaobao.xyz

[R76] 使用临时文件
来源：http://blg.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jcf.vehdjk.com

[R77] 读取用户输入
来源：http://hmy.mhx1999.top

read -rp "请输入: " ans
来源：http://imw.hammf.cn

[R78] 交互式菜单
来源：http://let.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bwu.yuxming.cn

[R79] 解析命令行选项
来源：http://vmu.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rlm.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://evh.yonumen.top

time ./run.sh
来源：http://fls.dianchejie.cn

================================================================================
来源：http://jyq.zhoulong.xyz

S. C / C++ 专题
来源：http://euz.daxiang520.top

================================================================================
来源：http://wnq.zdqjudy.top

[S01] C：Hello World
来源：http://dfn.gzhubu.top

#include <stdio.h>
来源：http://ooj.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tih.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://dbm.ppjwa.cn

int a = 10; printf("%d\n", a);
来源：http://aya.guowangkeji.top

[S03] C：读入整数
来源：http://gvi.andypj.xyz

int x; scanf("%d", &x);
来源：http://emi.zhoulong.xyz

[S04] C：字符串复制
来源：http://tnz.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://vvj.wangshuangyany.cn

[S05] C：字符串长度
来源：http://uhd.chenjidiqi.icu

strlen(s)
来源：http://vck.jinqigufen.top

[S06] C：字符串比较
来源：http://cra.guannengcc.top

strcmp(a, b) == 0
来源：http://zoz.guannengcc.top

[S07] C：数组遍历求和
来源：http://vlj.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wju.shuidangran.top

[S08] C：动态内存分配与释放
来源：http://bdq.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bbk.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://nci.0kj1m.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://icc.havefunace.top

[S10] C：指针与解引用
来源：http://ega.fengsongda.top

int *p = &a;  *p = 5;
来源：http://kte.chenlongwang.top

[S11] C：逐行读文件
来源：http://ere.bjfxy.top

FILE *f = fopen("a.txt", "r");
来源：http://eig.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wir.hysaishi.cn

fclose(f);
来源：http://nrw.xuanzx.com

[S12] C：写文件
来源：http://msg.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ubh.quarkkingdee.top

[S13] C：宏定义
来源：http://nvg.ehwqpu.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://csn.iojbl.cn

[S14] C：枚举
来源：http://wtr.daria6918.cn

enum Color { RED, GREEN, BLUE };
来源：http://vny.zycfv.cn

[S15] C：类型转换
来源：http://gae.andypj.xyz

(double) a / b
来源：http://wfs.zycfv.cn

[S16] C：位操作置位
来源：http://qlu.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://swf.yj20258.top

[S17] C：安全拼接字符串
来源：http://yvh.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dor.tarul.cn

[S18] C：命令行参数
来源：http://gnp.wangdashe.top

int main(int argc, char **argv)
来源：http://idn.daxiang520.top

[S19] C：快速排序
来源：http://mpb.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://kou.kuanghao11.cn

[S20] C：二分查找
来源：http://qmn.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mpu.tarul.cn

[S21] C：字符类别判断
来源：http://ppp.havefunace.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jmx.cdnleiting.top

[S22] C：字符串转数字
来源：http://aey.yj20258888.top

atoi("42");  strtod("3.14", NULL);
来源：http://vvg.svipenyu.cn

[S23] C：随机数
来源：http://xeq.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ksy.gogol.net.cn

[S24] C：获取本地时间
来源：http://boz.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mhu.zhongyouzk.top

[S25] C：内存拷贝
来源：http://vkj.zycfv.cn

memcpy(dst, src, n);
来源：http://ero.xuetiantiany.cn

[S26] C：内存清零
来源：http://opf.jianghu66.top

memset(a, 0, sizeof a);
来源：http://cdk.zhoulong.xyz

[S27] C：定义常量
来源：http://jto.uphjek.com

const double PI = 3.14159;
来源：http://mmf.zdqjudy.top

[S28] C：静态变量
来源：http://ygz.hfpthk.cn

static int counter = 0;
来源：http://jee.bbcook.cn

[S29] C：变参函数
来源：http://lzq.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zln.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://omq.zhiwuduotai.top

#ifndef X_H
来源：http://ujq.meibo888.top

#define X_H
来源：http://nbk.tanke756.top

#endif
来源：http://ulu.ydzc1.top

[S31] C++：Hello World
来源：http://olu.ydjk.org.cn

#include <iostream>
来源：http://ply.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://btg.gogol.net.cn

[S32] C++：字符串
来源：http://bdw.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://yqa.dianchejie.cn

[S33] C++：vector 增删
来源：http://wui.zhaomingkeji.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ppa.xziqi.cn

[S34] C++：遍历 vector
来源：http://uej.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://gbk.vqdsnc.cn

[S35] C++：map
来源：http://jnq.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sce.yj20258.top

[S36] C++：unordered_map
来源：http://ekf.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qhj.jinyuanbaomall.cn

[S37] C++：set
来源：http://nqb.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gsj.yfazqb.com

[S38] C++：排序
来源：http://pfy.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://dbn.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://uqp.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ybk.bbcook.cn

[S40] C++：查找元素
来源：http://zlu.epnwcf.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uuc.sysykeji.top

[S41] C++：类与构造函数
来源：http://mks.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hmu.sufxvd.cn

[S42] C++：继承与虚函数
来源：http://ijv.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://dqn.jinqigfzy.top

[S43] C++：智能指针
来源：http://abv.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://avj.hesvh.cn

[S44] C++：引用传参
来源：http://fph.gzhubu.top

void inc(int &x) { ++x; }
来源：http://hte.yj20258888.top

[S45] C++：lambda
来源：http://rkb.svipenyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ayi.cdnleiting.top

[S46] C++：函数模板
来源：http://ttv.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gic.yangfankeji.com

[S47] C++：结构化绑定遍历
来源：http://qza.fktsv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mei.smart0.xyz

[S48] C++：逐行读文件
来源：http://fvz.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://uaz.xylfe.cn

while (std::getline(in, line)) { }
来源：http://rbu.epnwcf.com

[S49] C++：写文件
来源：http://lcu.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://act.daria6918.cn

[S50] C++：格式化数字
来源：http://mxv.fzhhl.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wav.yueranfly.top

[S51] C++：显式类型转换
来源：http://wpj.jiagoushi.top

static_cast<double>(a) / b
来源：http://dpg.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://tio.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://nor.hysaishi.cn

[S53] C++：移动语义
来源：http://jyk.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://aid.ybcxt.top

[S54] C++：异常处理
来源：http://ksf.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tlt.bjfxy.top

[S55] C++：结构化绑定
来源：http://ivc.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://phd.9152youxi.cn

[S56] C++：optional
来源：http://frf.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tyi.fehbvm.com

[S57] C++：编译期常量
来源：http://uxv.chenjidiqi.icu

constexpr int N = 10;
来源：http://hsd.daxiang520.top

[S58] C++：命名空间
来源：http://ywx.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://cvo.hnqzz.top

[S59] C++：静态断言
来源：http://ggn.fanxiaobao.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qlw.meibo888.top

[S60] C++：遍历并删除元素
来源：http://iew.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oek.yj20258888.top

================================================================================
来源：http://yhm.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hyg.daria6918.cn

================================================================================
来源：http://ezz.nanxuanxn.top

[T01] Kotlin：Hello World
来源：http://tur.zhijiandao.cn

println("Hello")
来源：http://nsq.jqgufenzy.top

[T02] Kotlin：变量
来源：http://zoa.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qte.wangdashe.top

[T03] Kotlin：字符串模板
来源：http://ewi.xuetiantiany.cn

"值: $b"
来源：http://ckf.c1oappe.top

[T04] Kotlin：空安全
来源：http://asa.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://iei.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://wcc.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://akf.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://jdz.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pyp.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://avx.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rfm.nanxuanxn.top

[T08] Kotlin：数据类
来源：http://ljb.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://wff.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://fvo.yonumen.top

fun String.exclaim() = this + "!"
来源：http://erx.xziqi.cn

[T10] Kotlin：默认参数
来源：http://xbw.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uex.quarkkingdee.top

[T11] Kotlin：协程
来源：http://ppt.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eya.vehdjk.com

[T12] Kotlin：解构声明
来源：http://pcz.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://jsb.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://cmt.ybcxt.top

val m = mapOf("a" to 1)
来源：http://kze.daxiang520.top

[T14] Kotlin：循环
来源：http://puq.aibaodan.cn

for (i in 1..10) println(i)
来源：http://nen.yangfankeji.com

[T15] Kotlin：接口
来源：http://hmn.ydzc1.top

interface Shape { fun area(): Double }
来源：http://afs.ydjk.org.cn

[T16] Swift：Hello World
来源：http://srx.xinyue.icu

print("Hello")
来源：http://gjp.9152youxi.cn

[T17] Swift：变量与常量
来源：http://bmq.gogol.net.cn

var a = 1;  let b = 2
来源：http://tay.fengsongda.top

[T18] Swift：字符串插值
来源：http://joh.zhengqikj.top

"值: \(b)"
来源：http://lhc.tian-w.cn

[T19] Swift：可选绑定
来源：http://gbw.tanke756.top

if let n = opt { print(n) }
来源：http://hjj.epnwcf.com

[T20] Swift：数组操作
来源：http://lst.chenjidiqi.icu

var a = [1, 2, 3];  a.append(4)
来源：http://zwy.0kj1m.cn

[T21] Swift：遍历
来源：http://rew.fktsv.cn

for x in a { print(x) }
来源：http://xyi.zdbjq.cn

[T22] Swift：字典
来源：http://ewa.fengsongda.top

var d = ["a": 1];  d["b"] = 2
来源：http://wrt.redwolf501.top

[T23] Swift：函数
来源：http://stb.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wzy.fanxiaobao.xyz

[T24] Swift：闭包
来源：http://gir.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://kuq.tian-w.cn

[T25] Swift：结构体
来源：http://myq.yfazqb.com

struct P { var x: Int }
来源：http://vba.yonumen.top

[T26] Swift：类与重写
来源：http://qzm.dianchejie.cn

class A: Base { override func f() {} }
来源：http://eio.birdmap.top

[T27] Swift：错误处理
来源：http://jfc.cheryme.top

do { try f() } catch { print(error) }
来源：http://fax.yj20258888.top

[T28] Swift：枚举
来源：http://qpo.yongpay.top

enum Color { case red, green }
来源：http://nka.chenzaomai.com

[T29] Swift：guard 提前返回
来源：http://ocj.xingfuxueyuan.xyz

guard let x = opt else { return }
来源：http://jst.meibo888.top

[T30] Swift：协议
来源：http://tzs.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://isz.fehbvm.com

[T31] Lua：Hello World
来源：http://gzb.xylfe.cn

print("Hello")
来源：http://hdh.havefunace.top

[T32] Lua：局部变量
来源：http://ims.shanyushiyangkeji.top

local a = 1
来源：http://qbg.hnqzz.top

[T33] Lua：表（数组）
来源：http://vfr.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lwv.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://lja.chenlongwang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rpx.hfpthk.cn

[T35] Lua：字典表
来源：http://qpu.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://dya.pycfn.com

[T36] Lua：函数
来源：http://bqx.gaohongyu789.top

function add(a, b) return a + b end
来源：http://mwz.fehbvm.com

[T37] Lua：字符串拼接
来源：http://qtk.ctjpmb.com

"a" .. "b"
来源：http://yys.shzxlz.cn

[T38] Lua：条件
来源：http://vtw.havefunace.top

if x > 0 then print("正") end
来源：http://uzp.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://fia.quarkkingdee.top

string.find(s, "%d+")
来源：http://vlu.xinyue.icu

[T40] Lua：元表
来源：http://vjs.pycfn.com

setmetatable({}, { __index = base })
来源：http://zql.ywan-chungtsiang.top

[T41] Perl：Hello World
来源：http://orz.zycfv.cn

print "Hello\n";
来源：http://oeb.xylfe.cn

[T42] Perl：变量类型
来源：http://klf.haohaochexian.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qbs.fktsv.cn

[T43] Perl：字符串插值
来源：http://jxj.chenjidiqi.icu

"值: $a"
来源：http://map.hammf.cn

[T44] Perl：条件
来源：http://gni.nanxuanxn.top

if ($a > 0) { print "正"; }
来源：http://iot.redwolf501.top

[T45] Perl：数组遍历
来源：http://mnw.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://mdf.hongshengwenyu.top

[T46] Perl：哈希操作
来源：http://lvh.aibaodan.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lpw.iojbl.cn

[T47] Perl：正则捕获
来源：http://uhd.smart0.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://nxr.andypj.xyz

[T48] Perl：正则替换
来源：http://uvy.wangshuangyany.cn

$s =~ s/old/new/g;
来源：http://fro.hnxiangtu.top

[T49] Perl：函数
来源：http://qip.havefunace.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yzf.zhongyouzk.top

[T50] Perl：逐行读文件
来源：http://sgp.hywenlv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ysg.ydzc1.top

while (my $line = <$fh>) { print $line; }
来源：http://dqs.svipenyu.cn

[T51] Scala：Hello World
来源：http://tnb.shuidangran.top

println("Hello")
来源：http://nhn.yuxming.cn

[T52] Scala：变量
来源：http://dmx.snrcjt.cn

val a = 1;  var b = 2
来源：http://vzv.jianghu66.top

[T53] Scala：字符串插值
来源：http://nht.zhengqikj.top

s"值: $b"
来源：http://urr.nanxuanxn.top

[T54] Scala：集合映射
来源：http://lsm.yuanzhike.top

List(1, 2, 3).map(_ * 2)
来源：http://org.jianghu66.top

[T55] Scala：集合过滤
来源：http://qdb.zhengqikj.top

List(1, 2, 3).filter(_ > 1)
来源：http://pxd.fktsv.cn

[T56] Scala：样例类
来源：http://yqp.hnqzz.top

case class User(name: String, age: Int)
来源：http://rdv.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://wmj.ehwqpu.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://dyn.birdmap.top

[T58] Scala：函数定义
来源：http://dby.tian-w.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hhx.bjfxy.top

[T59] Scala：循环
来源：http://pus.yueranfly.top

for (i <- 1 to 10) println(i)
来源：http://qyz.quarkkingdee.top

[T60] Scala：折叠
来源：http://lov.ydzc1.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vti.c1oappe.top

================================================================================
来源：http://dfn.dashuyun.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bvt.ydzc1.top

================================================================================
来源：http://fux.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://psq.cheryme.top

python -m venv .venv && source .venv/bin/activate
来源：http://qgy.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://zdh.gogol.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://npv.chenjidiqi.icu

[U03] Py：加载 .env 配置
来源：http://qvp.zhaomingkeji.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://wmg.cheryme.top

[U04] Py：变量调试打印
来源：http://byo.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gtz.yj20258888.top

[U05] Py：列表去重且保序
来源：http://xju.chenzaomai.com

list(dict.fromkeys(arr))
来源：http://bbj.shzxlz.cn

[U06] Py：合并两个字典
来源：http://xkn.xziqi.cn

{**a, **b}
来源：http://ylf.9152youxi.cn


<!-- 参考信息 -->