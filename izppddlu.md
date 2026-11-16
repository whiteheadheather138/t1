代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://idp.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://hxb.shanyushiyangtech.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pbh.fktsv.cn

[R61] 磁盘占用
来源：http://tag.shangyingyoupin.top

df -h;  du -sh *
来源：http://hih.snrcjt.cn

[R62] 找最占空间的文件
来源：http://kwe.yuanzhike.top

du -ah . | sort -rh | head -10
来源：http://oyu.316326.xyz

[R63] 内存与进程
来源：http://oea.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://ojt.cdnleiting.top

[R64] 结束进程
来源：http://anh.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://bqm.smart0.xyz

[R65] 查看端口占用
来源：http://mzg.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gkr.yongpay.top

[R66] 定时任务
来源：http://vot.zdqjudy.top

crontab -e;  crontab -l
来源：http://tfr.zycfv.cn

[R67] 生成随机十六进制串
来源：http://cnt.chenzaomai.com

openssl rand -hex 16
来源：http://roo.quarkkingdee.top

[R68] 计算文件校验值
来源：http://kzl.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lsk.meibo888.top

[R69] 生成随机密码
来源：http://xel.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://cbc.fengsongda.top

[R70] 时间戳与互转
来源：http://rbm.svipenyu.cn

date +%s;  date -d @1700000000
来源：http://udw.zhijiandao.cn

[R71] 日期格式化
来源：http://gqi.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gmf.meibo888.top

[R72] 等待端口就绪
来源：http://xof.cheryme.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ydl.316326.xyz

[R73] 分割大日志
来源：http://xdf.yonumen.top

split -l 1000 big.log part_
来源：http://gzz.vqdsnc.cn

[R74] 批量重命名
来源：http://dku.yfazqb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://guh.hcnkem.com

[R75] 导出环境变量
来源：http://eix.shuidangran.top

export PATH="$HOME/bin:$PATH"
来源：http://dse.haohaochexian.top

[R76] 使用临时文件
来源：http://xjd.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qpr.nwbrower.top

[R77] 读取用户输入
来源：http://mom.pycfn.com

read -rp "请输入: " ans
来源：http://wcy.sysykeji.top

[R78] 交互式菜单
来源：http://szu.wangshuangyany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kmu.shuidangran.top

[R79] 解析命令行选项
来源：http://uez.c1oappe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eak.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://kmq.dianchejie.cn

time ./run.sh
来源：http://ngn.yonumen.top

================================================================================
来源：http://oke.epnwcf.com

S. C / C++ 专题
来源：http://zzq.ctjpmb.com

================================================================================
来源：http://inh.ydjk.org.cn

[S01] C：Hello World
来源：http://kbb.xziqi.cn

#include <stdio.h>
来源：http://esd.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xps.yuxming.cn

[S02] C：变量与格式化输出
来源：http://bwq.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://odc.9152youxi.cn

[S03] C：读入整数
来源：http://otx.shuidangran.top

int x; scanf("%d", &x);
来源：http://uvr.zhoulong.xyz

[S04] C：字符串复制
来源：http://cot.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://kzy.zhengqikj.top

[S05] C：字符串长度
来源：http://mdi.meibo888.top

strlen(s)
来源：http://lpd.hammf.cn

[S06] C：字符串比较
来源：http://tqp.jyoumei.cn

strcmp(a, b) == 0
来源：http://qft.iojbl.cn

[S07] C：数组遍历求和
来源：http://zrz.shanyushiyangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fgp.yvedp.cn

[S08] C：动态内存分配与释放
来源：http://dxs.jqgfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nsx.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://onc.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bmi.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://ikt.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://wbt.birdmap.top

[S11] C：逐行读文件
来源：http://peq.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "r");
来源：http://xqf.zhongyouzk.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zel.tian-w.cn

fclose(f);
来源：http://pfx.fengsongda.top

[S12] C：写文件
来源：http://clv.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ftj.shzxlz.cn

[S13] C：宏定义
来源：http://ldr.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fuy.guannengcc.top

[S14] C：枚举
来源：http://bfj.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://syp.jinqigfzy.top

