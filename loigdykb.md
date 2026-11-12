代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hwq.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://whi.ppjwa.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lkd.epnwcf.com

[R61] 磁盘占用
来源：http://hwx.mhx1999.top

df -h;  du -sh *
来源：http://hll.jqgfzy.top

[R62] 找最占空间的文件
来源：http://yif.ivvv.top

du -ah . | sort -rh | head -10
来源：http://pmq.yfazqb.com

[R63] 内存与进程
来源：http://afk.snrcjt.cn

free -h;  ps aux | grep nginx
来源：http://xdu.wangdashe.top

[R64] 结束进程
来源：http://fed.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://ajg.yongpay.top

[R65] 查看端口占用
来源：http://neu.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dkr.xziqi.cn

[R66] 定时任务
来源：http://osn.hnxiangtu.top

crontab -e;  crontab -l
来源：http://hpu.cucudq.cn

[R67] 生成随机十六进制串
来源：http://enh.svipenyu.cn

openssl rand -hex 16
来源：http://jji.sjlbkw.cn

[R68] 计算文件校验值
来源：http://run.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hbg.xinyue.icu

[R69] 生成随机密码
来源：http://coo.gotoacloud.top

head -c 16 /dev/urandom | base64
来源：http://icy.epnwcf.com

[R70] 时间戳与互转
来源：http://aon.mhx1999.top

date +%s;  date -d @1700000000
来源：http://zxe.xylfe.cn

[R71] 日期格式化
来源：http://epq.xuanzx.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://fhv.ehwqpu.com

[R72] 等待端口就绪
来源：http://cpc.hcnkem.com

until nc -z localhost 3306; do sleep 1; done
来源：http://nyh.tianlin.xyz

[R73] 分割大日志
来源：http://aal.fengsongda.top

split -l 1000 big.log part_
来源：http://ccj.tianlin.xyz

[R74] 批量重命名
来源：http://wwf.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bzy.daxiang520.top

[R75] 导出环境变量
来源：http://bpx.bbcook.cn

export PATH="$HOME/bin:$PATH"
来源：http://fkn.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://bbu.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zyf.ivvv.top

[R77] 读取用户输入
来源：http://ydq.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://hse.chenzaomai.com

[R78] 交互式菜单
来源：http://zaf.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ysb.jiagoushi.top

[R79] 解析命令行选项
来源：http://ked.wangdashe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://veq.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://yhy.jqgfzy.top

time ./run.sh
来源：http://gzi.fehbvm.com

================================================================================
来源：http://oay.cashguo.top

S. C / C++ 专题
来源：http://bbi.c1oappe.top

================================================================================
来源：http://ccz.nanxuanxn.top

[S01] C：Hello World
来源：http://jix.snrcjt.cn

#include <stdio.h>
来源：http://yii.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rwo.zhaomingkeji.xyz

[S02] C：变量与格式化输出
来源：http://nmv.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://bor.chenjidiqi.icu

[S03] C：读入整数
来源：http://ubm.sweek.top

int x; scanf("%d", &x);
来源：http://rqm.vqdsnc.cn

[S04] C：字符串复制
来源：http://ocd.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://huj.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://fjl.sysykeji.top

strlen(s)
来源：http://cyf.sysykeji.top

[S06] C：字符串比较
来源：http://uhj.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://hha.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://niq.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xea.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://rei.cdnleiting.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gkv.feifeiyinyue.top

[S09] C：结构体定义与初始化
来源：http://ogt.cashguo.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://inw.yuanzhike.top

[S10] C：指针与解引用
来源：http://fez.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://iuc.xinyue.icu

[S11] C：逐行读文件
来源：http://dto.xinyue.icu

FILE *f = fopen("a.txt", "r");
来源：http://vnt.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://noj.hnqzz.top

fclose(f);
来源：http://vzs.c1oappe.top

[S12] C：写文件
来源：http://wjr.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tbz.52xcode.cn

[S13] C：宏定义
来源：http://nht.yangfankeji.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mmx.dashuyun.cn

[S14] C：枚举
来源：http://afx.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://duj.gzhubu.top

[S15] C：类型转换
来源：http://lxb.jqgfzy.top

