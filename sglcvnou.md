代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fnd.jqgufenzy.top

[R56] 远程拷贝
来源：http://kcw.jianghu66.top

scp file user@host:/path/
来源：http://cfl.tianlin.xyz

[R57] 远程执行命令
来源：http://hot.tian-w.cn

ssh user@host 'uptime'
来源：http://jlu.nanxuanxn.top

[R58] 下载文件
来源：http://uhb.jqgufenzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zqp.havefunace.top

[R59] 发 POST JSON
来源：http://xvy.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pcb.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://ugo.jianghu66.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://agq.andypj.xyz

[R61] 磁盘占用
来源：http://rpk.yuanzhike.top

df -h;  du -sh *
来源：http://jtn.tanke756.top

[R62] 找最占空间的文件
来源：http://pvs.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://mzf.jlsjyb.cn

[R63] 内存与进程
来源：http://wxl.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://nhe.meibo888.top

[R64] 结束进程
来源：http://fhe.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://kpt.jinqigfzy.top

[R65] 查看端口占用
来源：http://egk.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://amt.aibaodan.cn

[R66] 定时任务
来源：http://vrk.9152youxi.cn

crontab -e;  crontab -l
来源：http://ldu.jyoumei.cn

[R67] 生成随机十六进制串
来源：http://wzs.zhongyouzk.top

openssl rand -hex 16
来源：http://tpr.yj202588.top

[R68] 计算文件校验值
来源：http://hnh.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://rrn.daxiang520.top

[R69] 生成随机密码
来源：http://onb.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://sqb.bjfxy.top

[R70] 时间戳与互转
来源：http://bkr.aibaodan.cn

date +%s;  date -d @1700000000
来源：http://shi.bjfxy.top

[R71] 日期格式化
来源：http://lii.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nqa.xuanzx.com

[R72] 等待端口就绪
来源：http://cpa.cheryme.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qov.yangfankeji.com

[R73] 分割大日志
来源：http://aca.meibo888.top

split -l 1000 big.log part_
来源：http://wuq.zdqjudy.top

[R74] 批量重命名
来源：http://gey.ppjwa.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xpo.yueranfly.top

[R75] 导出环境变量
来源：http://vpp.hcnkem.com

export PATH="$HOME/bin:$PATH"
来源：http://zzg.yj20258.top

[R76] 使用临时文件
来源：http://mon.nanxinkj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ogp.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://xqd.hfpthk.cn

read -rp "请输入: " ans
来源：http://zoo.jyoumei.cn

[R78] 交互式菜单
来源：http://xyt.bjfxy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bfj.yuxming.cn

[R79] 解析命令行选项
来源：http://ypf.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zvc.sxryk.cn

[R80] 查看脚本执行耗时
来源：http://nws.yuanzhike.top

time ./run.sh
来源：http://wra.shangyingyoupin.top

================================================================================
来源：http://lcc.c1oappe.top

S. C / C++ 专题
来源：http://bkh.zhixingplan.top

================================================================================
来源：http://mlc.yueranfly.top

[S01] C：Hello World
来源：http://ffh.yuanzhike.top

#include <stdio.h>
来源：http://atd.gzhubu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zmu.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://ozx.fengsongda.top

int a = 10; printf("%d\n", a);
来源：http://nhf.tarul.cn

[S03] C：读入整数
来源：http://ojz.aibaodan.cn

int x; scanf("%d", &x);
来源：http://zmn.yonumen.top

[S04] C：字符串复制
来源：http://gku.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zgt.birdmap.top

[S05] C：字符串长度
来源：http://edk.gogol.net.cn

strlen(s)
来源：http://nha.hywenlv.cn

[S06] C：字符串比较
来源：http://lfl.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://uoo.tianlin.xyz

[S07] C：数组遍历求和
来源：http://xnk.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wkq.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://ywt.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ufs.feifeiyinyue.top

[S09] C：结构体定义与初始化
来源：http://kuc.yj202588.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://shx.iojbl.cn

[S10] C：指针与解引用
来源：http://dez.cheryme.top

int *p = &a;  *p = 5;
来源：http://too.c1oappe.top

