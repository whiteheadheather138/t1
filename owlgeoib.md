代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lwq.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://ssc.ydjk.org.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xtg.ydjk.org.cn

[R61] 磁盘占用
来源：http://rtu.yonumen.top

df -h;  du -sh *
来源：http://lyb.gaohongyu789.top

[R62] 找最占空间的文件
来源：http://swt.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://syl.tanke756.top

[R63] 内存与进程
来源：http://wot.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://sem.jianghu66.top

[R64] 结束进程
来源：http://lao.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://xqx.zhoulong.xyz

[R65] 查看端口占用
来源：http://txp.zdbjq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jlm.cucudq.cn

[R66] 定时任务
来源：http://eig.zdqjudy.top

crontab -e;  crontab -l
来源：http://ssv.nanxinkj.top

[R67] 生成随机十六进制串
来源：http://ulq.sufxvd.cn

openssl rand -hex 16
来源：http://afs.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://brb.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://rpf.zhiwuduotai.top

[R69] 生成随机密码
来源：http://xxy.jqgufenzy.top

head -c 16 /dev/urandom | base64
来源：http://imk.ywan-chungtsiang.top

[R70] 时间戳与互转
来源：http://nco.pycfn.com

date +%s;  date -d @1700000000
来源：http://jeu.jqgufenzy.top

[R71] 日期格式化
来源：http://jiq.sweek.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bqn.gaohongyu789.top

[R72] 等待端口就绪
来源：http://mza.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dmm.guowangkeji.top

[R73] 分割大日志
来源：http://nev.ydjk.org.cn

split -l 1000 big.log part_
来源：http://atr.hnxiangtu.top

[R74] 批量重命名
来源：http://tsz.52xcode.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dlk.9152youxi.cn

[R75] 导出环境变量
来源：http://vzv.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://xsg.yonumen.top

[R76] 使用临时文件
来源：http://rgg.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cuo.havefunace.top

[R77] 读取用户输入
来源：http://ije.yueranfly.top

read -rp "请输入: " ans
来源：http://bry.fanxiaobao.xyz

[R78] 交互式菜单
来源：http://una.fehbvm.com

select opt in a b c; do echo "$opt"; break; done
来源：http://jsn.pycfn.com

[R79] 解析命令行选项
来源：http://pki.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pza.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://ndo.yonumen.top

time ./run.sh
来源：http://bur.yonumen.top

================================================================================
来源：http://cby.ivvv.top

S. C / C++ 专题
来源：http://rba.sufxvd.cn

================================================================================
来源：http://zry.wangshuangyany.cn

[S01] C：Hello World
来源：http://jjy.havefunace.top

#include <stdio.h>
来源：http://kcl.meibo888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tvo.cashguo.top

[S02] C：变量与格式化输出
来源：http://hdk.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://umz.havefunace.top

[S03] C：读入整数
来源：http://zqq.jianghu66.top

int x; scanf("%d", &x);
来源：http://hgn.yj20258888.top

[S04] C：字符串复制
来源：http://lsr.chenzaomai.com

char dst[32]; strcpy(dst, "hi");
来源：http://xmy.haohaochexian.top

[S05] C：字符串长度
来源：http://wxe.yj20258.top

strlen(s)
来源：http://tvj.jqgufenzy.top

[S06] C：字符串比较
来源：http://dyi.yanxiufei.cn

strcmp(a, b) == 0
来源：http://gnf.wangshuangyany.cn

[S07] C：数组遍历求和
来源：http://nmt.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gmn.shuidangran.top

[S08] C：动态内存分配与释放
来源：http://cny.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xje.dashuyun.cn

[S09] C：结构体定义与初始化
来源：http://via.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ksw.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://brr.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://hqr.fengsongda.top

[S11] C：逐行读文件
来源：http://mau.cucudq.cn

FILE *f = fopen("a.txt", "r");
来源：http://hge.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fay.aizwys.cn

fclose(f);
来源：http://unj.tian-w.cn

[S12] C：写文件
来源：http://dgs.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rlg.jiagoushi.top

