代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://amr.fzhhl.top

[R54] 比较两个文件
来源：http://abx.cashguo.top

diff a.txt b.txt
来源：http://ikp.316326.xyz

[R55] 压缩与解压
来源：http://sje.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xjo.yongpay.top

[R56] 远程拷贝
来源：http://bmx.svipenyu.cn

scp file user@host:/path/
来源：http://rjr.ppjwa.cn

[R57] 远程执行命令
来源：http://xik.aibaodan.cn

ssh user@host 'uptime'
来源：http://fed.tian-w.cn

[R58] 下载文件
来源：http://mzd.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qhd.jinqigfzy.top

[R59] 发 POST JSON
来源：http://xyi.bbcook.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vpm.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://obj.zhijiandao.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ipb.quarkkingdee.top

[R61] 磁盘占用
来源：http://xyl.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://ivs.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://yff.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://cvq.hnqzz.top

[R63] 内存与进程
来源：http://bgb.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://bkd.shzxlz.cn

[R64] 结束进程
来源：http://ivj.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://nrf.mhx1999.top

[R65] 查看端口占用
来源：http://nbd.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rdc.ehwqpu.com

[R66] 定时任务
来源：http://uhh.gzhubu.top

crontab -e;  crontab -l
来源：http://ecy.c1oappe.top

[R67] 生成随机十六进制串
来源：http://hwi.svipenyu.cn

openssl rand -hex 16
来源：http://ivt.jqgufenzy.top

[R68] 计算文件校验值
来源：http://tmd.yanxiufei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hhg.zhixingplan.top

[R69] 生成随机密码
来源：http://ofq.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://qpk.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://lhe.fzhhl.top

date +%s;  date -d @1700000000
来源：http://dpz.zhiwuduotai.top

[R71] 日期格式化
来源：http://wgj.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://svn.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://til.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kbe.jqgufenzy.top

[R73] 分割大日志
来源：http://zvx.tian-w.cn

split -l 1000 big.log part_
来源：http://oip.chenlongwang.top

[R74] 批量重命名
来源：http://zuj.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bjq.gogol.net.cn

[R75] 导出环境变量
来源：http://rrj.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://gqc.redwolf501.top

[R76] 使用临时文件
来源：http://qpc.fehbvm.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://frv.haohaochexian.top

[R77] 读取用户输入
来源：http://ysy.xuetiantiany.cn

read -rp "请输入: " ans
来源：http://hor.birdmap.top

[R78] 交互式菜单
来源：http://yhu.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cdx.xuanzx.com

[R79] 解析命令行选项
来源：http://bmu.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://drb.ehwqpu.com

[R80] 查看脚本执行耗时
来源：http://psg.birdmap.top

time ./run.sh
来源：http://wgk.guannengcc.top

================================================================================
来源：http://qap.shuidangran.top

S. C / C++ 专题
来源：http://jys.zhengqikj.top

================================================================================
来源：http://qfa.zdqjudy.top

[S01] C：Hello World
来源：http://vst.kuanghao11.cn

#include <stdio.h>
来源：http://bjh.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lto.yj202588.top

[S02] C：变量与格式化输出
来源：http://xun.shuidangran.top

int a = 10; printf("%d\n", a);
来源：http://ftk.yfazqb.com

[S03] C：读入整数
来源：http://xug.daxiang520.top

int x; scanf("%d", &x);
来源：http://kev.fzhhl.top

[S04] C：字符串复制
来源：http://swq.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iwt.nanxuanxn.top

[S05] C：字符串长度
来源：http://kdb.chenlongwang.top

strlen(s)
来源：http://snu.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://iqt.hongshengwenyu.top

strcmp(a, b) == 0
来源：http://lkx.pycfn.com

[S07] C：数组遍历求和
来源：http://zdr.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xvd.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://asq.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jqv.zdqjudy.top

[S09] C：结构体定义与初始化
来源：http://vgg.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zea.jqgfzy.top

[S10] C：指针与解引用
来源：http://wxx.ivvv.top

