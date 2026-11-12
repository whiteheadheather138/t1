代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hmy.shangyingyoupin.top

[R56] 远程拷贝
来源：http://ixi.ehwqpu.com

scp file user@host:/path/
来源：http://qmk.0kj1m.cn

[R57] 远程执行命令
来源：http://eas.hongshengwenyu.top

ssh user@host 'uptime'
来源：http://sgi.hywenlv.cn

[R58] 下载文件
来源：http://mxh.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hff.shanyushiyangtech.top

[R59] 发 POST JSON
来源：http://jgy.gotoacloud.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fue.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://miw.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rab.nanxinkj.top

[R61] 磁盘占用
来源：http://jpm.jinghuilouyu.cn

df -h;  du -sh *
来源：http://own.chenzaomai.com

[R62] 找最占空间的文件
来源：http://ucq.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://dnq.guannengcc.top

[R63] 内存与进程
来源：http://lyf.hesvh.cn

free -h;  ps aux | grep nginx
来源：http://rdy.jianghu66.top

[R64] 结束进程
来源：http://lqp.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://bhd.ybcxt.top

[R65] 查看端口占用
来源：http://yzy.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cqq.gzhubu.top

[R66] 定时任务
来源：http://ovj.hywenlv.cn

crontab -e;  crontab -l
来源：http://eer.havefunace.top

[R67] 生成随机十六进制串
来源：http://hdh.nwbrower.top

openssl rand -hex 16
来源：http://zbr.ppjwa.cn

[R68] 计算文件校验值
来源：http://zhe.xinyue.icu

sha256sum a.txt;  md5sum a.txt
来源：http://uii.bjfxy.top

[R69] 生成随机密码
来源：http://rnk.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://ihs.ctjpmb.com

[R70] 时间戳与互转
来源：http://eit.nwbrower.top

date +%s;  date -d @1700000000
来源：http://rqu.aizwys.cn

[R71] 日期格式化
来源：http://zqd.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wsd.snrcjt.cn

[R72] 等待端口就绪
来源：http://anr.birdmap.top

until nc -z localhost 3306; do sleep 1; done
来源：http://otm.c1oappe.top

[R73] 分割大日志
来源：http://azk.cqqwz.cn

split -l 1000 big.log part_
来源：http://arh.gotoacloud.top

[R74] 批量重命名
来源：http://igi.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blr.ybcxt.top

[R75] 导出环境变量
来源：http://qsu.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://yzv.fzhhl.top

[R76] 使用临时文件
来源：http://oay.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qgm.xylfe.cn

[R77] 读取用户输入
来源：http://hqy.zhixingplan.top

read -rp "请输入: " ans
来源：http://yux.shuidangran.top

[R78] 交互式菜单
来源：http://wfi.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://drw.redwolf501.top

[R79] 解析命令行选项
来源：http://vkj.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bmw.cheryme.top

[R80] 查看脚本执行耗时
来源：http://zww.zhiwuduotai.top

time ./run.sh
来源：http://ufl.316326.xyz

================================================================================
来源：http://zux.gogol.net.cn

S. C / C++ 专题
来源：http://qnz.chenzaomai.com

================================================================================
来源：http://yud.hammf.cn

[S01] C：Hello World
来源：http://mpo.yanxiufei.cn

#include <stdio.h>
来源：http://alo.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zdc.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://dbj.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://yxr.aizwys.cn

[S03] C：读入整数
来源：http://tyx.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://jjm.hnxiangtu.top

[S04] C：字符串复制
来源：http://qwy.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dtw.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://yho.jianghu66.top

strlen(s)
来源：http://vss.9152youxi.cn

[S06] C：字符串比较
来源：http://fzb.jyoumei.cn

strcmp(a, b) == 0
来源：http://zti.cucudq.cn

[S07] C：数组遍历求和
来源：http://bbq.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qxt.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://nem.yongpay.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ibr.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://ryh.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xgv.ehwqpu.com

[S10] C：指针与解引用
来源：http://ggj.sufxvd.cn

int *p = &a;  *p = 5;
来源：http://byg.xziqi.cn

[S11] C：逐行读文件
来源：http://yjh.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://net.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yzk.ydzc1.top

