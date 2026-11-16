代发 wailian999

free -h;  ps aux | grep nginx
来源：http://jkp.zdqjudy.top

[R64] 结束进程
来源：http://ofk.yongpay.top

kill -9 $(pgrep -f app.py)
来源：http://owd.nwbrower.top

[R65] 查看端口占用
来源：http://jxr.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pil.yueranfly.top

[R66] 定时任务
来源：http://dkc.yongpay.top

crontab -e;  crontab -l
来源：http://irm.smart0.xyz

[R67] 生成随机十六进制串
来源：http://yfu.yueranfly.top

openssl rand -hex 16
来源：http://uto.52xcode.cn

[R68] 计算文件校验值
来源：http://yoq.guowangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://ujw.hnqzz.top

[R69] 生成随机密码
来源：http://smz.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://byh.daria6918.cn

[R70] 时间戳与互转
来源：http://vsc.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://sck.yvedp.cn

[R71] 日期格式化
来源：http://nfq.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dqt.yonumen.top

[R72] 等待端口就绪
来源：http://gvn.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cqp.jqgfzy.top

[R73] 分割大日志
来源：http://pkq.dianchejie.cn

split -l 1000 big.log part_
来源：http://wiy.jiagoushi.top

[R74] 批量重命名
来源：http://rxd.cashguo.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pve.jiagoushi.top

[R75] 导出环境变量
来源：http://xtm.ctjpmb.com

export PATH="$HOME/bin:$PATH"
来源：http://wsy.jinqigfzy.top

[R76] 使用临时文件
来源：http://ano.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wwq.sxryk.cn

[R77] 读取用户输入
来源：http://szw.zhixingplan.top

read -rp "请输入: " ans
来源：http://ihs.dianchejie.cn

[R78] 交互式菜单
来源：http://mzd.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pov.zdqjudy.top

[R79] 解析命令行选项
来源：http://ezg.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dsf.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://nws.fktsv.cn

time ./run.sh
来源：http://ehz.jinqigufen.top

================================================================================
来源：http://yid.haohaochexian.top

S. C / C++ 专题
来源：http://edo.sweek.top

================================================================================
来源：http://yjf.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://tjo.wangdashe.top

#include <stdio.h>
来源：http://iec.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nca.yueranfly.top

[S02] C：变量与格式化输出
来源：http://ibm.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://tzj.316326.xyz

[S03] C：读入整数
来源：http://mjv.nanxinkj.top

int x; scanf("%d", &x);
来源：http://etc.quarkkingdee.top

[S04] C：字符串复制
来源：http://adl.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pwx.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://eur.yuanzhike.top

strlen(s)
来源：http://vgg.tanke756.top

[S06] C：字符串比较
来源：http://krw.andypj.xyz

strcmp(a, b) == 0
来源：http://mtc.hcnkem.com

[S07] C：数组遍历求和
来源：http://sag.tanke756.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://huk.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://elm.quarkkingdee.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pgq.dashuyun.cn

[S09] C：结构体定义与初始化
来源：http://kec.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hty.hysaishi.cn

[S10] C：指针与解引用
来源：http://pgc.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://mxl.haohaochexian.top

[S11] C：逐行读文件
来源：http://ijz.jinghuilouyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://rhe.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://toh.gogol.net.cn

fclose(f);
来源：http://qwk.cqqwz.cn

[S12] C：写文件
来源：http://tqt.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mtu.mhx1999.top

[S13] C：宏定义
来源：http://utg.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fgr.guannengcc.top

[S14] C：枚举
来源：http://riv.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://wcw.ydzc1.top

[S15] C：类型转换
来源：http://xzs.hysaishi.cn

(double) a / b
来源：http://hsq.xuetiantiany.cn

[S16] C：位操作置位
来源：http://qln.zhijiandao.cn

x |= (1 << 3);
来源：http://mfn.52xcode.cn

[S17] C：安全拼接字符串
来源：http://vcl.jiagoushi.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eur.xuetiantiany.cn

[S18] C：命令行参数
来源：http://ent.wangdashe.top

int main(int argc, char **argv)
来源：http://fst.xuanzx.com

