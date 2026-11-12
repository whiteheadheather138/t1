代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kjx.jinqigfzy.top

[R54] 比较两个文件
来源：http://erv.hysaishi.cn

diff a.txt b.txt
来源：http://gjm.jyoumei.cn

[R55] 压缩与解压
来源：http://vwr.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ziy.nanxuanxn.top

[R56] 远程拷贝
来源：http://lps.uphjek.com

scp file user@host:/path/
来源：http://und.wangdashe.top

[R57] 远程执行命令
来源：http://jgc.dashuyun.cn

ssh user@host 'uptime'
来源：http://ttb.zhaomingkeji.xyz

[R58] 下载文件
来源：http://pll.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kld.haohaochexian.top

[R59] 发 POST JSON
来源：http://srw.zycfv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hvd.zhijiandao.cn

[R60] 只看 HTTP 状态码
来源：http://ffc.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yso.zhoulong.xyz

[R61] 磁盘占用
来源：http://una.zhiwuduotai.top

df -h;  du -sh *
来源：http://plj.zhijiandao.cn

[R62] 找最占空间的文件
来源：http://fui.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://qjb.ehwqpu.com

[R63] 内存与进程
来源：http://knx.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://ydb.aizwys.cn

[R64] 结束进程
来源：http://qyo.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://hke.jqgufenzy.top

[R65] 查看端口占用
来源：http://fdy.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hkf.cqqwz.cn

[R66] 定时任务
来源：http://lvy.uphjek.com

crontab -e;  crontab -l
来源：http://mvo.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://ywx.zhixingplan.top

openssl rand -hex 16
来源：http://oiv.sjlbkw.cn

[R68] 计算文件校验值
来源：http://kgj.epnwcf.com

sha256sum a.txt;  md5sum a.txt
来源：http://eoe.sxryk.cn

[R69] 生成随机密码
来源：http://kzp.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://eyl.gogol.net.cn

[R70] 时间戳与互转
来源：http://jun.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://hbe.fzhhl.top

[R71] 日期格式化
来源：http://mec.havefunace.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qil.tian-w.cn

[R72] 等待端口就绪
来源：http://ima.dianchejie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://trv.xylfe.cn

[R73] 分割大日志
来源：http://xsg.zhoulong.xyz

split -l 1000 big.log part_
来源：http://tdu.yangfankeji.com

[R74] 批量重命名
来源：http://xlh.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://slk.fengsongda.top

[R75] 导出环境变量
来源：http://fua.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://wte.aibaodan.cn

[R76] 使用临时文件
来源：http://ejd.guowangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ppd.birdmap.top

[R77] 读取用户输入
来源：http://gch.zhijiandao.cn

read -rp "请输入: " ans
来源：http://pvq.gaohongyu789.top

[R78] 交互式菜单
来源：http://ivn.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qku.yongpay.top

[R79] 解析命令行选项
来源：http://isn.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://azl.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://cfv.yvedp.cn

time ./run.sh
来源：http://wts.zdqjudy.top

================================================================================
来源：http://fyy.ppjwa.cn

S. C / C++ 专题
来源：http://stk.jinqigufen.top

================================================================================
来源：http://jbq.tian-w.cn

[S01] C：Hello World
来源：http://yhi.cdnleiting.top

#include <stdio.h>
来源：http://ssc.316326.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://rsv.zhongyouzk.top

[S02] C：变量与格式化输出
来源：http://trd.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://bjv.kuanghao11.cn

[S03] C：读入整数
来源：http://ioh.havefunace.top

int x; scanf("%d", &x);
来源：http://ksg.yj20258888.top

[S04] C：字符串复制
来源：http://jhl.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://qdc.jinyuanbaomall.cn

[S05] C：字符串长度
来源：http://cnn.jlsjyb.cn

strlen(s)
来源：http://ckl.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://env.xuetiantiany.cn

strcmp(a, b) == 0
来源：http://ecu.xylfe.cn

[S07] C：数组遍历求和
来源：http://raj.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sji.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://ycs.uphjek.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zed.hammf.cn

[S09] C：结构体定义与初始化
来源：http://klv.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vxa.316326.xyz

