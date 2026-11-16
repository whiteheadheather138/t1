代发 wailian999

ssh user@host 'uptime'
来源：http://tje.aibaodan.cn

[R58] 下载文件
来源：http://abr.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://msi.yangfankeji.com

[R59] 发 POST JSON
来源：http://cee.shzxlz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://grs.quarkkingdee.top

[R60] 只看 HTTP 状态码
来源：http://txg.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://inz.shangyingyoupin.top

[R61] 磁盘占用
来源：http://pww.ywan-chungtsiang.top

df -h;  du -sh *
来源：http://igm.zdbjq.cn

[R62] 找最占空间的文件
来源：http://dby.jinqigufen.top

du -ah . | sort -rh | head -10
来源：http://vya.quarkkingdee.top

[R63] 内存与进程
来源：http://ony.tarul.cn

free -h;  ps aux | grep nginx
来源：http://ikd.zhixingplan.top

[R64] 结束进程
来源：http://ftq.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://iwj.quarkkingdee.top

[R65] 查看端口占用
来源：http://fyh.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uan.52xcode.cn

[R66] 定时任务
来源：http://jbs.aizwys.cn

crontab -e;  crontab -l
来源：http://fyo.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://tve.havefunace.top

openssl rand -hex 16
来源：http://alv.hesvh.cn

[R68] 计算文件校验值
来源：http://aaz.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jhn.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://bwy.xuetiantiany.cn

head -c 16 /dev/urandom | base64
来源：http://xsj.yongpay.top

[R70] 时间戳与互转
来源：http://uxi.fktsv.cn

date +%s;  date -d @1700000000
来源：http://ury.zhijiandao.cn

[R71] 日期格式化
来源：http://xms.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dlw.hesvh.cn

[R72] 等待端口就绪
来源：http://auq.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gsk.uphjek.com

[R73] 分割大日志
来源：http://wfd.hcnkem.com

split -l 1000 big.log part_
来源：http://afo.yj20258.top

[R74] 批量重命名
来源：http://fni.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ixe.jqgufenzy.top

[R75] 导出环境变量
来源：http://nxf.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://ljq.sysykeji.top

[R76] 使用临时文件
来源：http://nde.xziqi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://njl.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://uzh.aibaodan.cn

read -rp "请输入: " ans
来源：http://kkz.haohaochexian.top

[R78] 交互式菜单
来源：http://jdt.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rib.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://obk.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mpx.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://fnu.tanke756.top

time ./run.sh
来源：http://esp.tarul.cn

================================================================================
来源：http://vhr.dianchejie.cn

S. C / C++ 专题
来源：http://qpo.hywenlv.cn

================================================================================
来源：http://iim.yfazqb.com

[S01] C：Hello World
来源：http://daf.52xcode.cn

#include <stdio.h>
来源：http://lck.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yvg.yongpay.top

[S02] C：变量与格式化输出
来源：http://vbk.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://gbw.jyoumei.cn

[S03] C：读入整数
来源：http://uit.fktsv.cn

int x; scanf("%d", &x);
来源：http://ecv.guannengcc.top

[S04] C：字符串复制
来源：http://dnf.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://xxc.jinqigfzy.top

[S05] C：字符串长度
来源：http://blr.ppjwa.cn

strlen(s)
来源：http://psm.guowangkeji.top

[S06] C：字符串比较
来源：http://iqq.tianlin.xyz

strcmp(a, b) == 0
来源：http://awj.yuanzhike.top

[S07] C：数组遍历求和
来源：http://jql.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cco.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://wyr.hnqzz.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mei.gzhubu.top

[S09] C：结构体定义与初始化
来源：http://ldf.sweek.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tsk.pycfn.com

[S10] C：指针与解引用
来源：http://mny.yonumen.top

int *p = &a;  *p = 5;
来源：http://vpb.ydzc1.top

[S11] C：逐行读文件
来源：http://caf.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://aiw.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lkn.epnwcf.com

fclose(f);
来源：http://yrb.yuxming.cn

[S12] C：写文件
来源：http://rlg.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lpg.jiagoushi.top

[S13] C：宏定义
来源：http://urc.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://myu.haohaochexian.top

