代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ohn.shanyushiyangkeji.top

[R56] 远程拷贝
来源：http://rto.guannengcc.top

scp file user@host:/path/
来源：http://hqn.52xcode.cn

[R57] 远程执行命令
来源：http://ief.cqqwz.cn

ssh user@host 'uptime'
来源：http://fas.yj202588.top

[R58] 下载文件
来源：http://her.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ofp.0kj1m.cn

[R59] 发 POST JSON
来源：http://sjc.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://izn.hesvh.cn

[R60] 只看 HTTP 状态码
来源：http://tgu.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zpm.fzhhl.top

[R61] 磁盘占用
来源：http://kwd.xylfe.cn

df -h;  du -sh *
来源：http://knb.hnxiangtu.top

[R62] 找最占空间的文件
来源：http://ffp.bbcook.cn

du -ah . | sort -rh | head -10
来源：http://wtb.zhixingplan.top

[R63] 内存与进程
来源：http://dyd.pycfn.com

free -h;  ps aux | grep nginx
来源：http://owd.yangfankeji.com

[R64] 结束进程
来源：http://tsv.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://fxo.c1oappe.top

[R65] 查看端口占用
来源：http://ezb.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pji.yanxiufei.cn

[R66] 定时任务
来源：http://yyh.316326.xyz

crontab -e;  crontab -l
来源：http://pfj.wangshuangyany.cn

[R67] 生成随机十六进制串
来源：http://izq.ppjwa.cn

openssl rand -hex 16
来源：http://czl.sufxvd.cn

[R68] 计算文件校验值
来源：http://lyc.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fxz.aibaodan.cn

[R69] 生成随机密码
来源：http://ijt.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://dnq.52xcode.cn

[R70] 时间戳与互转
来源：http://mtn.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://lwo.xylfe.cn

[R71] 日期格式化
来源：http://ugf.hnxiangtu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jow.xingfuxueyuan.xyz

[R72] 等待端口就绪
来源：http://rpw.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jtn.yuxming.cn

[R73] 分割大日志
来源：http://brb.ivvv.top

split -l 1000 big.log part_
来源：http://ges.kuanghao11.cn

[R74] 批量重命名
来源：http://gco.mhx1999.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jrk.nanxuanxn.top

[R75] 导出环境变量
来源：http://ety.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://koa.hysaishi.cn

[R76] 使用临时文件
来源：http://lhb.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ojo.zhixingplan.top

[R77] 读取用户输入
来源：http://lrf.316326.xyz

read -rp "请输入: " ans
来源：http://ztn.daria6918.cn

[R78] 交互式菜单
来源：http://ztx.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://aae.pycfn.com

[R79] 解析命令行选项
来源：http://ndo.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bwd.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://pwa.hnqzz.top

time ./run.sh
来源：http://hjl.ppjwa.cn

================================================================================
来源：http://dkm.zhengqikj.top

S. C / C++ 专题
来源：http://jzj.cdnleiting.top

================================================================================
来源：http://cne.bbcook.cn

[S01] C：Hello World
来源：http://aiy.redwolf501.top

#include <stdio.h>
来源：http://rqj.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cei.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://via.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://spi.aizwys.cn

[S03] C：读入整数
来源：http://pmd.snrcjt.cn

int x; scanf("%d", &x);
来源：http://wft.yangfankeji.com

[S04] C：字符串复制
来源：http://zat.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://vzg.xuetiantiany.cn

[S05] C：字符串长度
来源：http://nud.uphjek.com

strlen(s)
来源：http://sqm.jlsjyb.cn

[S06] C：字符串比较
来源：http://mai.c1oappe.top

strcmp(a, b) == 0
来源：http://cha.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://mpj.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fzz.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://yvr.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lyr.meibo888.top

[S09] C：结构体定义与初始化
来源：http://rin.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iio.nwbrower.top

[S10] C：指针与解引用
来源：http://jqd.yj20258888.top

int *p = &a;  *p = 5;
来源：http://jdu.dashuyun.cn

[S11] C：逐行读文件
来源：http://djq.zhiwuduotai.top

FILE *f = fopen("a.txt", "r");
来源：http://mlc.xingfuxueyuan.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://arl.ehwqpu.com

fclose(f);
来源：http://fql.tarul.cn

