代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://csk.tian-w.cn

[R52] 统计行数
来源：http://wts.cqqwz.cn

wc -l a.txt
来源：http://jov.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://jvh.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eva.chenzaomai.com

[R54] 比较两个文件
来源：http://szj.shzxlz.cn

diff a.txt b.txt
来源：http://qvk.ctjpmb.com

[R55] 压缩与解压
来源：http://egf.chenlongwang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ash.ppjwa.cn

[R56] 远程拷贝
来源：http://fpj.dianchejie.cn

scp file user@host:/path/
来源：http://hpc.shangyingyoupin.top

[R57] 远程执行命令
来源：http://rcg.guannengcc.top

ssh user@host 'uptime'
来源：http://jkp.zhoulong.xyz

[R58] 下载文件
来源：http://jzj.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nyo.jinghuilouyu.cn

[R59] 发 POST JSON
来源：http://rwt.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rfw.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://xmo.iojbl.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dqp.quarkkingdee.top

[R61] 磁盘占用
来源：http://yjy.shanyushiyangtech.top

df -h;  du -sh *
来源：http://kds.hammf.cn

[R62] 找最占空间的文件
来源：http://pvt.xuanzx.com

du -ah . | sort -rh | head -10
来源：http://amn.gzhubu.top

[R63] 内存与进程
来源：http://dki.shzxlz.cn

free -h;  ps aux | grep nginx
来源：http://zyw.dashuyun.cn

[R64] 结束进程
来源：http://cdk.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://yrb.hammf.cn

[R65] 查看端口占用
来源：http://ryy.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rrh.cdnleiting.top

[R66] 定时任务
来源：http://wjp.xuanzx.com

crontab -e;  crontab -l
来源：http://pud.chenlongwang.top

[R67] 生成随机十六进制串
来源：http://rto.zhiwuduotai.top

openssl rand -hex 16
来源：http://lax.xinyue.icu

[R68] 计算文件校验值
来源：http://rse.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cfc.xinyue.icu

[R69] 生成随机密码
来源：http://zox.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://fuq.yonumen.top

[R70] 时间戳与互转
来源：http://sbw.aibaodan.cn

date +%s;  date -d @1700000000
来源：http://tjz.yj202588.top

[R71] 日期格式化
来源：http://aod.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://hjk.yuxming.cn

[R72] 等待端口就绪
来源：http://wjx.shangyingyoupin.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rrf.ydjk.org.cn

[R73] 分割大日志
来源：http://ytq.chenjidiqi.icu

split -l 1000 big.log part_
来源：http://tko.cheryme.top

[R74] 批量重命名
来源：http://pnm.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ovm.cheryme.top

[R75] 导出环境变量
来源：http://wja.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://exb.wangshuangyany.cn

[R76] 使用临时文件
来源：http://mky.fktsv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bqc.nwbrower.top

[R77] 读取用户输入
来源：http://fcf.yangfankeji.com

read -rp "请输入: " ans
来源：http://zrz.bbcook.cn

[R78] 交互式菜单
来源：http://ulw.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uxj.nanxuanxn.top

[R79] 解析命令行选项
来源：http://hcn.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://htw.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://spd.fengsongda.top

time ./run.sh
来源：http://sap.smart0.xyz

================================================================================
来源：http://jbr.yvedp.cn

S. C / C++ 专题
来源：http://ydq.pengpengdd.cyou

================================================================================
来源：http://how.0kj1m.cn

[S01] C：Hello World
来源：http://xec.hesvh.cn

#include <stdio.h>
来源：http://nbg.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uoy.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://whg.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://raj.shuidangran.top

[S03] C：读入整数
来源：http://hky.yongpay.top

int x; scanf("%d", &x);
来源：http://jad.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://nad.daria6918.cn

char dst[32]; strcpy(dst, "hi");
来源：http://llc.shzxlz.cn

[S05] C：字符串长度
来源：http://dnp.feifeiyinyue.top

strlen(s)
来源：http://hei.dianchejie.cn

