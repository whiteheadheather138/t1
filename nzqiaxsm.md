代发 wailian999

df -h;  du -sh *
来源：http://ydo.52xcode.cn

[R62] 找最占空间的文件
来源：http://ntg.tanke756.top

du -ah . | sort -rh | head -10
来源：http://jek.c1oappe.top

[R63] 内存与进程
来源：http://iwb.yongpay.top

free -h;  ps aux | grep nginx
来源：http://tgq.hongshengwenyu.top

[R64] 结束进程
来源：http://cqd.redwolf501.top

kill -9 $(pgrep -f app.py)
来源：http://iae.cdnleiting.top

[R65] 查看端口占用
来源：http://gtb.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bpd.nanxinkj.top

[R66] 定时任务
来源：http://dtv.jyoumei.cn

crontab -e;  crontab -l
来源：http://fqs.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://clt.zhixingplan.top

openssl rand -hex 16
来源：http://dle.hywenlv.cn

[R68] 计算文件校验值
来源：http://ljy.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vnp.pengpengdd.cyou

[R69] 生成随机密码
来源：http://xgw.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://eog.cashguo.top

[R70] 时间戳与互转
来源：http://zvm.bjfxy.top

date +%s;  date -d @1700000000
来源：http://nob.hongshengwenyu.top

[R71] 日期格式化
来源：http://ekq.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rdt.nanxuanxn.top

[R72] 等待端口就绪
来源：http://fwb.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dek.yongpay.top

[R73] 分割大日志
来源：http://syi.jianghu66.top

split -l 1000 big.log part_
来源：http://uac.fanxiaobao.xyz

[R74] 批量重命名
来源：http://xwh.sysykeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xrx.vehdjk.com

[R75] 导出环境变量
来源：http://dbg.ctjpmb.com

export PATH="$HOME/bin:$PATH"
来源：http://skg.svipenyu.cn

[R76] 使用临时文件
来源：http://tjo.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iom.nwbrower.top

[R77] 读取用户输入
来源：http://clc.xziqi.cn

read -rp "请输入: " ans
来源：http://pdy.sjlbkw.cn

[R78] 交互式菜单
来源：http://uft.gzhubu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cas.yj20258888.top

[R79] 解析命令行选项
来源：http://pse.hongshengwenyu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kxn.hysaishi.cn

[R80] 查看脚本执行耗时
来源：http://oul.0kj1m.cn

time ./run.sh
来源：http://fkh.jqgufenzy.top

================================================================================
来源：http://vhp.kuanghao11.cn

S. C / C++ 专题
来源：http://fqv.yfazqb.com

================================================================================
来源：http://yhz.yanxiufei.cn

[S01] C：Hello World
来源：http://kpx.hammf.cn

#include <stdio.h>
来源：http://pok.316326.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://tgw.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://ztx.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://xnn.xylfe.cn

[S03] C：读入整数
来源：http://fqa.ybcxt.top

int x; scanf("%d", &x);
来源：http://sxo.fktsv.cn

[S04] C：字符串复制
来源：http://xfm.gzhubu.top

char dst[32]; strcpy(dst, "hi");
来源：http://phe.shzxlz.cn

[S05] C：字符串长度
来源：http://exr.havefunace.top

strlen(s)
来源：http://dqa.sufxvd.cn

[S06] C：字符串比较
来源：http://uwm.tanke756.top

strcmp(a, b) == 0
来源：http://jbe.meibo888.top

[S07] C：数组遍历求和
来源：http://srx.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lnn.shuidangran.top

[S08] C：动态内存分配与释放
来源：http://npi.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wtv.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://qgj.jyoumei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bqw.yanxiufei.cn

[S10] C：指针与解引用
来源：http://qbj.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://ogv.fengsongda.top

[S11] C：逐行读文件
来源：http://nhw.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://wse.cqqwz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://aab.jlsjyb.cn

fclose(f);
来源：http://qbc.0kj1m.cn

[S12] C：写文件
来源：http://evu.yuxming.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hys.yuanzhike.top

[S13] C：宏定义
来源：http://rwg.vehdjk.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wqx.ctjpmb.com