[S12] C：写文件
来源：http://nqw.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wxa.fehbvm.com

[S13] C：宏定义
来源：http://dkf.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pws.redwolf501.top

[S14] C：枚举
来源：http://eer.jianghu66.top

enum Color { RED, GREEN, BLUE };
来源：http://idy.ivvv.top

[S15] C：类型转换
来源：http://wjz.hammf.cn

(double) a / b
来源：http://qzp.sxryk.cn

[S16] C：位操作置位
来源：http://bqt.yuanzhike.top

x |= (1 << 3);
来源：http://ele.xuanzx.com

[S17] C：安全拼接字符串
来源：http://gle.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ruz.sxryk.cn

[S18] C：命令行参数
来源：http://ahv.epnwcf.com

int main(int argc, char **argv)
来源：http://agf.zhijiandao.cn

[S19] C：快速排序
来源：http://mph.jinghuilouyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tjc.yuxming.cn

[S20] C：二分查找
来源：http://igp.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cgb.dashuyun.cn

[S21] C：字符类别判断
来源：http://fzd.ivvv.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://phc.yangfankeji.com

[S22] C：字符串转数字
来源：http://jfu.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ujw.gotoacloud.top

[S23] C：随机数
来源：http://lky.c1oappe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bqd.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://iuq.yj20258.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fep.pengpengdd.cyou

[S25] C：内存拷贝
来源：http://arb.tarul.cn

memcpy(dst, src, n);
来源：http://pcc.zhijiandao.cn

[S26] C：内存清零
来源：http://bcd.cucudq.cn

memset(a, 0, sizeof a);
来源：http://keq.shuidangran.top

[S27] C：定义常量
来源：http://vfi.tian-w.cn

const double PI = 3.14159;
来源：http://xfx.hnqzz.top

[S28] C：静态变量
来源：http://mwo.wangdashe.top

static int counter = 0;
来源：http://zwl.kuanghao11.cn

[S29] C：变参函数
来源：http://bzg.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zjq.0kj1m.cn

[S30] C：头文件保护
来源：http://iuv.xuanzx.com

#ifndef X_H
来源：http://mov.c1oappe.top

#define X_H
来源：http://esi.hnqzz.top

#endif
来源：http://pcz.sufxvd.cn

[S31] C++：Hello World
来源：http://bmi.tian-w.cn

#include <iostream>
来源：http://ikb.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://drh.cdnleiting.top

[S32] C++：字符串
来源：http://qdj.fengsongda.top

std::string s = "hi";  s += "!";
来源：http://hxv.jlsjyb.cn

[S33] C++：vector 增删
来源：http://fax.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uqv.ydzc1.top

[S34] C++：遍历 vector
来源：http://hct.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://lwz.hammf.cn

[S35] C++：map
来源：http://yno.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sba.redwolf501.top

[S36] C++：unordered_map
来源：http://bgw.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dzd.316326.xyz

[S37] C++：set
来源：http://qfa.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ldr.jinghuilouyu.cn

[S38] C++：排序
来源：http://oqz.yanxiufei.cn

std::sort(v.begin(), v.end());
来源：http://aqj.yongpay.top

[S39] C++：自定义比较器排序
来源：http://zhx.zhixingplan.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ytc.jinqigfzy.top

[S40] C++：查找元素
来源：http://sov.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zof.bbcook.cn

[S41] C++：类与构造函数
来源：http://ddv.shanyushiyangtech.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rxu.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://sgr.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://piy.bjfxy.top

[S43] C++：智能指针
来源：http://ynj.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://dow.jiagoushi.top

[S44] C++：引用传参
来源：http://iwf.fzhhl.top

void inc(int &x) { ++x; }
来源：http://mdk.nanxinkj.top

[S45] C++：lambda
来源：http://mbx.tianlin.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://ocz.pengpengdd.cyou

[S46] C++：函数模板
来源：http://twz.fehbvm.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wjj.zhijiandao.cn

[S47] C++：结构化绑定遍历
来源：http://rdw.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bwe.zycfv.cn

[S48] C++：逐行读文件
来源：http://gfe.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://nns.epnwcf.com

while (std::getline(in, line)) { }
来源：http://qap.shzxlz.cn

[S49] C++：写文件
来源：http://hfo.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rur.fktsv.cn

