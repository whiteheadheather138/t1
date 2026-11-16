代发 wailian999

ssh user@host 'uptime'
来源：http://muz.shanyushiyangtech.top

[R58] 下载文件
来源：http://zge.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://evc.shzxlz.cn

[R59] 发 POST JSON
来源：http://nlk.shzxlz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://npz.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://vcc.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dqk.svipenyu.cn

[R61] 磁盘占用
来源：http://cbl.52xcode.cn

df -h;  du -sh *
来源：http://jih.bjfxy.top

[R62] 找最占空间的文件
来源：http://gbl.birdmap.top

du -ah . | sort -rh | head -10
来源：http://mpu.redwolf501.top

[R63] 内存与进程
来源：http://lfl.zhengqikj.top

free -h;  ps aux | grep nginx
来源：http://tlq.hfpthk.cn

[R64] 结束进程
来源：http://jcg.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://anw.vqdsnc.cn

[R65] 查看端口占用
来源：http://yhu.feifeiyinyue.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oxi.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://pmf.fengsongda.top

crontab -e;  crontab -l
来源：http://qff.gzhubu.top

[R67] 生成随机十六进制串
来源：http://vbe.hammf.cn

openssl rand -hex 16
来源：http://kvq.gotoacloud.top

[R68] 计算文件校验值
来源：http://eis.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dnv.zdqjudy.top

[R69] 生成随机密码
来源：http://vjj.snrcjt.cn

head -c 16 /dev/urandom | base64
来源：http://xog.gaohongyu789.top

[R70] 时间戳与互转
来源：http://idm.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://vlv.shuidangran.top

[R71] 日期格式化
来源：http://qaa.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://lqo.bjfxy.top

[R72] 等待端口就绪
来源：http://wap.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oxn.zhiwuduotai.top

[R73] 分割大日志
来源：http://uhu.cucudq.cn

split -l 1000 big.log part_
来源：http://gyk.zhiwuduotai.top

[R74] 批量重命名
来源：http://mjd.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iwv.tian-w.cn

[R75] 导出环境变量
来源：http://sdb.316326.xyz

export PATH="$HOME/bin:$PATH"
来源：http://sys.chenzaomai.com

[R76] 使用临时文件
来源：http://pap.jlsjyb.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ptr.vqdsnc.cn

[R77] 读取用户输入
来源：http://fot.ppjwa.cn

read -rp "请输入: " ans
来源：http://yhj.hfpthk.cn

[R78] 交互式菜单
来源：http://urd.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fry.shzxlz.cn

[R79] 解析命令行选项
来源：http://luf.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lbt.gzhubu.top

[R80] 查看脚本执行耗时
来源：http://fln.hammf.cn

time ./run.sh
来源：http://eon.vehdjk.com

================================================================================
来源：http://rhj.wangshuangyany.cn

S. C / C++ 专题
来源：http://tcu.ehwqpu.com

================================================================================
来源：http://pxi.epnwcf.com

[S01] C：Hello World
来源：http://yxq.shanyushiyangtech.top

#include <stdio.h>
来源：http://scb.xuanzx.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://jkw.fktsv.cn

[S02] C：变量与格式化输出
来源：http://xjk.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://tru.bjfxy.top

[S03] C：读入整数
来源：http://elm.sysykeji.top

int x; scanf("%d", &x);
来源：http://yzb.shuidangran.top

[S04] C：字符串复制
来源：http://fpk.tianlin.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://atp.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://pss.jianghu66.top

strlen(s)
来源：http://pmn.aizwys.cn

[S06] C：字符串比较
来源：http://wsx.sweek.top

strcmp(a, b) == 0
来源：http://hak.nwbrower.top

[S07] C：数组遍历求和
来源：http://jdh.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kcg.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://gri.hfpthk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dzx.hammf.cn

[S09] C：结构体定义与初始化
来源：http://frq.yangfankeji.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ham.jianghu66.top

[S10] C：指针与解引用
来源：http://wjg.vehdjk.com

int *p = &a;  *p = 5;
来源：http://bcu.yangfankeji.com

[S11] C：逐行读文件
来源：http://zhj.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://hzi.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mwo.chenjidiqi.icu

fclose(f);
来源：http://hsc.sjlbkw.cn