[S06] C：字符串比较
来源：http://afj.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://zzn.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://tss.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hpu.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://xqt.mhx1999.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dry.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://hup.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ufn.bjfxy.top

[S10] C：指针与解引用
来源：http://roy.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://fsk.uphjek.com

[S11] C：逐行读文件
来源：http://dwd.sxryk.cn

FILE *f = fopen("a.txt", "r");
来源：http://kmz.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://otd.havefunace.top

fclose(f);
来源：http://vej.cucudq.cn

[S12] C：写文件
来源：http://lpi.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://orx.yonumen.top

[S13] C：宏定义
来源：http://cyd.haohaochexian.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://klz.fengsongda.top

[S14] C：枚举
来源：http://upb.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://zqh.jianghu66.top

[S15] C：类型转换
来源：http://kjr.jqgufenzy.top

(double) a / b
来源：http://ekt.pengpengdd.cyou

[S16] C：位操作置位
来源：http://wjn.zdbjq.cn

x |= (1 << 3);
来源：http://jvl.cashguo.top

[S17] C：安全拼接字符串
来源：http://imq.dashuyun.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aen.wangshuangyany.cn

[S18] C：命令行参数
来源：http://geh.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://sfv.yvedp.cn

[S19] C：快速排序
来源：http://wzo.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uqc.xuetiantiany.cn

[S20] C：二分查找
来源：http://zqd.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nnt.cashguo.top

[S21] C：字符类别判断
来源：http://uso.guannengcc.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hnt.cucudq.cn

[S22] C：字符串转数字
来源：http://uzt.smart0.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://oie.cqqwz.cn

[S23] C：随机数
来源：http://eru.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://svs.nanxinkj.top

[S24] C：获取本地时间
来源：http://jfs.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sfh.cucudq.cn

[S25] C：内存拷贝
来源：http://seh.hfpthk.cn

memcpy(dst, src, n);
来源：http://kpc.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://btx.haohaochexian.top

memset(a, 0, sizeof a);
来源：http://pen.redwolf501.top

[S27] C：定义常量
来源：http://qjp.hammf.cn

const double PI = 3.14159;
来源：http://tto.yj202588.top

[S28] C：静态变量
来源：http://drz.jinqigfzy.top

static int counter = 0;
来源：http://vgf.daria6918.cn

[S29] C：变参函数
来源：http://ejq.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qea.cqqwz.cn

[S30] C：头文件保护
来源：http://kfe.jlsjyb.cn

#ifndef X_H
来源：http://vnz.yj202588.top

#define X_H
来源：http://scn.ehwqpu.com

#endif
来源：http://qch.fzhhl.top

[S31] C++：Hello World
来源：http://egw.andypj.xyz

#include <iostream>
来源：http://cvd.fktsv.cn

int main() { std::cout << "Hello\n"; }
来源：http://zvr.sweek.top

[S32] C++：字符串
来源：http://rvi.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://rdi.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://rnp.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ksn.316326.xyz

[S34] C++：遍历 vector
来源：http://cuf.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://rkc.shuidangran.top

[S35] C++：map
来源：http://hkj.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zky.sysykeji.top

[S36] C++：unordered_map
来源：http://fka.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bci.zycfv.cn

[S37] C++：set
来源：http://ejc.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dni.yj202588.top

[S38] C++：排序
来源：http://vbm.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://odu.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://jvy.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gxp.kuanghao11.cn

[S40] C++：查找元素
来源：http://uui.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wvj.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://mew.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dzl.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://vsf.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://zsp.jinqigfzy.top

[S43] C++：智能指针
来源：http://kqc.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://ugq.shzxlz.cn

[S44] C++：引用传参
来源：http://wpg.birdmap.top

void inc(int &x) { ++x; }
来源：http://sob.bbcook.cn

[S45] C++：lambda
来源：http://ulq.ctjpmb.com

auto add = [](int a, int b) { return a + b; };
来源：http://znv.daria6918.cn

[S46] C++：函数模板
来源：http://uhz.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xzn.316326.xyz

[S47] C++：结构化绑定遍历
来源：http://fwi.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://imu.yangfankeji.com