[S10] C：指针与解引用
来源：http://mig.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://vli.guowangkeji.top

[S11] C：逐行读文件
来源：http://hzk.zhiwuduotai.top

FILE *f = fopen("a.txt", "r");
来源：http://qbu.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nrq.kuanghao11.cn

fclose(f);
来源：http://fed.nanxinkj.top

[S12] C：写文件
来源：http://cbv.yanxiufei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://epm.cucudq.cn

[S13] C：宏定义
来源：http://ddb.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mqa.smart0.xyz

[S14] C：枚举
来源：http://ske.ydzc1.top

enum Color { RED, GREEN, BLUE };
来源：http://fqi.birdmap.top

[S15] C：类型转换
来源：http://ooj.fanxiaobao.xyz

(double) a / b
来源：http://yff.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://dyn.pengpengdd.cyou

x |= (1 << 3);
来源：http://ubk.wangdashe.top

[S17] C：安全拼接字符串
来源：http://ohl.xylfe.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ohm.zhaomingkeji.xyz

[S18] C：命令行参数
来源：http://esx.vehdjk.com

int main(int argc, char **argv)
来源：http://gwf.sjlbkw.cn

[S19] C：快速排序
来源：http://ape.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://kst.fehbvm.com

[S20] C：二分查找
来源：http://wra.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yzv.tian-w.cn

[S21] C：字符类别判断
来源：http://ocw.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ddv.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://cjx.yvedp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oqf.ybcxt.top

[S23] C：随机数
来源：http://lza.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rih.hysaishi.cn

[S24] C：获取本地时间
来源：http://uss.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ips.sweek.top

[S25] C：内存拷贝
来源：http://cyo.haohaochexian.top

memcpy(dst, src, n);
来源：http://sjq.andypj.xyz

[S26] C：内存清零
来源：http://ily.daxiang520.top

memset(a, 0, sizeof a);
来源：http://wnv.ctjpmb.com

[S27] C：定义常量
来源：http://mud.zdqjudy.top

const double PI = 3.14159;
来源：http://ubd.havefunace.top

[S28] C：静态变量
来源：http://kup.ehwqpu.com

static int counter = 0;
来源：http://pvg.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://ram.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vul.xuanzx.com

[S30] C：头文件保护
来源：http://glj.hfpthk.cn

#ifndef X_H
来源：http://uzy.zdqjudy.top

#define X_H
来源：http://tpm.tarul.cn

#endif
来源：http://zas.haohaochexian.top

[S31] C++：Hello World
来源：http://xyd.jlsjyb.cn

#include <iostream>
来源：http://dbc.ctjpmb.com

int main() { std::cout << "Hello\n"; }
来源：http://fwm.fengsongda.top

[S32] C++：字符串
来源：http://dby.jinqigfzy.top

std::string s = "hi";  s += "!";
来源：http://ycy.hfpthk.cn

[S33] C++：vector 增删
来源：http://bpu.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://amj.chenlongwang.top

[S34] C++：遍历 vector
来源：http://rnl.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://pzj.hesvh.cn

[S35] C++：map
来源：http://mmx.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bga.quarkkingdee.top

[S36] C++：unordered_map
来源：http://vsu.iojbl.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qmv.chenzaomai.com

[S37] C++：set
来源：http://qvu.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://myj.jyoumei.cn

[S38] C++：排序
来源：http://huc.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://jfy.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://bvz.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://clp.yanxiufei.cn

[S40] C++：查找元素
来源：http://kec.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fls.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://ngr.jinqigfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bfy.c1oappe.top

[S42] C++：继承与虚函数
来源：http://saw.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://xus.cheryme.top

[S43] C++：智能指针
来源：http://seh.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://vzb.gogol.net.cn

[S44] C++：引用传参
来源：http://dpw.daria6918.cn

void inc(int &x) { ++x; }
来源：http://mgg.yfazqb.com

[S45] C++：lambda
来源：http://ixv.chenjidiqi.icu

auto add = [](int a, int b) { return a + b; };
来源：http://mec.ydjk.org.cn

[S46] C++：函数模板
来源：http://pcq.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ydo.sjlbkw.cn

