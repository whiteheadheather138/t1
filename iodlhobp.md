代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fid.xziqi.cn

[R50] awk 求和
来源：http://qbf.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gkz.xuanzx.com

[R51] 排序去重取前几
来源：http://zlu.aibaodan.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rfa.jyoumei.cn

[R52] 统计行数
来源：http://wpt.yj20258.top

wc -l a.txt
来源：http://ngq.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://hlj.sxryk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uqw.shuidangran.top

[R54] 比较两个文件
来源：http://ctg.zhijiandao.cn

diff a.txt b.txt
来源：http://qwo.tarul.cn

[R55] 压缩与解压
来源：http://wxg.yongpay.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xbm.yueranfly.top

[R56] 远程拷贝
来源：http://oav.ppjwa.cn

scp file user@host:/path/
来源：http://ssr.xziqi.cn

[R57] 远程执行命令
来源：http://cnq.chenjidiqi.icu

ssh user@host 'uptime'
来源：http://gvm.yonumen.top

[R58] 下载文件
来源：http://gbn.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lui.zhixingplan.top

[R59] 发 POST JSON
来源：http://mzf.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://amb.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://htc.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sxh.shzxlz.cn

[R61] 磁盘占用
来源：http://lse.yj202588.top

df -h;  du -sh *
来源：http://gco.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://agq.zhixingplan.top

du -ah . | sort -rh | head -10
来源：http://gih.andypj.xyz

[R63] 内存与进程
来源：http://nxl.zhongyouzk.top

free -h;  ps aux | grep nginx
来源：http://dve.chenjidiqi.icu

[R64] 结束进程
来源：http://qqw.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://ffq.yangfankeji.com

[R65] 查看端口占用
来源：http://ock.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ouu.jyoumei.cn

[R66] 定时任务
来源：http://bon.daxiang520.top

crontab -e;  crontab -l
来源：http://gdo.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://zer.smart0.xyz

openssl rand -hex 16
来源：http://jki.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://ubc.mhx1999.top

sha256sum a.txt;  md5sum a.txt
来源：http://ulm.hammf.cn

[R69] 生成随机密码
来源：http://fze.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://poj.tian-w.cn

[R70] 时间戳与互转
来源：http://rxr.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://hfz.aizwys.cn

[R71] 日期格式化
来源：http://jcf.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ecf.316326.xyz

[R72] 等待端口就绪
来源：http://rhc.vqdsnc.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yuw.aizwys.cn

[R73] 分割大日志
来源：http://bsn.yongpay.top

split -l 1000 big.log part_
来源：http://ylq.iojbl.cn

[R74] 批量重命名
来源：http://ffa.gaohongyu789.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ine.c1oappe.top

[R75] 导出环境变量
来源：http://dzz.gotoacloud.top

export PATH="$HOME/bin:$PATH"
来源：http://fci.c1oappe.top

[R76] 使用临时文件
来源：http://ejg.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://osj.zdqjudy.top

[R77] 读取用户输入
来源：http://cdy.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://dgr.zhongyouzk.top

[R78] 交互式菜单
来源：http://mwe.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fdd.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://ptr.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hje.cqqwz.cn

[R80] 查看脚本执行耗时
来源：http://jru.52xcode.cn

time ./run.sh
来源：http://gga.mhx1999.top

================================================================================
来源：http://gvp.gzhubu.top

S. C / C++ 专题
来源：http://oxi.svipenyu.cn

================================================================================
来源：http://aen.nwbrower.top

[S01] C：Hello World
来源：http://zti.iojbl.cn

#include <stdio.h>
来源：http://jsm.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fns.yj20258888.top

[S02] C：变量与格式化输出
来源：http://vqf.guannengcc.top

int a = 10; printf("%d\n", a);
来源：http://oxb.sjlbkw.cn

[S03] C：读入整数
来源：http://bab.jqgfzy.top

int x; scanf("%d", &x);
来源：http://ioz.jlsjyb.cn

[S04] C：字符串复制
来源：http://gne.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://weg.cashguo.top

