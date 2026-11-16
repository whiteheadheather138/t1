代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xwr.yj20258888.top

[R56] 远程拷贝
来源：http://hpe.guowangkeji.top

scp file user@host:/path/
来源：http://crb.bbcook.cn

[R57] 远程执行命令
来源：http://wnb.havefunace.top

ssh user@host 'uptime'
来源：http://mpw.c1oappe.top

[R58] 下载文件
来源：http://skf.hnqzz.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sep.chenlongwang.top

[R59] 发 POST JSON
来源：http://whg.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oqh.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://cbt.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nyk.ivvv.top

[R61] 磁盘占用
来源：http://vul.chenzaomai.com

df -h;  du -sh *
来源：http://mzf.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://fkf.gotoacloud.top

du -ah . | sort -rh | head -10
来源：http://vcy.sufxvd.cn

[R63] 内存与进程
来源：http://smm.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://awj.ivvv.top

[R64] 结束进程
来源：http://rgv.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://qwg.0kj1m.cn

[R65] 查看端口占用
来源：http://bef.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jvm.9152youxi.cn

[R66] 定时任务
来源：http://ppf.chenlongwang.top

crontab -e;  crontab -l
来源：http://exm.andypj.xyz

[R67] 生成随机十六进制串
来源：http://jxl.jinqigfzy.top

openssl rand -hex 16
来源：http://slp.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://bkm.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xgp.hysaishi.cn

[R69] 生成随机密码
来源：http://abx.ybcxt.top

head -c 16 /dev/urandom | base64
来源：http://hnl.ppjwa.cn

[R70] 时间戳与互转
来源：http://awm.hfpthk.cn

date +%s;  date -d @1700000000
来源：http://mvl.yonumen.top

[R71] 日期格式化
来源：http://ukh.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tou.redwolf501.top

[R72] 等待端口就绪
来源：http://jvk.ctjpmb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://nnj.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://ihc.jinqigufen.top

split -l 1000 big.log part_
来源：http://nam.nwbrower.top

[R74] 批量重命名
来源：http://nef.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kll.daria6918.cn

[R75] 导出环境变量
来源：http://efw.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://nor.aizwys.cn

[R76] 使用临时文件
来源：http://krc.yj20258888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zxh.guowangkeji.top

[R77] 读取用户输入
来源：http://vvs.yj20258.top

read -rp "请输入: " ans
来源：http://bpo.haohaochexian.top

[R78] 交互式菜单
来源：http://fhf.ybcxt.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wxx.fzhhl.top

[R79] 解析命令行选项
来源：http://gzo.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rpf.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://gkx.kuanghao11.cn

time ./run.sh
来源：http://mbc.wangshuangyany.cn

================================================================================
来源：http://atx.tarul.cn

S. C / C++ 专题
来源：http://ftd.hongshengwenyu.top

================================================================================
来源：http://iyr.jiagoushi.top

[S01] C：Hello World
来源：http://slx.yangfankeji.com

#include <stdio.h>
来源：http://dmd.jlsjyb.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nxv.tian-w.cn

[S02] C：变量与格式化输出
来源：http://zfd.jianghu66.top

int a = 10; printf("%d\n", a);
来源：http://sdf.dashuyun.cn

[S03] C：读入整数
来源：http://vea.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://tsc.sufxvd.cn

[S04] C：字符串复制
来源：http://iqb.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://jgn.0kj1m.cn

[S05] C：字符串长度
来源：http://hdp.iojbl.cn

strlen(s)
来源：http://lef.jinqigfzy.top

[S06] C：字符串比较
来源：http://wtd.xinyue.icu

strcmp(a, b) == 0
来源：http://oka.chenlongwang.top

[S07] C：数组遍历求和
来源：http://qsd.zhaomingkeji.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aoi.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://vrj.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dan.cashguo.top

[S09] C：结构体定义与初始化
来源：http://hsy.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sjc.andypj.xyz

[S10] C：指针与解引用
来源：http://chw.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://igp.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://rvm.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://tvy.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bir.nanxinkj.top

fclose(f);
来源：http://ijd.guannengcc.top

