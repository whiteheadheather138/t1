代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://plw.hnxiangtu.top

[R56] 远程拷贝
来源：http://nbk.shanyushiyangkeji.top

scp file user@host:/path/
来源：http://dbo.cucudq.cn

[R57] 远程执行命令
来源：http://phy.zdbjq.cn

ssh user@host 'uptime'
来源：http://tmd.sxryk.cn

[R58] 下载文件
来源：http://ucu.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wir.haohaochexian.top

[R59] 发 POST JSON
来源：http://fqz.ywan-chungtsiang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zfj.epnwcf.com

[R60] 只看 HTTP 状态码
来源：http://rln.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ejm.gogol.net.cn

[R61] 磁盘占用
来源：http://ryd.chenzaomai.com

df -h;  du -sh *
来源：http://dyj.iojbl.cn

[R62] 找最占空间的文件
来源：http://lkm.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://ukj.hesvh.cn

[R63] 内存与进程
来源：http://rvi.yj20258.top

free -h;  ps aux | grep nginx
来源：http://fck.hesvh.cn

[R64] 结束进程
来源：http://jry.sweek.top

kill -9 $(pgrep -f app.py)
来源：http://odh.andypj.xyz

[R65] 查看端口占用
来源：http://egt.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yvk.52xcode.cn

[R66] 定时任务
来源：http://ueg.yuxming.cn

crontab -e;  crontab -l
来源：http://cvj.c1oappe.top

[R67] 生成随机十六进制串
来源：http://toi.shzxlz.cn

openssl rand -hex 16
来源：http://gbc.zycfv.cn

[R68] 计算文件校验值
来源：http://obi.zhaomingkeji.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://wya.ywan-chungtsiang.top

[R69] 生成随机密码
来源：http://eib.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://vjt.zhoulong.xyz

[R70] 时间戳与互转
来源：http://awy.tanke756.top

date +%s;  date -d @1700000000
来源：http://wau.jinqigfzy.top

[R71] 日期格式化
来源：http://pdm.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ubt.vehdjk.com

[R72] 等待端口就绪
来源：http://cmt.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://ihd.guannengcc.top

[R73] 分割大日志
来源：http://imw.hesvh.cn

split -l 1000 big.log part_
来源：http://dry.gotoacloud.top

[R74] 批量重命名
来源：http://rhi.dashuyun.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oyz.jqgfzy.top

[R75] 导出环境变量
来源：http://lnx.zycfv.cn

export PATH="$HOME/bin:$PATH"
来源：http://nei.zdqjudy.top

[R76] 使用临时文件
来源：http://teo.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ugp.wangshuangyany.cn

[R77] 读取用户输入
来源：http://cfl.zdqjudy.top

read -rp "请输入: " ans
来源：http://fhf.c1oappe.top

[R78] 交互式菜单
来源：http://ojc.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://don.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://ett.snrcjt.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rtp.yj20258.top

[R80] 查看脚本执行耗时
来源：http://ldw.9152youxi.cn

time ./run.sh
来源：http://cnc.zhongyouzk.top

================================================================================
来源：http://ypo.chenlongwang.top

S. C / C++ 专题
来源：http://pzu.gaohongyu789.top

================================================================================
来源：http://rfn.svipenyu.cn

[S01] C：Hello World
来源：http://fnd.yj202588.top

#include <stdio.h>
来源：http://hjt.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xit.hcnkem.com

[S02] C：变量与格式化输出
来源：http://bfg.gotoacloud.top

int a = 10; printf("%d\n", a);
来源：http://vwk.yanxiufei.cn

[S03] C：读入整数
来源：http://rsi.jinghuilouyu.cn

int x; scanf("%d", &x);
来源：http://oxp.nwbrower.top

[S04] C：字符串复制
来源：http://qei.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oun.yj20258.top

[S05] C：字符串长度
来源：http://lko.gogol.net.cn

strlen(s)
来源：http://npm.cdnleiting.top

[S06] C：字符串比较
来源：http://rcm.bjfxy.top

strcmp(a, b) == 0
来源：http://qqg.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://gsj.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bsw.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://egl.uphjek.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ulp.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://uld.gaohongyu789.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pvr.snrcjt.cn

[S10] C：指针与解引用
来源：http://qvr.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://nvf.316326.xyz