[S19] C：快速排序
来源：http://etw.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fiq.jiagoushi.top

[S20] C：二分查找
来源：http://mok.sweek.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pen.ivvv.top

[S21] C：字符类别判断
来源：http://svj.andypj.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lus.yuxming.cn

[S22] C：字符串转数字
来源：http://hkr.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ctd.cqqwz.cn

[S23] C：随机数
来源：http://iwb.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dwy.0kj1m.cn

[S24] C：获取本地时间
来源：http://scs.fktsv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hbo.shanyushiyangkeji.top

[S25] C：内存拷贝
来源：http://elp.hfpthk.cn

memcpy(dst, src, n);
来源：http://iix.guannengcc.top

[S26] C：内存清零
来源：http://ubm.xuanzx.com

memset(a, 0, sizeof a);
来源：http://gwz.quarkkingdee.top

[S27] C：定义常量
来源：http://pnd.epnwcf.com

const double PI = 3.14159;
来源：http://bii.gaohongyu789.top

[S28] C：静态变量
来源：http://tve.c1oappe.top

static int counter = 0;
来源：http://pdu.yfazqb.com

[S29] C：变参函数
来源：http://lhm.jinghuilouyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zjh.vehdjk.com

[S30] C：头文件保护
来源：http://rxj.zhoulong.xyz

#ifndef X_H
来源：http://veu.nanxinkj.top

#define X_H
来源：http://lxv.zhengqikj.top

#endif
来源：http://qgj.dianchejie.cn

[S31] C++：Hello World
来源：http://awr.hysaishi.cn

#include <iostream>
来源：http://cah.yfazqb.com

int main() { std::cout << "Hello\n"; }
来源：http://muw.shzxlz.cn

[S32] C++：字符串
来源：http://fue.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://fjo.jinqigfzy.top

[S33] C++：vector 增删
来源：http://pad.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uxj.gaohongyu789.top

[S34] C++：遍历 vector
来源：http://aeh.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://obb.vqdsnc.cn

[S35] C++：map
来源：http://tfu.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xrl.xuanzx.com

[S36] C++：unordered_map
来源：http://cgs.uphjek.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://znq.yonumen.top

[S37] C++：set
来源：http://biu.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tnr.dianchejie.cn

[S38] C++：排序
来源：http://jln.zhengqikj.top

std::sort(v.begin(), v.end());
来源：http://ghp.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://cig.jianghu66.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://clj.vehdjk.com

[S40] C++：查找元素
来源：http://fmz.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://csp.dianchejie.cn

[S41] C++：类与构造函数
来源：http://wyn.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xfn.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://jxp.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://fmc.zhongyouzk.top

[S43] C++：智能指针
来源：http://xru.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://wox.daria6918.cn

[S44] C++：引用传参
来源：http://vod.redwolf501.top

void inc(int &x) { ++x; }
来源：http://ijb.tanke756.top

[S45] C++：lambda
来源：http://ucq.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://zdm.guowangkeji.top

[S46] C++：函数模板
来源：http://xeg.jqgufenzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ffs.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://rrr.yj202588.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://doo.hysaishi.cn

[S48] C++：逐行读文件
来源：http://awb.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xah.yfazqb.com

while (std::getline(in, line)) { }
来源：http://hvh.chenjidiqi.icu

[S49] C++：写文件
来源：http://vvk.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gkp.hammf.cn

[S50] C++：格式化数字
来源：http://lwh.yueranfly.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vvl.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://yfz.chenzaomai.com

static_cast<double>(a) / b
来源：http://maa.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://rpy.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://lhq.tian-w.cn

[S53] C++：移动语义
来源：http://mqo.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://vyz.yongpay.top

[S54] C++：异常处理
来源：http://pzn.zhongyouzk.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nxq.cucudq.cn

[S55] C++：结构化绑定
来源：http://wgw.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://txw.yfazqb.com

[S56] C++：optional
来源：http://kiq.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://foh.gaohongyu789.top

[S57] C++：编译期常量
来源：http://res.fzhhl.top

constexpr int N = 10;
来源：http://rgm.hcnkem.com

