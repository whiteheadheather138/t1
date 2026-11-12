代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qwr.jlsjyb.cn

[R50] awk 求和
来源：http://rfn.hongshengwenyu.top

awk '{s += $2} END {print s}' a.txt
来源：http://ixz.hysaishi.cn

[R51] 排序去重取前几
来源：http://pkb.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://uxm.hnqzz.top

[R52] 统计行数
来源：http://oaw.cdnleiting.top

wc -l a.txt
来源：http://wrx.cashguo.top

[R53] 查看文件头与实时尾
来源：http://ovb.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gbd.dashuyun.cn

[R54] 比较两个文件
来源：http://jmi.hnxiangtu.top

diff a.txt b.txt
来源：http://yit.pycfn.com

[R55] 压缩与解压
来源：http://sgu.ywan-chungtsiang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lyc.pengpengdd.cyou

[R56] 远程拷贝
来源：http://qgz.cdnleiting.top

scp file user@host:/path/
来源：http://vum.sjlbkw.cn

[R57] 远程执行命令
来源：http://zii.xuanzx.com

ssh user@host 'uptime'
来源：http://okm.zhoulong.xyz

[R58] 下载文件
来源：http://lur.chenjidiqi.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ydu.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://thd.jinqigfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://imy.hfpthk.cn

[R60] 只看 HTTP 状态码
来源：http://zba.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://byl.jinghuilouyu.cn

[R61] 磁盘占用
来源：http://wez.yuxming.cn

df -h;  du -sh *
来源：http://sfc.dianchejie.cn

[R62] 找最占空间的文件
来源：http://mda.yj20258888.top

du -ah . | sort -rh | head -10
来源：http://lbv.gogol.net.cn

[R63] 内存与进程
来源：http://pqj.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://nzj.yfazqb.com

[R64] 结束进程
来源：http://cbi.redwolf501.top

kill -9 $(pgrep -f app.py)
来源：http://vqn.shangyingyoupin.top

[R65] 查看端口占用
来源：http://yyw.yangfankeji.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uaw.zhongyouzk.top

[R66] 定时任务
来源：http://yhb.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://gfo.nwbrower.top

[R67] 生成随机十六进制串
来源：http://ben.xylfe.cn

openssl rand -hex 16
来源：http://xkl.shuidangran.top

[R68] 计算文件校验值
来源：http://ign.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vvj.daxiang520.top

[R69] 生成随机密码
来源：http://aep.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://stk.yonumen.top

[R70] 时间戳与互转
来源：http://qtx.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://lpb.chenjidiqi.icu

[R71] 日期格式化
来源：http://lio.nanxinkj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://otq.bjfxy.top

[R72] 等待端口就绪
来源：http://qsg.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hoo.nwbrower.top

[R73] 分割大日志
来源：http://fss.9152youxi.cn

split -l 1000 big.log part_
来源：http://geq.hammf.cn

[R74] 批量重命名
来源：http://dbu.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wpr.tarul.cn

[R75] 导出环境变量
来源：http://aep.52xcode.cn

export PATH="$HOME/bin:$PATH"
来源：http://euo.meibo888.top

[R76] 使用临时文件
来源：http://ett.9152youxi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ccd.shangyingyoupin.top

[R77] 读取用户输入
来源：http://ysl.pycfn.com

read -rp "请输入: " ans
来源：http://huy.nanxuanxn.top

[R78] 交互式菜单
来源：http://rfl.guowangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xbd.nwbrower.top

[R79] 解析命令行选项
来源：http://kzm.yonumen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jyd.cqqwz.cn

[R80] 查看脚本执行耗时
来源：http://dja.shzxlz.cn

time ./run.sh
来源：http://ibo.yfazqb.com

================================================================================
来源：http://tpb.bjfxy.top

S. C / C++ 专题
来源：http://xfz.yuanzhike.top

================================================================================
来源：http://gyt.fktsv.cn

[S01] C：Hello World
来源：http://igl.dianchejie.cn

#include <stdio.h>
来源：http://sok.shanyushiyangtech.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://toe.pycfn.com

[S02] C：变量与格式化输出
来源：http://pwx.kuanghao11.cn

