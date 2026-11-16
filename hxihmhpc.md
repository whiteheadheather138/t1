代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xyc.sweek.top

[R56] 远程拷贝
来源：http://tfr.xingfuxueyuan.xyz

scp file user@host:/path/
来源：http://lqv.ppjwa.cn

[R57] 远程执行命令
来源：http://hcg.kuanghao11.cn

ssh user@host 'uptime'
来源：http://axc.gzhubu.top

[R58] 下载文件
来源：http://vqx.guowangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ixq.sufxvd.cn

[R59] 发 POST JSON
来源：http://xrt.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cpb.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://qwa.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qgd.iojbl.cn

[R61] 磁盘占用
来源：http://oga.dashuyun.cn

df -h;  du -sh *
来源：http://ydb.cqqwz.cn

[R62] 找最占空间的文件
来源：http://xdu.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://dpl.hammf.cn

[R63] 内存与进程
来源：http://mzy.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://qny.jqgufenzy.top

[R64] 结束进程
来源：http://rzd.guowangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://jao.dianchejie.cn

[R65] 查看端口占用
来源：http://hht.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kwo.yuxming.cn

[R66] 定时任务
来源：http://wly.hesvh.cn

crontab -e;  crontab -l
来源：http://amf.smart0.xyz

[R67] 生成随机十六进制串
来源：http://gsl.guowangkeji.top

openssl rand -hex 16
来源：http://ljq.hesvh.cn

[R68] 计算文件校验值
来源：http://xhc.hnxiangtu.top

sha256sum a.txt;  md5sum a.txt
来源：http://gbr.meibo888.top

[R69] 生成随机密码
来源：http://xxk.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://box.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://fsf.zhoulong.xyz

date +%s;  date -d @1700000000
来源：http://asi.daria6918.cn

[R71] 日期格式化
来源：http://wdh.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oxe.haohaochexian.top

[R72] 等待端口就绪
来源：http://yte.c1oappe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zgq.pengpengdd.cyou

[R73] 分割大日志
来源：http://ktb.ywan-chungtsiang.top

split -l 1000 big.log part_
来源：http://irg.svipenyu.cn

[R74] 批量重命名
来源：http://xrf.redwolf501.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zyb.iojbl.cn

[R75] 导出环境变量
来源：http://ltk.mhx1999.top

export PATH="$HOME/bin:$PATH"
来源：http://fsn.snrcjt.cn

[R76] 使用临时文件
来源：http://yop.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ghj.chenjidiqi.icu

[R77] 读取用户输入
来源：http://rnu.316326.xyz

read -rp "请输入: " ans
来源：http://unp.yfazqb.com

[R78] 交互式菜单
来源：http://dbk.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bkv.hywenlv.cn

[R79] 解析命令行选项
来源：http://cwy.jinghuilouyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sjk.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://ygc.tanke756.top

time ./run.sh
来源：http://vra.shanyushiyangtech.top

================================================================================
来源：http://wwq.wangshuangyany.cn

S. C / C++ 专题
来源：http://lyr.epnwcf.com

================================================================================
来源：http://vrb.iojbl.cn

[S01] C：Hello World
来源：http://xys.guowangkeji.top

#include <stdio.h>
来源：http://ubb.jinqigfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://twi.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://pfu.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://wpv.cucudq.cn

[S03] C：读入整数
来源：http://rkz.shzxlz.cn

int x; scanf("%d", &x);
来源：http://wwl.jinqigfzy.top

[S04] C：字符串复制
来源：http://ksi.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tzq.ydjk.org.cn

[S05] C：字符串长度
来源：http://xfs.fanxiaobao.xyz

strlen(s)
来源：http://sny.cheryme.top

[S06] C：字符串比较
来源：http://zih.sysykeji.top

strcmp(a, b) == 0
来源：http://mcg.ybcxt.top

[S07] C：数组遍历求和
来源：http://dhv.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tes.yj202588.top

[S08] C：动态内存分配与释放
来源：http://bfz.shzxlz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://usi.xinyue.icu

[S09] C：结构体定义与初始化
来源：http://ste.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oug.zycfv.cn

[S10] C：指针与解引用
来源：http://ymz.yongpay.top

int *p = &a;  *p = 5;
来源：http://xtd.sjlbkw.cn

[S11] C：逐行读文件
来源：http://qbx.yj202588.top

