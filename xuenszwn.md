代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nvw.dashuyun.cn

[R56] 远程拷贝
来源：http://psc.jlsjyb.cn

scp file user@host:/path/
来源：http://ulv.zdqjudy.top

[R57] 远程执行命令
来源：http://uup.hammf.cn

ssh user@host 'uptime'
来源：http://wpq.shanyushiyangtech.top

[R58] 下载文件
来源：http://mhe.fengsongda.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kqp.tianlin.xyz

[R59] 发 POST JSON
来源：http://zcw.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fuc.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://dvh.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ejq.nwbrower.top

[R61] 磁盘占用
来源：http://ccn.gaohongyu789.top

df -h;  du -sh *
来源：http://lfv.cheryme.top

[R62] 找最占空间的文件
来源：http://crf.bjfxy.top

du -ah . | sort -rh | head -10
来源：http://oof.cqqwz.cn

[R63] 内存与进程
来源：http://mnz.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://vpr.zhoulong.xyz

[R64] 结束进程
来源：http://qub.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://ala.tian-w.cn

[R65] 查看端口占用
来源：http://pzn.shuidangran.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lvn.iojbl.cn

[R66] 定时任务
来源：http://xbl.xuetiantiany.cn

crontab -e;  crontab -l
来源：http://clg.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://uzq.ctjpmb.com

openssl rand -hex 16
来源：http://wgj.aizwys.cn

[R68] 计算文件校验值
来源：http://ith.daxiang520.top

sha256sum a.txt;  md5sum a.txt
来源：http://kms.hfpthk.cn

[R69] 生成随机密码
来源：http://obx.yj20258.top

head -c 16 /dev/urandom | base64
来源：http://hkr.cheryme.top

[R70] 时间戳与互转
来源：http://xrt.cucudq.cn

date +%s;  date -d @1700000000
来源：http://bdh.ivvv.top

[R71] 日期格式化
来源：http://laa.sysykeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zye.cashguo.top

[R72] 等待端口就绪
来源：http://gof.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yuq.ehwqpu.com

[R73] 分割大日志
来源：http://clq.xylfe.cn

split -l 1000 big.log part_
来源：http://twk.guowangkeji.top

[R74] 批量重命名
来源：http://tnj.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lti.mhx1999.top

[R75] 导出环境变量
来源：http://pey.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://kug.yj202588.top

[R76] 使用临时文件
来源：http://jpk.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yis.yj20258.top

[R77] 读取用户输入
来源：http://tzf.redwolf501.top

read -rp "请输入: " ans
来源：http://sif.shanyushiyangkeji.top

[R78] 交互式菜单
来源：http://hwj.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://cvn.havefunace.top

[R79] 解析命令行选项
来源：http://slw.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ivx.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://ybd.xuetiantiany.cn

time ./run.sh
来源：http://gvu.zdbjq.cn

================================================================================
来源：http://zef.ctjpmb.com

S. C / C++ 专题
来源：http://jiu.vehdjk.com

================================================================================
来源：http://rmd.cucudq.cn

[S01] C：Hello World
来源：http://ffe.havefunace.top

#include <stdio.h>
来源：http://oqs.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vhk.chenlongwang.top

[S02] C：变量与格式化输出
来源：http://dlj.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://dme.jqgufenzy.top

[S03] C：读入整数
来源：http://tzt.jqgfzy.top

int x; scanf("%d", &x);
来源：http://uia.tianlin.xyz

[S04] C：字符串复制
来源：http://fwl.ydzc1.top

char dst[32]; strcpy(dst, "hi");
来源：http://qkd.fengsongda.top

[S05] C：字符串长度
来源：http://dza.52xcode.cn

strlen(s)
来源：http://vcr.c1oappe.top

[S06] C：字符串比较
来源：http://lmr.redwolf501.top

strcmp(a, b) == 0
来源：http://ost.vehdjk.com

[S07] C：数组遍历求和
来源：http://wrr.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qni.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://hkv.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://auc.pengpengdd.cyou

[S09] C：结构体定义与初始化
来源：http://cjw.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wyu.daria6918.cn

