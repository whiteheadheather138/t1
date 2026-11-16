代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://bjc.shuidangran.top

[R52] 统计行数
来源：http://ovk.zhengqikj.top

wc -l a.txt
来源：http://gws.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://dwm.bjfxy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mzx.hongshengwenyu.top

[R54] 比较两个文件
来源：http://fdn.yj20258.top

diff a.txt b.txt
来源：http://ekg.fktsv.cn

[R55] 压缩与解压
来源：http://tfm.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://via.c1oappe.top

[R56] 远程拷贝
来源：http://ynh.zhixingplan.top

scp file user@host:/path/
来源：http://oic.fzhhl.top

[R57] 远程执行命令
来源：http://mkw.jqgfzy.top

ssh user@host 'uptime'
来源：http://bqw.gotoacloud.top

[R58] 下载文件
来源：http://oze.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ckg.fanxiaobao.xyz

[R59] 发 POST JSON
来源：http://ypi.xinyue.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://spy.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://qnn.snrcjt.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ruh.yuxming.cn

[R61] 磁盘占用
来源：http://olr.zhiwuduotai.top

df -h;  du -sh *
来源：http://rvp.yuanzhike.top

[R62] 找最占空间的文件
来源：http://oii.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://sbh.iojbl.cn

[R63] 内存与进程
来源：http://phz.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://dpa.zhengqikj.top

[R64] 结束进程
来源：http://rnl.ydzc1.top

kill -9 $(pgrep -f app.py)
来源：http://gvf.cqqwz.cn

[R65] 查看端口占用
来源：http://wow.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jxy.mhx1999.top

[R66] 定时任务
来源：http://xnm.cheryme.top

crontab -e;  crontab -l
来源：http://pdg.zhoulong.xyz

[R67] 生成随机十六进制串
来源：http://cjd.fktsv.cn

openssl rand -hex 16
来源：http://bnx.xinyue.icu

[R68] 计算文件校验值
来源：http://ttb.zhixingplan.top

sha256sum a.txt;  md5sum a.txt
来源：http://zcb.jinyuanbaomall.cn

[R69] 生成随机密码
来源：http://nqp.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://ejk.chenzaomai.com

[R70] 时间戳与互转
来源：http://rlv.yfazqb.com

date +%s;  date -d @1700000000
来源：http://afq.sysykeji.top

[R71] 日期格式化
来源：http://qzw.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ztt.cucudq.cn

[R72] 等待端口就绪
来源：http://tgx.hywenlv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pek.c1oappe.top

[R73] 分割大日志
来源：http://mtq.jqgufenzy.top

split -l 1000 big.log part_
来源：http://med.vehdjk.com

[R74] 批量重命名
来源：http://zby.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dmc.yuxming.cn

[R75] 导出环境变量
来源：http://mfu.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://ajz.hysaishi.cn

[R76] 使用临时文件
来源：http://aam.hywenlv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://otg.guowangkeji.top

[R77] 读取用户输入
来源：http://mce.chenlongwang.top

read -rp "请输入: " ans
来源：http://ssb.c1oappe.top

[R78] 交互式菜单
来源：http://wkc.zhoulong.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://vpw.uphjek.com

[R79] 解析命令行选项
来源：http://plx.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zte.jyoumei.cn

[R80] 查看脚本执行耗时
来源：http://yma.ydzc1.top

time ./run.sh
来源：http://mjz.svipenyu.cn

================================================================================
来源：http://erq.jinqigfzy.top

S. C / C++ 专题
来源：http://qxt.cashguo.top

================================================================================
来源：http://byx.bjfxy.top

[S01] C：Hello World
来源：http://zfn.yj20258888.top

#include <stdio.h>
来源：http://rkk.aizwys.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gzy.gzhubu.top

[S02] C：变量与格式化输出
来源：http://nna.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://uum.jinqigfzy.top

[S03] C：读入整数
来源：http://gnt.jiagoushi.top

int x; scanf("%d", &x);
来源：http://sfb.tarul.cn

[S04] C：字符串复制
来源：http://xrm.hcnkem.com

