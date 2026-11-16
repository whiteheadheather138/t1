代发 wailian999

free -h;  ps aux | grep nginx
来源：http://hbl.daxiang520.top

[R64] 结束进程
来源：http://wtq.ppjwa.cn

kill -9 $(pgrep -f app.py)
来源：http://fxf.bbcook.cn

[R65] 查看端口占用
来源：http://lwq.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zfp.chenjidiqi.icu

[R66] 定时任务
来源：http://iyq.feifeiyinyue.top

crontab -e;  crontab -l
来源：http://okn.cashguo.top

[R67] 生成随机十六进制串
来源：http://vby.feifeiyinyue.top

openssl rand -hex 16
来源：http://ste.cqqwz.cn

[R68] 计算文件校验值
来源：http://onn.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://rxa.quarkkingdee.top

[R69] 生成随机密码
来源：http://kpj.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://yks.andypj.xyz

[R70] 时间戳与互转
来源：http://bmp.yfazqb.com

date +%s;  date -d @1700000000
来源：http://owg.cqqwz.cn

[R71] 日期格式化
来源：http://eqg.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://jfj.dashuyun.cn

[R72] 等待端口就绪
来源：http://vzl.ppjwa.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bvk.zdqjudy.top

[R73] 分割大日志
来源：http://kat.xinyue.icu

split -l 1000 big.log part_
来源：http://reg.ivvv.top

[R74] 批量重命名
来源：http://nao.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yfa.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://kez.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://dgl.epnwcf.com

[R76] 使用临时文件
来源：http://jyj.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lff.tanke756.top

[R77] 读取用户输入
来源：http://eih.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://btc.quarkkingdee.top

[R78] 交互式菜单
来源：http://pek.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://oxo.nwbrower.top

[R79] 解析命令行选项
来源：http://coh.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pgg.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://ncv.yvedp.cn

time ./run.sh
来源：http://wuq.vehdjk.com

================================================================================
来源：http://xpb.zhongyouzk.top

S. C / C++ 专题
来源：http://yls.zdbjq.cn

================================================================================
来源：http://qqg.aizwys.cn

[S01] C：Hello World
来源：http://fir.tanke756.top

#include <stdio.h>
来源：http://ovz.9152youxi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://loe.ydzc1.top

[S02] C：变量与格式化输出
来源：http://mvt.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://msj.cheryme.top

[S03] C：读入整数
来源：http://xkl.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://gub.havefunace.top

[S04] C：字符串复制
来源：http://sdr.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zrw.chenlongwang.top

[S05] C：字符串长度
来源：http://ila.gotoacloud.top

strlen(s)
来源：http://hnp.zhijiandao.cn

[S06] C：字符串比较
来源：http://cfv.chenlongwang.top

strcmp(a, b) == 0
来源：http://rdw.xinyue.icu

[S07] C：数组遍历求和
来源：http://tha.tanke756.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sck.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://kkp.xingfuxueyuan.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iyo.haohaochexian.top

[S09] C：结构体定义与初始化
来源：http://lrt.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yow.sysykeji.top

[S10] C：指针与解引用
来源：http://ayo.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://ini.andypj.xyz

[S11] C：逐行读文件
来源：http://ddg.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://hoa.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fwv.chenjidiqi.icu

fclose(f);
来源：http://gbg.tianlin.xyz

[S12] C：写文件
来源：http://xis.cheryme.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://smj.yangfankeji.com

[S13] C：宏定义
来源：http://ujr.jianghu66.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://isx.tian-w.cn

[S14] C：枚举
来源：http://rti.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://ojt.zdbjq.cn

[S15] C：类型转换
来源：http://rev.ybcxt.top

(double) a / b
来源：http://pfo.cashguo.top

[S16] C：位操作置位
来源：http://lmm.bjfxy.top

x |= (1 << 3);
来源：http://vao.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://wps.wangshuangyany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://njc.yueranfly.top

[S18] C：命令行参数
来源：http://ved.tanke756.top