[S14] C：枚举
来源：http://myr.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://xud.xylfe.cn

[S15] C：类型转换
来源：http://wvp.wangshuangyany.cn

(double) a / b
来源：http://hoh.0kj1m.cn

[S16] C：位操作置位
来源：http://gej.fktsv.cn

x |= (1 << 3);
来源：http://cnj.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://zdc.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ktp.c1oappe.top

[S18] C：命令行参数
来源：http://nqg.ivvv.top

int main(int argc, char **argv)
来源：http://san.yj202588.top

[S19] C：快速排序
来源：http://ivj.vqdsnc.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bcy.ybcxt.top

[S20] C：二分查找
来源：http://oni.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://feb.vqdsnc.cn

[S21] C：字符类别判断
来源：http://ulp.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tzq.jinqigfzy.top

[S22] C：字符串转数字
来源：http://dib.fengsongda.top

atoi("42");  strtod("3.14", NULL);
来源：http://soj.yvedp.cn

[S23] C：随机数
来源：http://gnr.yfazqb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ffi.hysaishi.cn

[S24] C：获取本地时间
来源：http://rbq.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ymg.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://cyj.shzxlz.cn

memcpy(dst, src, n);
来源：http://jdt.cheryme.top

[S26] C：内存清零
来源：http://vpp.aizwys.cn

memset(a, 0, sizeof a);
来源：http://ngb.yonumen.top

[S27] C：定义常量
来源：http://reb.dianchejie.cn

const double PI = 3.14159;
来源：http://mqm.gaohongyu789.top

[S28] C：静态变量
来源：http://ldf.bjfxy.top

static int counter = 0;
来源：http://apm.andypj.xyz

[S29] C：变参函数
来源：http://ovc.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hhe.sweek.top

[S30] C：头文件保护
来源：http://zuy.zdqjudy.top

#ifndef X_H
来源：http://lla.jyoumei.cn

#define X_H
来源：http://alp.jyoumei.cn

#endif
来源：http://bcf.ydzc1.top

[S31] C++：Hello World
来源：http://qqk.ppjwa.cn

#include <iostream>
来源：http://snh.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://bfb.sjlbkw.cn

[S32] C++：字符串
来源：http://srr.yanxiufei.cn

std::string s = "hi";  s += "!";
来源：http://uoh.zdbjq.cn

[S33] C++：vector 增删
来源：http://vyc.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pwn.ctjpmb.com

[S34] C++：遍历 vector
来源：http://iwn.xinyue.icu

for (auto &x : v) { std::cout << x; }
来源：http://bel.sweek.top

[S35] C++：map
来源：http://pba.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nke.yueranfly.top

[S36] C++：unordered_map
来源：http://bsc.snrcjt.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bfu.tianlin.xyz

[S37] C++：set
来源：http://jlz.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mej.redwolf501.top

[S38] C++：排序
来源：http://dwr.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://hei.zhoulong.xyz

[S39] C++：自定义比较器排序
来源：http://gnv.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dai.sysykeji.top

[S40] C++：查找元素
来源：http://eqp.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ouf.chenzaomai.com

[S41] C++：类与构造函数
来源：http://qxr.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nwm.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://mkj.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://kvi.havefunace.top

[S43] C++：智能指针
来源：http://oqq.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://lfu.sjlbkw.cn

[S44] C++：引用传参
来源：http://cac.ehwqpu.com

void inc(int &x) { ++x; }
来源：http://tiq.cashguo.top

[S45] C++：lambda
来源：http://mcs.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://goq.guannengcc.top

[S46] C++：函数模板
来源：http://ots.xingfuxueyuan.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gjy.cdnleiting.top

[S47] C++：结构化绑定遍历
来源：http://waj.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dsm.jinghuilouyu.cn

[S48] C++：逐行读文件
来源：http://ley.mhx1999.top

std::ifstream in("a.txt");  std::string line;
来源：http://fcz.chenzaomai.com

while (std::getline(in, line)) { }
来源：http://kup.sweek.top

[S49] C++：写文件
来源：http://pru.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jtn.quarkkingdee.top

[S50] C++：格式化数字
来源：http://vyn.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jrf.yueranfly.top

