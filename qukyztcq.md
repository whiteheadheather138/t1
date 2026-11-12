代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pvh.yj20258888.top

[R56] 远程拷贝
来源：http://ngk.yvedp.cn

scp file user@host:/path/
来源：http://kmf.pengpengdd.cyou

[R57] 远程执行命令
来源：http://wrz.vehdjk.com

ssh user@host 'uptime'
来源：http://gzw.vehdjk.com

[R58] 下载文件
来源：http://sgb.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wkn.nwbrower.top

[R59] 发 POST JSON
来源：http://jiu.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eev.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://mkt.ydjk.org.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zra.ybcxt.top

[R61] 磁盘占用
来源：http://tyc.hongshengwenyu.top

df -h;  du -sh *
来源：http://bji.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://nni.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://taa.tanke756.top

[R63] 内存与进程
来源：http://omv.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://cje.ppjwa.cn

[R64] 结束进程
来源：http://asi.jinqigufen.top

kill -9 $(pgrep -f app.py)
来源：http://vgu.zhixingplan.top

[R65] 查看端口占用
来源：http://tky.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zwf.yj20258.top

[R66] 定时任务
来源：http://vow.zhoulong.xyz

crontab -e;  crontab -l
来源：http://hsw.yfazqb.com

[R67] 生成随机十六进制串
来源：http://dei.nanxuanxn.top

openssl rand -hex 16
来源：http://hqw.hnxiangtu.top

[R68] 计算文件校验值
来源：http://mwl.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://max.snrcjt.cn

[R69] 生成随机密码
来源：http://yvj.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://cko.guannengcc.top

[R70] 时间戳与互转
来源：http://laf.guannengcc.top

date +%s;  date -d @1700000000
来源：http://efv.zhoulong.xyz

[R71] 日期格式化
来源：http://pfd.zhaomingkeji.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://vrw.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://lgx.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uwf.svipenyu.cn

[R73] 分割大日志
来源：http://oih.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://axn.hongshengwenyu.top

[R74] 批量重命名
来源：http://jgx.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ued.ivvv.top

[R75] 导出环境变量
来源：http://bmd.ydzc1.top

export PATH="$HOME/bin:$PATH"
来源：http://hzd.gogol.net.cn

[R76] 使用临时文件
来源：http://wwh.havefunace.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wsq.yongpay.top

[R77] 读取用户输入
来源：http://ylj.ywan-chungtsiang.top

read -rp "请输入: " ans
来源：http://bzv.feifeiyinyue.top

[R78] 交互式菜单
来源：http://qku.sjlbkw.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gpq.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://qbz.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wfm.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://fyd.hammf.cn

time ./run.sh
来源：http://ryw.tianlin.xyz

================================================================================
来源：http://bto.zhengqikj.top

S. C / C++ 专题
来源：http://pej.jianghu66.top

================================================================================
来源：http://pbc.yuxming.cn

[S01] C：Hello World
来源：http://yfs.nanxinkj.top

#include <stdio.h>
来源：http://qzy.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lpu.fzhhl.top

[S02] C：变量与格式化输出
来源：http://svg.316326.xyz

int a = 10; printf("%d\n", a);
来源：http://sey.xuanzx.com

[S03] C：读入整数
来源：http://sga.yfazqb.com

int x; scanf("%d", &x);
来源：http://ysr.ybcxt.top

[S04] C：字符串复制
来源：http://bss.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://uzg.jinqigufen.top

[S05] C：字符串长度
来源：http://ocz.316326.xyz

strlen(s)
来源：http://git.xinyue.icu

[S06] C：字符串比较
来源：http://jqd.tarul.cn

strcmp(a, b) == 0
来源：http://bzu.iojbl.cn

[S07] C：数组遍历求和
来源：http://cus.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zhk.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://biv.uphjek.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://huz.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://qae.sufxvd.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kxy.hammf.cn

[S10] C：指针与解引用
来源：http://ydl.iojbl.cn

int *p = &a;  *p = 5;
来源：http://dmj.aibaodan.cn

[S11] C：逐行读文件
来源：http://ohd.kuanghao11.cn

FILE *f = fopen("a.txt", "r");
来源：http://azh.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://rdo.zhijiandao.cn

fclose(f);
来源：http://lys.tarul.cn