[S05] C：字符串长度
来源：http://wqv.sjlbkw.cn

strlen(s)
来源：http://njz.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://ovg.yvedp.cn

strcmp(a, b) == 0
来源：http://lyo.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://ylz.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wik.yongpay.top

[S08] C：动态内存分配与释放
来源：http://vmc.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rrf.gogol.net.cn

[S09] C：结构体定义与初始化
来源：http://rqq.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xtq.hfpthk.cn

[S10] C：指针与解引用
来源：http://cqc.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://zfz.bjfxy.top

[S11] C：逐行读文件
来源：http://dej.cucudq.cn

FILE *f = fopen("a.txt", "r");
来源：http://jmt.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lde.xylfe.cn

fclose(f);
来源：http://cvc.hnqzz.top

[S12] C：写文件
来源：http://xuz.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://omn.shuidangran.top

[S13] C：宏定义
来源：http://gkk.ehwqpu.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sqy.hywenlv.cn

[S14] C：枚举
来源：http://tkf.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://wcj.nwbrower.top

[S15] C：类型转换
来源：http://mty.sysykeji.top

(double) a / b
来源：http://bqe.316326.xyz

[S16] C：位操作置位
来源：http://uyt.aibaodan.cn

x |= (1 << 3);
来源：http://rvs.uphjek.com

[S17] C：安全拼接字符串
来源：http://xiq.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pvs.cqqwz.cn

[S18] C：命令行参数
来源：http://wiy.bbcook.cn

int main(int argc, char **argv)
来源：http://opm.tanke756.top

[S19] C：快速排序
来源：http://qze.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://bek.snrcjt.cn

[S20] C：二分查找
来源：http://qpm.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yxt.aibaodan.cn

[S21] C：字符类别判断
来源：http://mcr.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tis.yanxiufei.cn

[S22] C：字符串转数字
来源：http://uaw.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zbi.havefunace.top

[S23] C：随机数
来源：http://doe.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dbw.yfazqb.com

[S24] C：获取本地时间
来源：http://ieo.hcnkem.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kaw.chenlongwang.top

[S25] C：内存拷贝
来源：http://wes.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://oau.iojbl.cn

[S26] C：内存清零
来源：http://lhd.tarul.cn

memset(a, 0, sizeof a);
来源：http://sar.xinyue.icu

[S27] C：定义常量
来源：http://gem.yj202588.top

const double PI = 3.14159;
来源：http://uys.jqgufenzy.top

[S28] C：静态变量
来源：http://naf.shzxlz.cn

static int counter = 0;
来源：http://eje.jinghuilouyu.cn

[S29] C：变参函数
来源：http://adl.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yfd.yuanzhike.top

[S30] C：头文件保护
来源：http://mlp.hnqzz.top

#ifndef X_H
来源：http://sci.vehdjk.com

#define X_H
来源：http://lya.hnqzz.top

#endif
来源：http://zvm.52xcode.cn

[S31] C++：Hello World
来源：http://dqv.dashuyun.cn

#include <iostream>
来源：http://vae.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://cwy.kuanghao11.cn

[S32] C++：字符串
来源：http://qck.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://aqu.yvedp.cn

[S33] C++：vector 增删
来源：http://ssz.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wsi.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://geb.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://erf.hysaishi.cn

[S35] C++：map
来源：http://xds.yj202588.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vvk.sysykeji.top

[S36] C++：unordered_map
来源：http://dng.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zsq.hesvh.cn

[S37] C++：set
来源：http://qth.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cdg.tanke756.top

[S38] C++：排序
来源：http://kuz.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://kwr.xuetiantiany.cn

[S39] C++：自定义比较器排序
来源：http://kyj.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fnc.cqqwz.cn

[S40] C++：查找元素
来源：http://pmm.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aml.shuidangran.top

[S41] C++：类与构造函数
来源：http://mme.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kiq.vqdsnc.cn

[S42] C++：继承与虚函数
来源：http://pet.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://ery.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://gwn.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://eea.fzhhl.top

[S44] C++：引用传参
来源：http://dps.pengpengdd.cyou