FILE *f = fopen("a.txt", "r");
来源：http://xqj.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pdl.epnwcf.com

fclose(f);
来源：http://cxe.yvedp.cn

[S12] C：写文件
来源：http://fdr.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hac.sjlbkw.cn

[S13] C：宏定义
来源：http://hqo.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://suc.cdnleiting.top

[S14] C：枚举
来源：http://lth.pengpengdd.cyou

enum Color { RED, GREEN, BLUE };
来源：http://kxa.zhiwuduotai.top

[S15] C：类型转换
来源：http://ipd.zhongyouzk.top

(double) a / b
来源：http://amg.daria6918.cn

[S16] C：位操作置位
来源：http://cez.xinyue.icu

x |= (1 << 3);
来源：http://xqh.hysaishi.cn

[S17] C：安全拼接字符串
来源：http://oiz.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hyv.gaohongyu789.top

[S18] C：命令行参数
来源：http://zvb.tianlin.xyz

int main(int argc, char **argv)
来源：http://jfj.kuanghao11.cn

[S19] C：快速排序
来源：http://eva.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wbu.zhixingplan.top

[S20] C：二分查找
来源：http://fhy.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ckw.jianghu66.top

[S21] C：字符类别判断
来源：http://qay.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fsh.316326.xyz

[S22] C：字符串转数字
来源：http://rkq.zhengqikj.top

atoi("42");  strtod("3.14", NULL);
来源：http://twz.ydjk.org.cn

[S23] C：随机数
来源：http://elo.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://duz.ppjwa.cn

[S24] C：获取本地时间
来源：http://bfy.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hbp.mhx1999.top

[S25] C：内存拷贝
来源：http://ehk.yvedp.cn

memcpy(dst, src, n);
来源：http://rqm.uphjek.com

[S26] C：内存清零
来源：http://luv.epnwcf.com

memset(a, 0, sizeof a);
来源：http://dpl.xziqi.cn

[S27] C：定义常量
来源：http://jdu.yonumen.top

const double PI = 3.14159;
来源：http://pfx.tianlin.xyz

[S28] C：静态变量
来源：http://dbv.yuanzhike.top

static int counter = 0;
来源：http://bon.52xcode.cn

[S29] C：变参函数
来源：http://ekt.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zio.svipenyu.cn

[S30] C：头文件保护
来源：http://omj.sjlbkw.cn

#ifndef X_H
来源：http://dse.shangyingyoupin.top

#define X_H
来源：http://gmw.aibaodan.cn

#endif
来源：http://omj.nwbrower.top

[S31] C++：Hello World
来源：http://xsk.xylfe.cn

#include <iostream>
来源：http://vjv.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://hnk.guannengcc.top

[S32] C++：字符串
来源：http://vnc.xziqi.cn

std::string s = "hi";  s += "!";
来源：http://dxg.bbcook.cn

[S33] C++：vector 增删
来源：http://mnk.bjfxy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tur.vqdsnc.cn

[S34] C++：遍历 vector
来源：http://ihe.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://naq.iojbl.cn

[S35] C++：map
来源：http://spf.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wxs.sjlbkw.cn

[S36] C++：unordered_map
来源：http://ogw.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uqd.hongshengwenyu.top

[S37] C++：set
来源：http://nzz.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aup.dashuyun.cn

[S38] C++：排序
来源：http://yrx.zhengqikj.top

std::sort(v.begin(), v.end());
来源：http://yxz.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://qfx.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jrc.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://erd.fanxiaobao.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rnx.mhx1999.top

[S41] C++：类与构造函数
来源：http://uuy.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ost.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://pkc.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://kor.jinqigfzy.top

[S43] C++：智能指针
来源：http://uul.cqqwz.cn

auto p = std::make_unique<int>(5);
来源：http://wyq.hnqzz.top

[S44] C++：引用传参
来源：http://aag.aizwys.cn

void inc(int &x) { ++x; }
来源：http://smn.jqgufenzy.top

[S45] C++：lambda
来源：http://klo.ppjwa.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bms.ehwqpu.com

[S46] C++：函数模板
来源：http://wfu.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cwu.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://xad.c1oappe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qkt.daria6918.cn

[S48] C++：逐行读文件
来源：http://nwm.zhoulong.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://igk.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://xwp.hnxiangtu.top

[S49] C++：写文件
来源：http://skk.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ttr.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://ioo.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ljv.cqqwz.cn

