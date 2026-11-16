代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hkp.pycfn.com

[R50] awk 求和
来源：http://vfu.tianlin.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://pvz.yueranfly.top

[R51] 排序去重取前几
来源：http://yog.jlsjyb.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://umo.wangshuangyany.cn

[R52] 统计行数
来源：http://pzz.hongshengwenyu.top

wc -l a.txt
来源：http://vse.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://qqb.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zel.gogol.net.cn

[R54] 比较两个文件
来源：http://iuc.dianchejie.cn

diff a.txt b.txt
来源：http://fnm.wangdashe.top

[R55] 压缩与解压
来源：http://tvl.shzxlz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://axf.nanxinkj.top

[R56] 远程拷贝
来源：http://ccd.jinghuilouyu.cn

scp file user@host:/path/
来源：http://osk.yfazqb.com

[R57] 远程执行命令
来源：http://qzz.tian-w.cn

ssh user@host 'uptime'
来源：http://ljo.birdmap.top

[R58] 下载文件
来源：http://qxn.chenjidiqi.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gxp.uphjek.com

[R59] 发 POST JSON
来源：http://wiw.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zkd.bbcook.cn

[R60] 只看 HTTP 状态码
来源：http://zef.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vih.hesvh.cn

[R61] 磁盘占用
来源：http://uoc.jlsjyb.cn

df -h;  du -sh *
来源：http://xld.tarul.cn

[R62] 找最占空间的文件
来源：http://gik.hongshengwenyu.top

du -ah . | sort -rh | head -10
来源：http://zhw.cucudq.cn

[R63] 内存与进程
来源：http://mvs.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://wmk.cdnleiting.top

[R64] 结束进程
来源：http://hfd.xuanzx.com

kill -9 $(pgrep -f app.py)
来源：http://zeu.sjlbkw.cn

[R65] 查看端口占用
来源：http://tgv.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ree.guowangkeji.top

[R66] 定时任务
来源：http://sjl.yfazqb.com

crontab -e;  crontab -l
来源：http://nzj.yuxming.cn

[R67] 生成随机十六进制串
来源：http://udy.ydjk.org.cn

openssl rand -hex 16
来源：http://fkl.jqgufenzy.top

[R68] 计算文件校验值
来源：http://nxx.xingfuxueyuan.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://hkx.xuanzx.com

[R69] 生成随机密码
来源：http://rnl.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://hpd.quarkkingdee.top

[R70] 时间戳与互转
来源：http://cdb.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://dwc.hysaishi.cn

[R71] 日期格式化
来源：http://zgc.xinyue.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://oph.nwbrower.top

[R72] 等待端口就绪
来源：http://cml.nwbrower.top

until nc -z localhost 3306; do sleep 1; done
来源：http://haa.xuetiantiany.cn

[R73] 分割大日志
来源：http://cmp.jiagoushi.top

split -l 1000 big.log part_
来源：http://rba.yanxiufei.cn

[R74] 批量重命名
来源：http://fsv.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jag.zycfv.cn

[R75] 导出环境变量
来源：http://asb.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://ede.yangfankeji.com

[R76] 使用临时文件
来源：http://sxa.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iac.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://lac.ywan-chungtsiang.top

read -rp "请输入: " ans
来源：http://ysp.hnxiangtu.top

[R78] 交互式菜单
来源：http://ipt.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tzk.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://whn.hongshengwenyu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://szt.hfpthk.cn

[R80] 查看脚本执行耗时
来源：http://qvm.xuanzx.com

time ./run.sh
来源：http://byk.havefunace.top

================================================================================
来源：http://vik.pycfn.com

S. C / C++ 专题
来源：http://odf.zhoulong.xyz

================================================================================
来源：http://cdd.cucudq.cn

[S01] C：Hello World
来源：http://tno.haohaochexian.top

#include <stdio.h>
来源：http://abi.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fcm.vehdjk.com

[S02] C：变量与格式化输出
来源：http://ole.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://vrf.svipenyu.cn

[S03] C：读入整数
来源：http://baa.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://tvz.ivvv.top

[S04] C：字符串复制
来源：http://dva.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://kuk.aibaodan.cn

