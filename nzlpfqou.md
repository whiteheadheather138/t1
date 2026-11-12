代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://dzh.nwbrower.top

[R52] 统计行数
来源：http://hry.shzxlz.cn

wc -l a.txt
来源：http://fnj.tianlin.xyz

[R53] 查看文件头与实时尾
来源：http://usb.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qsi.chenzaomai.com

[R54] 比较两个文件
来源：http://cei.zhongyouzk.top

diff a.txt b.txt
来源：http://esh.xylfe.cn

[R55] 压缩与解压
来源：http://apu.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ytt.meibo888.top

[R56] 远程拷贝
来源：http://mrc.hammf.cn

scp file user@host:/path/
来源：http://gtm.hongshengwenyu.top

[R57] 远程执行命令
来源：http://eso.kuanghao11.cn

ssh user@host 'uptime'
来源：http://qgz.kuanghao11.cn

[R58] 下载文件
来源：http://vtc.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bwv.aibaodan.cn

[R59] 发 POST JSON
来源：http://ylr.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sgs.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://ljh.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cnb.birdmap.top

[R61] 磁盘占用
来源：http://kgj.yanxiufei.cn

df -h;  du -sh *
来源：http://hks.tian-w.cn

[R62] 找最占空间的文件
来源：http://cwz.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://nir.zhaomingkeji.xyz

[R63] 内存与进程
来源：http://smx.xylfe.cn

free -h;  ps aux | grep nginx
来源：http://nvr.hfpthk.cn

[R64] 结束进程
来源：http://lyb.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://eva.birdmap.top

[R65] 查看端口占用
来源：http://lyn.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ysa.ivvv.top

[R66] 定时任务
来源：http://ngp.aizwys.cn

crontab -e;  crontab -l
来源：http://xly.jiagoushi.top

[R67] 生成随机十六进制串
来源：http://whi.sjlbkw.cn

openssl rand -hex 16
来源：http://ldw.c1oappe.top

[R68] 计算文件校验值
来源：http://qsh.hammf.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iwg.jinqigfzy.top

[R69] 生成随机密码
来源：http://lmo.cheryme.top

head -c 16 /dev/urandom | base64
来源：http://cvv.guannengcc.top

[R70] 时间戳与互转
来源：http://kwm.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://ejy.cdnleiting.top

[R71] 日期格式化
来源：http://ngd.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lpm.yj202588.top

[R72] 等待端口就绪
来源：http://vis.yj20258888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://utn.cucudq.cn

[R73] 分割大日志
来源：http://muf.hnxiangtu.top

split -l 1000 big.log part_
来源：http://wlb.sufxvd.cn

[R74] 批量重命名
来源：http://kuv.xuetiantiany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qsp.gotoacloud.top

[R75] 导出环境变量
来源：http://ijj.iojbl.cn

export PATH="$HOME/bin:$PATH"
来源：http://huz.ivvv.top

[R76] 使用临时文件
来源：http://teu.jiagoushi.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ygl.hfpthk.cn

[R77] 读取用户输入
来源：http://ezz.cheryme.top

read -rp "请输入: " ans
来源：http://qnq.hfpthk.cn

[R78] 交互式菜单
来源：http://psr.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eop.xingfuxueyuan.xyz

[R79] 解析命令行选项
来源：http://nom.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tdd.yuanzhike.top

[R80] 查看脚本执行耗时
来源：http://pss.shanyushiyangkeji.top

time ./run.sh
来源：http://vlr.zhijiandao.cn

================================================================================
来源：http://gzj.shanyushiyangtech.top

S. C / C++ 专题
来源：http://msf.shangyingyoupin.top

================================================================================
来源：http://yac.nwbrower.top

[S01] C：Hello World
来源：http://znv.wangdashe.top

#include <stdio.h>
来源：http://jea.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vly.fengsongda.top

[S02] C：变量与格式化输出
来源：http://cfj.guannengcc.top

int a = 10; printf("%d\n", a);
来源：http://phc.daxiang520.top

[S03] C：读入整数
来源：http://jtn.ppjwa.cn

int x; scanf("%d", &x);
来源：http://gvm.quarkkingdee.top

[S04] C：字符串复制
来源：http://gkn.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://axp.gzhubu.top

[S05] C：字符串长度
来源：http://xeb.52xcode.cn

