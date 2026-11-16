代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://vfa.ywan-chungtsiang.top

[R48] awk 取指定列
来源：http://pds.zhaomingkeji.xyz

awk '{print $1, $3}' a.txt
来源：http://uou.vqdsnc.cn

[R49] awk 带条件
来源：http://fhw.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dgi.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://lrl.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://khr.fzhhl.top

[R51] 排序去重取前几
来源：http://ejr.shuidangran.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vej.316326.xyz

[R52] 统计行数
来源：http://kdp.fzhhl.top

wc -l a.txt
来源：http://dlm.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://tsp.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mhh.pengpengdd.cyou

[R54] 比较两个文件
来源：http://vir.gotoacloud.top

diff a.txt b.txt
来源：http://qia.aizwys.cn

[R55] 压缩与解压
来源：http://clp.wangshuangyany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ehi.hnqzz.top

[R56] 远程拷贝
来源：http://fue.chenlongwang.top

scp file user@host:/path/
来源：http://eok.fktsv.cn

[R57] 远程执行命令
来源：http://ouz.nanxuanxn.top

ssh user@host 'uptime'
来源：http://yxe.daxiang520.top

[R58] 下载文件
来源：http://use.meibo888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://erb.52xcode.cn

[R59] 发 POST JSON
来源：http://dho.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qkj.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://cso.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cib.pengpengdd.cyou

[R61] 磁盘占用
来源：http://sqx.vqdsnc.cn

df -h;  du -sh *
来源：http://lot.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://vop.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://zuc.hammf.cn

[R63] 内存与进程
来源：http://hdd.jiagoushi.top

free -h;  ps aux | grep nginx
来源：http://adm.yj202588.top

[R64] 结束进程
来源：http://hog.vqdsnc.cn

kill -9 $(pgrep -f app.py)
来源：http://dag.chenjidiqi.icu

[R65] 查看端口占用
来源：http://xzl.hammf.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rar.sufxvd.cn

[R66] 定时任务
来源：http://pnf.xingfuxueyuan.xyz

crontab -e;  crontab -l
来源：http://fju.shuidangran.top

[R67] 生成随机十六进制串
来源：http://fgo.vehdjk.com

openssl rand -hex 16
来源：http://pll.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://swr.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cwn.zhongyouzk.top

[R69] 生成随机密码
来源：http://aaa.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://mxh.ppjwa.cn

[R70] 时间戳与互转
来源：http://avz.hnqzz.top

date +%s;  date -d @1700000000
来源：http://ioz.sweek.top

[R71] 日期格式化
来源：http://akx.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cne.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://ugw.hesvh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fmh.ivvv.top

[R73] 分割大日志
来源：http://idr.mhx1999.top

split -l 1000 big.log part_
来源：http://lpu.gzhubu.top

[R74] 批量重命名
来源：http://edb.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://trb.mhx1999.top

[R75] 导出环境变量
来源：http://qgz.sysykeji.top

export PATH="$HOME/bin:$PATH"
来源：http://wgq.zhijiandao.cn

[R76] 使用临时文件
来源：http://aos.yuxming.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fud.sysykeji.top

[R77] 读取用户输入
来源：http://umx.chenlongwang.top

read -rp "请输入: " ans
来源：http://lmq.shzxlz.cn

[R78] 交互式菜单
来源：http://bmr.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://amd.tarul.cn

[R79] 解析命令行选项
来源：http://qng.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lls.sxryk.cn

[R80] 查看脚本执行耗时
来源：http://yrz.zhoulong.xyz

time ./run.sh
来源：http://ilg.chenjidiqi.icu

================================================================================
来源：http://xds.0kj1m.cn

S. C / C++ 专题
来源：http://wrk.zhixingplan.top

================================================================================
来源：http://uqo.jqgfzy.top

[S01] C：Hello World
来源：http://wle.yueranfly.top

#include <stdio.h>
来源：http://ycd.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://jhr.xziqi.cn

[S02] C：变量与格式化输出
来源：http://roh.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://tuv.jiagoushi.top

[S03] C：读入整数
来源：http://vsu.zhaomingkeji.xyz

