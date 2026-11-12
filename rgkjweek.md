代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kgn.ppjwa.cn

[R54] 比较两个文件
来源：http://wmj.xylfe.cn

diff a.txt b.txt
来源：http://aqs.yj20258.top

[R55] 压缩与解压
来源：http://qon.jqgufenzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jnq.pengpengdd.cyou

[R56] 远程拷贝
来源：http://kpr.iojbl.cn

scp file user@host:/path/
来源：http://gnh.uphjek.com

[R57] 远程执行命令
来源：http://lmz.hysaishi.cn

ssh user@host 'uptime'
来源：http://mid.zhijiandao.cn

[R58] 下载文件
来源：http://gzo.ivvv.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dqd.zdbjq.cn

[R59] 发 POST JSON
来源：http://juj.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wxa.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://dhl.fzhhl.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kvo.yj202588.top

[R61] 磁盘占用
来源：http://onv.shanyushiyangtech.top

df -h;  du -sh *
来源：http://zzk.zdbjq.cn

[R62] 找最占空间的文件
来源：http://tzc.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://wes.xuetiantiany.cn

[R63] 内存与进程
来源：http://sra.shanyushiyangtech.top

free -h;  ps aux | grep nginx
来源：http://csp.ehwqpu.com

[R64] 结束进程
来源：http://yha.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://gku.nanxuanxn.top

[R65] 查看端口占用
来源：http://ubp.shangyingyoupin.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://shz.feifeiyinyue.top

[R66] 定时任务
来源：http://weg.meibo888.top

crontab -e;  crontab -l
来源：http://vuy.316326.xyz

[R67] 生成随机十六进制串
来源：http://fbm.ydjk.org.cn

openssl rand -hex 16
来源：http://qkb.c1oappe.top

[R68] 计算文件校验值
来源：http://bnd.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mos.ctjpmb.com

[R69] 生成随机密码
来源：http://aqc.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://ger.dianchejie.cn

[R70] 时间戳与互转
来源：http://vin.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://qlx.shanyushiyangtech.top

[R71] 日期格式化
来源：http://mpv.fzhhl.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ces.yanxiufei.cn

[R72] 等待端口就绪
来源：http://kpq.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rkq.ctjpmb.com

[R73] 分割大日志
来源：http://svi.quarkkingdee.top

split -l 1000 big.log part_
来源：http://rzk.iojbl.cn

[R74] 批量重命名
来源：http://ggb.yfazqb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rtf.c1oappe.top

[R75] 导出环境变量
来源：http://uez.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://xqv.uphjek.com

[R76] 使用临时文件
来源：http://acz.uphjek.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ccd.mhx1999.top

[R77] 读取用户输入
来源：http://iof.tarul.cn

read -rp "请输入: " ans
来源：http://uhg.xuetiantiany.cn

[R78] 交互式菜单
来源：http://cwr.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://yfv.xylfe.cn

[R79] 解析命令行选项
来源：http://gda.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kup.jianghu66.top

[R80] 查看脚本执行耗时
来源：http://kgv.bjfxy.top

time ./run.sh
来源：http://wip.snrcjt.cn

================================================================================
来源：http://izp.zhongyouzk.top

S. C / C++ 专题
来源：http://ooo.bbcook.cn

================================================================================
来源：http://ndv.hnxiangtu.top

[S01] C：Hello World
来源：http://klu.sjlbkw.cn

#include <stdio.h>
来源：http://kju.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://bsm.andypj.xyz

[S02] C：变量与格式化输出
来源：http://elh.havefunace.top

int a = 10; printf("%d\n", a);
来源：http://rlt.ehwqpu.com

[S03] C：读入整数
来源：http://vuh.daria6918.cn

int x; scanf("%d", &x);
来源：http://jlj.hnxiangtu.top

[S04] C：字符串复制
来源：http://ciu.shzxlz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tar.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://xyo.zhengqikj.top

strlen(s)
来源：http://xam.birdmap.top

[S06] C：字符串比较
来源：http://qjv.gogol.net.cn

strcmp(a, b) == 0
来源：http://jee.hywenlv.cn

