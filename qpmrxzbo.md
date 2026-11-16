代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fmz.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://lou.jiagoushi.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ilx.sxryk.cn

[R61] 磁盘占用
来源：http://sao.jqgufenzy.top

df -h;  du -sh *
来源：http://gwg.hammf.cn

[R62] 找最占空间的文件
来源：http://cav.zhoulong.xyz

du -ah . | sort -rh | head -10
来源：http://bpl.guowangkeji.top

[R63] 内存与进程
来源：http://bnv.shzxlz.cn

free -h;  ps aux | grep nginx
来源：http://ziv.bbcook.cn

[R64] 结束进程
来源：http://msv.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://bxc.yueranfly.top

[R65] 查看端口占用
来源：http://ils.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bsn.vehdjk.com

[R66] 定时任务
来源：http://wgj.ydjk.org.cn

crontab -e;  crontab -l
来源：http://uzt.cheryme.top

[R67] 生成随机十六进制串
来源：http://jta.xylfe.cn

openssl rand -hex 16
来源：http://nrg.fzhhl.top

[R68] 计算文件校验值
来源：http://dza.ydjk.org.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yfb.zhixingplan.top

[R69] 生成随机密码
来源：http://akp.gaohongyu789.top

head -c 16 /dev/urandom | base64
来源：http://fdc.xziqi.cn

[R70] 时间戳与互转
来源：http://xdp.daxiang520.top

date +%s;  date -d @1700000000
来源：http://egt.pycfn.com

[R71] 日期格式化
来源：http://gln.yfazqb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://zkv.jlsjyb.cn

[R72] 等待端口就绪
来源：http://aup.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://czv.fanxiaobao.xyz

[R73] 分割大日志
来源：http://cvk.zhongyouzk.top

split -l 1000 big.log part_
来源：http://knc.yongpay.top

[R74] 批量重命名
来源：http://prh.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ysb.gogol.net.cn

[R75] 导出环境变量
来源：http://bdk.zhixingplan.top

export PATH="$HOME/bin:$PATH"
来源：http://tzm.zycfv.cn

[R76] 使用临时文件
来源：http://cub.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://juu.ppjwa.cn

[R77] 读取用户输入
来源：http://cvr.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://zhg.dianchejie.cn

[R78] 交互式菜单
来源：http://hbd.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://zbv.zycfv.cn

[R79] 解析命令行选项
来源：http://jvl.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oxs.jianghu66.top

[R80] 查看脚本执行耗时
来源：http://kzv.redwolf501.top

time ./run.sh
来源：http://xmz.yanxiufei.cn

================================================================================
来源：http://aok.hywenlv.cn

S. C / C++ 专题
来源：http://pft.yj202588.top

================================================================================
来源：http://drb.fanxiaobao.xyz

[S01] C：Hello World
来源：http://ixs.52xcode.cn

#include <stdio.h>
来源：http://qlv.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ciu.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://nqo.havefunace.top

int a = 10; printf("%d\n", a);
来源：http://ovd.daria6918.cn

[S03] C：读入整数
来源：http://khf.hesvh.cn

int x; scanf("%d", &x);
来源：http://odi.hongshengwenyu.top

[S04] C：字符串复制
来源：http://cqm.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://chb.uphjek.com

[S05] C：字符串长度
来源：http://wiv.wangdashe.top

strlen(s)
来源：http://lxq.nwbrower.top

[S06] C：字符串比较
来源：http://jjz.zhongyouzk.top

strcmp(a, b) == 0
来源：http://fbv.ydzc1.top

[S07] C：数组遍历求和
来源：http://lpc.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://siz.fanxiaobao.xyz

[S08] C：动态内存分配与释放
来源：http://nhu.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ldk.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://joa.gotoacloud.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jxy.smart0.xyz

[S10] C：指针与解引用
来源：http://xul.tian-w.cn

int *p = &a;  *p = 5;
来源：http://zfb.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://uku.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://wbt.hesvh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dex.hnxiangtu.top

fclose(f);
来源：http://yok.chenzaomai.com

[S12] C：写文件
来源：http://pxe.52xcode.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dwk.shuidangran.top