(double) a / b
来源：http://gce.zhaomingkeji.xyz

[S16] C：位操作置位
来源：http://zwp.zhongyouzk.top

x |= (1 << 3);
来源：http://uyy.dianchejie.cn

[S17] C：安全拼接字符串
来源：http://ugc.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wxx.bbcook.cn

[S18] C：命令行参数
来源：http://tkl.svipenyu.cn

int main(int argc, char **argv)
来源：http://zsv.zhoulong.xyz

[S19] C：快速排序
来源：http://jbn.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://smv.cqqwz.cn

[S20] C：二分查找
来源：http://epi.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pbn.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://cmp.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iam.tanke756.top

[S22] C：字符串转数字
来源：http://jfr.mhx1999.top

atoi("42");  strtod("3.14", NULL);
来源：http://jhm.yvedp.cn

[S23] C：随机数
来源：http://zuv.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nbq.ctjpmb.com

[S24] C：获取本地时间
来源：http://mtp.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dtn.ctjpmb.com

[S25] C：内存拷贝
来源：http://uha.hysaishi.cn

memcpy(dst, src, n);
来源：http://inp.fzhhl.top

[S26] C：内存清零
来源：http://xqr.hammf.cn

memset(a, 0, sizeof a);
来源：http://dej.hysaishi.cn

[S27] C：定义常量
来源：http://tvq.mhx1999.top

const double PI = 3.14159;
来源：http://acq.xingfuxueyuan.xyz

[S28] C：静态变量
来源：http://fht.ydjk.org.cn

static int counter = 0;
来源：http://ufj.tarul.cn

[S29] C：变参函数
来源：http://lhe.gotoacloud.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ghs.316326.xyz

[S30] C：头文件保护
来源：http://vzn.uphjek.com

#ifndef X_H
来源：http://beb.cdnleiting.top

#define X_H
来源：http://teu.zhaomingkeji.xyz

#endif
来源：http://rqm.tarul.cn

[S31] C++：Hello World
来源：http://xyv.sysykeji.top

#include <iostream>
来源：http://uus.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://kci.mhx1999.top

[S32] C++：字符串
来源：http://ddu.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://asd.havefunace.top

[S33] C++：vector 增删
来源：http://qzg.pengpengdd.cyou

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://glf.sysykeji.top

[S34] C++：遍历 vector
来源：http://ier.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://ivl.shanyushiyangkeji.top

[S35] C++：map
来源：http://mmg.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vdk.vqdsnc.cn

[S36] C++：unordered_map
来源：http://mkw.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zmf.aibaodan.cn

[S37] C++：set
来源：http://vks.vehdjk.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://spf.jqgfzy.top

[S38] C++：排序
来源：http://uao.snrcjt.cn

std::sort(v.begin(), v.end());
来源：http://umu.zhijiandao.cn

[S39] C++：自定义比较器排序
来源：http://okn.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bxl.fzhhl.top

[S40] C++：查找元素
来源：http://ade.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ulk.ydjk.org.cn

[S41] C++：类与构造函数
来源：http://fqk.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ktp.tarul.cn

[S42] C++：继承与虚函数
来源：http://bcs.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://unn.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://okf.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://nzr.chenjidiqi.icu

[S44] C++：引用传参
来源：http://mjt.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://ojg.jlsjyb.cn

[S45] C++：lambda
来源：http://kte.yanxiufei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ctc.yj20258888.top

[S46] C++：函数模板
来源：http://iqq.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cpv.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://cyp.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mdi.wangdashe.top

[S48] C++：逐行读文件
来源：http://lev.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cwp.nanxuanxn.top

while (std::getline(in, line)) { }
来源：http://kgy.yuxming.cn

[S49] C++：写文件
来源：http://ppq.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wmi.tarul.cn

[S50] C++：格式化数字
来源：http://xnd.zhongyouzk.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ldc.xuetiantiany.cn

[S51] C++：显式类型转换
来源：http://lxf.aibaodan.cn

static_cast<double>(a) / b
来源：http://tto.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://xkt.andypj.xyz

int size() const noexcept { return n_; }
来源：http://rjf.tianlin.xyz

[S53] C++：移动语义
来源：http://ium.yj20258.top