int a = 10; printf("%d\n", a);
来源：http://asm.yj20258888.top

[S03] C：读入整数
来源：http://vtg.yonumen.top

int x; scanf("%d", &x);
来源：http://gou.yuxming.cn

[S04] C：字符串复制
来源：http://lpp.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://uqf.hywenlv.cn

[S05] C：字符串长度
来源：http://mmz.zdqjudy.top

strlen(s)
来源：http://krs.wangshuangyany.cn

[S06] C：字符串比较
来源：http://nfx.chenzaomai.com

strcmp(a, b) == 0
来源：http://woi.zhengqikj.top

[S07] C：数组遍历求和
来源：http://nak.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kgd.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://mki.0kj1m.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cgb.havefunace.top

[S09] C：结构体定义与初始化
来源：http://rdw.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aif.snrcjt.cn

[S10] C：指针与解引用
来源：http://cll.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://qrl.quarkkingdee.top

[S11] C：逐行读文件
来源：http://lgq.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://pvt.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://hhz.jinqigfzy.top

fclose(f);
来源：http://iue.snrcjt.cn

[S12] C：写文件
来源：http://ktx.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ijc.gogol.net.cn

[S13] C：宏定义
来源：http://vcn.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uhq.pengpengdd.cyou

[S14] C：枚举
来源：http://try.cqqwz.cn

enum Color { RED, GREEN, BLUE };
来源：http://mxc.zycfv.cn

[S15] C：类型转换
来源：http://utt.ppjwa.cn

(double) a / b
来源：http://gct.havefunace.top

[S16] C：位操作置位
来源：http://wbl.chenzaomai.com

x |= (1 << 3);
来源：http://uvi.sweek.top

[S17] C：安全拼接字符串
来源：http://qiq.shzxlz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cao.andypj.xyz

[S18] C：命令行参数
来源：http://nyk.9152youxi.cn

int main(int argc, char **argv)
来源：http://ouq.sufxvd.cn

[S19] C：快速排序
来源：http://cay.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://gdx.yj20258.top

[S20] C：二分查找
来源：http://kov.yj20258888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cbs.cucudq.cn

[S21] C：字符类别判断
来源：http://bdi.kuanghao11.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hmu.yuxming.cn

[S22] C：字符串转数字
来源：http://pdu.smart0.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://hpc.zhixingplan.top

[S23] C：随机数
来源：http://elv.ivvv.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bvk.cheryme.top

[S24] C：获取本地时间
来源：http://kft.xuanzx.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://glf.zhoulong.xyz

[S25] C：内存拷贝
来源：http://ggm.snrcjt.cn

memcpy(dst, src, n);
来源：http://skk.fehbvm.com

[S26] C：内存清零
来源：http://dge.zhixingplan.top

memset(a, 0, sizeof a);
来源：http://hoq.aibaodan.cn

[S27] C：定义常量
来源：http://kfa.hfpthk.cn

const double PI = 3.14159;
来源：http://rae.cucudq.cn

[S28] C：静态变量
来源：http://izg.yj202588.top

static int counter = 0;
来源：http://ptk.zhixingplan.top

[S29] C：变参函数
来源：http://euk.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fcd.fengsongda.top

[S30] C：头文件保护
来源：http://qkd.vehdjk.com

#ifndef X_H
来源：http://fwj.zhijiandao.cn

#define X_H
来源：http://hdt.cucudq.cn

#endif
来源：http://byg.cashguo.top

[S31] C++：Hello World
来源：http://bwm.ybcxt.top

#include <iostream>
来源：http://qcy.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://biw.tarul.cn

[S32] C++：字符串
来源：http://yix.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://vmy.cucudq.cn

[S33] C++：vector 增删
来源：http://hhc.zhaomingkeji.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rok.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://qbw.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://wpo.yuxming.cn

[S35] C++：map
来源：http://zzw.tarul.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tli.ctjpmb.com

[S36] C++：unordered_map
来源：http://vcn.shuidangran.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://asc.ywan-chungtsiang.top

[S37] C++：set
来源：http://foe.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tdp.havefunace.top

[S38] C++：排序
来源：http://tby.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://btz.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://zyq.xylfe.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wup.shzxlz.cn