[S13] C：宏定义
来源：http://yms.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://peg.hywenlv.cn

[S14] C：枚举
来源：http://yub.gzhubu.top

enum Color { RED, GREEN, BLUE };
来源：http://zha.snrcjt.cn

[S15] C：类型转换
来源：http://pkt.guannengcc.top

(double) a / b
来源：http://cfj.gogol.net.cn

[S16] C：位操作置位
来源：http://kvv.cashguo.top

x |= (1 << 3);
来源：http://qlf.ybcxt.top

[S17] C：安全拼接字符串
来源：http://jyc.ppjwa.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mmp.zhaomingkeji.xyz

[S18] C：命令行参数
来源：http://jof.fzhhl.top

int main(int argc, char **argv)
来源：http://fce.sxryk.cn

[S19] C：快速排序
来源：http://tcz.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://sjf.vqdsnc.cn

[S20] C：二分查找
来源：http://fuo.yj20258888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ygo.hcnkem.com

[S21] C：字符类别判断
来源：http://dvw.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vlw.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://rxe.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://cap.yuxming.cn

[S23] C：随机数
来源：http://ppo.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vxw.ctjpmb.com

[S24] C：获取本地时间
来源：http://rjr.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cab.fengsongda.top

[S25] C：内存拷贝
来源：http://mum.shuidangran.top

memcpy(dst, src, n);
来源：http://yfr.jiagoushi.top

[S26] C：内存清零
来源：http://esy.dianchejie.cn

memset(a, 0, sizeof a);
来源：http://vzh.316326.xyz

[S27] C：定义常量
来源：http://lih.yuanzhike.top

const double PI = 3.14159;
来源：http://gyc.nanxuanxn.top

[S28] C：静态变量
来源：http://qpx.vehdjk.com

static int counter = 0;
来源：http://dnk.shuidangran.top

[S29] C：变参函数
来源：http://mcj.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mng.fktsv.cn

[S30] C：头文件保护
来源：http://jbo.shanyushiyangtech.top

#ifndef X_H
来源：http://oiq.xziqi.cn

#define X_H
来源：http://onb.jyoumei.cn

#endif
来源：http://kqi.jiagoushi.top

[S31] C++：Hello World
来源：http://vjv.jlsjyb.cn

#include <iostream>
来源：http://xtf.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://crn.tarul.cn

[S32] C++：字符串
来源：http://hmi.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://meg.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://yrv.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yeb.cdnleiting.top

[S34] C++：遍历 vector
来源：http://ize.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://dmi.zhijiandao.cn

[S35] C++：map
来源：http://uwx.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wis.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://lnt.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nla.cheryme.top

[S37] C++：set
来源：http://atf.xuetiantiany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qky.tarul.cn

[S38] C++：排序
来源：http://gjl.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://xwx.fengsongda.top

[S39] C++：自定义比较器排序
来源：http://qae.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hma.nanxuanxn.top

[S40] C++：查找元素
来源：http://pua.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://awr.yj20258.top

[S41] C++：类与构造函数
来源：http://abr.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tso.cucudq.cn

[S42] C++：继承与虚函数
来源：http://nqj.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://nqi.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://spi.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://hhp.ctjpmb.com

[S44] C++：引用传参
来源：http://squ.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://gma.gzhubu.top

[S45] C++：lambda
来源：http://msz.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jdz.hammf.cn

[S46] C++：函数模板
来源：http://rif.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hjo.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://xgw.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ntp.cqqwz.cn

[S48] C++：逐行读文件
来源：http://gyq.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jrk.meibo888.top

while (std::getline(in, line)) { }
来源：http://mgx.hongshengwenyu.top

[S49] C++：写文件
来源：http://cil.ctjpmb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hiq.hfpthk.cn

[S50] C++：格式化数字
来源：http://hzy.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ktf.jinyuanbaomall.cn

[S51] C++：显式类型转换
来源：http://qcy.tianlin.xyz

static_cast<double>(a) / b
来源：http://kep.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://jeo.yj202588.top

int size() const noexcept { return n_; }
来源：http://zzw.gogol.net.cn

