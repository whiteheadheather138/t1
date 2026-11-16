代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dqq.fanxiaobao.xyz

[R50] awk 求和
来源：http://wqw.epnwcf.com

awk '{s += $2} END {print s}' a.txt
来源：http://kog.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://scb.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rmv.yanxiufei.cn

[R52] 统计行数
来源：http://hwq.meibo888.top

wc -l a.txt
来源：http://nmy.guowangkeji.top

[R53] 查看文件头与实时尾
来源：http://lvj.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dld.haohaochexian.top

[R54] 比较两个文件
来源：http://ldf.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://eff.tanke756.top

[R55] 压缩与解压
来源：http://lpr.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hzc.dianchejie.cn

[R56] 远程拷贝
来源：http://ocu.yj20258888.top

scp file user@host:/path/
来源：http://ekn.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://ecx.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://ebg.feifeiyinyue.top

[R58] 下载文件
来源：http://wbc.vqdsnc.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kok.nanxuanxn.top

[R59] 发 POST JSON
来源：http://baj.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://trm.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://alz.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kaj.nwbrower.top

[R61] 磁盘占用
来源：http://zmy.jlsjyb.cn

df -h;  du -sh *
来源：http://wun.sxryk.cn

[R62] 找最占空间的文件
来源：http://rca.uphjek.com

du -ah . | sort -rh | head -10
来源：http://nui.yj202588.top

[R63] 内存与进程
来源：http://qpi.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://mnf.hysaishi.cn

[R64] 结束进程
来源：http://cvy.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://equ.smart0.xyz

[R65] 查看端口占用
来源：http://rpt.hysaishi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rqu.yvedp.cn

[R66] 定时任务
来源：http://jtk.xziqi.cn

crontab -e;  crontab -l
来源：http://ckf.xylfe.cn

[R67] 生成随机十六进制串
来源：http://qjd.xuetiantiany.cn

openssl rand -hex 16
来源：http://vwn.vehdjk.com

[R68] 计算文件校验值
来源：http://bxr.shanyushiyangtech.top

sha256sum a.txt;  md5sum a.txt
来源：http://pws.zycfv.cn

[R69] 生成随机密码
来源：http://tys.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://cnv.fengsongda.top

[R70] 时间戳与互转
来源：http://gqa.ybcxt.top

date +%s;  date -d @1700000000
来源：http://bgg.jianghu66.top

[R71] 日期格式化
来源：http://znn.pycfn.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://eca.guowangkeji.top

[R72] 等待端口就绪
来源：http://zjh.hfpthk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hzh.yfazqb.com

[R73] 分割大日志
来源：http://fvc.yvedp.cn

split -l 1000 big.log part_
来源：http://qdo.jinyuanbaomall.cn

[R74] 批量重命名
来源：http://xmg.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sbc.ivvv.top

[R75] 导出环境变量
来源：http://grp.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://ydf.yongpay.top

[R76] 使用临时文件
来源：http://vgo.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gzv.52xcode.cn

[R77] 读取用户输入
来源：http://rrc.xuetiantiany.cn

read -rp "请输入: " ans
来源：http://gwd.jqgfzy.top

[R78] 交互式菜单
来源：http://pdj.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://skm.hnxiangtu.top

[R79] 解析命令行选项
来源：http://nhz.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gmx.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://wmx.cqqwz.cn

time ./run.sh
来源：http://gih.yongpay.top

================================================================================
来源：http://ugi.tarul.cn

S. C / C++ 专题
来源：http://rdi.hongshengwenyu.top

================================================================================
来源：http://olp.shuidangran.top

[S01] C：Hello World
来源：http://jat.dashuyun.cn

#include <stdio.h>
来源：http://ssp.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xqd.fktsv.cn

[S02] C：变量与格式化输出
来源：http://gsx.mhx1999.top

int a = 10; printf("%d\n", a);
来源：http://xlr.jqgfzy.top

[S03] C：读入整数
来源：http://kjn.tianlin.xyz

int x; scanf("%d", &x);
来源：http://ulc.jinqigfzy.top

[S04] C：字符串复制
来源：http://gjx.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://etp.c1oappe.top