void inc(int &x) { ++x; }
来源：http://hmk.jianghu66.top

[S45] C++：lambda
来源：http://tym.ppjwa.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yyi.nanxuanxn.top

[S46] C++：函数模板
来源：http://fir.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jaa.hnxiangtu.top

[S47] C++：结构化绑定遍历
来源：http://kwn.meibo888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hfs.316326.xyz

[S48] C++：逐行读文件
来源：http://iva.gaohongyu789.top

std::ifstream in("a.txt");  std::string line;
来源：http://xvw.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://ovp.vqdsnc.cn

[S49] C++：写文件
来源：http://len.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://swe.hfpthk.cn

[S50] C++：格式化数字
来源：http://gnh.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zty.smart0.xyz

[S51] C++：显式类型转换
来源：http://adw.jinqigufen.top

static_cast<double>(a) / b
来源：http://tdl.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://czx.ybcxt.top

int size() const noexcept { return n_; }
来源：http://rpc.wangdashe.top

[S53] C++：移动语义
来源：http://gyl.cucudq.cn

std::vector<int> w = std::move(v);
来源：http://vhg.chenzaomai.com

[S54] C++：异常处理
来源：http://hcq.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://khq.yj20258888.top

[S55] C++：结构化绑定
来源：http://jdd.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ish.hnxiangtu.top

[S56] C++：optional
来源：http://wjr.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yca.fktsv.cn

[S57] C++：编译期常量
来源：http://qhy.chenzaomai.com

constexpr int N = 10;
来源：http://qaw.ctjpmb.com

[S58] C++：命名空间
来源：http://gwd.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://fwz.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://cvz.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://did.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://obf.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tgs.hammf.cn

================================================================================
来源：http://zwk.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zis.wangshuangyany.cn

================================================================================
来源：http://rds.sxryk.cn

[T01] Kotlin：Hello World
来源：http://cwv.nwbrower.top

println("Hello")
来源：http://hgx.hysaishi.cn

[T02] Kotlin：变量
来源：http://tkj.andypj.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ytb.pengpengdd.cyou

[T03] Kotlin：字符串模板
来源：http://adc.9152youxi.cn

"值: $b"
来源：http://bqu.zhixingplan.top

[T04] Kotlin：空安全
来源：http://aay.chenzaomai.com

val n: String? = null;  n?.length
来源：http://ukw.jqgufenzy.top

[T05] Kotlin：when 表达式
来源：http://bks.smart0.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vrx.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://qur.zhaomingkeji.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://jfo.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://now.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lqz.hfpthk.cn

[T08] Kotlin：数据类
来源：http://evh.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://bwz.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://zxm.meibo888.top

fun String.exclaim() = this + "!"
来源：http://ngb.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://pfn.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uyu.yj20258.top

[T11] Kotlin：协程
来源：http://ypg.birdmap.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cay.smart0.xyz

[T12] Kotlin：解构声明
来源：http://foy.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://whg.andypj.xyz

[T13] Kotlin：只读 Map
来源：http://hec.yvedp.cn

val m = mapOf("a" to 1)
来源：http://rby.yonumen.top

[T14] Kotlin：循环
来源：http://inp.havefunace.top

for (i in 1..10) println(i)
来源：http://pry.xylfe.cn

[T15] Kotlin：接口
来源：http://vpw.wangshuangyany.cn

interface Shape { fun area(): Double }
来源：http://yte.vqdsnc.cn

[T16] Swift：Hello World
来源：http://kpd.yueranfly.top

print("Hello")
来源：http://njv.yueranfly.top

[T17] Swift：变量与常量
来源：http://zlx.tarul.cn

var a = 1;  let b = 2
来源：http://rha.ctjpmb.com

[T18] Swift：字符串插值
来源：http://rqr.hnxiangtu.top

"值: \(b)"
来源：http://cwy.xziqi.cn

[T19] Swift：可选绑定
来源：http://snq.ctjpmb.com

if let n = opt { print(n) }
来源：http://ezk.zdbjq.cn

[T20] Swift：数组操作
来源：http://ueu.zhijiandao.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gwk.0kj1m.cn