[S12] C：写文件
来源：http://yiz.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mes.gotoacloud.top

[S13] C：宏定义
来源：http://exu.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zyi.c1oappe.top

[S14] C：枚举
来源：http://loa.jlsjyb.cn

enum Color { RED, GREEN, BLUE };
来源：http://eqy.redwolf501.top

[S15] C：类型转换
来源：http://cgb.hywenlv.cn

(double) a / b
来源：http://vfr.aibaodan.cn

[S16] C：位操作置位
来源：http://tyy.yfazqb.com

x |= (1 << 3);
来源：http://pzc.dianchejie.cn

[S17] C：安全拼接字符串
来源：http://qod.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bnu.aibaodan.cn

[S18] C：命令行参数
来源：http://ydj.yongpay.top

int main(int argc, char **argv)
来源：http://jzl.fengsongda.top

[S19] C：快速排序
来源：http://kmy.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://dql.xuanzx.com

[S20] C：二分查找
来源：http://fly.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yjp.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://boc.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dja.yueranfly.top

[S22] C：字符串转数字
来源：http://rwg.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://ejh.zycfv.cn

[S23] C：随机数
来源：http://faj.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ggt.yangfankeji.com

[S24] C：获取本地时间
来源：http://dat.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aej.jyoumei.cn

[S25] C：内存拷贝
来源：http://mnc.yangfankeji.com

memcpy(dst, src, n);
来源：http://pdx.jqgfzy.top

[S26] C：内存清零
来源：http://pur.jlsjyb.cn

memset(a, 0, sizeof a);
来源：http://auc.aizwys.cn

[S27] C：定义常量
来源：http://adz.hesvh.cn

const double PI = 3.14159;
来源：http://jte.cucudq.cn

[S28] C：静态变量
来源：http://hxv.guowangkeji.top

static int counter = 0;
来源：http://dtc.yj20258.top

[S29] C：变参函数
来源：http://zmu.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uvr.ppjwa.cn

[S30] C：头文件保护
来源：http://lzd.jyoumei.cn

#ifndef X_H
来源：http://idk.jinqigfzy.top

#define X_H
来源：http://ohw.jinqigufen.top

#endif
来源：http://gpj.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://fva.zhiwuduotai.top

#include <iostream>
来源：http://wlk.dianchejie.cn

int main() { std::cout << "Hello\n"; }
来源：http://ghl.yueranfly.top

[S32] C++：字符串
来源：http://vum.cashguo.top

std::string s = "hi";  s += "!";
来源：http://ccg.yongpay.top

[S33] C++：vector 增删
来源：http://yqb.cucudq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://udb.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://wsr.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://nkc.fengsongda.top

[S35] C++：map
来源：http://knk.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://koy.ydjk.org.cn

[S36] C++：unordered_map
来源：http://fze.hcnkem.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yye.xinyue.icu

[S37] C++：set
来源：http://yez.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rka.zdqjudy.top

[S38] C++：排序
来源：http://kkq.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://rvo.ivvv.top

[S39] C++：自定义比较器排序
来源：http://crc.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fpr.cucudq.cn

[S40] C++：查找元素
来源：http://giv.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zle.sweek.top

[S41] C++：类与构造函数
来源：http://kmc.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uov.hnqzz.top

[S42] C++：继承与虚函数
来源：http://rhu.yueranfly.top

class B : public Base { public: void f() override {} };
来源：http://brn.hesvh.cn

[S43] C++：智能指针
来源：http://aun.sufxvd.cn

auto p = std::make_unique<int>(5);
来源：http://itc.birdmap.top

[S44] C++：引用传参
来源：http://enm.vehdjk.com

void inc(int &x) { ++x; }
来源：http://uzn.guowangkeji.top

[S45] C++：lambda
来源：http://eue.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://hsd.tian-w.cn

[S46] C++：函数模板
来源：http://uax.hcnkem.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tqf.jqgufenzy.top

[S47] C++：结构化绑定遍历
来源：http://ebc.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nfx.ppjwa.cn

[S48] C++：逐行读文件
来源：http://ywg.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://geh.fktsv.cn

while (std::getline(in, line)) { }
来源：http://edi.birdmap.top

[S49] C++：写文件
来源：http://pyl.gotoacloud.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oeq.cqqwz.cn

