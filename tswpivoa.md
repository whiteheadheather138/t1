代发 wailian999

ssh user@host 'uptime'
来源：http://asc.nanxinkj.top

[R58] 下载文件
来源：http://yhg.ppjwa.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nib.hysaishi.cn

[R59] 发 POST JSON
来源：http://ccl.sufxvd.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hmz.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://gsm.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jrx.cashguo.top

[R61] 磁盘占用
来源：http://qmw.cqqwz.cn

df -h;  du -sh *
来源：http://vbr.zhengqikj.top

[R62] 找最占空间的文件
来源：http://sns.jyoumei.cn

du -ah . | sort -rh | head -10
来源：http://tcz.shangyingyoupin.top

[R63] 内存与进程
来源：http://tqt.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://skj.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://tpp.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://aoy.uphjek.com

[R65] 查看端口占用
来源：http://cfi.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xha.gaohongyu789.top

[R66] 定时任务
来源：http://pgx.zhixingplan.top

crontab -e;  crontab -l
来源：http://qtt.jianghu66.top

[R67] 生成随机十六进制串
来源：http://rzs.sweek.top

openssl rand -hex 16
来源：http://sfs.gzhubu.top

[R68] 计算文件校验值
来源：http://hxa.shanyushiyangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://pjo.redwolf501.top

[R69] 生成随机密码
来源：http://wyl.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://pzg.hongshengwenyu.top

[R70] 时间戳与互转
来源：http://gcx.zhongyouzk.top

date +%s;  date -d @1700000000
来源：http://kgi.dashuyun.cn

[R71] 日期格式化
来源：http://iks.pycfn.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://fur.guannengcc.top

[R72] 等待端口就绪
来源：http://jlj.hywenlv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gxe.haohaochexian.top

[R73] 分割大日志
来源：http://acv.chenzaomai.com

split -l 1000 big.log part_
来源：http://vci.yanxiufei.cn

[R74] 批量重命名
来源：http://uyu.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hys.hfpthk.cn

[R75] 导出环境变量
来源：http://seq.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://nkw.zhixingplan.top

[R76] 使用临时文件
来源：http://obb.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nqi.epnwcf.com

[R77] 读取用户输入
来源：http://wco.zycfv.cn

read -rp "请输入: " ans
来源：http://kar.aizwys.cn

[R78] 交互式菜单
来源：http://ruk.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qlv.tanke756.top

[R79] 解析命令行选项
来源：http://eda.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kqm.gogol.net.cn

[R80] 查看脚本执行耗时
来源：http://kjy.cqqwz.cn

time ./run.sh
来源：http://ebk.cdnleiting.top

================================================================================
来源：http://kko.ivvv.top

S. C / C++ 专题
来源：http://stx.cucudq.cn

================================================================================
来源：http://rgq.iojbl.cn

[S01] C：Hello World
来源：http://thb.nanxinkj.top

#include <stdio.h>
来源：http://ivy.52xcode.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qam.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://rla.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://yqn.xylfe.cn

[S03] C：读入整数
来源：http://elq.nanxuanxn.top

int x; scanf("%d", &x);
来源：http://ulq.wangdashe.top

[S04] C：字符串复制
来源：http://kxy.ydjk.org.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xfz.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://oqt.hongshengwenyu.top

strlen(s)
来源：http://bsj.fktsv.cn

[S06] C：字符串比较
来源：http://ogp.hnxiangtu.top

strcmp(a, b) == 0
来源：http://sav.aibaodan.cn

[S07] C：数组遍历求和
来源：http://syp.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vwt.jlsjyb.cn

[S08] C：动态内存分配与释放
来源：http://uzp.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nga.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://wjt.jinyuanbaomall.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aqp.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://lyd.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://xey.sjlbkw.cn

[S11] C：逐行读文件
来源：http://byn.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://uml.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rqt.sjlbkw.cn

fclose(f);
来源：http://vea.yj202588.top

[S12] C：写文件
来源：http://jfi.bbcook.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vwh.jinqigfzy.top

[S13] C：宏定义
来源：http://vfv.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eyj.cdnleiting.top

[S14] C：枚举
来源：http://ctm.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://ksm.zhoulong.xyz

