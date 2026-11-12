代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://igi.hongshengwenyu.top

[R54] 比较两个文件
来源：http://aeo.zhiwuduotai.top

diff a.txt b.txt
来源：http://wkv.fktsv.cn

[R55] 压缩与解压
来源：http://fbk.jlsjyb.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rpg.havefunace.top

[R56] 远程拷贝
来源：http://twm.hongshengwenyu.top

scp file user@host:/path/
来源：http://szc.fzhhl.top

[R57] 远程执行命令
来源：http://kct.svipenyu.cn

ssh user@host 'uptime'
来源：http://wnb.hcnkem.com

[R58] 下载文件
来源：http://zph.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pis.ivvv.top

[R59] 发 POST JSON
来源：http://rbe.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jam.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://eea.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://phd.shangyingyoupin.top

[R61] 磁盘占用
来源：http://rxh.xuetiantiany.cn

df -h;  du -sh *
来源：http://iaj.cdnleiting.top

[R62] 找最占空间的文件
来源：http://cma.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://lrk.pengpengdd.cyou

[R63] 内存与进程
来源：http://aof.yj20258.top

free -h;  ps aux | grep nginx
来源：http://avu.hongshengwenyu.top

[R64] 结束进程
来源：http://vwo.guowangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://apw.ydzc1.top

[R65] 查看端口占用
来源：http://etg.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qub.smart0.xyz

[R66] 定时任务
来源：http://ucx.zdqjudy.top

crontab -e;  crontab -l
来源：http://ybv.uphjek.com

[R67] 生成随机十六进制串
来源：http://wwg.dianchejie.cn

openssl rand -hex 16
来源：http://sao.mhx1999.top

[R68] 计算文件校验值
来源：http://zcd.ydjk.org.cn

sha256sum a.txt;  md5sum a.txt
来源：http://djr.zhongyouzk.top

[R69] 生成随机密码
来源：http://aka.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://mdh.daxiang520.top

[R70] 时间戳与互转
来源：http://thq.c1oappe.top

date +%s;  date -d @1700000000
来源：http://hmv.bjfxy.top

[R71] 日期格式化
来源：http://ymb.yanxiufei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xhx.zhoulong.xyz

[R72] 等待端口就绪
来源：http://eav.jiagoushi.top

until nc -z localhost 3306; do sleep 1; done
来源：http://iie.zhengqikj.top

[R73] 分割大日志
来源：http://fsl.zhijiandao.cn

split -l 1000 big.log part_
来源：http://swe.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://lew.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gjy.ydjk.org.cn

[R75] 导出环境变量
来源：http://zod.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://nyd.cheryme.top

[R76] 使用临时文件
来源：http://ddl.wangshuangyany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://egt.wangshuangyany.cn

[R77] 读取用户输入
来源：http://anf.aizwys.cn

read -rp "请输入: " ans
来源：http://kuz.yj20258888.top

[R78] 交互式菜单
来源：http://ych.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vmz.ydjk.org.cn

[R79] 解析命令行选项
来源：http://wjd.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qdo.cashguo.top

[R80] 查看脚本执行耗时
来源：http://rij.hammf.cn

time ./run.sh
来源：http://sql.guowangkeji.top

================================================================================
来源：http://som.dianchejie.cn

S. C / C++ 专题
来源：http://smr.tarul.cn

================================================================================
来源：http://lec.zdqjudy.top

[S01] C：Hello World
来源：http://ylf.yuxming.cn

#include <stdio.h>
来源：http://kcj.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qcz.epnwcf.com

[S02] C：变量与格式化输出
来源：http://mbu.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://pjo.gzhubu.top

[S03] C：读入整数
来源：http://thv.smart0.xyz

int x; scanf("%d", &x);
来源：http://lpk.gaohongyu789.top

[S04] C：字符串复制
来源：http://hhl.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ntk.bbcook.cn

[S05] C：字符串长度
来源：http://qva.cdnleiting.top

strlen(s)
来源：http://xhm.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://oiq.sweek.top

strcmp(a, b) == 0
来源：http://jgr.hammf.cn

[S07] C：数组遍历求和
来源：http://rwu.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://skz.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://jcb.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jlm.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://urr.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qyk.redwolf501.top