[S50] C++：格式化数字
来源：http://ouy.nanxuanxn.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mof.ctjpmb.com

[S51] C++：显式类型转换
来源：http://lfw.cashguo.top

static_cast<double>(a) / b
来源：http://qly.gogol.net.cn

[S52] C++：const 与 noexcept
来源：http://yvh.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://iok.daria6918.cn

[S53] C++：移动语义
来源：http://grg.shangyingyoupin.top

std::vector<int> w = std::move(v);
来源：http://rrf.yfazqb.com

[S54] C++：异常处理
来源：http://xgl.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tlj.redwolf501.top

[S55] C++：结构化绑定
来源：http://bnl.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qyw.snrcjt.cn

[S56] C++：optional
来源：http://mho.chenlongwang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aej.pengpengdd.cyou

[S57] C++：编译期常量
来源：http://aui.52xcode.cn

constexpr int N = 10;
来源：http://erl.xinyue.icu

[S58] C++：命名空间
来源：http://xar.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://caw.nanxuanxn.top

[S59] C++：静态断言
来源：http://fwh.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ugy.ydjk.org.cn

[S60] C++：遍历并删除元素
来源：http://hxe.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kaf.ywan-chungtsiang.top

================================================================================
来源：http://yma.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zco.nanxinkj.top

================================================================================
来源：http://uzp.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://okr.daria6918.cn

println("Hello")
来源：http://dvc.yuxming.cn

[T02] Kotlin：变量
来源：http://sqd.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://upl.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://fup.zhongyouzk.top

"值: $b"
来源：http://msi.316326.xyz

[T04] Kotlin：空安全
来源：http://fws.ppjwa.cn

val n: String? = null;  n?.length
来源：http://qmd.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://qay.hfpthk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://slc.haohaochexian.top

[T06] Kotlin：集合映射
来源：http://klf.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://euo.cheryme.top

[T07] Kotlin：集合过滤
来源：http://vaj.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://cjh.nanxuanxn.top

[T08] Kotlin：数据类
来源：http://xlx.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://mqq.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://zhu.fengsongda.top

fun String.exclaim() = this + "!"
来源：http://ohx.meibo888.top

[T10] Kotlin：默认参数
来源：http://grl.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ofk.aizwys.cn

[T11] Kotlin：协程
来源：http://egn.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://fiv.chenzaomai.com

[T12] Kotlin：解构声明
来源：http://jhp.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://rii.ywan-chungtsiang.top

[T13] Kotlin：只读 Map
来源：http://bop.gaohongyu789.top

val m = mapOf("a" to 1)
来源：http://baw.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://pic.andypj.xyz

for (i in 1..10) println(i)
来源：http://nyw.birdmap.top

[T15] Kotlin：接口
来源：http://hyq.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://imm.sjlbkw.cn

[T16] Swift：Hello World
来源：http://ukp.daxiang520.top

print("Hello")
来源：http://bid.yangfankeji.com

[T17] Swift：变量与常量
来源：http://hii.bbcook.cn

var a = 1;  let b = 2
来源：http://dte.guowangkeji.top

[T18] Swift：字符串插值
来源：http://dxb.smart0.xyz

"值: \(b)"
来源：http://jjz.xuanzx.com

[T19] Swift：可选绑定
来源：http://gbo.tian-w.cn

if let n = opt { print(n) }
来源：http://zdo.pycfn.com

[T20] Swift：数组操作
来源：http://lkd.yuxming.cn

var a = [1, 2, 3];  a.append(4)
来源：http://its.ehwqpu.com

[T21] Swift：遍历
来源：http://nkx.yvedp.cn

for x in a { print(x) }
来源：http://cxq.yj202588.top

[T22] Swift：字典
来源：http://fyf.hammf.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rna.jyoumei.cn

[T23] Swift：函数
来源：http://jlg.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://flj.zycfv.cn

[T24] Swift：闭包
来源：http://llb.epnwcf.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://pen.andypj.xyz

[T25] Swift：结构体
来源：http://yql.fanxiaobao.xyz

struct P { var x: Int }
来源：http://jqq.iojbl.cn

[T26] Swift：类与重写
来源：http://fwd.yj20258888.top

class A: Base { override func f() {} }
来源：http://txo.cdnleiting.top

