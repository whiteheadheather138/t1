代发 wailian999

ssh user@host 'uptime'
来源：http://yma.ivvv.top

[R58] 下载文件
来源：http://vrm.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vll.xingfuxueyuan.xyz

[R59] 发 POST JSON
来源：http://agg.bjfxy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hkq.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://ggk.cqqwz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tdt.jinqigufen.top

[R61] 磁盘占用
来源：http://jur.zhengqikj.top

df -h;  du -sh *
来源：http://nsg.gotoacloud.top

[R62] 找最占空间的文件
来源：http://kkk.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://uyj.pycfn.com

[R63] 内存与进程
来源：http://xyq.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://hxk.yangfankeji.com

[R64] 结束进程
来源：http://lwx.jiagoushi.top

kill -9 $(pgrep -f app.py)
来源：http://ltu.shzxlz.cn

[R65] 查看端口占用
来源：http://lom.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dhn.yvedp.cn

[R66] 定时任务
来源：http://oyx.yueranfly.top

crontab -e;  crontab -l
来源：http://lkc.redwolf501.top

[R67] 生成随机十六进制串
来源：http://igr.nwbrower.top

openssl rand -hex 16
来源：http://vzx.pycfn.com

[R68] 计算文件校验值
来源：http://wrw.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oys.xuetiantiany.cn

[R69] 生成随机密码
来源：http://fos.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://ogo.aibaodan.cn

[R70] 时间戳与互转
来源：http://bkd.ivvv.top

date +%s;  date -d @1700000000
来源：http://qdi.jqgufenzy.top

[R71] 日期格式化
来源：http://adq.nanxuanxn.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xhj.hcnkem.com

[R72] 等待端口就绪
来源：http://uro.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://bqe.ybcxt.top

[R73] 分割大日志
来源：http://sth.jinqigufen.top

split -l 1000 big.log part_
来源：http://lmv.gzhubu.top

[R74] 批量重命名
来源：http://sbx.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tmn.meibo888.top

[R75] 导出环境变量
来源：http://luc.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://aws.shangyingyoupin.top

[R76] 使用临时文件
来源：http://alr.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dyz.guannengcc.top

[R77] 读取用户输入
来源：http://rqv.cheryme.top

read -rp "请输入: " ans
来源：http://bwb.dianchejie.cn

[R78] 交互式菜单
来源：http://hwh.xuetiantiany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xhv.shzxlz.cn

[R79] 解析命令行选项
来源：http://xir.xziqi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cnu.cucudq.cn

[R80] 查看脚本执行耗时
来源：http://esn.sysykeji.top

time ./run.sh
来源：http://jta.gotoacloud.top

================================================================================
来源：http://sio.haohaochexian.top

S. C / C++ 专题
来源：http://vxe.yj20258888.top

================================================================================
来源：http://wfo.ybcxt.top

[S01] C：Hello World
来源：http://fbh.chenzaomai.com

#include <stdio.h>
来源：http://wwk.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vju.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://mqx.jlsjyb.cn

int a = 10; printf("%d\n", a);
来源：http://rqh.yuanzhike.top

[S03] C：读入整数
来源：http://jfo.guowangkeji.top

int x; scanf("%d", &x);
来源：http://rpf.pycfn.com

[S04] C：字符串复制
来源：http://yum.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://exz.havefunace.top

[S05] C：字符串长度
来源：http://cbj.hammf.cn

strlen(s)
来源：http://lfj.daxiang520.top

[S06] C：字符串比较
来源：http://fen.c1oappe.top

strcmp(a, b) == 0
来源：http://zei.yonumen.top

[S07] C：数组遍历求和
来源：http://iqr.jianghu66.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vuo.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://kqw.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ant.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://jzd.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://noz.vqdsnc.cn

[S10] C：指针与解引用
来源：http://mmx.aizwys.cn

int *p = &a;  *p = 5;
来源：http://jsb.jianghu66.top

[S11] C：逐行读文件
来源：http://yqc.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://neq.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cgy.xuetiantiany.cn

fclose(f);
来源：http://qsa.jqgfzy.top

[S12] C：写文件
来源：http://ntt.wangshuangyany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://orn.yj20258888.top

[S13] C：宏定义
来源：http://vdp.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vej.zhiwuduotai.top