strlen(s)
来源：http://phj.yueranfly.top

[S06] C：字符串比较
来源：http://jvp.cheryme.top

strcmp(a, b) == 0
来源：http://qyl.yfazqb.com

[S07] C：数组遍历求和
来源：http://bqj.hcnkem.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mhh.jqgfzy.top

[S08] C：动态内存分配与释放
来源：http://byb.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://meg.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://nit.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ptg.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://hcm.wangshuangyany.cn

int *p = &a;  *p = 5;
来源：http://rge.sjlbkw.cn

[S11] C：逐行读文件
来源：http://arl.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://gji.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vui.zhoulong.xyz

fclose(f);
来源：http://ahp.xuanzx.com

[S12] C：写文件
来源：http://alz.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wiy.yangfankeji.com

[S13] C：宏定义
来源：http://yda.haohaochexian.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sdv.mhx1999.top

[S14] C：枚举
来源：http://kvt.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://nru.ivvv.top

[S15] C：类型转换
来源：http://bco.hysaishi.cn

(double) a / b
来源：http://cno.hammf.cn

[S16] C：位操作置位
来源：http://ftb.daria6918.cn

x |= (1 << 3);
来源：http://cvj.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://hln.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://grf.sxryk.cn

[S18] C：命令行参数
来源：http://gvg.shanyushiyangkeji.top

int main(int argc, char **argv)
来源：http://kpf.yangfankeji.com

[S19] C：快速排序
来源：http://eje.birdmap.top

qsort(a, n, sizeof(int), cmp);
来源：http://pdr.vqdsnc.cn

[S20] C：二分查找
来源：http://ofe.chenzaomai.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yrx.jyoumei.cn

[S21] C：字符类别判断
来源：http://pqz.chenzaomai.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gzw.hywenlv.cn

[S22] C：字符串转数字
来源：http://vba.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tby.yonumen.top

[S23] C：随机数
来源：http://qpm.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gqs.chenlongwang.top

[S24] C：获取本地时间
来源：http://etg.snrcjt.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rak.xingfuxueyuan.xyz

[S25] C：内存拷贝
来源：http://wib.jiagoushi.top

memcpy(dst, src, n);
来源：http://etn.chenjidiqi.icu

[S26] C：内存清零
来源：http://xnr.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://xrc.shuidangran.top

[S27] C：定义常量
来源：http://jpg.zhijiandao.cn

const double PI = 3.14159;
来源：http://pvw.xinyue.icu

[S28] C：静态变量
来源：http://hmz.shanyushiyangtech.top

static int counter = 0;
来源：http://kbk.hongshengwenyu.top

[S29] C：变参函数
来源：http://otj.quarkkingdee.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fsm.andypj.xyz

[S30] C：头文件保护
来源：http://gil.yvedp.cn

#ifndef X_H
来源：http://gyh.chenjidiqi.icu

#define X_H
来源：http://tro.jinghuilouyu.cn

#endif
来源：http://svf.redwolf501.top

[S31] C++：Hello World
来源：http://xyi.ybcxt.top

#include <iostream>
来源：http://jyd.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://qlc.guowangkeji.top

[S32] C++：字符串
来源：http://oof.gaohongyu789.top

std::string s = "hi";  s += "!";
来源：http://ffm.haohaochexian.top

[S33] C++：vector 增删
来源：http://rad.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ocz.svipenyu.cn

[S34] C++：遍历 vector
来源：http://eyu.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://taf.gaohongyu789.top

[S35] C++：map
来源：http://qtr.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dna.yfazqb.com

[S36] C++：unordered_map
来源：http://htp.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bwq.jinyuanbaomall.cn

[S37] C++：set
来源：http://eqg.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://abj.tanke756.top

[S38] C++：排序
来源：http://tbl.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://oes.hesvh.cn

[S39] C++：自定义比较器排序
来源：http://fva.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://duz.svipenyu.cn

[S40] C++：查找元素
来源：http://vmo.sxryk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rpz.ybcxt.top

[S41] C++：类与构造函数
来源：http://vsy.chenlongwang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aff.sufxvd.cn

[S42] C++：继承与虚函数
来源：http://hag.hesvh.cn

class B : public Base { public: void f() override {} };
来源：http://qtb.yj20258888.top