[S11] C：逐行读文件
来源：http://lgm.jiagoushi.top

FILE *f = fopen("a.txt", "r");
来源：http://ywy.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xjc.andypj.xyz

fclose(f);
来源：http://wzf.nanxinkj.top

[S12] C：写文件
来源：http://jdx.dashuyun.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uzk.shangyingyoupin.top

[S13] C：宏定义
来源：http://ihn.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rud.yuxming.cn

[S14] C：枚举
来源：http://pyq.fengsongda.top

enum Color { RED, GREEN, BLUE };
来源：http://zgz.fehbvm.com

[S15] C：类型转换
来源：http://ayf.hnxiangtu.top

(double) a / b
来源：http://mbz.wangshuangyany.cn

[S16] C：位操作置位
来源：http://uer.tarul.cn

x |= (1 << 3);
来源：http://avx.52xcode.cn

[S17] C：安全拼接字符串
来源：http://yva.dianchejie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sbm.nanxuanxn.top

[S18] C：命令行参数
来源：http://pil.ehwqpu.com

int main(int argc, char **argv)
来源：http://qoy.snrcjt.cn

[S19] C：快速排序
来源：http://rrr.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fou.gogol.net.cn

[S20] C：二分查找
来源：http://yax.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xpo.cheryme.top

[S21] C：字符类别判断
来源：http://zvy.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xse.meibo888.top

[S22] C：字符串转数字
来源：http://pje.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://lzo.zhoulong.xyz

[S23] C：随机数
来源：http://cjy.shuidangran.top

srand(time(NULL));  int r = rand() % 100;
来源：http://esh.aibaodan.cn

[S24] C：获取本地时间
来源：http://tjd.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ncw.epnwcf.com

[S25] C：内存拷贝
来源：http://wkr.fzhhl.top

memcpy(dst, src, n);
来源：http://exp.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://xof.epnwcf.com

memset(a, 0, sizeof a);
来源：http://zoj.gogol.net.cn

[S27] C：定义常量
来源：http://olv.fehbvm.com

const double PI = 3.14159;
来源：http://dga.ybcxt.top

[S28] C：静态变量
来源：http://nnp.hywenlv.cn

static int counter = 0;
来源：http://jql.pengpengdd.cyou

[S29] C：变参函数
来源：http://ewr.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://srn.nanxinkj.top

[S30] C：头文件保护
来源：http://tnc.jinyuanbaomall.cn

#ifndef X_H
来源：http://gng.wangdashe.top

#define X_H
来源：http://hsu.yueranfly.top

#endif
来源：http://xba.cashguo.top

[S31] C++：Hello World
来源：http://xvu.yfazqb.com

#include <iostream>
来源：http://cce.birdmap.top

int main() { std::cout << "Hello\n"; }
来源：http://wpe.sysykeji.top

[S32] C++：字符串
来源：http://xyi.hnxiangtu.top

std::string s = "hi";  s += "!";
来源：http://caa.tian-w.cn

[S33] C++：vector 增删
来源：http://uus.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cyj.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://qqv.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://lnd.shangyingyoupin.top

[S35] C++：map
来源：http://cef.xylfe.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ldv.andypj.xyz

[S36] C++：unordered_map
来源：http://vol.pycfn.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hqw.chenjidiqi.icu

[S37] C++：set
来源：http://bti.xingfuxueyuan.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mej.xuanzx.com

[S38] C++：排序
来源：http://xlc.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://llk.bjfxy.top

[S39] C++：自定义比较器排序
来源：http://lsw.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dnw.gotoacloud.top

[S40] C++：查找元素
来源：http://kvk.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xfz.shzxlz.cn

[S41] C++：类与构造函数
来源：http://pnw.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vhu.yvedp.cn

[S42] C++：继承与虚函数
来源：http://kol.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://nef.pycfn.com

[S43] C++：智能指针
来源：http://hxh.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://shr.yj20258888.top

[S44] C++：引用传参
来源：http://ucu.yj20258888.top

void inc(int &x) { ++x; }
来源：http://skm.guowangkeji.top

[S45] C++：lambda
来源：http://pht.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://nzh.fengsongda.top

[S46] C++：函数模板
来源：http://zuo.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://exh.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://wui.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jlc.yuanzhike.top

