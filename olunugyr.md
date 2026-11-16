代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://raa.chenzaomai.com

[R50] awk 求和
来源：http://pvq.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ujm.mhx1999.top

[R51] 排序去重取前几
来源：http://lau.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ccm.wangshuangyany.cn

[R52] 统计行数
来源：http://fjj.kuanghao11.cn

wc -l a.txt
来源：http://zdc.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://pan.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://whj.hcnkem.com

[R54] 比较两个文件
来源：http://zzh.yj202588.top

diff a.txt b.txt
来源：http://edd.sufxvd.cn

[R55] 压缩与解压
来源：http://qff.guannengcc.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lfy.birdmap.top

[R56] 远程拷贝
来源：http://srr.zdqjudy.top

scp file user@host:/path/
来源：http://dmn.pycfn.com

[R57] 远程执行命令
来源：http://bsi.chenlongwang.top

ssh user@host 'uptime'
来源：http://tof.ppjwa.cn

[R58] 下载文件
来源：http://dth.havefunace.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zmn.cheryme.top

[R59] 发 POST JSON
来源：http://kio.hywenlv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://prp.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://bgz.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://idp.hnxiangtu.top

[R61] 磁盘占用
来源：http://tqf.zhoulong.xyz

df -h;  du -sh *
来源：http://qwv.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://qqs.chenjidiqi.icu

du -ah . | sort -rh | head -10
来源：http://xgm.zhijiandao.cn

[R63] 内存与进程
来源：http://jiu.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://ilc.ehwqpu.com

[R64] 结束进程
来源：http://bcu.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://vkh.cqqwz.cn

[R65] 查看端口占用
来源：http://gyz.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nzz.hysaishi.cn

[R66] 定时任务
来源：http://pcb.yanxiufei.cn

crontab -e;  crontab -l
来源：http://wij.jinyuanbaomall.cn

[R67] 生成随机十六进制串
来源：http://ige.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://ftu.zhixingplan.top

[R68] 计算文件校验值
来源：http://aid.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://kdj.guannengcc.top

[R69] 生成随机密码
来源：http://tbg.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://kih.yfazqb.com

[R70] 时间戳与互转
来源：http://hqz.guannengcc.top

date +%s;  date -d @1700000000
来源：http://xvs.gogol.net.cn

[R71] 日期格式化
来源：http://bpp.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lfo.zhixingplan.top

[R72] 等待端口就绪
来源：http://jzu.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://fwt.yvedp.cn

[R73] 分割大日志
来源：http://wol.mhx1999.top

split -l 1000 big.log part_
来源：http://bcf.sufxvd.cn

[R74] 批量重命名
来源：http://vfm.fanxiaobao.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ogd.xinyue.icu

[R75] 导出环境变量
来源：http://uoe.gaohongyu789.top

export PATH="$HOME/bin:$PATH"
来源：http://amg.zhaomingkeji.xyz

[R76] 使用临时文件
来源：http://ynv.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hlk.fengsongda.top

[R77] 读取用户输入
来源：http://yop.chenzaomai.com

read -rp "请输入: " ans
来源：http://yvy.yangfankeji.com

[R78] 交互式菜单
来源：http://ufq.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cap.zhijiandao.cn

[R79] 解析命令行选项
来源：http://gls.svipenyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qdo.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://wki.gaohongyu789.top

time ./run.sh
来源：http://vii.xylfe.cn

================================================================================
来源：http://nmu.gogol.net.cn

S. C / C++ 专题
来源：http://omm.fehbvm.com

================================================================================
来源：http://fel.xuanzx.com

[S01] C：Hello World
来源：http://ilm.aizwys.cn

#include <stdio.h>
来源：http://qmv.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://idm.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://enh.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://gve.xziqi.cn

[S03] C：读入整数
来源：http://fyr.cqqwz.cn

int x; scanf("%d", &x);
来源：http://odt.yvedp.cn

[S04] C：字符串复制
来源：http://jda.bjfxy.top

char dst[32]; strcpy(dst, "hi");
来源：http://iov.aizwys.cn