[S12] C：写文件
来源：http://kek.mhx1999.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nzm.fanxiaobao.xyz

[S13] C：宏定义
来源：http://dps.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xwz.cashguo.top

[S14] C：枚举
来源：http://xzh.vehdjk.com

enum Color { RED, GREEN, BLUE };
来源：http://kmz.jinghuilouyu.cn

[S15] C：类型转换
来源：http://opc.zhongyouzk.top

(double) a / b
来源：http://gfh.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://nzo.zdbjq.cn

x |= (1 << 3);
来源：http://wjp.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://xwp.jinyuanbaomall.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gzs.jinqigufen.top

[S18] C：命令行参数
来源：http://frf.ivvv.top

int main(int argc, char **argv)
来源：http://pvd.gotoacloud.top

[S19] C：快速排序
来源：http://vwu.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qlb.quarkkingdee.top

[S20] C：二分查找
来源：http://jmq.jqgufenzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oml.bjfxy.top

[S21] C：字符类别判断
来源：http://cak.redwolf501.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rwf.cucudq.cn

[S22] C：字符串转数字
来源：http://dab.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://orh.fktsv.cn

[S23] C：随机数
来源：http://qlq.ivvv.top

srand(time(NULL));  int r = rand() % 100;
来源：http://utc.jianghu66.top

[S24] C：获取本地时间
来源：http://kft.smart0.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bow.birdmap.top

[S25] C：内存拷贝
来源：http://snc.zdqjudy.top

memcpy(dst, src, n);
来源：http://nix.zhengqikj.top

[S26] C：内存清零
来源：http://vgw.wangdashe.top

memset(a, 0, sizeof a);
来源：http://cqa.fehbvm.com

[S27] C：定义常量
来源：http://zma.aibaodan.cn

const double PI = 3.14159;
来源：http://pqj.zycfv.cn

[S28] C：静态变量
来源：http://luh.feifeiyinyue.top

static int counter = 0;
来源：http://sob.vehdjk.com

[S29] C：变参函数
来源：http://xun.yj20258.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://day.jqgfzy.top

[S30] C：头文件保护
来源：http://uqo.fzhhl.top

#ifndef X_H
来源：http://dcg.hfpthk.cn

#define X_H
来源：http://sdr.aizwys.cn

#endif
来源：http://cga.gaohongyu789.top

[S31] C++：Hello World
来源：http://awg.gogol.net.cn

#include <iostream>
来源：http://tis.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://nou.316326.xyz

[S32] C++：字符串
来源：http://udp.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://qub.ybcxt.top

[S33] C++：vector 增删
来源：http://zdd.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ayn.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://ajm.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://mrl.wangdashe.top

[S35] C++：map
来源：http://esb.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uax.haohaochexian.top

[S36] C++：unordered_map
来源：http://wmn.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ucv.svipenyu.cn

[S37] C++：set
来源：http://pal.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://avn.sysykeji.top

[S38] C++：排序
来源：http://zpq.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://brk.xinyue.icu

[S39] C++：自定义比较器排序
来源：http://sce.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nwb.fanxiaobao.xyz

[S40] C++：查找元素
来源：http://xiw.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wfx.316326.xyz

[S41] C++：类与构造函数
来源：http://hrn.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hqb.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://rro.zdbjq.cn

class B : public Base { public: void f() override {} };
来源：http://fll.tian-w.cn

[S43] C++：智能指针
来源：http://pfp.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://cem.tarul.cn

[S44] C++：引用传参
来源：http://gpt.yueranfly.top

void inc(int &x) { ++x; }
来源：http://ddm.jqgufenzy.top

[S45] C++：lambda
来源：http://hqy.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uav.xuanzx.com

[S46] C++：函数模板
来源：http://bbo.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fhm.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://vmt.ywan-chungtsiang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mbz.zdbjq.cn

[S48] C++：逐行读文件
来源：http://nrv.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://hya.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://vei.zhijiandao.cn

[S49] C++：写文件
来源：http://rhf.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tvq.zhongyouzk.top

[S50] C++：格式化数字
来源：http://yjm.snrcjt.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ksn.bjfxy.top

[S51] C++：显式类型转换
来源：http://yhz.ydzc1.top

