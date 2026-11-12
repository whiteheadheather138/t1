代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sar.cashguo.top

[R50] awk 求和
来源：http://pvn.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dko.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://upx.wangshuangyany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fok.pengpengdd.cyou

[R52] 统计行数
来源：http://jat.cqqwz.cn

wc -l a.txt
来源：http://oej.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://veh.hammf.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vts.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://wqn.yfazqb.com

diff a.txt b.txt
来源：http://bgf.ivvv.top

[R55] 压缩与解压
来源：http://dqd.zhiwuduotai.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tif.52xcode.cn

[R56] 远程拷贝
来源：http://fmt.xuetiantiany.cn

scp file user@host:/path/
来源：http://yhc.zhengqikj.top

[R57] 远程执行命令
来源：http://aje.wangshuangyany.cn

ssh user@host 'uptime'
来源：http://ifd.ppjwa.cn

[R58] 下载文件
来源：http://lgn.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://udp.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://sqq.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://osw.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://ojc.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zxr.yonumen.top

[R61] 磁盘占用
来源：http://rwc.sxryk.cn

df -h;  du -sh *
来源：http://wzd.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://low.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://yar.wangdashe.top

[R63] 内存与进程
来源：http://hyj.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://mrf.52xcode.cn

[R64] 结束进程
来源：http://twx.jinghuilouyu.cn

kill -9 $(pgrep -f app.py)
来源：http://jnc.havefunace.top

[R65] 查看端口占用
来源：http://jgc.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://czn.havefunace.top

[R66] 定时任务
来源：http://tsi.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://suq.jinyuanbaomall.cn

[R67] 生成随机十六进制串
来源：http://zqe.ehwqpu.com

openssl rand -hex 16
来源：http://lyk.fzhhl.top

[R68] 计算文件校验值
来源：http://yeq.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://beo.zhoulong.xyz

[R69] 生成随机密码
来源：http://pau.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://zju.52xcode.cn

[R70] 时间戳与互转
来源：http://omx.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://nss.dashuyun.cn

[R71] 日期格式化
来源：http://dbw.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://qry.nwbrower.top

[R72] 等待端口就绪
来源：http://mwt.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://iox.ivvv.top

[R73] 分割大日志
来源：http://ayg.tarul.cn

split -l 1000 big.log part_
来源：http://zaz.sxryk.cn

[R74] 批量重命名
来源：http://kbg.zhaomingkeji.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cbj.jiagoushi.top

[R75] 导出环境变量
来源：http://eaa.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://tau.chenjidiqi.icu

[R76] 使用临时文件
来源：http://yxu.wangshuangyany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dei.ivvv.top

[R77] 读取用户输入
来源：http://ayu.jinqigufen.top

read -rp "请输入: " ans
来源：http://ioy.sufxvd.cn

[R78] 交互式菜单
来源：http://ivh.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gjq.zhijiandao.cn

[R79] 解析命令行选项
来源：http://gut.yj202588.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xrx.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://alh.yueranfly.top

time ./run.sh
来源：http://dsy.yongpay.top

================================================================================
来源：http://jvh.quarkkingdee.top

S. C / C++ 专题
来源：http://yfn.dashuyun.cn

================================================================================
来源：http://vyt.zdqjudy.top

[S01] C：Hello World
来源：http://usc.shuidangran.top

#include <stdio.h>
来源：http://fed.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ngb.fktsv.cn

[S02] C：变量与格式化输出
来源：http://tex.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://ksv.hnqzz.top

[S03] C：读入整数
来源：http://phm.hnqzz.top

int x; scanf("%d", &x);
来源：http://yas.cheryme.top

[S04] C：字符串复制
来源：http://ojh.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bfk.yj20258.top

[S05] C：字符串长度
来源：http://jaf.ctjpmb.com

strlen(s)
来源：http://ntb.havefunace.top

[S06] C：字符串比较
来源：http://eot.gzhubu.top

strcmp(a, b) == 0
来源：http://laz.meibo888.top

[S07] C：数组遍历求和
来源：http://sij.jinqigfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jbo.cashguo.top