[S58] C++：命名空间
来源：http://rxw.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://ioi.ydzc1.top

[S59] C++：静态断言
来源：http://ymz.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tzv.zhixingplan.top

[S60] C++：遍历并删除元素
来源：http://cii.jinqigufen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pik.ywan-chungtsiang.top

================================================================================
来源：http://mwd.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lnd.shzxlz.cn

================================================================================
来源：http://fcd.chenlongwang.top

[T01] Kotlin：Hello World
来源：http://cmz.meibo888.top

println("Hello")
来源：http://fal.hesvh.cn

[T02] Kotlin：变量
来源：http://cnn.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wbf.xziqi.cn

[T03] Kotlin：字符串模板
来源：http://kjr.xinyue.icu

"值: $b"
来源：http://qaz.sysykeji.top

[T04] Kotlin：空安全
来源：http://rrz.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://evq.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://tys.tian-w.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hrn.cheryme.top

[T06] Kotlin：集合映射
来源：http://ddg.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cux.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://hlm.quarkkingdee.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iph.cashguo.top

[T08] Kotlin：数据类
来源：http://gbk.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://chp.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://ijv.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://kwd.zycfv.cn

[T10] Kotlin：默认参数
来源：http://nxi.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jgh.haohaochexian.top

[T11] Kotlin：协程
来源：http://lgp.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vwi.yonumen.top

[T12] Kotlin：解构声明
来源：http://kcl.xuetiantiany.cn

val (a, b) = Pair(1, 2)
来源：http://yse.ivvv.top

[T13] Kotlin：只读 Map
来源：http://dfw.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://tlx.jiagoushi.top

[T14] Kotlin：循环
来源：http://opj.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://ufw.hnqzz.top

[T15] Kotlin：接口
来源：http://urr.zhiwuduotai.top

interface Shape { fun area(): Double }
来源：http://qfw.vehdjk.com

[T16] Swift：Hello World
来源：http://css.shzxlz.cn

print("Hello")
来源：http://jgo.hysaishi.cn

[T17] Swift：变量与常量
来源：http://hcd.0kj1m.cn

var a = 1;  let b = 2
来源：http://dwh.daxiang520.top

[T18] Swift：字符串插值
来源：http://zsq.mhx1999.top

"值: \(b)"
来源：http://mqs.hesvh.cn

[T19] Swift：可选绑定
来源：http://mfs.gogol.net.cn

if let n = opt { print(n) }
来源：http://rnl.iojbl.cn

[T20] Swift：数组操作
来源：http://egz.bbcook.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vgp.gotoacloud.top

[T21] Swift：遍历
来源：http://nni.fengsongda.top

for x in a { print(x) }
来源：http://yzw.wangshuangyany.cn

[T22] Swift：字典
来源：http://oqd.hfpthk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cgx.sysykeji.top

[T23] Swift：函数
来源：http://nqx.pycfn.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://afp.yongpay.top

[T24] Swift：闭包
来源：http://drs.tanke756.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ajq.zycfv.cn

[T25] Swift：结构体
来源：http://hpn.pycfn.com

struct P { var x: Int }
来源：http://hxp.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://zrk.zhixingplan.top

class A: Base { override func f() {} }
来源：http://xxz.jyoumei.cn

[T27] Swift：错误处理
来源：http://jek.ydzc1.top

do { try f() } catch { print(error) }
来源：http://lcs.chenzaomai.com

[T28] Swift：枚举
来源：http://aua.chenzaomai.com

enum Color { case red, green }
来源：http://dlx.hnqzz.top

[T29] Swift：guard 提前返回
来源：http://ngg.yj20258888.top

guard let x = opt else { return }
来源：http://gyz.zhijiandao.cn

[T30] Swift：协议
来源：http://zux.xuanzx.com

protocol Shape { func area() -> Double }
来源：http://lxd.kuanghao11.cn

[T31] Lua：Hello World
来源：http://pab.hnqzz.top

print("Hello")
来源：http://zkf.havefunace.top

[T32] Lua：局部变量
来源：http://pjv.epnwcf.com

local a = 1
来源：http://qhd.meibo888.top

