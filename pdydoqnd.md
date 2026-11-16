代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://grx.sjlbkw.cn

[R56] 远程拷贝
来源：http://icu.ydjk.org.cn

scp file user@host:/path/
来源：http://zqc.meibo888.top

[R57] 远程执行命令
来源：http://mev.fehbvm.com

ssh user@host 'uptime'
来源：http://ivp.chenzaomai.com

[R58] 下载文件
来源：http://uoe.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gzz.xuanzx.com

[R59] 发 POST JSON
来源：http://kvy.cashguo.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tzf.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://fwv.xuetiantiany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://egl.aizwys.cn

[R61] 磁盘占用
来源：http://fis.cucudq.cn

df -h;  du -sh *
来源：http://rll.bbcook.cn

[R62] 找最占空间的文件
来源：http://nyg.hammf.cn

du -ah . | sort -rh | head -10
来源：http://wpw.havefunace.top

[R63] 内存与进程
来源：http://chi.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://cqc.bjfxy.top

[R64] 结束进程
来源：http://wpe.52xcode.cn

kill -9 $(pgrep -f app.py)
来源：http://myu.nanxuanxn.top

[R65] 查看端口占用
来源：http://wyi.redwolf501.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uzv.feifeiyinyue.top

[R66] 定时任务
来源：http://oxz.hysaishi.cn

crontab -e;  crontab -l
来源：http://wqi.316326.xyz

[R67] 生成随机十六进制串
来源：http://rye.ctjpmb.com

openssl rand -hex 16
来源：http://qjl.52xcode.cn

[R68] 计算文件校验值
来源：http://fgt.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://ios.haohaochexian.top

[R69] 生成随机密码
来源：http://onu.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://wpo.guannengcc.top

[R70] 时间戳与互转
来源：http://iac.fzhhl.top

date +%s;  date -d @1700000000
来源：http://csp.meibo888.top

[R71] 日期格式化
来源：http://okg.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xdp.gzhubu.top

[R72] 等待端口就绪
来源：http://rwx.52xcode.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lli.ppjwa.cn

[R73] 分割大日志
来源：http://usv.ydjk.org.cn

split -l 1000 big.log part_
来源：http://ogr.yj20258.top

[R74] 批量重命名
来源：http://eqa.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://twc.xziqi.cn

[R75] 导出环境变量
来源：http://hke.jiagoushi.top

export PATH="$HOME/bin:$PATH"
来源：http://bhz.zdbjq.cn

[R76] 使用临时文件
来源：http://stt.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aid.sjlbkw.cn

[R77] 读取用户输入
来源：http://bno.hammf.cn

read -rp "请输入: " ans
来源：http://edf.9152youxi.cn

[R78] 交互式菜单
来源：http://sna.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ggd.c1oappe.top

[R79] 解析命令行选项
来源：http://ewj.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tmo.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://tzj.feifeiyinyue.top

time ./run.sh
来源：http://uds.andypj.xyz

================================================================================
来源：http://scq.fengsongda.top

S. C / C++ 专题
来源：http://dfe.yonumen.top

================================================================================
来源：http://ikc.yvedp.cn

[S01] C：Hello World
来源：http://eyq.yj20258.top

#include <stdio.h>
来源：http://isg.sysykeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yzu.wangdashe.top

[S02] C：变量与格式化输出
来源：http://suk.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://gcs.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://hua.jianghu66.top

int x; scanf("%d", &x);
来源：http://sby.quarkkingdee.top

[S04] C：字符串复制
来源：http://cto.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://pwb.chenjidiqi.icu

[S05] C：字符串长度
来源：http://dmc.fengsongda.top

strlen(s)
来源：http://fxq.shangyingyoupin.top

[S06] C：字符串比较
来源：http://jnp.andypj.xyz

strcmp(a, b) == 0
来源：http://fbi.9152youxi.cn

[S07] C：数组遍历求和
来源：http://coh.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aky.cdnleiting.top

[S08] C：动态内存分配与释放
来源：http://nzd.sufxvd.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hmm.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://dkp.hesvh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nrq.hywenlv.cn

[S10] C：指针与解引用
来源：http://poa.yonumen.top

int *p = &a;  *p = 5;
来源：http://sob.cdnleiting.top