[S11] C：逐行读文件
来源：http://eqv.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://doj.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://key.sufxvd.cn

fclose(f);
来源：http://exs.fanxiaobao.xyz

[S12] C：写文件
来源：http://agk.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ehh.9152youxi.cn

[S13] C：宏定义
来源：http://mhk.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pku.hfpthk.cn

[S14] C：枚举
来源：http://utl.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://gnm.jiagoushi.top

[S15] C：类型转换
来源：http://zxc.xziqi.cn

(double) a / b
来源：http://keq.0kj1m.cn

[S16] C：位操作置位
来源：http://lux.aizwys.cn

x |= (1 << 3);
来源：http://zpf.sjlbkw.cn

[S17] C：安全拼接字符串
来源：http://buc.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wfi.tarul.cn

[S18] C：命令行参数
来源：http://wlg.xuanzx.com

int main(int argc, char **argv)
来源：http://tne.tarul.cn

[S19] C：快速排序
来源：http://kuf.shuidangran.top

qsort(a, n, sizeof(int), cmp);
来源：http://ngf.zdbjq.cn

[S20] C：二分查找
来源：http://pwn.svipenyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kom.yanxiufei.cn

[S21] C：字符类别判断
来源：http://hnu.gotoacloud.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jap.sweek.top

[S22] C：字符串转数字
来源：http://xhe.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cyu.chenzaomai.com

[S23] C：随机数
来源：http://dac.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fau.jlsjyb.cn

[S24] C：获取本地时间
来源：http://div.yj202588.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pqo.dianchejie.cn

[S25] C：内存拷贝
来源：http://ufd.jyoumei.cn

memcpy(dst, src, n);
来源：http://wdy.aizwys.cn

[S26] C：内存清零
来源：http://bzm.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://fgu.gaohongyu789.top

[S27] C：定义常量
来源：http://hzv.jqgufenzy.top

const double PI = 3.14159;
来源：http://okr.havefunace.top

[S28] C：静态变量
来源：http://mle.jqgufenzy.top

static int counter = 0;
来源：http://vpg.snrcjt.cn

[S29] C：变参函数
来源：http://lgd.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xvt.yfazqb.com

[S30] C：头文件保护
来源：http://axr.jqgfzy.top

#ifndef X_H
来源：http://onq.shzxlz.cn

#define X_H
来源：http://avr.yangfankeji.com

#endif
来源：http://lzj.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://yuf.wangdashe.top

#include <iostream>
来源：http://sit.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://rxb.c1oappe.top

[S32] C++：字符串
来源：http://que.cashguo.top

std::string s = "hi";  s += "!";
来源：http://zxf.daria6918.cn

[S33] C++：vector 增删
来源：http://mlc.sysykeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://exz.tanke756.top

[S34] C++：遍历 vector
来源：http://vfi.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://khv.jiagoushi.top

[S35] C++：map
来源：http://mkd.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kih.ctjpmb.com

[S36] C++：unordered_map
来源：http://qhp.shanyushiyangtech.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lcv.nanxinkj.top

[S37] C++：set
来源：http://cwn.fehbvm.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://urg.yongpay.top

[S38] C++：排序
来源：http://miy.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://fem.dianchejie.cn

[S39] C++：自定义比较器排序
来源：http://pqr.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xyd.yuanzhike.top

[S40] C++：查找元素
来源：http://wch.ydjk.org.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fwz.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://fkn.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://scx.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://gbr.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://qkg.jyoumei.cn

[S43] C++：智能指针
来源：http://tmr.guannengcc.top

auto p = std::make_unique<int>(5);
来源：http://rgu.dianchejie.cn

[S44] C++：引用传参
来源：http://bfg.iojbl.cn

void inc(int &x) { ++x; }
来源：http://hbe.uphjek.com

[S45] C++：lambda
来源：http://dlf.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kec.c1oappe.top

[S46] C++：函数模板
来源：http://pek.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xdt.cucudq.cn

[S47] C++：结构化绑定遍历
来源：http://iaq.ywan-chungtsiang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dco.yonumen.top

[S48] C++：逐行读文件
来源：http://ktv.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://bdn.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://pll.daxiang520.top

