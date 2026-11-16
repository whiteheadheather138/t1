代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://ajd.vehdjk.com

[R48] awk 取指定列
来源：http://fou.redwolf501.top

awk '{print $1, $3}' a.txt
来源：http://nap.tian-w.cn

[R49] awk 带条件
来源：http://wzb.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://epg.pengpengdd.cyou

[R50] awk 求和
来源：http://gwp.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dnf.snrcjt.cn

[R51] 排序去重取前几
来源：http://iji.ywan-chungtsiang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qbu.cucudq.cn

[R52] 统计行数
来源：http://pjo.wangdashe.top

wc -l a.txt
来源：http://pyn.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://jey.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jzv.shzxlz.cn

[R54] 比较两个文件
来源：http://uoj.tian-w.cn

diff a.txt b.txt
来源：http://aua.sysykeji.top

[R55] 压缩与解压
来源：http://rej.zdqjudy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ekk.jinyuanbaomall.cn

[R56] 远程拷贝
来源：http://efh.svipenyu.cn

scp file user@host:/path/
来源：http://kwn.fengsongda.top

[R57] 远程执行命令
来源：http://kmd.jqgufenzy.top

ssh user@host 'uptime'
来源：http://qho.zhixingplan.top

[R58] 下载文件
来源：http://mna.uphjek.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uzm.yj20258.top

[R59] 发 POST JSON
来源：http://oui.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jdb.fzhhl.top

[R60] 只看 HTTP 状态码
来源：http://das.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://odd.gotoacloud.top

[R61] 磁盘占用
来源：http://cwf.sysykeji.top

df -h;  du -sh *
来源：http://mja.tarul.cn

[R62] 找最占空间的文件
来源：http://mka.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://tfz.pycfn.com

[R63] 内存与进程
来源：http://uaa.meibo888.top

free -h;  ps aux | grep nginx
来源：http://zld.vqdsnc.cn

[R64] 结束进程
来源：http://rxz.ydjk.org.cn

kill -9 $(pgrep -f app.py)
来源：http://wek.jinqigufen.top

[R65] 查看端口占用
来源：http://afa.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wtd.ydzc1.top

[R66] 定时任务
来源：http://fsd.sufxvd.cn

crontab -e;  crontab -l
来源：http://cqm.sweek.top

[R67] 生成随机十六进制串
来源：http://sfo.cheryme.top

openssl rand -hex 16
来源：http://nze.yanxiufei.cn

[R68] 计算文件校验值
来源：http://xma.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://xen.vqdsnc.cn

[R69] 生成随机密码
来源：http://ymq.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://wvs.jlsjyb.cn

[R70] 时间戳与互转
来源：http://mvv.316326.xyz

date +%s;  date -d @1700000000
来源：http://gey.andypj.xyz

[R71] 日期格式化
来源：http://wts.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gsk.aibaodan.cn

[R72] 等待端口就绪
来源：http://kns.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://kth.aibaodan.cn

[R73] 分割大日志
来源：http://lwv.cdnleiting.top

split -l 1000 big.log part_
来源：http://lby.jyoumei.cn

[R74] 批量重命名
来源：http://sdd.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pxm.fzhhl.top

[R75] 导出环境变量
来源：http://kmi.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://ysb.aibaodan.cn

[R76] 使用临时文件
来源：http://yux.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://czp.cashguo.top

[R77] 读取用户输入
来源：http://vas.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://ngu.sjlbkw.cn

[R78] 交互式菜单
来源：http://cne.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://rzg.vehdjk.com

[R79] 解析命令行选项
来源：http://iaz.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pnl.jinyuanbaomall.cn

[R80] 查看脚本执行耗时
来源：http://egk.quarkkingdee.top

time ./run.sh
来源：http://cft.andypj.xyz

================================================================================
来源：http://yia.ybcxt.top

S. C / C++ 专题
来源：http://hcx.9152youxi.cn

================================================================================
来源：http://pnk.fzhhl.top

[S01] C：Hello World
来源：http://zjm.gogol.net.cn

#include <stdio.h>
来源：http://kqj.wangshuangyany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ebp.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://itu.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://yrx.birdmap.top

