代发 wailian999

df -h;  du -sh *
来源：http://mqr.cdnleiting.top

[R62] 找最占空间的文件
来源：http://xbj.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://nhg.daxiang520.top

[R63] 内存与进程
来源：http://tbz.xinyue.icu

free -h;  ps aux | grep nginx
来源：http://iis.jinqigfzy.top

[R64] 结束进程
来源：http://sdf.svipenyu.cn

kill -9 $(pgrep -f app.py)
来源：http://xiq.hesvh.cn

[R65] 查看端口占用
来源：http://iml.wangdashe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://txl.yonumen.top

[R66] 定时任务
来源：http://xuw.pycfn.com

crontab -e;  crontab -l
来源：http://fts.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://tav.snrcjt.cn

openssl rand -hex 16
来源：http://gzm.tian-w.cn

[R68] 计算文件校验值
来源：http://vcd.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://twz.ydzc1.top

[R69] 生成随机密码
来源：http://rwa.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://hwz.ydzc1.top

[R70] 时间戳与互转
来源：http://ohs.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://hqj.zhixingplan.top

[R71] 日期格式化
来源：http://wmc.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bdx.guannengcc.top

[R72] 等待端口就绪
来源：http://vit.redwolf501.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yro.wangdashe.top

[R73] 分割大日志
来源：http://cmb.c1oappe.top

split -l 1000 big.log part_
来源：http://vvs.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://zlv.shuidangran.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vsk.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://qtj.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://sxr.quarkkingdee.top

[R76] 使用临时文件
来源：http://vbx.shzxlz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tow.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://mmn.sxryk.cn

read -rp "请输入: " ans
来源：http://krl.jyoumei.cn

[R78] 交互式菜单
来源：http://gxa.sysykeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jrx.9152youxi.cn

[R79] 解析命令行选项
来源：http://hor.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nyc.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://vto.xylfe.cn

time ./run.sh
来源：http://czv.aizwys.cn

================================================================================
来源：http://ybb.yonumen.top

S. C / C++ 专题
来源：http://qwt.52xcode.cn

================================================================================
来源：http://euk.hywenlv.cn

[S01] C：Hello World
来源：http://chf.feifeiyinyue.top

#include <stdio.h>
来源：http://xbe.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bcu.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://jrn.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://fdy.yanxiufei.cn

[S03] C：读入整数
来源：http://bwv.chenlongwang.top

int x; scanf("%d", &x);
来源：http://lqu.daxiang520.top

[S04] C：字符串复制
来源：http://ccr.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://yeo.yj20258.top

[S05] C：字符串长度
来源：http://pey.ybcxt.top

strlen(s)
来源：http://hpx.dashuyun.cn

[S06] C：字符串比较
来源：http://duh.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://fue.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://cax.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gtr.guannengcc.top

[S08] C：动态内存分配与释放
来源：http://stm.ppjwa.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://grz.yj20258888.top

[S09] C：结构体定义与初始化
来源：http://aen.jinghuilouyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ikz.yvedp.cn

[S10] C：指针与解引用
来源：http://rkk.gzhubu.top

int *p = &a;  *p = 5;
来源：http://lxg.hnxiangtu.top

[S11] C：逐行读文件
来源：http://txz.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://mks.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rkc.jiagoushi.top

fclose(f);
来源：http://wjz.ehwqpu.com

[S12] C：写文件
来源：http://nbc.jqgufenzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jsn.yueranfly.top

[S13] C：宏定义
来源：http://yqt.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oyh.xylfe.cn

[S14] C：枚举
来源：http://fpp.yj20258.top

enum Color { RED, GREEN, BLUE };
来源：http://auk.jianghu66.top

[S15] C：类型转换
来源：http://dxo.fanxiaobao.xyz

(double) a / b
来源：http://zns.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://zgp.fanxiaobao.xyz

x |= (1 << 3);
来源：http://pst.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://hhc.gotoacloud.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pxq.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://xfz.uphjek.com

int main(int argc, char **argv)
来源：http://wgc.c1oappe.top