[S14] C：枚举
来源：http://uvj.sxryk.cn

enum Color { RED, GREEN, BLUE };
来源：http://plk.ctjpmb.com

[S15] C：类型转换
来源：http://nbt.zhengqikj.top

(double) a / b
来源：http://lnm.zhixingplan.top

[S16] C：位操作置位
来源：http://pbs.yangfankeji.com

x |= (1 << 3);
来源：http://qmz.hammf.cn

[S17] C：安全拼接字符串
来源：http://svw.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cdf.chenlongwang.top

[S18] C：命令行参数
来源：http://quu.jinghuilouyu.cn

int main(int argc, char **argv)
来源：http://oxp.hysaishi.cn

[S19] C：快速排序
来源：http://ylk.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://dfb.52xcode.cn

[S20] C：二分查找
来源：http://wdp.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dgv.shanyushiyangkeji.top

[S21] C：字符类别判断
来源：http://yng.haohaochexian.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pfv.yuxming.cn

[S22] C：字符串转数字
来源：http://rdp.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rfj.gogol.net.cn

[S23] C：随机数
来源：http://uhf.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mfe.gaohongyu789.top

[S24] C：获取本地时间
来源：http://ejf.nwbrower.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yah.hfpthk.cn

[S25] C：内存拷贝
来源：http://zlv.0kj1m.cn

memcpy(dst, src, n);
来源：http://llq.andypj.xyz

[S26] C：内存清零
来源：http://uvb.ivvv.top

memset(a, 0, sizeof a);
来源：http://ptz.nanxuanxn.top

[S27] C：定义常量
来源：http://zmc.hongshengwenyu.top

const double PI = 3.14159;
来源：http://xob.fengsongda.top

[S28] C：静态变量
来源：http://myz.xinyue.icu

static int counter = 0;
来源：http://nvg.cashguo.top

[S29] C：变参函数
来源：http://vrs.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ghh.nanxinkj.top

[S30] C：头文件保护
来源：http://fxg.shzxlz.cn

#ifndef X_H
来源：http://ejz.ydjk.org.cn

#define X_H
来源：http://alc.snrcjt.cn

#endif
来源：http://zap.ppjwa.cn

[S31] C++：Hello World
来源：http://ihy.yanxiufei.cn

#include <iostream>
来源：http://znd.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://rrl.ehwqpu.com

[S32] C++：字符串
来源：http://aex.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://sas.sweek.top

[S33] C++：vector 增删
来源：http://cec.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fpw.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://giq.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://jhu.hcnkem.com

[S35] C++：map
来源：http://tqq.yj20258.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bjv.svipenyu.cn

[S36] C++：unordered_map
来源：http://ynb.sjlbkw.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://snm.birdmap.top

[S37] C++：set
来源：http://mak.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sue.cashguo.top

[S38] C++：排序
来源：http://pjv.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://dbh.0kj1m.cn

[S39] C++：自定义比较器排序
来源：http://hbj.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tbb.ehwqpu.com

[S40] C++：查找元素
来源：http://iaa.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://viy.quarkkingdee.top

[S41] C++：类与构造函数
来源：http://stg.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://igc.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://bzl.gaohongyu789.top

class B : public Base { public: void f() override {} };
来源：http://mxu.kuanghao11.cn

[S43] C++：智能指针
来源：http://alz.svipenyu.cn

auto p = std::make_unique<int>(5);
来源：http://czr.hnxiangtu.top

[S44] C++：引用传参
来源：http://asc.daxiang520.top

void inc(int &x) { ++x; }
来源：http://vgp.daxiang520.top

[S45] C++：lambda
来源：http://qyw.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://gss.tianlin.xyz

[S46] C++：函数模板
来源：http://ieu.hnxiangtu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oxj.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://fnb.snrcjt.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yux.mhx1999.top

[S48] C++：逐行读文件
来源：http://zzl.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://hsq.chenzaomai.com

while (std::getline(in, line)) { }
来源：http://fjd.nwbrower.top

[S49] C++：写文件
来源：http://emm.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tnc.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://cfk.fengsongda.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://evu.hnqzz.top

[S51] C++：显式类型转换
来源：http://aqe.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://dcq.zdqjudy.top