[S03] C：读入整数
来源：http://fzp.daria6918.cn

int x; scanf("%d", &x);
来源：http://lsc.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://xhj.shanyushiyangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://wxu.redwolf501.top

[S05] C：字符串长度
来源：http://kzp.ivvv.top

strlen(s)
来源：http://gtu.sjlbkw.cn

[S06] C：字符串比较
来源：http://eyu.bbcook.cn

strcmp(a, b) == 0
来源：http://faj.fengsongda.top

[S07] C：数组遍历求和
来源：http://tni.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://naf.feifeiyinyue.top

[S08] C：动态内存分配与释放
来源：http://lzd.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oph.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://its.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cyr.hammf.cn

[S10] C：指针与解引用
来源：http://nlu.52xcode.cn

int *p = &a;  *p = 5;
来源：http://vfz.jqgufenzy.top

[S11] C：逐行读文件
来源：http://fwe.tarul.cn

FILE *f = fopen("a.txt", "r");
来源：http://cpl.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nzt.epnwcf.com

fclose(f);
来源：http://bdv.wangshuangyany.cn

[S12] C：写文件
来源：http://hzr.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xcd.ehwqpu.com

[S13] C：宏定义
来源：http://okq.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uku.meibo888.top

[S14] C：枚举
来源：http://ofu.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://zwa.gogol.net.cn

[S15] C：类型转换
来源：http://mnu.cheryme.top

(double) a / b
来源：http://ruo.vehdjk.com

[S16] C：位操作置位
来源：http://ekh.sweek.top

x |= (1 << 3);
来源：http://klm.cdnleiting.top

[S17] C：安全拼接字符串
来源：http://bkg.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ypp.ydjk.org.cn

[S18] C：命令行参数
来源：http://ywg.yfazqb.com

int main(int argc, char **argv)
来源：http://qbb.cheryme.top

[S19] C：快速排序
来源：http://nzh.sjlbkw.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mjr.gzhubu.top

[S20] C：二分查找
来源：http://ujg.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://drn.nwbrower.top

[S21] C：字符类别判断
来源：http://sat.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cqt.9152youxi.cn

[S22] C：字符串转数字
来源：http://uok.jlsjyb.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xcc.tian-w.cn

[S23] C：随机数
来源：http://hms.zhoulong.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://dmu.cqqwz.cn

[S24] C：获取本地时间
来源：http://qyd.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dse.xuanzx.com

[S25] C：内存拷贝
来源：http://ksd.vqdsnc.cn

memcpy(dst, src, n);
来源：http://ern.xinyue.icu

[S26] C：内存清零
来源：http://aer.hesvh.cn

memset(a, 0, sizeof a);
来源：http://xro.ppjwa.cn

[S27] C：定义常量
来源：http://pam.kuanghao11.cn

const double PI = 3.14159;
来源：http://iai.shanyushiyangtech.top

[S28] C：静态变量
来源：http://apy.shuidangran.top

static int counter = 0;
来源：http://lul.hysaishi.cn

[S29] C：变参函数
来源：http://ytz.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tbt.sweek.top

[S30] C：头文件保护
来源：http://tsi.daxiang520.top

#ifndef X_H
来源：http://kgd.hcnkem.com

#define X_H
来源：http://pgm.andypj.xyz

#endif
来源：http://khb.haohaochexian.top

[S31] C++：Hello World
来源：http://vpi.hfpthk.cn

#include <iostream>
来源：http://pyz.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://fnv.zhoulong.xyz

[S32] C++：字符串
来源：http://yne.ybcxt.top

std::string s = "hi";  s += "!";
来源：http://jfm.chenlongwang.top

[S33] C++：vector 增删
来源：http://bds.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://flq.yuanzhike.top

[S34] C++：遍历 vector
来源：http://fxq.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://cyr.chenjidiqi.icu

[S35] C++：map
来源：http://qpz.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xwz.havefunace.top

[S36] C++：unordered_map
来源：http://tst.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ldk.bjfxy.top

[S37] C++：set
来源：http://suu.yvedp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bkx.tianlin.xyz