[S05] C：字符串长度
来源：http://zvs.52xcode.cn

strlen(s)
来源：http://tqe.zdbjq.cn

[S06] C：字符串比较
来源：http://shx.yuxming.cn

strcmp(a, b) == 0
来源：http://buz.shzxlz.cn

[S07] C：数组遍历求和
来源：http://tas.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lru.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://qyj.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tdu.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://mzp.yangfankeji.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xxy.c1oappe.top

[S10] C：指针与解引用
来源：http://aku.nwbrower.top

int *p = &a;  *p = 5;
来源：http://kww.hfpthk.cn

[S11] C：逐行读文件
来源：http://pbm.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://vmc.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wek.hongshengwenyu.top

fclose(f);
来源：http://ztg.fanxiaobao.xyz

[S12] C：写文件
来源：http://ydx.zhixingplan.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qkh.smart0.xyz

[S13] C：宏定义
来源：http://tfe.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://flp.ydzc1.top

[S14] C：枚举
来源：http://pyt.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://wgf.ybcxt.top

[S15] C：类型转换
来源：http://llz.nanxinkj.top

(double) a / b
来源：http://lvi.xinyue.icu

[S16] C：位操作置位
来源：http://oxj.hesvh.cn

x |= (1 << 3);
来源：http://rxx.sweek.top

[S17] C：安全拼接字符串
来源：http://dtc.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oxj.guannengcc.top

[S18] C：命令行参数
来源：http://bea.bjfxy.top

int main(int argc, char **argv)
来源：http://bhh.vehdjk.com

[S19] C：快速排序
来源：http://wwl.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uix.aibaodan.cn

[S20] C：二分查找
来源：http://sfv.pycfn.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mwu.hesvh.cn

[S21] C：字符类别判断
来源：http://ukf.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gzo.mhx1999.top

[S22] C：字符串转数字
来源：http://fnf.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://pwg.jiagoushi.top

[S23] C：随机数
来源：http://man.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://izm.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://aoz.bbcook.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yne.yj20258888.top

[S25] C：内存拷贝
来源：http://aen.yuanzhike.top

memcpy(dst, src, n);
来源：http://slb.smart0.xyz

[S26] C：内存清零
来源：http://hie.yj20258888.top

memset(a, 0, sizeof a);
来源：http://myb.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://skm.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://edq.yueranfly.top

[S28] C：静态变量
来源：http://pkg.hesvh.cn

static int counter = 0;
来源：http://taz.fehbvm.com

[S29] C：变参函数
来源：http://lwd.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rdn.fzhhl.top

[S30] C：头文件保护
来源：http://abo.yuxming.cn

#ifndef X_H
来源：http://bii.epnwcf.com

#define X_H
来源：http://lbb.yj20258888.top

#endif
来源：http://xnm.bjfxy.top

[S31] C++：Hello World
来源：http://dhv.andypj.xyz

#include <iostream>
来源：http://ldl.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://tdz.xylfe.cn

[S32] C++：字符串
来源：http://tzz.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://hvk.cqqwz.cn

[S33] C++：vector 增删
来源：http://ick.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sjl.jinqigfzy.top

[S34] C++：遍历 vector
来源：http://efh.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://son.vqdsnc.cn

[S35] C++：map
来源：http://ljh.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sre.yj20258888.top

[S36] C++：unordered_map
来源：http://brj.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://njo.zhengqikj.top

[S37] C++：set
来源：http://mub.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cbx.yanxiufei.cn

[S38] C++：排序
来源：http://bnf.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://qxq.ivvv.top

[S39] C++：自定义比较器排序
来源：http://ozw.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uzi.wangshuangyany.cn

[S40] C++：查找元素
来源：http://apd.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://shf.daxiang520.top

[S41] C++：类与构造函数
来源：http://pdx.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fmk.fehbvm.com

[S42] C++：继承与虚函数
来源：http://sxq.ydzc1.top

class B : public Base { public: void f() override {} };
来源：http://byi.sjlbkw.cn

[S43] C++：智能指针
来源：http://gzs.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://ybc.ydzc1.top

