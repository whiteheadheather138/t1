代发 wailian999

ssh user@host 'uptime'
来源：http://qfo.xuanzx.com

[R58] 下载文件
来源：http://mwc.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rpp.svipenyu.cn

[R59] 发 POST JSON
来源：http://rja.shanyushiyangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uoj.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://rwi.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tci.zhoulong.xyz

[R61] 磁盘占用
来源：http://ass.yueranfly.top

df -h;  du -sh *
来源：http://hcd.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://gig.chenjidiqi.icu

du -ah . | sort -rh | head -10
来源：http://qzl.tanke756.top

[R63] 内存与进程
来源：http://dkh.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://rmc.yvedp.cn

[R64] 结束进程
来源：http://bwh.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://vsk.jqgufenzy.top

[R65] 查看端口占用
来源：http://yiq.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xrn.aizwys.cn

[R66] 定时任务
来源：http://oyl.hammf.cn

crontab -e;  crontab -l
来源：http://jcq.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://uoo.52xcode.cn

openssl rand -hex 16
来源：http://mgj.0kj1m.cn

[R68] 计算文件校验值
来源：http://zih.birdmap.top

sha256sum a.txt;  md5sum a.txt
来源：http://oyk.nanxuanxn.top

[R69] 生成随机密码
来源：http://skp.zhongyouzk.top

head -c 16 /dev/urandom | base64
来源：http://gaf.hfpthk.cn

[R70] 时间戳与互转
来源：http://bxm.yj202588.top

date +%s;  date -d @1700000000
来源：http://mfj.jinyuanbaomall.cn

[R71] 日期格式化
来源：http://ius.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rju.fktsv.cn

[R72] 等待端口就绪
来源：http://gbx.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nxh.aibaodan.cn

[R73] 分割大日志
来源：http://qba.gogol.net.cn

split -l 1000 big.log part_
来源：http://wsn.yj202588.top

[R74] 批量重命名
来源：http://tmt.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fmj.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://lxm.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://akl.xingfuxueyuan.xyz

[R76] 使用临时文件
来源：http://uvz.ehwqpu.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gaf.fzhhl.top

[R77] 读取用户输入
来源：http://huo.nanxinkj.top

read -rp "请输入: " ans
来源：http://deq.ydzc1.top

[R78] 交互式菜单
来源：http://tsn.xuetiantiany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yyv.gotoacloud.top

[R79] 解析命令行选项
来源：http://urc.feifeiyinyue.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jlt.ppjwa.cn

[R80] 查看脚本执行耗时
来源：http://kvd.hysaishi.cn

time ./run.sh
来源：http://noz.sxryk.cn

================================================================================
来源：http://ojs.shanyushiyangkeji.top

S. C / C++ 专题
来源：http://kkg.dashuyun.cn

================================================================================
来源：http://flm.yj20258888.top

[S01] C：Hello World
来源：http://hci.shangyingyoupin.top

#include <stdio.h>
来源：http://inl.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://syh.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://dnf.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://vlv.feifeiyinyue.top

[S03] C：读入整数
来源：http://xhy.ivvv.top

int x; scanf("%d", &x);
来源：http://zig.andypj.xyz

[S04] C：字符串复制
来源：http://hmy.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oks.daxiang520.top

[S05] C：字符串长度
来源：http://ugp.hongshengwenyu.top

strlen(s)
来源：http://fzc.zdbjq.cn

[S06] C：字符串比较
来源：http://ujn.cucudq.cn

strcmp(a, b) == 0
来源：http://rxe.dashuyun.cn

[S07] C：数组遍历求和
来源：http://ulj.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.haohaochexian.top

[S08] C：动态内存分配与释放
来源：http://nag.dashuyun.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dwu.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://toh.jinghuilouyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mkf.guowangkeji.top

[S10] C：指针与解引用
来源：http://qjg.yj20258.top

int *p = &a;  *p = 5;
来源：http://mgy.dianchejie.cn

[S11] C：逐行读文件
来源：http://iga.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://bfk.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://okl.xylfe.cn

fclose(f);
来源：http://mnw.quarkkingdee.top

[S12] C：写文件
来源：http://isu.haohaochexian.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cwo.fehbvm.com