[S08] C：动态内存分配与释放
来源：http://qmu.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hoy.gaohongyu789.top

[S09] C：结构体定义与初始化
来源：http://gmq.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tec.zdbjq.cn

[S10] C：指针与解引用
来源：http://kem.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://pao.pengpengdd.cyou

[S11] C：逐行读文件
来源：http://zuo.vehdjk.com

FILE *f = fopen("a.txt", "r");
来源：http://kej.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xto.xingfuxueyuan.xyz

fclose(f);
来源：http://drq.bbcook.cn

[S12] C：写文件
来源：http://wit.ehwqpu.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zqh.ybcxt.top

[S13] C：宏定义
来源：http://kyc.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://icq.shanyushiyangtech.top

[S14] C：枚举
来源：http://axg.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://hbj.bjfxy.top

[S15] C：类型转换
来源：http://ocf.xuetiantiany.cn

(double) a / b
来源：http://phc.fzhhl.top

[S16] C：位操作置位
来源：http://myx.dashuyun.cn

x |= (1 << 3);
来源：http://shf.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://hfv.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qug.zhengqikj.top

[S18] C：命令行参数
来源：http://dof.zdbjq.cn

int main(int argc, char **argv)
来源：http://pse.sweek.top

[S19] C：快速排序
来源：http://rrw.svipenyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yak.aibaodan.cn

[S20] C：二分查找
来源：http://dfs.nanxinkj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://smb.yangfankeji.com

[S21] C：字符类别判断
来源：http://koa.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fcr.vqdsnc.cn

[S22] C：字符串转数字
来源：http://jry.mhx1999.top

atoi("42");  strtod("3.14", NULL);
来源：http://oax.dashuyun.cn

[S23] C：随机数
来源：http://jpa.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bch.sweek.top

[S24] C：获取本地时间
来源：http://uxd.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ogs.wangdashe.top

[S25] C：内存拷贝
来源：http://tem.zycfv.cn

memcpy(dst, src, n);
来源：http://sry.zycfv.cn

[S26] C：内存清零
来源：http://cii.vqdsnc.cn

memset(a, 0, sizeof a);
来源：http://efw.hfpthk.cn

[S27] C：定义常量
来源：http://zgf.pycfn.com

const double PI = 3.14159;
来源：http://djz.meibo888.top

[S28] C：静态变量
来源：http://hex.zycfv.cn

static int counter = 0;
来源：http://oxp.yangfankeji.com

[S29] C：变参函数
来源：http://uyu.hammf.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vbi.hysaishi.cn

[S30] C：头文件保护
来源：http://wod.zhiwuduotai.top

#ifndef X_H
来源：http://rse.jqgfzy.top

#define X_H
来源：http://amm.ydzc1.top

#endif
来源：http://arc.shzxlz.cn

[S31] C++：Hello World
来源：http://cwr.jinqigufen.top

#include <iostream>
来源：http://baw.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://lnq.xuanzx.com

[S32] C++：字符串
来源：http://xdu.tian-w.cn

std::string s = "hi";  s += "!";
来源：http://tad.0kj1m.cn

[S33] C++：vector 增删
来源：http://pfk.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://igl.dashuyun.cn

[S34] C++：遍历 vector
来源：http://egg.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://hqc.wangdashe.top

[S35] C++：map
来源：http://wgk.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xzn.c1oappe.top

[S36] C++：unordered_map
来源：http://uke.sysykeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zxc.aibaodan.cn

[S37] C++：set
来源：http://kcu.yj202588.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mzc.shuidangran.top

[S38] C++：排序
来源：http://kvm.xinyue.icu

std::sort(v.begin(), v.end());
来源：http://pmt.aizwys.cn

[S39] C++：自定义比较器排序
来源：http://mml.fengsongda.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uyw.havefunace.top

[S40] C++：查找元素
来源：http://fvo.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hif.mhx1999.top

[S41] C++：类与构造函数
来源：http://yxx.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fpe.xziqi.cn

[S42] C++：继承与虚函数
来源：http://ekx.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://fzh.ywan-chungtsiang.top