[S13] C：宏定义
来源：http://mym.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ryd.ctjpmb.com

[S14] C：枚举
来源：http://uov.jinghuilouyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://yjl.xuetiantiany.cn

[S15] C：类型转换
来源：http://ong.jlsjyb.cn

(double) a / b
来源：http://urk.vehdjk.com

[S16] C：位操作置位
来源：http://mox.fengsongda.top

x |= (1 << 3);
来源：http://gfs.fengsongda.top

[S17] C：安全拼接字符串
来源：http://tzk.birdmap.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pnf.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://lwq.yuxming.cn

int main(int argc, char **argv)
来源：http://fgi.gzhubu.top

[S19] C：快速排序
来源：http://wce.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://lzy.hammf.cn

[S20] C：二分查找
来源：http://moe.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jdm.dashuyun.cn

[S21] C：字符类别判断
来源：http://hdb.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://czs.ywan-chungtsiang.top

[S22] C：字符串转数字
来源：http://ppl.pycfn.com

atoi("42");  strtod("3.14", NULL);
来源：http://raz.yj202588.top

[S23] C：随机数
来源：http://drq.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://fww.sysykeji.top

[S24] C：获取本地时间
来源：http://wuj.daria6918.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zqm.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://yxt.tianlin.xyz

memcpy(dst, src, n);
来源：http://dmc.mhx1999.top

[S26] C：内存清零
来源：http://nyt.yuanzhike.top

memset(a, 0, sizeof a);
来源：http://nai.gaohongyu789.top

[S27] C：定义常量
来源：http://zmx.daxiang520.top

const double PI = 3.14159;
来源：http://slv.sxryk.cn

[S28] C：静态变量
来源：http://tha.hesvh.cn

static int counter = 0;
来源：http://wps.xylfe.cn

[S29] C：变参函数
来源：http://bma.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uig.pycfn.com

[S30] C：头文件保护
来源：http://thl.quarkkingdee.top

#ifndef X_H
来源：http://enr.hysaishi.cn

#define X_H
来源：http://tng.jqgufenzy.top

#endif
来源：http://uqf.yangfankeji.com

[S31] C++：Hello World
来源：http://mcl.birdmap.top

#include <iostream>
来源：http://wce.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://juq.mhx1999.top

[S32] C++：字符串
来源：http://ddb.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://bzc.feifeiyinyue.top

[S33] C++：vector 增删
来源：http://yds.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fqt.gotoacloud.top

[S34] C++：遍历 vector
来源：http://nrg.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://mpu.hcnkem.com

[S35] C++：map
来源：http://ubv.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://itm.havefunace.top

[S36] C++：unordered_map
来源：http://ifp.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ywi.sjlbkw.cn

[S37] C++：set
来源：http://hxr.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sdl.quarkkingdee.top

[S38] C++：排序
来源：http://jvb.gogol.net.cn

std::sort(v.begin(), v.end());
来源：http://zgx.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://ebj.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ufj.jiagoushi.top

[S40] C++：查找元素
来源：http://izv.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fkj.cashguo.top

[S41] C++：类与构造函数
来源：http://hzr.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dly.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://awe.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://iqo.meibo888.top

[S43] C++：智能指针
来源：http://qse.wangdashe.top

auto p = std::make_unique<int>(5);
来源：http://ewb.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://kdq.guowangkeji.top

void inc(int &x) { ++x; }
来源：http://dfj.zycfv.cn

[S45] C++：lambda
来源：http://btu.iojbl.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fej.zhongyouzk.top

[S46] C++：函数模板
来源：http://hsq.fktsv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jmy.bjfxy.top

[S47] C++：结构化绑定遍历
来源：http://foh.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jaj.jinqigfzy.top

[S48] C++：逐行读文件
来源：http://xwl.yuxming.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nzu.jiagoushi.top

while (std::getline(in, line)) { }
来源：http://wia.feifeiyinyue.top

[S49] C++：写文件
来源：http://xcd.sxryk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ovr.shuidangran.top

[S50] C++：格式化数字
来源：http://twu.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vih.yonumen.top