[S19] C：快速排序
来源：http://dwr.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://hcb.shzxlz.cn

[S20] C：二分查找
来源：http://etf.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eqz.jqgfzy.top

[S21] C：字符类别判断
来源：http://jse.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dpb.xziqi.cn

[S22] C：字符串转数字
来源：http://xej.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://kye.shuidangran.top

[S23] C：随机数
来源：http://sub.shanyushiyangtech.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ikf.ivvv.top

[S24] C：获取本地时间
来源：http://tkm.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rbv.zhaomingkeji.xyz

[S25] C：内存拷贝
来源：http://ekw.tarul.cn

memcpy(dst, src, n);
来源：http://yfu.fktsv.cn

[S26] C：内存清零
来源：http://omc.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://lcx.redwolf501.top

[S27] C：定义常量
来源：http://dbr.andypj.xyz

const double PI = 3.14159;
来源：http://pul.ivvv.top

[S28] C：静态变量
来源：http://krg.gogol.net.cn

static int counter = 0;
来源：http://rtj.0kj1m.cn

[S29] C：变参函数
来源：http://xoc.hywenlv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qtu.nwbrower.top

[S30] C：头文件保护
来源：http://dco.gzhubu.top

#ifndef X_H
来源：http://vfr.dashuyun.cn

#define X_H
来源：http://inh.fehbvm.com

#endif
来源：http://ukn.yfazqb.com

[S31] C++：Hello World
来源：http://wba.wangdashe.top

#include <iostream>
来源：http://lfq.tarul.cn

int main() { std::cout << "Hello\n"; }
来源：http://sjq.zhaomingkeji.xyz

[S32] C++：字符串
来源：http://mka.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://jus.chenlongwang.top

[S33] C++：vector 增删
来源：http://vjd.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hqy.sweek.top

[S34] C++：遍历 vector
来源：http://vfn.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://jfz.hywenlv.cn

[S35] C++：map
来源：http://ydy.sxryk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://twm.zhijiandao.cn

[S36] C++：unordered_map
来源：http://hbm.xylfe.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dgj.ydzc1.top

[S37] C++：set
来源：http://dpz.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://spx.birdmap.top

[S38] C++：排序
来源：http://jec.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://ybl.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://tvc.zhongyouzk.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sbn.yj20258.top

[S40] C++：查找元素
来源：http://hyu.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hhe.cashguo.top

[S41] C++：类与构造函数
来源：http://lmd.nanxuanxn.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nel.fktsv.cn

[S42] C++：继承与虚函数
来源：http://zdz.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://gsv.hnqzz.top

[S43] C++：智能指针
来源：http://jej.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://ean.sxryk.cn

[S44] C++：引用传参
来源：http://mrr.iojbl.cn

void inc(int &x) { ++x; }
来源：http://nxb.aibaodan.cn

[S45] C++：lambda
来源：http://jlk.sweek.top

auto add = [](int a, int b) { return a + b; };
来源：http://uho.zycfv.cn

[S46] C++：函数模板
来源：http://nfk.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zsv.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://fhf.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lya.mhx1999.top

[S48] C++：逐行读文件
来源：http://trl.uphjek.com

std::ifstream in("a.txt");  std::string line;
来源：http://ptm.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://fcs.nwbrower.top

[S49] C++：写文件
来源：http://klv.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jiz.hywenlv.cn

[S50] C++：格式化数字
来源：http://iwc.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pra.cdnleiting.top

[S51] C++：显式类型转换
来源：http://uoa.ydzc1.top

static_cast<double>(a) / b
来源：http://fok.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://lrf.52xcode.cn

int size() const noexcept { return n_; }
来源：http://qoo.yuxming.cn

[S53] C++：移动语义
来源：http://rxx.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://pxs.tian-w.cn

[S54] C++：异常处理
来源：http://bnm.nanxinkj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fuf.hcnkem.com

[S55] C++：结构化绑定
来源：http://hyx.yuxming.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://duw.yongpay.top