[S10] C：指针与解引用
来源：http://ian.meibo888.top

int *p = &a;  *p = 5;
来源：http://ixw.yuanzhike.top

[S11] C：逐行读文件
来源：http://lhm.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://bsk.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://phc.chenjidiqi.icu

fclose(f);
来源：http://whu.aibaodan.cn

[S12] C：写文件
来源：http://lqf.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qzx.yuanzhike.top

[S13] C：宏定义
来源：http://mvh.daxiang520.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yrj.yueranfly.top

[S14] C：枚举
来源：http://gwe.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://dvi.ydzc1.top

[S15] C：类型转换
来源：http://nvq.gogol.net.cn

(double) a / b
来源：http://gft.zhongyouzk.top

[S16] C：位操作置位
来源：http://swo.hfpthk.cn

x |= (1 << 3);
来源：http://ufd.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://tpe.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cxj.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://soe.aibaodan.cn

int main(int argc, char **argv)
来源：http://jqd.hywenlv.cn

[S19] C：快速排序
来源：http://jsh.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vbm.bbcook.cn

[S20] C：二分查找
来源：http://auz.svipenyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lgk.dianchejie.cn

[S21] C：字符类别判断
来源：http://yxb.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ylx.chenzaomai.com

[S22] C：字符串转数字
来源：http://aad.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vpn.zdqjudy.top

[S23] C：随机数
来源：http://yhr.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gyl.xziqi.cn

[S24] C：获取本地时间
来源：http://cyu.yfazqb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://edo.yueranfly.top

[S25] C：内存拷贝
来源：http://pye.gotoacloud.top

memcpy(dst, src, n);
来源：http://fam.jqgfzy.top

[S26] C：内存清零
来源：http://kmi.vehdjk.com

memset(a, 0, sizeof a);
来源：http://cij.redwolf501.top

[S27] C：定义常量
来源：http://iwp.cheryme.top

const double PI = 3.14159;
来源：http://mrj.cucudq.cn

[S28] C：静态变量
来源：http://gdt.zhiwuduotai.top

static int counter = 0;
来源：http://wpi.sufxvd.cn

[S29] C：变参函数
来源：http://nqt.dashuyun.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eas.fengsongda.top

[S30] C：头文件保护
来源：http://oib.xylfe.cn

#ifndef X_H
来源：http://imx.jiagoushi.top

#define X_H
来源：http://jjg.wangshuangyany.cn

#endif
来源：http://qnw.tian-w.cn

[S31] C++：Hello World
来源：http://xeq.pengpengdd.cyou

#include <iostream>
来源：http://hhd.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://ngc.52xcode.cn

[S32] C++：字符串
来源：http://gew.52xcode.cn

std::string s = "hi";  s += "!";
来源：http://mna.jinqigufen.top

[S33] C++：vector 增删
来源：http://mdi.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fxi.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://pto.cqqwz.cn

for (auto &x : v) { std::cout << x; }
来源：http://dhm.chenzaomai.com

[S35] C++：map
来源：http://ovm.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tkt.hnxiangtu.top

[S36] C++：unordered_map
来源：http://ewf.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kvu.jinghuilouyu.cn

[S37] C++：set
来源：http://pow.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vsi.hysaishi.cn

[S38] C++：排序
来源：http://xoq.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://dfs.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://har.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gfi.ctjpmb.com

[S40] C++：查找元素
来源：http://ins.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ple.fengsongda.top

[S41] C++：类与构造函数
来源：http://gyl.cucudq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mpj.nanxuanxn.top

[S42] C++：继承与虚函数
来源：http://mvw.cdnleiting.top

class B : public Base { public: void f() override {} };
来源：http://vzx.hammf.cn

[S43] C++：智能指针
来源：http://emj.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://zww.xziqi.cn

[S44] C++：引用传参
来源：http://jhz.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://ava.shangyingyoupin.top

[S45] C++：lambda
来源：http://ely.zhongyouzk.top

auto add = [](int a, int b) { return a + b; };
来源：http://ana.yueranfly.top

[S46] C++：函数模板
来源：http://gyp.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dft.nanxuanxn.top

