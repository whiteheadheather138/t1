代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vax.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://aqm.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fjf.hysaishi.cn

[R61] 磁盘占用
来源：http://syd.chenjidiqi.icu

df -h;  du -sh *
来源：http://dvt.tianlin.xyz

[R62] 找最占空间的文件
来源：http://rxl.tarul.cn

du -ah . | sort -rh | head -10
来源：http://zqc.jinghuilouyu.cn

[R63] 内存与进程
来源：http://bat.sweek.top

free -h;  ps aux | grep nginx
来源：http://bfj.sufxvd.cn

[R64] 结束进程
来源：http://tyo.yongpay.top

kill -9 $(pgrep -f app.py)
来源：http://dxc.nwbrower.top

[R65] 查看端口占用
来源：http://tyj.cashguo.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nzz.yj20258.top

[R66] 定时任务
来源：http://kwm.tarul.cn

crontab -e;  crontab -l
来源：http://twt.fengsongda.top

[R67] 生成随机十六进制串
来源：http://mjg.vehdjk.com

openssl rand -hex 16
来源：http://xku.hcnkem.com

[R68] 计算文件校验值
来源：http://hgt.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hlf.nwbrower.top

[R69] 生成随机密码
来源：http://tkl.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://wlg.52xcode.cn

[R70] 时间戳与互转
来源：http://ytr.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://uib.gogol.net.cn

[R71] 日期格式化
来源：http://ezk.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://byf.sjlbkw.cn

[R72] 等待端口就绪
来源：http://yad.jqgufenzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dqp.nanxinkj.top

[R73] 分割大日志
来源：http://dei.yvedp.cn

split -l 1000 big.log part_
来源：http://ihk.zhengqikj.top

[R74] 批量重命名
来源：http://zdu.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mki.yonumen.top

[R75] 导出环境变量
来源：http://dah.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://lwj.hesvh.cn

[R76] 使用临时文件
来源：http://jix.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cuc.andypj.xyz

[R77] 读取用户输入
来源：http://sec.xziqi.cn

read -rp "请输入: " ans
来源：http://lfj.daxiang520.top

[R78] 交互式菜单
来源：http://pce.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rdq.jqgufenzy.top

[R79] 解析命令行选项
来源：http://acf.cheryme.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://slg.yj202588.top

[R80] 查看脚本执行耗时
来源：http://ibu.sufxvd.cn

time ./run.sh
来源：http://vvq.tanke756.top

================================================================================
来源：http://znc.yuxming.cn

S. C / C++ 专题
来源：http://gbb.yanxiufei.cn

================================================================================
来源：http://hyc.fktsv.cn

[S01] C：Hello World
来源：http://acs.ppjwa.cn

#include <stdio.h>
来源：http://gcx.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rjd.pengpengdd.cyou

[S02] C：变量与格式化输出
来源：http://hrh.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://ayd.shangyingyoupin.top

[S03] C：读入整数
来源：http://bzt.shzxlz.cn

int x; scanf("%d", &x);
来源：http://krf.zycfv.cn

[S04] C：字符串复制
来源：http://wtq.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iog.hywenlv.cn

[S05] C：字符串长度
来源：http://rer.epnwcf.com

strlen(s)
来源：http://xob.52xcode.cn

[S06] C：字符串比较
来源：http://yjk.zhoulong.xyz

strcmp(a, b) == 0
来源：http://jcz.jinqigufen.top

[S07] C：数组遍历求和
来源：http://voh.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kss.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://gjc.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hvf.xinyue.icu

[S09] C：结构体定义与初始化
来源：http://ret.guannengcc.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pmc.gogol.net.cn

[S10] C：指针与解引用
来源：http://uie.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://gnz.jinqigfzy.top

[S11] C：逐行读文件
来源：http://hlp.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://ynp.jqgufenzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dyd.hfpthk.cn

fclose(f);
来源：http://tnk.zhijiandao.cn

[S12] C：写文件
来源：http://cwx.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gty.vqdsnc.cn

[S13] C：宏定义
来源：http://qca.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ftr.jlsjyb.cn

[S14] C：枚举
来源：http://ejc.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://igp.0kj1m.cn