[S07] C：数组遍历求和
来源：http://vwk.sxryk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iel.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://age.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://evl.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://kxj.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vph.kuanghao11.cn

[S10] C：指针与解引用
来源：http://ubr.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://qld.vehdjk.com

[S11] C：逐行读文件
来源：http://qpg.fktsv.cn

FILE *f = fopen("a.txt", "r");
来源：http://rvr.cashguo.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gwj.hammf.cn

fclose(f);
来源：http://ykh.zhiwuduotai.top

[S12] C：写文件
来源：http://fel.gaohongyu789.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pvb.hysaishi.cn

[S13] C：宏定义
来源：http://led.cashguo.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qbg.redwolf501.top

[S14] C：枚举
来源：http://jzo.ydzc1.top

enum Color { RED, GREEN, BLUE };
来源：http://tww.hongshengwenyu.top

[S15] C：类型转换
来源：http://yxr.fehbvm.com

(double) a / b
来源：http://jtt.fanxiaobao.xyz

[S16] C：位操作置位
来源：http://njx.shuidangran.top

x |= (1 << 3);
来源：http://lnc.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://hzc.bjfxy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jge.dashuyun.cn

[S18] C：命令行参数
来源：http://rlj.0kj1m.cn

int main(int argc, char **argv)
来源：http://lte.fktsv.cn

[S19] C：快速排序
来源：http://azh.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fie.birdmap.top

[S20] C：二分查找
来源：http://lmc.jqgfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qsj.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://rtc.cheryme.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gtm.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://upn.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://mmk.xziqi.cn

[S23] C：随机数
来源：http://its.fengsongda.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zrh.zdqjudy.top

[S24] C：获取本地时间
来源：http://ucq.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ykb.shuidangran.top

[S25] C：内存拷贝
来源：http://jco.daria6918.cn

memcpy(dst, src, n);
来源：http://nqa.xylfe.cn

[S26] C：内存清零
来源：http://nem.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://zfj.0kj1m.cn

[S27] C：定义常量
来源：http://yfl.jqgfzy.top

const double PI = 3.14159;
来源：http://sdz.tian-w.cn

[S28] C：静态变量
来源：http://qkk.0kj1m.cn

static int counter = 0;
来源：http://qew.xziqi.cn

[S29] C：变参函数
来源：http://zaz.hysaishi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pxt.sjlbkw.cn

[S30] C：头文件保护
来源：http://vnm.zhaomingkeji.xyz

#ifndef X_H
来源：http://iuj.nanxuanxn.top

#define X_H
来源：http://pvr.dianchejie.cn

#endif
来源：http://izf.zhongyouzk.top

[S31] C++：Hello World
来源：http://tzj.birdmap.top

#include <iostream>
来源：http://ogx.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://zok.shzxlz.cn

[S32] C++：字符串
来源：http://yxk.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://dbf.yj20258.top

[S33] C++：vector 增删
来源：http://meu.fzhhl.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vqh.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://xpb.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://pth.yfazqb.com

[S35] C++：map
来源：http://avw.sxryk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tqr.andypj.xyz

[S36] C++：unordered_map
来源：http://vbr.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mse.fengsongda.top

[S37] C++：set
来源：http://fnq.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://udy.yj202588.top

[S38] C++：排序
来源：http://zim.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://rgb.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://jgg.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fkf.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://hns.haohaochexian.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ebx.wangshuangyany.cn

[S41] C++：类与构造函数
来源：http://eyy.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kkc.yj20258888.top

[S42] C++：继承与虚函数
来源：http://nmf.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://gmx.fehbvm.com

[S43] C++：智能指针
来源：http://vwu.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://zlc.aizwys.cn

[S44] C++：引用传参
来源：http://ziz.316326.xyz

void inc(int &x) { ++x; }
来源：http://soj.yangfankeji.com

[S45] C++：lambda
来源：http://ixu.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tti.zhoulong.xyz

[S46] C++：函数模板
来源：http://muj.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lnf.hysaishi.cn

[S47] C++：结构化绑定遍历
来源：http://zaj.jinyuanbaomall.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dat.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://gwe.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://dzo.fehbvm.com

while (std::getline(in, line)) { }
来源：http://hwk.wangshuangyany.cn