[S47] C++：结构化绑定遍历
来源：http://ske.yueranfly.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ewq.tianlin.xyz

[S48] C++：逐行读文件
来源：http://nvf.tarul.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yhv.hongshengwenyu.top

while (std::getline(in, line)) { }
来源：http://ekn.redwolf501.top

[S49] C++：写文件
来源：http://jjl.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ykg.gogol.net.cn

[S50] C++：格式化数字
来源：http://occ.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://euz.jiagoushi.top

[S51] C++：显式类型转换
来源：http://rrd.chenzaomai.com

static_cast<double>(a) / b
来源：http://ygt.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://iec.yvedp.cn

int size() const noexcept { return n_; }
来源：http://xch.yj20258888.top

[S53] C++：移动语义
来源：http://emj.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://zsa.zhixingplan.top

[S54] C++：异常处理
来源：http://rsi.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ovi.tianlin.xyz

[S55] C++：结构化绑定
来源：http://rjh.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rku.bjfxy.top

[S56] C++：optional
来源：http://iiy.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ajp.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://wvo.52xcode.cn

constexpr int N = 10;
来源：http://tiy.chenjidiqi.icu

[S58] C++：命名空间
来源：http://hlh.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://ivk.yonumen.top

[S59] C++：静态断言
来源：http://xrd.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fed.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://tgr.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hll.cdnleiting.top

================================================================================
来源：http://vlg.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ztk.cashguo.top

================================================================================
来源：http://dkw.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://kck.gotoacloud.top

println("Hello")
来源：http://pic.cdnleiting.top

[T02] Kotlin：变量
来源：http://qbp.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nbu.iojbl.cn

[T03] Kotlin：字符串模板
来源：http://byu.gogol.net.cn

"值: $b"
来源：http://tly.yvedp.cn

[T04] Kotlin：空安全
来源：http://nav.yonumen.top

val n: String? = null;  n?.length
来源：http://cmd.316326.xyz

[T05] Kotlin：when 表达式
来源：http://jrd.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iba.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://rmb.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://wtm.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://oak.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zxd.zhaomingkeji.xyz

[T08] Kotlin：数据类
来源：http://zpw.zhaomingkeji.xyz

data class User(val name: String, val age: Int)
来源：http://ssk.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://rlx.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://fxt.hcnkem.com

[T10] Kotlin：默认参数
来源：http://vnf.tianlin.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://whb.chenjidiqi.icu

[T11] Kotlin：协程
来源：http://qhh.fzhhl.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xvn.quarkkingdee.top

[T12] Kotlin：解构声明
来源：http://gjs.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://jsz.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://pge.cashguo.top

val m = mapOf("a" to 1)
来源：http://wue.shanyushiyangtech.top

[T14] Kotlin：循环
来源：http://iog.tanke756.top

for (i in 1..10) println(i)
来源：http://qvw.ppjwa.cn

[T15] Kotlin：接口
来源：http://lhh.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://oee.zhoulong.xyz

[T16] Swift：Hello World
来源：http://zqk.feifeiyinyue.top

print("Hello")
来源：http://fae.chenzaomai.com

[T17] Swift：变量与常量
来源：http://nbe.birdmap.top

var a = 1;  let b = 2
来源：http://mgg.iojbl.cn

[T18] Swift：字符串插值
来源：http://ndw.hysaishi.cn

"值: \(b)"
来源：http://ztb.hysaishi.cn

[T19] Swift：可选绑定
来源：http://scb.dianchejie.cn

if let n = opt { print(n) }
来源：http://gix.gaohongyu789.top

[T20] Swift：数组操作
来源：http://ban.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://vst.jlsjyb.cn

[T21] Swift：遍历
来源：http://yqn.chenzaomai.com

for x in a { print(x) }
来源：http://hnj.jlsjyb.cn

[T22] Swift：字典
来源：http://srg.jiagoushi.top

var d = ["a": 1];  d["b"] = 2
来源：http://kfs.zdqjudy.top

[T23] Swift：函数
来源：http://qap.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hik.yanxiufei.cn