char dst[32]; strcpy(dst, "hi");
来源：http://lff.hongshengwenyu.top

[S05] C：字符串长度
来源：http://upv.zhoulong.xyz

strlen(s)
来源：http://jbi.sweek.top

[S06] C：字符串比较
来源：http://npg.xuetiantiany.cn

strcmp(a, b) == 0
来源：http://lup.9152youxi.cn

[S07] C：数组遍历求和
来源：http://bra.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hsh.cdnleiting.top

[S08] C：动态内存分配与释放
来源：http://uiz.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lnu.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://fad.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fta.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://zed.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://qub.fehbvm.com

[S11] C：逐行读文件
来源：http://zkl.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://cxs.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://eqx.zhixingplan.top

fclose(f);
来源：http://zcb.yvedp.cn

[S12] C：写文件
来源：http://bwm.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hiu.xuetiantiany.cn

[S13] C：宏定义
来源：http://uax.jinyuanbaomall.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://flc.sysykeji.top

[S14] C：枚举
来源：http://lvy.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://elg.hesvh.cn

[S15] C：类型转换
来源：http://wfe.nwbrower.top

(double) a / b
来源：http://tgh.birdmap.top

[S16] C：位操作置位
来源：http://zjf.zycfv.cn

x |= (1 << 3);
来源：http://yik.dianchejie.cn

[S17] C：安全拼接字符串
来源：http://kpp.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dpj.xuetiantiany.cn

[S18] C：命令行参数
来源：http://uwd.chenlongwang.top

int main(int argc, char **argv)
来源：http://sdn.ydzc1.top

[S19] C：快速排序
来源：http://snf.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://brp.gogol.net.cn

[S20] C：二分查找
来源：http://zgy.hysaishi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qcw.xylfe.cn

[S21] C：字符类别判断
来源：http://obi.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yur.hesvh.cn

[S22] C：字符串转数字
来源：http://ude.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://sdh.yueranfly.top

[S23] C：随机数
来源：http://tzd.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dbc.tanke756.top

[S24] C：获取本地时间
来源：http://llk.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zvz.uphjek.com

[S25] C：内存拷贝
来源：http://bic.gaohongyu789.top

memcpy(dst, src, n);
来源：http://luy.nwbrower.top

[S26] C：内存清零
来源：http://xpt.cashguo.top

memset(a, 0, sizeof a);
来源：http://mzx.hnqzz.top

[S27] C：定义常量
来源：http://gcq.shzxlz.cn

const double PI = 3.14159;
来源：http://urp.pengpengdd.cyou

[S28] C：静态变量
来源：http://qps.yuxming.cn

static int counter = 0;
来源：http://hfv.c1oappe.top

[S29] C：变参函数
来源：http://abm.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qvt.yj20258888.top

[S30] C：头文件保护
来源：http://pjh.zycfv.cn

#ifndef X_H
来源：http://byx.jlsjyb.cn

#define X_H
来源：http://tbr.shuidangran.top

#endif
来源：http://eih.sxryk.cn

[S31] C++：Hello World
来源：http://bce.snrcjt.cn

#include <iostream>
来源：http://ezl.yj20258.top

int main() { std::cout << "Hello\n"; }
来源：http://qhe.aibaodan.cn

[S32] C++：字符串
来源：http://oav.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://tzt.xuanzx.com

[S33] C++：vector 增删
来源：http://rnt.hesvh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://epg.tian-w.cn

[S34] C++：遍历 vector
来源：http://lkf.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://yce.nwbrower.top

[S35] C++：map
来源：http://smx.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://whl.xinyue.icu

[S36] C++：unordered_map
来源：http://txw.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hxv.xuanzx.com

[S37] C++：set
来源：http://veh.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zlh.zycfv.cn

[S38] C++：排序
来源：http://sos.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://imu.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://ggl.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eui.hywenlv.cn

[S40] C++：查找元素
来源：http://hdr.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hyo.cashguo.top

[S41] C++：类与构造函数
来源：http://kdv.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eiv.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://imv.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://mgf.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://qmh.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://tmy.zhengqikj.top

[S44] C++：引用传参
来源：http://bpc.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://ckg.316326.xyz

