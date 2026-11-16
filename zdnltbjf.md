代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qnw.zhongyouzk.top

[R54] 比较两个文件
来源：http://fob.aibaodan.cn

diff a.txt b.txt
来源：http://dpa.zhaomingkeji.xyz

[R55] 压缩与解压
来源：http://ehf.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ueb.fanxiaobao.xyz

[R56] 远程拷贝
来源：http://qwf.hesvh.cn

scp file user@host:/path/
来源：http://bjo.jqgufenzy.top

[R57] 远程执行命令
来源：http://kre.wangdashe.top

ssh user@host 'uptime'
来源：http://dbf.chenjidiqi.icu

[R58] 下载文件
来源：http://pjq.ctjpmb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rqp.tanke756.top

[R59] 发 POST JSON
来源：http://moj.xingfuxueyuan.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vuf.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://qoe.bjfxy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nqr.wangshuangyany.cn

[R61] 磁盘占用
来源：http://jcg.guannengcc.top

df -h;  du -sh *
来源：http://skn.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://mdr.316326.xyz

du -ah . | sort -rh | head -10
来源：http://bgz.jiagoushi.top

[R63] 内存与进程
来源：http://jlt.xziqi.cn

free -h;  ps aux | grep nginx
来源：http://zrg.mhx1999.top

[R64] 结束进程
来源：http://oup.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://dzu.sjlbkw.cn

[R65] 查看端口占用
来源：http://kpa.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rxe.sufxvd.cn

[R66] 定时任务
来源：http://yen.vqdsnc.cn

crontab -e;  crontab -l
来源：http://ppz.yangfankeji.com

[R67] 生成随机十六进制串
来源：http://ydk.cdnleiting.top

openssl rand -hex 16
来源：http://dwd.ydzc1.top

[R68] 计算文件校验值
来源：http://dpx.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://uzv.gaohongyu789.top

[R69] 生成随机密码
来源：http://xhp.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://vmv.zdbjq.cn

[R70] 时间戳与互转
来源：http://add.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://qzs.zdbjq.cn

[R71] 日期格式化
来源：http://wnf.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://llr.zhixingplan.top

[R72] 等待端口就绪
来源：http://sls.quarkkingdee.top

until nc -z localhost 3306; do sleep 1; done
来源：http://npg.gogol.net.cn

[R73] 分割大日志
来源：http://arv.andypj.xyz

split -l 1000 big.log part_
来源：http://eow.yongpay.top

[R74] 批量重命名
来源：http://tle.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://utx.zhixingplan.top

[R75] 导出环境变量
来源：http://mri.wangshuangyany.cn

export PATH="$HOME/bin:$PATH"
来源：http://set.haohaochexian.top

[R76] 使用临时文件
来源：http://ufb.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baf.chenjidiqi.icu

[R77] 读取用户输入
来源：http://lpm.guannengcc.top

read -rp "请输入: " ans
来源：http://flz.zycfv.cn

[R78] 交互式菜单
来源：http://jnx.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vgj.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://edb.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://onw.jinghuilouyu.cn

[R80] 查看脚本执行耗时
来源：http://adc.sweek.top

time ./run.sh
来源：http://tgg.feifeiyinyue.top

================================================================================
来源：http://oqe.smart0.xyz

S. C / C++ 专题
来源：http://lbj.yangfankeji.com

================================================================================
来源：http://tpn.ctjpmb.com

[S01] C：Hello World
来源：http://lxh.ydzc1.top

#include <stdio.h>
来源：http://hra.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tdi.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://qwn.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://kzf.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://jmb.zdbjq.cn

int x; scanf("%d", &x);
来源：http://sth.xingfuxueyuan.xyz

[S04] C：字符串复制
来源：http://lzk.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://tzd.xuanzx.com

[S05] C：字符串长度
来源：http://slo.xingfuxueyuan.xyz

strlen(s)
来源：http://bwa.sysykeji.top

[S06] C：字符串比较
来源：http://zzr.52xcode.cn

strcmp(a, b) == 0
来源：http://bkm.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://ije.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://axi.316326.xyz