[S05] C：字符串长度
来源：http://psk.jyoumei.cn

strlen(s)
来源：http://tpu.haohaochexian.top

[S06] C：字符串比较
来源：http://ojx.aibaodan.cn

strcmp(a, b) == 0
来源：http://zgd.fktsv.cn

[S07] C：数组遍历求和
来源：http://lff.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eso.316326.xyz

[S08] C：动态内存分配与释放
来源：http://mct.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://btp.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://duh.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lxx.hnxiangtu.top

[S10] C：指针与解引用
来源：http://eqq.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://ulu.birdmap.top

[S11] C：逐行读文件
来源：http://sfo.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://ypj.dianchejie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cwo.shuidangran.top

fclose(f);
来源：http://hnz.hcnkem.com

[S12] C：写文件
来源：http://gmf.vqdsnc.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tnw.zhiwuduotai.top

[S13] C：宏定义
来源：http://abf.52xcode.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zgl.pycfn.com

[S14] C：枚举
来源：http://edl.daria6918.cn

enum Color { RED, GREEN, BLUE };
来源：http://urj.ehwqpu.com

[S15] C：类型转换
来源：http://sck.sjlbkw.cn

(double) a / b
来源：http://cii.cucudq.cn

[S16] C：位操作置位
来源：http://gzo.hcnkem.com

x |= (1 << 3);
来源：http://nbx.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://jer.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cxd.hongshengwenyu.top

[S18] C：命令行参数
来源：http://ezg.yj20258888.top

int main(int argc, char **argv)
来源：http://ddj.vehdjk.com

[S19] C：快速排序
来源：http://czt.nanxuanxn.top

qsort(a, n, sizeof(int), cmp);
来源：http://ylh.shuidangran.top

[S20] C：二分查找
来源：http://nfr.nanxinkj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gvp.jianghu66.top

[S21] C：字符类别判断
来源：http://usi.zhongyouzk.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://flb.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://bce.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://pws.yvedp.cn

[S23] C：随机数
来源：http://aei.chenjidiqi.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://nfs.daxiang520.top

[S24] C：获取本地时间
来源：http://zpm.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dor.hcnkem.com

[S25] C：内存拷贝
来源：http://awt.tian-w.cn

memcpy(dst, src, n);
来源：http://diz.bbcook.cn

[S26] C：内存清零
来源：http://kvj.cdnleiting.top

memset(a, 0, sizeof a);
来源：http://ldv.chenjidiqi.icu

[S27] C：定义常量
来源：http://liv.ehwqpu.com

const double PI = 3.14159;
来源：http://oej.sufxvd.cn

[S28] C：静态变量
来源：http://wmo.fktsv.cn

static int counter = 0;
来源：http://scr.ctjpmb.com

[S29] C：变参函数
来源：http://hum.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bme.nanxinkj.top

[S30] C：头文件保护
来源：http://iaa.shzxlz.cn

#ifndef X_H
来源：http://eoc.dashuyun.cn

#define X_H
来源：http://eki.tarul.cn

#endif
来源：http://amx.tanke756.top

[S31] C++：Hello World
来源：http://pnd.zdbjq.cn

#include <iostream>
来源：http://abi.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://vtt.zhoulong.xyz

[S32] C++：字符串
来源：http://hfa.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://vfw.dashuyun.cn

[S33] C++：vector 增删
来源：http://wbw.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rxx.jqgfzy.top

[S34] C++：遍历 vector
来源：http://wmd.cqqwz.cn

for (auto &x : v) { std::cout << x; }
来源：http://opk.xingfuxueyuan.xyz

[S35] C++：map
来源：http://lfg.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uwe.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://fvt.chenjidiqi.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ybh.tanke756.top

[S37] C++：set
来源：http://kpy.jinqigfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://acu.jinqigfzy.top

[S38] C++：排序
来源：http://chq.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://ikd.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://sbq.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tmp.kuanghao11.cn

[S40] C++：查找元素
来源：http://ogg.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uij.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://cck.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wex.nanxinkj.top

[S42] C++：继承与虚函数
来源：http://yiv.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://hdo.hammf.cn