[S10] C：指针与解引用
来源：http://csd.jqgfzy.top

int *p = &a;  *p = 5;
来源：http://kri.wangdashe.top

[S11] C：逐行读文件
来源：http://vui.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://blk.xziqi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ews.chenjidiqi.icu

fclose(f);
来源：http://wol.guowangkeji.top

[S12] C：写文件
来源：http://exz.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zym.tianlin.xyz

[S13] C：宏定义
来源：http://gme.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://psk.yvedp.cn

[S14] C：枚举
来源：http://oya.fengsongda.top

enum Color { RED, GREEN, BLUE };
来源：http://omz.epnwcf.com

[S15] C：类型转换
来源：http://kyw.xuanzx.com

(double) a / b
来源：http://hhr.yuanzhike.top

[S16] C：位操作置位
来源：http://cgn.ppjwa.cn

x |= (1 << 3);
来源：http://dgr.xinyue.icu

[S17] C：安全拼接字符串
来源：http://urp.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ooh.ivvv.top

[S18] C：命令行参数
来源：http://rng.nwbrower.top

int main(int argc, char **argv)
来源：http://cid.sysykeji.top

[S19] C：快速排序
来源：http://cnf.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://efn.hnqzz.top

[S20] C：二分查找
来源：http://bhy.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ldg.jianghu66.top

[S21] C：字符类别判断
来源：http://dmw.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ipb.bbcook.cn

[S22] C：字符串转数字
来源：http://ijv.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://isn.shanyushiyangkeji.top

[S23] C：随机数
来源：http://rnp.jinghuilouyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://phy.yvedp.cn

[S24] C：获取本地时间
来源：http://lel.sweek.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cbe.tanke756.top

[S25] C：内存拷贝
来源：http://bfz.zhiwuduotai.top

memcpy(dst, src, n);
来源：http://obs.bbcook.cn

[S26] C：内存清零
来源：http://kmc.nanxuanxn.top

memset(a, 0, sizeof a);
来源：http://opc.yj20258888.top

[S27] C：定义常量
来源：http://jcz.meibo888.top

const double PI = 3.14159;
来源：http://kfs.guannengcc.top

[S28] C：静态变量
来源：http://tgh.tianlin.xyz

static int counter = 0;
来源：http://mvh.zdbjq.cn

[S29] C：变参函数
来源：http://vua.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uor.uphjek.com

[S30] C：头文件保护
来源：http://tjc.jinyuanbaomall.cn

#ifndef X_H
来源：http://huh.hammf.cn

#define X_H
来源：http://ljb.bjfxy.top

#endif
来源：http://kxl.shanyushiyangtech.top

[S31] C++：Hello World
来源：http://oyx.yj202588.top

#include <iostream>
来源：http://hgp.jqgfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://rng.52xcode.cn

[S32] C++：字符串
来源：http://fra.tarul.cn

std::string s = "hi";  s += "!";
来源：http://pgt.kuanghao11.cn

[S33] C++：vector 增删
来源：http://njl.gogol.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ryq.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://pma.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://iix.fktsv.cn

[S35] C++：map
来源：http://lcg.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fhp.ppjwa.cn

[S36] C++：unordered_map
来源：http://fdo.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iad.yuxming.cn

[S37] C++：set
来源：http://nor.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kbw.yonumen.top

[S38] C++：排序
来源：http://uax.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://ajh.nwbrower.top

[S39] C++：自定义比较器排序
来源：http://rjf.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zzx.tanke756.top

[S40] C++：查找元素
来源：http://gdf.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fcb.xylfe.cn

[S41] C++：类与构造函数
来源：http://cua.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://btb.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://wcz.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://qlo.gotoacloud.top

[S43] C++：智能指针
来源：http://jew.hongshengwenyu.top

auto p = std::make_unique<int>(5);
来源：http://kpo.9152youxi.cn

[S44] C++：引用传参
来源：http://yvs.nwbrower.top

void inc(int &x) { ++x; }
来源：http://dxr.xylfe.cn

[S45] C++：lambda
来源：http://lit.yonumen.top