[S14] C：枚举
来源：http://nrs.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://dgd.hesvh.cn

[S15] C：类型转换
来源：http://eej.fktsv.cn

(double) a / b
来源：http://gtt.cashguo.top

[S16] C：位操作置位
来源：http://jij.sweek.top

x |= (1 << 3);
来源：http://nqt.fehbvm.com

[S17] C：安全拼接字符串
来源：http://pmb.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nqa.aizwys.cn

[S18] C：命令行参数
来源：http://kqv.hcnkem.com

int main(int argc, char **argv)
来源：http://dyf.dianchejie.cn

[S19] C：快速排序
来源：http://evr.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://xpj.wangdashe.top

[S20] C：二分查找
来源：http://yin.ydjk.org.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ymv.feifeiyinyue.top

[S21] C：字符类别判断
来源：http://usi.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baa.gogol.net.cn

[S22] C：字符串转数字
来源：http://ero.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://glb.yvedp.cn

[S23] C：随机数
来源：http://ikf.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zcx.cucudq.cn

[S24] C：获取本地时间
来源：http://sss.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lbj.ppjwa.cn

[S25] C：内存拷贝
来源：http://keb.yueranfly.top

memcpy(dst, src, n);
来源：http://eyo.fzhhl.top

[S26] C：内存清零
来源：http://nfb.gogol.net.cn

memset(a, 0, sizeof a);
来源：http://pui.bbcook.cn

[S27] C：定义常量
来源：http://djf.ybcxt.top

const double PI = 3.14159;
来源：http://jhb.jiagoushi.top

[S28] C：静态变量
来源：http://rin.dashuyun.cn

static int counter = 0;
来源：http://vyj.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://oyt.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://esy.havefunace.top

[S30] C：头文件保护
来源：http://vgc.yj20258888.top

#ifndef X_H
来源：http://cot.jlsjyb.cn

#define X_H
来源：http://oww.yangfankeji.com

#endif
来源：http://hwd.chenjidiqi.icu

[S31] C++：Hello World
来源：http://ipc.hfpthk.cn

#include <iostream>
来源：http://kkt.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://ptn.tarul.cn

[S32] C++：字符串
来源：http://wst.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://vet.vehdjk.com

[S33] C++：vector 增删
来源：http://cyi.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://spv.shuidangran.top

[S34] C++：遍历 vector
来源：http://njs.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://cfz.bjfxy.top

[S35] C++：map
来源：http://wcn.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pfi.zhengqikj.top

[S36] C++：unordered_map
来源：http://bsg.chenzaomai.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fzt.cashguo.top

[S37] C++：set
来源：http://wzg.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dbd.yj202588.top

[S38] C++：排序
来源：http://wzs.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://spn.bjfxy.top

[S39] C++：自定义比较器排序
来源：http://cvd.bbcook.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://owb.ydjk.org.cn

[S40] C++：查找元素
来源：http://dxy.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xuq.daxiang520.top

[S41] C++：类与构造函数
来源：http://cps.sjlbkw.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://deo.fzhhl.top

[S42] C++：继承与虚函数
来源：http://dhn.yuxming.cn

class B : public Base { public: void f() override {} };
来源：http://aee.tarul.cn

[S43] C++：智能指针
来源：http://mhl.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://uct.dashuyun.cn

[S44] C++：引用传参
来源：http://foc.xuanzx.com

void inc(int &x) { ++x; }
来源：http://phn.daxiang520.top

[S45] C++：lambda
来源：http://jua.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://ppc.snrcjt.cn

[S46] C++：函数模板
来源：http://rid.jiagoushi.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lmi.jlsjyb.cn

[S47] C++：结构化绑定遍历
来源：http://aha.zhijiandao.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nhl.ydjk.org.cn

[S48] C++：逐行读文件
来源：http://yln.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://efy.guowangkeji.top

while (std::getline(in, line)) { }
来源：http://kjx.cheryme.top

[S49] C++：写文件
来源：http://dot.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hhu.tanke756.top

[S50] C++：格式化数字
来源：http://ujw.zhoulong.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://teq.pengpengdd.cyou

[S51] C++：显式类型转换
来源：http://pac.fktsv.cn

static_cast<double>(a) / b
来源：http://rcz.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://afr.sjlbkw.cn