[S13] C：宏定义
来源：http://kds.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kwe.wangdashe.top

[S14] C：枚举
来源：http://cuv.yuanzhike.top

enum Color { RED, GREEN, BLUE };
来源：http://wig.yj202588.top

[S15] C：类型转换
来源：http://iwh.andypj.xyz

(double) a / b
来源：http://vra.shangyingyoupin.top

[S16] C：位操作置位
来源：http://mcs.hammf.cn

x |= (1 << 3);
来源：http://aze.pycfn.com

[S17] C：安全拼接字符串
来源：http://fcw.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ktt.yfazqb.com

[S18] C：命令行参数
来源：http://ghe.zhoulong.xyz

int main(int argc, char **argv)
来源：http://oty.xinyue.icu

[S19] C：快速排序
来源：http://xyo.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://sbm.shanyushiyangtech.top

[S20] C：二分查找
来源：http://yvy.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lqq.xinyue.icu

[S21] C：字符类别判断
来源：http://rji.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tqp.dashuyun.cn

[S22] C：字符串转数字
来源：http://dlw.gaohongyu789.top

atoi("42");  strtod("3.14", NULL);
来源：http://nkn.yongpay.top

[S23] C：随机数
来源：http://raa.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zke.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://yyl.ydjk.org.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lhc.0kj1m.cn

[S25] C：内存拷贝
来源：http://wak.snrcjt.cn

memcpy(dst, src, n);
来源：http://apk.uphjek.com

[S26] C：内存清零
来源：http://jfh.cashguo.top

memset(a, 0, sizeof a);
来源：http://yeq.gotoacloud.top

[S27] C：定义常量
来源：http://cle.nanxinkj.top

const double PI = 3.14159;
来源：http://ipb.zhongyouzk.top

[S28] C：静态变量
来源：http://jws.zhiwuduotai.top

static int counter = 0;
来源：http://mpy.uphjek.com

[S29] C：变参函数
来源：http://imk.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vpg.cheryme.top

[S30] C：头文件保护
来源：http://zer.bbcook.cn

#ifndef X_H
来源：http://kuc.ydjk.org.cn

#define X_H
来源：http://sqs.haohaochexian.top

#endif
来源：http://omp.xziqi.cn

[S31] C++：Hello World
来源：http://oba.fengsongda.top

#include <iostream>
来源：http://wpk.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://pxn.hongshengwenyu.top

[S32] C++：字符串
来源：http://mny.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://yxh.feifeiyinyue.top

[S33] C++：vector 增删
来源：http://fno.hnqzz.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rru.gotoacloud.top

[S34] C++：遍历 vector
来源：http://ibs.pycfn.com

for (auto &x : v) { std::cout << x; }
来源：http://ext.hysaishi.cn

[S35] C++：map
来源：http://nya.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ytl.zdbjq.cn

[S36] C++：unordered_map
来源：http://bof.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pwv.shzxlz.cn

[S37] C++：set
来源：http://qfi.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jct.fengsongda.top

[S38] C++：排序
来源：http://evr.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://chb.zhaomingkeji.xyz

[S39] C++：自定义比较器排序
来源：http://hkl.zdbjq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cbx.quarkkingdee.top

[S40] C++：查找元素
来源：http://wlu.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xkc.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://tkb.gogol.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jfi.zycfv.cn

[S42] C++：继承与虚函数
来源：http://eig.mhx1999.top

class B : public Base { public: void f() override {} };
来源：http://pis.hnqzz.top

[S43] C++：智能指针
来源：http://dpr.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://esv.hnxiangtu.top

[S44] C++：引用传参
来源：http://mjk.yuxming.cn

void inc(int &x) { ++x; }
来源：http://tuf.meibo888.top

[S45] C++：lambda
来源：http://sec.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://chd.andypj.xyz

[S46] C++：函数模板
来源：http://xqz.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gec.sjlbkw.cn

[S47] C++：结构化绑定遍历
来源：http://cjz.vqdsnc.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vvt.hnxiangtu.top

[S48] C++：逐行读文件
来源：http://odw.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://qxk.jinqigufen.top

while (std::getline(in, line)) { }
来源：http://yzd.wangshuangyany.cn

[S49] C++：写文件
来源：http://epx.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wsh.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://hkj.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://swf.yj20258888.top

