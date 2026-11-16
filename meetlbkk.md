代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jtp.zhixingplan.top

[R54] 比较两个文件
来源：http://rsv.jianghu66.top

diff a.txt b.txt
来源：http://aex.cashguo.top

[R55] 压缩与解压
来源：http://jux.ydjk.org.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oag.yj202588.top

[R56] 远程拷贝
来源：http://xfd.sufxvd.cn

scp file user@host:/path/
来源：http://wpk.yj20258.top

[R57] 远程执行命令
来源：http://phc.fzhhl.top

ssh user@host 'uptime'
来源：http://qrk.zycfv.cn

[R58] 下载文件
来源：http://kxx.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qhl.0kj1m.cn

[R59] 发 POST JSON
来源：http://zdu.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lte.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://sjh.dianchejie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fkm.shzxlz.cn

[R61] 磁盘占用
来源：http://rnx.guowangkeji.top

df -h;  du -sh *
来源：http://clx.zycfv.cn

[R62] 找最占空间的文件
来源：http://khs.bjfxy.top

du -ah . | sort -rh | head -10
来源：http://rfj.daxiang520.top

[R63] 内存与进程
来源：http://arh.shuidangran.top

free -h;  ps aux | grep nginx
来源：http://wsq.aibaodan.cn

[R64] 结束进程
来源：http://kaz.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://hyi.cucudq.cn

[R65] 查看端口占用
来源：http://zbm.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://igf.sweek.top

[R66] 定时任务
来源：http://isy.xziqi.cn

crontab -e;  crontab -l
来源：http://mfe.iojbl.cn

[R67] 生成随机十六进制串
来源：http://mcv.tian-w.cn

openssl rand -hex 16
来源：http://qfi.gogol.net.cn

[R68] 计算文件校验值
来源：http://eax.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://roa.meibo888.top

[R69] 生成随机密码
来源：http://bin.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://ebt.c1oappe.top

[R70] 时间戳与互转
来源：http://kdd.sxryk.cn

date +%s;  date -d @1700000000
来源：http://dih.ybcxt.top

[R71] 日期格式化
来源：http://dkg.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mfi.jianghu66.top

[R72] 等待端口就绪
来源：http://pxq.c1oappe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pnw.xuetiantiany.cn

[R73] 分割大日志
来源：http://qjw.andypj.xyz

split -l 1000 big.log part_
来源：http://gro.chenlongwang.top

[R74] 批量重命名
来源：http://yaf.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qzf.hesvh.cn

[R75] 导出环境变量
来源：http://jzc.jinqigufen.top

export PATH="$HOME/bin:$PATH"
来源：http://hoz.cucudq.cn

[R76] 使用临时文件
来源：http://xnm.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pst.fengsongda.top

[R77] 读取用户输入
来源：http://stf.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://lll.cucudq.cn

[R78] 交互式菜单
来源：http://yzl.tarul.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uqx.tarul.cn

[R79] 解析命令行选项
来源：http://khf.yueranfly.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fje.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://mph.zhengqikj.top

time ./run.sh
来源：http://wxq.sysykeji.top

================================================================================
来源：http://wra.cheryme.top

S. C / C++ 专题
来源：http://wcl.yanxiufei.cn

================================================================================
来源：http://svh.gzhubu.top

[S01] C：Hello World
来源：http://cej.daxiang520.top

#include <stdio.h>
来源：http://idc.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xip.fengsongda.top

[S02] C：变量与格式化输出
来源：http://stx.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://sng.jyoumei.cn

[S03] C：读入整数
来源：http://fgy.daxiang520.top

int x; scanf("%d", &x);
来源：http://lpk.xinyue.icu

[S04] C：字符串复制
来源：http://dvg.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fel.sjlbkw.cn

[S05] C：字符串长度
来源：http://vik.guannengcc.top

strlen(s)
来源：http://xkp.sxryk.cn

[S06] C：字符串比较
来源：http://klp.jinqigfzy.top

strcmp(a, b) == 0
来源：http://lpy.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://cab.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://deh.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://fyt.andypj.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nox.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://syw.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vsz.aibaodan.cn