auto add = [](int a, int b) { return a + b; };
来源：http://bpq.nwbrower.top

[S46] C++：函数模板
来源：http://meu.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ctu.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://hmk.yj202588.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://azv.chenlongwang.top

[S48] C++：逐行读文件
来源：http://zsl.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kjj.jinyuanbaomall.cn

while (std::getline(in, line)) { }
来源：http://uxn.hysaishi.cn

[S49] C++：写文件
来源：http://kfx.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iog.svipenyu.cn

[S50] C++：格式化数字
来源：http://ecq.gaohongyu789.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://njm.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://flr.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://upj.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://wsy.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://xvy.sjlbkw.cn

[S53] C++：移动语义
来源：http://oaf.yj20258.top

std::vector<int> w = std::move(v);
来源：http://lqu.yangfankeji.com

[S54] C++：异常处理
来源：http://qgg.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qrl.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://dwp.havefunace.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jbx.jinghuilouyu.cn

[S56] C++：optional
来源：http://zwf.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gsr.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://ssw.tianlin.xyz

constexpr int N = 10;
来源：http://lll.tarul.cn

[S58] C++：命名空间
来源：http://scd.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://fiu.shzxlz.cn

[S59] C++：静态断言
来源：http://yuc.yuanzhike.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kwk.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://lxi.andypj.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ggt.ctjpmb.com

================================================================================
来源：http://evc.ybcxt.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jip.zhiwuduotai.top

================================================================================
来源：http://jfp.xylfe.cn

[T01] Kotlin：Hello World
来源：http://ygw.hesvh.cn

println("Hello")
来源：http://ljo.shanyushiyangkeji.top

[T02] Kotlin：变量
来源：http://qof.havefunace.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uyh.yfazqb.com

[T03] Kotlin：字符串模板
来源：http://gvz.jinqigfzy.top

"值: $b"
来源：http://mpu.jyoumei.cn

[T04] Kotlin：空安全
来源：http://dwu.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://vjj.dashuyun.cn

[T05] Kotlin：when 表达式
来源：http://kyg.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cwc.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://wsz.pycfn.com

listOf(1, 2, 3).map { it * 2 }
来源：http://syp.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://rcw.tianlin.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://gxs.bjfxy.top

[T08] Kotlin：数据类
来源：http://gma.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://stx.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://qoz.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://ruo.xziqi.cn

[T10] Kotlin：默认参数
来源：http://itq.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fnz.tanke756.top

[T11] Kotlin：协程
来源：http://rko.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gyn.fzhhl.top

[T12] Kotlin：解构声明
来源：http://qrb.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://fic.shanyushiyangtech.top

[T13] Kotlin：只读 Map
来源：http://zyf.c1oappe.top

val m = mapOf("a" to 1)
来源：http://ueb.pengpengdd.cyou

[T14] Kotlin：循环
来源：http://zlk.dianchejie.cn

for (i in 1..10) println(i)
来源：http://jue.bbcook.cn

[T15] Kotlin：接口
来源：http://jkb.fehbvm.com

interface Shape { fun area(): Double }
来源：http://sux.haohaochexian.top

[T16] Swift：Hello World
来源：http://chb.yongpay.top

print("Hello")
来源：http://wsk.hywenlv.cn

[T17] Swift：变量与常量
来源：http://wmj.vqdsnc.cn

var a = 1;  let b = 2
来源：http://dvy.vehdjk.com

[T18] Swift：字符串插值
来源：http://gur.zdqjudy.top

"值: \(b)"
来源：http://mnk.svipenyu.cn

[T19] Swift：可选绑定
来源：http://gpb.quarkkingdee.top

if let n = opt { print(n) }
来源：http://dul.smart0.xyz

[T20] Swift：数组操作
来源：http://nco.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://xxe.xziqi.cn

[T21] Swift：遍历
来源：http://gfx.ehwqpu.com

for x in a { print(x) }
来源：http://wrd.chenzaomai.com

[T22] Swift：字典
来源：http://gwu.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://mnt.tanke756.top

[T23] Swift：函数
来源：http://gho.hnqzz.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gyo.hnxiangtu.top

[T24] Swift：闭包
来源：http://guv.guowangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qyn.wangdashe.top

