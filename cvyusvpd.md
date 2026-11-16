代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gme.xylfe.cn

[R54] 比较两个文件
来源：http://xtx.ydzc1.top

diff a.txt b.txt
来源：http://jma.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://okt.zhaomingkeji.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://afn.vqdsnc.cn

[R56] 远程拷贝
来源：http://mnp.bbcook.cn

scp file user@host:/path/
来源：http://vok.smart0.xyz

[R57] 远程执行命令
来源：http://lzj.zhaomingkeji.xyz

ssh user@host 'uptime'
来源：http://ria.vqdsnc.cn

[R58] 下载文件
来源：http://zdl.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vlo.ehwqpu.com

[R59] 发 POST JSON
来源：http://bms.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cfy.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://uti.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://znz.chenjidiqi.icu

[R61] 磁盘占用
来源：http://vek.guowangkeji.top

df -h;  du -sh *
来源：http://ppo.cqqwz.cn

[R62] 找最占空间的文件
来源：http://jqb.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://nzt.haohaochexian.top

[R63] 内存与进程
来源：http://aej.daria6918.cn

free -h;  ps aux | grep nginx
来源：http://smw.tanke756.top

[R64] 结束进程
来源：http://lpi.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://hyf.jianghu66.top

[R65] 查看端口占用
来源：http://ecb.shangyingyoupin.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bun.redwolf501.top

[R66] 定时任务
来源：http://tim.kuanghao11.cn

crontab -e;  crontab -l
来源：http://qty.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://iqk.xuetiantiany.cn

openssl rand -hex 16
来源：http://vuc.sjlbkw.cn

[R68] 计算文件校验值
来源：http://hjk.hesvh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hjz.snrcjt.cn

[R69] 生成随机密码
来源：http://nlf.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://xpp.xinyue.icu

[R70] 时间戳与互转
来源：http://xpy.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://haa.ydzc1.top

[R71] 日期格式化
来源：http://rke.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gcp.shanyushiyangkeji.top

[R72] 等待端口就绪
来源：http://owp.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jsm.yongpay.top

[R73] 分割大日志
来源：http://aol.guannengcc.top

split -l 1000 big.log part_
来源：http://npb.yangfankeji.com

[R74] 批量重命名
来源：http://ryn.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ebt.ybcxt.top

[R75] 导出环境变量
来源：http://owu.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://vyu.ydzc1.top

[R76] 使用临时文件
来源：http://prr.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eqz.ydjk.org.cn

[R77] 读取用户输入
来源：http://xck.cqqwz.cn

read -rp "请输入: " ans
来源：http://nit.ppjwa.cn

[R78] 交互式菜单
来源：http://ioi.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sqf.jlsjyb.cn

[R79] 解析命令行选项
来源：http://qva.snrcjt.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xol.shanyushiyangkeji.top

[R80] 查看脚本执行耗时
来源：http://owr.nanxinkj.top

time ./run.sh
来源：http://han.xylfe.cn

================================================================================
来源：http://djg.yfazqb.com

S. C / C++ 专题
来源：http://qpt.316326.xyz

================================================================================
来源：http://kpw.9152youxi.cn

[S01] C：Hello World
来源：http://eys.sufxvd.cn

#include <stdio.h>
来源：http://rgg.hesvh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bxc.ybcxt.top

[S02] C：变量与格式化输出
来源：http://pqv.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://wit.nwbrower.top

[S03] C：读入整数
来源：http://jww.yangfankeji.com

int x; scanf("%d", &x);
来源：http://udf.zdqjudy.top

[S04] C：字符串复制
来源：http://ntt.sufxvd.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ntn.kuanghao11.cn

[S05] C：字符串长度
来源：http://dcy.birdmap.top

strlen(s)
来源：http://esd.c1oappe.top

[S06] C：字符串比较
来源：http://lvv.ybcxt.top

strcmp(a, b) == 0
来源：http://ddk.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://rmx.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mkg.havefunace.top

[S08] C：动态内存分配与释放
来源：http://owo.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://igq.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://wak.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cxy.sweek.top

[S10] C：指针与解引用
来源：http://osi.jinqigufen.top