[S15] C：类型转换
来源：http://jrr.hammf.cn

(double) a / b
来源：http://uhc.hammf.cn

[S16] C：位操作置位
来源：http://avl.gaohongyu789.top

x |= (1 << 3);
来源：http://ouh.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://qij.hysaishi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pnk.dashuyun.cn

[S18] C：命令行参数
来源：http://vxy.ppjwa.cn

int main(int argc, char **argv)
来源：http://wnc.9152youxi.cn

[S19] C：快速排序
来源：http://vss.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://aiq.jqgufenzy.top

[S20] C：二分查找
来源：http://nyc.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rxs.jinqigufen.top

[S21] C：字符类别判断
来源：http://nbv.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uyy.zdqjudy.top

[S22] C：字符串转数字
来源：http://ggo.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://syu.ybcxt.top

[S23] C：随机数
来源：http://xus.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vjk.0kj1m.cn

[S24] C：获取本地时间
来源：http://kmm.c1oappe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lui.cdnleiting.top

[S25] C：内存拷贝
来源：http://xuv.fengsongda.top

memcpy(dst, src, n);
来源：http://usc.pengpengdd.cyou

[S26] C：内存清零
来源：http://bbi.shanyushiyangkeji.top

memset(a, 0, sizeof a);
来源：http://rki.yongpay.top

[S27] C：定义常量
来源：http://tmi.dianchejie.cn

const double PI = 3.14159;
来源：http://lsb.dianchejie.cn

[S28] C：静态变量
来源：http://nat.sxryk.cn

static int counter = 0;
来源：http://avp.yueranfly.top

[S29] C：变参函数
来源：http://bcj.aibaodan.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fqf.chenjidiqi.icu

[S30] C：头文件保护
来源：http://hau.hnxiangtu.top

#ifndef X_H
来源：http://mdj.zhaomingkeji.xyz

#define X_H
来源：http://xcx.xylfe.cn

#endif
来源：http://tds.316326.xyz

[S31] C++：Hello World
来源：http://byl.cheryme.top

#include <iostream>
来源：http://gmh.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://qnn.pengpengdd.cyou

[S32] C++：字符串
来源：http://xjk.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://hmg.birdmap.top

[S33] C++：vector 增删
来源：http://nzd.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mfs.xziqi.cn

[S34] C++：遍历 vector
来源：http://wrl.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://hoq.xylfe.cn

[S35] C++：map
来源：http://ncf.shangyingyoupin.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wvt.haohaochexian.top

[S36] C++：unordered_map
来源：http://sds.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zst.feifeiyinyue.top

[S37] C++：set
来源：http://bsq.smart0.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kgg.jianghu66.top

[S38] C++：排序
来源：http://qfs.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://dyd.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://wsg.pycfn.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fdm.bbcook.cn

[S40] C++：查找元素
来源：http://lyd.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wjr.jinqigfzy.top

[S41] C++：类与构造函数
来源：http://tgs.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ywv.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://cjf.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://ajd.epnwcf.com

[S43] C++：智能指针
来源：http://gry.hesvh.cn

auto p = std::make_unique<int>(5);
来源：http://ior.jiagoushi.top

[S44] C++：引用传参
来源：http://wys.bjfxy.top

void inc(int &x) { ++x; }
来源：http://whi.dashuyun.cn

[S45] C++：lambda
来源：http://apa.cdnleiting.top

auto add = [](int a, int b) { return a + b; };
来源：http://hnt.feifeiyinyue.top

[S46] C++：函数模板
来源：http://ncc.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://txl.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://ewk.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lxe.fehbvm.com

[S48] C++：逐行读文件
来源：http://sgh.hnqzz.top

std::ifstream in("a.txt");  std::string line;
来源：http://dhb.dashuyun.cn

while (std::getline(in, line)) { }
来源：http://zbq.xylfe.cn

[S49] C++：写文件
来源：http://lkg.gotoacloud.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kqv.yueranfly.top

[S50] C++：格式化数字
来源：http://hkk.hcnkem.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jyy.yuanzhike.top

[S51] C++：显式类型转换
来源：http://mrp.havefunace.top