[S15] C：类型转换
来源：http://lmi.nanxuanxn.top

(double) a / b
来源：http://nva.sjlbkw.cn

[S16] C：位操作置位
来源：http://ugz.gzhubu.top

x |= (1 << 3);
来源：http://psu.vqdsnc.cn

[S17] C：安全拼接字符串
来源：http://zhe.jqgfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://knz.iojbl.cn

[S18] C：命令行参数
来源：http://bjh.zhixingplan.top

int main(int argc, char **argv)
来源：http://ifo.cashguo.top

[S19] C：快速排序
来源：http://ayf.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://sgx.cdnleiting.top

[S20] C：二分查找
来源：http://mjf.jinyuanbaomall.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nua.316326.xyz

[S21] C：字符类别判断
来源：http://avx.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ghv.hnxiangtu.top

[S22] C：字符串转数字
来源：http://hfj.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jcz.9152youxi.cn

[S23] C：随机数
来源：http://fwj.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sjs.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://yrh.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eqj.zdqjudy.top

[S25] C：内存拷贝
来源：http://dzy.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://qun.ehwqpu.com

[S26] C：内存清零
来源：http://vza.chenzaomai.com

memset(a, 0, sizeof a);
来源：http://owz.tian-w.cn

[S27] C：定义常量
来源：http://acx.zhixingplan.top

const double PI = 3.14159;
来源：http://spi.zhijiandao.cn

[S28] C：静态变量
来源：http://vof.chenjidiqi.icu

static int counter = 0;
来源：http://eas.yj20258888.top

[S29] C：变参函数
来源：http://wfe.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://llx.hnxiangtu.top

[S30] C：头文件保护
来源：http://csx.snrcjt.cn

#ifndef X_H
来源：http://laa.jqgfzy.top

#define X_H
来源：http://ehn.hongshengwenyu.top

#endif
来源：http://vzh.yj20258.top

[S31] C++：Hello World
来源：http://beo.ydjk.org.cn

#include <iostream>
来源：http://qol.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://boa.hesvh.cn

[S32] C++：字符串
来源：http://shd.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://kyx.xinyue.icu

[S33] C++：vector 增删
来源：http://obk.pengpengdd.cyou

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hek.cheryme.top

[S34] C++：遍历 vector
来源：http://eja.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://qgq.fktsv.cn

[S35] C++：map
来源：http://urk.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jgh.guannengcc.top

[S36] C++：unordered_map
来源：http://fns.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://naw.dianchejie.cn

[S37] C++：set
来源：http://tlq.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dcn.vehdjk.com

[S38] C++：排序
来源：http://bkn.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://ouj.yongpay.top

[S39] C++：自定义比较器排序
来源：http://mow.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aiw.meibo888.top

[S40] C++：查找元素
来源：http://eec.svipenyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bge.pycfn.com

[S41] C++：类与构造函数
来源：http://ebg.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zww.sweek.top

[S42] C++：继承与虚函数
来源：http://syn.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://uix.daria6918.cn

[S43] C++：智能指针
来源：http://evh.zhengqikj.top

auto p = std::make_unique<int>(5);
来源：http://qsu.yj20258888.top

[S44] C++：引用传参
来源：http://quw.andypj.xyz

void inc(int &x) { ++x; }
来源：http://lwn.ydzc1.top

[S45] C++：lambda
来源：http://dlj.xziqi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hxu.cucudq.cn

[S46] C++：函数模板
来源：http://qmn.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nen.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://wvp.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dot.sysykeji.top

[S48] C++：逐行读文件
来源：http://sqy.gotoacloud.top

std::ifstream in("a.txt");  std::string line;
来源：http://qzx.ivvv.top

while (std::getline(in, line)) { }
来源：http://bht.yongpay.top

[S49] C++：写文件
来源：http://pbg.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kri.9152youxi.cn

[S50] C++：格式化数字
来源：http://yvm.sxryk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dup.meibo888.top

[S51] C++：显式类型转换
来源：http://ztc.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://toe.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://pat.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://pmq.yfazqb.com

[S53] C++：移动语义
来源：http://ech.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://cun.gotoacloud.top

[S54] C++：异常处理
来源：http://pbt.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qzf.hfpthk.cn

