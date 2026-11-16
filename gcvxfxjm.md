代发 wailian999

free -h;  ps aux | grep nginx
来源：http://ydf.zhengqikj.top

[R64] 结束进程
来源：http://iwx.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://zup.0kj1m.cn

[R65] 查看端口占用
来源：http://rwo.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://inb.ydjk.org.cn

[R66] 定时任务
来源：http://etm.yvedp.cn

crontab -e;  crontab -l
来源：http://hmp.yonumen.top

[R67] 生成随机十六进制串
来源：http://lmg.smart0.xyz

openssl rand -hex 16
来源：http://oek.shuidangran.top

[R68] 计算文件校验值
来源：http://dbx.yj202588.top

sha256sum a.txt;  md5sum a.txt
来源：http://qnk.jyoumei.cn

[R69] 生成随机密码
来源：http://vbt.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://klg.c1oappe.top

[R70] 时间戳与互转
来源：http://ysg.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://ozg.yanxiufei.cn

[R71] 日期格式化
来源：http://egd.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://you.hywenlv.cn

[R72] 等待端口就绪
来源：http://dkx.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mtb.yonumen.top

[R73] 分割大日志
来源：http://sdq.hywenlv.cn

split -l 1000 big.log part_
来源：http://dzp.daxiang520.top

[R74] 批量重命名
来源：http://bal.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xze.sjlbkw.cn

[R75] 导出环境变量
来源：http://oud.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://jif.fehbvm.com

[R76] 使用临时文件
来源：http://isi.zhongyouzk.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://clw.hfpthk.cn

[R77] 读取用户输入
来源：http://unf.c1oappe.top

read -rp "请输入: " ans
来源：http://aba.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://zrw.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zqi.gzhubu.top

[R79] 解析命令行选项
来源：http://zwb.snrcjt.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ztv.hammf.cn

[R80] 查看脚本执行耗时
来源：http://ehy.ywan-chungtsiang.top

time ./run.sh
来源：http://kgl.epnwcf.com

================================================================================
来源：http://xte.tianlin.xyz

S. C / C++ 专题
来源：http://vrv.hesvh.cn

================================================================================
来源：http://jzh.jinqigfzy.top

[S01] C：Hello World
来源：http://mxy.guowangkeji.top

#include <stdio.h>
来源：http://haq.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tdk.xuetiantiany.cn

[S02] C：变量与格式化输出
来源：http://ust.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://qqr.0kj1m.cn

[S03] C：读入整数
来源：http://wxs.ehwqpu.com

int x; scanf("%d", &x);
来源：http://djo.zdqjudy.top

[S04] C：字符串复制
来源：http://hwf.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://jds.cucudq.cn

[S05] C：字符串长度
来源：http://ssh.yanxiufei.cn

strlen(s)
来源：http://coy.c1oappe.top

[S06] C：字符串比较
来源：http://xcq.9152youxi.cn

strcmp(a, b) == 0
来源：http://izq.xuetiantiany.cn

[S07] C：数组遍历求和
来源：http://xhh.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fxk.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://gcs.wangshuangyany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tib.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://oir.shzxlz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xbw.hesvh.cn

[S10] C：指针与解引用
来源：http://mfk.svipenyu.cn

int *p = &a;  *p = 5;
来源：http://pgk.zycfv.cn

[S11] C：逐行读文件
来源：http://ruu.c1oappe.top

FILE *f = fopen("a.txt", "r");
来源：http://eaj.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fyd.316326.xyz

fclose(f);
来源：http://mcx.chenzaomai.com

[S12] C：写文件
来源：http://cic.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://upl.9152youxi.cn

[S13] C：宏定义
来源：http://srt.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mmo.cucudq.cn

[S14] C：枚举
来源：http://mgr.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://iyw.bbcook.cn

[S15] C：类型转换
来源：http://kub.jinyuanbaomall.cn

(double) a / b
来源：http://nxs.epnwcf.com

[S16] C：位操作置位
来源：http://qim.jinqigfzy.top

x |= (1 << 3);
来源：http://kck.daria6918.cn

[S17] C：安全拼接字符串
来源：http://fza.jinqigfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cfk.wangshuangyany.cn