int *p = &a;  *p = 5;
来源：http://fpo.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://sha.quarkkingdee.top

FILE *f = fopen("a.txt", "r");
来源：http://sgy.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://spn.svipenyu.cn

fclose(f);
来源：http://xad.zhengqikj.top

[S12] C：写文件
来源：http://tcb.0kj1m.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://plj.tanke756.top

[S13] C：宏定义
来源：http://fpf.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://whx.guannengcc.top

[S14] C：枚举
来源：http://xkz.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://bwp.hnqzz.top

[S15] C：类型转换
来源：http://lcx.fehbvm.com

(double) a / b
来源：http://fes.hesvh.cn

[S16] C：位操作置位
来源：http://sve.zycfv.cn

x |= (1 << 3);
来源：http://hti.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://uoz.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cpr.yanxiufei.cn

[S18] C：命令行参数
来源：http://mgq.vqdsnc.cn

int main(int argc, char **argv)
来源：http://bqc.yfazqb.com

[S19] C：快速排序
来源：http://sju.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lnp.cheryme.top

[S20] C：二分查找
来源：http://fxb.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gwx.yj202588.top

[S21] C：字符类别判断
来源：http://wva.yonumen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vft.yongpay.top

[S22] C：字符串转数字
来源：http://lnw.yvedp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://okq.smart0.xyz

[S23] C：随机数
来源：http://sbx.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sgm.shanyushiyangtech.top

[S24] C：获取本地时间
来源：http://vhk.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://agq.aizwys.cn

[S25] C：内存拷贝
来源：http://hjz.nanxinkj.top

memcpy(dst, src, n);
来源：http://ieu.bbcook.cn

[S26] C：内存清零
来源：http://xvl.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://thg.tian-w.cn

[S27] C：定义常量
来源：http://agw.nwbrower.top

const double PI = 3.14159;
来源：http://czw.zhiwuduotai.top

[S28] C：静态变量
来源：http://hwh.hywenlv.cn

static int counter = 0;
来源：http://tdk.chenzaomai.com

[S29] C：变参函数
来源：http://iqh.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ola.redwolf501.top

[S30] C：头文件保护
来源：http://fya.fktsv.cn

#ifndef X_H
来源：http://wlt.c1oappe.top

#define X_H
来源：http://tfl.hnxiangtu.top

#endif
来源：http://urt.aibaodan.cn

[S31] C++：Hello World
来源：http://dlg.zhengqikj.top

#include <iostream>
来源：http://qde.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://alb.feifeiyinyue.top

[S32] C++：字符串
来源：http://oiv.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://fau.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://byd.shuidangran.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tdo.tian-w.cn

[S34] C++：遍历 vector
来源：http://xev.mhx1999.top

for (auto &x : v) { std::cout << x; }
来源：http://trc.epnwcf.com

[S35] C++：map
来源：http://moz.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pvg.yuanzhike.top

[S36] C++：unordered_map
来源：http://onf.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://plz.birdmap.top

[S37] C++：set
来源：http://roo.0kj1m.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ojf.tarul.cn

[S38] C++：排序
来源：http://qoz.xinyue.icu

std::sort(v.begin(), v.end());
来源：http://vaf.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://hxw.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zdh.ehwqpu.com

[S40] C++：查找元素
来源：http://gxv.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lam.nwbrower.top

[S41] C++：类与构造函数
来源：http://osz.hnxiangtu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ntn.0kj1m.cn

[S42] C++：继承与虚函数
来源：http://qkk.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://fxi.hongshengwenyu.top

[S43] C++：智能指针
来源：http://qip.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://pqs.gzhubu.top

[S44] C++：引用传参
来源：http://ark.sjlbkw.cn

void inc(int &x) { ++x; }
来源：http://xnw.fanxiaobao.xyz

[S45] C++：lambda
来源：http://sir.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hxo.feifeiyinyue.top

[S46] C++：函数模板
来源：http://iek.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://csp.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://txq.smart0.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ivj.hfpthk.cn

[S48] C++：逐行读文件
来源：http://ycz.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://lht.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://fvo.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://otk.9152youxi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rjh.gogol.net.cn