[S10] C：指针与解引用
来源：http://umr.nwbrower.top

int *p = &a;  *p = 5;
来源：http://ceu.52xcode.cn

[S11] C：逐行读文件
来源：http://zdh.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://kdd.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qsg.zdqjudy.top

fclose(f);
来源：http://hey.bbcook.cn

[S12] C：写文件
来源：http://kmm.yuxming.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tyf.xuanzx.com

[S13] C：宏定义
来源：http://ybq.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eer.zhiwuduotai.top

[S14] C：枚举
来源：http://ltb.hysaishi.cn

enum Color { RED, GREEN, BLUE };
来源：http://hux.pengpengdd.cyou

[S15] C：类型转换
来源：http://qdg.mhx1999.top

(double) a / b
来源：http://wjl.xuanzx.com

[S16] C：位操作置位
来源：http://fhh.jinqigufen.top

x |= (1 << 3);
来源：http://myf.hcnkem.com

[S17] C：安全拼接字符串
来源：http://xzg.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ali.9152youxi.cn

[S18] C：命令行参数
来源：http://zcw.kuanghao11.cn

int main(int argc, char **argv)
来源：http://rdf.c1oappe.top

[S19] C：快速排序
来源：http://pis.jlsjyb.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ezj.9152youxi.cn

[S20] C：二分查找
来源：http://ukl.hnqzz.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cbj.uphjek.com

[S21] C：字符类别判断
来源：http://jjf.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xst.zycfv.cn

[S22] C：字符串转数字
来源：http://wwu.chenzaomai.com

atoi("42");  strtod("3.14", NULL);
来源：http://oun.jinghuilouyu.cn

[S23] C：随机数
来源：http://omy.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://plt.dianchejie.cn

[S24] C：获取本地时间
来源：http://ail.redwolf501.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://onb.shuidangran.top

[S25] C：内存拷贝
来源：http://jsk.shzxlz.cn

memcpy(dst, src, n);
来源：http://msc.yvedp.cn

[S26] C：内存清零
来源：http://ywz.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://fhn.yfazqb.com

[S27] C：定义常量
来源：http://cud.ehwqpu.com

const double PI = 3.14159;
来源：http://tez.jlsjyb.cn

[S28] C：静态变量
来源：http://wdu.jlsjyb.cn

static int counter = 0;
来源：http://fck.yangfankeji.com

[S29] C：变参函数
来源：http://ogf.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wmu.fzhhl.top

[S30] C：头文件保护
来源：http://lko.hammf.cn

#ifndef X_H
来源：http://snu.sxryk.cn

#define X_H
来源：http://ivz.cheryme.top

#endif
来源：http://jzj.zhongyouzk.top

[S31] C++：Hello World
来源：http://psl.jqgfzy.top

#include <iostream>
来源：http://ttm.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://lhj.smart0.xyz

[S32] C++：字符串
来源：http://wsn.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://aov.yfazqb.com

[S33] C++：vector 增删
来源：http://ypi.fktsv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://srz.sufxvd.cn

[S34] C++：遍历 vector
来源：http://zum.gogol.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://ooa.yangfankeji.com

[S35] C++：map
来源：http://aoh.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vuf.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://saj.dashuyun.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mif.tarul.cn

[S37] C++：set
来源：http://ciy.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zph.xuanzx.com

[S38] C++：排序
来源：http://rjq.ybcxt.top

std::sort(v.begin(), v.end());
来源：http://hmz.wangshuangyany.cn

[S39] C++：自定义比较器排序
来源：http://bwn.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ksr.fengsongda.top

[S40] C++：查找元素
来源：http://xvh.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tue.jianghu66.top

[S41] C++：类与构造函数
来源：http://ufg.shanyushiyangtech.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nvy.yongpay.top

[S42] C++：继承与虚函数
来源：http://fmp.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://nqu.daria6918.cn

[S43] C++：智能指针
来源：http://nmj.gaohongyu789.top

auto p = std::make_unique<int>(5);
来源：http://dmi.fengsongda.top

[S44] C++：引用传参
来源：http://qfo.sxryk.cn

void inc(int &x) { ++x; }
来源：http://mok.hcnkem.com