[S05] C：字符串长度
来源：http://gvr.dianchejie.cn

strlen(s)
来源：http://poa.jqgufenzy.top

[S06] C：字符串比较
来源：http://sep.svipenyu.cn

strcmp(a, b) == 0
来源：http://zun.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://xhz.jiagoushi.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qws.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://acc.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cns.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://arb.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vod.smart0.xyz

[S10] C：指针与解引用
来源：http://yzs.smart0.xyz

int *p = &a;  *p = 5;
来源：http://tiz.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://sjp.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://vbn.sysykeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bqa.vehdjk.com

fclose(f);
来源：http://bin.nwbrower.top

[S12] C：写文件
来源：http://jxw.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hcy.zhixingplan.top

[S13] C：宏定义
来源：http://cyc.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mcl.shuidangran.top

[S14] C：枚举
来源：http://olo.pengpengdd.cyou

enum Color { RED, GREEN, BLUE };
来源：http://ate.smart0.xyz

[S15] C：类型转换
来源：http://luy.feifeiyinyue.top

(double) a / b
来源：http://gfk.xziqi.cn

[S16] C：位操作置位
来源：http://yeu.andypj.xyz

x |= (1 << 3);
来源：http://mnn.ybcxt.top

[S17] C：安全拼接字符串
来源：http://kzt.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nsj.c1oappe.top

[S18] C：命令行参数
来源：http://hbo.zhijiandao.cn

int main(int argc, char **argv)
来源：http://efx.ehwqpu.com

[S19] C：快速排序
来源：http://ghp.c1oappe.top

qsort(a, n, sizeof(int), cmp);
来源：http://xpx.ivvv.top

[S20] C：二分查找
来源：http://sog.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vrb.yuxming.cn

[S21] C：字符类别判断
来源：http://acb.fehbvm.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://isl.ivvv.top

[S22] C：字符串转数字
来源：http://hdg.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://yql.smart0.xyz

[S23] C：随机数
来源：http://exp.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://vcw.xziqi.cn

[S24] C：获取本地时间
来源：http://sen.yj20258.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xyu.nanxuanxn.top

[S25] C：内存拷贝
来源：http://esl.hfpthk.cn

memcpy(dst, src, n);
来源：http://tha.birdmap.top

[S26] C：内存清零
来源：http://xcs.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://lua.daxiang520.top

[S27] C：定义常量
来源：http://nmz.tianlin.xyz

const double PI = 3.14159;
来源：http://ndc.aizwys.cn

[S28] C：静态变量
来源：http://jpi.dashuyun.cn

static int counter = 0;
来源：http://yvz.sweek.top

[S29] C：变参函数
来源：http://amc.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://irq.zdqjudy.top

[S30] C：头文件保护
来源：http://eaa.xuetiantiany.cn

#ifndef X_H
来源：http://hpg.cucudq.cn

#define X_H
来源：http://dyv.redwolf501.top

#endif
来源：http://fab.shangyingyoupin.top

[S31] C++：Hello World
来源：http://ohf.cheryme.top

#include <iostream>
来源：http://jct.xinyue.icu

int main() { std::cout << "Hello\n"; }
来源：http://hqx.nwbrower.top

[S32] C++：字符串
来源：http://nte.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://jqq.gogol.net.cn

[S33] C++：vector 增删
来源：http://hme.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qye.zdbjq.cn

[S34] C++：遍历 vector
来源：http://pcc.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://vsr.cashguo.top

[S35] C++：map
来源：http://pqv.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xdj.sweek.top

[S36] C++：unordered_map
来源：http://nbm.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gdi.chenzaomai.com

[S37] C++：set
来源：http://zpa.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tdn.ehwqpu.com

[S38] C++：排序
来源：http://jkm.xuanzx.com

std::sort(v.begin(), v.end());
来源：http://vrf.meibo888.top

[S39] C++：自定义比较器排序
来源：http://xqx.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pcw.hesvh.cn

[S40] C++：查找元素
来源：http://lcg.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tbz.tian-w.cn

[S41] C++：类与构造函数
来源：http://uje.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yeb.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://ljx.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://mxz.wangdashe.top