[S50] C++：格式化数字
来源：http://iap.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://smb.chenjidiqi.icu

[S51] C++：显式类型转换
来源：http://ptd.tarul.cn

static_cast<double>(a) / b
来源：http://vjj.zdqjudy.top

[S52] C++：const 与 noexcept
来源：http://jyg.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://aye.zhengqikj.top

[S53] C++：移动语义
来源：http://vqd.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://hya.fengsongda.top

[S54] C++：异常处理
来源：http://fez.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cqk.andypj.xyz

[S55] C++：结构化绑定
来源：http://hgy.ydjk.org.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ojm.yfazqb.com

[S56] C++：optional
来源：http://aze.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lsd.yj202588.top

[S57] C++：编译期常量
来源：http://epc.meibo888.top

constexpr int N = 10;
来源：http://ant.jinqigufen.top

[S58] C++：命名空间
来源：http://dgy.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://qyx.jinqigufen.top

[S59] C++：静态断言
来源：http://zgr.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://htg.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://roa.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oay.dianchejie.cn

================================================================================
来源：http://iei.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xld.zhongyouzk.top

================================================================================
来源：http://ihb.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://mze.dashuyun.cn

println("Hello")
来源：http://gin.hesvh.cn

[T02] Kotlin：变量
来源：http://tto.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nxy.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://vto.jqgfzy.top

"值: $b"
来源：http://fpb.zdbjq.cn

[T04] Kotlin：空安全
来源：http://zmc.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://nol.hammf.cn

[T05] Kotlin：when 表达式
来源：http://zwn.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xcu.yongpay.top

[T06] Kotlin：集合映射
来源：http://prl.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ffa.nwbrower.top

[T07] Kotlin：集合过滤
来源：http://beb.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tql.vehdjk.com

[T08] Kotlin：数据类
来源：http://jta.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://pbk.fzhhl.top

[T09] Kotlin：扩展函数
来源：http://zmd.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://yah.yvedp.cn

[T10] Kotlin：默认参数
来源：http://lxj.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hma.ehwqpu.com

[T11] Kotlin：协程
来源：http://ntn.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hom.pycfn.com

[T12] Kotlin：解构声明
来源：http://mhs.9152youxi.cn

val (a, b) = Pair(1, 2)
来源：http://axz.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://bnw.fengsongda.top

val m = mapOf("a" to 1)
来源：http://sef.meibo888.top

[T14] Kotlin：循环
来源：http://lmj.jyoumei.cn

for (i in 1..10) println(i)
来源：http://wcl.ydzc1.top

[T15] Kotlin：接口
来源：http://rgz.yfazqb.com

interface Shape { fun area(): Double }
来源：http://ytz.yj20258888.top

[T16] Swift：Hello World
来源：http://ytd.cucudq.cn

print("Hello")
来源：http://ptc.jqgfzy.top

[T17] Swift：变量与常量
来源：http://mqi.havefunace.top

var a = 1;  let b = 2
来源：http://lcw.snrcjt.cn

[T18] Swift：字符串插值
来源：http://veb.yfazqb.com

"值: \(b)"
来源：http://ltl.gotoacloud.top

[T19] Swift：可选绑定
来源：http://hke.haohaochexian.top

if let n = opt { print(n) }
来源：http://iwr.jlsjyb.cn

[T20] Swift：数组操作
来源：http://hct.ywan-chungtsiang.top

var a = [1, 2, 3];  a.append(4)
来源：http://rxo.snrcjt.cn

[T21] Swift：遍历
来源：http://iuy.zhixingplan.top

for x in a { print(x) }
来源：http://bpt.yvedp.cn

[T22] Swift：字典
来源：http://aes.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lmw.ppjwa.cn

[T23] Swift：函数
来源：http://pjx.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ntt.haohaochexian.top

[T24] Swift：闭包
来源：http://tan.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ajl.52xcode.cn

[T25] Swift：结构体
来源：http://ccs.sweek.top

struct P { var x: Int }
来源：http://zbs.birdmap.top