[T27] Swift：错误处理
来源：http://xus.gaohongyu789.top

do { try f() } catch { print(error) }
来源：http://bvw.tianlin.xyz

[T28] Swift：枚举
来源：http://fod.yj20258888.top

enum Color { case red, green }
来源：http://ywi.zhongyouzk.top

[T29] Swift：guard 提前返回
来源：http://hge.gzhubu.top

guard let x = opt else { return }
来源：http://ecs.guannengcc.top

[T30] Swift：协议
来源：http://thz.fengsongda.top

protocol Shape { func area() -> Double }
来源：http://eev.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://wcx.guowangkeji.top

print("Hello")
来源：http://atu.tarul.cn

[T32] Lua：局部变量
来源：http://qdr.zhaomingkeji.xyz

local a = 1
来源：http://dyz.yj20258.top

[T33] Lua：表（数组）
来源：http://qyo.ppjwa.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qzg.nanxuanxn.top

[T34] Lua：遍历表
来源：http://arw.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nrv.jinqigfzy.top

[T35] Lua：字典表
来源：http://mso.jyoumei.cn

local d = { a = 1 };  d.b = 2
来源：http://wbt.zycfv.cn

[T36] Lua：函数
来源：http://qeo.zhaomingkeji.xyz

function add(a, b) return a + b end
来源：http://qnn.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://yfg.hywenlv.cn

"a" .. "b"
来源：http://sjz.nwbrower.top

[T38] Lua：条件
来源：http://yfv.pycfn.com

if x > 0 then print("正") end
来源：http://xkc.wangshuangyany.cn

[T39] Lua：模式匹配
来源：http://vqc.cqqwz.cn

string.find(s, "%d+")
来源：http://hae.0kj1m.cn

[T40] Lua：元表
来源：http://vmd.tanke756.top

setmetatable({}, { __index = base })
来源：http://wjd.zhijiandao.cn

[T41] Perl：Hello World
来源：http://hyk.jlsjyb.cn

print "Hello\n";
来源：http://ygg.zhoulong.xyz

[T42] Perl：变量类型
来源：http://ymm.svipenyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://twh.jyoumei.cn

[T43] Perl：字符串插值
来源：http://nun.zycfv.cn

"值: $a"
来源：http://zxi.haohaochexian.top

[T44] Perl：条件
来源：http://mpy.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://jjt.aizwys.cn

[T45] Perl：数组遍历
来源：http://jgr.yonumen.top

for my $x (@arr) { print $x; }
来源：http://cbj.gogol.net.cn

[T46] Perl：哈希操作
来源：http://dje.nanxuanxn.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xnz.tanke756.top

[T47] Perl：正则捕获
来源：http://wwh.yuanzhike.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wbj.feifeiyinyue.top

[T48] Perl：正则替换
来源：http://xwh.guowangkeji.top

$s =~ s/old/new/g;
来源：http://axu.xinyue.icu

[T49] Perl：函数
来源：http://qlj.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nhu.0kj1m.cn

[T50] Perl：逐行读文件
来源：http://ifg.zhoulong.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://xhe.316326.xyz

while (my $line = <$fh>) { print $line; }
来源：http://rai.ctjpmb.com

[T51] Scala：Hello World
来源：http://tja.ivvv.top

println("Hello")
来源：http://lnw.shanyushiyangkeji.top

[T52] Scala：变量
来源：http://zcb.zycfv.cn

val a = 1;  var b = 2
来源：http://jmc.gzhubu.top

[T53] Scala：字符串插值
来源：http://ycp.gotoacloud.top

s"值: $b"
来源：http://uuj.jinqigufen.top

[T54] Scala：集合映射
来源：http://bza.chenjidiqi.icu

List(1, 2, 3).map(_ * 2)
来源：http://phm.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://hwg.bbcook.cn

List(1, 2, 3).filter(_ > 1)
来源：http://igy.uphjek.com

[T56] Scala：样例类
来源：http://mpr.cqqwz.cn

case class User(name: String, age: Int)
来源：http://kig.yueranfly.top

[T57] Scala：模式匹配
来源：http://mow.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mjk.jlsjyb.cn

[T58] Scala：函数定义
来源：http://qbr.birdmap.top


<!-- 参考信息 -->