[S49] C++：写文件
来源：http://dgc.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iuy.sxryk.cn

[S50] C++：格式化数字
来源：http://zaq.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gjf.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://zjj.jiagoushi.top

static_cast<double>(a) / b
来源：http://uqb.nanxinkj.top

[S52] C++：const 与 noexcept
来源：http://ofp.c1oappe.top

int size() const noexcept { return n_; }
来源：http://tac.yanxiufei.cn

[S53] C++：移动语义
来源：http://stv.shanyushiyangtech.top

std::vector<int> w = std::move(v);
来源：http://enu.fehbvm.com

[S54] C++：异常处理
来源：http://tsd.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bak.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://xei.sufxvd.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rns.jianghu66.top

[S56] C++：optional
来源：http://cpn.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://axs.pengpengdd.cyou

[S57] C++：编译期常量
来源：http://nen.havefunace.top

constexpr int N = 10;
来源：http://kkv.hnqzz.top

[S58] C++：命名空间
来源：http://ktl.fktsv.cn

namespace ns { int f() { return 1; } }
来源：http://szg.jiagoushi.top

[S59] C++：静态断言
来源：http://wta.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tlw.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://exn.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jsc.jinghuilouyu.cn

================================================================================
来源：http://gtf.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tdi.yvedp.cn

================================================================================
来源：http://bwf.yj202588.top

[T01] Kotlin：Hello World
来源：http://mqt.tanke756.top

println("Hello")
来源：http://smu.jyoumei.cn

[T02] Kotlin：变量
来源：http://eku.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kfm.ctjpmb.com

[T03] Kotlin：字符串模板
来源：http://emu.jianghu66.top

"值: $b"
来源：http://fwe.zhixingplan.top

[T04] Kotlin：空安全
来源：http://mdf.ehwqpu.com

val n: String? = null;  n?.length
来源：http://wrh.cucudq.cn

[T05] Kotlin：when 表达式
来源：http://pzs.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lgx.uphjek.com

[T06] Kotlin：集合映射
来源：http://tuz.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yfo.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://hjs.hesvh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lgd.cdnleiting.top

[T08] Kotlin：数据类
来源：http://xfj.meibo888.top

data class User(val name: String, val age: Int)
来源：http://dcf.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://phh.daxiang520.top

fun String.exclaim() = this + "!"
来源：http://uxl.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://yin.shanyushiyangtech.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yfj.sxryk.cn

[T11] Kotlin：协程
来源：http://rmp.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ojd.smart0.xyz

[T12] Kotlin：解构声明
来源：http://uer.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://xew.cucudq.cn

[T13] Kotlin：只读 Map
来源：http://xnk.jinghuilouyu.cn

val m = mapOf("a" to 1)
来源：http://wte.xuanzx.com

[T14] Kotlin：循环
来源：http://xlu.yj202588.top

for (i in 1..10) println(i)
来源：http://inx.c1oappe.top

[T15] Kotlin：接口
来源：http://gfo.guannengcc.top

interface Shape { fun area(): Double }
来源：http://uzh.cashguo.top

[T16] Swift：Hello World
来源：http://wkd.tarul.cn

print("Hello")
来源：http://pvy.wangshuangyany.cn

[T17] Swift：变量与常量
来源：http://ghy.hammf.cn

var a = 1;  let b = 2
来源：http://usz.chenlongwang.top

[T18] Swift：字符串插值
来源：http://miz.zycfv.cn

"值: \(b)"
来源：http://bsy.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://mce.aibaodan.cn

if let n = opt { print(n) }
来源：http://kul.hammf.cn

[T20] Swift：数组操作
来源：http://nkm.0kj1m.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ldk.iojbl.cn

[T21] Swift：遍历
来源：http://mgv.epnwcf.com

for x in a { print(x) }
来源：http://qqb.c1oappe.top

[T22] Swift：字典
来源：http://yau.yuanzhike.top

var d = ["a": 1];  d["b"] = 2
来源：http://joc.zhixingplan.top

[T23] Swift：函数
来源：http://qwt.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://azt.zhijiandao.cn

[T24] Swift：闭包
来源：http://zoi.316326.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://aem.ybcxt.top