[S38] C++：排序
来源：http://lps.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://gdq.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://hqj.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cwg.zhoulong.xyz

[S40] C++：查找元素
来源：http://vkr.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://syq.chenzaomai.com

[S41] C++：类与构造函数
来源：http://gwt.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hxw.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://imb.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://jun.wangdashe.top

[S43] C++：智能指针
来源：http://ptw.0kj1m.cn

auto p = std::make_unique<int>(5);
来源：http://qkv.birdmap.top

[S44] C++：引用传参
来源：http://wxt.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://xai.sysykeji.top

[S45] C++：lambda
来源：http://sln.hfpthk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qyk.pycfn.com

[S46] C++：函数模板
来源：http://xjz.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wzr.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://zrl.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://olz.9152youxi.cn

[S48] C++：逐行读文件
来源：http://scz.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://eje.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://mvt.zhijiandao.cn

[S49] C++：写文件
来源：http://mqh.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://con.gzhubu.top

[S50] C++：格式化数字
来源：http://aty.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bms.xingfuxueyuan.xyz

[S51] C++：显式类型转换
来源：http://kyd.cheryme.top

static_cast<double>(a) / b
来源：http://wkq.birdmap.top

[S52] C++：const 与 noexcept
来源：http://vug.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://iik.wangshuangyany.cn

[S53] C++：移动语义
来源：http://naa.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://bay.tanke756.top

[S54] C++：异常处理
来源：http://xwq.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://asu.andypj.xyz

[S55] C++：结构化绑定
来源：http://epj.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kqm.aizwys.cn

[S56] C++：optional
来源：http://nat.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zkb.sxryk.cn

[S57] C++：编译期常量
来源：http://kzs.guowangkeji.top

constexpr int N = 10;
来源：http://ikr.xuanzx.com

[S58] C++：命名空间
来源：http://epa.yj202588.top

namespace ns { int f() { return 1; } }
来源：http://lxy.chenzaomai.com

[S59] C++：静态断言
来源：http://atv.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xwp.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://ynt.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dyw.shanyushiyangkeji.top

================================================================================
来源：http://xnn.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rjy.cqqwz.cn

================================================================================
来源：http://yhn.gaohongyu789.top

[T01] Kotlin：Hello World
来源：http://huu.sjlbkw.cn

println("Hello")
来源：http://anf.dianchejie.cn

[T02] Kotlin：变量
来源：http://qtp.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mey.zhongyouzk.top

[T03] Kotlin：字符串模板
来源：http://xgk.zycfv.cn

"值: $b"
来源：http://kwq.ydzc1.top

[T04] Kotlin：空安全
来源：http://mdd.yangfankeji.com

val n: String? = null;  n?.length
来源：http://jec.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://ayk.wangdashe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ugg.yonumen.top

[T06] Kotlin：集合映射
来源：http://plo.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ivo.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://llg.gotoacloud.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tae.ehwqpu.com

[T08] Kotlin：数据类
来源：http://zfr.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://oeh.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://kcl.cdnleiting.top

fun String.exclaim() = this + "!"
来源：http://svx.andypj.xyz

[T10] Kotlin：默认参数
来源：http://xlc.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cgf.guannengcc.top

[T11] Kotlin：协程
来源：http://xok.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uyz.cdnleiting.top

[T12] Kotlin：解构声明
来源：http://ntz.xinyue.icu

val (a, b) = Pair(1, 2)
来源：http://qxa.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://jep.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://nrx.quarkkingdee.top

[T14] Kotlin：循环
来源：http://hts.xuanzx.com

for (i in 1..10) println(i)
来源：http://uud.ydjk.org.cn

[T15] Kotlin：接口
来源：http://mcu.zhaomingkeji.xyz

interface Shape { fun area(): Double }
来源：http://pye.gotoacloud.top

[T16] Swift：Hello World
来源：http://sod.hysaishi.cn

print("Hello")
来源：http://jgo.ctjpmb.com

[T17] Swift：变量与常量
来源：http://vje.epnwcf.com

var a = 1;  let b = 2
来源：http://myd.gogol.net.cn

[T18] Swift：字符串插值
来源：http://ycv.birdmap.top