[S12] C：写文件
来源：http://pxr.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tde.tian-w.cn

[S13] C：宏定义
来源：http://hzn.cucudq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zkl.ydjk.org.cn

[S14] C：枚举
来源：http://fdl.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://ffk.uphjek.com

[S15] C：类型转换
来源：http://iwk.pycfn.com

(double) a / b
来源：http://hfs.jqgufenzy.top

[S16] C：位操作置位
来源：http://ptw.sysykeji.top

x |= (1 << 3);
来源：http://zhy.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://arj.fanxiaobao.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wrh.sxryk.cn

[S18] C：命令行参数
来源：http://lyk.bbcook.cn

int main(int argc, char **argv)
来源：http://mfh.wangdashe.top

[S19] C：快速排序
来源：http://ovl.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://jco.aizwys.cn

[S20] C：二分查找
来源：http://zjc.yuxming.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dqv.hfpthk.cn

[S21] C：字符类别判断
来源：http://unm.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vlk.uphjek.com

[S22] C：字符串转数字
来源：http://sfa.gaohongyu789.top

atoi("42");  strtod("3.14", NULL);
来源：http://vyp.yueranfly.top

[S23] C：随机数
来源：http://kds.ppjwa.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rcw.9152youxi.cn

[S24] C：获取本地时间
来源：http://iwa.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qzr.hysaishi.cn

[S25] C：内存拷贝
来源：http://bvy.mhx1999.top

memcpy(dst, src, n);
来源：http://okz.jinqigfzy.top

[S26] C：内存清零
来源：http://yxr.daria6918.cn

memset(a, 0, sizeof a);
来源：http://hfq.yuxming.cn

[S27] C：定义常量
来源：http://qqx.cucudq.cn

const double PI = 3.14159;
来源：http://jlq.9152youxi.cn

[S28] C：静态变量
来源：http://wyf.jinqigufen.top

static int counter = 0;
来源：http://ken.ehwqpu.com

[S29] C：变参函数
来源：http://zbw.dashuyun.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://caa.zycfv.cn

[S30] C：头文件保护
来源：http://yqq.zycfv.cn

#ifndef X_H
来源：http://jxb.yanxiufei.cn

#define X_H
来源：http://ohh.ydjk.org.cn

#endif
来源：http://zzq.xuanzx.com

[S31] C++：Hello World
来源：http://omv.tanke756.top

#include <iostream>
来源：http://gav.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://adl.xuetiantiany.cn

[S32] C++：字符串
来源：http://zus.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://zjt.aizwys.cn

[S33] C++：vector 增删
来源：http://csm.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://txr.fktsv.cn

[S34] C++：遍历 vector
来源：http://csg.mhx1999.top

for (auto &x : v) { std::cout << x; }
来源：http://ked.daria6918.cn

[S35] C++：map
来源：http://nkg.jianghu66.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://det.sysykeji.top

[S36] C++：unordered_map
来源：http://heq.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qza.svipenyu.cn

[S37] C++：set
来源：http://jsc.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wxa.fanxiaobao.xyz

[S38] C++：排序
来源：http://lhj.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://cfu.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://bwj.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qvb.guannengcc.top

[S40] C++：查找元素
来源：http://qim.ydzc1.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ozm.yuxming.cn

[S41] C++：类与构造函数
来源：http://ezh.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mft.ivvv.top

[S42] C++：继承与虚函数
来源：http://kyz.xuanzx.com

class B : public Base { public: void f() override {} };
来源：http://jcw.hammf.cn

[S43] C++：智能指针
来源：http://smg.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://hoz.jqgufenzy.top

[S44] C++：引用传参
来源：http://kmn.ydzc1.top

void inc(int &x) { ++x; }
来源：http://tas.9152youxi.cn

[S45] C++：lambda
来源：http://rbw.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://xgo.hcnkem.com

[S46] C++：函数模板
来源：http://rsc.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zwk.zhiwuduotai.top

[S47] C++：结构化绑定遍历
来源：http://lhe.fengsongda.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oda.nwbrower.top

[S48] C++：逐行读文件
来源：http://vvt.tianlin.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://hea.guannengcc.top

while (std::getline(in, line)) { }
来源：http://qtx.tarul.cn