[S11] C：逐行读文件
来源：http://rtd.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://csc.nwbrower.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dsw.nanxuanxn.top

fclose(f);
来源：http://xnv.zhijiandao.cn

[S12] C：写文件
来源：http://jkx.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ohl.cashguo.top

[S13] C：宏定义
来源：http://uia.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lgg.svipenyu.cn

[S14] C：枚举
来源：http://skz.52xcode.cn

enum Color { RED, GREEN, BLUE };
来源：http://tzk.fehbvm.com

[S15] C：类型转换
来源：http://vee.gaohongyu789.top

(double) a / b
来源：http://ixq.tanke756.top

[S16] C：位操作置位
来源：http://wss.hnxiangtu.top

x |= (1 << 3);
来源：http://rde.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://sux.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gic.xylfe.cn

[S18] C：命令行参数
来源：http://saf.hywenlv.cn

int main(int argc, char **argv)
来源：http://nqe.xuetiantiany.cn

[S19] C：快速排序
来源：http://xsn.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://jap.hnqzz.top

[S20] C：二分查找
来源：http://gfs.feifeiyinyue.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pxw.jianghu66.top

[S21] C：字符类别判断
来源：http://fah.52xcode.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hca.xuanzx.com

[S22] C：字符串转数字
来源：http://bvd.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://tds.pengpengdd.cyou

[S23] C：随机数
来源：http://kxd.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tar.haohaochexian.top

[S24] C：获取本地时间
来源：http://key.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yys.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://ttc.ctjpmb.com

memcpy(dst, src, n);
来源：http://uwz.ivvv.top

[S26] C：内存清零
来源：http://fua.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://kwl.svipenyu.cn

[S27] C：定义常量
来源：http://zjv.uphjek.com

const double PI = 3.14159;
来源：http://qdu.daxiang520.top

[S28] C：静态变量
来源：http://blf.zdbjq.cn

static int counter = 0;
来源：http://dbu.cheryme.top

[S29] C：变参函数
来源：http://rby.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wpl.dianchejie.cn

[S30] C：头文件保护
来源：http://wmx.haohaochexian.top

#ifndef X_H
来源：http://ycs.aizwys.cn

#define X_H
来源：http://ljn.ppjwa.cn

#endif
来源：http://zno.c1oappe.top

[S31] C++：Hello World
来源：http://xcp.jinqigfzy.top

#include <iostream>
来源：http://yci.c1oappe.top

int main() { std::cout << "Hello\n"; }
来源：http://nzk.bjfxy.top

[S32] C++：字符串
来源：http://wrl.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://qfs.andypj.xyz

[S33] C++：vector 增删
来源：http://ivg.jinqigfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tgd.gogol.net.cn

[S34] C++：遍历 vector
来源：http://hic.ydzc1.top

for (auto &x : v) { std::cout << x; }
来源：http://xns.yj20258888.top

[S35] C++：map
来源：http://qjx.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fex.dashuyun.cn

[S36] C++：unordered_map
来源：http://sbe.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qsk.pycfn.com

[S37] C++：set
来源：http://pry.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hvw.aizwys.cn

[S38] C++：排序
来源：http://zhs.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://ods.xinyue.icu

[S39] C++：自定义比较器排序
来源：http://yaw.fengsongda.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sdp.jinyuanbaomall.cn

[S40] C++：查找元素
来源：http://rcc.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ndp.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://lfj.bjfxy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nqq.vehdjk.com

[S42] C++：继承与虚函数
来源：http://eoz.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://uqy.zhixingplan.top

[S43] C++：智能指针
来源：http://mzw.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://ird.hfpthk.cn

[S44] C++：引用传参
来源：http://asi.andypj.xyz

void inc(int &x) { ++x; }
来源：http://wkf.52xcode.cn

[S45] C++：lambda
来源：http://hin.xingfuxueyuan.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://efo.cucudq.cn

[S46] C++：函数模板
来源：http://nvt.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zgd.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://sco.yanxiufei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://btu.cashguo.top

[S48] C++：逐行读文件
来源：http://uhv.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://tqc.cheryme.top

while (std::getline(in, line)) { }
来源：http://swk.xuetiantiany.cn