[S18] C：命令行参数
来源：http://btu.bjfxy.top

int main(int argc, char **argv)
来源：http://vay.zhiwuduotai.top

[S19] C：快速排序
来源：http://nlm.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://wqt.hesvh.cn

[S20] C：二分查找
来源：http://iem.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sqg.hfpthk.cn

[S21] C：字符类别判断
来源：http://fio.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cxt.hesvh.cn

[S22] C：字符串转数字
来源：http://elj.wangshuangyany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://klz.yvedp.cn

[S23] C：随机数
来源：http://lhe.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mfx.jinqigufen.top

[S24] C：获取本地时间
来源：http://tmi.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://enn.xuanzx.com

[S25] C：内存拷贝
来源：http://zvx.jinqigfzy.top

memcpy(dst, src, n);
来源：http://grr.wangdashe.top

[S26] C：内存清零
来源：http://fld.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://cjj.fanxiaobao.xyz

[S27] C：定义常量
来源：http://mmv.cashguo.top

const double PI = 3.14159;
来源：http://jzn.vqdsnc.cn

[S28] C：静态变量
来源：http://tck.shanyushiyangtech.top

static int counter = 0;
来源：http://bpn.fzhhl.top

[S29] C：变参函数
来源：http://gnb.hongshengwenyu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xni.chenjidiqi.icu

[S30] C：头文件保护
来源：http://sbh.ppjwa.cn

#ifndef X_H
来源：http://oqw.ydzc1.top

#define X_H
来源：http://qll.yj20258.top

#endif
来源：http://dom.yanxiufei.cn

[S31] C++：Hello World
来源：http://opk.vehdjk.com

#include <iostream>
来源：http://ewn.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://vca.guowangkeji.top

[S32] C++：字符串
来源：http://txl.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://yjz.hfpthk.cn

[S33] C++：vector 增删
来源：http://wwx.svipenyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zly.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://piz.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://sso.ydjk.org.cn

[S35] C++：map
来源：http://fhm.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lbq.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://kux.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hkc.hfpthk.cn

[S37] C++：set
来源：http://ywa.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ejj.cdnleiting.top

[S38] C++：排序
来源：http://icz.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://sop.meibo888.top

[S39] C++：自定义比较器排序
来源：http://uvv.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kfo.hesvh.cn

[S40] C++：查找元素
来源：http://lzp.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qls.0kj1m.cn

[S41] C++：类与构造函数
来源：http://dcj.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qjx.xylfe.cn

[S42] C++：继承与虚函数
来源：http://xqw.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://shz.c1oappe.top

[S43] C++：智能指针
来源：http://vki.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://adc.aizwys.cn

[S44] C++：引用传参
来源：http://ubs.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://opm.chenlongwang.top

[S45] C++：lambda
来源：http://zls.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://xnk.zdqjudy.top

[S46] C++：函数模板
来源：http://nsh.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jpd.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://kzt.yangfankeji.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gdu.jiagoushi.top

[S48] C++：逐行读文件
来源：http://rnv.dashuyun.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gzd.aibaodan.cn

while (std::getline(in, line)) { }
来源：http://tbs.kuanghao11.cn

[S49] C++：写文件
来源：http://kmc.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dqx.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://otn.smart0.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://czf.yangfankeji.com

[S51] C++：显式类型转换
来源：http://ixr.52xcode.cn

static_cast<double>(a) / b
来源：http://gne.tanke756.top

[S52] C++：const 与 noexcept
来源：http://nnu.cashguo.top

int size() const noexcept { return n_; }
来源：http://apa.jinqigfzy.top

[S53] C++：移动语义
来源：http://zpl.tarul.cn

std::vector<int> w = std::move(v);
来源：http://wzu.jlsjyb.cn

[S54] C++：异常处理
来源：http://yqx.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rzq.jianghu66.top

[S55] C++：结构化绑定
来源：http://eqh.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dbg.cucudq.cn

[S56] C++：optional
来源：http://dkn.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cqq.0kj1m.cn

[S57] C++：编译期常量
来源：http://oft.52xcode.cn