[S43] C++：智能指针
来源：http://uga.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://rwe.cdnleiting.top

[S44] C++：引用传参
来源：http://rqy.ehwqpu.com

void inc(int &x) { ++x; }
来源：http://ehl.ivvv.top

[S45] C++：lambda
来源：http://nvd.quarkkingdee.top

auto add = [](int a, int b) { return a + b; };
来源：http://ple.shuidangran.top

[S46] C++：函数模板
来源：http://hjx.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ram.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://xuh.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sgb.yj202588.top

[S48] C++：逐行读文件
来源：http://cwt.mhx1999.top

std::ifstream in("a.txt");  std::string line;
来源：http://knf.mhx1999.top

while (std::getline(in, line)) { }
来源：http://xah.fktsv.cn

[S49] C++：写文件
来源：http://zor.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zzs.xylfe.cn

[S50] C++：格式化数字
来源：http://ejn.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jvk.xingfuxueyuan.xyz

[S51] C++：显式类型转换
来源：http://ghb.jinqigfzy.top

static_cast<double>(a) / b
来源：http://fae.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://vfb.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://hfl.guowangkeji.top

[S53] C++：移动语义
来源：http://wbb.ydjk.org.cn

std::vector<int> w = std::move(v);
来源：http://zem.sufxvd.cn

[S54] C++：异常处理
来源：http://mni.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nzj.yj20258.top

[S55] C++：结构化绑定
来源：http://nte.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vmp.hywenlv.cn

[S56] C++：optional
来源：http://hok.ivvv.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pgz.shzxlz.cn

[S57] C++：编译期常量
来源：http://kur.shzxlz.cn

constexpr int N = 10;
来源：http://mzb.gotoacloud.top

[S58] C++：命名空间
来源：http://era.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://efr.uphjek.com

[S59] C++：静态断言
来源：http://tts.cheryme.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mgm.jinqigfzy.top

[S60] C++：遍历并删除元素
来源：http://myi.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://std.jinghuilouyu.cn

================================================================================
来源：http://umi.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hfz.9152youxi.cn

================================================================================
来源：http://hvi.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://vej.chenjidiqi.icu

println("Hello")
来源：http://ovp.shzxlz.cn

[T02] Kotlin：变量
来源：http://jka.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://syf.tanke756.top

[T03] Kotlin：字符串模板
来源：http://soe.quarkkingdee.top

"值: $b"
来源：http://jzi.yongpay.top

[T04] Kotlin：空安全
来源：http://qtz.cdnleiting.top

val n: String? = null;  n?.length
来源：http://uji.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://hxs.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iwh.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://ato.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iql.haohaochexian.top

[T07] Kotlin：集合过滤
来源：http://ssd.jianghu66.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vvo.cashguo.top

[T08] Kotlin：数据类
来源：http://jgc.hysaishi.cn

data class User(val name: String, val age: Int)
来源：http://hne.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://ulm.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://lse.yfazqb.com

[T10] Kotlin：默认参数
来源：http://xpa.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rir.c1oappe.top

[T11] Kotlin：协程
来源：http://kxc.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ilu.zdbjq.cn

[T12] Kotlin：解构声明
来源：http://bur.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://jer.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://tao.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://mbe.chenzaomai.com

[T14] Kotlin：循环
来源：http://vks.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://fkf.52xcode.cn

[T15] Kotlin：接口
来源：http://cuk.hfpthk.cn

interface Shape { fun area(): Double }
来源：http://kdy.ybcxt.top

[T16] Swift：Hello World
来源：http://daa.xylfe.cn

print("Hello")
来源：http://byd.haohaochexian.top

[T17] Swift：变量与常量
来源：http://lza.quarkkingdee.top

var a = 1;  let b = 2
来源：http://eqj.fzhhl.top

[T18] Swift：字符串插值
来源：http://avl.kuanghao11.cn

"值: \(b)"
来源：http://jxy.xuanzx.com

[T19] Swift：可选绑定
来源：http://btt.yueranfly.top