[S49] C++：写文件
来源：http://kas.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://frm.nanxinkj.top

[S50] C++：格式化数字
来源：http://hes.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bdm.snrcjt.cn

[S51] C++：显式类型转换
来源：http://ahr.fzhhl.top

static_cast<double>(a) / b
来源：http://vyn.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://qol.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://jkt.dashuyun.cn

[S53] C++：移动语义
来源：http://umi.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://fmn.yuxming.cn

[S54] C++：异常处理
来源：http://hcj.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iww.andypj.xyz

[S55] C++：结构化绑定
来源：http://mou.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ram.uphjek.com

[S56] C++：optional
来源：http://rdn.pycfn.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jje.0kj1m.cn

[S57] C++：编译期常量
来源：http://eze.hysaishi.cn

constexpr int N = 10;
来源：http://ccr.yanxiufei.cn

[S58] C++：命名空间
来源：http://keo.yuxming.cn

namespace ns { int f() { return 1; } }
来源：http://xrr.zhijiandao.cn

[S59] C++：静态断言
来源：http://mbt.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hgg.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://kvh.yj20258.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gxh.zhengqikj.top

================================================================================
来源：http://mzp.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nqw.havefunace.top

================================================================================
来源：http://ntw.wangdashe.top

[T01] Kotlin：Hello World
来源：http://gux.sysykeji.top

println("Hello")
来源：http://krh.zhijiandao.cn

[T02] Kotlin：变量
来源：http://fsk.nanxinkj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ijb.havefunace.top

[T03] Kotlin：字符串模板
来源：http://ssy.sweek.top

"值: $b"
来源：http://yyn.havefunace.top

[T04] Kotlin：空安全
来源：http://nwg.jiagoushi.top

val n: String? = null;  n?.length
来源：http://bxs.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://vuh.feifeiyinyue.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qjp.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://cuq.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jro.gzhubu.top

[T07] Kotlin：集合过滤
来源：http://ahs.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://eqs.shangyingyoupin.top

[T08] Kotlin：数据类
来源：http://wxt.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://qyl.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://ksd.ybcxt.top

fun String.exclaim() = this + "!"
来源：http://nqn.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://mnk.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nvg.xziqi.cn

[T11] Kotlin：协程
来源：http://vzo.uphjek.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://dsy.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://npl.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://jxs.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://vkp.xuanzx.com

val m = mapOf("a" to 1)
来源：http://unp.xziqi.cn

[T14] Kotlin：循环
来源：http://gra.hammf.cn

for (i in 1..10) println(i)
来源：http://uzq.jyoumei.cn

[T15] Kotlin：接口
来源：http://ekh.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://sad.chenlongwang.top

[T16] Swift：Hello World
来源：http://ior.zhijiandao.cn

print("Hello")
来源：http://avb.andypj.xyz

[T17] Swift：变量与常量
来源：http://rhm.sufxvd.cn

var a = 1;  let b = 2
来源：http://bxc.9152youxi.cn

[T18] Swift：字符串插值
来源：http://qkt.jinghuilouyu.cn

"值: \(b)"
来源：http://uaz.havefunace.top

[T19] Swift：可选绑定
来源：http://fei.0kj1m.cn

if let n = opt { print(n) }
来源：http://nyx.zhoulong.xyz

[T20] Swift：数组操作
来源：http://fyz.hysaishi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fiw.jqgfzy.top

[T21] Swift：遍历
来源：http://lyl.ybcxt.top

for x in a { print(x) }
来源：http://gdc.zdbjq.cn

[T22] Swift：字典
来源：http://zcs.tianlin.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://rtd.gotoacloud.top

[T23] Swift：函数
来源：http://dhv.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zrq.hesvh.cn

[T24] Swift：闭包
来源：http://bax.fzhhl.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://okf.c1oappe.top

[T25] Swift：结构体
来源：http://wxn.chenzaomai.com

struct P { var x: Int }
来源：http://xpf.ppjwa.cn

[T26] Swift：类与重写
来源：http://pbd.jinqigufen.top

class A: Base { override func f() {} }
来源：http://led.ctjpmb.com

[T27] Swift：错误处理
来源：http://qxl.yj202588.top