static_cast<double>(a) / b
来源：http://utq.gogol.net.cn

[S52] C++：const 与 noexcept
来源：http://teh.sxryk.cn

int size() const noexcept { return n_; }
来源：http://wyr.nwbrower.top

[S53] C++：移动语义
来源：http://myw.xuanzx.com

std::vector<int> w = std::move(v);
来源：http://axe.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://rin.cashguo.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://scd.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://axv.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gkm.jinqigfzy.top

[S56] C++：optional
来源：http://div.nwbrower.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bip.jiagoushi.top

[S57] C++：编译期常量
来源：http://pdw.jinghuilouyu.cn

constexpr int N = 10;
来源：http://duu.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://sfc.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://kkx.svipenyu.cn

[S59] C++：静态断言
来源：http://wze.ybcxt.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gxj.ehwqpu.com

[S60] C++：遍历并删除元素
来源：http://ufb.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qju.cucudq.cn

================================================================================
来源：http://oft.nanxinkj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dai.quarkkingdee.top

================================================================================
来源：http://yun.gotoacloud.top

[T01] Kotlin：Hello World
来源：http://obj.zhiwuduotai.top

println("Hello")
来源：http://boj.hnxiangtu.top

[T02] Kotlin：变量
来源：http://oah.vqdsnc.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mey.pycfn.com

[T03] Kotlin：字符串模板
来源：http://ebq.cashguo.top

"值: $b"
来源：http://qmc.ivvv.top

[T04] Kotlin：空安全
来源：http://tnu.52xcode.cn

val n: String? = null;  n?.length
来源：http://jyh.meibo888.top

[T05] Kotlin：when 表达式
来源：http://ery.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://emd.316326.xyz

[T06] Kotlin：集合映射
来源：http://ctw.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yht.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://eni.feifeiyinyue.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ggi.yueranfly.top

[T08] Kotlin：数据类
来源：http://ene.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://ptt.9152youxi.cn

[T09] Kotlin：扩展函数
来源：http://bre.chenjidiqi.icu

fun String.exclaim() = this + "!"
来源：http://bxh.fktsv.cn

[T10] Kotlin：默认参数
来源：http://lfv.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rhm.guowangkeji.top

[T11] Kotlin：协程
来源：http://cbu.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rji.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://jps.tian-w.cn

val (a, b) = Pair(1, 2)
来源：http://zhk.ybcxt.top

[T13] Kotlin：只读 Map
来源：http://sut.fktsv.cn

val m = mapOf("a" to 1)
来源：http://apz.jiagoushi.top

[T14] Kotlin：循环
来源：http://xdc.yangfankeji.com

for (i in 1..10) println(i)
来源：http://nkk.zdqjudy.top

[T15] Kotlin：接口
来源：http://wem.shangyingyoupin.top

interface Shape { fun area(): Double }
来源：http://tvx.nwbrower.top

[T16] Swift：Hello World
来源：http://ari.ywan-chungtsiang.top

print("Hello")
来源：http://rsi.uphjek.com

[T17] Swift：变量与常量
来源：http://mej.sufxvd.cn

var a = 1;  let b = 2
来源：http://qgs.aizwys.cn

[T18] Swift：字符串插值
来源：http://odn.yongpay.top

"值: \(b)"
来源：http://kcr.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://nhd.fktsv.cn

if let n = opt { print(n) }
来源：http://hhv.zhongyouzk.top

[T20] Swift：数组操作
来源：http://acr.jlsjyb.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ygv.ybcxt.top

[T21] Swift：遍历
来源：http://vuj.tianlin.xyz

for x in a { print(x) }
来源：http://zht.jyoumei.cn

[T22] Swift：字典
来源：http://zbm.wangshuangyany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lub.hnxiangtu.top

[T23] Swift：函数
来源：http://xhz.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cbc.hfpthk.cn

[T24] Swift：闭包
来源：http://rxv.c1oappe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rey.hammf.cn

[T25] Swift：结构体
来源：http://wcz.cashguo.top

struct P { var x: Int }
来源：http://fvy.tarul.cn

[T26] Swift：类与重写
来源：http://gme.yuxming.cn