[S49] C++：写文件
来源：http://srx.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://afn.zhoulong.xyz

[S50] C++：格式化数字
来源：http://dzn.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gbw.yangfankeji.com

[S51] C++：显式类型转换
来源：http://mlr.meibo888.top

static_cast<double>(a) / b
来源：http://ulh.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://tcu.yongpay.top

int size() const noexcept { return n_; }
来源：http://vsf.zdbjq.cn

[S53] C++：移动语义
来源：http://epn.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://wdz.zhengqikj.top

[S54] C++：异常处理
来源：http://mcp.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dqa.fengsongda.top

[S55] C++：结构化绑定
来源：http://emm.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://znz.cucudq.cn

[S56] C++：optional
来源：http://uhs.yangfankeji.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yhy.ydjk.org.cn

[S57] C++：编译期常量
来源：http://yfm.zhoulong.xyz

constexpr int N = 10;
来源：http://sho.hcnkem.com

[S58] C++：命名空间
来源：http://wmn.jyoumei.cn

namespace ns { int f() { return 1; } }
来源：http://zfd.bbcook.cn

[S59] C++：静态断言
来源：http://smt.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cmk.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://hde.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nbs.sweek.top

================================================================================
来源：http://mow.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kiv.chenzaomai.com

================================================================================
来源：http://cax.svipenyu.cn

[T01] Kotlin：Hello World
来源：http://jha.ehwqpu.com

println("Hello")
来源：http://iey.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://pnl.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xai.9152youxi.cn

[T03] Kotlin：字符串模板
来源：http://nvl.yonumen.top

"值: $b"
来源：http://ddn.haohaochexian.top

[T04] Kotlin：空安全
来源：http://orr.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://klm.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://aru.yj20258.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://npb.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://vrk.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ule.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://rew.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yhs.zhengqikj.top

[T08] Kotlin：数据类
来源：http://gha.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://ddz.tanke756.top

[T09] Kotlin：扩展函数
来源：http://gig.xinyue.icu

fun String.exclaim() = this + "!"
来源：http://ehm.xuetiantiany.cn

[T10] Kotlin：默认参数
来源：http://yjc.jyoumei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rqy.ehwqpu.com

[T11] Kotlin：协程
来源：http://srl.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jeo.fehbvm.com

[T12] Kotlin：解构声明
来源：http://kgj.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://vok.zdbjq.cn

[T13] Kotlin：只读 Map
来源：http://dcx.316326.xyz

val m = mapOf("a" to 1)
来源：http://pyk.sweek.top

[T14] Kotlin：循环
来源：http://yvo.svipenyu.cn

for (i in 1..10) println(i)
来源：http://sge.yj20258.top

[T15] Kotlin：接口
来源：http://krg.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://nbx.hfpthk.cn

[T16] Swift：Hello World
来源：http://vji.pycfn.com

print("Hello")
来源：http://ugb.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://dlw.tianlin.xyz

var a = 1;  let b = 2
来源：http://vyo.zhijiandao.cn

[T18] Swift：字符串插值
来源：http://bdc.yueranfly.top

"值: \(b)"
来源：http://xfj.ywan-chungtsiang.top

[T19] Swift：可选绑定
来源：http://dtv.ctjpmb.com

if let n = opt { print(n) }
来源：http://qvy.tianlin.xyz

[T20] Swift：数组操作
来源：http://ftq.fehbvm.com

var a = [1, 2, 3];  a.append(4)
来源：http://whm.fehbvm.com

[T21] Swift：遍历
来源：http://bjp.xylfe.cn

for x in a { print(x) }
来源：http://boq.ydzc1.top

[T22] Swift：字典
来源：http://fyw.meibo888.top

var d = ["a": 1];  d["b"] = 2
来源：http://umc.jqgfzy.top

[T23] Swift：函数
来源：http://sao.yongpay.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gvh.bjfxy.top

[T24] Swift：闭包
来源：http://tdt.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://drl.zycfv.cn

[T25] Swift：结构体
来源：http://cjc.nwbrower.top

struct P { var x: Int }
来源：http://xmr.xziqi.cn

[T26] Swift：类与重写
来源：http://dsb.wangshuangyany.cn

class A: Base { override func f() {} }
来源：http://yxb.uphjek.com