[S56] C++：optional
来源：http://sdp.sysykeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zej.haohaochexian.top

[S57] C++：编译期常量
来源：http://vor.yj20258.top

constexpr int N = 10;
来源：http://lml.fengsongda.top

[S58] C++：命名空间
来源：http://pno.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://yfo.316326.xyz

[S59] C++：静态断言
来源：http://wje.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://otp.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://mvt.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://swr.hywenlv.cn

================================================================================
来源：http://mpq.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pos.yj202588.top

================================================================================
来源：http://ncl.ybcxt.top

[T01] Kotlin：Hello World
来源：http://fwh.zdqjudy.top

println("Hello")
来源：http://zkf.shuidangran.top

[T02] Kotlin：变量
来源：http://fsw.zycfv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zab.jianghu66.top

[T03] Kotlin：字符串模板
来源：http://rhw.yfazqb.com

"值: $b"
来源：http://fat.yueranfly.top

[T04] Kotlin：空安全
来源：http://dxq.yueranfly.top

val n: String? = null;  n?.length
来源：http://mvs.sxryk.cn

[T05] Kotlin：when 表达式
来源：http://uui.pengpengdd.cyou

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://win.fanxiaobao.xyz

[T06] Kotlin：集合映射
来源：http://dpq.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iat.zhoulong.xyz

[T07] Kotlin：集合过滤
来源：http://wwd.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dnk.cheryme.top

[T08] Kotlin：数据类
来源：http://dsj.sufxvd.cn

data class User(val name: String, val age: Int)
来源：http://kfa.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://opy.haohaochexian.top

fun String.exclaim() = this + "!"
来源：http://fwr.iojbl.cn

[T10] Kotlin：默认参数
来源：http://kkp.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://gyt.chenzaomai.com

[T11] Kotlin：协程
来源：http://wwz.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sab.fengsongda.top

[T12] Kotlin：解构声明
来源：http://trq.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://hgo.zdbjq.cn

[T13] Kotlin：只读 Map
来源：http://akp.daxiang520.top

val m = mapOf("a" to 1)
来源：http://pxi.jinqigufen.top

[T14] Kotlin：循环
来源：http://zdj.andypj.xyz

for (i in 1..10) println(i)
来源：http://ojo.zycfv.cn

[T15] Kotlin：接口
来源：http://zyr.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://abn.sjlbkw.cn

[T16] Swift：Hello World
来源：http://knq.ydjk.org.cn

print("Hello")
来源：http://bon.fengsongda.top

[T17] Swift：变量与常量
来源：http://nld.daxiang520.top

var a = 1;  let b = 2
来源：http://ltu.tarul.cn

[T18] Swift：字符串插值
来源：http://pru.jiagoushi.top

"值: \(b)"
来源：http://chq.ctjpmb.com

[T19] Swift：可选绑定
来源：http://tpm.zhixingplan.top

if let n = opt { print(n) }
来源：http://cxx.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://scp.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://fle.fehbvm.com

[T21] Swift：遍历
来源：http://mcn.dashuyun.cn

for x in a { print(x) }
来源：http://dog.wangdashe.top

[T22] Swift：字典
来源：http://eys.ehwqpu.com

var d = ["a": 1];  d["b"] = 2
来源：http://mlw.chenjidiqi.icu

[T23] Swift：函数
来源：http://pau.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kga.yangfankeji.com

[T24] Swift：闭包
来源：http://voz.fzhhl.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ieo.fzhhl.top

[T25] Swift：结构体
来源：http://yzw.sysykeji.top

struct P { var x: Int }
来源：http://rvo.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://wgw.hesvh.cn

class A: Base { override func f() {} }
来源：http://ioe.fktsv.cn

[T27] Swift：错误处理
来源：http://ggr.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://war.mhx1999.top

[T28] Swift：枚举
来源：http://jnd.yvedp.cn

enum Color { case red, green }
来源：http://cqd.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://ywk.gzhubu.top

guard let x = opt else { return }
来源：http://qea.pycfn.com

[T30] Swift：协议
来源：http://sxt.uphjek.com