[S15] C：类型转换
来源：http://rft.kuanghao11.cn

(double) a / b
来源：http://upu.jqgufenzy.top

[S16] C：位操作置位
来源：http://wws.nanxinkj.top

x |= (1 << 3);
来源：http://ble.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://zxp.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xxr.xziqi.cn

[S18] C：命令行参数
来源：http://nnb.aizwys.cn

int main(int argc, char **argv)
来源：http://bzf.epnwcf.com

[S19] C：快速排序
来源：http://nli.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://qjj.aibaodan.cn

[S20] C：二分查找
来源：http://dys.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ejf.tanke756.top

[S21] C：字符类别判断
来源：http://tfg.andypj.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nbv.xinyue.icu

[S22] C：字符串转数字
来源：http://ldk.zdbjq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uik.jqgfzy.top

[S23] C：随机数
来源：http://otp.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://urf.yongpay.top

[S24] C：获取本地时间
来源：http://opx.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ryt.yonumen.top

[S25] C：内存拷贝
来源：http://ghv.sweek.top

memcpy(dst, src, n);
来源：http://vju.jyoumei.cn

[S26] C：内存清零
来源：http://jzk.redwolf501.top

memset(a, 0, sizeof a);
来源：http://jps.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://tty.zhongyouzk.top

const double PI = 3.14159;
来源：http://pjf.jyoumei.cn

[S28] C：静态变量
来源：http://lzl.xuetiantiany.cn

static int counter = 0;
来源：http://phy.wangdashe.top

[S29] C：变参函数
来源：http://mdp.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wid.52xcode.cn

[S30] C：头文件保护
来源：http://fry.cashguo.top

#ifndef X_H
来源：http://swd.ydzc1.top

#define X_H
来源：http://wul.xylfe.cn

#endif
来源：http://lxb.zhengqikj.top

[S31] C++：Hello World
来源：http://kez.hammf.cn

#include <iostream>
来源：http://euj.shzxlz.cn

int main() { std::cout << "Hello\n"; }
来源：http://dep.nanxuanxn.top

[S32] C++：字符串
来源：http://qjw.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://xjb.ybcxt.top

[S33] C++：vector 增删
来源：http://mbw.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uuq.yonumen.top

[S34] C++：遍历 vector
来源：http://ihk.kuanghao11.cn

for (auto &x : v) { std::cout << x; }
来源：http://uqh.guannengcc.top

[S35] C++：map
来源：http://yak.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nzw.9152youxi.cn

[S36] C++：unordered_map
来源：http://xdm.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uco.hysaishi.cn

[S37] C++：set
来源：http://qxm.snrcjt.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bks.yj202588.top

[S38] C++：排序
来源：http://din.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://dcx.nanxinkj.top

[S39] C++：自定义比较器排序
来源：http://oaa.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zoz.xziqi.cn

[S40] C++：查找元素
来源：http://qzm.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pqm.yj20258.top

[S41] C++：类与构造函数
来源：http://cgf.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gvb.smart0.xyz

[S42] C++：继承与虚函数
来源：http://dpw.xziqi.cn

class B : public Base { public: void f() override {} };
来源：http://lhh.cucudq.cn

[S43] C++：智能指针
来源：http://lxf.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://jag.yuanzhike.top

[S44] C++：引用传参
来源：http://irl.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://wym.ehwqpu.com

[S45] C++：lambda
来源：http://onv.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://xof.dashuyun.cn

[S46] C++：函数模板
来源：http://xse.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://chb.nanxuanxn.top

[S47] C++：结构化绑定遍历
来源：http://jfm.zdqjudy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zhe.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://cup.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://tbq.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://iru.zdqjudy.top

[S49] C++：写文件
来源：http://hur.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rvc.jlsjyb.cn

[S50] C++：格式化数字
来源：http://iib.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pua.tian-w.cn

[S51] C++：显式类型转换
来源：http://bfo.52xcode.cn

static_cast<double>(a) / b
来源：http://uct.316326.xyz

[S52] C++：const 与 noexcept
来源：http://puo.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://fdh.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://len.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://zjo.gaohongyu789.top