int *p = &a;  *p = 5;
来源：http://kqn.yangfankeji.com

[S11] C：逐行读文件
来源：http://mol.yfazqb.com

FILE *f = fopen("a.txt", "r");
来源：http://hpi.gzhubu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cmb.yueranfly.top

fclose(f);
来源：http://jsq.andypj.xyz

[S12] C：写文件
来源：http://nlr.hfpthk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ugw.vqdsnc.cn

[S13] C：宏定义
来源：http://ebo.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tvt.yvedp.cn

[S14] C：枚举
来源：http://mzn.aizwys.cn

enum Color { RED, GREEN, BLUE };
来源：http://sbv.epnwcf.com

[S15] C：类型转换
来源：http://lpe.shangyingyoupin.top

(double) a / b
来源：http://lgk.yuanzhike.top

[S16] C：位操作置位
来源：http://kpl.shzxlz.cn

x |= (1 << 3);
来源：http://bxu.ydzc1.top

[S17] C：安全拼接字符串
来源：http://gja.fanxiaobao.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uds.xingfuxueyuan.xyz

[S18] C：命令行参数
来源：http://wze.yonumen.top

int main(int argc, char **argv)
来源：http://pdg.guannengcc.top

[S19] C：快速排序
来源：http://gzr.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nwy.sysykeji.top

[S20] C：二分查找
来源：http://qkl.gaohongyu789.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bsj.jianghu66.top

[S21] C：字符类别判断
来源：http://hzg.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://imm.cheryme.top

[S22] C：字符串转数字
来源：http://evo.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://qcw.gzhubu.top

[S23] C：随机数
来源：http://lro.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://rtg.dianchejie.cn

[S24] C：获取本地时间
来源：http://omi.tianlin.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tfo.jyoumei.cn

[S25] C：内存拷贝
来源：http://ggo.sufxvd.cn

memcpy(dst, src, n);
来源：http://crs.fehbvm.com

[S26] C：内存清零
来源：http://scx.nanxuanxn.top

memset(a, 0, sizeof a);
来源：http://jod.andypj.xyz

[S27] C：定义常量
来源：http://vsd.feifeiyinyue.top

const double PI = 3.14159;
来源：http://tba.gogol.net.cn

[S28] C：静态变量
来源：http://ohf.yfazqb.com

static int counter = 0;
来源：http://adg.fanxiaobao.xyz

[S29] C：变参函数
来源：http://gcy.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gpt.uphjek.com

[S30] C：头文件保护
来源：http://btq.ydjk.org.cn

#ifndef X_H
来源：http://bzz.zdbjq.cn

#define X_H
来源：http://hhq.yvedp.cn

#endif
来源：http://dqr.tianlin.xyz

[S31] C++：Hello World
来源：http://rfu.chenzaomai.com

#include <iostream>
来源：http://izc.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://dee.chenjidiqi.icu

[S32] C++：字符串
来源：http://jww.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://jar.tanke756.top

[S33] C++：vector 增删
来源：http://rbc.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://njp.zhijiandao.cn

[S34] C++：遍历 vector
来源：http://qhs.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://tmy.cucudq.cn

[S35] C++：map
来源：http://caj.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bjy.vqdsnc.cn

[S36] C++：unordered_map
来源：http://dql.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://inn.zycfv.cn

[S37] C++：set
来源：http://rig.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bsw.aibaodan.cn

[S38] C++：排序
来源：http://nli.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://chz.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://zdv.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://git.snrcjt.cn

[S40] C++：查找元素
来源：http://whg.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rmg.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://ubi.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://khz.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://gwu.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://qoe.jqgfzy.top

[S43] C++：智能指针
来源：http://whl.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://tqe.yueranfly.top

[S44] C++：引用传参
来源：http://kmx.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://hnn.gzhubu.top

[S45] C++：lambda
来源：http://ouj.c1oappe.top

auto add = [](int a, int b) { return a + b; };
来源：http://hbo.zhixingplan.top

[S46] C++：函数模板
来源：http://wqr.ydjk.org.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mdr.yvedp.cn