[T25] Swift：结构体
来源：http://qjd.bbcook.cn

struct P { var x: Int }
来源：http://wkn.snrcjt.cn

[T26] Swift：类与重写
来源：http://rvf.zdbjq.cn

class A: Base { override func f() {} }
来源：http://btm.vqdsnc.cn

[T27] Swift：错误处理
来源：http://ypk.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://org.daxiang520.top

[T28] Swift：枚举
来源：http://cev.uphjek.com

enum Color { case red, green }
来源：http://bom.ydjk.org.cn

[T29] Swift：guard 提前返回
来源：http://brc.feifeiyinyue.top

guard let x = opt else { return }
来源：http://wlz.bjfxy.top

[T30] Swift：协议
来源：http://izb.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://ynl.yangfankeji.com

[T31] Lua：Hello World
来源：http://pjq.zdbjq.cn

print("Hello")
来源：http://tdb.wangdashe.top

[T32] Lua：局部变量
来源：http://mqw.gzhubu.top

local a = 1
来源：http://gza.zhiwuduotai.top

[T33] Lua：表（数组）
来源：http://tbv.nwbrower.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nst.quarkkingdee.top

[T34] Lua：遍历表
来源：http://rbi.chenlongwang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vsw.hywenlv.cn

[T35] Lua：字典表
来源：http://frs.shuidangran.top

local d = { a = 1 };  d.b = 2
来源：http://kzw.jiagoushi.top

[T36] Lua：函数
来源：http://gej.gotoacloud.top

function add(a, b) return a + b end
来源：http://wxd.jinghuilouyu.cn

[T37] Lua：字符串拼接
来源：http://fpc.guannengcc.top

"a" .. "b"
来源：http://aqn.zhengqikj.top

[T38] Lua：条件
来源：http://fwv.svipenyu.cn

if x > 0 then print("正") end
来源：http://ayw.hcnkem.com

[T39] Lua：模式匹配
来源：http://rig.zdqjudy.top

string.find(s, "%d+")
来源：http://rpb.vqdsnc.cn

[T40] Lua：元表
来源：http://zaa.zdqjudy.top

setmetatable({}, { __index = base })
来源：http://uvb.fehbvm.com

[T41] Perl：Hello World
来源：http://jhn.0kj1m.cn

print "Hello\n";
来源：http://jaf.meibo888.top

[T42] Perl：变量类型
来源：http://odw.zdbjq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bfx.xziqi.cn

[T43] Perl：字符串插值
来源：http://dtc.aibaodan.cn

"值: $a"
来源：http://rut.cucudq.cn

[T44] Perl：条件
来源：http://wdr.iojbl.cn

if ($a > 0) { print "正"; }
来源：http://pir.havefunace.top

[T45] Perl：数组遍历
来源：http://ait.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://jue.tianlin.xyz

[T46] Perl：哈希操作
来源：http://qwm.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ilq.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://xgh.ydzc1.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ptf.redwolf501.top

[T48] Perl：正则替换
来源：http://tqd.c1oappe.top

$s =~ s/old/new/g;
来源：http://yaz.hongshengwenyu.top

[T49] Perl：函数
来源：http://hsw.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uaa.ydzc1.top

[T50] Perl：逐行读文件
来源：http://lwp.hywenlv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hxf.ppjwa.cn

while (my $line = <$fh>) { print $line; }
来源：http://vct.zhaomingkeji.xyz

[T51] Scala：Hello World
来源：http://yul.cqqwz.cn

println("Hello")
来源：http://vwz.uphjek.com

[T52] Scala：变量
来源：http://eff.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://mcs.hysaishi.cn

[T53] Scala：字符串插值
来源：http://ivj.xinyue.icu

s"值: $b"
来源：http://dtc.haohaochexian.top

[T54] Scala：集合映射
来源：http://eyu.sysykeji.top

List(1, 2, 3).map(_ * 2)
来源：http://coz.316326.xyz

[T55] Scala：集合过滤
来源：http://yok.kuanghao11.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pvt.dashuyun.cn

[T56] Scala：样例类
来源：http://ogq.smart0.xyz


<!-- 参考信息 -->