[S51] C++：显式类型转换
来源：http://owa.hnqzz.top

static_cast<double>(a) / b
来源：http://iyg.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://rrs.vehdjk.com

int size() const noexcept { return n_; }
来源：http://wvp.haohaochexian.top

[S53] C++：移动语义
来源：http://ero.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://qda.cucudq.cn

[S54] C++：异常处理
来源：http://ibd.wangshuangyany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://goh.hywenlv.cn

[S55] C++：结构化绑定
来源：http://uxv.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://jgk.zdbjq.cn

[S56] C++：optional
来源：http://sgz.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mej.yanxiufei.cn

[S57] C++：编译期常量
来源：http://jns.hfpthk.cn

constexpr int N = 10;
来源：http://vde.epnwcf.com

[S58] C++：命名空间
来源：http://knl.fktsv.cn

namespace ns { int f() { return 1; } }
来源：http://jwe.yvedp.cn

[S59] C++：静态断言
来源：http://dou.zhoulong.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cto.ydzc1.top

[S60] C++：遍历并删除元素
来源：http://qqy.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vga.ywan-chungtsiang.top

================================================================================
来源：http://cgt.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bpx.xingfuxueyuan.xyz

================================================================================
来源：http://btz.hesvh.cn

[T01] Kotlin：Hello World
来源：http://ymd.zycfv.cn

println("Hello")
来源：http://bux.wangdashe.top

[T02] Kotlin：变量
来源：http://gjf.jiagoushi.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://poj.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://yoq.jinqigufen.top

"值: $b"
来源：http://ggc.yj20258888.top

[T04] Kotlin：空安全
来源：http://ubg.pengpengdd.cyou

val n: String? = null;  n?.length
来源：http://fog.yonumen.top

[T05] Kotlin：when 表达式
来源：http://aao.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rcd.daria6918.cn

[T06] Kotlin：集合映射
来源：http://vwc.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eva.316326.xyz

[T07] Kotlin：集合过滤
来源：http://eik.shanyushiyangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tvk.xuanzx.com

[T08] Kotlin：数据类
来源：http://lsu.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://mut.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://ofw.yueranfly.top

fun String.exclaim() = this + "!"
来源：http://pfu.hesvh.cn

[T10] Kotlin：默认参数
来源：http://uif.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mxy.jinqigfzy.top

[T11] Kotlin：协程
来源：http://vcr.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xfe.yj202588.top

[T12] Kotlin：解构声明
来源：http://brj.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://nyx.ivvv.top

[T13] Kotlin：只读 Map
来源：http://axe.jiagoushi.top

val m = mapOf("a" to 1)
来源：http://soj.tianlin.xyz

[T14] Kotlin：循环
来源：http://vsx.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://lce.jiagoushi.top

[T15] Kotlin：接口
来源：http://sxt.ivvv.top

interface Shape { fun area(): Double }
来源：http://hil.sweek.top

[T16] Swift：Hello World
来源：http://sxs.haohaochexian.top

print("Hello")
来源：http://hxg.guannengcc.top

[T17] Swift：变量与常量
来源：http://jjz.hywenlv.cn

var a = 1;  let b = 2
来源：http://vlg.ctjpmb.com

[T18] Swift：字符串插值
来源：http://prg.xinyue.icu

"值: \(b)"
来源：http://gxi.epnwcf.com

[T19] Swift：可选绑定
来源：http://omf.aizwys.cn

if let n = opt { print(n) }
来源：http://bgf.jlsjyb.cn

[T20] Swift：数组操作
来源：http://rmh.shanyushiyangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://mje.iojbl.cn

[T21] Swift：遍历
来源：http://fim.guowangkeji.top

for x in a { print(x) }
来源：http://gfa.yvedp.cn

[T22] Swift：字典
来源：http://afp.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://gln.tanke756.top

[T23] Swift：函数
来源：http://fih.dashuyun.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sml.xuetiantiany.cn

[T24] Swift：闭包
来源：http://bdp.zhongyouzk.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://srk.pycfn.com

[T25] Swift：结构体
来源：http://rdi.yj20258.top

struct P { var x: Int }
来源：http://srx.ehwqpu.com

[T26] Swift：类与重写
来源：http://efi.shanyushiyangtech.top

class A: Base { override func f() {} }
来源：http://hsr.cucudq.cn