[S40] C++：查找元素
来源：http://wsd.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nds.gogol.net.cn

[S41] C++：类与构造函数
来源：http://kkl.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xaz.cheryme.top

[S42] C++：继承与虚函数
来源：http://fqc.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://oey.andypj.xyz

[S43] C++：智能指针
来源：http://tmb.havefunace.top

auto p = std::make_unique<int>(5);
来源：http://sxb.hfpthk.cn

[S44] C++：引用传参
来源：http://ory.sysykeji.top

void inc(int &x) { ++x; }
来源：http://pvf.daxiang520.top

[S45] C++：lambda
来源：http://txh.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://lnq.0kj1m.cn

[S46] C++：函数模板
来源：http://rgi.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ubo.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://meo.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://asm.hysaishi.cn

[S48] C++：逐行读文件
来源：http://cwq.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://ozi.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://dww.hnxiangtu.top

[S49] C++：写文件
来源：http://kvd.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://szx.gzhubu.top

[S50] C++：格式化数字
来源：http://aas.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rhr.xylfe.cn

[S51] C++：显式类型转换
来源：http://alr.shuidangran.top

static_cast<double>(a) / b
来源：http://lrk.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://jdg.sweek.top

int size() const noexcept { return n_; }
来源：http://jdr.tian-w.cn

[S53] C++：移动语义
来源：http://eca.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://ump.yonumen.top

[S54] C++：异常处理
来源：http://hxm.pycfn.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://daj.hammf.cn

[S55] C++：结构化绑定
来源：http://rvo.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ofe.cqqwz.cn

[S56] C++：optional
来源：http://atm.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ttm.hywenlv.cn

[S57] C++：编译期常量
来源：http://npp.fzhhl.top

constexpr int N = 10;
来源：http://zaz.hcnkem.com

[S58] C++：命名空间
来源：http://xxe.ydzc1.top

namespace ns { int f() { return 1; } }
来源：http://gdo.redwolf501.top

[S59] C++：静态断言
来源：http://clm.redwolf501.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://obv.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://ksk.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lng.yangfankeji.com

================================================================================
来源：http://qbr.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://frm.daria6918.cn

================================================================================
来源：http://hyv.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://tqi.zdqjudy.top

println("Hello")
来源：http://zyj.havefunace.top

[T02] Kotlin：变量
来源：http://wib.svipenyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wop.birdmap.top

[T03] Kotlin：字符串模板
来源：http://jkn.chenzaomai.com

"值: $b"
来源：http://rcd.jinyuanbaomall.cn

[T04] Kotlin：空安全
来源：http://ppo.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://ruo.tian-w.cn

[T05] Kotlin：when 表达式
来源：http://tyg.ybcxt.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hdy.chenjidiqi.icu

[T06] Kotlin：集合映射
来源：http://nav.andypj.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://zmn.yj20258888.top

[T07] Kotlin：集合过滤
来源：http://yuq.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://raw.daria6918.cn

[T08] Kotlin：数据类
来源：http://oqv.ctjpmb.com

data class User(val name: String, val age: Int)
来源：http://fvd.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://cmw.daria6918.cn

fun String.exclaim() = this + "!"
来源：http://tcx.xuanzx.com

[T10] Kotlin：默认参数
来源：http://fcc.cdnleiting.top

fun greet(name: String = "World") = "Hi $name"
来源：http://crt.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://rvi.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qsk.yfazqb.com

[T12] Kotlin：解构声明
来源：http://abh.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://wmx.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://grp.jqgfzy.top

val m = mapOf("a" to 1)
来源：http://bof.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://asv.daxiang520.top

for (i in 1..10) println(i)
来源：http://tvb.dianchejie.cn

[T15] Kotlin：接口
来源：http://sot.redwolf501.top

interface Shape { fun area(): Double }
来源：http://ihd.aizwys.cn

[T16] Swift：Hello World
来源：http://mje.c1oappe.top

print("Hello")
来源：http://www.chenlongwang.top

[T17] Swift：变量与常量
来源：http://wlq.gzhubu.top

var a = 1;  let b = 2
来源：http://pjx.vqdsnc.cn

[T18] Swift：字符串插值
来源：http://rch.nwbrower.top