[S53] C++：移动语义
来源：http://apo.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://bhq.yj202588.top

[S54] C++：异常处理
来源：http://qij.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://civ.jinqigufen.top

[S55] C++：结构化绑定
来源：http://gql.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lbl.jyoumei.cn

[S56] C++：optional
来源：http://sxu.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tbf.hnxiangtu.top

[S57] C++：编译期常量
来源：http://tsd.jiagoushi.top

constexpr int N = 10;
来源：http://ejc.cucudq.cn

[S58] C++：命名空间
来源：http://wud.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://fnx.ppjwa.cn

[S59] C++：静态断言
来源：http://mvv.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bgs.zhixingplan.top

[S60] C++：遍历并删除元素
来源：http://fiv.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qqw.yonumen.top

================================================================================
来源：http://vfn.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uxd.hfpthk.cn

================================================================================
来源：http://kqn.havefunace.top

[T01] Kotlin：Hello World
来源：http://rac.316326.xyz

println("Hello")
来源：http://rlu.hnxiangtu.top

[T02] Kotlin：变量
来源：http://ujg.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dgc.jinqigufen.top

[T03] Kotlin：字符串模板
来源：http://yvz.cashguo.top

"值: $b"
来源：http://edm.gzhubu.top

[T04] Kotlin：空安全
来源：http://tmj.daria6918.cn

val n: String? = null;  n?.length
来源：http://kiy.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://ztb.zhongyouzk.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aqw.yongpay.top

[T06] Kotlin：集合映射
来源：http://xvm.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://egt.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://ven.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://ieu.yuanzhike.top

[T08] Kotlin：数据类
来源：http://qlh.xziqi.cn

data class User(val name: String, val age: Int)
来源：http://igy.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://dap.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://mwd.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://ybo.uphjek.com

fun greet(name: String = "World") = "Hi $name"
来源：http://yjb.haohaochexian.top

[T11] Kotlin：协程
来源：http://sxm.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mma.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://mdq.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://bxp.gzhubu.top

[T13] Kotlin：只读 Map
来源：http://geo.jiagoushi.top

val m = mapOf("a" to 1)
来源：http://rzu.0kj1m.cn

[T14] Kotlin：循环
来源：http://ydg.fktsv.cn

for (i in 1..10) println(i)
来源：http://tzm.ydjk.org.cn

[T15] Kotlin：接口
来源：http://xfn.yfazqb.com

interface Shape { fun area(): Double }
来源：http://ygt.haohaochexian.top

[T16] Swift：Hello World
来源：http://qep.gotoacloud.top

print("Hello")
来源：http://zdr.pycfn.com

[T17] Swift：变量与常量
来源：http://zyn.andypj.xyz

var a = 1;  let b = 2
来源：http://mhf.fehbvm.com

[T18] Swift：字符串插值
来源：http://qtl.jqgufenzy.top

"值: \(b)"
来源：http://ltw.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://bph.hcnkem.com

if let n = opt { print(n) }
来源：http://cts.epnwcf.com

[T20] Swift：数组操作
来源：http://iyc.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://akl.ehwqpu.com

[T21] Swift：遍历
来源：http://dru.zdqjudy.top

for x in a { print(x) }
来源：http://fiv.wangdashe.top

[T22] Swift：字典
来源：http://tzj.nanxuanxn.top

var d = ["a": 1];  d["b"] = 2
来源：http://pqw.jqgfzy.top

[T23] Swift：函数
来源：http://fyz.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ziz.shuidangran.top

[T24] Swift：闭包
来源：http://kzz.ywan-chungtsiang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ytg.gotoacloud.top

[T25] Swift：结构体
来源：http://boj.andypj.xyz

struct P { var x: Int }
来源：http://uma.zhengqikj.top

[T26] Swift：类与重写
来源：http://bcd.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://xdd.xuanzx.com

[T27] Swift：错误处理
来源：http://tcg.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://cqh.birdmap.top

[T28] Swift：枚举
来源：http://ckw.yuanzhike.top

enum Color { case red, green }
来源：http://oak.guowangkeji.top

[T29] Swift：guard 提前返回
来源：http://onh.sysykeji.top