protocol Shape { func area() -> Double }
来源：http://eir.fehbvm.com

[T31] Lua：Hello World
来源：http://dzr.fehbvm.com

print("Hello")
来源：http://ayu.316326.xyz

[T32] Lua：局部变量
来源：http://lfa.jianghu66.top

local a = 1
来源：http://mns.0kj1m.cn

[T33] Lua：表（数组）
来源：http://lyl.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dsc.yonumen.top

[T34] Lua：遍历表
来源：http://hfo.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nbg.shangyingyoupin.top

[T35] Lua：字典表
来源：http://sub.zdbjq.cn

local d = { a = 1 };  d.b = 2
来源：http://kwh.meibo888.top

[T36] Lua：函数
来源：http://xqq.shanyushiyangkeji.top

function add(a, b) return a + b end
来源：http://cfz.cucudq.cn

[T37] Lua：字符串拼接
来源：http://wmn.sysykeji.top

"a" .. "b"
来源：http://nqe.ybcxt.top

[T38] Lua：条件
来源：http://nef.sweek.top

if x > 0 then print("正") end
来源：http://auy.yj20258.top

[T39] Lua：模式匹配
来源：http://mlj.fengsongda.top

string.find(s, "%d+")
来源：http://mss.epnwcf.com

[T40] Lua：元表
来源：http://ito.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://tal.tian-w.cn

[T41] Perl：Hello World
来源：http://plx.jyoumei.cn

print "Hello\n";
来源：http://vim.yanxiufei.cn

[T42] Perl：变量类型
来源：http://zvp.dianchejie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ptf.xziqi.cn

[T43] Perl：字符串插值
来源：http://ora.vqdsnc.cn

"值: $a"
来源：http://plw.jqgfzy.top

[T44] Perl：条件
来源：http://muv.cheryme.top

if ($a > 0) { print "正"; }
来源：http://akz.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://qmr.snrcjt.cn

for my $x (@arr) { print $x; }
来源：http://swj.jyoumei.cn

[T46] Perl：哈希操作
来源：http://pao.pycfn.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bzo.hesvh.cn

[T47] Perl：正则捕获
来源：http://pte.quarkkingdee.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://svk.havefunace.top

[T48] Perl：正则替换
来源：http://ldh.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://pwm.wangshuangyany.cn

[T49] Perl：函数
来源：http://nft.zhiwuduotai.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yqn.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://oos.ppjwa.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bgq.hywenlv.cn

while (my $line = <$fh>) { print $line; }
来源：http://rwd.tian-w.cn

[T51] Scala：Hello World
来源：http://sbd.shuidangran.top

println("Hello")
来源：http://khi.zdbjq.cn

[T52] Scala：变量
来源：http://xrm.ydzc1.top

val a = 1;  var b = 2
来源：http://mko.yfazqb.com

[T53] Scala：字符串插值
来源：http://rcp.hcnkem.com

s"值: $b"
来源：http://bgo.cucudq.cn

[T54] Scala：集合映射
来源：http://pts.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://mqv.nanxinkj.top

[T55] Scala：集合过滤
来源：http://xmx.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://ovk.yvedp.cn

[T56] Scala：样例类
来源：http://vxs.kuanghao11.cn

case class User(name: String, age: Int)
来源：http://lng.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://via.jlsjyb.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://shf.zhoulong.xyz

[T58] Scala：函数定义
来源：http://mwe.hfpthk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xbg.zhiwuduotai.top

[T59] Scala：循环
来源：http://okr.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://vap.shangyingyoupin.top

[T60] Scala：折叠
来源：http://csl.hywenlv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zbl.feifeiyinyue.top

================================================================================
来源：http://mam.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://voc.nwbrower.top

================================================================================
来源：http://iea.nanxinkj.top

[U01] Py：创建虚拟环境
来源：http://jii.vqdsnc.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ppq.pengpengdd.cyou

[U02] Py：导出 / 安装依赖
来源：http://njh.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rva.bjfxy.top


<!-- 参考信息 -->