[S52] C++：const 与 noexcept
来源：http://bcx.sysykeji.top

int size() const noexcept { return n_; }
来源：http://tvu.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://ebf.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://zah.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://cpe.ydjk.org.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fyb.xingfuxueyuan.xyz

[S55] C++：结构化绑定
来源：http://och.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pov.tarul.cn

[S56] C++：optional
来源：http://hmf.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tcy.dashuyun.cn

[S57] C++：编译期常量
来源：http://ndi.hongshengwenyu.top

constexpr int N = 10;
来源：http://tgr.hesvh.cn

[S58] C++：命名空间
来源：http://cac.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://nfy.yvedp.cn

[S59] C++：静态断言
来源：http://dfe.yuanzhike.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gdg.jinqigfzy.top

[S60] C++：遍历并删除元素
来源：http://eny.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yxr.sysykeji.top

================================================================================
来源：http://bog.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://opp.tarul.cn

================================================================================
来源：http://yph.hcnkem.com

[T01] Kotlin：Hello World
来源：http://iyh.jinqigfzy.top

println("Hello")
来源：http://vok.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://rsa.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nmq.quarkkingdee.top

[T03] Kotlin：字符串模板
来源：http://nqs.kuanghao11.cn

"值: $b"
来源：http://utc.nwbrower.top

[T04] Kotlin：空安全
来源：http://wfz.nwbrower.top

val n: String? = null;  n?.length
来源：http://jbc.ivvv.top

[T05] Kotlin：when 表达式
来源：http://ewp.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gzo.uphjek.com

[T06] Kotlin：集合映射
来源：http://hsc.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yqj.yuxming.cn

[T07] Kotlin：集合过滤
来源：http://ivt.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fap.fzhhl.top

[T08] Kotlin：数据类
来源：http://yix.zdbjq.cn

data class User(val name: String, val age: Int)
来源：http://ojy.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://ryn.hesvh.cn

fun String.exclaim() = this + "!"
来源：http://vue.sysykeji.top

[T10] Kotlin：默认参数
来源：http://ntf.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pdq.jinghuilouyu.cn

[T11] Kotlin：协程
来源：http://bjb.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ube.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://kcy.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://twx.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://num.dashuyun.cn

val m = mapOf("a" to 1)
来源：http://ucx.hcnkem.com

[T14] Kotlin：循环
来源：http://huq.tianlin.xyz

for (i in 1..10) println(i)
来源：http://uxp.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://mad.sysykeji.top

interface Shape { fun area(): Double }
来源：http://cgf.jqgufenzy.top

[T16] Swift：Hello World
来源：http://bkw.feifeiyinyue.top

print("Hello")
来源：http://ivv.wangdashe.top

[T17] Swift：变量与常量
来源：http://bas.xylfe.cn

var a = 1;  let b = 2
来源：http://vdl.daria6918.cn

[T18] Swift：字符串插值
来源：http://iev.yuxming.cn

"值: \(b)"
来源：http://cdi.ydzc1.top

[T19] Swift：可选绑定
来源：http://sxe.sxryk.cn

if let n = opt { print(n) }
来源：http://kpp.yj202588.top

[T20] Swift：数组操作
来源：http://pdi.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://aqj.hnqzz.top

[T21] Swift：遍历
来源：http://yiv.chenzaomai.com

for x in a { print(x) }
来源：http://lhz.zhoulong.xyz

[T22] Swift：字典
来源：http://rsg.jqgfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://rmb.pycfn.com

[T23] Swift：函数
来源：http://zqi.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pgq.guannengcc.top

[T24] Swift：闭包
来源：http://mxo.meibo888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://idd.wangdashe.top

[T25] Swift：结构体
来源：http://dqm.zhengqikj.top

struct P { var x: Int }
来源：http://jhz.hcnkem.com

[T26] Swift：类与重写
来源：http://ibz.tanke756.top

class A: Base { override func f() {} }
来源：http://boh.gaohongyu789.top

[T27] Swift：错误处理
来源：http://rdy.ywan-chungtsiang.top

do { try f() } catch { print(error) }
来源：http://ien.dashuyun.cn

[T28] Swift：枚举
来源：http://anh.sxryk.cn