[S45] C++：lambda
来源：http://jbg.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://nge.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://vyz.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://afn.hammf.cn

[S47] C++：结构化绑定遍历
来源：http://qad.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bwj.gzhubu.top

[S48] C++：逐行读文件
来源：http://fuz.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://gyg.birdmap.top

while (std::getline(in, line)) { }
来源：http://lyg.shzxlz.cn

[S49] C++：写文件
来源：http://idn.hcnkem.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wly.hongshengwenyu.top

[S50] C++：格式化数字
来源：http://ybj.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dhn.nwbrower.top

[S51] C++：显式类型转换
来源：http://omo.jinqigfzy.top

static_cast<double>(a) / b
来源：http://eov.xingfuxueyuan.xyz

[S52] C++：const 与 noexcept
来源：http://lva.meibo888.top

int size() const noexcept { return n_; }
来源：http://rkv.sweek.top

[S53] C++：移动语义
来源：http://mbp.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://dqj.gogol.net.cn

[S54] C++：异常处理
来源：http://tpg.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ohk.zhoulong.xyz

[S55] C++：结构化绑定
来源：http://unx.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jgd.birdmap.top

[S56] C++：optional
来源：http://xbv.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xcw.hysaishi.cn

[S57] C++：编译期常量
来源：http://xmw.c1oappe.top

constexpr int N = 10;
来源：http://xzx.yuxming.cn

[S58] C++：命名空间
来源：http://wgq.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://nkk.feifeiyinyue.top

[S59] C++：静态断言
来源：http://env.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://udo.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://byd.yj202588.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bgl.mhx1999.top

================================================================================
来源：http://ikv.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lzk.guowangkeji.top

================================================================================
来源：http://hwe.zhaomingkeji.xyz

[T01] Kotlin：Hello World
来源：http://ghz.guowangkeji.top

println("Hello")
来源：http://rpd.sweek.top

[T02] Kotlin：变量
来源：http://uwi.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kcl.yuxming.cn

[T03] Kotlin：字符串模板
来源：http://uhs.52xcode.cn

"值: $b"
来源：http://xml.smart0.xyz

[T04] Kotlin：空安全
来源：http://kdn.shanyushiyangkeji.top

val n: String? = null;  n?.length
来源：http://fjd.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://ppv.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mkw.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://jlk.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://okl.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://onm.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://axd.bbcook.cn

[T08] Kotlin：数据类
来源：http://lte.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://yfv.chenjidiqi.icu

[T09] Kotlin：扩展函数
来源：http://akt.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://aem.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://izl.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://imf.kuanghao11.cn

[T11] Kotlin：协程
来源：http://sis.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://yzq.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://qlh.hcnkem.com

val (a, b) = Pair(1, 2)
来源：http://nrh.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://vrc.xinyue.icu

val m = mapOf("a" to 1)
来源：http://rxa.jinqigufen.top

[T14] Kotlin：循环
来源：http://zzh.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://isq.yuxming.cn

[T15] Kotlin：接口
来源：http://qay.yangfankeji.com

interface Shape { fun area(): Double }
来源：http://hos.quarkkingdee.top

[T16] Swift：Hello World
来源：http://adh.wangshuangyany.cn

print("Hello")
来源：http://yaf.aibaodan.cn

[T17] Swift：变量与常量
来源：http://lro.yj20258888.top

var a = 1;  let b = 2
来源：http://ztb.yfazqb.com

[T18] Swift：字符串插值
来源：http://erf.fzhhl.top

"值: \(b)"
来源：http://edp.tianlin.xyz

[T19] Swift：可选绑定
来源：http://ftv.yvedp.cn

if let n = opt { print(n) }
来源：http://bby.c1oappe.top

[T20] Swift：数组操作
来源：http://gwh.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xei.fktsv.cn

[T21] Swift：遍历
来源：http://erz.tanke756.top

for x in a { print(x) }
来源：http://yhr.zhoulong.xyz

[T22] Swift：字典
来源：http://ulx.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://tao.sjlbkw.cn

[T23] Swift：函数
来源：http://dik.daria6918.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qls.zhengqikj.top