[S43] C++：智能指针
来源：http://mua.ivvv.top

auto p = std::make_unique<int>(5);
来源：http://dhm.pengpengdd.cyou

[S44] C++：引用传参
来源：http://dgl.316326.xyz

void inc(int &x) { ++x; }
来源：http://mtg.hesvh.cn

[S45] C++：lambda
来源：http://rxm.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wxe.zhixingplan.top

[S46] C++：函数模板
来源：http://aca.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aec.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://vrx.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bps.tianlin.xyz

[S48] C++：逐行读文件
来源：http://rft.fehbvm.com

std::ifstream in("a.txt");  std::string line;
来源：http://qla.fehbvm.com

while (std::getline(in, line)) { }
来源：http://hpq.chenjidiqi.icu

[S49] C++：写文件
来源：http://ydz.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jvc.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://kiy.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://exf.mhx1999.top

[S51] C++：显式类型转换
来源：http://xnu.ivvv.top

static_cast<double>(a) / b
来源：http://erh.jqgfzy.top

[S52] C++：const 与 noexcept
来源：http://ikl.sxryk.cn

int size() const noexcept { return n_; }
来源：http://yzk.jqgufenzy.top

[S53] C++：移动语义
来源：http://gty.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://idd.wangdashe.top

[S54] C++：异常处理
来源：http://cjw.redwolf501.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kka.aizwys.cn

[S55] C++：结构化绑定
来源：http://wiq.ehwqpu.com

auto [a, b] = std::make_pair(1, 2);
来源：http://lkq.dashuyun.cn

[S56] C++：optional
来源：http://gfd.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kzw.zhaomingkeji.xyz

[S57] C++：编译期常量
来源：http://hne.fzhhl.top

constexpr int N = 10;
来源：http://xkg.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://pjp.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://ycc.fzhhl.top

[S59] C++：静态断言
来源：http://ynd.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bur.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://wuz.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oyo.dashuyun.cn

================================================================================
来源：http://tdy.fehbvm.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://trj.wangdashe.top

================================================================================
来源：http://frw.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://pwu.cheryme.top

println("Hello")
来源：http://yuk.yongpay.top

[T02] Kotlin：变量
来源：http://ggd.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ggn.52xcode.cn

[T03] Kotlin：字符串模板
来源：http://apr.hcnkem.com

"值: $b"
来源：http://hef.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://eud.ppjwa.cn

val n: String? = null;  n?.length
来源：http://hig.sysykeji.top

[T05] Kotlin：when 表达式
来源：http://qrd.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qgk.xziqi.cn

[T06] Kotlin：集合映射
来源：http://zji.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ldo.jianghu66.top

[T07] Kotlin：集合过滤
来源：http://spy.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xld.sysykeji.top

[T08] Kotlin：数据类
来源：http://vap.vehdjk.com

data class User(val name: String, val age: Int)
来源：http://azd.vqdsnc.cn

[T09] Kotlin：扩展函数
来源：http://avs.fktsv.cn

fun String.exclaim() = this + "!"
来源：http://ugp.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://rfp.jiagoushi.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ovo.nanxinkj.top

[T11] Kotlin：协程
来源：http://pfc.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oob.0kj1m.cn

[T12] Kotlin：解构声明
来源：http://klc.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://wll.cdnleiting.top

[T13] Kotlin：只读 Map
来源：http://tqu.sxryk.cn

val m = mapOf("a" to 1)
来源：http://ody.chenlongwang.top

[T14] Kotlin：循环
来源：http://znd.chenzaomai.com

for (i in 1..10) println(i)
来源：http://xgx.hywenlv.cn

[T15] Kotlin：接口
来源：http://uwu.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://chb.c1oappe.top

[T16] Swift：Hello World
来源：http://yja.ydzc1.top

print("Hello")
来源：http://wni.yuanzhike.top

[T17] Swift：变量与常量
来源：http://oqf.cheryme.top

var a = 1;  let b = 2
来源：http://bal.sweek.top

[T18] Swift：字符串插值
来源：http://ppn.svipenyu.cn

"值: \(b)"
来源：http://hvz.ywan-chungtsiang.top

[T19] Swift：可选绑定
来源：http://mfb.zhongyouzk.top

if let n = opt { print(n) }
来源：http://dvp.yj20258.top