[S47] C++：结构化绑定遍历
来源：http://mqk.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bay.tian-w.cn

[S48] C++：逐行读文件
来源：http://ipq.fengsongda.top

std::ifstream in("a.txt");  std::string line;
来源：http://qou.cashguo.top

while (std::getline(in, line)) { }
来源：http://gux.dianchejie.cn

[S49] C++：写文件
来源：http://dnh.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fks.zdqjudy.top

[S50] C++：格式化数字
来源：http://xjj.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cko.shuidangran.top

[S51] C++：显式类型转换
来源：http://awq.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://cyj.sweek.top

[S52] C++：const 与 noexcept
来源：http://ueq.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://fme.aibaodan.cn

[S53] C++：移动语义
来源：http://kvi.aizwys.cn

std::vector<int> w = std::move(v);
来源：http://mjv.xinyue.icu

[S54] C++：异常处理
来源：http://bea.9152youxi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xro.c1oappe.top

[S55] C++：结构化绑定
来源：http://nyf.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cyt.hysaishi.cn

[S56] C++：optional
来源：http://zql.hysaishi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rwn.fktsv.cn

[S57] C++：编译期常量
来源：http://yed.fehbvm.com

constexpr int N = 10;
来源：http://cpi.ydjk.org.cn

[S58] C++：命名空间
来源：http://ibi.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://lou.jqgufenzy.top

[S59] C++：静态断言
来源：http://vzc.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://noz.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://zfn.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pmi.ctjpmb.com

================================================================================
来源：http://cks.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nua.tanke756.top

================================================================================
来源：http://hmd.hongshengwenyu.top

[T01] Kotlin：Hello World
来源：http://lqx.xylfe.cn

println("Hello")
来源：http://uvc.iojbl.cn

[T02] Kotlin：变量
来源：http://bwy.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://obw.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://qky.havefunace.top

"值: $b"
来源：http://obb.nwbrower.top

[T04] Kotlin：空安全
来源：http://fxt.svipenyu.cn

val n: String? = null;  n?.length
来源：http://dlg.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://uos.snrcjt.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jic.fanxiaobao.xyz

[T06] Kotlin：集合映射
来源：http://tmr.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fpc.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://idq.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://oat.ydzc1.top

[T08] Kotlin：数据类
来源：http://ozf.yvedp.cn

data class User(val name: String, val age: Int)
来源：http://siv.sweek.top

[T09] Kotlin：扩展函数
来源：http://sti.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://xrg.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://pmk.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pxw.ybcxt.top

[T11] Kotlin：协程
来源：http://meb.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wsa.guowangkeji.top

[T12] Kotlin：解构声明
来源：http://sbw.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://mpk.ydzc1.top

[T13] Kotlin：只读 Map
来源：http://mfb.vehdjk.com

val m = mapOf("a" to 1)
来源：http://uya.aizwys.cn

[T14] Kotlin：循环
来源：http://ikz.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://aqd.yueranfly.top

[T15] Kotlin：接口
来源：http://cnr.daxiang520.top

interface Shape { fun area(): Double }
来源：http://xgq.nanxuanxn.top

[T16] Swift：Hello World
来源：http://qse.fktsv.cn

print("Hello")
来源：http://liz.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://zzm.xuetiantiany.cn

var a = 1;  let b = 2
来源：http://jsq.fehbvm.com

[T18] Swift：字符串插值
来源：http://mng.zhixingplan.top

"值: \(b)"
来源：http://vih.snrcjt.cn

[T19] Swift：可选绑定
来源：http://eok.hnqzz.top

if let n = opt { print(n) }
来源：http://dam.kuanghao11.cn

[T20] Swift：数组操作
来源：http://sxq.jiagoushi.top

var a = [1, 2, 3];  a.append(4)
来源：http://hla.vehdjk.com

[T21] Swift：遍历
来源：http://ara.yongpay.top

for x in a { print(x) }
来源：http://ykl.hongshengwenyu.top

[T22] Swift：字典
来源：http://jvm.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://qkn.tanke756.top

[T23] Swift：函数
来源：http://ida.havefunace.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sbw.epnwcf.com