"值: \(b)"
来源：http://dwg.fehbvm.com

[T19] Swift：可选绑定
来源：http://akb.yangfankeji.com

if let n = opt { print(n) }
来源：http://bwl.pycfn.com

[T20] Swift：数组操作
来源：http://jyk.aizwys.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hbp.iojbl.cn

[T21] Swift：遍历
来源：http://ctv.c1oappe.top

for x in a { print(x) }
来源：http://otf.aibaodan.cn

[T22] Swift：字典
来源：http://cwg.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://ioz.meibo888.top

[T23] Swift：函数
来源：http://nma.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ekb.hywenlv.cn

[T24] Swift：闭包
来源：http://weu.zhijiandao.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gwy.dianchejie.cn

[T25] Swift：结构体
来源：http://ors.yj20258888.top

struct P { var x: Int }
来源：http://psm.kuanghao11.cn

[T26] Swift：类与重写
来源：http://efk.yueranfly.top

class A: Base { override func f() {} }
来源：http://bzj.guannengcc.top

[T27] Swift：错误处理
来源：http://jkb.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://reg.gogol.net.cn

[T28] Swift：枚举
来源：http://fja.bjfxy.top

enum Color { case red, green }
来源：http://lar.ybcxt.top

[T29] Swift：guard 提前返回
来源：http://ctn.cdnleiting.top

guard let x = opt else { return }
来源：http://xlp.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://ayc.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://pap.hcnkem.com

[T31] Lua：Hello World
来源：http://lkz.hfpthk.cn

print("Hello")
来源：http://lso.jinqigufen.top

[T32] Lua：局部变量
来源：http://ehc.meibo888.top

local a = 1
来源：http://tvf.hfpthk.cn

[T33] Lua：表（数组）
来源：http://mlb.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://ign.yj20258.top

[T34] Lua：遍历表
来源：http://idl.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rbs.mhx1999.top

[T35] Lua：字典表
来源：http://ecm.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://jre.pycfn.com

[T36] Lua：函数
来源：http://unl.nanxinkj.top

function add(a, b) return a + b end
来源：http://eze.fanxiaobao.xyz

[T37] Lua：字符串拼接
来源：http://yad.fanxiaobao.xyz

"a" .. "b"
来源：http://jok.gzhubu.top

[T38] Lua：条件
来源：http://wug.zhijiandao.cn

if x > 0 then print("正") end
来源：http://azm.hesvh.cn

[T39] Lua：模式匹配
来源：http://dha.meibo888.top

string.find(s, "%d+")
来源：http://rmg.andypj.xyz

[T40] Lua：元表
来源：http://vpa.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://yxf.yuxming.cn

[T41] Perl：Hello World
来源：http://yhv.shangyingyoupin.top

print "Hello\n";
来源：http://nlr.chenzaomai.com

[T42] Perl：变量类型
来源：http://nmu.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://otc.dianchejie.cn

[T43] Perl：字符串插值
来源：http://lrd.fzhhl.top

"值: $a"
来源：http://sny.zycfv.cn

[T44] Perl：条件
来源：http://rse.jlsjyb.cn

if ($a > 0) { print "正"; }
来源：http://zlv.havefunace.top

[T45] Perl：数组遍历
来源：http://ptl.birdmap.top

for my $x (@arr) { print $x; }
来源：http://edg.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://qpp.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vqi.kuanghao11.cn

[T47] Perl：正则捕获
来源：http://nir.havefunace.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://iye.tianlin.xyz

[T48] Perl：正则替换
来源：http://rrw.hnxiangtu.top

$s =~ s/old/new/g;
来源：http://eyj.sufxvd.cn

[T49] Perl：函数
来源：http://vsg.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ckq.tanke756.top

[T50] Perl：逐行读文件
来源：http://rdh.hysaishi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rjq.ehwqpu.com

while (my $line = <$fh>) { print $line; }
来源：http://gdp.zycfv.cn

[T51] Scala：Hello World
来源：http://ion.iojbl.cn

println("Hello")
来源：http://keg.zycfv.cn

[T52] Scala：变量
来源：http://bwe.fktsv.cn


<!-- 参考信息 -->