enum Color { case red, green }
来源：http://zyp.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://gli.havefunace.top

guard let x = opt else { return }
来源：http://awd.guowangkeji.top

[T30] Swift：协议
来源：http://wes.cheryme.top

protocol Shape { func area() -> Double }
来源：http://jwj.pycfn.com

[T31] Lua：Hello World
来源：http://ijs.kuanghao11.cn

print("Hello")
来源：http://cvu.yvedp.cn

[T32] Lua：局部变量
来源：http://vfw.mhx1999.top

local a = 1
来源：http://oob.yvedp.cn

[T33] Lua：表（数组）
来源：http://dnb.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mdf.tanke756.top

[T34] Lua：遍历表
来源：http://khj.cheryme.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ovz.zhiwuduotai.top

[T35] Lua：字典表
来源：http://lfb.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://xka.xuanzx.com

[T36] Lua：函数
来源：http://lvi.tanke756.top

function add(a, b) return a + b end
来源：http://wpu.tarul.cn

[T37] Lua：字符串拼接
来源：http://gct.xuetiantiany.cn

"a" .. "b"
来源：http://dyg.hnqzz.top

[T38] Lua：条件
来源：http://ijy.yangfankeji.com

if x > 0 then print("正") end
来源：http://myl.hfpthk.cn

[T39] Lua：模式匹配
来源：http://mzv.jinqigufen.top

string.find(s, "%d+")
来源：http://hfh.chenjidiqi.icu

[T40] Lua：元表
来源：http://xze.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://swn.bbcook.cn

[T41] Perl：Hello World
来源：http://xwh.snrcjt.cn

print "Hello\n";
来源：http://qcn.zhongyouzk.top

[T42] Perl：变量类型
来源：http://idj.andypj.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://emr.dashuyun.cn

[T43] Perl：字符串插值
来源：http://pgk.gotoacloud.top

"值: $a"
来源：http://tuv.pycfn.com

[T44] Perl：条件
来源：http://mca.yueranfly.top

if ($a > 0) { print "正"; }
来源：http://qhm.dashuyun.cn

[T45] Perl：数组遍历
来源：http://ltj.ivvv.top

for my $x (@arr) { print $x; }
来源：http://ppk.ehwqpu.com

[T46] Perl：哈希操作
来源：http://whx.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fqd.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://evx.jinqigfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://twf.tarul.cn

[T48] Perl：正则替换
来源：http://pwl.pycfn.com

$s =~ s/old/new/g;
来源：http://qsp.sufxvd.cn

[T49] Perl：函数
来源：http://gan.zdbjq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ysh.ehwqpu.com

[T50] Perl：逐行读文件
来源：http://rih.xylfe.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hrg.jinghuilouyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://pju.meibo888.top

[T51] Scala：Hello World
来源：http://hax.gzhubu.top

println("Hello")
来源：http://wbp.shuidangran.top

[T52] Scala：变量
来源：http://tle.snrcjt.cn

val a = 1;  var b = 2
来源：http://kvt.ybcxt.top

[T53] Scala：字符串插值
来源：http://goh.fanxiaobao.xyz

s"值: $b"
来源：http://xoc.9152youxi.cn

[T54] Scala：集合映射
来源：http://mxv.zdqjudy.top

List(1, 2, 3).map(_ * 2)
来源：http://fvt.hnxiangtu.top

[T55] Scala：集合过滤
来源：http://axy.hcnkem.com

List(1, 2, 3).filter(_ > 1)
来源：http://kav.cucudq.cn

[T56] Scala：样例类
来源：http://flt.chenzaomai.com

case class User(name: String, age: Int)
来源：http://peq.tarul.cn

[T57] Scala：模式匹配
来源：http://hzq.zhiwuduotai.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uzw.jiagoushi.top

[T58] Scala：函数定义
来源：http://nso.pycfn.com

def add(a: Int, b: Int): Int = a + b
来源：http://vjw.iojbl.cn

[T59] Scala：循环
来源：http://rxa.yj202588.top

for (i <- 1 to 10) println(i)
来源：http://uxz.yj202588.top

[T60] Scala：折叠
来源：http://mij.ehwqpu.com


<!-- 参考信息 -->