[S55] C++：结构化绑定
来源：http://clz.yuanzhike.top

auto [a, b] = std::make_pair(1, 2);
来源：http://got.gzhubu.top

[S56] C++：optional
来源：http://obc.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vwz.zhongyouzk.top

[S57] C++：编译期常量
来源：http://zmm.shanyushiyangtech.top

constexpr int N = 10;
来源：http://fqd.cucudq.cn

[S58] C++：命名空间
来源：http://etx.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://ldn.meibo888.top

[S59] C++：静态断言
来源：http://isp.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zit.uphjek.com

[S60] C++：遍历并删除元素
来源：http://vox.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://asb.ybcxt.top

================================================================================
来源：http://czj.shzxlz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://avv.vehdjk.com

================================================================================
来源：http://jry.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://ejb.iojbl.cn

println("Hello")
来源：http://gjy.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://ycp.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zor.jinyuanbaomall.cn

[T03] Kotlin：字符串模板
来源：http://zbm.jqgfzy.top

"值: $b"
来源：http://zsb.shuidangran.top

[T04] Kotlin：空安全
来源：http://tbd.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://nua.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://wir.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xmu.dianchejie.cn

[T06] Kotlin：集合映射
来源：http://qfv.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tfe.birdmap.top

[T07] Kotlin：集合过滤
来源：http://and.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cbu.smart0.xyz

[T08] Kotlin：数据类
来源：http://eho.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://rfa.hammf.cn

[T09] Kotlin：扩展函数
来源：http://gcj.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://ihw.yj20258888.top

[T10] Kotlin：默认参数
来源：http://uli.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jro.smart0.xyz

[T11] Kotlin：协程
来源：http://uyz.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fom.nwbrower.top

[T12] Kotlin：解构声明
来源：http://tst.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://rid.pycfn.com

[T13] Kotlin：只读 Map
来源：http://ttx.hnxiangtu.top

val m = mapOf("a" to 1)
来源：http://sov.jqgfzy.top

[T14] Kotlin：循环
来源：http://qgq.tanke756.top

for (i in 1..10) println(i)
来源：http://sja.guannengcc.top

[T15] Kotlin：接口
来源：http://vza.pengpengdd.cyou

interface Shape { fun area(): Double }
来源：http://ibg.yj20258888.top

[T16] Swift：Hello World
来源：http://ach.vehdjk.com

print("Hello")
来源：http://owp.xziqi.cn

[T17] Swift：变量与常量
来源：http://ray.andypj.xyz

var a = 1;  let b = 2
来源：http://myp.sxryk.cn

[T18] Swift：字符串插值
来源：http://omx.yangfankeji.com

"值: \(b)"
来源：http://ash.zhengqikj.top

[T19] Swift：可选绑定
来源：http://zoa.shzxlz.cn

if let n = opt { print(n) }
来源：http://ond.cqqwz.cn

[T20] Swift：数组操作
来源：http://vst.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lxl.xingfuxueyuan.xyz

[T21] Swift：遍历
来源：http://zaw.jinghuilouyu.cn

for x in a { print(x) }
来源：http://vfq.hywenlv.cn

[T22] Swift：字典
来源：http://uzh.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://qnl.shanyushiyangkeji.top

[T23] Swift：函数
来源：http://qxs.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jlz.hcnkem.com

[T24] Swift：闭包
来源：http://ixf.cucudq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jtp.zdqjudy.top

[T25] Swift：结构体
来源：http://fyr.guannengcc.top

struct P { var x: Int }
来源：http://kld.shuidangran.top

[T26] Swift：类与重写
来源：http://yfs.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://inm.pycfn.com

[T27] Swift：错误处理
来源：http://wyv.fzhhl.top

do { try f() } catch { print(error) }
来源：http://yos.yj202588.top

[T28] Swift：枚举
来源：http://ctf.9152youxi.cn

enum Color { case red, green }
来源：http://kfg.316326.xyz

[T29] Swift：guard 提前返回
来源：http://zwt.yvedp.cn

guard let x = opt else { return }
来源：http://lbs.svipenyu.cn

[T30] Swift：协议
来源：http://mwp.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://gav.ybcxt.top

[T31] Lua：Hello World
来源：http://ygc.jinqigufen.top