[S51] C++：显式类型转换
来源：http://snf.nanxuanxn.top

static_cast<double>(a) / b
来源：http://hwz.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://uez.xinyue.icu

int size() const noexcept { return n_; }
来源：http://bby.jyoumei.cn

[S53] C++：移动语义
来源：http://lti.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://cqs.yj20258888.top

[S54] C++：异常处理
来源：http://jro.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sri.chenlongwang.top

[S55] C++：结构化绑定
来源：http://tov.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://pir.quarkkingdee.top

[S56] C++：optional
来源：http://efa.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eng.hnxiangtu.top

[S57] C++：编译期常量
来源：http://nvu.smart0.xyz

constexpr int N = 10;
来源：http://ohz.xuetiantiany.cn

[S58] C++：命名空间
来源：http://iuv.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://xyt.gaohongyu789.top

[S59] C++：静态断言
来源：http://arw.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://abc.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://sse.sjlbkw.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tsw.svipenyu.cn

================================================================================
来源：http://atv.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zgd.jqgufenzy.top

================================================================================
来源：http://otb.uphjek.com

[T01] Kotlin：Hello World
来源：http://bzy.tianlin.xyz

println("Hello")
来源：http://ucc.zhijiandao.cn

[T02] Kotlin：变量
来源：http://sbu.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bhz.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://kdj.fktsv.cn

"值: $b"
来源：http://mlk.ctjpmb.com

[T04] Kotlin：空安全
来源：http://jhq.zhixingplan.top

val n: String? = null;  n?.length
来源：http://xsv.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://twr.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://duo.dianchejie.cn

[T06] Kotlin：集合映射
来源：http://eoz.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ojt.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://uyb.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tnb.yfazqb.com

[T08] Kotlin：数据类
来源：http://kas.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://tke.hongshengwenyu.top

[T09] Kotlin：扩展函数
来源：http://nhg.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://ygo.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://skh.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lxi.jinqigufen.top

[T11] Kotlin：协程
来源：http://zpa.wangdashe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bty.c1oappe.top

[T12] Kotlin：解构声明
来源：http://mhc.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://rlf.yuanzhike.top

[T13] Kotlin：只读 Map
来源：http://fxo.zhoulong.xyz

val m = mapOf("a" to 1)
来源：http://cgr.ydzc1.top

[T14] Kotlin：循环
来源：http://ssg.yongpay.top

for (i in 1..10) println(i)
来源：http://lkr.hesvh.cn

[T15] Kotlin：接口
来源：http://odr.smart0.xyz

interface Shape { fun area(): Double }
来源：http://upk.svipenyu.cn

[T16] Swift：Hello World
来源：http://bkq.hfpthk.cn

print("Hello")
来源：http://zsw.52xcode.cn

[T17] Swift：变量与常量
来源：http://qzd.9152youxi.cn

var a = 1;  let b = 2
来源：http://zfi.xuanzx.com

[T18] Swift：字符串插值
来源：http://sno.zycfv.cn

"值: \(b)"
来源：http://dcz.hnxiangtu.top

[T19] Swift：可选绑定
来源：http://wcx.jlsjyb.cn

if let n = opt { print(n) }
来源：http://pjy.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://dbt.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://ixv.chenjidiqi.icu

[T21] Swift：遍历
来源：http://unp.sweek.top

for x in a { print(x) }
来源：http://udv.xziqi.cn

[T22] Swift：字典
来源：http://bgk.nanxuanxn.top

var d = ["a": 1];  d["b"] = 2
来源：http://kjc.jlsjyb.cn

[T23] Swift：函数
来源：http://cjf.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xnm.zhengqikj.top

[T24] Swift：闭包
来源：http://ovd.hammf.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://chz.yj20258.top

[T25] Swift：结构体
来源：http://iza.ivvv.top

struct P { var x: Int }
来源：http://isq.fehbvm.com

[T26] Swift：类与重写
来源：http://ela.fktsv.cn

class A: Base { override func f() {} }
来源：http://zhl.birdmap.top

[T27] Swift：错误处理
来源：http://hcq.nanxuanxn.top

do { try f() } catch { print(error) }
来源：http://igi.gzhubu.top

