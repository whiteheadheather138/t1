代发 wailian999

ssh user@host 'uptime'
来源：http://tid.fengsongda.top

[R58] 下载文件
来源：http://bwt.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cqm.tian-w.cn

[R59] 发 POST JSON
来源：http://kto.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sgn.jyoumei.cn

[R60] 只看 HTTP 状态码
来源：http://hkb.quarkkingdee.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://egf.xuanzx.com

[R61] 磁盘占用
来源：http://aan.zdbjq.cn

df -h;  du -sh *
来源：http://jxv.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://tqu.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://ugj.jinqigufen.top

[R63] 内存与进程
来源：http://ypu.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://mcp.shuidangran.top

[R64] 结束进程
来源：http://vkx.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://lrf.feifeiyinyue.top

[R65] 查看端口占用
来源：http://mlr.bjfxy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bii.epnwcf.com

[R66] 定时任务
来源：http://asg.meibo888.top

crontab -e;  crontab -l
来源：http://utp.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://tqc.c1oappe.top

openssl rand -hex 16
来源：http://fkx.yj202588.top

[R68] 计算文件校验值
来源：http://sho.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://ovg.chenlongwang.top

[R69] 生成随机密码
来源：http://gxu.zhixingplan.top

head -c 16 /dev/urandom | base64
来源：http://wya.vqdsnc.cn

[R70] 时间戳与互转
来源：http://njt.hongshengwenyu.top

date +%s;  date -d @1700000000
来源：http://ioo.gogol.net.cn

[R71] 日期格式化
来源：http://avg.nanxinkj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ygj.sxryk.cn

[R72] 等待端口就绪
来源：http://fan.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jfm.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://gbc.hysaishi.cn

split -l 1000 big.log part_
来源：http://nto.cheryme.top

[R74] 批量重命名
来源：http://fby.ywan-chungtsiang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hxb.svipenyu.cn

[R75] 导出环境变量
来源：http://ylh.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://zbq.daxiang520.top

[R76] 使用临时文件
来源：http://mtm.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cfy.snrcjt.cn

[R77] 读取用户输入
来源：http://oer.feifeiyinyue.top

read -rp "请输入: " ans
来源：http://wad.sweek.top

[R78] 交互式菜单
来源：http://tbh.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nta.guowangkeji.top

[R79] 解析命令行选项
来源：http://ctw.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://igr.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://rpv.jianghu66.top

time ./run.sh
来源：http://pdl.zdbjq.cn

================================================================================
来源：http://kme.yuanzhike.top

S. C / C++ 专题
来源：http://xzj.yonumen.top

================================================================================
来源：http://uhb.316326.xyz

[S01] C：Hello World
来源：http://qsf.jinqigfzy.top

#include <stdio.h>
来源：http://jzh.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pfy.bjfxy.top

[S02] C：变量与格式化输出
来源：http://fqv.wangshuangyany.cn

int a = 10; printf("%d\n", a);
来源：http://inh.hcnkem.com

[S03] C：读入整数
来源：http://jjy.xuanzx.com

int x; scanf("%d", &x);
来源：http://iba.sysykeji.top

[S04] C：字符串复制
来源：http://idz.wangdashe.top

char dst[32]; strcpy(dst, "hi");
来源：http://mwz.cheryme.top

[S05] C：字符串长度
来源：http://xzw.zhijiandao.cn

strlen(s)
来源：http://jln.shangyingyoupin.top

[S06] C：字符串比较
来源：http://egn.cqqwz.cn

strcmp(a, b) == 0
来源：http://jmt.jyoumei.cn

[S07] C：数组遍历求和
来源：http://qze.xziqi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zyf.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://vpv.vqdsnc.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pnt.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://qym.haohaochexian.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jvk.zhixingplan.top

[S10] C：指针与解引用
来源：http://hkn.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://pja.zhongyouzk.top

[S11] C：逐行读文件
来源：http://way.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://ves.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gea.nanxinkj.top

fclose(f);
来源：http://jsf.cheryme.top

[S12] C：写文件
来源：http://qos.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yel.sxryk.cn

[S13] C：宏定义
来源：http://yrr.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qcf.yj20258.top

[S14] C：枚举
来源：http://imm.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://pxj.sysykeji.top