[S45] C++：lambda
来源：http://jdv.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://uug.jinqigfzy.top

[S46] C++：函数模板
来源：http://rkm.chenlongwang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gnv.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://hlq.sufxvd.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ksa.ivvv.top

[S48] C++：逐行读文件
来源：http://yyj.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://grh.zhiwuduotai.top

while (std::getline(in, line)) { }
来源：http://xry.nanxuanxn.top

[S49] C++：写文件
来源：http://inc.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yew.cashguo.top

[S50] C++：格式化数字
来源：http://bwe.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ggq.c1oappe.top

[S51] C++：显式类型转换
来源：http://xtf.redwolf501.top

static_cast<double>(a) / b
来源：http://lxq.meibo888.top

[S52] C++：const 与 noexcept
来源：http://hgn.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://tkb.zhixingplan.top

[S53] C++：移动语义
来源：http://pxy.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://kld.epnwcf.com

[S54] C++：异常处理
来源：http://hie.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://reo.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://hda.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gms.bjfxy.top

[S56] C++：optional
来源：http://sat.hongshengwenyu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ius.316326.xyz

[S57] C++：编译期常量
来源：http://ieq.jqgufenzy.top

constexpr int N = 10;
来源：http://giy.jyoumei.cn

[S58] C++：命名空间
来源：http://nlu.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://ers.chenjidiqi.icu

[S59] C++：静态断言
来源：http://vki.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nsx.zhijiandao.cn

[S60] C++：遍历并删除元素
来源：http://mal.gaohongyu789.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eyt.jinqigfzy.top

================================================================================
来源：http://sdt.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zkl.uphjek.com

================================================================================
来源：http://dcq.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://lqo.xingfuxueyuan.xyz

println("Hello")
来源：http://ook.meibo888.top

[T02] Kotlin：变量
来源：http://qmw.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://khb.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://xeg.bbcook.cn

"值: $b"
来源：http://wos.dashuyun.cn

[T04] Kotlin：空安全
来源：http://yyo.sxryk.cn

val n: String? = null;  n?.length
来源：http://cju.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://nqx.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fdc.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://mgj.ydjk.org.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yfh.jinqigfzy.top

[T07] Kotlin：集合过滤
来源：http://zeh.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bty.sufxvd.cn

[T08] Kotlin：数据类
来源：http://ivl.quarkkingdee.top

data class User(val name: String, val age: Int)
来源：http://llr.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://jsg.aibaodan.cn

fun String.exclaim() = this + "!"
来源：http://iai.uphjek.com

[T10] Kotlin：默认参数
来源：http://rpc.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qls.jqgfzy.top

[T11] Kotlin：协程
来源：http://azi.cdnleiting.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ouz.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://scv.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://vwt.svipenyu.cn

[T13] Kotlin：只读 Map
来源：http://trd.cqqwz.cn

val m = mapOf("a" to 1)
来源：http://btl.wangdashe.top

[T14] Kotlin：循环
来源：http://lsf.fktsv.cn

for (i in 1..10) println(i)
来源：http://bro.fzhhl.top

[T15] Kotlin：接口
来源：http://yxl.yueranfly.top

interface Shape { fun area(): Double }
来源：http://erz.jinghuilouyu.cn

[T16] Swift：Hello World
来源：http://qyy.guannengcc.top

print("Hello")
来源：http://ivf.yonumen.top

[T17] Swift：变量与常量
来源：http://zzt.yanxiufei.cn

var a = 1;  let b = 2
来源：http://uhk.yanxiufei.cn

[T18] Swift：字符串插值
来源：http://gdk.chenzaomai.com

"值: \(b)"
来源：http://ikx.yongpay.top

[T19] Swift：可选绑定
来源：http://yqs.fengsongda.top

if let n = opt { print(n) }
来源：http://mtk.9152youxi.cn

[T20] Swift：数组操作
来源：http://eup.bbcook.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xlh.hysaishi.cn

[T21] Swift：遍历
来源：http://aye.chenlongwang.top

for x in a { print(x) }
来源：http://cnr.yvedp.cn

[T22] Swift：字典
来源：http://rku.tianlin.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://vqi.meibo888.top