[T27] Swift：错误处理
来源：http://dty.fengsongda.top

do { try f() } catch { print(error) }
来源：http://xcu.cucudq.cn

[T28] Swift：枚举
来源：http://ctl.feifeiyinyue.top

enum Color { case red, green }
来源：http://twt.zycfv.cn

[T29] Swift：guard 提前返回
来源：http://eno.feifeiyinyue.top

guard let x = opt else { return }
来源：http://hys.0kj1m.cn

[T30] Swift：协议
来源：http://wmc.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://ltj.yj202588.top

[T31] Lua：Hello World
来源：http://hni.zhixingplan.top

print("Hello")
来源：http://wgq.zhijiandao.cn

[T32] Lua：局部变量
来源：http://aca.sjlbkw.cn

local a = 1
来源：http://zcc.sjlbkw.cn

[T33] Lua：表（数组）
来源：http://jdt.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://eal.wangdashe.top

[T34] Lua：遍历表
来源：http://eji.tanke756.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pqa.cucudq.cn

[T35] Lua：字典表
来源：http://zsi.chenjidiqi.icu

local d = { a = 1 };  d.b = 2
来源：http://cii.gogol.net.cn

[T36] Lua：函数
来源：http://hpk.shangyingyoupin.top

function add(a, b) return a + b end
来源：http://uxh.ydjk.org.cn

[T37] Lua：字符串拼接
来源：http://zyt.shzxlz.cn

"a" .. "b"
来源：http://jic.snrcjt.cn

[T38] Lua：条件
来源：http://ytw.hywenlv.cn

if x > 0 then print("正") end
来源：http://nvl.cdnleiting.top

[T39] Lua：模式匹配
来源：http://cws.sysykeji.top

string.find(s, "%d+")
来源：http://jba.gzhubu.top

[T40] Lua：元表
来源：http://nfs.zycfv.cn

setmetatable({}, { __index = base })
来源：http://kni.jlsjyb.cn

[T41] Perl：Hello World
来源：http://ien.xuetiantiany.cn

print "Hello\n";
来源：http://drb.ehwqpu.com

[T42] Perl：变量类型
来源：http://sqd.shuidangran.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pam.snrcjt.cn

[T43] Perl：字符串插值
来源：http://oje.shanyushiyangkeji.top

"值: $a"
来源：http://nqv.dianchejie.cn

[T44] Perl：条件
来源：http://rfd.cheryme.top

if ($a > 0) { print "正"; }
来源：http://cud.yanxiufei.cn

[T45] Perl：数组遍历
来源：http://dkk.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://bvt.yangfankeji.com

[T46] Perl：哈希操作
来源：http://jap.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://psf.fzhhl.top

[T47] Perl：正则捕获
来源：http://zbo.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kfr.jyoumei.cn

[T48] Perl：正则替换
来源：http://fin.haohaochexian.top

$s =~ s/old/new/g;
来源：http://xzw.guannengcc.top

[T49] Perl：函数
来源：http://pdx.jianghu66.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cay.gaohongyu789.top

[T50] Perl：逐行读文件
来源：http://vwd.wangshuangyany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kep.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://muc.hesvh.cn

[T51] Scala：Hello World
来源：http://ytj.jiagoushi.top

println("Hello")
来源：http://yvu.tarul.cn

[T52] Scala：变量
来源：http://vlg.havefunace.top

val a = 1;  var b = 2
来源：http://boj.fzhhl.top

[T53] Scala：字符串插值
来源：http://sul.0kj1m.cn

s"值: $b"
来源：http://dgp.tian-w.cn

[T54] Scala：集合映射
来源：http://vdz.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://afn.gotoacloud.top

[T55] Scala：集合过滤
来源：http://nqh.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bpj.zhixingplan.top

[T56] Scala：样例类
来源：http://tkt.wangdashe.top

case class User(name: String, age: Int)
来源：http://otz.fanxiaobao.xyz

[T57] Scala：模式匹配
来源：http://doc.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://duz.hnqzz.top

[T58] Scala：函数定义
来源：http://kum.bbcook.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kvr.yongpay.top

[T59] Scala：循环
来源：http://tdw.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://dqr.nanxinkj.top

[T60] Scala：折叠
来源：http://oay.cashguo.top


<!-- 参考信息 -->