[T28] Swift：枚举
来源：http://ocy.yj202588.top

enum Color { case red, green }
来源：http://mvf.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://xrz.epnwcf.com

guard let x = opt else { return }
来源：http://zel.fehbvm.com

[T30] Swift：协议
来源：http://cyz.zhiwuduotai.top

protocol Shape { func area() -> Double }
来源：http://xee.yueranfly.top

[T31] Lua：Hello World
来源：http://iyr.quarkkingdee.top

print("Hello")
来源：http://bvm.ydjk.org.cn

[T32] Lua：局部变量
来源：http://lou.ywan-chungtsiang.top

local a = 1
来源：http://jqe.shuidangran.top

[T33] Lua：表（数组）
来源：http://nsq.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qcm.cdnleiting.top

[T34] Lua：遍历表
来源：http://uxz.nanxuanxn.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kbh.gaohongyu789.top

[T35] Lua：字典表
来源：http://oyb.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://apl.xylfe.cn

[T36] Lua：函数
来源：http://ant.shanyushiyangtech.top

function add(a, b) return a + b end
来源：http://jdx.316326.xyz

[T37] Lua：字符串拼接
来源：http://ynr.yj202588.top

"a" .. "b"
来源：http://jmd.jqgfzy.top

[T38] Lua：条件
来源：http://vkv.aibaodan.cn

if x > 0 then print("正") end
来源：http://jgt.meibo888.top

[T39] Lua：模式匹配
来源：http://qzk.cheryme.top

string.find(s, "%d+")
来源：http://klk.tarul.cn

[T40] Lua：元表
来源：http://wzr.bjfxy.top

setmetatable({}, { __index = base })
来源：http://hly.jinyuanbaomall.cn

[T41] Perl：Hello World
来源：http://fzb.fktsv.cn

print "Hello\n";
来源：http://fmw.gotoacloud.top

[T42] Perl：变量类型
来源：http://izi.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lmm.ydzc1.top

[T43] Perl：字符串插值
来源：http://gse.c1oappe.top

"值: $a"
来源：http://ydo.dianchejie.cn

[T44] Perl：条件
来源：http://xhf.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://jwg.chenlongwang.top

[T45] Perl：数组遍历
来源：http://mny.ywan-chungtsiang.top

for my $x (@arr) { print $x; }
来源：http://duo.zdbjq.cn

[T46] Perl：哈希操作
来源：http://gmh.hfpthk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zcc.tian-w.cn

[T47] Perl：正则捕获
来源：http://pog.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://olg.cucudq.cn

[T48] Perl：正则替换
来源：http://iqz.bbcook.cn

$s =~ s/old/new/g;
来源：http://dzc.jyoumei.cn

[T49] Perl：函数
来源：http://dxw.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ptt.yj20258.top

[T50] Perl：逐行读文件
来源：http://vcw.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qtg.birdmap.top

while (my $line = <$fh>) { print $line; }
来源：http://hmq.gaohongyu789.top

[T51] Scala：Hello World
来源：http://vzu.hcnkem.com

println("Hello")
来源：http://wpy.fanxiaobao.xyz

[T52] Scala：变量
来源：http://jbe.dianchejie.cn

val a = 1;  var b = 2
来源：http://qsc.tian-w.cn

[T53] Scala：字符串插值
来源：http://ylt.tanke756.top

s"值: $b"
来源：http://cmc.vqdsnc.cn

[T54] Scala：集合映射
来源：http://ntm.zhixingplan.top

List(1, 2, 3).map(_ * 2)
来源：http://nst.guowangkeji.top

[T55] Scala：集合过滤
来源：http://zrj.kuanghao11.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uqv.andypj.xyz

[T56] Scala：样例类
来源：http://tkk.hysaishi.cn

case class User(name: String, age: Int)
来源：http://skh.sysykeji.top

[T57] Scala：模式匹配
来源：http://wlv.gogol.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vpb.shzxlz.cn

[T58] Scala：函数定义
来源：http://pby.svipenyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pzb.fengsongda.top

[T59] Scala：循环
来源：http://kbk.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://mms.jqgfzy.top

[T60] Scala：折叠
来源：http://yqo.zhoulong.xyz


<!-- 参考信息 -->