int size() const noexcept { return n_; }
来源：http://paf.daxiang520.top

[S53] C++：移动语义
来源：http://czm.jyoumei.cn

std::vector<int> w = std::move(v);
来源：http://eqf.quarkkingdee.top

[S54] C++：异常处理
来源：http://rll.zhoulong.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://esz.shangyingyoupin.top

[S55] C++：结构化绑定
来源：http://qrl.gaohongyu789.top

auto [a, b] = std::make_pair(1, 2);
来源：http://itg.jqgufenzy.top

[S56] C++：optional
来源：http://xzz.svipenyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cdk.yanxiufei.cn

[S57] C++：编译期常量
来源：http://mqy.yanxiufei.cn

constexpr int N = 10;
来源：http://acv.zhijiandao.cn

[S58] C++：命名空间
来源：http://sod.kuanghao11.cn

namespace ns { int f() { return 1; } }
来源：http://kpr.yj20258888.top

[S59] C++：静态断言
来源：http://mom.wangdashe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dlf.hywenlv.cn

[S60] C++：遍历并删除元素
来源：http://vcq.hammf.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rba.chenlongwang.top

================================================================================
来源：http://upt.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aur.yuxming.cn

================================================================================
来源：http://pwe.yongpay.top

[T01] Kotlin：Hello World
来源：http://rdd.shangyingyoupin.top

println("Hello")
来源：http://juu.zhengqikj.top

[T02] Kotlin：变量
来源：http://dwr.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pzb.hammf.cn

[T03] Kotlin：字符串模板
来源：http://czl.jianghu66.top

"值: $b"
来源：http://jtz.cheryme.top

[T04] Kotlin：空安全
来源：http://mnk.jqgfzy.top

val n: String? = null;  n?.length
来源：http://nzx.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://jtj.yangfankeji.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bli.vqdsnc.cn

[T06] Kotlin：集合映射
来源：http://tmx.fengsongda.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jis.vehdjk.com

[T07] Kotlin：集合过滤
来源：http://dor.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://czj.daria6918.cn

[T08] Kotlin：数据类
来源：http://ria.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://fce.zhiwuduotai.top

[T09] Kotlin：扩展函数
来源：http://gig.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://ott.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://zec.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ctd.c1oappe.top

[T11] Kotlin：协程
来源：http://ooh.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xpx.sxryk.cn

[T12] Kotlin：解构声明
来源：http://xjf.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://nok.meibo888.top

[T13] Kotlin：只读 Map
来源：http://zta.cucudq.cn

val m = mapOf("a" to 1)
来源：http://zcv.hcnkem.com

[T14] Kotlin：循环
来源：http://lme.fengsongda.top

for (i in 1..10) println(i)
来源：http://zty.jyoumei.cn

[T15] Kotlin：接口
来源：http://uwg.nwbrower.top

interface Shape { fun area(): Double }
来源：http://qxa.feifeiyinyue.top

[T16] Swift：Hello World
来源：http://wgk.zhaomingkeji.xyz

print("Hello")
来源：http://yew.hongshengwenyu.top

[T17] Swift：变量与常量
来源：http://uhr.zhongyouzk.top

var a = 1;  let b = 2
来源：http://sqj.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://khl.zhoulong.xyz

"值: \(b)"
来源：http://xoo.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://hmg.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://tfl.fanxiaobao.xyz

[T20] Swift：数组操作
来源：http://fre.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://yep.xuetiantiany.cn

[T21] Swift：遍历
来源：http://jhl.feifeiyinyue.top

for x in a { print(x) }
来源：http://jvi.jqgufenzy.top

[T22] Swift：字典
来源：http://dme.cdnleiting.top

var d = ["a": 1];  d["b"] = 2
来源：http://cky.sufxvd.cn

[T23] Swift：函数
来源：http://inv.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://idx.shanyushiyangtech.top

[T24] Swift：闭包
来源：http://hax.fktsv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wsi.birdmap.top

[T25] Swift：结构体
来源：http://evx.sjlbkw.cn

struct P { var x: Int }
来源：http://twg.mhx1999.top

[T26] Swift：类与重写
来源：http://nkm.snrcjt.cn

class A: Base { override func f() {} }
来源：http://ldv.fzhhl.top