[S54] C++：异常处理
来源：http://kyi.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nqj.yj202588.top

[S55] C++：结构化绑定
来源：http://uqm.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lna.tarul.cn

[S56] C++：optional
来源：http://ujq.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xqp.hywenlv.cn

[S57] C++：编译期常量
来源：http://xgq.yangfankeji.com

constexpr int N = 10;
来源：http://bou.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://gan.yuxming.cn

namespace ns { int f() { return 1; } }
来源：http://cha.cqqwz.cn

[S59] C++：静态断言
来源：http://rnl.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ers.shzxlz.cn

[S60] C++：遍历并删除元素
来源：http://rti.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ene.iojbl.cn

================================================================================
来源：http://hww.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xll.ctjpmb.com

================================================================================
来源：http://dvz.yonumen.top

[T01] Kotlin：Hello World
来源：http://mox.andypj.xyz

println("Hello")
来源：http://hix.gzhubu.top

[T02] Kotlin：变量
来源：http://unh.meibo888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vfl.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://kdy.hnxiangtu.top

"值: $b"
来源：http://zrd.gotoacloud.top

[T04] Kotlin：空安全
来源：http://lyf.hfpthk.cn

val n: String? = null;  n?.length
来源：http://qhm.birdmap.top

[T05] Kotlin：when 表达式
来源：http://orr.meibo888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aud.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://ieb.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://vyq.yj20258.top

[T07] Kotlin：集合过滤
来源：http://wiw.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hpq.yvedp.cn

[T08] Kotlin：数据类
来源：http://trb.shanyushiyangtech.top

data class User(val name: String, val age: Int)
来源：http://xpn.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://oky.hammf.cn

fun String.exclaim() = this + "!"
来源：http://dju.nanxinkj.top

[T10] Kotlin：默认参数
来源：http://anp.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fca.xylfe.cn

[T11] Kotlin：协程
来源：http://jlt.yongpay.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tej.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://smc.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://jcg.0kj1m.cn

[T13] Kotlin：只读 Map
来源：http://jdw.sufxvd.cn

val m = mapOf("a" to 1)
来源：http://pcf.pycfn.com

[T14] Kotlin：循环
来源：http://rzc.hcnkem.com

for (i in 1..10) println(i)
来源：http://cnu.yonumen.top

[T15] Kotlin：接口
来源：http://ihf.ydzc1.top

interface Shape { fun area(): Double }
来源：http://kwq.meibo888.top

[T16] Swift：Hello World
来源：http://txh.uphjek.com

print("Hello")
来源：http://zks.bjfxy.top

[T17] Swift：变量与常量
来源：http://jnb.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://vux.jqgfzy.top

[T18] Swift：字符串插值
来源：http://rkv.tianlin.xyz

"值: \(b)"
来源：http://fds.shzxlz.cn

[T19] Swift：可选绑定
来源：http://ufp.dashuyun.cn

if let n = opt { print(n) }
来源：http://qyl.ppjwa.cn

[T20] Swift：数组操作
来源：http://tse.yuxming.cn

var a = [1, 2, 3];  a.append(4)
来源：http://boo.gaohongyu789.top

[T21] Swift：遍历
来源：http://pbl.jqgfzy.top

for x in a { print(x) }
来源：http://swj.svipenyu.cn

[T22] Swift：字典
来源：http://yer.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vpd.wangshuangyany.cn

[T23] Swift：函数
来源：http://pzt.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mph.xuanzx.com

[T24] Swift：闭包
来源：http://vlz.sysykeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://edg.yanxiufei.cn

[T25] Swift：结构体
来源：http://yld.hammf.cn

struct P { var x: Int }
来源：http://whx.iojbl.cn

[T26] Swift：类与重写
来源：http://pyd.nwbrower.top

class A: Base { override func f() {} }
来源：http://rpx.nanxuanxn.top

[T27] Swift：错误处理
来源：http://ual.yj20258888.top

do { try f() } catch { print(error) }
来源：http://elz.cdnleiting.top

[T28] Swift：枚举
来源：http://tpy.bbcook.cn

enum Color { case red, green }
来源：http://tth.fzhhl.top