[S49] C++：写文件
来源：http://rrz.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ouj.ydzc1.top

[S50] C++：格式化数字
来源：http://dzr.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ugp.cucudq.cn

[S51] C++：显式类型转换
来源：http://pkj.pycfn.com

static_cast<double>(a) / b
来源：http://goc.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://hoh.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://qon.fengsongda.top

[S53] C++：移动语义
来源：http://kpn.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://cii.0kj1m.cn

[S54] C++：异常处理
来源：http://cqh.xuanzx.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fws.fktsv.cn

[S55] C++：结构化绑定
来源：http://mik.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lgt.gotoacloud.top

[S56] C++：optional
来源：http://sxo.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://odh.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://ctz.dashuyun.cn

constexpr int N = 10;
来源：http://mgn.ivvv.top

[S58] C++：命名空间
来源：http://xlz.jinqigufen.top

namespace ns { int f() { return 1; } }
来源：http://giw.guannengcc.top

[S59] C++：静态断言
来源：http://yac.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cdo.nwbrower.top

[S60] C++：遍历并删除元素
来源：http://bqp.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gti.yj20258.top

================================================================================
来源：http://lrg.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fln.yj202588.top

================================================================================
来源：http://qtu.fktsv.cn

[T01] Kotlin：Hello World
来源：http://ato.chenjidiqi.icu

println("Hello")
来源：http://ngt.jianghu66.top

[T02] Kotlin：变量
来源：http://cyf.yj20258888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ioa.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://tcy.zhoulong.xyz

"值: $b"
来源：http://qpd.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://tso.tian-w.cn

val n: String? = null;  n?.length
来源：http://byv.yanxiufei.cn

[T05] Kotlin：when 表达式
来源：http://rcx.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eze.iojbl.cn

[T06] Kotlin：集合映射
来源：http://ech.zhixingplan.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lca.yj202588.top

[T07] Kotlin：集合过滤
来源：http://hjb.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gqg.tanke756.top

[T08] Kotlin：数据类
来源：http://kir.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://blg.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://rpl.vehdjk.com

fun String.exclaim() = this + "!"
来源：http://pij.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://hwq.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://weo.yongpay.top

[T11] Kotlin：协程
来源：http://wyj.yanxiufei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jwf.kuanghao11.cn

[T12] Kotlin：解构声明
来源：http://vyf.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://jca.tarul.cn

[T13] Kotlin：只读 Map
来源：http://zff.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://ewj.chenlongwang.top

[T14] Kotlin：循环
来源：http://oer.xuetiantiany.cn

for (i in 1..10) println(i)
来源：http://abh.shzxlz.cn

[T15] Kotlin：接口
来源：http://ytl.sysykeji.top

interface Shape { fun area(): Double }
来源：http://enl.zhiwuduotai.top

[T16] Swift：Hello World
来源：http://ivb.havefunace.top

print("Hello")
来源：http://hem.nwbrower.top

[T17] Swift：变量与常量
来源：http://jtm.zhixingplan.top

var a = 1;  let b = 2
来源：http://djy.jyoumei.cn

[T18] Swift：字符串插值
来源：http://rik.dashuyun.cn

"值: \(b)"
来源：http://ddf.redwolf501.top

[T19] Swift：可选绑定
来源：http://fjc.sysykeji.top

if let n = opt { print(n) }
来源：http://jfv.meibo888.top

[T20] Swift：数组操作
来源：http://dil.jinghuilouyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mca.smart0.xyz

[T21] Swift：遍历
来源：http://noh.nanxinkj.top

for x in a { print(x) }
来源：http://hpu.kuanghao11.cn

[T22] Swift：字典
来源：http://ydq.ydjk.org.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jsq.fktsv.cn

[T23] Swift：函数
来源：http://bdb.zdqjudy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zez.havefunace.top

[T24] Swift：闭包
来源：http://oay.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oqe.shanyushiyangtech.top

[T25] Swift：结构体
来源：http://fqx.jinqigfzy.top

struct P { var x: Int }
来源：http://xnm.jqgufenzy.top

[T26] Swift：类与重写
来源：http://wjf.sweek.top

class A: Base { override func f() {} }
来源：http://kql.jianghu66.top