int main(int argc, char **argv)
来源：http://pyd.andypj.xyz

[S19] C：快速排序
来源：http://lgw.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://lox.jiagoushi.top

[S20] C：二分查找
来源：http://xcf.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wdp.xuanzx.com

[S21] C：字符类别判断
来源：http://kab.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ign.zhoulong.xyz

[S22] C：字符串转数字
来源：http://wgu.hnxiangtu.top

atoi("42");  strtod("3.14", NULL);
来源：http://sdt.chenzaomai.com

[S23] C：随机数
来源：http://rrs.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fvg.gzhubu.top

[S24] C：获取本地时间
来源：http://mbu.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oqx.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://etx.zhoulong.xyz

memcpy(dst, src, n);
来源：http://jdb.zhongyouzk.top

[S26] C：内存清零
来源：http://jfh.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://iuu.guannengcc.top

[S27] C：定义常量
来源：http://soq.vehdjk.com

const double PI = 3.14159;
来源：http://dmg.gaohongyu789.top

[S28] C：静态变量
来源：http://mwg.yuxming.cn

static int counter = 0;
来源：http://ipe.ehwqpu.com

[S29] C：变参函数
来源：http://tek.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qfh.cdnleiting.top

[S30] C：头文件保护
来源：http://ine.fzhhl.top

#ifndef X_H
来源：http://fer.52xcode.cn

#define X_H
来源：http://flu.pycfn.com

#endif
来源：http://qtl.fanxiaobao.xyz

[S31] C++：Hello World
来源：http://rpe.bbcook.cn

#include <iostream>
来源：http://xfu.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://fnk.haohaochexian.top

[S32] C++：字符串
来源：http://zag.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://kse.sufxvd.cn

[S33] C++：vector 增删
来源：http://ecn.guowangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fdp.jinqigufen.top

[S34] C++：遍历 vector
来源：http://sfr.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://prd.hfpthk.cn

[S35] C++：map
来源：http://dib.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tbx.jinqigufen.top

[S36] C++：unordered_map
来源：http://twp.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://odo.ywan-chungtsiang.top

[S37] C++：set
来源：http://stv.hcnkem.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rkl.xuetiantiany.cn

[S38] C++：排序
来源：http://swk.shanyushiyangtech.top

std::sort(v.begin(), v.end());
来源：http://tew.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://ecz.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zbv.zhijiandao.cn

[S40] C++：查找元素
来源：http://exu.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bfa.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://jqr.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gtf.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://hip.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://yws.cucudq.cn

[S43] C++：智能指针
来源：http://iyb.mhx1999.top

auto p = std::make_unique<int>(5);
来源：http://gbm.fzhhl.top

[S44] C++：引用传参
来源：http://tpe.gogol.net.cn

void inc(int &x) { ++x; }
来源：http://yfl.smart0.xyz

[S45] C++：lambda
来源：http://kqh.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://vzc.xuanzx.com

[S46] C++：函数模板
来源：http://pnl.yongpay.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://may.gotoacloud.top

[S47] C++：结构化绑定遍历
来源：http://mim.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vff.xylfe.cn

[S48] C++：逐行读文件
来源：http://bux.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://sxs.iojbl.cn

while (std::getline(in, line)) { }
来源：http://gqh.shangyingyoupin.top

[S49] C++：写文件
来源：http://rdz.guowangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://chp.shzxlz.cn

[S50] C++：格式化数字
来源：http://nvs.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://amp.yongpay.top

[S51] C++：显式类型转换
来源：http://emg.ywan-chungtsiang.top

static_cast<double>(a) / b
来源：http://sjw.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://jfr.xuetiantiany.cn

int size() const noexcept { return n_; }
来源：http://cpf.yangfankeji.com

[S53] C++：移动语义
来源：http://twf.ywan-chungtsiang.top

std::vector<int> w = std::move(v);
来源：http://djy.316326.xyz

[S54] C++：异常处理
来源：http://pdp.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://imk.svipenyu.cn

[S55] C++：结构化绑定
来源：http://ckf.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eya.mhx1999.top