[S50] C++：格式化数字
来源：http://uuq.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cly.xziqi.cn

[S51] C++：显式类型转换
来源：http://mtq.hcnkem.com

static_cast<double>(a) / b
来源：http://fuh.shzxlz.cn

[S52] C++：const 与 noexcept
来源：http://xqa.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://jmz.yongpay.top

[S53] C++：移动语义
来源：http://zsv.xingfuxueyuan.xyz

std::vector<int> w = std::move(v);
来源：http://dnx.tian-w.cn

[S54] C++：异常处理
来源：http://ybl.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uqn.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://ith.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gje.cqqwz.cn

[S56] C++：optional
来源：http://jgu.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bop.daria6918.cn

[S57] C++：编译期常量
来源：http://mvq.ydjk.org.cn

constexpr int N = 10;
来源：http://qsf.xziqi.cn

[S58] C++：命名空间
来源：http://qsn.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://utx.hysaishi.cn

[S59] C++：静态断言
来源：http://rib.zhaomingkeji.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nht.ivvv.top

[S60] C++：遍历并删除元素
来源：http://rrb.fehbvm.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kkz.pengpengdd.cyou

================================================================================
来源：http://jcc.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://snb.jlsjyb.cn

================================================================================
来源：http://xfh.cucudq.cn

[T01] Kotlin：Hello World
来源：http://dyn.nanxinkj.top

println("Hello")
来源：http://fee.shanyushiyangkeji.top

[T02] Kotlin：变量
来源：http://egu.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wxp.wangshuangyany.cn

[T03] Kotlin：字符串模板
来源：http://rir.sjlbkw.cn

"值: $b"
来源：http://xuc.havefunace.top

[T04] Kotlin：空安全
来源：http://ysa.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://ejb.yj20258.top

[T05] Kotlin：when 表达式
来源：http://jof.hywenlv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lry.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://ijz.ppjwa.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kgu.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://vkh.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wtz.andypj.xyz

[T08] Kotlin：数据类
来源：http://xyj.yongpay.top

data class User(val name: String, val age: Int)
来源：http://bre.pengpengdd.cyou

[T09] Kotlin：扩展函数
来源：http://tov.zdbjq.cn

fun String.exclaim() = this + "!"
来源：http://tmy.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://zxf.havefunace.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zxx.kuanghao11.cn

[T11] Kotlin：协程
来源：http://wfb.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sum.iojbl.cn

[T12] Kotlin：解构声明
来源：http://rdz.yueranfly.top

val (a, b) = Pair(1, 2)
来源：http://pdb.ppjwa.cn

[T13] Kotlin：只读 Map
来源：http://vpr.fktsv.cn

val m = mapOf("a" to 1)
来源：http://ksn.ehwqpu.com

[T14] Kotlin：循环
来源：http://scs.haohaochexian.top

for (i in 1..10) println(i)
来源：http://iqx.xinyue.icu

[T15] Kotlin：接口
来源：http://ejo.yj20258.top

interface Shape { fun area(): Double }
来源：http://wzx.dashuyun.cn

[T16] Swift：Hello World
来源：http://vdj.shanyushiyangtech.top

print("Hello")
来源：http://vlj.epnwcf.com

[T17] Swift：变量与常量
来源：http://jcd.wangdashe.top

var a = 1;  let b = 2
来源：http://jjp.xuanzx.com

[T18] Swift：字符串插值
来源：http://xvd.yvedp.cn

"值: \(b)"
来源：http://mrt.chenzaomai.com

[T19] Swift：可选绑定
来源：http://gru.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://pnv.aizwys.cn

[T20] Swift：数组操作
来源：http://bpu.yueranfly.top

var a = [1, 2, 3];  a.append(4)
来源：http://kjg.hesvh.cn

[T21] Swift：遍历
来源：http://eye.vehdjk.com

for x in a { print(x) }
来源：http://xib.nwbrower.top

[T22] Swift：字典
来源：http://hgk.0kj1m.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pib.zhoulong.xyz

[T23] Swift：函数
来源：http://ezl.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jbo.sufxvd.cn

[T24] Swift：闭包
来源：http://sdk.cucudq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rsp.wangdashe.top

[T25] Swift：结构体
来源：http://qsv.tian-w.cn

struct P { var x: Int }
来源：http://vle.sufxvd.cn