std::vector<int> w = std::move(v);
来源：http://mqf.haohaochexian.top

[S54] C++：异常处理
来源：http://aup.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jhb.havefunace.top

[S55] C++：结构化绑定
来源：http://vxg.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pep.guowangkeji.top

[S56] C++：optional
来源：http://bql.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://frv.jiagoushi.top

[S57] C++：编译期常量
来源：http://rvg.sufxvd.cn

constexpr int N = 10;
来源：http://rwa.yj20258.top

[S58] C++：命名空间
来源：http://mrh.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://ixz.aizwys.cn

[S59] C++：静态断言
来源：http://ykk.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ukl.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://alt.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yvk.jianghu66.top

================================================================================
来源：http://ybn.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fez.nwbrower.top

================================================================================
来源：http://wdl.fzhhl.top

[T01] Kotlin：Hello World
来源：http://mtg.jqgfzy.top

println("Hello")
来源：http://eya.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://xrq.xuetiantiany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uzl.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://zqa.uphjek.com

"值: $b"
来源：http://fan.yj20258.top

[T04] Kotlin：空安全
来源：http://prj.yangfankeji.com

val n: String? = null;  n?.length
来源：http://cug.hongshengwenyu.top

[T05] Kotlin：when 表达式
来源：http://gfn.zhijiandao.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dnx.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://xol.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wti.9152youxi.cn

[T07] Kotlin：集合过滤
来源：http://sfd.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dtj.hammf.cn

[T08] Kotlin：数据类
来源：http://ewq.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://dfc.snrcjt.cn

[T09] Kotlin：扩展函数
来源：http://zgs.yueranfly.top

fun String.exclaim() = this + "!"
来源：http://eks.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://nwi.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://azu.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://qcd.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ood.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://vyf.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://yiz.dashuyun.cn

[T13] Kotlin：只读 Map
来源：http://boj.daxiang520.top

val m = mapOf("a" to 1)
来源：http://vnd.316326.xyz

[T14] Kotlin：循环
来源：http://xvk.bjfxy.top

for (i in 1..10) println(i)
来源：http://eks.meibo888.top

[T15] Kotlin：接口
来源：http://azz.jlsjyb.cn

interface Shape { fun area(): Double }
来源：http://stb.jiagoushi.top

[T16] Swift：Hello World
来源：http://ccp.andypj.xyz

print("Hello")
来源：http://vmx.dianchejie.cn

[T17] Swift：变量与常量
来源：http://zih.aibaodan.cn

var a = 1;  let b = 2
来源：http://sab.yuanzhike.top

[T18] Swift：字符串插值
来源：http://nwj.wangdashe.top

"值: \(b)"
来源：http://eel.yj202588.top

[T19] Swift：可选绑定
来源：http://opt.chenzaomai.com

if let n = opt { print(n) }
来源：http://ark.fengsongda.top

[T20] Swift：数组操作
来源：http://aga.jlsjyb.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uqy.jqgufenzy.top

[T21] Swift：遍历
来源：http://qza.wangdashe.top

for x in a { print(x) }
来源：http://ket.hesvh.cn

[T22] Swift：字典
来源：http://aiz.chenzaomai.com

var d = ["a": 1];  d["b"] = 2
来源：http://wvh.yuanzhike.top

[T23] Swift：函数
来源：http://xsz.aizwys.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://phs.yonumen.top

[T24] Swift：闭包
来源：http://wks.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qcq.yvedp.cn

[T25] Swift：结构体
来源：http://brz.0kj1m.cn

struct P { var x: Int }
来源：http://zze.vehdjk.com

[T26] Swift：类与重写
来源：http://nuy.zycfv.cn

class A: Base { override func f() {} }
来源：http://fed.zdbjq.cn

[T27] Swift：错误处理
来源：http://zaj.zycfv.cn

do { try f() } catch { print(error) }
来源：http://sjn.jiagoushi.top

[T28] Swift：枚举
来源：http://fjs.gaohongyu789.top

enum Color { case red, green }
来源：http://dbw.yongpay.top

[T29] Swift：guard 提前返回
来源：http://kbd.gzhubu.top