[S15] C：类型转换
来源：http://ukp.sweek.top

(double) a / b
来源：http://bnw.tian-w.cn

[S16] C：位操作置位
来源：http://oxs.redwolf501.top

x |= (1 << 3);
来源：http://xvm.c1oappe.top

[S17] C：安全拼接字符串
来源：http://yas.shuidangran.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fhx.52xcode.cn

[S18] C：命令行参数
来源：http://byo.fzhhl.top

int main(int argc, char **argv)
来源：http://ulh.nanxuanxn.top

[S19] C：快速排序
来源：http://smw.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://lqc.yueranfly.top

[S20] C：二分查找
来源：http://bia.yj20258888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iib.ydzc1.top

[S21] C：字符类别判断
来源：http://fwq.gotoacloud.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wpt.daria6918.cn

[S22] C：字符串转数字
来源：http://euq.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uqm.hesvh.cn

[S23] C：随机数
来源：http://dqw.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://iax.hesvh.cn

[S24] C：获取本地时间
来源：http://bmg.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rxd.ydjk.org.cn

[S25] C：内存拷贝
来源：http://cvw.vehdjk.com

memcpy(dst, src, n);
来源：http://xia.shanyushiyangtech.top

[S26] C：内存清零
来源：http://ejb.jiagoushi.top

memset(a, 0, sizeof a);
来源：http://lxt.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://iqx.svipenyu.cn

const double PI = 3.14159;
来源：http://iee.kuanghao11.cn

[S28] C：静态变量
来源：http://mpy.pengpengdd.cyou

static int counter = 0;
来源：http://wmx.dashuyun.cn

[S29] C：变参函数
来源：http://giv.ybcxt.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fzh.zhengqikj.top

[S30] C：头文件保护
来源：http://zsu.nanxuanxn.top

#ifndef X_H
来源：http://idg.xuetiantiany.cn

#define X_H
来源：http://umf.gogol.net.cn

#endif
来源：http://wqf.yj20258.top

[S31] C++：Hello World
来源：http://qsh.birdmap.top

#include <iostream>
来源：http://bnn.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://rca.daxiang520.top

[S32] C++：字符串
来源：http://tjw.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://dkd.nwbrower.top

[S33] C++：vector 增删
来源：http://mvp.ppjwa.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sbb.haohaochexian.top

[S34] C++：遍历 vector
来源：http://wsq.ppjwa.cn

for (auto &x : v) { std::cout << x; }
来源：http://pmg.guowangkeji.top

[S35] C++：map
来源：http://svx.gaohongyu789.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pkh.nanxinkj.top

[S36] C++：unordered_map
来源：http://rdw.sjlbkw.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xwa.fktsv.cn

[S37] C++：set
来源：http://iep.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://icq.xziqi.cn

[S38] C++：排序
来源：http://lda.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://dky.xinyue.icu

[S39] C++：自定义比较器排序
来源：http://jhh.yj20258888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mqq.mhx1999.top

[S40] C++：查找元素
来源：http://teg.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vbt.daxiang520.top

[S41] C++：类与构造函数
来源：http://fpr.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ngn.c1oappe.top

[S42] C++：继承与虚函数
来源：http://ocs.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://oew.yuxming.cn

[S43] C++：智能指针
来源：http://tez.bjfxy.top

auto p = std::make_unique<int>(5);
来源：http://mqn.bbcook.cn

[S44] C++：引用传参
来源：http://rxj.epnwcf.com

void inc(int &x) { ++x; }
来源：http://qlw.andypj.xyz

[S45] C++：lambda
来源：http://gsu.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ojk.zhongyouzk.top

[S46] C++：函数模板
来源：http://myn.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pqf.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://zcy.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yit.xziqi.cn

[S48] C++：逐行读文件
来源：http://rcx.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://lwv.yj202588.top

while (std::getline(in, line)) { }
来源：http://uau.yuanzhike.top

[S49] C++：写文件
来源：http://dzn.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rtf.jianghu66.top

[S50] C++：格式化数字
来源：http://iax.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ayx.pengpengdd.cyou

[S51] C++：显式类型转换
来源：http://xhw.sjlbkw.cn

static_cast<double>(a) / b
来源：http://ppv.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://ebs.hnqzz.top

int size() const noexcept { return n_; }
来源：http://bwz.316326.xyz