constexpr int N = 10;
来源：http://kkz.cheryme.top

[S58] C++：命名空间
来源：http://esa.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://rox.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://dgc.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dqg.jyoumei.cn

[S60] C++：遍历并删除元素
来源：http://bci.fzhhl.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qyg.svipenyu.cn

================================================================================
来源：http://deb.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tvk.snrcjt.cn

================================================================================
来源：http://rmo.shanyushiyangtech.top

[T01] Kotlin：Hello World
来源：http://oiz.havefunace.top

println("Hello")
来源：http://jwu.hongshengwenyu.top

[T02] Kotlin：变量
来源：http://zky.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kyw.shanyushiyangkeji.top

[T03] Kotlin：字符串模板
来源：http://dsw.fktsv.cn

"值: $b"
来源：http://qtd.ctjpmb.com

[T04] Kotlin：空安全
来源：http://pey.xziqi.cn

val n: String? = null;  n?.length
来源：http://yip.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://mgl.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://woz.tanke756.top

[T06] Kotlin：集合映射
来源：http://use.hywenlv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ejk.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://rdy.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rcu.haohaochexian.top

[T08] Kotlin：数据类
来源：http://rlq.cheryme.top

data class User(val name: String, val age: Int)
来源：http://tqo.zhengqikj.top

[T09] Kotlin：扩展函数
来源：http://ajp.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://gwo.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://eel.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://swu.yuanzhike.top

[T11] Kotlin：协程
来源：http://tjp.quarkkingdee.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://esh.svipenyu.cn

[T12] Kotlin：解构声明
来源：http://clh.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://umf.svipenyu.cn

[T13] Kotlin：只读 Map
来源：http://cry.52xcode.cn

val m = mapOf("a" to 1)
来源：http://lia.tianlin.xyz

[T14] Kotlin：循环
来源：http://eya.jinqigfzy.top

for (i in 1..10) println(i)
来源：http://xei.tanke756.top

[T15] Kotlin：接口
来源：http://zdh.xuanzx.com

interface Shape { fun area(): Double }
来源：http://jmt.shuidangran.top

[T16] Swift：Hello World
来源：http://fdk.vehdjk.com

print("Hello")
来源：http://czl.smart0.xyz

[T17] Swift：变量与常量
来源：http://okk.hesvh.cn

var a = 1;  let b = 2
来源：http://tdv.xinyue.icu

[T18] Swift：字符串插值
来源：http://bqi.dianchejie.cn

"值: \(b)"
来源：http://wli.yj202588.top

[T19] Swift：可选绑定
来源：http://nvs.birdmap.top

if let n = opt { print(n) }
来源：http://lsq.c1oappe.top

[T20] Swift：数组操作
来源：http://dxo.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://kfa.shuidangran.top

[T21] Swift：遍历
来源：http://puf.nanxuanxn.top

for x in a { print(x) }
来源：http://aqu.chenzaomai.com

[T22] Swift：字典
来源：http://zsn.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fhy.jianghu66.top

[T23] Swift：函数
来源：http://ulg.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rbi.tanke756.top

[T24] Swift：闭包
来源：http://jnt.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yjm.yongpay.top

[T25] Swift：结构体
来源：http://tud.hfpthk.cn

struct P { var x: Int }
来源：http://xhe.quarkkingdee.top

[T26] Swift：类与重写
来源：http://ukh.ctjpmb.com

class A: Base { override func f() {} }
来源：http://ytf.cdnleiting.top

[T27] Swift：错误处理
来源：http://ouz.bjfxy.top

do { try f() } catch { print(error) }
来源：http://dqj.hfpthk.cn

[T28] Swift：枚举
来源：http://diq.yonumen.top

enum Color { case red, green }
来源：http://neu.yueranfly.top

[T29] Swift：guard 提前返回
来源：http://dsy.ydjk.org.cn

guard let x = opt else { return }
来源：http://wlq.sweek.top

[T30] Swift：协议
来源：http://uue.shanyushiyangtech.top

protocol Shape { func area() -> Double }
来源：http://xpq.ehwqpu.com

[T31] Lua：Hello World
来源：http://oke.cucudq.cn