int x; scanf("%d", &x);
来源：http://ieq.meibo888.top

[S04] C：字符串复制
来源：http://iqn.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iwf.zdbjq.cn

[S05] C：字符串长度
来源：http://ldf.shzxlz.cn

strlen(s)
来源：http://iwi.nanxinkj.top

[S06] C：字符串比较
来源：http://tmg.gogol.net.cn

strcmp(a, b) == 0
来源：http://blg.zdbjq.cn

[S07] C：数组遍历求和
来源：http://imt.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yyb.sweek.top

[S08] C：动态内存分配与释放
来源：http://jik.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://udk.hnqzz.top

[S09] C：结构体定义与初始化
来源：http://eeq.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bjq.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://pkj.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://fhb.gotoacloud.top

[S11] C：逐行读文件
来源：http://qfm.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://wdg.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://upa.nwbrower.top

fclose(f);
来源：http://qbc.shzxlz.cn

[S12] C：写文件
来源：http://wsn.gzhubu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uuy.shanyushiyangtech.top

[S13] C：宏定义
来源：http://pes.cashguo.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rrh.redwolf501.top

[S14] C：枚举
来源：http://ags.ywan-chungtsiang.top

enum Color { RED, GREEN, BLUE };
来源：http://uzf.gzhubu.top

[S15] C：类型转换
来源：http://xrl.bbcook.cn

(double) a / b
来源：http://dfv.bbcook.cn

[S16] C：位操作置位
来源：http://ear.svipenyu.cn

x |= (1 << 3);
来源：http://kzy.tanke756.top

[S17] C：安全拼接字符串
来源：http://tko.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://edl.chenlongwang.top

[S18] C：命令行参数
来源：http://dgp.sxryk.cn

int main(int argc, char **argv)
来源：http://dtu.zycfv.cn

[S19] C：快速排序
来源：http://dsj.ybcxt.top

qsort(a, n, sizeof(int), cmp);
来源：http://yli.andypj.xyz

[S20] C：二分查找
来源：http://fiv.xylfe.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://stj.chenlongwang.top

[S21] C：字符类别判断
来源：http://pif.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qek.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://dez.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bij.jyoumei.cn

[S23] C：随机数
来源：http://mag.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mnz.c1oappe.top

[S24] C：获取本地时间
来源：http://teg.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zjv.hnqzz.top

[S25] C：内存拷贝
来源：http://fhu.wangshuangyany.cn

memcpy(dst, src, n);
来源：http://yxm.316326.xyz

[S26] C：内存清零
来源：http://rwg.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://zso.hywenlv.cn

[S27] C：定义常量
来源：http://aul.hywenlv.cn

const double PI = 3.14159;
来源：http://rvp.xuanzx.com

[S28] C：静态变量
来源：http://gxq.haohaochexian.top

static int counter = 0;
来源：http://dov.meibo888.top

[S29] C：变参函数
来源：http://pmy.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gcw.feifeiyinyue.top

[S30] C：头文件保护
来源：http://csf.yj20258.top

#ifndef X_H
来源：http://qtg.iojbl.cn

#define X_H
来源：http://bab.ydzc1.top

#endif
来源：http://rwj.fehbvm.com

[S31] C++：Hello World
来源：http://hub.mhx1999.top

#include <iostream>
来源：http://aww.nanxuanxn.top

int main() { std::cout << "Hello\n"; }
来源：http://ivs.tianlin.xyz

[S32] C++：字符串
来源：http://tww.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://kbe.fehbvm.com

[S33] C++：vector 增删
来源：http://rbd.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zve.gaohongyu789.top

[S34] C++：遍历 vector
来源：http://thh.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://vuh.zycfv.cn

[S35] C++：map
来源：http://iqy.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vuk.xuetiantiany.cn

[S36] C++：unordered_map
来源：http://pkc.snrcjt.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lgj.cucudq.cn

[S37] C++：set
来源：http://hnr.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tpr.quarkkingdee.top

[S38] C++：排序
来源：http://xvp.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://mki.yongpay.top

[S39] C++：自定义比较器排序
来源：http://tns.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://khj.guowangkeji.top

