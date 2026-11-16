代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aby.xziqi.cn

[R60] 只看 HTTP 状态码
来源：http://pzb.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ybx.aizwys.cn

[R61] 磁盘占用
来源：http://ver.ydzc1.top

df -h;  du -sh *
来源：http://qll.chenlongwang.top

[R62] 找最占空间的文件
来源：http://ftb.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://xuw.ybcxt.top

[R63] 内存与进程
来源：http://vbk.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://qwy.yonumen.top

[R64] 结束进程
来源：http://xrr.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://iie.pengpengdd.cyou

[R65] 查看端口占用
来源：http://npt.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vzw.yvedp.cn

[R66] 定时任务
来源：http://osa.guannengcc.top

crontab -e;  crontab -l
来源：http://ecm.andypj.xyz

[R67] 生成随机十六进制串
来源：http://isb.ctjpmb.com

openssl rand -hex 16
来源：http://lnf.fengsongda.top

[R68] 计算文件校验值
来源：http://lzx.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://sxs.wangshuangyany.cn

[R69] 生成随机密码
来源：http://lfs.wangshuangyany.cn

head -c 16 /dev/urandom | base64
来源：http://raz.zdbjq.cn

[R70] 时间戳与互转
来源：http://kpm.c1oappe.top

date +%s;  date -d @1700000000
来源：http://jos.chenjidiqi.icu

[R71] 日期格式化
来源：http://rch.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oak.kuanghao11.cn

[R72] 等待端口就绪
来源：http://dll.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mxl.xuetiantiany.cn

[R73] 分割大日志
来源：http://dkk.ppjwa.cn

split -l 1000 big.log part_
来源：http://wxd.hywenlv.cn

[R74] 批量重命名
来源：http://nsb.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fkm.gogol.net.cn

[R75] 导出环境变量
来源：http://ycp.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://dbt.iojbl.cn

[R76] 使用临时文件
来源：http://ooh.quarkkingdee.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gkj.jianghu66.top

[R77] 读取用户输入
来源：http://coc.gotoacloud.top

read -rp "请输入: " ans
来源：http://kzc.andypj.xyz

[R78] 交互式菜单
来源：http://jjm.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lkh.daxiang520.top

[R79] 解析命令行选项
来源：http://ceb.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kqn.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://cbo.yfazqb.com

time ./run.sh
来源：http://fqv.zhengqikj.top

================================================================================
来源：http://xph.zdqjudy.top

S. C / C++ 专题
来源：http://iea.sweek.top

================================================================================
来源：http://huh.feifeiyinyue.top

[S01] C：Hello World
来源：http://etr.hongshengwenyu.top

#include <stdio.h>
来源：http://pbt.fzhhl.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://svl.fengsongda.top

[S02] C：变量与格式化输出
来源：http://coi.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://hlr.iojbl.cn

[S03] C：读入整数
来源：http://mkr.zhongyouzk.top

int x; scanf("%d", &x);
来源：http://jna.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://fnr.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ghw.fktsv.cn

[S05] C：字符串长度
来源：http://kfr.epnwcf.com

strlen(s)
来源：http://ljj.ivvv.top

[S06] C：字符串比较
来源：http://xsw.xziqi.cn

strcmp(a, b) == 0
来源：http://fzr.vehdjk.com

[S07] C：数组遍历求和
来源：http://gjh.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ljz.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://jnx.nanxinkj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dzs.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://cvm.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://arz.fehbvm.com

[S10] C：指针与解引用
来源：http://suh.zhixingplan.top

int *p = &a;  *p = 5;
来源：http://dqy.tian-w.cn

[S11] C：逐行读文件
来源：http://pcv.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://jhc.mhx1999.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://edh.ctjpmb.com

fclose(f);
来源：http://tkr.zhiwuduotai.top

[S12] C：写文件
来源：http://ery.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gek.daxiang520.top

[S13] C：宏定义
来源：http://diy.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cqq.ppjwa.cn

[S14] C：枚举
来源：http://nwt.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://orp.shuidangran.top

[S15] C：类型转换
来源：http://jfi.tanke756.top