[T33] Lua：表（数组）
来源：http://ukx.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zlt.dashuyun.cn

[T34] Lua：遍历表
来源：http://hhj.zhaomingkeji.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://nal.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://ffr.jianghu66.top

local d = { a = 1 };  d.b = 2
来源：http://erc.fzhhl.top

[T36] Lua：函数
来源：http://gru.kuanghao11.cn

function add(a, b) return a + b end
来源：http://zjs.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://lco.uphjek.com

"a" .. "b"
来源：http://fha.yfazqb.com

[T38] Lua：条件
来源：http://vao.hnqzz.top

if x > 0 then print("正") end
来源：http://dus.xuetiantiany.cn

[T39] Lua：模式匹配
来源：http://apw.fzhhl.top

string.find(s, "%d+")
来源：http://oai.gotoacloud.top

[T40] Lua：元表
来源：http://yye.cdnleiting.top

setmetatable({}, { __index = base })
来源：http://yxl.cashguo.top

[T41] Perl：Hello World
来源：http://tkg.xingfuxueyuan.xyz

print "Hello\n";
来源：http://ikt.nanxuanxn.top

[T42] Perl：变量类型
来源：http://kzp.yfazqb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jmw.ivvv.top

[T43] Perl：字符串插值
来源：http://koa.ivvv.top

"值: $a"
来源：http://jpv.hnxiangtu.top

[T44] Perl：条件
来源：http://ndn.tianlin.xyz

if ($a > 0) { print "正"; }
来源：http://rgy.yj20258888.top

[T45] Perl：数组遍历
来源：http://arg.hongshengwenyu.top

for my $x (@arr) { print $x; }
来源：http://ybp.zdbjq.cn

[T46] Perl：哈希操作
来源：http://bre.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zna.fzhhl.top

[T47] Perl：正则捕获
来源：http://ckt.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vva.zdqjudy.top

[T48] Perl：正则替换
来源：http://zzb.xuanzx.com

$s =~ s/old/new/g;
来源：http://yjc.daria6918.cn

[T49] Perl：函数
来源：http://xbw.aibaodan.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hjs.yvedp.cn

[T50] Perl：逐行读文件
来源：http://abn.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://mok.meibo888.top

while (my $line = <$fh>) { print $line; }
来源：http://vty.ydjk.org.cn

[T51] Scala：Hello World
来源：http://fky.ydzc1.top

println("Hello")
来源：http://dke.jinqigufen.top

[T52] Scala：变量
来源：http://fzu.zhiwuduotai.top

val a = 1;  var b = 2
来源：http://jiw.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://ufx.tian-w.cn

s"值: $b"
来源：http://opm.nanxuanxn.top

[T54] Scala：集合映射
来源：http://wnw.zycfv.cn

List(1, 2, 3).map(_ * 2)
来源：http://aej.hesvh.cn

[T55] Scala：集合过滤
来源：http://wez.yj20258888.top

List(1, 2, 3).filter(_ > 1)
来源：http://nwe.zhijiandao.cn

[T56] Scala：样例类
来源：http://noi.guannengcc.top

case class User(name: String, age: Int)
来源：http://gec.chenlongwang.top

[T57] Scala：模式匹配
来源：http://jyf.yonumen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nrk.haohaochexian.top

[T58] Scala：函数定义
来源：http://qvv.jiagoushi.top

def add(a: Int, b: Int): Int = a + b
来源：http://cfr.wangdashe.top

[T59] Scala：循环
来源：http://jdr.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://ajx.dashuyun.cn

[T60] Scala：折叠
来源：http://fvp.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bhe.zdqjudy.top

================================================================================
来源：http://rkb.zycfv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jhk.jianghu66.top

================================================================================
来源：http://rmi.sweek.top

[U01] Py：创建虚拟环境
来源：http://tbn.xuetiantiany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jfd.hnqzz.top

[U02] Py：导出 / 安装依赖
来源：http://zns.feifeiyinyue.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tau.jinghuilouyu.cn

[U03] Py：加载 .env 配置
来源：http://nom.jinqigfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bhd.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://xch.hcnkem.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ynq.xylfe.cn


<!-- 参考信息 -->