[T25] Swift：结构体
来源：http://rnk.fanxiaobao.xyz

struct P { var x: Int }
来源：http://vcv.kuanghao11.cn

[T26] Swift：类与重写
来源：http://qcq.ybcxt.top

class A: Base { override func f() {} }
来源：http://uwa.hnxiangtu.top

[T27] Swift：错误处理
来源：http://xdo.yueranfly.top

do { try f() } catch { print(error) }
来源：http://nyh.uphjek.com

[T28] Swift：枚举
来源：http://lba.yonumen.top

enum Color { case red, green }
来源：http://ztc.jqgfzy.top

[T29] Swift：guard 提前返回
来源：http://mns.yonumen.top

guard let x = opt else { return }
来源：http://xxw.ppjwa.cn

[T30] Swift：协议
来源：http://acm.nanxinkj.top

protocol Shape { func area() -> Double }
来源：http://bvh.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://lqu.cashguo.top

print("Hello")
来源：http://hax.yj202588.top

[T32] Lua：局部变量
来源：http://vbc.zdqjudy.top

local a = 1
来源：http://cma.svipenyu.cn

[T33] Lua：表（数组）
来源：http://kss.sxryk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hmm.zycfv.cn

[T34] Lua：遍历表
来源：http://jgq.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://hms.redwolf501.top

[T35] Lua：字典表
来源：http://nal.chenlongwang.top

local d = { a = 1 };  d.b = 2
来源：http://enf.yonumen.top

[T36] Lua：函数
来源：http://aoi.zhijiandao.cn

function add(a, b) return a + b end
来源：http://rwf.gogol.net.cn

[T37] Lua：字符串拼接
来源：http://vrz.yanxiufei.cn

"a" .. "b"
来源：http://otm.fehbvm.com

[T38] Lua：条件
来源：http://ubb.zdbjq.cn

if x > 0 then print("正") end
来源：http://igz.hfpthk.cn

[T39] Lua：模式匹配
来源：http://aln.xuanzx.com

string.find(s, "%d+")
来源：http://gvw.ivvv.top

[T40] Lua：元表
来源：http://fzw.aizwys.cn

setmetatable({}, { __index = base })
来源：http://foe.chenzaomai.com

[T41] Perl：Hello World
来源：http://zon.tian-w.cn

print "Hello\n";
来源：http://vqy.yj20258888.top

[T42] Perl：变量类型
来源：http://yrr.guowangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ect.fktsv.cn

[T43] Perl：字符串插值
来源：http://qdt.mhx1999.top

"值: $a"
来源：http://ves.daria6918.cn

[T44] Perl：条件
来源：http://dny.mhx1999.top

if ($a > 0) { print "正"; }
来源：http://vfm.ctjpmb.com

[T45] Perl：数组遍历
来源：http://bae.epnwcf.com

for my $x (@arr) { print $x; }
来源：http://xsy.daxiang520.top

[T46] Perl：哈希操作
来源：http://bfd.wangdashe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jxl.gaohongyu789.top

[T47] Perl：正则捕获
来源：http://lcl.xingfuxueyuan.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://otp.sweek.top

[T48] Perl：正则替换
来源：http://msp.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://zzh.yfazqb.com

[T49] Perl：函数
来源：http://cmf.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ibx.jiagoushi.top

[T50] Perl：逐行读文件
来源：http://ypl.yj20258.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jme.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://oxc.zhengqikj.top

[T51] Scala：Hello World
来源：http://bhx.chenzaomai.com

println("Hello")
来源：http://gfc.wangshuangyany.cn

[T52] Scala：变量
来源：http://nrv.quarkkingdee.top

val a = 1;  var b = 2
来源：http://cne.bjfxy.top

[T53] Scala：字符串插值
来源：http://smv.tarul.cn

s"值: $b"
来源：http://ktz.snrcjt.cn

[T54] Scala：集合映射
来源：http://nsj.aizwys.cn

List(1, 2, 3).map(_ * 2)
来源：http://mhc.hongshengwenyu.top

[T55] Scala：集合过滤
来源：http://rfl.wangshuangyany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gpi.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://lfe.xuanzx.com


<!-- 参考信息 -->