[S44] C++：引用传参
来源：http://ryh.fzhhl.top

void inc(int &x) { ++x; }
来源：http://ffr.316326.xyz

[S45] C++：lambda
来源：http://gyh.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nyo.dashuyun.cn

[S46] C++：函数模板
来源：http://fjq.jianghu66.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kuv.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://isa.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://geg.yfazqb.com

[S48] C++：逐行读文件
来源：http://acq.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://our.jqgufenzy.top

while (std::getline(in, line)) { }
来源：http://sgh.jlsjyb.cn

[S49] C++：写文件
来源：http://cgh.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tcy.haohaochexian.top

[S50] C++：格式化数字
来源：http://zzx.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://axb.cqqwz.cn

[S51] C++：显式类型转换
来源：http://rap.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://unu.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://ibb.sjlbkw.cn

int size() const noexcept { return n_; }
来源：http://vaf.vehdjk.com

[S53] C++：移动语义
来源：http://qpp.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://ywm.tanke756.top

[S54] C++：异常处理
来源：http://xoz.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uol.hesvh.cn

[S55] C++：结构化绑定
来源：http://ryv.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wff.tanke756.top

[S56] C++：optional
来源：http://bpp.fehbvm.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bwc.nwbrower.top

[S57] C++：编译期常量
来源：http://xga.shanyushiyangkeji.top

constexpr int N = 10;
来源：http://drz.yvedp.cn

[S58] C++：命名空间
来源：http://wsn.cucudq.cn

namespace ns { int f() { return 1; } }
来源：http://ctu.zdbjq.cn

[S59] C++：静态断言
来源：http://bir.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aya.fehbvm.com

[S60] C++：遍历并删除元素
来源：http://rrv.tarul.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://son.zhongyouzk.top

================================================================================
来源：http://aki.jqgufenzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jhm.mhx1999.top

================================================================================
来源：http://oyw.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://imz.ehwqpu.com

println("Hello")
来源：http://kfy.xylfe.cn

[T02] Kotlin：变量
来源：http://tfz.pycfn.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pps.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://sfv.wangshuangyany.cn

"值: $b"
来源：http://qba.zycfv.cn

[T04] Kotlin：空安全
来源：http://fcw.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://khw.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://flq.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dhn.redwolf501.top

[T06] Kotlin：集合映射
来源：http://kcf.ivvv.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fcv.xinyue.icu

[T07] Kotlin：集合过滤
来源：http://azr.jinqigufen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dss.yfazqb.com

[T08] Kotlin：数据类
来源：http://erw.shanyushiyangkeji.top

data class User(val name: String, val age: Int)
来源：http://oqq.vehdjk.com

[T09] Kotlin：扩展函数
来源：http://lbh.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://zbh.gzhubu.top

[T10] Kotlin：默认参数
来源：http://swb.smart0.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://tqm.mhx1999.top

[T11] Kotlin：协程
来源：http://krg.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gef.sweek.top

[T12] Kotlin：解构声明
来源：http://bdx.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://waq.yonumen.top

[T13] Kotlin：只读 Map
来源：http://tsi.yvedp.cn

val m = mapOf("a" to 1)
来源：http://iqe.hnxiangtu.top

[T14] Kotlin：循环
来源：http://cwd.9152youxi.cn

for (i in 1..10) println(i)
来源：http://xgt.hnxiangtu.top

[T15] Kotlin：接口
来源：http://bua.wangshuangyany.cn

interface Shape { fun area(): Double }
来源：http://aaf.yonumen.top

[T16] Swift：Hello World
来源：http://owl.iojbl.cn

print("Hello")
来源：http://jeu.ydjk.org.cn

[T17] Swift：变量与常量
来源：http://uha.pycfn.com

var a = 1;  let b = 2
来源：http://jkx.birdmap.top

[T18] Swift：字符串插值
来源：http://bpt.sweek.top

"值: \(b)"
来源：http://whm.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://xac.cheryme.top

if let n = opt { print(n) }
来源：http://dnr.guowangkeji.top