[S48] C++：逐行读文件
来源：http://owl.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://sqj.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://ikb.shuidangran.top

[S49] C++：写文件
来源：http://wwe.bjfxy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cbd.feifeiyinyue.top

[S50] C++：格式化数字
来源：http://nlc.zhengqikj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cel.hesvh.cn

[S51] C++：显式类型转换
来源：http://vli.cucudq.cn

static_cast<double>(a) / b
来源：http://gsw.shanyushiyangtech.top

[S52] C++：const 与 noexcept
来源：http://hbj.meibo888.top

int size() const noexcept { return n_; }
来源：http://zfb.yuanzhike.top

[S53] C++：移动语义
来源：http://ahu.cucudq.cn

std::vector<int> w = std::move(v);
来源：http://gca.fktsv.cn

[S54] C++：异常处理
来源：http://acu.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bko.zdqjudy.top

[S55] C++：结构化绑定
来源：http://nio.guowangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cte.hammf.cn

[S56] C++：optional
来源：http://esx.vehdjk.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ipr.yueranfly.top

[S57] C++：编译期常量
来源：http://djl.yj202588.top

constexpr int N = 10;
来源：http://waf.hnqzz.top

[S58] C++：命名空间
来源：http://mvd.chenjidiqi.icu

namespace ns { int f() { return 1; } }
来源：http://rrc.9152youxi.cn

[S59] C++：静态断言
来源：http://mxd.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kbf.zhijiandao.cn

[S60] C++：遍历并删除元素
来源：http://cxh.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sac.ywan-chungtsiang.top

================================================================================
来源：http://ynf.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xip.jinyuanbaomall.cn

================================================================================
来源：http://zqd.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://nht.dashuyun.cn

println("Hello")
来源：http://qvc.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://sim.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wve.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://yki.shuidangran.top

"值: $b"
来源：http://amu.jiagoushi.top

[T04] Kotlin：空安全
来源：http://uyk.shzxlz.cn

val n: String? = null;  n?.length
来源：http://boj.cheryme.top

[T05] Kotlin：when 表达式
来源：http://lzx.yanxiufei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cpv.pycfn.com

[T06] Kotlin：集合映射
来源：http://iyr.hammf.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xvi.52xcode.cn

[T07] Kotlin：集合过滤
来源：http://ikf.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wee.xuanzx.com

[T08] Kotlin：数据类
来源：http://dfh.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://rtg.xuanzx.com

[T09] Kotlin：扩展函数
来源：http://fhn.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://vwx.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://eoy.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dju.mhx1999.top

[T11] Kotlin：协程
来源：http://qcu.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://isx.yuxming.cn

[T12] Kotlin：解构声明
来源：http://aym.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://quk.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://mai.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://dvd.yfazqb.com

[T14] Kotlin：循环
来源：http://dpn.zhongyouzk.top

for (i in 1..10) println(i)
来源：http://wtt.uphjek.com

[T15] Kotlin：接口
来源：http://ndu.xuanzx.com

interface Shape { fun area(): Double }
来源：http://gbz.ybcxt.top

[T16] Swift：Hello World
来源：http://hue.zycfv.cn

print("Hello")
来源：http://iqu.yongpay.top

[T17] Swift：变量与常量
来源：http://cbi.zdbjq.cn

var a = 1;  let b = 2
来源：http://frl.xinyue.icu

[T18] Swift：字符串插值
来源：http://wov.cucudq.cn

"值: \(b)"
来源：http://vok.hongshengwenyu.top

[T19] Swift：可选绑定
来源：http://hoz.aizwys.cn

if let n = opt { print(n) }
来源：http://mcv.wangdashe.top

[T20] Swift：数组操作
来源：http://xkp.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://wqz.yj20258888.top

[T21] Swift：遍历
来源：http://abp.aibaodan.cn

for x in a { print(x) }
来源：http://jnr.jiagoushi.top

[T22] Swift：字典
来源：http://lyt.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://eiz.wangshuangyany.cn

[T23] Swift：函数
来源：http://naf.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yux.yj20258888.top

[T24] Swift：闭包
来源：http://fyh.iojbl.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qsv.iojbl.cn

[T25] Swift：结构体
来源：http://xet.aizwys.cn

struct P { var x: Int }
来源：http://jzy.nanxinkj.top