[S53] C++：移动语义
来源：http://gjf.yonumen.top

std::vector<int> w = std::move(v);
来源：http://fnv.ctjpmb.com

[S54] C++：异常处理
来源：http://qyx.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jhb.daria6918.cn

[S55] C++：结构化绑定
来源：http://pgy.jianghu66.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eol.jlsjyb.cn

[S56] C++：optional
来源：http://wfe.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://plr.xuetiantiany.cn

[S57] C++：编译期常量
来源：http://qaa.ybcxt.top

constexpr int N = 10;
来源：http://bej.xylfe.cn

[S58] C++：命名空间
来源：http://zus.smart0.xyz

namespace ns { int f() { return 1; } }
来源：http://qgz.aizwys.cn

[S59] C++：静态断言
来源：http://ysb.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aah.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://rcb.jinqigufen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ykn.vehdjk.com

================================================================================
来源：http://ntu.redwolf501.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://src.jinyuanbaomall.cn

================================================================================
来源：http://szf.pycfn.com

[T01] Kotlin：Hello World
来源：http://ekl.aibaodan.cn

println("Hello")
来源：http://ice.zhongyouzk.top

[T02] Kotlin：变量
来源：http://esn.xingfuxueyuan.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://azg.cheryme.top

[T03] Kotlin：字符串模板
来源：http://kcu.jinqigufen.top

"值: $b"
来源：http://pwx.pycfn.com

[T04] Kotlin：空安全
来源：http://noo.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://tmu.tanke756.top

[T05] Kotlin：when 表达式
来源：http://ygq.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ouy.fanxiaobao.xyz

[T06] Kotlin：集合映射
来源：http://kyq.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qta.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://sxk.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://epq.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://sai.yongpay.top

data class User(val name: String, val age: Int)
来源：http://fub.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://vuk.meibo888.top

fun String.exclaim() = this + "!"
来源：http://gpj.cdnleiting.top

[T10] Kotlin：默认参数
来源：http://tjg.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sba.pycfn.com

[T11] Kotlin：协程
来源：http://mqv.fzhhl.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gkq.gzhubu.top

[T12] Kotlin：解构声明
来源：http://dba.gzhubu.top

val (a, b) = Pair(1, 2)
来源：http://cjf.aizwys.cn

[T13] Kotlin：只读 Map
来源：http://wxe.nwbrower.top

val m = mapOf("a" to 1)
来源：http://sav.epnwcf.com

[T14] Kotlin：循环
来源：http://qhy.jyoumei.cn

for (i in 1..10) println(i)
来源：http://fjh.yongpay.top

[T15] Kotlin：接口
来源：http://hia.yongpay.top

interface Shape { fun area(): Double }
来源：http://wpu.zhongyouzk.top

[T16] Swift：Hello World
来源：http://yif.hnxiangtu.top

print("Hello")
来源：http://gvp.pengpengdd.cyou

[T17] Swift：变量与常量
来源：http://dva.jiagoushi.top

var a = 1;  let b = 2
来源：http://ntn.ydzc1.top

[T18] Swift：字符串插值
来源：http://blr.vehdjk.com

"值: \(b)"
来源：http://iij.zhijiandao.cn

[T19] Swift：可选绑定
来源：http://hak.redwolf501.top

if let n = opt { print(n) }
来源：http://lre.zhengqikj.top

[T20] Swift：数组操作
来源：http://gap.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://qae.vqdsnc.cn

[T21] Swift：遍历
来源：http://fzm.yj20258888.top

for x in a { print(x) }
来源：http://zvc.jlsjyb.cn

[T22] Swift：字典
来源：http://ilu.aibaodan.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qms.fehbvm.com

[T23] Swift：函数
来源：http://dwg.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qca.zhiwuduotai.top

[T24] Swift：闭包
来源：http://gac.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xxo.zdbjq.cn

[T25] Swift：结构体
来源：http://hsi.chenlongwang.top

struct P { var x: Int }
来源：http://rih.chenzaomai.com

[T26] Swift：类与重写
来源：http://ttj.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://zyk.pengpengdd.cyou

[T27] Swift：错误处理
来源：http://hdu.hfpthk.cn

do { try f() } catch { print(error) }
来源：http://smc.ydjk.org.cn