fclose(f);
来源：http://nqs.svipenyu.cn

[S12] C：写文件
来源：http://sji.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fvc.gaohongyu789.top

[S13] C：宏定义
来源：http://xyp.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ymj.yj20258.top

[S14] C：枚举
来源：http://onc.zhaomingkeji.xyz

enum Color { RED, GREEN, BLUE };
来源：http://tlz.yfazqb.com

[S15] C：类型转换
来源：http://quy.sysykeji.top

(double) a / b
来源：http://lyk.shuidangran.top

[S16] C：位操作置位
来源：http://cju.ydjk.org.cn

x |= (1 << 3);
来源：http://cae.fengsongda.top

[S17] C：安全拼接字符串
来源：http://ogf.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://poy.jinghuilouyu.cn

[S18] C：命令行参数
来源：http://xeh.quarkkingdee.top

int main(int argc, char **argv)
来源：http://ebu.shuidangran.top

[S19] C：快速排序
来源：http://ccc.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://ffb.gogol.net.cn

[S20] C：二分查找
来源：http://ham.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://did.52xcode.cn

[S21] C：字符类别判断
来源：http://sxj.cucudq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lta.hysaishi.cn

[S22] C：字符串转数字
来源：http://iwe.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://zpp.yueranfly.top

[S23] C：随机数
来源：http://dam.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ptr.mhx1999.top

[S24] C：获取本地时间
来源：http://jrm.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pof.yvedp.cn

[S25] C：内存拷贝
来源：http://hkw.meibo888.top

memcpy(dst, src, n);
来源：http://pwd.hnqzz.top

[S26] C：内存清零
来源：http://drd.yfazqb.com

memset(a, 0, sizeof a);
来源：http://fwq.dashuyun.cn

[S27] C：定义常量
来源：http://zzu.hcnkem.com

const double PI = 3.14159;
来源：http://cps.svipenyu.cn

[S28] C：静态变量
来源：http://ttt.ybcxt.top

static int counter = 0;
来源：http://yir.birdmap.top

[S29] C：变参函数
来源：http://boz.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qdt.yfazqb.com

[S30] C：头文件保护
来源：http://lip.shzxlz.cn

#ifndef X_H
来源：http://vyg.yfazqb.com

#define X_H
来源：http://fyk.ydzc1.top

#endif
来源：http://zhy.52xcode.cn

[S31] C++：Hello World
来源：http://sua.gaohongyu789.top

#include <iostream>
来源：http://iyo.cucudq.cn

int main() { std::cout << "Hello\n"; }
来源：http://qkc.sxryk.cn

[S32] C++：字符串
来源：http://jlh.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://neg.vqdsnc.cn

[S33] C++：vector 增删
来源：http://bxi.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jss.shzxlz.cn

[S34] C++：遍历 vector
来源：http://ryd.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://sik.shzxlz.cn

[S35] C++：map
来源：http://ryq.xziqi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wyc.zdqjudy.top

[S36] C++：unordered_map
来源：http://nwi.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aqg.bbcook.cn

[S37] C++：set
来源：http://sje.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://isp.aizwys.cn

[S38] C++：排序
来源：http://frs.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://zjn.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://uwm.yvedp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bmg.jiagoushi.top

[S40] C++：查找元素
来源：http://nyt.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jvh.hesvh.cn

[S41] C++：类与构造函数
来源：http://jzd.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jnd.uphjek.com

[S42] C++：继承与虚函数
来源：http://iau.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://hfo.pycfn.com

[S43] C++：智能指针
来源：http://qje.pengpengdd.cyou

auto p = std::make_unique<int>(5);
来源：http://obr.0kj1m.cn

[S44] C++：引用传参
来源：http://pvw.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://plh.guowangkeji.top

[S45] C++：lambda
来源：http://jyt.hammf.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yog.ydzc1.top

[S46] C++：函数模板
来源：http://zyf.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xng.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://utj.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pqb.fengsongda.top

[S48] C++：逐行读文件
来源：http://vgk.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://ysm.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://eik.chenzaomai.com

[S49] C++：写文件
来源：http://due.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qhk.zhoulong.xyz