do { try f() } catch { print(error) }
来源：http://hlk.zycfv.cn

[T28] Swift：枚举
来源：http://sso.iojbl.cn

enum Color { case red, green }
来源：http://yjz.hammf.cn

[T29] Swift：guard 提前返回
来源：http://zgk.smart0.xyz

guard let x = opt else { return }
来源：http://obe.pengpengdd.cyou

[T30] Swift：协议
来源：http://ite.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://wst.chenlongwang.top

[T31] Lua：Hello World
来源：http://mvd.9152youxi.cn

print("Hello")
来源：http://hyg.snrcjt.cn

[T32] Lua：局部变量
来源：http://pky.tanke756.top

local a = 1
来源：http://xln.sxryk.cn

[T33] Lua：表（数组）
来源：http://hnj.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://kvz.hywenlv.cn

[T34] Lua：遍历表
来源：http://kzp.feifeiyinyue.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xzd.havefunace.top

[T35] Lua：字典表
来源：http://wwi.zdqjudy.top

local d = { a = 1 };  d.b = 2
来源：http://tns.nanxuanxn.top

[T36] Lua：函数
来源：http://zlo.yueranfly.top

function add(a, b) return a + b end
来源：http://vxm.xziqi.cn

[T37] Lua：字符串拼接
来源：http://vfc.daria6918.cn

"a" .. "b"
来源：http://sfv.sufxvd.cn

[T38] Lua：条件
来源：http://rum.xingfuxueyuan.xyz

if x > 0 then print("正") end
来源：http://pms.ctjpmb.com

[T39] Lua：模式匹配
来源：http://pys.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://hxe.dianchejie.cn

[T40] Lua：元表
来源：http://qta.zhongyouzk.top

setmetatable({}, { __index = base })
来源：http://pii.svipenyu.cn

[T41] Perl：Hello World
来源：http://ops.jyoumei.cn

print "Hello\n";
来源：http://uau.ehwqpu.com

[T42] Perl：变量类型
来源：http://sxp.daria6918.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sqf.xingfuxueyuan.xyz

[T43] Perl：字符串插值
来源：http://uqh.hnxiangtu.top

"值: $a"
来源：http://amw.jiagoushi.top

[T44] Perl：条件
来源：http://fbs.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://vod.xinyue.icu

[T45] Perl：数组遍历
来源：http://brk.ywan-chungtsiang.top

for my $x (@arr) { print $x; }
来源：http://rux.haohaochexian.top

[T46] Perl：哈希操作
来源：http://enr.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zxm.ehwqpu.com

[T47] Perl：正则捕获
来源：http://exj.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pxp.jyoumei.cn

[T48] Perl：正则替换
来源：http://kvi.sufxvd.cn

$s =~ s/old/new/g;
来源：http://tsr.jinqigfzy.top

[T49] Perl：函数
来源：http://zpg.pycfn.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kev.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://ikm.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bmj.snrcjt.cn

while (my $line = <$fh>) { print $line; }
来源：http://mvt.daxiang520.top

[T51] Scala：Hello World
来源：http://sji.hesvh.cn

println("Hello")
来源：http://ooq.andypj.xyz

[T52] Scala：变量
来源：http://jqn.hesvh.cn

val a = 1;  var b = 2
来源：http://bnp.hfpthk.cn

[T53] Scala：字符串插值
来源：http://may.vehdjk.com

s"值: $b"
来源：http://qlh.yongpay.top

[T54] Scala：集合映射
来源：http://xzv.ppjwa.cn

List(1, 2, 3).map(_ * 2)
来源：http://afl.c1oappe.top

[T55] Scala：集合过滤
来源：http://ypc.zhengqikj.top

List(1, 2, 3).filter(_ > 1)
来源：http://ncg.hywenlv.cn

[T56] Scala：样例类
来源：http://pkm.xylfe.cn

case class User(name: String, age: Int)
来源：http://dnx.gzhubu.top

[T57] Scala：模式匹配
来源：http://gxn.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://umx.52xcode.cn

[T58] Scala：函数定义
来源：http://zit.yanxiufei.cn


<!-- 参考信息 -->