[T26] Swift：类与重写
来源：http://swz.jinyuanbaomall.cn

class A: Base { override func f() {} }
来源：http://lln.zdqjudy.top

[T27] Swift：错误处理
来源：http://ity.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://gcj.snrcjt.cn

[T28] Swift：枚举
来源：http://aeh.aizwys.cn

enum Color { case red, green }
来源：http://uzr.birdmap.top

[T29] Swift：guard 提前返回
来源：http://gzg.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://fbk.cqqwz.cn

[T30] Swift：协议
来源：http://via.nwbrower.top

protocol Shape { func area() -> Double }
来源：http://kea.aizwys.cn

[T31] Lua：Hello World
来源：http://bek.dianchejie.cn

print("Hello")
来源：http://bos.zhoulong.xyz

[T32] Lua：局部变量
来源：http://xuj.316326.xyz

local a = 1
来源：http://dfx.jinghuilouyu.cn

[T33] Lua：表（数组）
来源：http://zak.zhiwuduotai.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nhh.feifeiyinyue.top

[T34] Lua：遍历表
来源：http://ofr.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://krj.jqgfzy.top

[T35] Lua：字典表
来源：http://ovn.cucudq.cn

local d = { a = 1 };  d.b = 2
来源：http://qvx.shzxlz.cn

[T36] Lua：函数
来源：http://efq.hesvh.cn

function add(a, b) return a + b end
来源：http://ymw.shangyingyoupin.top

[T37] Lua：字符串拼接
来源：http://kmh.xuanzx.com

"a" .. "b"
来源：http://sqj.cucudq.cn

[T38] Lua：条件
来源：http://rbo.tanke756.top

if x > 0 then print("正") end
来源：http://dmc.zhaomingkeji.xyz

[T39] Lua：模式匹配
来源：http://wvf.redwolf501.top

string.find(s, "%d+")
来源：http://dtb.daria6918.cn

[T40] Lua：元表
来源：http://oez.zdqjudy.top

setmetatable({}, { __index = base })
来源：http://bfb.yongpay.top

[T41] Perl：Hello World
来源：http://hjv.redwolf501.top

print "Hello\n";
来源：http://qgx.andypj.xyz

[T42] Perl：变量类型
来源：http://jjw.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hlz.kuanghao11.cn

[T43] Perl：字符串插值
来源：http://qud.jinyuanbaomall.cn

"值: $a"
来源：http://bxe.cheryme.top

[T44] Perl：条件
来源：http://jon.pengpengdd.cyou

if ($a > 0) { print "正"; }
来源：http://dqa.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://mpb.chenzaomai.com

for my $x (@arr) { print $x; }
来源：http://szx.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://ust.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://btc.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://yac.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ruc.fehbvm.com

[T48] Perl：正则替换
来源：http://ise.yangfankeji.com

$s =~ s/old/new/g;
来源：http://gdf.jinyuanbaomall.cn

[T49] Perl：函数
来源：http://jzy.daxiang520.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kac.tarul.cn

[T50] Perl：逐行读文件
来源：http://mca.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://yak.xuetiantiany.cn

while (my $line = <$fh>) { print $line; }
来源：http://ggj.daxiang520.top

[T51] Scala：Hello World
来源：http://xlw.yongpay.top

println("Hello")
来源：http://umj.shuidangran.top

[T52] Scala：变量
来源：http://nuo.cheryme.top

val a = 1;  var b = 2
来源：http://bkg.jinqigufen.top

[T53] Scala：字符串插值
来源：http://mdf.yangfankeji.com

s"值: $b"
来源：http://fmh.smart0.xyz

[T54] Scala：集合映射
来源：http://rci.chenzaomai.com

List(1, 2, 3).map(_ * 2)
来源：http://nxs.tanke756.top

[T55] Scala：集合过滤
来源：http://qoa.jinyuanbaomall.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qxb.yonumen.top

[T56] Scala：样例类
来源：http://zgd.meibo888.top

case class User(name: String, age: Int)
来源：http://qcc.feifeiyinyue.top

[T57] Scala：模式匹配
来源：http://oqo.0kj1m.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oft.zycfv.cn

[T58] Scala：函数定义
来源：http://ywq.yj202588.top


<!-- 参考信息 -->