[S50] C++：格式化数字
来源：http://rxz.feifeiyinyue.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://boj.shanyushiyangkeji.top

[S51] C++：显式类型转换
来源：http://cpv.sufxvd.cn

static_cast<double>(a) / b
来源：http://web.cheryme.top

[S52] C++：const 与 noexcept
来源：http://vub.yuanzhike.top

int size() const noexcept { return n_; }
来源：http://doc.hammf.cn

[S53] C++：移动语义
来源：http://lfw.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://prz.meibo888.top

[S54] C++：异常处理
来源：http://frt.yvedp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vdk.epnwcf.com

[S55] C++：结构化绑定
来源：http://jwh.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jzf.chenzaomai.com

[S56] C++：optional
来源：http://vna.jqgufenzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xhv.snrcjt.cn

[S57] C++：编译期常量
来源：http://pib.sysykeji.top

constexpr int N = 10;
来源：http://yhg.zhixingplan.top

[S58] C++：命名空间
来源：http://bwb.uphjek.com

namespace ns { int f() { return 1; } }
来源：http://vrl.epnwcf.com

[S59] C++：静态断言
来源：http://azs.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zey.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://ckk.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://osu.sysykeji.top

================================================================================
来源：http://jsw.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ftb.dashuyun.cn

================================================================================
来源：http://nlr.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://oou.guowangkeji.top

println("Hello")
来源：http://tev.xuanzx.com

[T02] Kotlin：变量
来源：http://jum.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://elv.havefunace.top

[T03] Kotlin：字符串模板
来源：http://xyf.vehdjk.com

"值: $b"
来源：http://qxz.hnqzz.top

[T04] Kotlin：空安全
来源：http://ucz.nanxuanxn.top

val n: String? = null;  n?.length
来源：http://xhy.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://kxe.hfpthk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pwp.birdmap.top

[T06] Kotlin：集合映射
来源：http://mwf.zycfv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lsv.shanyushiyangkeji.top

[T07] Kotlin：集合过滤
来源：http://xnn.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://nkv.jianghu66.top

[T08] Kotlin：数据类
来源：http://gmy.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://ddh.meibo888.top

[T09] Kotlin：扩展函数
来源：http://ujd.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://qbz.wangdashe.top

[T10] Kotlin：默认参数
来源：http://sgw.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ces.daxiang520.top

[T11] Kotlin：协程
来源：http://waw.52xcode.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jew.c1oappe.top

[T12] Kotlin：解构声明
来源：http://ire.xinyue.icu

val (a, b) = Pair(1, 2)
来源：http://uuu.ywan-chungtsiang.top

[T13] Kotlin：只读 Map
来源：http://jxv.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://ros.tarul.cn

[T14] Kotlin：循环
来源：http://jrp.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://wer.jqgufenzy.top

[T15] Kotlin：接口
来源：http://qdt.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://krp.yfazqb.com

[T16] Swift：Hello World
来源：http://eez.jyoumei.cn

print("Hello")
来源：http://tjs.haohaochexian.top

[T17] Swift：变量与常量
来源：http://xcw.jianghu66.top

var a = 1;  let b = 2
来源：http://xzp.tian-w.cn

[T18] Swift：字符串插值
来源：http://giv.shangyingyoupin.top

"值: \(b)"
来源：http://aqg.smart0.xyz

[T19] Swift：可选绑定
来源：http://ifq.sxryk.cn

if let n = opt { print(n) }
来源：http://scr.shuidangran.top

[T20] Swift：数组操作
来源：http://xsw.hysaishi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://juo.sjlbkw.cn

[T21] Swift：遍历
来源：http://cmi.gzhubu.top

for x in a { print(x) }
来源：http://qun.yueranfly.top

[T22] Swift：字典
来源：http://lpw.pengpengdd.cyou

var d = ["a": 1];  d["b"] = 2
来源：http://nkr.xziqi.cn

[T23] Swift：函数
来源：http://qle.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lde.cqqwz.cn

[T24] Swift：闭包
来源：http://qyg.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://wjc.hammf.cn

[T25] Swift：结构体
来源：http://son.vehdjk.com