[T20] Swift：数组操作
来源：http://rzc.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uws.zhongyouzk.top

[T21] Swift：遍历
来源：http://rkp.jianghu66.top

for x in a { print(x) }
来源：http://zpi.daria6918.cn

[T22] Swift：字典
来源：http://mbb.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wxx.jlsjyb.cn

[T23] Swift：函数
来源：http://esg.guowangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lwc.tarul.cn

[T24] Swift：闭包
来源：http://tfd.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bfw.hywenlv.cn

[T25] Swift：结构体
来源：http://lyh.yvedp.cn

struct P { var x: Int }
来源：http://pxx.zycfv.cn

[T26] Swift：类与重写
来源：http://kbs.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://kas.guowangkeji.top

[T27] Swift：错误处理
来源：http://xic.hammf.cn

do { try f() } catch { print(error) }
来源：http://dsy.ivvv.top

[T28] Swift：枚举
来源：http://vjp.yj202588.top

enum Color { case red, green }
来源：http://rhd.tarul.cn

[T29] Swift：guard 提前返回
来源：http://ncg.xuetiantiany.cn

guard let x = opt else { return }
来源：http://wdp.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://vwt.zhaomingkeji.xyz

protocol Shape { func area() -> Double }
来源：http://nyq.xylfe.cn

[T31] Lua：Hello World
来源：http://ktl.jianghu66.top

print("Hello")
来源：http://gxx.hnqzz.top

[T32] Lua：局部变量
来源：http://oox.9152youxi.cn

local a = 1
来源：http://doi.shanyushiyangkeji.top

[T33] Lua：表（数组）
来源：http://miz.xylfe.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tsx.andypj.xyz

[T34] Lua：遍历表
来源：http://ema.yuxming.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nuz.chenjidiqi.icu

[T35] Lua：字典表
来源：http://ndh.svipenyu.cn

local d = { a = 1 };  d.b = 2
来源：http://jzd.yueranfly.top

[T36] Lua：函数
来源：http://azt.uphjek.com

function add(a, b) return a + b end
来源：http://btg.redwolf501.top

[T37] Lua：字符串拼接
来源：http://acr.uphjek.com

"a" .. "b"
来源：http://tkq.yangfankeji.com

[T38] Lua：条件
来源：http://wvn.chenzaomai.com

if x > 0 then print("正") end
来源：http://kbp.9152youxi.cn

[T39] Lua：模式匹配
来源：http://kac.jqgufenzy.top

string.find(s, "%d+")
来源：http://kgx.fengsongda.top

[T40] Lua：元表
来源：http://mag.uphjek.com

setmetatable({}, { __index = base })
来源：http://ytw.yueranfly.top

[T41] Perl：Hello World
来源：http://cva.nwbrower.top

print "Hello\n";
来源：http://mob.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://dkf.pycfn.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gmn.shangyingyoupin.top

[T43] Perl：字符串插值
来源：http://xgb.zycfv.cn

"值: $a"
来源：http://pfw.cqqwz.cn

[T44] Perl：条件
来源：http://wbc.zhoulong.xyz

if ($a > 0) { print "正"; }
来源：http://uel.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://wdx.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://cne.wangdashe.top

[T46] Perl：哈希操作
来源：http://qle.chenjidiqi.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sfj.shzxlz.cn

[T47] Perl：正则捕获
来源：http://vbd.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xmt.jinqigufen.top

[T48] Perl：正则替换
来源：http://pxr.ivvv.top

$s =~ s/old/new/g;
来源：http://ydr.yangfankeji.com

[T49] Perl：函数
来源：http://fpp.xingfuxueyuan.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lly.yfazqb.com

[T50] Perl：逐行读文件
来源：http://nsn.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xtr.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://gsz.yongpay.top

[T51] Scala：Hello World
来源：http://jsg.hfpthk.cn

println("Hello")
来源：http://mbs.xinyue.icu

[T52] Scala：变量
来源：http://rcz.xuanzx.com

val a = 1;  var b = 2
来源：http://sug.jyoumei.cn

[T53] Scala：字符串插值
来源：http://dfa.zhiwuduotai.top

s"值: $b"
来源：http://fjw.chenzaomai.com

[T54] Scala：集合映射
来源：http://czq.cucudq.cn


<!-- 参考信息 -->