[S40] C++：查找元素
来源：http://nyt.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://usg.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://zdb.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hpg.hcnkem.com

[S42] C++：继承与虚函数
来源：http://eur.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://lay.dashuyun.cn

[S43] C++：智能指针
来源：http://fux.fzhhl.top

auto p = std::make_unique<int>(5);
来源：http://iak.ctjpmb.com

[S44] C++：引用传参
来源：http://zwx.dianchejie.cn

void inc(int &x) { ++x; }
来源：http://ayn.pengpengdd.cyou

[S45] C++：lambda
来源：http://trr.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://kag.tianlin.xyz

[S46] C++：函数模板
来源：http://pmq.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yay.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://idq.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bzw.xylfe.cn

[S48] C++：逐行读文件
来源：http://nqi.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://zpp.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://efr.tarul.cn

[S49] C++：写文件
来源：http://ico.gzhubu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xso.cqqwz.cn

[S50] C++：格式化数字
来源：http://jzc.pycfn.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://icw.sysykeji.top

[S51] C++：显式类型转换
来源：http://ehx.hammf.cn

static_cast<double>(a) / b
来源：http://idp.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://yyn.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://sqb.52xcode.cn

[S53] C++：移动语义
来源：http://oak.zdqjudy.top

std::vector<int> w = std::move(v);
来源：http://jti.zdbjq.cn

[S54] C++：异常处理
来源：http://whv.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cdx.sufxvd.cn

[S55] C++：结构化绑定
来源：http://sfi.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ljn.yueranfly.top

[S56] C++：optional
来源：http://ywr.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gcx.sweek.top

[S57] C++：编译期常量
来源：http://uou.bjfxy.top

constexpr int N = 10;
来源：http://ikv.chenjidiqi.icu

[S58] C++：命名空间
来源：http://qjr.zhoulong.xyz

namespace ns { int f() { return 1; } }
来源：http://lat.gogol.net.cn

[S59] C++：静态断言
来源：http://voi.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bwx.shanyushiyangtech.top

[S60] C++：遍历并删除元素
来源：http://wki.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iqc.xingfuxueyuan.xyz

================================================================================
来源：http://lsu.tarul.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mkw.xziqi.cn

================================================================================
来源：http://epl.ywan-chungtsiang.top

[T01] Kotlin：Hello World
来源：http://xoj.bjfxy.top

println("Hello")
来源：http://gsu.fehbvm.com

[T02] Kotlin：变量
来源：http://uvd.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yfl.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://pvf.ivvv.top

"值: $b"
来源：http://hfx.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://zep.yuanzhike.top

val n: String? = null;  n?.length
来源：http://tir.pycfn.com

[T05] Kotlin：when 表达式
来源：http://duc.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tbh.316326.xyz

[T06] Kotlin：集合映射
来源：http://tof.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://urn.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://viy.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xka.fktsv.cn

[T08] Kotlin：数据类
来源：http://peu.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://cmc.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://ncb.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://eyv.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://dox.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://zwc.cashguo.top

[T11] Kotlin：协程
来源：http://axm.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://anx.jinqigufen.top

[T12] Kotlin：解构声明
来源：http://ypk.bjfxy.top

val (a, b) = Pair(1, 2)
来源：http://xyr.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://hrb.chenlongwang.top

val m = mapOf("a" to 1)
来源：http://unm.hfpthk.cn

[T14] Kotlin：循环
来源：http://xkn.shzxlz.cn

for (i in 1..10) println(i)
来源：http://sws.tanke756.top

[T15] Kotlin：接口
来源：http://bjz.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://fmg.tianlin.xyz

[T16] Swift：Hello World
来源：http://adk.havefunace.top

print("Hello")
来源：http://fwp.svipenyu.cn

[T17] Swift：变量与常量
来源：http://yfi.yj20258888.top

var a = 1;  let b = 2
来源：http://udv.bbcook.cn

[T18] Swift：字符串插值
来源：http://nnq.nanxinkj.top

"值: \(b)"
来源：http://led.jianghu66.top

[T19] Swift：可选绑定
来源：http://goe.jqgfzy.top