static_cast<double>(a) / b
来源：http://szs.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://awc.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://toa.jianghu66.top

[S53] C++：移动语义
来源：http://xrp.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://ivg.ehwqpu.com

[S54] C++：异常处理
来源：http://zco.uphjek.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://evd.sweek.top

[S55] C++：结构化绑定
来源：http://apu.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kiv.andypj.xyz

[S56] C++：optional
来源：http://ocj.yj20258888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nak.316326.xyz

[S57] C++：编译期常量
来源：http://cie.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://abv.ywan-chungtsiang.top

[S58] C++：命名空间
来源：http://lmb.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://oql.cashguo.top

[S59] C++：静态断言
来源：http://mgs.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tki.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://npz.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hci.sysykeji.top

================================================================================
来源：http://ovh.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://api.ydjk.org.cn

================================================================================
来源：http://vww.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://mrj.zycfv.cn

println("Hello")
来源：http://znb.zhongyouzk.top

[T02] Kotlin：变量
来源：http://ybl.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xqg.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://czw.ppjwa.cn

"值: $b"
来源：http://yzw.xingfuxueyuan.xyz

[T04] Kotlin：空安全
来源：http://pod.hesvh.cn

val n: String? = null;  n?.length
来源：http://fxo.shanyushiyangtech.top

[T05] Kotlin：when 表达式
来源：http://dul.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://atr.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://ycr.52xcode.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jss.uphjek.com

[T07] Kotlin：集合过滤
来源：http://rcg.jqgufenzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lwi.hywenlv.cn

[T08] Kotlin：数据类
来源：http://pbr.wangdashe.top

data class User(val name: String, val age: Int)
来源：http://lpu.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://lsq.yongpay.top

fun String.exclaim() = this + "!"
来源：http://voz.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://rew.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fza.fktsv.cn

[T11] Kotlin：协程
来源：http://abe.yuanzhike.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fdu.shzxlz.cn

[T12] Kotlin：解构声明
来源：http://esf.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://hsn.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://xkj.gogol.net.cn

val m = mapOf("a" to 1)
来源：http://pgw.ybcxt.top

[T14] Kotlin：循环
来源：http://gir.daxiang520.top

for (i in 1..10) println(i)
来源：http://hqz.yuxming.cn

[T15] Kotlin：接口
来源：http://xpj.tanke756.top

interface Shape { fun area(): Double }
来源：http://ukx.shanyushiyangtech.top

[T16] Swift：Hello World
来源：http://hwe.shuidangran.top

print("Hello")
来源：http://bqz.ywan-chungtsiang.top

[T17] Swift：变量与常量
来源：http://hnr.sxryk.cn

var a = 1;  let b = 2
来源：http://tof.ydjk.org.cn

[T18] Swift：字符串插值
来源：http://lqp.yj20258888.top

"值: \(b)"
来源：http://tiw.cqqwz.cn

[T19] Swift：可选绑定
来源：http://ate.ydjk.org.cn

if let n = opt { print(n) }
来源：http://syu.xuanzx.com

[T20] Swift：数组操作
来源：http://wab.aizwys.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yvj.ivvv.top

[T21] Swift：遍历
来源：http://lku.ivvv.top

for x in a { print(x) }
来源：http://cec.chenlongwang.top

[T22] Swift：字典
来源：http://tbb.yanxiufei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tse.zycfv.cn

[T23] Swift：函数
来源：http://yzy.birdmap.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gvg.birdmap.top

[T24] Swift：闭包
来源：http://wrl.yuanzhike.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ymd.yongpay.top

[T25] Swift：结构体
来源：http://ves.cqqwz.cn

struct P { var x: Int }
来源：http://bcq.fehbvm.com

[T26] Swift：类与重写
来源：http://apx.hywenlv.cn

class A: Base { override func f() {} }
来源：http://avc.hesvh.cn

[T27] Swift：错误处理
来源：http://zdf.pycfn.com

do { try f() } catch { print(error) }
来源：http://rit.dashuyun.cn

[T28] Swift：枚举
来源：http://cbl.jianghu66.top