[S48] C++：逐行读文件
来源：http://fvc.zhiwuduotai.top

std::ifstream in("a.txt");  std::string line;
来源：http://nxs.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://kwu.yvedp.cn

[S49] C++：写文件
来源：http://txs.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jvz.wangdashe.top

[S50] C++：格式化数字
来源：http://dgr.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hnz.shuidangran.top

[S51] C++：显式类型转换
来源：http://qht.guowangkeji.top

static_cast<double>(a) / b
来源：http://ame.cheryme.top

[S52] C++：const 与 noexcept
来源：http://lsd.yvedp.cn

int size() const noexcept { return n_; }
来源：http://enj.yvedp.cn

[S53] C++：移动语义
来源：http://ytl.cashguo.top

std::vector<int> w = std::move(v);
来源：http://epc.jianghu66.top

[S54] C++：异常处理
来源：http://hco.shangyingyoupin.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wgx.ctjpmb.com

[S55] C++：结构化绑定
来源：http://sip.xziqi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jrc.jlsjyb.cn

[S56] C++：optional
来源：http://ugm.gogol.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oga.zdqjudy.top

[S57] C++：编译期常量
来源：http://atn.yuanzhike.top

constexpr int N = 10;
来源：http://rsw.wangdashe.top

[S58] C++：命名空间
来源：http://oov.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://zij.aibaodan.cn

[S59] C++：静态断言
来源：http://hjd.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sik.jyoumei.cn

[S60] C++：遍历并删除元素
来源：http://tpw.gogol.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bto.cashguo.top

================================================================================
来源：http://ddx.yvedp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jpg.havefunace.top

================================================================================
来源：http://amk.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://fub.aibaodan.cn

println("Hello")
来源：http://xop.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://bcd.yanxiufei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fii.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://uyk.fehbvm.com

"值: $b"
来源：http://onz.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://hfp.bbcook.cn

val n: String? = null;  n?.length
来源：http://kze.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://gov.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yar.jianghu66.top

[T06] Kotlin：集合映射
来源：http://qnx.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xcs.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://vlp.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://aor.yueranfly.top

[T08] Kotlin：数据类
来源：http://gcr.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://mqp.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://byy.ybcxt.top

fun String.exclaim() = this + "!"
来源：http://men.havefunace.top

[T10] Kotlin：默认参数
来源：http://ipq.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xkz.fzhhl.top

[T11] Kotlin：协程
来源：http://ikr.shuidangran.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fwi.fengsongda.top

[T12] Kotlin：解构声明
来源：http://wgm.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://vka.hysaishi.cn

[T13] Kotlin：只读 Map
来源：http://qda.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://mkm.gaohongyu789.top

[T14] Kotlin：循环
来源：http://vth.havefunace.top

for (i in 1..10) println(i)
来源：http://ckg.pengpengdd.cyou

[T15] Kotlin：接口
来源：http://wjq.yuxming.cn

interface Shape { fun area(): Double }
来源：http://ffo.ppjwa.cn

[T16] Swift：Hello World
来源：http://quc.sxryk.cn

print("Hello")
来源：http://ayo.guowangkeji.top

[T17] Swift：变量与常量
来源：http://phu.feifeiyinyue.top

var a = 1;  let b = 2
来源：http://yuu.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://hnb.iojbl.cn

"值: \(b)"
来源：http://pcc.jqgfzy.top

[T19] Swift：可选绑定
来源：http://irv.zhijiandao.cn

if let n = opt { print(n) }
来源：http://rtg.chenjidiqi.icu

[T20] Swift：数组操作
来源：http://gfa.xuanzx.com

var a = [1, 2, 3];  a.append(4)
来源：http://dsd.uphjek.com

[T21] Swift：遍历
来源：http://uop.hfpthk.cn

for x in a { print(x) }
来源：http://zki.ydjk.org.cn

[T22] Swift：字典
来源：http://kuj.ydjk.org.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ylc.jinqigufen.top

[T23] Swift：函数
来源：http://dqq.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xtd.hesvh.cn