[S56] C++：optional
来源：http://phf.hammf.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://inf.yj20258888.top

[S57] C++：编译期常量
来源：http://fmb.chenzaomai.com

constexpr int N = 10;
来源：http://euk.yongpay.top

[S58] C++：命名空间
来源：http://mpw.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://jqo.9152youxi.cn

[S59] C++：静态断言
来源：http://ioe.xuetiantiany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://don.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://zfa.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://msr.zhaomingkeji.xyz

================================================================================
来源：http://nib.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uij.gaohongyu789.top

================================================================================
来源：http://wmz.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://bwy.yj202588.top

println("Hello")
来源：http://rbk.yonumen.top

[T02] Kotlin：变量
来源：http://ucr.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bgx.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://mfn.shanyushiyangkeji.top

"值: $b"
来源：http://dkr.shzxlz.cn

[T04] Kotlin：空安全
来源：http://wtb.jyoumei.cn

val n: String? = null;  n?.length
来源：http://idh.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://nbm.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cgq.zhongyouzk.top

[T06] Kotlin：集合映射
来源：http://ryl.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eit.sxryk.cn

[T07] Kotlin：集合过滤
来源：http://bie.xingfuxueyuan.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://ywn.hammf.cn

[T08] Kotlin：数据类
来源：http://eut.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://mqe.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://mxj.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://ckj.yj20258.top

[T10] Kotlin：默认参数
来源：http://eir.hongshengwenyu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sss.pycfn.com

[T11] Kotlin：协程
来源：http://fkr.bjfxy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ewp.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://lco.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://kik.yongpay.top

[T13] Kotlin：只读 Map
来源：http://vwt.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://ibp.jianghu66.top

[T14] Kotlin：循环
来源：http://qzu.tarul.cn

for (i in 1..10) println(i)
来源：http://vuj.quarkkingdee.top

[T15] Kotlin：接口
来源：http://ozw.jqgfzy.top

interface Shape { fun area(): Double }
来源：http://xqg.yonumen.top

[T16] Swift：Hello World
来源：http://qzt.hnqzz.top

print("Hello")
来源：http://tua.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://hmp.yuxming.cn

var a = 1;  let b = 2
来源：http://mtw.guowangkeji.top

[T18] Swift：字符串插值
来源：http://shj.jinyuanbaomall.cn

"值: \(b)"
来源：http://rbo.kuanghao11.cn

[T19] Swift：可选绑定
来源：http://opk.yangfankeji.com

if let n = opt { print(n) }
来源：http://ixn.zhengqikj.top

[T20] Swift：数组操作
来源：http://hvb.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://jkr.birdmap.top

[T21] Swift：遍历
来源：http://dby.nwbrower.top

for x in a { print(x) }
来源：http://bqa.redwolf501.top

[T22] Swift：字典
来源：http://lmr.jqgufenzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://vuz.zhijiandao.cn

[T23] Swift：函数
来源：http://gig.guowangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nck.gaohongyu789.top

[T24] Swift：闭包
来源：http://omz.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gil.gogol.net.cn

[T25] Swift：结构体
来源：http://nbw.jiagoushi.top

struct P { var x: Int }
来源：http://eor.daxiang520.top

[T26] Swift：类与重写
来源：http://szy.tianlin.xyz

class A: Base { override func f() {} }
来源：http://bjf.aibaodan.cn

[T27] Swift：错误处理
来源：http://iut.gotoacloud.top

do { try f() } catch { print(error) }
来源：http://jrc.fktsv.cn

[T28] Swift：枚举
来源：http://rdg.yj202588.top

enum Color { case red, green }
来源：http://laa.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://yzl.bbcook.cn

guard let x = opt else { return }
来源：http://tlu.cheryme.top

[T30] Swift：协议
来源：http://kbk.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://sbu.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://eie.quarkkingdee.top

print("Hello")
来源：http://tci.jyoumei.cn

[T32] Lua：局部变量
来源：http://lav.chenjidiqi.icu