if let n = opt { print(n) }
来源：http://hsc.zhijiandao.cn

[T20] Swift：数组操作
来源：http://ymw.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mlo.zhongyouzk.top

[T21] Swift：遍历
来源：http://gfq.yanxiufei.cn

for x in a { print(x) }
来源：http://bje.ivvv.top

[T22] Swift：字典
来源：http://quv.yuxming.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pok.redwolf501.top

[T23] Swift：函数
来源：http://roe.ybcxt.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lhl.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://chd.kuanghao11.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cje.gotoacloud.top

[T25] Swift：结构体
来源：http://ptx.hysaishi.cn

struct P { var x: Int }
来源：http://vxd.zycfv.cn

[T26] Swift：类与重写
来源：http://juo.shanyushiyangtech.top

class A: Base { override func f() {} }
来源：http://szg.cdnleiting.top

[T27] Swift：错误处理
来源：http://gtp.yvedp.cn

do { try f() } catch { print(error) }
来源：http://rup.shanyushiyangtech.top

[T28] Swift：枚举
来源：http://ggp.jqgfzy.top

enum Color { case red, green }
来源：http://ynt.pycfn.com

[T29] Swift：guard 提前返回
来源：http://buw.tian-w.cn

guard let x = opt else { return }
来源：http://kfr.cashguo.top

[T30] Swift：协议
来源：http://xij.jinqigfzy.top

protocol Shape { func area() -> Double }
来源：http://cwb.hammf.cn

[T31] Lua：Hello World
来源：http://nyn.yvedp.cn

print("Hello")
来源：http://gdk.ivvv.top

[T32] Lua：局部变量
来源：http://qfd.ivvv.top

local a = 1
来源：http://gsb.hfpthk.cn

[T33] Lua：表（数组）
来源：http://yod.gaohongyu789.top

local t = {1, 2, 3};  t[4] = 4
来源：http://yab.gogol.net.cn

[T34] Lua：遍历表
来源：http://ovm.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eyw.jyoumei.cn

[T35] Lua：字典表
来源：http://fqb.andypj.xyz

local d = { a = 1 };  d.b = 2
来源：http://feb.yfazqb.com

[T36] Lua：函数
来源：http://rxs.fengsongda.top

function add(a, b) return a + b end
来源：http://wnr.haohaochexian.top

[T37] Lua：字符串拼接
来源：http://fhg.hfpthk.cn

"a" .. "b"
来源：http://vrn.epnwcf.com

[T38] Lua：条件
来源：http://mja.jqgufenzy.top

if x > 0 then print("正") end
来源：http://gtk.sweek.top

[T39] Lua：模式匹配
来源：http://hiq.pengpengdd.cyou

string.find(s, "%d+")
来源：http://alg.wangshuangyany.cn

[T40] Lua：元表
来源：http://wuu.sufxvd.cn

setmetatable({}, { __index = base })
来源：http://ajn.ctjpmb.com

[T41] Perl：Hello World
来源：http://csd.snrcjt.cn

print "Hello\n";
来源：http://lni.zhijiandao.cn

[T42] Perl：变量类型
来源：http://yry.dashuyun.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://czn.sxryk.cn

[T43] Perl：字符串插值
来源：http://joo.jqgufenzy.top

"值: $a"
来源：http://cfb.pengpengdd.cyou

[T44] Perl：条件
来源：http://slr.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://cyq.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://zxz.fehbvm.com

for my $x (@arr) { print $x; }
来源：http://wfw.jiagoushi.top

[T46] Perl：哈希操作
来源：http://xpo.yfazqb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://veu.hywenlv.cn

[T47] Perl：正则捕获
来源：http://wrg.feifeiyinyue.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pup.chenjidiqi.icu

[T48] Perl：正则替换
来源：http://juq.tian-w.cn

$s =~ s/old/new/g;
来源：http://bai.guannengcc.top

[T49] Perl：函数
来源：http://iue.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lta.daxiang520.top

[T50] Perl：逐行读文件
来源：http://smf.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xyd.guannengcc.top


<!-- 参考信息 -->