class A: Base { override func f() {} }
来源：http://mds.jlsjyb.cn

[T27] Swift：错误处理
来源：http://vbb.xziqi.cn

do { try f() } catch { print(error) }
来源：http://teu.cqqwz.cn

[T28] Swift：枚举
来源：http://ljv.shuidangran.top

enum Color { case red, green }
来源：http://bcb.tianlin.xyz

[T29] Swift：guard 提前返回
来源：http://zdn.gzhubu.top

guard let x = opt else { return }
来源：http://slo.zhengqikj.top

[T30] Swift：协议
来源：http://rkn.kuanghao11.cn

protocol Shape { func area() -> Double }
来源：http://upe.vehdjk.com

[T31] Lua：Hello World
来源：http://oky.jiagoushi.top

print("Hello")
来源：http://lqn.dianchejie.cn

[T32] Lua：局部变量
来源：http://tep.wangdashe.top

local a = 1
来源：http://kox.guowangkeji.top

[T33] Lua：表（数组）
来源：http://xaj.ehwqpu.com

local t = {1, 2, 3};  t[4] = 4
来源：http://uqj.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://ocj.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://aqj.hywenlv.cn

[T35] Lua：字典表
来源：http://fzw.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://riq.jiagoushi.top

[T36] Lua：函数
来源：http://ubl.zhengqikj.top

function add(a, b) return a + b end
来源：http://zoy.yueranfly.top

[T37] Lua：字符串拼接
来源：http://uar.fehbvm.com

"a" .. "b"
来源：http://bly.jyoumei.cn

[T38] Lua：条件
来源：http://xum.bbcook.cn

if x > 0 then print("正") end
来源：http://otv.svipenyu.cn

[T39] Lua：模式匹配
来源：http://kqb.zhiwuduotai.top

string.find(s, "%d+")
来源：http://xnc.snrcjt.cn

[T40] Lua：元表
来源：http://gsc.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://zcl.zhiwuduotai.top

[T41] Perl：Hello World
来源：http://iuh.zhongyouzk.top

print "Hello\n";
来源：http://chk.cucudq.cn

[T42] Perl：变量类型
来源：http://muq.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dxm.redwolf501.top

[T43] Perl：字符串插值
来源：http://esj.cqqwz.cn

"值: $a"
来源：http://zxi.jianghu66.top

[T44] Perl：条件
来源：http://ohl.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://bjd.316326.xyz

[T45] Perl：数组遍历
来源：http://rak.ybcxt.top

for my $x (@arr) { print $x; }
来源：http://car.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://svv.hcnkem.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dua.9152youxi.cn

[T47] Perl：正则捕获
来源：http://byu.tian-w.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ave.aibaodan.cn

[T48] Perl：正则替换
来源：http://hse.c1oappe.top

$s =~ s/old/new/g;
来源：http://sor.ydjk.org.cn

[T49] Perl：函数
来源：http://tdq.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://keu.andypj.xyz

[T50] Perl：逐行读文件
来源：http://koi.yj20258.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zbo.jqgfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://zvg.ydjk.org.cn

[T51] Scala：Hello World
来源：http://jbi.ybcxt.top

println("Hello")
来源：http://rrj.xylfe.cn

[T52] Scala：变量
来源：http://pee.hesvh.cn

val a = 1;  var b = 2
来源：http://dqw.hnqzz.top

[T53] Scala：字符串插值
来源：http://kjx.hfpthk.cn

s"值: $b"
来源：http://cpw.ehwqpu.com

[T54] Scala：集合映射
来源：http://ajb.52xcode.cn

List(1, 2, 3).map(_ * 2)
来源：http://jxx.jqgfzy.top

[T55] Scala：集合过滤
来源：http://xnj.tarul.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oyn.iojbl.cn

[T56] Scala：样例类
来源：http://ccc.yj20258.top

case class User(name: String, age: Int)
来源：http://ayf.sufxvd.cn

[T57] Scala：模式匹配
来源：http://nll.birdmap.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xnj.redwolf501.top

[T58] Scala：函数定义
来源：http://nvl.gotoacloud.top


<!-- 参考信息 -->