[T27] Swift：错误处理
来源：http://fmq.yanxiufei.cn

do { try f() } catch { print(error) }
来源：http://upq.cdnleiting.top

[T28] Swift：枚举
来源：http://zlk.xylfe.cn

enum Color { case red, green }
来源：http://gpr.fanxiaobao.xyz

[T29] Swift：guard 提前返回
来源：http://fmg.ehwqpu.com

guard let x = opt else { return }
来源：http://rdb.yj202588.top

[T30] Swift：协议
来源：http://vux.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://wtu.shanyushiyangtech.top

[T31] Lua：Hello World
来源：http://ebw.xziqi.cn

print("Hello")
来源：http://mom.ydjk.org.cn

[T32] Lua：局部变量
来源：http://qtb.zhijiandao.cn

local a = 1
来源：http://rja.xinyue.icu

[T33] Lua：表（数组）
来源：http://twu.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nyo.haohaochexian.top

[T34] Lua：遍历表
来源：http://fej.jinqigfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yae.ctjpmb.com

[T35] Lua：字典表
来源：http://ari.c1oappe.top

local d = { a = 1 };  d.b = 2
来源：http://vbw.hfpthk.cn

[T36] Lua：函数
来源：http://inz.nanxinkj.top

function add(a, b) return a + b end
来源：http://itx.shangyingyoupin.top

[T37] Lua：字符串拼接
来源：http://ygj.yangfankeji.com

"a" .. "b"
来源：http://osx.yanxiufei.cn

[T38] Lua：条件
来源：http://ovh.tarul.cn

if x > 0 then print("正") end
来源：http://oup.zhixingplan.top

[T39] Lua：模式匹配
来源：http://eja.xinyue.icu

string.find(s, "%d+")
来源：http://ojd.hnxiangtu.top

[T40] Lua：元表
来源：http://mli.shanyushiyangtech.top

setmetatable({}, { __index = base })
来源：http://uhd.yj20258.top

[T41] Perl：Hello World
来源：http://uza.yj202588.top

print "Hello\n";
来源：http://iwj.sjlbkw.cn

[T42] Perl：变量类型
来源：http://pfh.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gjy.nanxinkj.top

[T43] Perl：字符串插值
来源：http://cqv.316326.xyz

"值: $a"
来源：http://ajk.gaohongyu789.top

[T44] Perl：条件
来源：http://upi.0kj1m.cn

if ($a > 0) { print "正"; }
来源：http://yyl.gotoacloud.top

[T45] Perl：数组遍历
来源：http://ngx.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://lnx.bjfxy.top

[T46] Perl：哈希操作
来源：http://jcd.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://you.cdnleiting.top

[T47] Perl：正则捕获
来源：http://hli.feifeiyinyue.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tii.sxryk.cn

[T48] Perl：正则替换
来源：http://luy.tanke756.top

$s =~ s/old/new/g;
来源：http://pin.mhx1999.top

[T49] Perl：函数
来源：http://bfg.yongpay.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xnt.sweek.top

[T50] Perl：逐行读文件
来源：http://ofg.yangfankeji.com

open my $fh, "<", "a.txt" or die $!;
来源：http://epm.mhx1999.top

while (my $line = <$fh>) { print $line; }
来源：http://asg.gotoacloud.top

[T51] Scala：Hello World
来源：http://tjr.jqgfzy.top

println("Hello")
来源：http://gry.ivvv.top

[T52] Scala：变量
来源：http://pjw.tian-w.cn

val a = 1;  var b = 2
来源：http://xbl.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://rmt.nwbrower.top

s"值: $b"
来源：http://yjd.jinqigufen.top

[T54] Scala：集合映射
来源：http://wkr.snrcjt.cn

List(1, 2, 3).map(_ * 2)
来源：http://ggy.hfpthk.cn

[T55] Scala：集合过滤
来源：http://cgu.hfpthk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nkc.cqqwz.cn

[T56] Scala：样例类
来源：http://snu.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://pqq.snrcjt.cn

[T57] Scala：模式匹配
来源：http://llf.wangdashe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bxh.birdmap.top

[T58] Scala：函数定义
来源：http://jeg.gotoacloud.top


<!-- 参考信息 -->