[T24] Swift：闭包
来源：http://nbf.xingfuxueyuan.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://die.jinqigufen.top

[T25] Swift：结构体
来源：http://ntw.cdnleiting.top

struct P { var x: Int }
来源：http://fzt.jqgfzy.top

[T26] Swift：类与重写
来源：http://evr.yuanzhike.top

class A: Base { override func f() {} }
来源：http://zlp.haohaochexian.top

[T27] Swift：错误处理
来源：http://vuj.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://xlm.shuidangran.top

[T28] Swift：枚举
来源：http://csr.smart0.xyz

enum Color { case red, green }
来源：http://mcy.hongshengwenyu.top

[T29] Swift：guard 提前返回
来源：http://bpg.bbcook.cn

guard let x = opt else { return }
来源：http://lif.ctjpmb.com

[T30] Swift：协议
来源：http://ngd.fengsongda.top

protocol Shape { func area() -> Double }
来源：http://mgb.zycfv.cn

[T31] Lua：Hello World
来源：http://ekb.xingfuxueyuan.xyz

print("Hello")
来源：http://zog.shzxlz.cn

[T32] Lua：局部变量
来源：http://vjn.xuetiantiany.cn

local a = 1
来源：http://mcg.smart0.xyz

[T33] Lua：表（数组）
来源：http://fnq.aizwys.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ord.hcnkem.com

[T34] Lua：遍历表
来源：http://bnj.yangfankeji.com

for i, v in ipairs(t) do print(i, v) end
来源：http://dhz.epnwcf.com

[T35] Lua：字典表
来源：http://jmo.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://aqs.zhixingplan.top

[T36] Lua：函数
来源：http://njb.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://svy.cashguo.top

[T37] Lua：字符串拼接
来源：http://buq.ybcxt.top

"a" .. "b"
来源：http://yne.cdnleiting.top

[T38] Lua：条件
来源：http://lzy.shuidangran.top

if x > 0 then print("正") end
来源：http://zgc.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://znv.yanxiufei.cn

string.find(s, "%d+")
来源：http://rqq.wangshuangyany.cn

[T40] Lua：元表
来源：http://mqn.xuanzx.com

setmetatable({}, { __index = base })
来源：http://jnu.jyoumei.cn

[T41] Perl：Hello World
来源：http://jzu.andypj.xyz

print "Hello\n";
来源：http://dgi.meibo888.top

[T42] Perl：变量类型
来源：http://zda.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wki.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://gok.ehwqpu.com

"值: $a"
来源：http://ffv.mhx1999.top

[T44] Perl：条件
来源：http://wvl.ydjk.org.cn

if ($a > 0) { print "正"; }
来源：http://bcu.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://dua.yonumen.top

for my $x (@arr) { print $x; }
来源：http://joq.ehwqpu.com

[T46] Perl：哈希操作
来源：http://gbc.vehdjk.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pwj.chenzaomai.com

[T47] Perl：正则捕获
来源：http://qyv.ybcxt.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ips.chenjidiqi.icu

[T48] Perl：正则替换
来源：http://uvd.jlsjyb.cn

$s =~ s/old/new/g;
来源：http://tlb.cucudq.cn

[T49] Perl：函数
来源：http://bpd.wangshuangyany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://guh.hywenlv.cn

[T50] Perl：逐行读文件
来源：http://zxa.epnwcf.com

open my $fh, "<", "a.txt" or die $!;
来源：http://uuc.fehbvm.com

while (my $line = <$fh>) { print $line; }
来源：http://bsp.zhongyouzk.top

[T51] Scala：Hello World
来源：http://irj.guannengcc.top

println("Hello")
来源：http://puq.yuxming.cn

[T52] Scala：变量
来源：http://bpv.andypj.xyz

val a = 1;  var b = 2
来源：http://zht.bjfxy.top

[T53] Scala：字符串插值
来源：http://mpr.cqqwz.cn

s"值: $b"
来源：http://ylx.daria6918.cn

[T54] Scala：集合映射
来源：http://ofc.sxryk.cn


<!-- 参考信息 -->