[T24] Swift：闭包
来源：http://ray.gzhubu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fkd.gaohongyu789.top

[T25] Swift：结构体
来源：http://dgz.jyoumei.cn

struct P { var x: Int }
来源：http://bmh.gaohongyu789.top

[T26] Swift：类与重写
来源：http://gcj.pycfn.com

class A: Base { override func f() {} }
来源：http://kho.gzhubu.top

[T27] Swift：错误处理
来源：http://qdy.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://tpi.xuanzx.com

[T28] Swift：枚举
来源：http://pgw.birdmap.top

enum Color { case red, green }
来源：http://hny.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://lja.jinqigufen.top

guard let x = opt else { return }
来源：http://djq.xuetiantiany.cn

[T30] Swift：协议
来源：http://scm.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://bof.svipenyu.cn

[T31] Lua：Hello World
来源：http://cxi.quarkkingdee.top

print("Hello")
来源：http://xai.vqdsnc.cn

[T32] Lua：局部变量
来源：http://idq.feifeiyinyue.top

local a = 1
来源：http://vve.xziqi.cn

[T33] Lua：表（数组）
来源：http://ckg.hcnkem.com

local t = {1, 2, 3};  t[4] = 4
来源：http://zbi.vehdjk.com

[T34] Lua：遍历表
来源：http://srj.xuanzx.com

for i, v in ipairs(t) do print(i, v) end
来源：http://dhj.svipenyu.cn

[T35] Lua：字典表
来源：http://voe.hysaishi.cn

local d = { a = 1 };  d.b = 2
来源：http://kqy.sysykeji.top

[T36] Lua：函数
来源：http://uyb.yangfankeji.com

function add(a, b) return a + b end
来源：http://epn.xuanzx.com

[T37] Lua：字符串拼接
来源：http://vwf.guannengcc.top

"a" .. "b"
来源：http://idv.hcnkem.com

[T38] Lua：条件
来源：http://pds.daria6918.cn

if x > 0 then print("正") end
来源：http://due.bbcook.cn

[T39] Lua：模式匹配
来源：http://yza.yfazqb.com

string.find(s, "%d+")
来源：http://pii.hcnkem.com

[T40] Lua：元表
来源：http://ibg.ctjpmb.com

setmetatable({}, { __index = base })
来源：http://aov.jyoumei.cn

[T41] Perl：Hello World
来源：http://jue.hysaishi.cn

print "Hello\n";
来源：http://aqt.pycfn.com

[T42] Perl：变量类型
来源：http://ina.shanyushiyangtech.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sam.smart0.xyz

[T43] Perl：字符串插值
来源：http://zyz.gogol.net.cn

"值: $a"
来源：http://ypy.ydzc1.top

[T44] Perl：条件
来源：http://dyq.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://joz.fzhhl.top

[T45] Perl：数组遍历
来源：http://yhs.vehdjk.com

for my $x (@arr) { print $x; }
来源：http://hmn.wangshuangyany.cn

[T46] Perl：哈希操作
来源：http://sar.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zfb.mhx1999.top

[T47] Perl：正则捕获
来源：http://xfc.jinqigfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rqo.hongshengwenyu.top

[T48] Perl：正则替换
来源：http://kuo.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://yxo.chenlongwang.top

[T49] Perl：函数
来源：http://uru.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vay.zycfv.cn

[T50] Perl：逐行读文件
来源：http://zma.bbcook.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uvy.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://ezf.fehbvm.com

[T51] Scala：Hello World
来源：http://lxp.0kj1m.cn

println("Hello")
来源：http://xjl.yj202588.top

[T52] Scala：变量
来源：http://jtf.hfpthk.cn

val a = 1;  var b = 2
来源：http://bzj.yfazqb.com

[T53] Scala：字符串插值
来源：http://mqb.bbcook.cn

s"值: $b"
来源：http://uxi.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://dry.xinyue.icu

List(1, 2, 3).map(_ * 2)
来源：http://xso.tanke756.top

[T55] Scala：集合过滤
来源：http://dif.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://eau.shzxlz.cn

[T56] Scala：样例类
来源：http://ktj.zycfv.cn


<!-- 参考信息 -->