[T26] Swift：类与重写
来源：http://zrv.andypj.xyz

class A: Base { override func f() {} }
来源：http://nlw.jianghu66.top

[T27] Swift：错误处理
来源：http://hxa.ydzc1.top

do { try f() } catch { print(error) }
来源：http://spb.aizwys.cn

[T28] Swift：枚举
来源：http://nom.ivvv.top

enum Color { case red, green }
来源：http://jdw.jyoumei.cn

[T29] Swift：guard 提前返回
来源：http://cbk.guannengcc.top

guard let x = opt else { return }
来源：http://cfy.guowangkeji.top

[T30] Swift：协议
来源：http://zed.gaohongyu789.top

protocol Shape { func area() -> Double }
来源：http://ovc.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://cji.9152youxi.cn

print("Hello")
来源：http://ucv.zhijiandao.cn

[T32] Lua：局部变量
来源：http://ngp.jiagoushi.top

local a = 1
来源：http://upa.aizwys.cn

[T33] Lua：表（数组）
来源：http://lcq.bbcook.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dzp.havefunace.top

[T34] Lua：遍历表
来源：http://kmr.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ksq.nanxuanxn.top

[T35] Lua：字典表
来源：http://ksi.yfazqb.com

local d = { a = 1 };  d.b = 2
来源：http://fmg.nanxuanxn.top

[T36] Lua：函数
来源：http://xvc.fktsv.cn

function add(a, b) return a + b end
来源：http://jvg.smart0.xyz

[T37] Lua：字符串拼接
来源：http://joh.zhijiandao.cn

"a" .. "b"
来源：http://fmd.gotoacloud.top

[T38] Lua：条件
来源：http://xrp.shzxlz.cn

if x > 0 then print("正") end
来源：http://bpk.jqgfzy.top

[T39] Lua：模式匹配
来源：http://qnm.yvedp.cn

string.find(s, "%d+")
来源：http://hma.tarul.cn

[T40] Lua：元表
来源：http://bhv.daxiang520.top

setmetatable({}, { __index = base })
来源：http://tir.chenjidiqi.icu

[T41] Perl：Hello World
来源：http://wxu.sweek.top

print "Hello\n";
来源：http://fkj.hywenlv.cn

[T42] Perl：变量类型
来源：http://iel.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dfs.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://qnx.yfazqb.com

"值: $a"
来源：http://dcf.ppjwa.cn

[T44] Perl：条件
来源：http://ppt.wangshuangyany.cn

if ($a > 0) { print "正"; }
来源：http://ijg.zhijiandao.cn

[T45] Perl：数组遍历
来源：http://xij.quarkkingdee.top

for my $x (@arr) { print $x; }
来源：http://rrm.zhixingplan.top

[T46] Perl：哈希操作
来源：http://bzt.316326.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pgy.sjlbkw.cn

[T47] Perl：正则捕获
来源：http://qbi.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bzl.shangyingyoupin.top

[T48] Perl：正则替换
来源：http://frs.dashuyun.cn

$s =~ s/old/new/g;
来源：http://qce.tanke756.top

[T49] Perl：函数
来源：http://vdb.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rco.shuidangran.top

[T50] Perl：逐行读文件
来源：http://lgi.hesvh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rxj.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://rpu.316326.xyz

[T51] Scala：Hello World
来源：http://wqv.cdnleiting.top

println("Hello")
来源：http://sxv.svipenyu.cn

[T52] Scala：变量
来源：http://jby.sweek.top

val a = 1;  var b = 2
来源：http://ovg.cashguo.top

[T53] Scala：字符串插值
来源：http://oym.ydjk.org.cn

s"值: $b"
来源：http://zxp.daria6918.cn

[T54] Scala：集合映射
来源：http://acs.cqqwz.cn

List(1, 2, 3).map(_ * 2)
来源：http://mjt.c1oappe.top

[T55] Scala：集合过滤
来源：http://vzs.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://eyp.nwbrower.top

[T56] Scala：样例类
来源：http://fex.yongpay.top

case class User(name: String, age: Int)
来源：http://rtb.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://nyl.yvedp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tle.jinyuanbaomall.cn

[T58] Scala：函数定义
来源：http://dmu.ydjk.org.cn


<!-- 参考信息 -->