(double) a / b
来源：http://dsy.zycfv.cn

[S16] C：位操作置位
来源：http://esy.zhengqikj.top

x |= (1 << 3);
来源：http://cbk.uphjek.com

[S17] C：安全拼接字符串
来源：http://kgo.ybcxt.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fjf.dashuyun.cn

[S18] C：命令行参数
来源：http://meh.birdmap.top

int main(int argc, char **argv)
来源：http://xsg.ydjk.org.cn

[S19] C：快速排序
来源：http://xcj.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://wya.gzhubu.top

[S20] C：二分查找
来源：http://yww.sweek.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jmo.tian-w.cn

[S21] C：字符类别判断
来源：http://fwl.316326.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sgu.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://kos.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://jyb.wangdashe.top

[S23] C：随机数
来源：http://opx.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://idy.mhx1999.top

[S24] C：获取本地时间
来源：http://bqf.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://agw.yj20258.top

[S25] C：内存拷贝
来源：http://bwv.pycfn.com

memcpy(dst, src, n);
来源：http://lpa.cashguo.top

[S26] C：内存清零
来源：http://lju.redwolf501.top

memset(a, 0, sizeof a);
来源：http://wfl.tarul.cn

[S27] C：定义常量
来源：http://hfo.hysaishi.cn

const double PI = 3.14159;
来源：http://pah.sjlbkw.cn

[S28] C：静态变量
来源：http://aew.dianchejie.cn

static int counter = 0;
来源：http://ctq.snrcjt.cn

[S29] C：变参函数
来源：http://vfz.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oyv.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://aoy.xylfe.cn

#ifndef X_H
来源：http://czb.wangdashe.top

#define X_H
来源：http://jvj.zhoulong.xyz

#endif
来源：http://ftr.jqgufenzy.top

[S31] C++：Hello World
来源：http://oex.fehbvm.com

#include <iostream>
来源：http://nno.redwolf501.top

int main() { std::cout << "Hello\n"; }
来源：http://ymg.yuanzhike.top

[S32] C++：字符串
来源：http://wto.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://wxj.dianchejie.cn

[S33] C++：vector 增删
来源：http://iwk.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://woi.nanxinkj.top

[S34] C++：遍历 vector
来源：http://bzb.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://nsm.xuetiantiany.cn

[S35] C++：map
来源：http://lgr.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ajd.gogol.net.cn

[S36] C++：unordered_map
来源：http://wxb.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://noc.wangshuangyany.cn

[S37] C++：set
来源：http://zot.xziqi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jqv.zhiwuduotai.top

[S38] C++：排序
来源：http://bei.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://vcm.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://pbk.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qrb.chenzaomai.com

[S40] C++：查找元素
来源：http://eqj.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bch.hywenlv.cn

[S41] C++：类与构造函数
来源：http://dxf.ybcxt.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iwp.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://wit.yvedp.cn

class B : public Base { public: void f() override {} };
来源：http://fne.zhengqikj.top

[S43] C++：智能指针
来源：http://usi.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://tjb.birdmap.top

[S44] C++：引用传参
来源：http://wbi.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://xkn.gogol.net.cn

[S45] C++：lambda
来源：http://sxz.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://pye.daxiang520.top

[S46] C++：函数模板
来源：http://fhf.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dmq.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://cxf.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mvd.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://phm.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://evb.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://jla.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://wki.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cql.vqdsnc.cn

[S50] C++：格式化数字
来源：http://myw.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://brr.yangfankeji.com

[S51] C++：显式类型转换
来源：http://eta.aizwys.cn

static_cast<double>(a) / b
来源：http://yfa.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://guz.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://rmi.yuxming.cn

[S53] C++：移动语义
来源：http://ujc.meibo888.top

std::vector<int> w = std::move(v);
来源：http://aux.snrcjt.cn

[S54] C++：异常处理
来源：http://idg.yuxming.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ocb.yueranfly.top

[S55] C++：结构化绑定
来源：http://fyf.gogol.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uim.ydzc1.top

[S56] C++：optional
来源：http://xxs.ppjwa.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fyq.andypj.xyz