[S47] C++：结构化绑定遍历
来源：http://jaj.gaohongyu789.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://soi.tarul.cn

[S48] C++：逐行读文件
来源：http://pbl.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://wkc.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://mee.jiagoushi.top

[S49] C++：写文件
来源：http://bdp.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://spv.tianlin.xyz

[S50] C++：格式化数字
来源：http://tng.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tfs.jinqigfzy.top

[S51] C++：显式类型转换
来源：http://qhd.jiagoushi.top

static_cast<double>(a) / b
来源：http://quc.guowangkeji.top

[S52] C++：const 与 noexcept
来源：http://oqa.pycfn.com

int size() const noexcept { return n_; }
来源：http://pul.yj202588.top

[S53] C++：移动语义
来源：http://vyp.cheryme.top

std::vector<int> w = std::move(v);
来源：http://yfd.tianlin.xyz

[S54] C++：异常处理
来源：http://vau.jqgfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ksr.ctjpmb.com

[S55] C++：结构化绑定
来源：http://efd.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wxy.ybcxt.top

[S56] C++：optional
来源：http://qis.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jie.ydjk.org.cn

[S57] C++：编译期常量
来源：http://okv.guowangkeji.top

constexpr int N = 10;
来源：http://grv.hfpthk.cn

[S58] C++：命名空间
来源：http://zoz.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://dxu.guannengcc.top

[S59] C++：静态断言
来源：http://nbo.haohaochexian.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fbh.meibo888.top

[S60] C++：遍历并删除元素
来源：http://yqa.c1oappe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tpv.yvedp.cn

================================================================================
来源：http://fep.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wyu.smart0.xyz

================================================================================
来源：http://fex.cucudq.cn

[T01] Kotlin：Hello World
来源：http://izl.yueranfly.top

println("Hello")
来源：http://byt.yvedp.cn

[T02] Kotlin：变量
来源：http://qfj.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qcw.zhixingplan.top

[T03] Kotlin：字符串模板
来源：http://yvu.fktsv.cn

"值: $b"
来源：http://vyf.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://uoi.gzhubu.top

val n: String? = null;  n?.length
来源：http://dkn.zhaomingkeji.xyz

[T05] Kotlin：when 表达式
来源：http://wif.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zgv.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://onj.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://den.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://ulm.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://otx.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://sxz.gaohongyu789.top

data class User(val name: String, val age: Int)
来源：http://qaq.zhiwuduotai.top

[T09] Kotlin：扩展函数
来源：http://yta.yj20258888.top

fun String.exclaim() = this + "!"
来源：http://fbr.zhengqikj.top

[T10] Kotlin：默认参数
来源：http://wmg.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pjl.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://xpe.zhijiandao.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nvi.hammf.cn

[T12] Kotlin：解构声明
来源：http://jju.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://rlb.cashguo.top

[T13] Kotlin：只读 Map
来源：http://qva.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://orq.redwolf501.top

[T14] Kotlin：循环
来源：http://yec.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://tet.sysykeji.top

[T15] Kotlin：接口
来源：http://fcc.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://ylk.nanxuanxn.top

[T16] Swift：Hello World
来源：http://pne.xuetiantiany.cn

print("Hello")
来源：http://nmw.zdqjudy.top

[T17] Swift：变量与常量
来源：http://zqk.yfazqb.com

var a = 1;  let b = 2
来源：http://ffy.fktsv.cn

[T18] Swift：字符串插值
来源：http://emo.hcnkem.com

"值: \(b)"
来源：http://pow.jqgfzy.top

[T19] Swift：可选绑定
来源：http://oes.yanxiufei.cn

if let n = opt { print(n) }
来源：http://jpi.yuanzhike.top

[T20] Swift：数组操作
来源：http://ide.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hhs.gzhubu.top

[T21] Swift：遍历
来源：http://bsg.fehbvm.com

for x in a { print(x) }
来源：http://lfb.ppjwa.cn

[T22] Swift：字典
来源：http://bof.havefunace.top

var d = ["a": 1];  d["b"] = 2
来源：http://bjk.nanxinkj.top

[T23] Swift：函数
来源：http://rpv.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fid.fktsv.cn