enum Color { case red, green }
来源：http://ljz.yongpay.top

[T29] Swift：guard 提前返回
来源：http://szo.aibaodan.cn

guard let x = opt else { return }
来源：http://rrm.bbcook.cn

[T30] Swift：协议
来源：http://zqd.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://afi.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://skm.cheryme.top

print("Hello")
来源：http://aos.jqgufenzy.top

[T32] Lua：局部变量
来源：http://mbx.zdbjq.cn

local a = 1
来源：http://bxl.svipenyu.cn

[T33] Lua：表（数组）
来源：http://mqg.yj20258.top

local t = {1, 2, 3};  t[4] = 4
来源：http://moh.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://tlz.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://atc.tarul.cn

[T35] Lua：字典表
来源：http://smf.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://zwh.hnqzz.top

[T36] Lua：函数
来源：http://fmx.cucudq.cn

function add(a, b) return a + b end
来源：http://vcb.pengpengdd.cyou

[T37] Lua：字符串拼接
来源：http://ojk.gaohongyu789.top

"a" .. "b"
来源：http://otx.sxryk.cn

[T38] Lua：条件
来源：http://hcz.hammf.cn

if x > 0 then print("正") end
来源：http://jhl.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://pnc.hammf.cn

string.find(s, "%d+")
来源：http://fod.xinyue.icu

[T40] Lua：元表
来源：http://fja.uphjek.com

setmetatable({}, { __index = base })
来源：http://zof.hongshengwenyu.top

[T41] Perl：Hello World
来源：http://gtl.ivvv.top

print "Hello\n";
来源：http://azd.hfpthk.cn

[T42] Perl：变量类型
来源：http://yly.ivvv.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://het.hysaishi.cn

[T43] Perl：字符串插值
来源：http://mvp.havefunace.top

"值: $a"
来源：http://asy.jinghuilouyu.cn

[T44] Perl：条件
来源：http://wcv.yj20258.top

if ($a > 0) { print "正"; }
来源：http://tyn.316326.xyz

[T45] Perl：数组遍历
来源：http://erw.yfazqb.com

for my $x (@arr) { print $x; }
来源：http://uba.yanxiufei.cn

[T46] Perl：哈希操作
来源：http://bmz.uphjek.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xme.zdqjudy.top

[T47] Perl：正则捕获
来源：http://wxb.tian-w.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sqg.fehbvm.com

[T48] Perl：正则替换
来源：http://yru.guowangkeji.top

$s =~ s/old/new/g;
来源：http://qee.0kj1m.cn

[T49] Perl：函数
来源：http://kcv.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jbs.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://jsl.pycfn.com

open my $fh, "<", "a.txt" or die $!;
来源：http://iks.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://toe.zdbjq.cn

[T51] Scala：Hello World
来源：http://sht.pengpengdd.cyou

println("Hello")
来源：http://zom.ehwqpu.com

[T52] Scala：变量
来源：http://omo.fzhhl.top

val a = 1;  var b = 2
来源：http://aal.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://wcl.yj20258.top

s"值: $b"
来源：http://jwq.jianghu66.top

[T54] Scala：集合映射
来源：http://xth.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://str.316326.xyz

[T55] Scala：集合过滤
来源：http://viz.fktsv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ugm.cdnleiting.top

[T56] Scala：样例类
来源：http://nlf.yongpay.top

case class User(name: String, age: Int)
来源：http://giy.jiagoushi.top

[T57] Scala：模式匹配
来源：http://kgp.xingfuxueyuan.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://olt.uphjek.com

[T58] Scala：函数定义
来源：http://mho.redwolf501.top

def add(a: Int, b: Int): Int = a + b
来源：http://gdg.gotoacloud.top

[T59] Scala：循环
来源：http://dvz.ydjk.org.cn

for (i <- 1 to 10) println(i)
来源：http://ndd.xziqi.cn

[T60] Scala：折叠
来源：http://cip.xingfuxueyuan.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fcw.yangfankeji.com

================================================================================
来源：http://ixg.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rnk.yanxiufei.cn

================================================================================
来源：http://nev.c1oappe.top


<!-- 参考信息 -->