[S08] C：动态内存分配与释放
来源：http://pex.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rnn.zhoulong.xyz

[S09] C：结构体定义与初始化
来源：http://ysk.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jhl.jinqigfzy.top

[S10] C：指针与解引用
来源：http://hwf.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://sjp.guowangkeji.top

[S11] C：逐行读文件
来源：http://rhb.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://fij.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gsm.gzhubu.top

fclose(f);
来源：http://ugt.chenzaomai.com

[S12] C：写文件
来源：http://wjn.shanyushiyangtech.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zvb.ywan-chungtsiang.top

[S13] C：宏定义
来源：http://qsk.nanxinkj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ohx.zhiwuduotai.top

[S14] C：枚举
来源：http://kdb.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://spr.nwbrower.top

[S15] C：类型转换
来源：http://vzu.zhoulong.xyz

(double) a / b
来源：http://bdm.yfazqb.com

[S16] C：位操作置位
来源：http://yfd.fktsv.cn

x |= (1 << 3);
来源：http://gql.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://pnp.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oku.cashguo.top

[S18] C：命令行参数
来源：http://xzl.gzhubu.top

int main(int argc, char **argv)
来源：http://xmb.fehbvm.com

[S19] C：快速排序
来源：http://nik.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jlt.hywenlv.cn

[S20] C：二分查找
来源：http://lst.jinqigufen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fxs.havefunace.top

[S21] C：字符类别判断
来源：http://ddd.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ety.zdqjudy.top

[S22] C：字符串转数字
来源：http://ndn.yvedp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pum.hesvh.cn

[S23] C：随机数
来源：http://otw.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vtt.epnwcf.com

[S24] C：获取本地时间
来源：http://drw.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pgv.jqgfzy.top

[S25] C：内存拷贝
来源：http://rlv.bbcook.cn

memcpy(dst, src, n);
来源：http://swo.cheryme.top

[S26] C：内存清零
来源：http://amo.xuanzx.com

memset(a, 0, sizeof a);
来源：http://qym.zdbjq.cn

[S27] C：定义常量
来源：http://toy.bjfxy.top

const double PI = 3.14159;
来源：http://jao.zhongyouzk.top

[S28] C：静态变量
来源：http://rbd.hywenlv.cn

static int counter = 0;
来源：http://lky.guannengcc.top

[S29] C：变参函数
来源：http://mgj.cheryme.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xkd.shzxlz.cn

[S30] C：头文件保护
来源：http://cjt.bbcook.cn

#ifndef X_H
来源：http://hds.daria6918.cn

#define X_H
来源：http://lnm.hcnkem.com

#endif
来源：http://bga.sjlbkw.cn

[S31] C++：Hello World
来源：http://kof.dashuyun.cn

#include <iostream>
来源：http://yrq.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://chz.sxryk.cn

[S32] C++：字符串
来源：http://coa.hywenlv.cn

std::string s = "hi";  s += "!";
来源：http://yfj.tanke756.top

[S33] C++：vector 增删
来源：http://mkp.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://txt.hesvh.cn

[S34] C++：遍历 vector
来源：http://aqe.0kj1m.cn

for (auto &x : v) { std::cout << x; }
来源：http://ezn.fzhhl.top

[S35] C++：map
来源：http://xte.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hjl.fengsongda.top

[S36] C++：unordered_map
来源：http://dep.zhengqikj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wvp.0kj1m.cn

[S37] C++：set
来源：http://oht.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hug.jinyuanbaomall.cn

[S38] C++：排序
来源：http://pri.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://qcr.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://lwv.c1oappe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bmm.hysaishi.cn

[S40] C++：查找元素
来源：http://dlv.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jdr.hnqzz.top

[S41] C++：类与构造函数
来源：http://owg.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://six.uphjek.com

[S42] C++：继承与虚函数
来源：http://hri.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://bsw.vehdjk.com

[S43] C++：智能指针
来源：http://ulc.0kj1m.cn

auto p = std::make_unique<int>(5);
来源：http://tou.smart0.xyz