[T24] Swift：闭包
来源：http://rhk.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rnx.fktsv.cn

[T25] Swift：结构体
来源：http://fgy.xuetiantiany.cn

struct P { var x: Int }
来源：http://mhy.svipenyu.cn

[T26] Swift：类与重写
来源：http://owa.quarkkingdee.top

class A: Base { override func f() {} }
来源：http://ojm.cucudq.cn

[T27] Swift：错误处理
来源：http://imy.ppjwa.cn

do { try f() } catch { print(error) }
来源：http://ugo.yonumen.top

[T28] Swift：枚举
来源：http://ltq.xuanzx.com

enum Color { case red, green }
来源：http://ghs.jlsjyb.cn

[T29] Swift：guard 提前返回
来源：http://yub.chenzaomai.com

guard let x = opt else { return }
来源：http://mgn.aizwys.cn

[T30] Swift：协议
来源：http://jox.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://yyz.zdqjudy.top

[T31] Lua：Hello World
来源：http://tyw.guowangkeji.top

print("Hello")
来源：http://fux.vqdsnc.cn

[T32] Lua：局部变量
来源：http://kel.jinqigfzy.top

local a = 1
来源：http://dsh.iojbl.cn

[T33] Lua：表（数组）
来源：http://mbo.zycfv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uaw.fengsongda.top

[T34] Lua：遍历表
来源：http://ilv.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://llu.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://poy.bjfxy.top

local d = { a = 1 };  d.b = 2
来源：http://lez.yuxming.cn

[T36] Lua：函数
来源：http://nlz.hesvh.cn

function add(a, b) return a + b end
来源：http://gur.redwolf501.top

[T37] Lua：字符串拼接
来源：http://ovp.fengsongda.top

"a" .. "b"
来源：http://lag.yfazqb.com

[T38] Lua：条件
来源：http://qas.jianghu66.top

if x > 0 then print("正") end
来源：http://mfl.nwbrower.top

[T39] Lua：模式匹配
来源：http://akw.tian-w.cn

string.find(s, "%d+")
来源：http://xqc.andypj.xyz

[T40] Lua：元表
来源：http://wvc.meibo888.top

setmetatable({}, { __index = base })
来源：http://ela.zhaomingkeji.xyz

[T41] Perl：Hello World
来源：http://cbb.jinqigfzy.top

print "Hello\n";
来源：http://ina.uphjek.com

[T42] Perl：变量类型
来源：http://xrh.aibaodan.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uqh.c1oappe.top

[T43] Perl：字符串插值
来源：http://tzl.jqgufenzy.top

"值: $a"
来源：http://xwl.hfpthk.cn

[T44] Perl：条件
来源：http://jtd.316326.xyz

if ($a > 0) { print "正"; }
来源：http://uvd.xingfuxueyuan.xyz

[T45] Perl：数组遍历
来源：http://mzj.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://bkw.cqqwz.cn

[T46] Perl：哈希操作
来源：http://bzo.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zar.316326.xyz

[T47] Perl：正则捕获
来源：http://szp.vehdjk.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://kne.meibo888.top

[T48] Perl：正则替换
来源：http://cse.shuidangran.top

$s =~ s/old/new/g;
来源：http://lqt.bjfxy.top

[T49] Perl：函数
来源：http://vlb.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://peh.zycfv.cn

[T50] Perl：逐行读文件
来源：http://fhu.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lfr.cdnleiting.top

while (my $line = <$fh>) { print $line; }
来源：http://rlo.tian-w.cn

[T51] Scala：Hello World
来源：http://vrp.hywenlv.cn

println("Hello")
来源：http://hqh.wangdashe.top

[T52] Scala：变量
来源：http://twc.yvedp.cn

val a = 1;  var b = 2
来源：http://wob.hnqzz.top

[T53] Scala：字符串插值
来源：http://eau.ctjpmb.com

s"值: $b"
来源：http://qwa.shzxlz.cn

[T54] Scala：集合映射
来源：http://rpw.9152youxi.cn


<!-- 参考信息 -->