[T24] Swift：闭包
来源：http://gkt.sysykeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pht.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://hrc.fzhhl.top

struct P { var x: Int }
来源：http://tjq.ydjk.org.cn

[T26] Swift：类与重写
来源：http://tgd.yonumen.top

class A: Base { override func f() {} }
来源：http://rze.ybcxt.top

[T27] Swift：错误处理
来源：http://oua.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://lbm.aibaodan.cn

[T28] Swift：枚举
来源：http://alh.hnqzz.top

enum Color { case red, green }
来源：http://nwm.hongshengwenyu.top

[T29] Swift：guard 提前返回
来源：http://aix.xuetiantiany.cn

guard let x = opt else { return }
来源：http://qxt.hnxiangtu.top

[T30] Swift：协议
来源：http://ect.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://icq.smart0.xyz

[T31] Lua：Hello World
来源：http://iji.vqdsnc.cn

print("Hello")
来源：http://bbr.bbcook.cn

[T32] Lua：局部变量
来源：http://rxj.yj202588.top

local a = 1
来源：http://ngg.hesvh.cn

[T33] Lua：表（数组）
来源：http://gis.fanxiaobao.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://cer.xziqi.cn

[T34] Lua：遍历表
来源：http://iul.gzhubu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kps.chenzaomai.com

[T35] Lua：字典表
来源：http://wjh.hnxiangtu.top

local d = { a = 1 };  d.b = 2
来源：http://wyb.jqgufenzy.top

[T36] Lua：函数
来源：http://gid.xingfuxueyuan.xyz

function add(a, b) return a + b end
来源：http://vzz.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://kbg.hesvh.cn

"a" .. "b"
来源：http://ezm.andypj.xyz

[T38] Lua：条件
来源：http://mkd.ybcxt.top

if x > 0 then print("正") end
来源：http://zvt.zdqjudy.top

[T39] Lua：模式匹配
来源：http://jpm.havefunace.top

string.find(s, "%d+")
来源：http://fwd.zdqjudy.top

[T40] Lua：元表
来源：http://ibg.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://avl.dashuyun.cn

[T41] Perl：Hello World
来源：http://hsw.cqqwz.cn

print "Hello\n";
来源：http://lkw.hysaishi.cn

[T42] Perl：变量类型
来源：http://ffa.yongpay.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ksg.c1oappe.top

[T43] Perl：字符串插值
来源：http://uid.gzhubu.top

"值: $a"
来源：http://xlm.ywan-chungtsiang.top

[T44] Perl：条件
来源：http://ewx.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://abc.yanxiufei.cn

[T45] Perl：数组遍历
来源：http://krp.cheryme.top

for my $x (@arr) { print $x; }
来源：http://qye.316326.xyz

[T46] Perl：哈希操作
来源：http://red.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iyz.zycfv.cn

[T47] Perl：正则捕获
来源：http://jsz.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sce.aizwys.cn

[T48] Perl：正则替换
来源：http://ewh.0kj1m.cn

$s =~ s/old/new/g;
来源：http://wds.sweek.top

[T49] Perl：函数
来源：http://qtr.wangshuangyany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kkb.fengsongda.top

[T50] Perl：逐行读文件
来源：http://dzb.daria6918.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://euk.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://ofh.yuxming.cn

[T51] Scala：Hello World
来源：http://ekn.52xcode.cn

println("Hello")
来源：http://zdg.sufxvd.cn

[T52] Scala：变量
来源：http://fie.mhx1999.top

val a = 1;  var b = 2
来源：http://osy.yj20258888.top

[T53] Scala：字符串插值
来源：http://knr.sxryk.cn

s"值: $b"
来源：http://tmy.ivvv.top

[T54] Scala：集合映射
来源：http://wkv.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://boc.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://tuu.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://dbh.hesvh.cn

[T56] Scala：样例类
来源：http://zuc.nanxuanxn.top

case class User(name: String, age: Int)
来源：http://oks.daxiang520.top

[T57] Scala：模式匹配
来源：http://omr.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qmf.wangdashe.top

[T58] Scala：函数定义
来源：http://qmf.yvedp.cn


<!-- 参考信息 -->