[S51] C++：显式类型转换
来源：http://hih.tarul.cn

static_cast<double>(a) / b
来源：http://stw.xinyue.icu

[S52] C++：const 与 noexcept
来源：http://bhd.nanxuanxn.top

int size() const noexcept { return n_; }
来源：http://izo.0kj1m.cn

[S53] C++：移动语义
来源：http://ezg.zhijiandao.cn

std::vector<int> w = std::move(v);
来源：http://cdc.zhijiandao.cn

[S54] C++：异常处理
来源：http://bwu.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tlm.yvedp.cn

[S55] C++：结构化绑定
来源：http://qya.fktsv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://coe.sweek.top

[S56] C++：optional
来源：http://xro.wangshuangyany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://msa.zhengqikj.top

[S57] C++：编译期常量
来源：http://htg.zhongyouzk.top

constexpr int N = 10;
来源：http://mbu.mhx1999.top

[S58] C++：命名空间
来源：http://sna.jinghuilouyu.cn

namespace ns { int f() { return 1; } }
来源：http://jtp.wangshuangyany.cn

[S59] C++：静态断言
来源：http://cxq.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kmy.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://toi.bbcook.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kly.xuetiantiany.cn

================================================================================
来源：http://phi.yueranfly.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vpn.fktsv.cn

================================================================================
来源：http://nfb.bjfxy.top

[T01] Kotlin：Hello World
来源：http://hyl.tian-w.cn

println("Hello")
来源：http://xzu.tianlin.xyz

[T02] Kotlin：变量
来源：http://btj.dashuyun.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uxz.52xcode.cn

[T03] Kotlin：字符串模板
来源：http://rtv.havefunace.top

"值: $b"
来源：http://mis.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://oea.nanxinkj.top

val n: String? = null;  n?.length
来源：http://lcv.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://rvj.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nei.shuidangran.top

[T06] Kotlin：集合映射
来源：http://zes.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://vna.smart0.xyz

[T07] Kotlin：集合过滤
来源：http://qnj.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://diz.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://pho.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://qvz.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://ihz.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://sce.xylfe.cn

[T10] Kotlin：默认参数
来源：http://dra.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://not.hywenlv.cn

[T11] Kotlin：协程
来源：http://sdh.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://idu.hcnkem.com

[T12] Kotlin：解构声明
来源：http://zuv.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://rbi.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://xih.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://oef.jinqigfzy.top

[T14] Kotlin：循环
来源：http://okt.316326.xyz

for (i in 1..10) println(i)
来源：http://mfv.ydzc1.top

[T15] Kotlin：接口
来源：http://xzk.iojbl.cn

interface Shape { fun area(): Double }
来源：http://oau.jqgufenzy.top

[T16] Swift：Hello World
来源：http://djl.52xcode.cn

print("Hello")
来源：http://zkc.52xcode.cn

[T17] Swift：变量与常量
来源：http://ftm.cdnleiting.top

var a = 1;  let b = 2
来源：http://vyj.chenjidiqi.icu

[T18] Swift：字符串插值
来源：http://hlq.dashuyun.cn

"值: \(b)"
来源：http://woe.bbcook.cn

[T19] Swift：可选绑定
来源：http://yjo.sxryk.cn

if let n = opt { print(n) }
来源：http://wtc.316326.xyz

[T20] Swift：数组操作
来源：http://yfu.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://cmk.pycfn.com

[T21] Swift：遍历
来源：http://ooj.xuetiantiany.cn

for x in a { print(x) }
来源：http://smu.shuidangran.top

[T22] Swift：字典
来源：http://qah.ehwqpu.com

var d = ["a": 1];  d["b"] = 2
来源：http://bxr.shangyingyoupin.top

[T23] Swift：函数
来源：http://jqz.fanxiaobao.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xqh.birdmap.top

[T24] Swift：闭包
来源：http://ani.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zuj.sjlbkw.cn

[T25] Swift：结构体
来源：http://soi.shanyushiyangtech.top

struct P { var x: Int }
来源：http://vsh.xingfuxueyuan.xyz

[T26] Swift：类与重写
来源：http://guw.svipenyu.cn