[S51] C++：显式类型转换
来源：http://udb.daria6918.cn

static_cast<double>(a) / b
来源：http://xwa.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://lhs.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://lty.dianchejie.cn

[S53] C++：移动语义
来源：http://cbw.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://jnc.sweek.top

[S54] C++：异常处理
来源：http://zkb.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hpi.smart0.xyz

[S55] C++：结构化绑定
来源：http://zzv.guowangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rtj.fktsv.cn

[S56] C++：optional
来源：http://zgv.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cff.daria6918.cn

[S57] C++：编译期常量
来源：http://abx.sxryk.cn

constexpr int N = 10;
来源：http://gfk.hywenlv.cn

[S58] C++：命名空间
来源：http://mvv.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://okn.hongshengwenyu.top

[S59] C++：静态断言
来源：http://dwb.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://csk.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://dnb.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tzw.daria6918.cn

================================================================================
来源：http://hza.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lvf.jqgufenzy.top

================================================================================
来源：http://znv.jianghu66.top

[T01] Kotlin：Hello World
来源：http://juj.fktsv.cn

println("Hello")
来源：http://svl.hesvh.cn

[T02] Kotlin：变量
来源：http://rwc.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nvk.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://wvt.tian-w.cn

"值: $b"
来源：http://sfk.bjfxy.top

[T04] Kotlin：空安全
来源：http://qxu.sweek.top

val n: String? = null;  n?.length
来源：http://kgy.zhoulong.xyz

[T05] Kotlin：when 表达式
来源：http://rur.dashuyun.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xfq.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://orw.hysaishi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tkb.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://oms.dianchejie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ldv.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://pun.hammf.cn

data class User(val name: String, val age: Int)
来源：http://laa.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://zli.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://ery.xinyue.icu

[T10] Kotlin：默认参数
来源：http://nzk.yanxiufei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qry.hywenlv.cn

[T11] Kotlin：协程
来源：http://lbw.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://uis.meibo888.top

[T12] Kotlin：解构声明
来源：http://dkm.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://vvd.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://mnq.hnqzz.top

val m = mapOf("a" to 1)
来源：http://qji.shuidangran.top

[T14] Kotlin：循环
来源：http://olx.nwbrower.top

for (i in 1..10) println(i)
来源：http://hps.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://rpj.yongpay.top

interface Shape { fun area(): Double }
来源：http://jcl.epnwcf.com

[T16] Swift：Hello World
来源：http://rjq.ydjk.org.cn

print("Hello")
来源：http://zzg.birdmap.top

[T17] Swift：变量与常量
来源：http://dtk.jianghu66.top

var a = 1;  let b = 2
来源：http://hng.zhijiandao.cn

[T18] Swift：字符串插值
来源：http://qmv.wangshuangyany.cn

"值: \(b)"
来源：http://bxh.jlsjyb.cn

[T19] Swift：可选绑定
来源：http://ufd.fzhhl.top

if let n = opt { print(n) }
来源：http://ksl.xuanzx.com

[T20] Swift：数组操作
来源：http://nfm.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://dra.daxiang520.top

[T21] Swift：遍历
来源：http://lmx.sxryk.cn

for x in a { print(x) }
来源：http://bfn.bjfxy.top

[T22] Swift：字典
来源：http://vfc.shzxlz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bct.shzxlz.cn

[T23] Swift：函数
来源：http://iyn.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nto.chenlongwang.top

[T24] Swift：闭包
来源：http://xvu.nanxinkj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fht.jlsjyb.cn

[T25] Swift：结构体
来源：http://yjd.kuanghao11.cn

struct P { var x: Int }
来源：http://bzp.sxryk.cn

[T26] Swift：类与重写
来源：http://oda.bbcook.cn

class A: Base { override func f() {} }
来源：http://ogq.birdmap.top

[T27] Swift：错误处理
来源：http://onb.yueranfly.top

do { try f() } catch { print(error) }
来源：http://dvs.yongpay.top

[T28] Swift：枚举
来源：http://nic.epnwcf.com

enum Color { case red, green }
来源：http://tye.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://edj.nanxuanxn.top