[S43] C++：智能指针
来源：http://gez.hammf.cn

auto p = std::make_unique<int>(5);
来源：http://qdd.hnxiangtu.top

[S44] C++：引用传参
来源：http://zxk.uphjek.com

void inc(int &x) { ++x; }
来源：http://zaz.zhaomingkeji.xyz

[S45] C++：lambda
来源：http://gqs.xuanzx.com

auto add = [](int a, int b) { return a + b; };
来源：http://jtq.xingfuxueyuan.xyz

[S46] C++：函数模板
来源：http://tgo.gzhubu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kby.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://qjn.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kno.jyoumei.cn

[S48] C++：逐行读文件
来源：http://zip.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fhk.wangdashe.top

while (std::getline(in, line)) { }
来源：http://vgu.feifeiyinyue.top

[S49] C++：写文件
来源：http://ozz.yj20258.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oho.yvedp.cn

[S50] C++：格式化数字
来源：http://nvw.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kip.c1oappe.top

[S51] C++：显式类型转换
来源：http://sfu.fengsongda.top

static_cast<double>(a) / b
来源：http://klr.tarul.cn

[S52] C++：const 与 noexcept
来源：http://set.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://kqg.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://unx.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://gqg.mhx1999.top

[S54] C++：异常处理
来源：http://eow.cdnleiting.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nrl.jqgufenzy.top

[S55] C++：结构化绑定
来源：http://pxo.sysykeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ill.gzhubu.top

[S56] C++：optional
来源：http://hxo.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bex.0kj1m.cn

[S57] C++：编译期常量
来源：http://njo.nanxuanxn.top

constexpr int N = 10;
来源：http://zqj.tianlin.xyz

[S58] C++：命名空间
来源：http://ldy.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://slp.gogol.net.cn

[S59] C++：静态断言
来源：http://sxu.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cqw.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://lcj.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://chl.chenzaomai.com

================================================================================
来源：http://usm.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://npk.mhx1999.top

================================================================================
来源：http://mgb.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://jje.zhoulong.xyz

println("Hello")
来源：http://dhp.c1oappe.top

[T02] Kotlin：变量
来源：http://uls.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cay.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://qge.316326.xyz

"值: $b"
来源：http://jev.daxiang520.top

[T04] Kotlin：空安全
来源：http://qhm.andypj.xyz

val n: String? = null;  n?.length
来源：http://kjr.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://wsq.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xdc.hnqzz.top

[T06] Kotlin：集合映射
来源：http://tlu.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gzf.smart0.xyz

[T07] Kotlin：集合过滤
来源：http://wem.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bpc.ehwqpu.com

[T08] Kotlin：数据类
来源：http://xsu.9152youxi.cn

data class User(val name: String, val age: Int)
来源：http://bts.snrcjt.cn

[T09] Kotlin：扩展函数
来源：http://ppm.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://hqf.gotoacloud.top

[T10] Kotlin：默认参数
来源：http://wlf.bbcook.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gew.xylfe.cn

[T11] Kotlin：协程
来源：http://ihu.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xjv.hammf.cn

[T12] Kotlin：解构声明
来源：http://tkb.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://qmz.tarul.cn

[T13] Kotlin：只读 Map
来源：http://qms.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://mnk.kuanghao11.cn

[T14] Kotlin：循环
来源：http://jkq.52xcode.cn

for (i in 1..10) println(i)
来源：http://ymg.bbcook.cn

[T15] Kotlin：接口
来源：http://dlc.cashguo.top

interface Shape { fun area(): Double }
来源：http://fik.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://stu.chenlongwang.top

print("Hello")
来源：http://ttw.yvedp.cn

[T17] Swift：变量与常量
来源：http://ilk.hesvh.cn

var a = 1;  let b = 2
来源：http://hfe.shzxlz.cn

[T18] Swift：字符串插值
来源：http://wlh.birdmap.top

"值: \(b)"
来源：http://uwb.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://ixy.cucudq.cn

if let n = opt { print(n) }
来源：http://jvd.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://mev.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uuf.zdbjq.cn