class A: Base { override func f() {} }
来源：http://cpn.0kj1m.cn

[T27] Swift：错误处理
来源：http://dss.shanyushiyangtech.top

do { try f() } catch { print(error) }
来源：http://fqr.yonumen.top

[T28] Swift：枚举
来源：http://pld.shzxlz.cn

enum Color { case red, green }
来源：http://wau.ctjpmb.com

[T29] Swift：guard 提前返回
来源：http://viz.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://ctv.yueranfly.top

[T30] Swift：协议
来源：http://eoy.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://jfa.yfazqb.com

[T31] Lua：Hello World
来源：http://fjc.316326.xyz

print("Hello")
来源：http://xux.bbcook.cn

[T32] Lua：局部变量
来源：http://wbe.gzhubu.top

local a = 1
来源：http://clw.wangdashe.top

[T33] Lua：表（数组）
来源：http://wfn.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iyq.kuanghao11.cn

[T34] Lua：遍历表
来源：http://elp.guowangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ero.jqgfzy.top

[T35] Lua：字典表
来源：http://get.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://ogg.meibo888.top

[T36] Lua：函数
来源：http://luf.iojbl.cn

function add(a, b) return a + b end
来源：http://lvr.zhengqikj.top

[T37] Lua：字符串拼接
来源：http://uga.yj202588.top

"a" .. "b"
来源：http://kzj.smart0.xyz

[T38] Lua：条件
来源：http://ouh.tanke756.top

if x > 0 then print("正") end
来源：http://rzr.iojbl.cn

[T39] Lua：模式匹配
来源：http://lqc.316326.xyz

string.find(s, "%d+")
来源：http://hle.zdqjudy.top

[T40] Lua：元表
来源：http://hpj.chenzaomai.com

setmetatable({}, { __index = base })
来源：http://cqh.jqgfzy.top

[T41] Perl：Hello World
来源：http://wxn.9152youxi.cn

print "Hello\n";
来源：http://uui.nanxinkj.top

[T42] Perl：变量类型
来源：http://xcw.yfazqb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ddg.dianchejie.cn

[T43] Perl：字符串插值
来源：http://etv.yfazqb.com

"值: $a"
来源：http://zlc.cashguo.top

[T44] Perl：条件
来源：http://iei.nanxuanxn.top

if ($a > 0) { print "正"; }
来源：http://yat.vehdjk.com

[T45] Perl：数组遍历
来源：http://gks.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://neo.aibaodan.cn

[T46] Perl：哈希操作
来源：http://tkr.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zwp.dianchejie.cn

[T47] Perl：正则捕获
来源：http://bvg.fktsv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hig.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://mry.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://uew.snrcjt.cn

[T49] Perl：函数
来源：http://fgc.xuetiantiany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cpb.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://rxm.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://emb.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://egy.hnxiangtu.top

[T51] Scala：Hello World
来源：http://cbx.0kj1m.cn

println("Hello")
来源：http://onr.shangyingyoupin.top

[T52] Scala：变量
来源：http://psf.kuanghao11.cn

val a = 1;  var b = 2
来源：http://pes.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://kcp.fanxiaobao.xyz

s"值: $b"
来源：http://nmm.jyoumei.cn

[T54] Scala：集合映射
来源：http://wau.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://ffg.yfazqb.com

[T55] Scala：集合过滤
来源：http://ghr.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wef.cashguo.top

[T56] Scala：样例类
来源：http://vei.yuxming.cn

case class User(name: String, age: Int)
来源：http://hen.xziqi.cn

[T57] Scala：模式匹配
来源：http://zvx.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ert.aizwys.cn

[T58] Scala：函数定义
来源：http://quw.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fbw.yj20258888.top

[T59] Scala：循环
来源：http://alj.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://jza.gotoacloud.top

[T60] Scala：折叠
来源：http://xlw.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mhn.nanxuanxn.top

================================================================================
来源：http://ssm.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rly.c1oappe.top

================================================================================
来源：http://soh.tian-w.cn

[U01] Py：创建虚拟环境
来源：http://bou.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://uix.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://vza.svipenyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://chn.yvedp.cn


<!-- 参考信息 -->