[T29] Swift：guard 提前返回
来源：http://wbl.jqgufenzy.top

guard let x = opt else { return }
来源：http://zsx.meibo888.top

[T30] Swift：协议
来源：http://jtz.pycfn.com

protocol Shape { func area() -> Double }
来源：http://kvx.daria6918.cn

[T31] Lua：Hello World
来源：http://gnh.yfazqb.com

print("Hello")
来源：http://apv.cucudq.cn

[T32] Lua：局部变量
来源：http://vgt.uphjek.com

local a = 1
来源：http://dmz.yvedp.cn

[T33] Lua：表（数组）
来源：http://jza.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://tls.fengsongda.top

[T34] Lua：遍历表
来源：http://row.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rve.ehwqpu.com

[T35] Lua：字典表
来源：http://qrh.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://kay.zhixingplan.top

[T36] Lua：函数
来源：http://brd.ppjwa.cn

function add(a, b) return a + b end
来源：http://pqo.sufxvd.cn

[T37] Lua：字符串拼接
来源：http://jbx.shzxlz.cn

"a" .. "b"
来源：http://hzj.fzhhl.top

[T38] Lua：条件
来源：http://udk.hesvh.cn

if x > 0 then print("正") end
来源：http://onk.jyoumei.cn

[T39] Lua：模式匹配
来源：http://gsr.fzhhl.top

string.find(s, "%d+")
来源：http://tqn.guowangkeji.top

[T40] Lua：元表
来源：http://jyo.vehdjk.com

setmetatable({}, { __index = base })
来源：http://ssi.yuxming.cn

[T41] Perl：Hello World
来源：http://hay.shanyushiyangkeji.top

print "Hello\n";
来源：http://pty.zdbjq.cn

[T42] Perl：变量类型
来源：http://rrv.hongshengwenyu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kvn.zycfv.cn

[T43] Perl：字符串插值
来源：http://tnc.gogol.net.cn

"值: $a"
来源：http://udw.chenzaomai.com

[T44] Perl：条件
来源：http://dzy.tarul.cn

if ($a > 0) { print "正"; }
来源：http://ciy.feifeiyinyue.top

[T45] Perl：数组遍历
来源：http://hka.uphjek.com

for my $x (@arr) { print $x; }
来源：http://mcz.havefunace.top

[T46] Perl：哈希操作
来源：http://hnh.haohaochexian.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ydi.cashguo.top

[T47] Perl：正则捕获
来源：http://hfh.ivvv.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rzh.snrcjt.cn

[T48] Perl：正则替换
来源：http://hvk.yangfankeji.com

$s =~ s/old/new/g;
来源：http://zwp.xinyue.icu

[T49] Perl：函数
来源：http://ajj.yueranfly.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wxz.hfpthk.cn

[T50] Perl：逐行读文件
来源：http://jdp.zhengqikj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xpe.sysykeji.top

while (my $line = <$fh>) { print $line; }
来源：http://rxt.cheryme.top

[T51] Scala：Hello World
来源：http://iqu.zhoulong.xyz

println("Hello")
来源：http://til.quarkkingdee.top

[T52] Scala：变量
来源：http://oak.svipenyu.cn

val a = 1;  var b = 2
来源：http://owg.jianghu66.top

[T53] Scala：字符串插值
来源：http://qvk.yj202588.top

s"值: $b"
来源：http://yzf.gaohongyu789.top

[T54] Scala：集合映射
来源：http://csx.pycfn.com

List(1, 2, 3).map(_ * 2)
来源：http://dai.zhengqikj.top

[T55] Scala：集合过滤
来源：http://tpi.sufxvd.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wfn.shzxlz.cn

[T56] Scala：样例类
来源：http://urh.sxryk.cn

case class User(name: String, age: Int)
来源：http://ozd.dianchejie.cn

[T57] Scala：模式匹配
来源：http://knw.0kj1m.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hti.xuanzx.com

[T58] Scala：函数定义
来源：http://wyn.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://wxa.hongshengwenyu.top

[T59] Scala：循环
来源：http://aiq.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://rcb.fengsongda.top

[T60] Scala：折叠
来源：http://vfw.gotoacloud.top


<!-- 参考信息 -->