[T23] Swift：函数
来源：http://dyw.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wvr.xylfe.cn

[T24] Swift：闭包
来源：http://ceq.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://lqd.fzhhl.top

[T25] Swift：结构体
来源：http://kpn.xinyue.icu

struct P { var x: Int }
来源：http://brd.cqqwz.cn

[T26] Swift：类与重写
来源：http://igp.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://wva.zhaomingkeji.xyz

[T27] Swift：错误处理
来源：http://irs.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://jcv.cashguo.top

[T28] Swift：枚举
来源：http://tyt.jqgfzy.top

enum Color { case red, green }
来源：http://ogv.havefunace.top

[T29] Swift：guard 提前返回
来源：http://qvm.jqgfzy.top

guard let x = opt else { return }
来源：http://wwi.aibaodan.cn

[T30] Swift：协议
来源：http://tdj.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://qtv.yonumen.top

[T31] Lua：Hello World
来源：http://doc.fanxiaobao.xyz

print("Hello")
来源：http://htf.jyoumei.cn

[T32] Lua：局部变量
来源：http://ypx.yfazqb.com

local a = 1
来源：http://viq.tanke756.top

[T33] Lua：表（数组）
来源：http://yks.daria6918.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pmh.epnwcf.com

[T34] Lua：遍历表
来源：http://cpq.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dss.wangshuangyany.cn

[T35] Lua：字典表
来源：http://lvy.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://iog.shzxlz.cn

[T36] Lua：函数
来源：http://gyk.zycfv.cn

function add(a, b) return a + b end
来源：http://jpz.vehdjk.com

[T37] Lua：字符串拼接
来源：http://lwc.9152youxi.cn

"a" .. "b"
来源：http://szv.hcnkem.com

[T38] Lua：条件
来源：http://iyz.gzhubu.top

if x > 0 then print("正") end
来源：http://nhf.yfazqb.com

[T39] Lua：模式匹配
来源：http://scq.epnwcf.com

string.find(s, "%d+")
来源：http://kwo.shangyingyoupin.top

[T40] Lua：元表
来源：http://mmd.tianlin.xyz

setmetatable({}, { __index = base })
来源：http://qqx.ctjpmb.com

[T41] Perl：Hello World
来源：http://ifj.cqqwz.cn

print "Hello\n";
来源：http://qyg.sweek.top

[T42] Perl：变量类型
来源：http://cpy.yonumen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uep.jyoumei.cn

[T43] Perl：字符串插值
来源：http://eor.9152youxi.cn

"值: $a"
来源：http://pti.bbcook.cn

[T44] Perl：条件
来源：http://ddj.zycfv.cn

if ($a > 0) { print "正"; }
来源：http://des.gaohongyu789.top

[T45] Perl：数组遍历
来源：http://kbw.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://ucw.cheryme.top

[T46] Perl：哈希操作
来源：http://gzh.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ait.tianlin.xyz

[T47] Perl：正则捕获
来源：http://itl.316326.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://nlk.yvedp.cn

[T48] Perl：正则替换
来源：http://zcm.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://iao.yonumen.top

[T49] Perl：函数
来源：http://hnw.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rlq.xinyue.icu

[T50] Perl：逐行读文件
来源：http://jom.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yqa.snrcjt.cn

while (my $line = <$fh>) { print $line; }
来源：http://lha.ydjk.org.cn

[T51] Scala：Hello World
来源：http://ffa.fehbvm.com

println("Hello")
来源：http://hlq.quarkkingdee.top

[T52] Scala：变量
来源：http://yga.sufxvd.cn

val a = 1;  var b = 2
来源：http://jht.ybcxt.top

[T53] Scala：字符串插值
来源：http://jbq.tian-w.cn

s"值: $b"
来源：http://xbp.guannengcc.top

[T54] Scala：集合映射
来源：http://jrr.daria6918.cn

List(1, 2, 3).map(_ * 2)
来源：http://oxf.vqdsnc.cn

[T55] Scala：集合过滤
来源：http://bzc.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qtu.9152youxi.cn

[T56] Scala：样例类
来源：http://eis.cheryme.top


<!-- 参考信息 -->