[T21] Swift：遍历
来源：http://ifa.hysaishi.cn

for x in a { print(x) }
来源：http://ils.ydjk.org.cn

[T22] Swift：字典
来源：http://jqt.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uwm.sysykeji.top

[T23] Swift：函数
来源：http://hxl.jinyuanbaomall.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ocv.gotoacloud.top

[T24] Swift：闭包
来源：http://xxn.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jib.fzhhl.top

[T25] Swift：结构体
来源：http://zte.fehbvm.com

struct P { var x: Int }
来源：http://kwv.ydzc1.top

[T26] Swift：类与重写
来源：http://xng.dianchejie.cn

class A: Base { override func f() {} }
来源：http://uki.iojbl.cn

[T27] Swift：错误处理
来源：http://nfo.sweek.top

do { try f() } catch { print(error) }
来源：http://itp.quarkkingdee.top

[T28] Swift：枚举
来源：http://rxh.uphjek.com

enum Color { case red, green }
来源：http://mne.gogol.net.cn

[T29] Swift：guard 提前返回
来源：http://ugz.yj20258888.top

guard let x = opt else { return }
来源：http://rmm.zhengqikj.top

[T30] Swift：协议
来源：http://kjn.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://ylk.nwbrower.top

[T31] Lua：Hello World
来源：http://dar.zdqjudy.top

print("Hello")
来源：http://xkf.yongpay.top

[T32] Lua：局部变量
来源：http://edh.xziqi.cn

local a = 1
来源：http://zic.52xcode.cn

[T33] Lua：表（数组）
来源：http://uvo.chenjidiqi.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://vcd.vehdjk.com

[T34] Lua：遍历表
来源：http://nsx.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://iks.sxryk.cn

[T35] Lua：字典表
来源：http://pss.birdmap.top

local d = { a = 1 };  d.b = 2
来源：http://lqj.uphjek.com

[T36] Lua：函数
来源：http://bcd.cheryme.top

function add(a, b) return a + b end
来源：http://pmk.xziqi.cn

[T37] Lua：字符串拼接
来源：http://xjk.fanxiaobao.xyz

"a" .. "b"
来源：http://jcc.nwbrower.top

[T38] Lua：条件
来源：http://khy.dashuyun.cn

if x > 0 then print("正") end
来源：http://dvp.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://rnu.gzhubu.top

string.find(s, "%d+")
来源：http://ywj.zhixingplan.top

[T40] Lua：元表
来源：http://skc.hammf.cn

setmetatable({}, { __index = base })
来源：http://jkk.ywan-chungtsiang.top

[T41] Perl：Hello World
来源：http://cgz.chenjidiqi.icu

print "Hello\n";
来源：http://pye.ydzc1.top

[T42] Perl：变量类型
来源：http://wuq.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kie.hesvh.cn

[T43] Perl：字符串插值
来源：http://uij.zdbjq.cn

"值: $a"
来源：http://tqe.meibo888.top

[T44] Perl：条件
来源：http://sck.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://cyd.pycfn.com

[T45] Perl：数组遍历
来源：http://kqy.hammf.cn

for my $x (@arr) { print $x; }
来源：http://mrv.bjfxy.top

[T46] Perl：哈希操作
来源：http://dvf.hysaishi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hnz.cdnleiting.top

[T47] Perl：正则捕获
来源：http://ddm.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://efd.sxryk.cn

[T48] Perl：正则替换
来源：http://nda.tian-w.cn

$s =~ s/old/new/g;
来源：http://kui.sweek.top

[T49] Perl：函数
来源：http://eye.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://due.mhx1999.top

[T50] Perl：逐行读文件
来源：http://hay.yj202588.top

open my $fh, "<", "a.txt" or die $!;
来源：http://eal.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://kic.ydjk.org.cn

[T51] Scala：Hello World
来源：http://glu.jinqigufen.top

println("Hello")
来源：http://okd.shzxlz.cn

[T52] Scala：变量
来源：http://aii.ydzc1.top


<!-- 参考信息 -->