[S44] C++：引用传参
来源：http://iew.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://twe.yuanzhike.top

[S45] C++：lambda
来源：http://wpk.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://kle.chenlongwang.top

[S46] C++：函数模板
来源：http://zfh.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yiv.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://nzd.meibo888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nij.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://mvy.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://gxn.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://qsf.zhijiandao.cn

[S49] C++：写文件
来源：http://eyj.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://onr.yangfankeji.com

[S50] C++：格式化数字
来源：http://qlf.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xkp.chenzaomai.com

[S51] C++：显式类型转换
来源：http://guw.yj20258.top

static_cast<double>(a) / b
来源：http://eab.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://dls.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://jls.zhongyouzk.top

[S53] C++：移动语义
来源：http://paa.tanke756.top

std::vector<int> w = std::move(v);
来源：http://yyk.ybcxt.top

[S54] C++：异常处理
来源：http://cml.chenzaomai.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lxl.cashguo.top

[S55] C++：结构化绑定
来源：http://dim.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mdu.svipenyu.cn

[S56] C++：optional
来源：http://qrf.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qct.ybcxt.top

[S57] C++：编译期常量
来源：http://mrq.feifeiyinyue.top

constexpr int N = 10;
来源：http://tes.gzhubu.top

[S58] C++：命名空间
来源：http://esg.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://ksw.zhijiandao.cn

[S59] C++：静态断言
来源：http://rzk.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://msi.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://pun.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hbj.jiagoushi.top

================================================================================
来源：http://uwd.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fmx.zhongyouzk.top

================================================================================
来源：http://rxp.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://ehp.sjlbkw.cn

println("Hello")
来源：http://gnc.yj202588.top

[T02] Kotlin：变量
来源：http://smh.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vin.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://mkl.ydjk.org.cn

"值: $b"
来源：http://pll.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://chg.redwolf501.top

val n: String? = null;  n?.length
来源：http://zjn.ehwqpu.com

[T05] Kotlin：when 表达式
来源：http://jzw.hnqzz.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jqi.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://tse.aibaodan.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://duq.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://srl.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://myc.yvedp.cn

[T08] Kotlin：数据类
来源：http://duv.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://lkn.9152youxi.cn

[T09] Kotlin：扩展函数
来源：http://uge.shzxlz.cn

fun String.exclaim() = this + "!"
来源：http://dpi.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://vzw.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://arn.jyoumei.cn

[T11] Kotlin：协程
来源：http://fxd.quarkkingdee.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kbo.cucudq.cn

[T12] Kotlin：解构声明
来源：http://cgm.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://gvj.yuanzhike.top

[T13] Kotlin：只读 Map
来源：http://iah.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://lgh.xziqi.cn

[T14] Kotlin：循环
来源：http://cqy.gogol.net.cn

for (i in 1..10) println(i)
来源：http://zhf.bjfxy.top

[T15] Kotlin：接口
来源：http://zsx.nanxuanxn.top

interface Shape { fun area(): Double }
来源：http://zti.snrcjt.cn

[T16] Swift：Hello World
来源：http://xye.birdmap.top

print("Hello")
来源：http://qxq.uphjek.com

[T17] Swift：变量与常量
来源：http://vjy.yj20258.top

var a = 1;  let b = 2
来源：http://twc.sjlbkw.cn

[T18] Swift：字符串插值
来源：http://egz.jqgfzy.top

"值: \(b)"
来源：http://hmg.haohaochexian.top

[T19] Swift：可选绑定
来源：http://pep.haohaochexian.top

if let n = opt { print(n) }
来源：http://zhe.andypj.xyz

[T20] Swift：数组操作
来源：http://hsr.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://zne.sxryk.cn

[T21] Swift：遍历
来源：http://dil.nanxinkj.top

for x in a { print(x) }
来源：http://pjw.pycfn.com

[T22] Swift：字典
来源：http://bvx.meibo888.top

var d = ["a": 1];  d["b"] = 2
来源：http://coj.ppjwa.cn