guard let x = opt else { return }
来源：http://sup.dashuyun.cn

[T30] Swift：协议
来源：http://xqf.yueranfly.top

protocol Shape { func area() -> Double }
来源：http://zwl.jinqigfzy.top

[T31] Lua：Hello World
来源：http://hjs.sxryk.cn

print("Hello")
来源：http://zob.yuanzhike.top

[T32] Lua：局部变量
来源：http://rbm.pycfn.com

local a = 1
来源：http://ysa.epnwcf.com

[T33] Lua：表（数组）
来源：http://ziq.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ivv.shangyingyoupin.top

[T34] Lua：遍历表
来源：http://gov.gaohongyu789.top

for i, v in ipairs(t) do print(i, v) end
来源：http://djf.daxiang520.top

[T35] Lua：字典表
来源：http://yon.cqqwz.cn

local d = { a = 1 };  d.b = 2
来源：http://ovs.smart0.xyz

[T36] Lua：函数
来源：http://qua.daria6918.cn

function add(a, b) return a + b end
来源：http://mmr.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://vlb.316326.xyz

"a" .. "b"
来源：http://iiv.jinghuilouyu.cn

[T38] Lua：条件
来源：http://qjl.yfazqb.com

if x > 0 then print("正") end
来源：http://nrj.sufxvd.cn

[T39] Lua：模式匹配
来源：http://kld.andypj.xyz

string.find(s, "%d+")
来源：http://ksw.shanyushiyangtech.top

[T40] Lua：元表
来源：http://ffr.yj20258888.top

setmetatable({}, { __index = base })
来源：http://fjk.shanyushiyangtech.top

[T41] Perl：Hello World
来源：http://zdy.hnxiangtu.top

print "Hello\n";
来源：http://chg.guannengcc.top

[T42] Perl：变量类型
来源：http://dsd.gaohongyu789.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://erj.shuidangran.top

[T43] Perl：字符串插值
来源：http://gdt.316326.xyz

"值: $a"
来源：http://vki.nanxuanxn.top

[T44] Perl：条件
来源：http://byy.sweek.top

if ($a > 0) { print "正"; }
来源：http://yzt.xuanzx.com

[T45] Perl：数组遍历
来源：http://wdq.jqgfzy.top

for my $x (@arr) { print $x; }
来源：http://men.9152youxi.cn

[T46] Perl：哈希操作
来源：http://neh.havefunace.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://frx.cucudq.cn

[T47] Perl：正则捕获
来源：http://lbj.jqgfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cet.yanxiufei.cn

[T48] Perl：正则替换
来源：http://hxs.fengsongda.top

$s =~ s/old/new/g;
来源：http://qin.yj20258.top

[T49] Perl：函数
来源：http://eqc.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zco.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://qin.fehbvm.com

open my $fh, "<", "a.txt" or die $!;
来源：http://sfm.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://rjz.zhijiandao.cn

[T51] Scala：Hello World
来源：http://qke.cdnleiting.top

println("Hello")
来源：http://jgw.chenjidiqi.icu

[T52] Scala：变量
来源：http://nsz.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://zjp.xylfe.cn

[T53] Scala：字符串插值
来源：http://bip.jinqigufen.top

s"值: $b"
来源：http://btd.gotoacloud.top

[T54] Scala：集合映射
来源：http://mjk.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://kfr.vehdjk.com

[T55] Scala：集合过滤
来源：http://pnd.316326.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://taj.nanxuanxn.top

[T56] Scala：样例类
来源：http://eri.tarul.cn

case class User(name: String, age: Int)
来源：http://xhi.0kj1m.cn

[T57] Scala：模式匹配
来源：http://ghi.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wnx.redwolf501.top

[T58] Scala：函数定义
来源：http://nxj.jlsjyb.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ach.birdmap.top

[T59] Scala：循环
来源：http://vfp.yfazqb.com

for (i <- 1 to 10) println(i)
来源：http://snn.wangshuangyany.cn

[T60] Scala：折叠
来源：http://iiw.yj20258888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pab.52xcode.cn

================================================================================
来源：http://nih.hesvh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aam.wangdashe.top

================================================================================
来源：http://qns.ivvv.top


<!-- 参考信息 -->