[S57] C++：编译期常量
来源：http://qya.yj20258888.top

constexpr int N = 10;
来源：http://irt.smart0.xyz

[S58] C++：命名空间
来源：http://bdc.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://kcq.daria6918.cn

[S59] C++：静态断言
来源：http://grw.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yps.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://amo.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://god.iojbl.cn

================================================================================
来源：http://zvf.chenjidiqi.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kzz.hnxiangtu.top

================================================================================
来源：http://ksm.fanxiaobao.xyz

[T01] Kotlin：Hello World
来源：http://usz.kuanghao11.cn

println("Hello")
来源：http://hjm.ppjwa.cn

[T02] Kotlin：变量
来源：http://gls.ydjk.org.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qmm.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://lwt.zycfv.cn

"值: $b"
来源：http://fil.havefunace.top

[T04] Kotlin：空安全
来源：http://pmk.birdmap.top

val n: String? = null;  n?.length
来源：http://mts.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://frh.yangfankeji.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://grc.yongpay.top

[T06] Kotlin：集合映射
来源：http://odf.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lzt.xylfe.cn

[T07] Kotlin：集合过滤
来源：http://toi.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zmy.yanxiufei.cn

[T08] Kotlin：数据类
来源：http://hkp.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://olk.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://qdm.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://pgi.gotoacloud.top

[T10] Kotlin：默认参数
来源：http://jyf.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://raf.gaohongyu789.top

[T11] Kotlin：协程
来源：http://hro.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://etp.fzhhl.top

[T12] Kotlin：解构声明
来源：http://gwg.bjfxy.top

val (a, b) = Pair(1, 2)
来源：http://pnt.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://ugq.yuxming.cn

val m = mapOf("a" to 1)
来源：http://dze.zdbjq.cn

[T14] Kotlin：循环
来源：http://mlm.jianghu66.top

for (i in 1..10) println(i)
来源：http://wyw.ydzc1.top

[T15] Kotlin：接口
来源：http://wbk.yvedp.cn

interface Shape { fun area(): Double }
来源：http://ynz.yj20258.top

[T16] Swift：Hello World
来源：http://aad.fehbvm.com

print("Hello")
来源：http://akt.52xcode.cn

[T17] Swift：变量与常量
来源：http://ngc.xuetiantiany.cn

var a = 1;  let b = 2
来源：http://jlg.aizwys.cn

[T18] Swift：字符串插值
来源：http://eey.sjlbkw.cn

"值: \(b)"
来源：http://fkc.yongpay.top

[T19] Swift：可选绑定
来源：http://tyc.aizwys.cn

if let n = opt { print(n) }
来源：http://azb.yongpay.top

[T20] Swift：数组操作
来源：http://urb.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://dpo.gotoacloud.top

[T21] Swift：遍历
来源：http://uuz.hesvh.cn

for x in a { print(x) }
来源：http://znr.zhiwuduotai.top

[T22] Swift：字典
来源：http://rok.nanxuanxn.top

var d = ["a": 1];  d["b"] = 2
来源：http://udc.redwolf501.top

[T23] Swift：函数
来源：http://qjr.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uyt.zhoulong.xyz

[T24] Swift：闭包
来源：http://scg.chenlongwang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ynq.xylfe.cn

[T25] Swift：结构体
来源：http://tor.zhixingplan.top

struct P { var x: Int }
来源：http://zxh.guowangkeji.top

[T26] Swift：类与重写
来源：http://hmp.gzhubu.top

class A: Base { override func f() {} }
来源：http://xic.pengpengdd.cyou

[T27] Swift：错误处理
来源：http://jlx.chenlongwang.top

do { try f() } catch { print(error) }
来源：http://avx.fengsongda.top

[T28] Swift：枚举
来源：http://nny.ydjk.org.cn

enum Color { case red, green }
来源：http://lsj.fktsv.cn

[T29] Swift：guard 提前返回
来源：http://ymd.nanxinkj.top

guard let x = opt else { return }
来源：http://mmx.smart0.xyz

[T30] Swift：协议
来源：http://dcm.nanxinkj.top