struct P { var x: Int }
来源：http://zkk.svipenyu.cn

[T26] Swift：类与重写
来源：http://vlk.nanxinkj.top

class A: Base { override func f() {} }
来源：http://mrb.yj20258888.top

[T27] Swift：错误处理
来源：http://brs.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://kzn.hesvh.cn

[T28] Swift：枚举
来源：http://gii.jyoumei.cn

enum Color { case red, green }
来源：http://cab.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://qxe.ivvv.top

guard let x = opt else { return }
来源：http://jhv.tian-w.cn

[T30] Swift：协议
来源：http://ghe.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://zrf.52xcode.cn

[T31] Lua：Hello World
来源：http://bql.xziqi.cn

print("Hello")
来源：http://tzp.nwbrower.top

[T32] Lua：局部变量
来源：http://vde.tarul.cn

local a = 1
来源：http://yio.aibaodan.cn

[T33] Lua：表（数组）
来源：http://mry.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://yez.snrcjt.cn

[T34] Lua：遍历表
来源：http://ywq.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hye.yuxming.cn

[T35] Lua：字典表
来源：http://ngn.zhijiandao.cn

local d = { a = 1 };  d.b = 2
来源：http://giz.yj20258888.top

[T36] Lua：函数
来源：http://sjw.hammf.cn

function add(a, b) return a + b end
来源：http://fka.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://dfj.yanxiufei.cn

"a" .. "b"
来源：http://mgk.yvedp.cn

[T38] Lua：条件
来源：http://kbl.xinyue.icu

if x > 0 then print("正") end
来源：http://wln.xuanzx.com

[T39] Lua：模式匹配
来源：http://meq.0kj1m.cn

string.find(s, "%d+")
来源：http://icf.jiagoushi.top

[T40] Lua：元表
来源：http://iun.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://xjj.c1oappe.top

[T41] Perl：Hello World
来源：http://efr.yuxming.cn

print "Hello\n";
来源：http://uyl.sjlbkw.cn

[T42] Perl：变量类型
来源：http://lab.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rky.ydzc1.top

[T43] Perl：字符串插值
来源：http://hxd.daxiang520.top

"值: $a"
来源：http://zvn.smart0.xyz

[T44] Perl：条件
来源：http://nex.ehwqpu.com

if ($a > 0) { print "正"; }
来源：http://bsp.birdmap.top

[T45] Perl：数组遍历
来源：http://dld.316326.xyz

for my $x (@arr) { print $x; }
来源：http://jrm.tarul.cn

[T46] Perl：哈希操作
来源：http://quh.shuidangran.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dwx.xingfuxueyuan.xyz

[T47] Perl：正则捕获
来源：http://iai.uphjek.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://cqv.mhx1999.top

[T48] Perl：正则替换
来源：http://jgh.jqgfzy.top

$s =~ s/old/new/g;
来源：http://okj.zhengqikj.top

[T49] Perl：函数
来源：http://vot.chenjidiqi.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wan.nanxuanxn.top

[T50] Perl：逐行读文件
来源：http://swn.zhiwuduotai.top

open my $fh, "<", "a.txt" or die $!;
来源：http://znz.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://mqc.hnxiangtu.top

[T51] Scala：Hello World
来源：http://gmi.jiagoushi.top

println("Hello")
来源：http://yyq.jqgufenzy.top

[T52] Scala：变量
来源：http://gob.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://mci.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://tod.shangyingyoupin.top

s"值: $b"
来源：http://goh.pengpengdd.cyou

[T54] Scala：集合映射
来源：http://zlv.316326.xyz

List(1, 2, 3).map(_ * 2)
来源：http://puv.dashuyun.cn

[T55] Scala：集合过滤
来源：http://pek.birdmap.top

List(1, 2, 3).filter(_ > 1)
来源：http://jto.havefunace.top

[T56] Scala：样例类
来源：http://xxl.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://kap.tianlin.xyz

[T57] Scala：模式匹配
来源：http://tvv.mhx1999.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uqg.zycfv.cn

[T58] Scala：函数定义
来源：http://ncz.ybcxt.top


<!-- 参考信息 -->