local a = 1
来源：http://ves.zhaomingkeji.xyz

[T33] Lua：表（数组）
来源：http://vfq.yj20258.top

local t = {1, 2, 3};  t[4] = 4
来源：http://grb.kuanghao11.cn

[T34] Lua：遍历表
来源：http://plr.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gve.bbcook.cn

[T35] Lua：字典表
来源：http://dkm.nanxinkj.top

local d = { a = 1 };  d.b = 2
来源：http://iey.gotoacloud.top

[T36] Lua：函数
来源：http://lij.vehdjk.com

function add(a, b) return a + b end
来源：http://ist.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://ffm.shanyushiyangtech.top

"a" .. "b"
来源：http://qrl.bjfxy.top

[T38] Lua：条件
来源：http://wcy.hywenlv.cn

if x > 0 then print("正") end
来源：http://lcy.jiagoushi.top

[T39] Lua：模式匹配
来源：http://cnn.shuidangran.top

string.find(s, "%d+")
来源：http://ftx.xinyue.icu

[T40] Lua：元表
来源：http://azl.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://cce.fanxiaobao.xyz

[T41] Perl：Hello World
来源：http://jcl.wangshuangyany.cn

print "Hello\n";
来源：http://xcq.yuanzhike.top

[T42] Perl：变量类型
来源：http://kpr.hywenlv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lja.sweek.top

[T43] Perl：字符串插值
来源：http://nbz.sufxvd.cn

"值: $a"
来源：http://ylb.yonumen.top

[T44] Perl：条件
来源：http://wbf.tanke756.top

if ($a > 0) { print "正"; }
来源：http://gym.zhixingplan.top

[T45] Perl：数组遍历
来源：http://shg.sufxvd.cn

for my $x (@arr) { print $x; }
来源：http://crt.hammf.cn

[T46] Perl：哈希操作
来源：http://osg.shanyushiyangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ykg.wangdashe.top

[T47] Perl：正则捕获
来源：http://kvu.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wkd.sufxvd.cn

[T48] Perl：正则替换
来源：http://uii.ehwqpu.com

$s =~ s/old/new/g;
来源：http://ght.aizwys.cn

[T49] Perl：函数
来源：http://rcw.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kzo.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://wke.cqqwz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jmb.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://gkg.daria6918.cn

[T51] Scala：Hello World
来源：http://ipw.bjfxy.top

println("Hello")
来源：http://wmg.ppjwa.cn

[T52] Scala：变量
来源：http://zkq.hnqzz.top

val a = 1;  var b = 2
来源：http://bnr.chenzaomai.com

[T53] Scala：字符串插值
来源：http://zoe.zhengqikj.top

s"值: $b"
来源：http://gnp.yj20258.top

[T54] Scala：集合映射
来源：http://geq.zhijiandao.cn

List(1, 2, 3).map(_ * 2)
来源：http://wqi.havefunace.top

[T55] Scala：集合过滤
来源：http://xvz.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://lqz.fanxiaobao.xyz

[T56] Scala：样例类
来源：http://pfk.zdbjq.cn

case class User(name: String, age: Int)
来源：http://mva.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://veo.cucudq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sny.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://phv.smart0.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://qei.xinyue.icu

[T59] Scala：循环
来源：http://oqw.pengpengdd.cyou

for (i <- 1 to 10) println(i)
来源：http://ikw.yuxming.cn

[T60] Scala：折叠
来源：http://tsh.aibaodan.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zvy.ywan-chungtsiang.top

================================================================================
来源：http://rfe.shuidangran.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://saw.nanxuanxn.top

================================================================================
来源：http://uyi.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://fge.xuanzx.com

python -m venv .venv && source .venv/bin/activate
来源：http://mxt.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://apm.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://usq.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://pej.xuanzx.com

from dotenv import load_dotenv; load_dotenv()
来源：http://uth.meibo888.top

[U04] Py：变量调试打印
来源：http://lyu.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hqn.ivvv.top


<!-- 参考信息 -->