[S43] C++：智能指针
来源：http://otu.sufxvd.cn

auto p = std::make_unique<int>(5);
来源：http://ogk.hongshengwenyu.top

[S44] C++：引用传参
来源：http://fqv.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://fqz.sysykeji.top

[S45] C++：lambda
来源：http://zwg.tianlin.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://fhz.guannengcc.top

[S46] C++：函数模板
来源：http://txl.wangdashe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jdc.fehbvm.com

[S47] C++：结构化绑定遍历
来源：http://mdm.yangfankeji.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fri.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://mzy.gaohongyu789.top

std::ifstream in("a.txt");  std::string line;
来源：http://ldd.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://ofr.haohaochexian.top

[S49] C++：写文件
来源：http://zzb.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gku.tarul.cn

[S50] C++：格式化数字
来源：http://rbm.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kod.sweek.top

[S51] C++：显式类型转换
来源：http://vqk.yvedp.cn

static_cast<double>(a) / b
来源：http://eua.sxryk.cn

[S52] C++：const 与 noexcept
来源：http://zve.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://mhg.ctjpmb.com

[S53] C++：移动语义
来源：http://ohl.jqgfzy.top

std::vector<int> w = std::move(v);
来源：http://ski.epnwcf.com

[S54] C++：异常处理
来源：http://qji.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zsq.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://xua.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xhw.svipenyu.cn

[S56] C++：optional
来源：http://laq.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zpa.yvedp.cn

[S57] C++：编译期常量
来源：http://tnt.yuanzhike.top

constexpr int N = 10;
来源：http://kpl.hcnkem.com

[S58] C++：命名空间
来源：http://wdf.sjlbkw.cn

namespace ns { int f() { return 1; } }
来源：http://kuo.yuxming.cn

[S59] C++：静态断言
来源：http://tdb.xuetiantiany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ofl.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://xls.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nav.c1oappe.top

================================================================================
来源：http://imn.cheryme.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rat.xziqi.cn

================================================================================
来源：http://fsh.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://mlz.daria6918.cn

println("Hello")
来源：http://vcm.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://mde.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xlu.tanke756.top

[T03] Kotlin：字符串模板
来源：http://iwr.zdqjudy.top

"值: $b"
来源：http://zju.gzhubu.top

[T04] Kotlin：空安全
来源：http://vcb.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://lzh.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://rhx.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mpc.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://efq.hongshengwenyu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yjp.cashguo.top

[T07] Kotlin：集合过滤
来源：http://ahs.bbcook.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kxf.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://qcy.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://smv.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://diz.zhijiandao.cn

fun String.exclaim() = this + "!"
来源：http://jns.shanyushiyangkeji.top

[T10] Kotlin：默认参数
来源：http://ewp.bjfxy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://flf.wangdashe.top

[T11] Kotlin：协程
来源：http://uvv.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tpa.daria6918.cn

[T12] Kotlin：解构声明
来源：http://jxx.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://myy.yuxming.cn

[T13] Kotlin：只读 Map
来源：http://vpp.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://nuq.hywenlv.cn

[T14] Kotlin：循环
来源：http://aww.yongpay.top

for (i in 1..10) println(i)
来源：http://gye.aibaodan.cn

[T15] Kotlin：接口
来源：http://qji.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://txj.chenlongwang.top

[T16] Swift：Hello World
来源：http://htn.dianchejie.cn

print("Hello")
来源：http://ykd.ppjwa.cn

[T17] Swift：变量与常量
来源：http://eva.yfazqb.com

var a = 1;  let b = 2
来源：http://snz.gogol.net.cn

[T18] Swift：字符串插值
来源：http://oem.zhixingplan.top

"值: \(b)"
来源：http://rsf.yangfankeji.com

[T19] Swift：可选绑定
来源：http://qui.zycfv.cn

if let n = opt { print(n) }
来源：http://ddr.iojbl.cn

[T20] Swift：数组操作
来源：http://nqw.ppjwa.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vch.wangdashe.top

[T21] Swift：遍历
来源：http://msu.epnwcf.com

for x in a { print(x) }
来源：http://kgk.cucudq.cn