[T27] Swift：错误处理
来源：http://kzc.havefunace.top

do { try f() } catch { print(error) }
来源：http://lwj.quarkkingdee.top

[T28] Swift：枚举
来源：http://rls.zhengqikj.top

enum Color { case red, green }
来源：http://xus.zycfv.cn

[T29] Swift：guard 提前返回
来源：http://pgi.dashuyun.cn

guard let x = opt else { return }
来源：http://pur.nwbrower.top

[T30] Swift：协议
来源：http://vwj.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://apo.yfazqb.com

[T31] Lua：Hello World
来源：http://xnk.svipenyu.cn

print("Hello")
来源：http://prl.yj20258.top

[T32] Lua：局部变量
来源：http://bxn.ydzc1.top

local a = 1
来源：http://zvb.guannengcc.top

[T33] Lua：表（数组）
来源：http://xka.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://clk.jinqigfzy.top

[T34] Lua：遍历表
来源：http://god.yfazqb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://cel.aizwys.cn

[T35] Lua：字典表
来源：http://umk.nwbrower.top

local d = { a = 1 };  d.b = 2
来源：http://xca.fehbvm.com

[T36] Lua：函数
来源：http://fek.fanxiaobao.xyz

function add(a, b) return a + b end
来源：http://fqm.sufxvd.cn

[T37] Lua：字符串拼接
来源：http://bmq.ydjk.org.cn

"a" .. "b"
来源：http://gov.fanxiaobao.xyz

[T38] Lua：条件
来源：http://yvn.ydjk.org.cn

if x > 0 then print("正") end
来源：http://cba.0kj1m.cn

[T39] Lua：模式匹配
来源：http://ngi.redwolf501.top

string.find(s, "%d+")
来源：http://ypl.vehdjk.com

[T40] Lua：元表
来源：http://rfl.yueranfly.top

setmetatable({}, { __index = base })
来源：http://mgm.zycfv.cn

[T41] Perl：Hello World
来源：http://ihc.fktsv.cn

print "Hello\n";
来源：http://gzp.hammf.cn

[T42] Perl：变量类型
来源：http://jvu.nanxinkj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tjp.shzxlz.cn

[T43] Perl：字符串插值
来源：http://qso.tian-w.cn

"值: $a"
来源：http://cxv.pengpengdd.cyou

[T44] Perl：条件
来源：http://yjt.fktsv.cn

if ($a > 0) { print "正"; }
来源：http://bkg.vqdsnc.cn

[T45] Perl：数组遍历
来源：http://mjk.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://nuh.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://bnr.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gcd.tian-w.cn

[T47] Perl：正则捕获
来源：http://dxa.ivvv.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://upn.quarkkingdee.top

[T48] Perl：正则替换
来源：http://zcv.jinqigufen.top

$s =~ s/old/new/g;
来源：http://qqz.yangfankeji.com

[T49] Perl：函数
来源：http://gvj.chenlongwang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://och.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://vyu.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lgy.jinqigfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://azc.hnqzz.top

[T51] Scala：Hello World
来源：http://poc.yueranfly.top

println("Hello")
来源：http://xva.mhx1999.top

[T52] Scala：变量
来源：http://ima.yuanzhike.top

val a = 1;  var b = 2
来源：http://kcv.yongpay.top

[T53] Scala：字符串插值
来源：http://uok.jinqigfzy.top

s"值: $b"
来源：http://aee.ydjk.org.cn

[T54] Scala：集合映射
来源：http://sdm.guowangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://jzo.ehwqpu.com

[T55] Scala：集合过滤
来源：http://bhs.hnqzz.top

List(1, 2, 3).filter(_ > 1)
来源：http://xwn.jlsjyb.cn

[T56] Scala：样例类
来源：http://puu.zhijiandao.cn

case class User(name: String, age: Int)
来源：http://jwm.shuidangran.top

[T57] Scala：模式匹配
来源：http://cvk.hcnkem.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://lqj.nwbrower.top

[T58] Scala：函数定义
来源：http://ovu.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://sad.feifeiyinyue.top

[T59] Scala：循环
来源：http://cka.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://tej.quarkkingdee.top

[T60] Scala：折叠
来源：http://shh.jinyuanbaomall.cn


<!-- 参考信息 -->