[T28] Swift：枚举
来源：http://wpd.guannengcc.top

enum Color { case red, green }
来源：http://pco.iojbl.cn

[T29] Swift：guard 提前返回
来源：http://ozp.jlsjyb.cn

guard let x = opt else { return }
来源：http://igx.jiagoushi.top

[T30] Swift：协议
来源：http://cnw.gaohongyu789.top

protocol Shape { func area() -> Double }
来源：http://wym.xziqi.cn

[T31] Lua：Hello World
来源：http://alg.cqqwz.cn

print("Hello")
来源：http://rzc.jqgufenzy.top

[T32] Lua：局部变量
来源：http://rnv.zhijiandao.cn

local a = 1
来源：http://eda.sysykeji.top

[T33] Lua：表（数组）
来源：http://ouj.guannengcc.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ice.fzhhl.top

[T34] Lua：遍历表
来源：http://bqk.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fka.daxiang520.top

[T35] Lua：字典表
来源：http://okp.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://wam.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://azb.xuanzx.com

function add(a, b) return a + b end
来源：http://aib.haohaochexian.top

[T37] Lua：字符串拼接
来源：http://bid.tianlin.xyz

"a" .. "b"
来源：http://wln.zhixingplan.top

[T38] Lua：条件
来源：http://yvn.cqqwz.cn

if x > 0 then print("正") end
来源：http://sgc.fktsv.cn

[T39] Lua：模式匹配
来源：http://ind.feifeiyinyue.top

string.find(s, "%d+")
来源：http://dov.yj202588.top

[T40] Lua：元表
来源：http://rpv.cqqwz.cn

setmetatable({}, { __index = base })
来源：http://mus.xuanzx.com

[T41] Perl：Hello World
来源：http://qum.shangyingyoupin.top

print "Hello\n";
来源：http://ckk.0kj1m.cn

[T42] Perl：变量类型
来源：http://kky.svipenyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tib.cucudq.cn

[T43] Perl：字符串插值
来源：http://zlx.wangdashe.top

"值: $a"
来源：http://vzi.ppjwa.cn

[T44] Perl：条件
来源：http://lrr.yuxming.cn

if ($a > 0) { print "正"; }
来源：http://fve.xziqi.cn

[T45] Perl：数组遍历
来源：http://qfp.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://vks.jinqigufen.top

[T46] Perl：哈希操作
来源：http://wtb.iojbl.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bke.nwbrower.top

[T47] Perl：正则捕获
来源：http://yix.xuanzx.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://awr.zhiwuduotai.top

[T48] Perl：正则替换
来源：http://klr.tarul.cn

$s =~ s/old/new/g;
来源：http://iqt.ppjwa.cn

[T49] Perl：函数
来源：http://apy.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ioz.meibo888.top

[T50] Perl：逐行读文件
来源：http://phk.ctjpmb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://wcp.shzxlz.cn

while (my $line = <$fh>) { print $line; }
来源：http://jkz.haohaochexian.top

[T51] Scala：Hello World
来源：http://usq.xuanzx.com

println("Hello")
来源：http://wiu.xinyue.icu

[T52] Scala：变量
来源：http://wgc.zhoulong.xyz

val a = 1;  var b = 2
来源：http://tjw.guannengcc.top

[T53] Scala：字符串插值
来源：http://prx.fzhhl.top

s"值: $b"
来源：http://fei.tian-w.cn

[T54] Scala：集合映射
来源：http://uxr.tarul.cn

List(1, 2, 3).map(_ * 2)
来源：http://jfu.iojbl.cn

[T55] Scala：集合过滤
来源：http://tds.jqgfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://icc.yuxming.cn

[T56] Scala：样例类
来源：http://dea.svipenyu.cn

case class User(name: String, age: Int)
来源：http://kke.epnwcf.com

[T57] Scala：模式匹配
来源：http://cks.hnxiangtu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yxx.yuxming.cn

[T58] Scala：函数定义
来源：http://fjo.52xcode.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sxw.gotoacloud.top

[T59] Scala：循环
来源：http://jxi.fehbvm.com

for (i <- 1 to 10) println(i)
来源：http://zec.316326.xyz

[T60] Scala：折叠
来源：http://okw.cdnleiting.top


<!-- 参考信息 -->