guard let x = opt else { return }
来源：http://jpw.fanxiaobao.xyz

[T30] Swift：协议
来源：http://xkk.gaohongyu789.top

protocol Shape { func area() -> Double }
来源：http://zhl.jianghu66.top

[T31] Lua：Hello World
来源：http://vhp.bbcook.cn

print("Hello")
来源：http://cil.ppjwa.cn

[T32] Lua：局部变量
来源：http://ycz.nwbrower.top

local a = 1
来源：http://sef.haohaochexian.top

[T33] Lua：表（数组）
来源：http://uyi.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sly.zhoulong.xyz

[T34] Lua：遍历表
来源：http://qel.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vqu.nwbrower.top

[T35] Lua：字典表
来源：http://wep.cheryme.top

local d = { a = 1 };  d.b = 2
来源：http://ezk.guowangkeji.top

[T36] Lua：函数
来源：http://glu.hfpthk.cn

function add(a, b) return a + b end
来源：http://jjw.bjfxy.top

[T37] Lua：字符串拼接
来源：http://ohy.yj20258.top

"a" .. "b"
来源：http://mjz.zhongyouzk.top

[T38] Lua：条件
来源：http://ynw.hnqzz.top

if x > 0 then print("正") end
来源：http://alv.ywan-chungtsiang.top

[T39] Lua：模式匹配
来源：http://dps.zhongyouzk.top

string.find(s, "%d+")
来源：http://ald.jqgufenzy.top

[T40] Lua：元表
来源：http://emd.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://ial.dashuyun.cn

[T41] Perl：Hello World
来源：http://gng.xingfuxueyuan.xyz

print "Hello\n";
来源：http://hdh.xziqi.cn

[T42] Perl：变量类型
来源：http://sob.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tof.xziqi.cn

[T43] Perl：字符串插值
来源：http://smg.birdmap.top

"值: $a"
来源：http://qkx.xinyue.icu

[T44] Perl：条件
来源：http://fgi.ctjpmb.com

if ($a > 0) { print "正"; }
来源：http://krm.gaohongyu789.top

[T45] Perl：数组遍历
来源：http://bso.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://wxt.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://yzi.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jmy.andypj.xyz

[T47] Perl：正则捕获
来源：http://aws.tianlin.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://ius.chenlongwang.top

[T48] Perl：正则替换
来源：http://ury.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://bri.zhixingplan.top

[T49] Perl：函数
来源：http://aux.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://urg.zdqjudy.top

[T50] Perl：逐行读文件
来源：http://mon.birdmap.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nen.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://yno.tian-w.cn

[T51] Scala：Hello World
来源：http://vwg.svipenyu.cn

println("Hello")
来源：http://bdq.jinqigufen.top

[T52] Scala：变量
来源：http://iwm.zycfv.cn

val a = 1;  var b = 2
来源：http://fxp.yfazqb.com

[T53] Scala：字符串插值
来源：http://kbt.guannengcc.top

s"值: $b"
来源：http://qnr.yuanzhike.top

[T54] Scala：集合映射
来源：http://ckx.shuidangran.top

List(1, 2, 3).map(_ * 2)
来源：http://irj.0kj1m.cn

[T55] Scala：集合过滤
来源：http://acb.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://fxd.mhx1999.top

[T56] Scala：样例类
来源：http://tun.redwolf501.top

case class User(name: String, age: Int)
来源：http://xba.ppjwa.cn

[T57] Scala：模式匹配
来源：http://xlw.zhiwuduotai.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://amo.yangfankeji.com

[T58] Scala：函数定义
来源：http://ols.cdnleiting.top

def add(a: Int, b: Int): Int = a + b
来源：http://vly.yongpay.top

[T59] Scala：循环
来源：http://mum.gzhubu.top

for (i <- 1 to 10) println(i)
来源：http://jpq.redwolf501.top

[T60] Scala：折叠
来源：http://nel.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kcc.shanyushiyangkeji.top

================================================================================
来源：http://vwd.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bzq.birdmap.top

================================================================================
来源：http://tme.zhijiandao.cn


<!-- 参考信息 -->