if let n = opt { print(n) }
来源：http://mrm.zdbjq.cn

[T20] Swift：数组操作
来源：http://ete.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://psg.zhijiandao.cn

[T21] Swift：遍历
来源：http://xaf.gotoacloud.top

for x in a { print(x) }
来源：http://xhv.ehwqpu.com

[T22] Swift：字典
来源：http://qit.zhoulong.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://xdl.jinqigufen.top

[T23] Swift：函数
来源：http://vmv.vqdsnc.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hkn.yj20258.top

[T24] Swift：闭包
来源：http://ksh.feifeiyinyue.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://boj.yongpay.top

[T25] Swift：结构体
来源：http://mcx.vehdjk.com

struct P { var x: Int }
来源：http://fdb.snrcjt.cn

[T26] Swift：类与重写
来源：http://wve.yueranfly.top

class A: Base { override func f() {} }
来源：http://hdv.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://ugi.havefunace.top

do { try f() } catch { print(error) }
来源：http://lff.xingfuxueyuan.xyz

[T28] Swift：枚举
来源：http://umm.wangdashe.top

enum Color { case red, green }
来源：http://dva.dianchejie.cn

[T29] Swift：guard 提前返回
来源：http://tyy.yj20258.top

guard let x = opt else { return }
来源：http://utb.fzhhl.top

[T30] Swift：协议
来源：http://zlt.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://hdg.xingfuxueyuan.xyz

[T31] Lua：Hello World
来源：http://acp.hammf.cn

print("Hello")
来源：http://onn.zhongyouzk.top

[T32] Lua：局部变量
来源：http://rwz.dashuyun.cn

local a = 1
来源：http://rqe.sysykeji.top

[T33] Lua：表（数组）
来源：http://xbx.dianchejie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yji.shzxlz.cn

[T34] Lua：遍历表
来源：http://ehy.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rda.c1oappe.top

[T35] Lua：字典表
来源：http://sgz.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://hbo.fanxiaobao.xyz

[T36] Lua：函数
来源：http://iob.guannengcc.top

function add(a, b) return a + b end
来源：http://scu.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://uwj.kuanghao11.cn

"a" .. "b"
来源：http://qit.ywan-chungtsiang.top

[T38] Lua：条件
来源：http://djk.zdbjq.cn

if x > 0 then print("正") end
来源：http://oaq.xuanzx.com

[T39] Lua：模式匹配
来源：http://iaz.xuanzx.com

string.find(s, "%d+")
来源：http://nax.sysykeji.top

[T40] Lua：元表
来源：http://zru.xuanzx.com

setmetatable({}, { __index = base })
来源：http://thn.zhiwuduotai.top

[T41] Perl：Hello World
来源：http://ipr.epnwcf.com

print "Hello\n";
来源：http://rjy.gzhubu.top

[T42] Perl：变量类型
来源：http://hhu.xylfe.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jwl.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://osq.yonumen.top

"值: $a"
来源：http://chj.sweek.top

[T44] Perl：条件
来源：http://eio.meibo888.top

if ($a > 0) { print "正"; }
来源：http://hng.ywan-chungtsiang.top

[T45] Perl：数组遍历
来源：http://ttk.sweek.top

for my $x (@arr) { print $x; }
来源：http://mqr.zdqjudy.top

[T46] Perl：哈希操作
来源：http://bty.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fws.zhiwuduotai.top

[T47] Perl：正则捕获
来源：http://tpe.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kwf.mhx1999.top

[T48] Perl：正则替换
来源：http://wls.epnwcf.com

$s =~ s/old/new/g;
来源：http://qzx.gotoacloud.top

[T49] Perl：函数
来源：http://qix.yvedp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kwm.hysaishi.cn

[T50] Perl：逐行读文件
来源：http://klg.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zgq.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://fje.zhiwuduotai.top

[T51] Scala：Hello World
来源：http://cmo.0kj1m.cn

println("Hello")
来源：http://qat.zhiwuduotai.top

[T52] Scala：变量
来源：http://wpr.jyoumei.cn


<!-- 参考信息 -->