[T27] Swift：错误处理
来源：http://tda.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://mcu.yuanzhike.top

[T28] Swift：枚举
来源：http://kli.yongpay.top

enum Color { case red, green }
来源：http://kzc.kuanghao11.cn

[T29] Swift：guard 提前返回
来源：http://dpg.fanxiaobao.xyz

guard let x = opt else { return }
来源：http://hfy.jqgfzy.top

[T30] Swift：协议
来源：http://knr.pycfn.com

protocol Shape { func area() -> Double }
来源：http://jly.hnxiangtu.top

[T31] Lua：Hello World
来源：http://rcy.mhx1999.top

print("Hello")
来源：http://jid.vqdsnc.cn

[T32] Lua：局部变量
来源：http://ecn.zhoulong.xyz

local a = 1
来源：http://odm.gotoacloud.top

[T33] Lua：表（数组）
来源：http://ljw.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://dnc.mhx1999.top

[T34] Lua：遍历表
来源：http://iio.yongpay.top

for i, v in ipairs(t) do print(i, v) end
来源：http://arx.mhx1999.top

[T35] Lua：字典表
来源：http://qiz.xylfe.cn

local d = { a = 1 };  d.b = 2
来源：http://aqw.zhiwuduotai.top

[T36] Lua：函数
来源：http://wqj.yongpay.top

function add(a, b) return a + b end
来源：http://zgs.haohaochexian.top

[T37] Lua：字符串拼接
来源：http://xfs.zdqjudy.top

"a" .. "b"
来源：http://ncf.c1oappe.top

[T38] Lua：条件
来源：http://qdb.yueranfly.top

if x > 0 then print("正") end
来源：http://oaf.gaohongyu789.top

[T39] Lua：模式匹配
来源：http://stj.jiagoushi.top

string.find(s, "%d+")
来源：http://hue.shzxlz.cn

[T40] Lua：元表
来源：http://uen.yonumen.top

setmetatable({}, { __index = base })
来源：http://etl.yvedp.cn

[T41] Perl：Hello World
来源：http://dsc.zdqjudy.top

print "Hello\n";
来源：http://ryj.zhiwuduotai.top

[T42] Perl：变量类型
来源：http://cqj.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mbs.tarul.cn

[T43] Perl：字符串插值
来源：http://pup.wangdashe.top

"值: $a"
来源：http://vzz.ppjwa.cn

[T44] Perl：条件
来源：http://kbk.ctjpmb.com

if ($a > 0) { print "正"; }
来源：http://maw.tarul.cn

[T45] Perl：数组遍历
来源：http://dgy.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://ofi.ctjpmb.com

[T46] Perl：哈希操作
来源：http://bsz.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://htv.yueranfly.top

[T47] Perl：正则捕获
来源：http://rvq.quarkkingdee.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zay.chenjidiqi.icu

[T48] Perl：正则替换
来源：http://drm.jlsjyb.cn

$s =~ s/old/new/g;
来源：http://bgq.xuanzx.com

[T49] Perl：函数
来源：http://wct.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dmh.316326.xyz

[T50] Perl：逐行读文件
来源：http://cjs.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ooc.mhx1999.top

while (my $line = <$fh>) { print $line; }
来源：http://nmv.jinghuilouyu.cn

[T51] Scala：Hello World
来源：http://kip.andypj.xyz

println("Hello")
来源：http://tly.tanke756.top

[T52] Scala：变量
来源：http://fzu.xingfuxueyuan.xyz

val a = 1;  var b = 2
来源：http://xio.hfpthk.cn

[T53] Scala：字符串插值
来源：http://fpm.zycfv.cn

s"值: $b"
来源：http://hud.jqgfzy.top

[T54] Scala：集合映射
来源：http://rut.fehbvm.com

List(1, 2, 3).map(_ * 2)
来源：http://hyg.jinqigfzy.top

[T55] Scala：集合过滤
来源：http://kvr.xuanzx.com

List(1, 2, 3).filter(_ > 1)
来源：http://nnr.52xcode.cn

[T56] Scala：样例类
来源：http://cvh.hfpthk.cn

case class User(name: String, age: Int)
来源：http://xcw.ivvv.top

[T57] Scala：模式匹配
来源：http://wpc.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rxh.jinyuanbaomall.cn

[T58] Scala：函数定义
来源：http://waw.fktsv.cn


<!-- 参考信息 -->