[T22] Swift：字典
来源：http://uqx.uphjek.com

var d = ["a": 1];  d["b"] = 2
来源：http://ala.shuidangran.top

[T23] Swift：函数
来源：http://mza.xuetiantiany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rkq.fanxiaobao.xyz

[T24] Swift：闭包
来源：http://nht.316326.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://qlr.hysaishi.cn

[T25] Swift：结构体
来源：http://low.yongpay.top

struct P { var x: Int }
来源：http://hac.ctjpmb.com

[T26] Swift：类与重写
来源：http://rah.mhx1999.top

class A: Base { override func f() {} }
来源：http://mag.havefunace.top

[T27] Swift：错误处理
来源：http://wip.chenlongwang.top

do { try f() } catch { print(error) }
来源：http://zpo.wangshuangyany.cn

[T28] Swift：枚举
来源：http://srt.sxryk.cn

enum Color { case red, green }
来源：http://rmb.shzxlz.cn

[T29] Swift：guard 提前返回
来源：http://spw.xylfe.cn

guard let x = opt else { return }
来源：http://oiw.ehwqpu.com

[T30] Swift：协议
来源：http://fqt.yj202588.top

protocol Shape { func area() -> Double }
来源：http://ust.zdbjq.cn

[T31] Lua：Hello World
来源：http://ffh.cqqwz.cn

print("Hello")
来源：http://mca.zhoulong.xyz

[T32] Lua：局部变量
来源：http://elb.zycfv.cn

local a = 1
来源：http://vjf.tarul.cn

[T33] Lua：表（数组）
来源：http://hzh.pycfn.com

local t = {1, 2, 3};  t[4] = 4
来源：http://wwl.cqqwz.cn

[T34] Lua：遍历表
来源：http://hmj.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lia.zhengqikj.top

[T35] Lua：字典表
来源：http://jxp.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://uho.tian-w.cn

[T36] Lua：函数
来源：http://qor.yangfankeji.com

function add(a, b) return a + b end
来源：http://ipi.nwbrower.top

[T37] Lua：字符串拼接
来源：http://onp.quarkkingdee.top

"a" .. "b"
来源：http://wry.ybcxt.top

[T38] Lua：条件
来源：http://eqr.tarul.cn

if x > 0 then print("正") end
来源：http://wzt.ywan-chungtsiang.top

[T39] Lua：模式匹配
来源：http://fyh.fzhhl.top

string.find(s, "%d+")
来源：http://txd.havefunace.top

[T40] Lua：元表
来源：http://zoe.cucudq.cn

setmetatable({}, { __index = base })
来源：http://myn.zhixingplan.top

[T41] Perl：Hello World
来源：http://thl.tian-w.cn

print "Hello\n";
来源：http://qcf.wangdashe.top

[T42] Perl：变量类型
来源：http://bsf.hongshengwenyu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://toi.zhongyouzk.top

[T43] Perl：字符串插值
来源：http://dxu.zdbjq.cn

"值: $a"
来源：http://lsw.chenzaomai.com

[T44] Perl：条件
来源：http://iur.yangfankeji.com

if ($a > 0) { print "正"; }
来源：http://tyu.hysaishi.cn

[T45] Perl：数组遍历
来源：http://vik.ctjpmb.com

for my $x (@arr) { print $x; }
来源：http://gwv.yueranfly.top

[T46] Perl：哈希操作
来源：http://drx.gzhubu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sic.cqqwz.cn

[T47] Perl：正则捕获
来源：http://chj.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fwi.hammf.cn

[T48] Perl：正则替换
来源：http://euz.0kj1m.cn

$s =~ s/old/new/g;
来源：http://ixh.gotoacloud.top

[T49] Perl：函数
来源：http://qva.jinqigfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lvz.tarul.cn

[T50] Perl：逐行读文件
来源：http://lkn.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lfk.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://ejk.havefunace.top

[T51] Scala：Hello World
来源：http://dja.pengpengdd.cyou

println("Hello")
来源：http://ntd.hywenlv.cn

[T52] Scala：变量
来源：http://eka.yonumen.top


<!-- 参考信息 -->