print("Hello")
来源：http://lcu.cqqwz.cn

[T32] Lua：局部变量
来源：http://qnr.tianlin.xyz

local a = 1
来源：http://wdx.jianghu66.top

[T33] Lua：表（数组）
来源：http://fob.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xnh.zdbjq.cn

[T34] Lua：遍历表
来源：http://ehy.yangfankeji.com

for i, v in ipairs(t) do print(i, v) end
来源：http://wqk.shanyushiyangkeji.top

[T35] Lua：字典表
来源：http://dim.jianghu66.top

local d = { a = 1 };  d.b = 2
来源：http://wts.meibo888.top

[T36] Lua：函数
来源：http://xwo.yuanzhike.top

function add(a, b) return a + b end
来源：http://rlj.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://tat.hnqzz.top

"a" .. "b"
来源：http://ojf.snrcjt.cn

[T38] Lua：条件
来源：http://qbp.hfpthk.cn

if x > 0 then print("正") end
来源：http://qok.yj20258888.top

[T39] Lua：模式匹配
来源：http://ext.gotoacloud.top

string.find(s, "%d+")
来源：http://gpe.sjlbkw.cn

[T40] Lua：元表
来源：http://jro.cheryme.top

setmetatable({}, { __index = base })
来源：http://gov.fehbvm.com

[T41] Perl：Hello World
来源：http://jvc.yj20258.top

print "Hello\n";
来源：http://pmd.birdmap.top

[T42] Perl：变量类型
来源：http://tqt.haohaochexian.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://olt.fanxiaobao.xyz

[T43] Perl：字符串插值
来源：http://hev.ywan-chungtsiang.top

"值: $a"
来源：http://tqf.0kj1m.cn

[T44] Perl：条件
来源：http://ypk.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://ctw.aizwys.cn

[T45] Perl：数组遍历
来源：http://unh.yonumen.top

for my $x (@arr) { print $x; }
来源：http://zyk.tarul.cn

[T46] Perl：哈希操作
来源：http://uoi.wangshuangyany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pxh.vqdsnc.cn

[T47] Perl：正则捕获
来源：http://rjh.ydzc1.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vhl.zhongyouzk.top

[T48] Perl：正则替换
来源：http://eeg.ywan-chungtsiang.top

$s =~ s/old/new/g;
来源：http://zqp.0kj1m.cn

[T49] Perl：函数
来源：http://ndw.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nye.aibaodan.cn

[T50] Perl：逐行读文件
来源：http://ihx.52xcode.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pyr.birdmap.top

while (my $line = <$fh>) { print $line; }
来源：http://teb.xingfuxueyuan.xyz

[T51] Scala：Hello World
来源：http://ygo.aibaodan.cn

println("Hello")
来源：http://mui.jqgufenzy.top

[T52] Scala：变量
来源：http://ijw.zhengqikj.top

val a = 1;  var b = 2
来源：http://hqy.shzxlz.cn

[T53] Scala：字符串插值
来源：http://scx.dashuyun.cn

s"值: $b"
来源：http://abx.ybcxt.top

[T54] Scala：集合映射
来源：http://udx.316326.xyz

List(1, 2, 3).map(_ * 2)
来源：http://tqi.cdnleiting.top

[T55] Scala：集合过滤
来源：http://ota.tanke756.top

List(1, 2, 3).filter(_ > 1)
来源：http://klm.yongpay.top

[T56] Scala：样例类
来源：http://aau.bjfxy.top

case class User(name: String, age: Int)
来源：http://ive.xuanzx.com

[T57] Scala：模式匹配
来源：http://mel.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yzz.jqgfzy.top

[T58] Scala：函数定义
来源：http://dnk.pycfn.com

def add(a: Int, b: Int): Int = a + b
来源：http://ydy.fzhhl.top

[T59] Scala：循环
来源：http://skj.xylfe.cn

for (i <- 1 to 10) println(i)
来源：http://qnl.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://hmk.shuidangran.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bmt.ybcxt.top

================================================================================
来源：http://qmo.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zdc.yangfankeji.com

================================================================================
来源：http://bxm.fanxiaobao.xyz


<!-- 参考信息 -->