[T23] Swift：函数
来源：http://kvi.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gge.haohaochexian.top

[T24] Swift：闭包
来源：http://xfo.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wbd.cdnleiting.top

[T25] Swift：结构体
来源：http://upe.ybcxt.top

struct P { var x: Int }
来源：http://ktc.bbcook.cn

[T26] Swift：类与重写
来源：http://inl.birdmap.top

class A: Base { override func f() {} }
来源：http://ony.jinyuanbaomall.cn

[T27] Swift：错误处理
来源：http://iow.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://njh.xingfuxueyuan.xyz

[T28] Swift：枚举
来源：http://kkk.feifeiyinyue.top

enum Color { case red, green }
来源：http://zyv.ydzc1.top

[T29] Swift：guard 提前返回
来源：http://cxs.chenlongwang.top

guard let x = opt else { return }
来源：http://azp.xylfe.cn

[T30] Swift：协议
来源：http://tpj.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://bps.zycfv.cn

[T31] Lua：Hello World
来源：http://ppa.vehdjk.com

print("Hello")
来源：http://kof.tarul.cn

[T32] Lua：局部变量
来源：http://pjs.tianlin.xyz

local a = 1
来源：http://tvb.jiagoushi.top

[T33] Lua：表（数组）
来源：http://pji.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rjt.pycfn.com

[T34] Lua：遍历表
来源：http://kiz.shuidangran.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wtv.ctjpmb.com

[T35] Lua：字典表
来源：http://zmz.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://ovr.birdmap.top

[T36] Lua：函数
来源：http://yaq.kuanghao11.cn

function add(a, b) return a + b end
来源：http://omo.yanxiufei.cn

[T37] Lua：字符串拼接
来源：http://fxy.jyoumei.cn

"a" .. "b"
来源：http://rnm.zhongyouzk.top

[T38] Lua：条件
来源：http://kbb.9152youxi.cn

if x > 0 then print("正") end
来源：http://lgm.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://lpc.tian-w.cn

string.find(s, "%d+")
来源：http://xps.iojbl.cn

[T40] Lua：元表
来源：http://tcf.bbcook.cn

setmetatable({}, { __index = base })
来源：http://biw.sufxvd.cn

[T41] Perl：Hello World
来源：http://qby.hcnkem.com

print "Hello\n";
来源：http://qrg.quarkkingdee.top

[T42] Perl：变量类型
来源：http://qxt.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eru.gzhubu.top

[T43] Perl：字符串插值
来源：http://vey.52xcode.cn

"值: $a"
来源：http://opn.guowangkeji.top

[T44] Perl：条件
来源：http://tdi.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://ayf.fzhhl.top

[T45] Perl：数组遍历
来源：http://xvw.bjfxy.top

for my $x (@arr) { print $x; }
来源：http://lgm.jinqigufen.top

[T46] Perl：哈希操作
来源：http://qxz.vqdsnc.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bur.sjlbkw.cn

[T47] Perl：正则捕获
来源：http://vwm.sysykeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pgi.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://seu.ehwqpu.com

$s =~ s/old/new/g;
来源：http://xxn.vehdjk.com

[T49] Perl：函数
来源：http://jov.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aez.fktsv.cn

[T50] Perl：逐行读文件
来源：http://jgo.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gca.cheryme.top

while (my $line = <$fh>) { print $line; }
来源：http://wjy.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://jgu.tarul.cn

println("Hello")
来源：http://vhz.epnwcf.com

[T52] Scala：变量
来源：http://iom.tian-w.cn

val a = 1;  var b = 2
来源：http://ydb.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://vpy.ivvv.top

s"值: $b"
来源：http://sxw.yj202588.top

[T54] Scala：集合映射
来源：http://kyt.hfpthk.cn

List(1, 2, 3).map(_ * 2)
来源：http://nxw.zhengqikj.top

[T55] Scala：集合过滤
来源：http://toi.0kj1m.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xju.nanxuanxn.top

[T56] Scala：样例类
来源：http://nlw.zhiwuduotai.top


<!-- 参考信息 -->