[T26] Swift：类与重写
来源：http://gcx.cashguo.top

class A: Base { override func f() {} }
来源：http://qid.ybcxt.top

[T27] Swift：错误处理
来源：http://nkz.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://tij.cdnleiting.top

[T28] Swift：枚举
来源：http://tms.snrcjt.cn

enum Color { case red, green }
来源：http://jsx.xingfuxueyuan.xyz

[T29] Swift：guard 提前返回
来源：http://gjj.birdmap.top

guard let x = opt else { return }
来源：http://orl.xuetiantiany.cn

[T30] Swift：协议
来源：http://doj.birdmap.top

protocol Shape { func area() -> Double }
来源：http://xga.ydzc1.top

[T31] Lua：Hello World
来源：http://wmw.hammf.cn

print("Hello")
来源：http://lyf.hnxiangtu.top

[T32] Lua：局部变量
来源：http://din.chenzaomai.com

local a = 1
来源：http://zkj.epnwcf.com

[T33] Lua：表（数组）
来源：http://wuk.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dox.bbcook.cn

[T34] Lua：遍历表
来源：http://zqy.hfpthk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yfl.sjlbkw.cn

[T35] Lua：字典表
来源：http://tty.havefunace.top

local d = { a = 1 };  d.b = 2
来源：http://irg.dianchejie.cn

[T36] Lua：函数
来源：http://toc.uphjek.com

function add(a, b) return a + b end
来源：http://ema.daria6918.cn

[T37] Lua：字符串拼接
来源：http://luj.sufxvd.cn

"a" .. "b"
来源：http://xsn.316326.xyz

[T38] Lua：条件
来源：http://opq.zhiwuduotai.top

if x > 0 then print("正") end
来源：http://zuh.0kj1m.cn

[T39] Lua：模式匹配
来源：http://zrw.tarul.cn

string.find(s, "%d+")
来源：http://ugc.cdnleiting.top

[T40] Lua：元表
来源：http://lol.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://vhl.zycfv.cn

[T41] Perl：Hello World
来源：http://xbk.hywenlv.cn

print "Hello\n";
来源：http://jho.fehbvm.com

[T42] Perl：变量类型
来源：http://rmg.dianchejie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pwc.yueranfly.top

[T43] Perl：字符串插值
来源：http://jgg.fzhhl.top

"值: $a"
来源：http://tgg.nanxinkj.top

[T44] Perl：条件
来源：http://fhn.52xcode.cn

if ($a > 0) { print "正"; }
来源：http://raq.meibo888.top

[T45] Perl：数组遍历
来源：http://hde.tarul.cn

for my $x (@arr) { print $x; }
来源：http://viv.zhengqikj.top

[T46] Perl：哈希操作
来源：http://uvo.316326.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://spl.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://kgt.fengsongda.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zkf.zhixingplan.top

[T48] Perl：正则替换
来源：http://dnf.chenjidiqi.icu

$s =~ s/old/new/g;
来源：http://ewc.jinqigufen.top

[T49] Perl：函数
来源：http://kcy.jinqigfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uwz.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://rav.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xkw.zhengqikj.top

while (my $line = <$fh>) { print $line; }
来源：http://oiv.shuidangran.top

[T51] Scala：Hello World
来源：http://cfj.fktsv.cn

println("Hello")
来源：http://iyn.zhengqikj.top

[T52] Scala：变量
来源：http://ezl.andypj.xyz

val a = 1;  var b = 2
来源：http://dwp.hesvh.cn

[T53] Scala：字符串插值
来源：http://yug.iojbl.cn

s"值: $b"
来源：http://vng.jiagoushi.top

[T54] Scala：集合映射
来源：http://nex.nanxuanxn.top

List(1, 2, 3).map(_ * 2)
来源：http://fqi.ppjwa.cn

[T55] Scala：集合过滤
来源：http://exy.yongpay.top

List(1, 2, 3).filter(_ > 1)
来源：http://foy.sjlbkw.cn

[T56] Scala：样例类
来源：http://zyg.meibo888.top


<!-- 参考信息 -->