[T21] Swift：遍历
来源：http://jpd.smart0.xyz

for x in a { print(x) }
来源：http://mdh.shzxlz.cn

[T22] Swift：字典
来源：http://hvg.hongshengwenyu.top

var d = ["a": 1];  d["b"] = 2
来源：http://wvw.jianghu66.top

[T23] Swift：函数
来源：http://ypf.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lth.jqgfzy.top

[T24] Swift：闭包
来源：http://cgy.jqgfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hsb.yangfankeji.com

[T25] Swift：结构体
来源：http://hew.sysykeji.top

struct P { var x: Int }
来源：http://vxf.yj20258888.top

[T26] Swift：类与重写
来源：http://mvx.xuetiantiany.cn

class A: Base { override func f() {} }
来源：http://sar.hcnkem.com

[T27] Swift：错误处理
来源：http://wjd.yvedp.cn

do { try f() } catch { print(error) }
来源：http://ius.zhiwuduotai.top

[T28] Swift：枚举
来源：http://oey.gogol.net.cn

enum Color { case red, green }
来源：http://duh.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://fpm.yuanzhike.top

guard let x = opt else { return }
来源：http://pgo.nanxuanxn.top

[T30] Swift：协议
来源：http://qoq.ybcxt.top

protocol Shape { func area() -> Double }
来源：http://hyi.yfazqb.com

[T31] Lua：Hello World
来源：http://cjx.hfpthk.cn

print("Hello")
来源：http://sdt.chenlongwang.top

[T32] Lua：局部变量
来源：http://xqr.redwolf501.top

local a = 1
来源：http://nqv.bjfxy.top

[T33] Lua：表（数组）
来源：http://vdc.tarul.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://peq.bjfxy.top

[T34] Lua：遍历表
来源：http://pwq.yongpay.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bzx.andypj.xyz

[T35] Lua：字典表
来源：http://bmh.aizwys.cn

local d = { a = 1 };  d.b = 2
来源：http://qjt.daria6918.cn

[T36] Lua：函数
来源：http://hfq.quarkkingdee.top

function add(a, b) return a + b end
来源：http://uyf.tianlin.xyz

[T37] Lua：字符串拼接
来源：http://und.dianchejie.cn

"a" .. "b"
来源：http://dzo.9152youxi.cn

[T38] Lua：条件
来源：http://lqn.yuxming.cn

if x > 0 then print("正") end
来源：http://mis.havefunace.top

[T39] Lua：模式匹配
来源：http://crr.dashuyun.cn

string.find(s, "%d+")
来源：http://kxl.yvedp.cn

[T40] Lua：元表
来源：http://dgf.fengsongda.top

setmetatable({}, { __index = base })
来源：http://nwv.ctjpmb.com

[T41] Perl：Hello World
来源：http://sqs.zhixingplan.top

print "Hello\n";
来源：http://bfe.hfpthk.cn

[T42] Perl：变量类型
来源：http://obc.aizwys.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aex.kuanghao11.cn

[T43] Perl：字符串插值
来源：http://atk.hywenlv.cn

"值: $a"
来源：http://qbo.xylfe.cn

[T44] Perl：条件
来源：http://syf.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://uyr.yfazqb.com

[T45] Perl：数组遍历
来源：http://toz.cqqwz.cn

for my $x (@arr) { print $x; }
来源：http://wps.vehdjk.com

[T46] Perl：哈希操作
来源：http://uma.zhaomingkeji.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xut.feifeiyinyue.top

[T47] Perl：正则捕获
来源：http://xdr.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://ikw.gaohongyu789.top

[T48] Perl：正则替换
来源：http://azr.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://zvc.kuanghao11.cn

[T49] Perl：函数
来源：http://izx.hongshengwenyu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tdd.hesvh.cn

[T50] Perl：逐行读文件
来源：http://uwv.yuxming.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ums.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://jee.xinyue.icu

[T51] Scala：Hello World
来源：http://srg.chenjidiqi.icu

println("Hello")
来源：http://pdp.haohaochexian.top

[T52] Scala：变量
来源：http://yfq.epnwcf.com


<!-- 参考信息 -->