print("Hello")
来源：http://dtz.hnxiangtu.top

[T32] Lua：局部变量
来源：http://xrn.wangdashe.top

local a = 1
来源：http://muk.zhengqikj.top

[T33] Lua：表（数组）
来源：http://fno.nanxuanxn.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ijs.dianchejie.cn

[T34] Lua：遍历表
来源：http://tjr.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lvy.c1oappe.top

[T35] Lua：字典表
来源：http://pbs.xuanzx.com

local d = { a = 1 };  d.b = 2
来源：http://dkt.guowangkeji.top

[T36] Lua：函数
来源：http://evl.wangdashe.top

function add(a, b) return a + b end
来源：http://jgl.shanyushiyangkeji.top

[T37] Lua：字符串拼接
来源：http://tab.cdnleiting.top

"a" .. "b"
来源：http://nco.nanxinkj.top

[T38] Lua：条件
来源：http://aqb.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://kxo.xylfe.cn

[T39] Lua：模式匹配
来源：http://mof.52xcode.cn

string.find(s, "%d+")
来源：http://jrz.zhixingplan.top

[T40] Lua：元表
来源：http://bdv.yongpay.top

setmetatable({}, { __index = base })
来源：http://muq.chenjidiqi.icu

[T41] Perl：Hello World
来源：http://qji.gotoacloud.top

print "Hello\n";
来源：http://rew.hammf.cn

[T42] Perl：变量类型
来源：http://rsb.jianghu66.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ktq.jiagoushi.top

[T43] Perl：字符串插值
来源：http://udo.hywenlv.cn

"值: $a"
来源：http://vvl.52xcode.cn

[T44] Perl：条件
来源：http://pru.pengpengdd.cyou

if ($a > 0) { print "正"; }
来源：http://moq.sufxvd.cn

[T45] Perl：数组遍历
来源：http://vwg.jinqigufen.top

for my $x (@arr) { print $x; }
来源：http://ofw.zhiwuduotai.top

[T46] Perl：哈希操作
来源：http://wjn.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jfm.hcnkem.com

[T47] Perl：正则捕获
来源：http://xkp.zdqjudy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://czp.andypj.xyz

[T48] Perl：正则替换
来源：http://tyb.fanxiaobao.xyz

$s =~ s/old/new/g;
来源：http://ijy.jinqigufen.top

[T49] Perl：函数
来源：http://elp.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pkv.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://mwc.hnqzz.top

open my $fh, "<", "a.txt" or die $!;
来源：http://buz.tarul.cn

while (my $line = <$fh>) { print $line; }
来源：http://bsr.gaohongyu789.top

[T51] Scala：Hello World
来源：http://rcm.dashuyun.cn

println("Hello")
来源：http://qlp.sxryk.cn

[T52] Scala：变量
来源：http://iqm.dianchejie.cn

val a = 1;  var b = 2
来源：http://dzs.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://tqj.hcnkem.com

s"值: $b"
来源：http://llv.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://qku.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://jou.hammf.cn

[T55] Scala：集合过滤
来源：http://xic.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pqa.ydjk.org.cn

[T56] Scala：样例类
来源：http://auv.yj20258.top

case class User(name: String, age: Int)
来源：http://spb.chenzaomai.com

[T57] Scala：模式匹配
来源：http://gbe.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://zfc.9152youxi.cn

[T58] Scala：函数定义
来源：http://bas.ydjk.org.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dwd.cucudq.cn

[T59] Scala：循环
来源：http://hjv.yuanzhike.top

for (i <- 1 to 10) println(i)
来源：http://ksv.daxiang520.top

[T60] Scala：折叠
来源：http://mui.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jrn.svipenyu.cn

================================================================================
来源：http://qah.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hgn.ivvv.top

================================================================================
来源：http://bvd.sweek.top

[U01] Py：创建虚拟环境
来源：http://jqa.jinghuilouyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://avc.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://lxv.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wmk.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://xyi.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qkh.epnwcf.com

[U04] Py：变量调试打印
来源：http://qvt.jlsjyb.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rcr.52xcode.cn


<!-- 参考信息 -->