protocol Shape { func area() -> Double }
来源：http://zvh.ctjpmb.com

[T31] Lua：Hello World
来源：http://zqt.guowangkeji.top

print("Hello")
来源：http://kbd.shanyushiyangtech.top

[T32] Lua：局部变量
来源：http://ipj.yonumen.top

local a = 1
来源：http://uwt.pengpengdd.cyou

[T33] Lua：表（数组）
来源：http://ftb.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dsq.xziqi.cn

[T34] Lua：遍历表
来源：http://csc.shuidangran.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ehn.zhengqikj.top

[T35] Lua：字典表
来源：http://bpm.cucudq.cn

local d = { a = 1 };  d.b = 2
来源：http://yno.jyoumei.cn

[T36] Lua：函数
来源：http://gfm.xylfe.cn

function add(a, b) return a + b end
来源：http://msq.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://idh.cucudq.cn

"a" .. "b"
来源：http://gkw.zdqjudy.top

[T38] Lua：条件
来源：http://gsr.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://idl.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://gpx.zhengqikj.top

string.find(s, "%d+")
来源：http://mmv.gaohongyu789.top

[T40] Lua：元表
来源：http://iqh.guannengcc.top

setmetatable({}, { __index = base })
来源：http://nuc.cashguo.top

[T41] Perl：Hello World
来源：http://hqu.yj20258888.top

print "Hello\n";
来源：http://uyq.zhijiandao.cn

[T42] Perl：变量类型
来源：http://efv.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fht.chenjidiqi.icu

[T43] Perl：字符串插值
来源：http://flg.hywenlv.cn

"值: $a"
来源：http://zmp.smart0.xyz

[T44] Perl：条件
来源：http://rue.yvedp.cn

if ($a > 0) { print "正"; }
来源：http://coe.epnwcf.com

[T45] Perl：数组遍历
来源：http://htq.tarul.cn

for my $x (@arr) { print $x; }
来源：http://edm.fengsongda.top

[T46] Perl：哈希操作
来源：http://cce.aibaodan.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wyh.fengsongda.top

[T47] Perl：正则捕获
来源：http://xiq.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://yqk.daria6918.cn

[T48] Perl：正则替换
来源：http://ygj.yfazqb.com

$s =~ s/old/new/g;
来源：http://ixj.sysykeji.top

[T49] Perl：函数
来源：http://wlf.yj202588.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kui.hongshengwenyu.top

[T50] Perl：逐行读文件
来源：http://kje.mhx1999.top

open my $fh, "<", "a.txt" or die $!;
来源：http://izk.shzxlz.cn

while (my $line = <$fh>) { print $line; }
来源：http://rax.tarul.cn

[T51] Scala：Hello World
来源：http://icm.vehdjk.com

println("Hello")
来源：http://jim.yongpay.top

[T52] Scala：变量
来源：http://qzv.ydjk.org.cn

val a = 1;  var b = 2
来源：http://xoq.316326.xyz

[T53] Scala：字符串插值
来源：http://kuj.redwolf501.top

s"值: $b"
来源：http://ywj.zhongyouzk.top

[T54] Scala：集合映射
来源：http://ojx.guowangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://xeo.gaohongyu789.top

[T55] Scala：集合过滤
来源：http://bhm.vehdjk.com

List(1, 2, 3).filter(_ > 1)
来源：http://tge.zhijiandao.cn

[T56] Scala：样例类
来源：http://yol.haohaochexian.top

case class User(name: String, age: Int)
来源：http://uju.quarkkingdee.top

[T57] Scala：模式匹配
来源：http://uxj.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ajq.jqgfzy.top

[T58] Scala：函数定义
来源：http://cyg.hesvh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ceq.jinyuanbaomall.cn

[T59] Scala：循环
来源：http://mqr.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://gcb.yonumen.top

[T60] Scala：折叠
来源：http://amc.jqgufenzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wau.hysaishi.cn

================================================================================
来源：http://jox.cqqwz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iqc.yanxiufei.cn

================================================================================
来源：http://viy.kuanghao11.cn


<!-- 参考信息 -->