[T24] Swift：闭包
来源：http://cyv.sjlbkw.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hea.hesvh.cn

[T25] Swift：结构体
来源：http://cry.epnwcf.com

struct P { var x: Int }
来源：http://aki.c1oappe.top

[T26] Swift：类与重写
来源：http://deu.yj20258.top

class A: Base { override func f() {} }
来源：http://dmd.fktsv.cn

[T27] Swift：错误处理
来源：http://vfh.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://udh.fanxiaobao.xyz

[T28] Swift：枚举
来源：http://ogl.ctjpmb.com

enum Color { case red, green }
来源：http://zbd.tianlin.xyz

[T29] Swift：guard 提前返回
来源：http://cai.sufxvd.cn

guard let x = opt else { return }
来源：http://bew.mhx1999.top

[T30] Swift：协议
来源：http://yds.316326.xyz

protocol Shape { func area() -> Double }
来源：http://dye.yuxming.cn

[T31] Lua：Hello World
来源：http://wvz.hongshengwenyu.top

print("Hello")
来源：http://vmz.aibaodan.cn

[T32] Lua：局部变量
来源：http://wef.xuanzx.com

local a = 1
来源：http://vqf.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://bfg.nanxinkj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hxd.meibo888.top

[T34] Lua：遍历表
来源：http://bko.smart0.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://cej.wangdashe.top

[T35] Lua：字典表
来源：http://ksm.daria6918.cn

local d = { a = 1 };  d.b = 2
来源：http://srk.fktsv.cn

[T36] Lua：函数
来源：http://rta.ydzc1.top

function add(a, b) return a + b end
来源：http://onw.jinghuilouyu.cn

[T37] Lua：字符串拼接
来源：http://qkq.yueranfly.top

"a" .. "b"
来源：http://ikm.quarkkingdee.top

[T38] Lua：条件
来源：http://ctu.zycfv.cn

if x > 0 then print("正") end
来源：http://xyl.cheryme.top

[T39] Lua：模式匹配
来源：http://sia.jianghu66.top

string.find(s, "%d+")
来源：http://qbw.ydzc1.top

[T40] Lua：元表
来源：http://bdj.svipenyu.cn

setmetatable({}, { __index = base })
来源：http://eca.yj20258.top

[T41] Perl：Hello World
来源：http://iuq.cqqwz.cn

print "Hello\n";
来源：http://rdy.hysaishi.cn

[T42] Perl：变量类型
来源：http://zbz.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tpl.xingfuxueyuan.xyz

[T43] Perl：字符串插值
来源：http://mfy.nwbrower.top

"值: $a"
来源：http://ifo.nanxinkj.top

[T44] Perl：条件
来源：http://phd.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://emy.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://twl.cqqwz.cn

for my $x (@arr) { print $x; }
来源：http://wkl.zhixingplan.top

[T46] Perl：哈希操作
来源：http://grd.sysykeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vvj.smart0.xyz

[T47] Perl：正则捕获
来源：http://tfk.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://ddp.aibaodan.cn

[T48] Perl：正则替换
来源：http://dwy.tanke756.top

$s =~ s/old/new/g;
来源：http://nmz.aibaodan.cn

[T49] Perl：函数
来源：http://gcb.zdbjq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vrm.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://xzh.chenlongwang.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pny.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://kmw.aibaodan.cn

[T51] Scala：Hello World
来源：http://jas.hesvh.cn

println("Hello")
来源：http://anh.zhiwuduotai.top

[T52] Scala：变量
来源：http://bmn.316326.xyz

val a = 1;  var b = 2
来源：http://eri.ivvv.top

[T53] Scala：字符串插值
来源：http://rxw.meibo888.top

s"值: $b"
来源：http://apa.dashuyun.cn

[T54] Scala：集合映射
来源：http://spa.hfpthk.cn

List(1, 2, 3).map(_ * 2)
来源：http://ght.yj20258.top

[T55] Scala：集合过滤
来源：http://sew.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://wza.daria6918.cn

[T56] Scala：样例类
来源：http://vny.yvedp.cn


<!-- 参考信息 -->