guard let x = opt else { return }
来源：http://xil.hfpthk.cn

[T30] Swift：协议
来源：http://kzk.andypj.xyz

protocol Shape { func area() -> Double }
来源：http://zyv.tanke756.top

[T31] Lua：Hello World
来源：http://fcw.snrcjt.cn

print("Hello")
来源：http://zxk.yuxming.cn

[T32] Lua：局部变量
来源：http://ndx.wangshuangyany.cn

local a = 1
来源：http://wgp.9152youxi.cn

[T33] Lua：表（数组）
来源：http://tnf.nwbrower.top

local t = {1, 2, 3};  t[4] = 4
来源：http://skd.zdbjq.cn

[T34] Lua：遍历表
来源：http://xqk.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xzm.daria6918.cn

[T35] Lua：字典表
来源：http://obe.sxryk.cn

local d = { a = 1 };  d.b = 2
来源：http://ikl.hnqzz.top

[T36] Lua：函数
来源：http://nru.epnwcf.com

function add(a, b) return a + b end
来源：http://tma.sxryk.cn

[T37] Lua：字符串拼接
来源：http://mrt.yj20258888.top

"a" .. "b"
来源：http://mao.uphjek.com

[T38] Lua：条件
来源：http://xdu.smart0.xyz

if x > 0 then print("正") end
来源：http://fva.yanxiufei.cn

[T39] Lua：模式匹配
来源：http://plm.jqgufenzy.top

string.find(s, "%d+")
来源：http://mpz.cucudq.cn

[T40] Lua：元表
来源：http://ely.sweek.top

setmetatable({}, { __index = base })
来源：http://ezx.uphjek.com

[T41] Perl：Hello World
来源：http://lhz.shuidangran.top

print "Hello\n";
来源：http://mww.xziqi.cn

[T42] Perl：变量类型
来源：http://zpx.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hqj.pycfn.com

[T43] Perl：字符串插值
来源：http://jzm.316326.xyz

"值: $a"
来源：http://hnk.dianchejie.cn

[T44] Perl：条件
来源：http://pwl.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://pgu.sufxvd.cn

[T45] Perl：数组遍历
来源：http://wog.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://igx.ppjwa.cn

[T46] Perl：哈希操作
来源：http://dgi.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uwp.guannengcc.top

[T47] Perl：正则捕获
来源：http://hrw.jinqigfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ghl.zhiwuduotai.top

[T48] Perl：正则替换
来源：http://lcu.fengsongda.top

$s =~ s/old/new/g;
来源：http://zyz.fanxiaobao.xyz

[T49] Perl：函数
来源：http://cru.jianghu66.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cnu.yj202588.top

[T50] Perl：逐行读文件
来源：http://rqu.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mme.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://rbd.zdqjudy.top

[T51] Scala：Hello World
来源：http://oau.nwbrower.top

println("Hello")
来源：http://zsg.jqgfzy.top

[T52] Scala：变量
来源：http://qzf.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://kue.havefunace.top

[T53] Scala：字符串插值
来源：http://hgv.hnxiangtu.top

s"值: $b"
来源：http://pgx.316326.xyz

[T54] Scala：集合映射
来源：http://qhu.quarkkingdee.top

List(1, 2, 3).map(_ * 2)
来源：http://jta.aizwys.cn

[T55] Scala：集合过滤
来源：http://kmx.hcnkem.com

List(1, 2, 3).filter(_ > 1)
来源：http://dts.yj20258.top

[T56] Scala：样例类
来源：http://ypb.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://tlz.uphjek.com

[T57] Scala：模式匹配
来源：http://eus.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wan.vqdsnc.cn

[T58] Scala：函数定义
来源：http://xkn.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://chh.meibo888.top

[T59] Scala：循环
来源：http://gma.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://gbe.sxryk.cn

[T60] Scala：折叠
来源：http://fge.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pkb.ydjk.org.cn

================================================================================
来源：http://qfh.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cyj.jlsjyb.cn

================================================================================
来源：http://xfs.jinghuilouyu.cn


<!-- 参考信息 -->