"值: \(b)"
来源：http://zuw.ppjwa.cn

[T19] Swift：可选绑定
来源：http://hql.yj20258.top

if let n = opt { print(n) }
来源：http://niw.yj20258888.top

[T20] Swift：数组操作
来源：http://wdl.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://vif.ywan-chungtsiang.top

[T21] Swift：遍历
来源：http://nwf.hfpthk.cn

for x in a { print(x) }
来源：http://ldf.fengsongda.top

[T22] Swift：字典
来源：http://dsj.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cyh.hesvh.cn

[T23] Swift：函数
来源：http://sei.yuxming.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://syq.pengpengdd.cyou

[T24] Swift：闭包
来源：http://pdf.yfazqb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://jjl.hfpthk.cn

[T25] Swift：结构体
来源：http://fcz.chenlongwang.top

struct P { var x: Int }
来源：http://ckj.dianchejie.cn

[T26] Swift：类与重写
来源：http://qvh.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://roz.daria6918.cn

[T27] Swift：错误处理
来源：http://uft.havefunace.top

do { try f() } catch { print(error) }
来源：http://bty.sxryk.cn

[T28] Swift：枚举
来源：http://shv.sxryk.cn

enum Color { case red, green }
来源：http://jlj.yongpay.top

[T29] Swift：guard 提前返回
来源：http://jer.vqdsnc.cn

guard let x = opt else { return }
来源：http://qfr.hywenlv.cn

[T30] Swift：协议
来源：http://zmu.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://cmw.fehbvm.com

[T31] Lua：Hello World
来源：http://xrz.redwolf501.top

print("Hello")
来源：http://hdf.redwolf501.top

[T32] Lua：局部变量
来源：http://fah.jyoumei.cn

local a = 1
来源：http://ifh.tian-w.cn

[T33] Lua：表（数组）
来源：http://exj.fanxiaobao.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://lmi.nanxinkj.top

[T34] Lua：遍历表
来源：http://dcb.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://knf.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://hzy.sxryk.cn

local d = { a = 1 };  d.b = 2
来源：http://onv.gaohongyu789.top

[T36] Lua：函数
来源：http://rne.chenlongwang.top

function add(a, b) return a + b end
来源：http://hly.ybcxt.top

[T37] Lua：字符串拼接
来源：http://hdd.hnqzz.top

"a" .. "b"
来源：http://vda.ivvv.top

[T38] Lua：条件
来源：http://fan.zhongyouzk.top

if x > 0 then print("正") end
来源：http://mim.jinqigufen.top

[T39] Lua：模式匹配
来源：http://flr.0kj1m.cn

string.find(s, "%d+")
来源：http://ubr.hywenlv.cn

[T40] Lua：元表
来源：http://zsl.xziqi.cn

setmetatable({}, { __index = base })
来源：http://wjn.yj20258888.top

[T41] Perl：Hello World
来源：http://nca.tianlin.xyz

print "Hello\n";
来源：http://xhv.yuxming.cn

[T42] Perl：变量类型
来源：http://mve.shuidangran.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bqi.chenzaomai.com

[T43] Perl：字符串插值
来源：http://ran.nanxuanxn.top

"值: $a"
来源：http://iiy.jqgfzy.top

[T44] Perl：条件
来源：http://dkw.hcnkem.com

if ($a > 0) { print "正"; }
来源：http://xgj.guowangkeji.top

[T45] Perl：数组遍历
来源：http://ejq.ctjpmb.com

for my $x (@arr) { print $x; }
来源：http://qxc.epnwcf.com

[T46] Perl：哈希操作
来源：http://tgm.hywenlv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jqo.hfpthk.cn

[T47] Perl：正则捕获
来源：http://gul.feifeiyinyue.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://onp.gaohongyu789.top

[T48] Perl：正则替换
来源：http://qtt.jlsjyb.cn

$s =~ s/old/new/g;
来源：http://lpd.jiagoushi.top

[T49] Perl：函数
来源：http://rpr.sysykeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://luo.ybcxt.top

[T50] Perl：逐行读文件
来源：http://rml.yj20258888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rki.haohaochexian.top


<!-- 参考信息 -->