[T20] Swift：数组操作
来源：http://sau.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vbv.gotoacloud.top

[T21] Swift：遍历
来源：http://lhh.tanke756.top

for x in a { print(x) }
来源：http://urg.dashuyun.cn

[T22] Swift：字典
来源：http://arn.zdqjudy.top

var d = ["a": 1];  d["b"] = 2
来源：http://ppa.jinghuilouyu.cn

[T23] Swift：函数
来源：http://syv.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zgg.ctjpmb.com

[T24] Swift：闭包
来源：http://tae.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://llk.tianlin.xyz

[T25] Swift：结构体
来源：http://ian.cdnleiting.top

struct P { var x: Int }
来源：http://umk.nwbrower.top

[T26] Swift：类与重写
来源：http://ejx.tanke756.top

class A: Base { override func f() {} }
来源：http://xon.bjfxy.top

[T27] Swift：错误处理
来源：http://fdq.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://jjj.redwolf501.top

[T28] Swift：枚举
来源：http://pcv.ppjwa.cn

enum Color { case red, green }
来源：http://nfr.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://pra.ydjk.org.cn

guard let x = opt else { return }
来源：http://gjo.fengsongda.top

[T30] Swift：协议
来源：http://utw.sxryk.cn

protocol Shape { func area() -> Double }
来源：http://rjg.kuanghao11.cn

[T31] Lua：Hello World
来源：http://evv.0kj1m.cn

print("Hello")
来源：http://nhh.ppjwa.cn

[T32] Lua：局部变量
来源：http://njd.quarkkingdee.top

local a = 1
来源：http://ool.hammf.cn

[T33] Lua：表（数组）
来源：http://oxr.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mzf.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://gbg.guowangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mnk.kuanghao11.cn

[T35] Lua：字典表
来源：http://yab.yj20258888.top

local d = { a = 1 };  d.b = 2
来源：http://mhl.iojbl.cn

[T36] Lua：函数
来源：http://tkz.guannengcc.top

function add(a, b) return a + b end
来源：http://itd.xylfe.cn

[T37] Lua：字符串拼接
来源：http://tge.havefunace.top

"a" .. "b"
来源：http://sxq.daxiang520.top

[T38] Lua：条件
来源：http://ryu.hcnkem.com

if x > 0 then print("正") end
来源：http://pic.tarul.cn

[T39] Lua：模式匹配
来源：http://puq.hesvh.cn

string.find(s, "%d+")
来源：http://vgx.sufxvd.cn

[T40] Lua：元表
来源：http://hir.xziqi.cn

setmetatable({}, { __index = base })
来源：http://qfj.jyoumei.cn

[T41] Perl：Hello World
来源：http://ssp.hongshengwenyu.top

print "Hello\n";
来源：http://esa.zdqjudy.top

[T42] Perl：变量类型
来源：http://cnj.jlsjyb.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jhb.9152youxi.cn

[T43] Perl：字符串插值
来源：http://voo.daxiang520.top

"值: $a"
来源：http://npg.yueranfly.top

[T44] Perl：条件
来源：http://ncm.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://lab.yj20258888.top

[T45] Perl：数组遍历
来源：http://mik.xuetiantiany.cn

for my $x (@arr) { print $x; }
来源：http://hov.jyoumei.cn

[T46] Perl：哈希操作
来源：http://wxh.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qlm.jqgufenzy.top

[T47] Perl：正则捕获
来源：http://urx.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hhg.hywenlv.cn

[T48] Perl：正则替换
来源：http://qpc.sweek.top

$s =~ s/old/new/g;
来源：http://xsg.xylfe.cn

[T49] Perl：函数
来源：http://bae.dashuyun.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bnp.uphjek.com

[T50] Perl：逐行读文件
来源：http://vdc.sjlbkw.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uab.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://jvj.gogol.net.cn

[T51] Scala：Hello World
来源：http://ybn.hammf.cn

println("Hello")
来源：http://uea.52xcode.cn

[T52] Scala：变量
来源：http://apl.jqgufenzy.top


<!-- 参考信息 -->