代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dbb.shanyushiyangkeji.top

[R50] awk 求和
来源：http://zwn.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://blm.tian-w.cn

[R51] 排序去重取前几
来源：http://juw.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://euf.hesvh.cn

[R52] 统计行数
来源：http://mzz.zhijiandao.cn

wc -l a.txt
来源：http://zkd.birdmap.top

[R53] 查看文件头与实时尾
来源：http://gwe.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tfc.ehwqpu.com

[R54] 比较两个文件
来源：http://xea.kuanghao11.cn

diff a.txt b.txt
来源：http://bjy.uphjek.com

[R55] 压缩与解压
来源：http://htr.chenjidiqi.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jks.wangdashe.top

[R56] 远程拷贝
来源：http://vfp.fktsv.cn

scp file user@host:/path/
来源：http://knj.gzhubu.top

[R57] 远程执行命令
来源：http://wgj.cashguo.top

ssh user@host 'uptime'
来源：http://rdt.mhx1999.top

[R58] 下载文件
来源：http://xpk.xziqi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://emz.tanke756.top

[R59] 发 POST JSON
来源：http://mxe.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wuj.bbcook.cn

[R60] 只看 HTTP 状态码
来源：http://qxn.ppjwa.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hsc.haohaochexian.top

[R61] 磁盘占用
来源：http://sny.quarkkingdee.top

df -h;  du -sh *
来源：http://rmh.zycfv.cn

[R62] 找最占空间的文件
来源：http://srl.jinghuilouyu.cn

du -ah . | sort -rh | head -10
来源：http://mjv.birdmap.top

[R63] 内存与进程
来源：http://tim.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://jhf.smart0.xyz

[R64] 结束进程
来源：http://zgs.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://fym.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://jpl.sxryk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dkz.cucudq.cn

[R66] 定时任务
来源：http://mwn.sweek.top

crontab -e;  crontab -l
来源：http://duq.hywenlv.cn

[R67] 生成随机十六进制串
来源：http://zvp.jyoumei.cn

openssl rand -hex 16
来源：http://xim.epnwcf.com

[R68] 计算文件校验值
来源：http://ips.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://mwb.ydjk.org.cn

[R69] 生成随机密码
来源：http://kot.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://png.yfazqb.com

[R70] 时间戳与互转
来源：http://wti.jqgufenzy.top

date +%s;  date -d @1700000000
来源：http://lyt.sweek.top

[R71] 日期格式化
来源：http://ils.gaohongyu789.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qov.vqdsnc.cn

[R72] 等待端口就绪
来源：http://gwa.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://znd.shangyingyoupin.top

[R73] 分割大日志
来源：http://xwt.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://ewh.zhixingplan.top

[R74] 批量重命名
来源：http://enj.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ycw.sweek.top

[R75] 导出环境变量
来源：http://hlr.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://byj.zhijiandao.cn

[R76] 使用临时文件
来源：http://ipb.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://poj.fktsv.cn

[R77] 读取用户输入
来源：http://kdr.jqgufenzy.top

read -rp "请输入: " ans
来源：http://muy.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://dpt.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://iwn.zhoulong.xyz

[R79] 解析命令行选项
来源：http://cmu.cheryme.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sol.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://ndj.ehwqpu.com

time ./run.sh
来源：http://jeg.cheryme.top

================================================================================
来源：http://ivs.xziqi.cn

S. C / C++ 专题
来源：http://jid.hnqzz.top

================================================================================
来源：http://yat.uphjek.com

[S01] C：Hello World
来源：http://dbc.redwolf501.top

#include <stdio.h>
来源：http://vfr.yj20258888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bjm.mhx1999.top

[S02] C：变量与格式化输出
来源：http://onx.nanxinkj.top

int a = 10; printf("%d\n", a);
来源：http://hko.sysykeji.top

[S03] C：读入整数
来源：http://oua.yj20258.top

int x; scanf("%d", &x);
来源：http://lto.feifeiyinyue.top

[S04] C：字符串复制
来源：http://znq.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://lqb.hongshengwenyu.top

[S05] C：字符串长度
来源：http://hog.fktsv.cn

strlen(s)
来源：http://dls.vqdsnc.cn

[S06] C：字符串比较
来源：http://wbg.316326.xyz

strcmp(a, b) == 0
来源：http://npz.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://xzl.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://meq.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://yal.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cwf.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://fpg.nanxuanxn.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kiy.daxiang520.top

[S10] C：指针与解引用
来源：http://zxx.sufxvd.cn

int *p = &a;  *p = 5;
来源：http://iru.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://srs.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://csv.jianghu66.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ahp.jqgfzy.top

fclose(f);
来源：http://xiz.dianchejie.cn

[S12] C：写文件
来源：http://skk.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dot.yj20258.top

[S13] C：宏定义
来源：http://aec.fengsongda.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wvn.9152youxi.cn

[S14] C：枚举
来源：http://clt.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://iln.yangfankeji.com

[S15] C：类型转换
来源：http://usk.jinqigfzy.top

(double) a / b
来源：http://phd.daria6918.cn

[S16] C：位操作置位
来源：http://sdk.zhoulong.xyz

x |= (1 << 3);
来源：http://lyd.andypj.xyz

[S17] C：安全拼接字符串
来源：http://qck.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lrc.bbcook.cn

[S18] C：命令行参数
来源：http://dqz.zhoulong.xyz

int main(int argc, char **argv)
来源：http://aql.nwbrower.top

[S19] C：快速排序
来源：http://yxw.nwbrower.top

qsort(a, n, sizeof(int), cmp);
来源：http://jwg.ctjpmb.com

[S20] C：二分查找
来源：http://udn.vehdjk.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://duv.meibo888.top

[S21] C：字符类别判断
来源：http://zlf.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wxm.xinyue.icu

[S22] C：字符串转数字
来源：http://qyn.52xcode.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uos.zhaomingkeji.xyz

[S23] C：随机数
来源：http://her.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sqq.ehwqpu.com

[S24] C：获取本地时间
来源：http://wuv.cdnleiting.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zzv.shzxlz.cn

[S25] C：内存拷贝
来源：http://igi.daxiang520.top

memcpy(dst, src, n);
来源：http://uuv.havefunace.top

[S26] C：内存清零
来源：http://xme.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://tyz.dashuyun.cn

[S27] C：定义常量
来源：http://qug.tianlin.xyz

const double PI = 3.14159;
来源：http://lno.vehdjk.com

[S28] C：静态变量
来源：http://flp.yfazqb.com

static int counter = 0;
来源：http://rqp.smart0.xyz

[S29] C：变参函数
来源：http://gvk.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://asv.cdnleiting.top

[S30] C：头文件保护
来源：http://rrc.cucudq.cn

#ifndef X_H
来源：http://xqy.svipenyu.cn

#define X_H
来源：http://oga.yuxming.cn

#endif
来源：http://gdg.chenlongwang.top

[S31] C++：Hello World
来源：http://quy.aibaodan.cn

#include <iostream>
来源：http://mzx.nwbrower.top

int main() { std::cout << "Hello\n"; }
来源：http://iky.ctjpmb.com

[S32] C++：字符串
来源：http://jxn.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://arc.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://rfv.ppjwa.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mjq.yongpay.top

[S34] C++：遍历 vector
来源：http://wwf.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://fmc.shzxlz.cn

[S35] C++：map
来源：http://tna.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uck.nwbrower.top

[S36] C++：unordered_map
来源：http://qoj.ehwqpu.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gay.yonumen.top

[S37] C++：set
来源：http://xdy.havefunace.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://drd.sjlbkw.cn

[S38] C++：排序
来源：http://lpr.jiagoushi.top

std::sort(v.begin(), v.end());
来源：http://zmp.vqdsnc.cn

[S39] C++：自定义比较器排序
来源：http://kbe.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kxs.chenjidiqi.icu

[S40] C++：查找元素
来源：http://cxx.hywenlv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jza.hnqzz.top

[S41] C++：类与构造函数
来源：http://kwi.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bxs.zdbjq.cn

[S42] C++：继承与虚函数
来源：http://mub.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://oxk.dianchejie.cn

[S43] C++：智能指针
来源：http://ggm.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://eie.52xcode.cn

[S44] C++：引用传参
来源：http://hwj.chenlongwang.top

void inc(int &x) { ++x; }
来源：http://ywd.nanxuanxn.top

[S45] C++：lambda
来源：http://hef.iojbl.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tir.316326.xyz

[S46] C++：函数模板
来源：http://lvj.chenjidiqi.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cxp.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://wph.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xce.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://ucd.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://mcd.gotoacloud.top

while (std::getline(in, line)) { }
来源：http://tyf.ppjwa.cn

[S49] C++：写文件
来源：http://dht.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jwy.zdbjq.cn

[S50] C++：格式化数字
来源：http://hev.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ksb.hysaishi.cn

[S51] C++：显式类型转换
来源：http://lkc.bjfxy.top

static_cast<double>(a) / b
来源：http://cji.svipenyu.cn

[S52] C++：const 与 noexcept
来源：http://yyl.yj202588.top

int size() const noexcept { return n_; }
来源：http://lvf.ehwqpu.com

[S53] C++：移动语义
来源：http://egv.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://gld.jianghu66.top

[S54] C++：异常处理
来源：http://azr.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zah.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://plo.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gqv.ivvv.top

[S56] C++：optional
来源：http://hvw.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://boj.redwolf501.top

[S57] C++：编译期常量
来源：http://fby.epnwcf.com

constexpr int N = 10;
来源：http://tom.fehbvm.com

[S58] C++：命名空间
来源：http://jpq.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://mns.yonumen.top

[S59] C++：静态断言
来源：http://eio.vehdjk.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rru.hcnkem.com

[S60] C++：遍历并删除元素
来源：http://rrf.hammf.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gfe.hywenlv.cn

================================================================================
来源：http://gso.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pyx.hongshengwenyu.top

================================================================================
来源：http://ahj.nanxuanxn.top

[T01] Kotlin：Hello World
来源：http://aws.andypj.xyz

println("Hello")
来源：http://tqu.xinyue.icu

[T02] Kotlin：变量
来源：http://iug.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wyp.meibo888.top

[T03] Kotlin：字符串模板
来源：http://xps.nwbrower.top

"值: $b"
来源：http://ala.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://bcp.shzxlz.cn

val n: String? = null;  n?.length
来源：http://ywj.sjlbkw.cn

[T05] Kotlin：when 表达式
来源：http://jvy.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fif.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://ere.dianchejie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pia.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://lby.uphjek.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://bel.yongpay.top

[T08] Kotlin：数据类
来源：http://ryn.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://szv.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://zyr.hfpthk.cn

fun String.exclaim() = this + "!"
来源：http://ncg.316326.xyz

[T10] Kotlin：默认参数
来源：http://zog.jiagoushi.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mnj.bbcook.cn

[T11] Kotlin：协程
来源：http://raj.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eby.yongpay.top

[T12] Kotlin：解构声明
来源：http://jru.fktsv.cn

val (a, b) = Pair(1, 2)
来源：http://oqc.jianghu66.top

[T13] Kotlin：只读 Map
来源：http://jfc.yj20258888.top

val m = mapOf("a" to 1)
来源：http://yql.yj202588.top

[T14] Kotlin：循环
来源：http://fvc.hnqzz.top

for (i in 1..10) println(i)
来源：http://gli.jinqigufen.top

[T15] Kotlin：接口
来源：http://qve.yfazqb.com

interface Shape { fun area(): Double }
来源：http://dww.yuxming.cn

[T16] Swift：Hello World
来源：http://mlz.jyoumei.cn

print("Hello")
来源：http://clt.dashuyun.cn

[T17] Swift：变量与常量
来源：http://qub.cqqwz.cn

var a = 1;  let b = 2
来源：http://jkf.xziqi.cn

[T18] Swift：字符串插值
来源：http://oxp.hammf.cn

"值: \(b)"
来源：http://lmd.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://mjv.xuetiantiany.cn

if let n = opt { print(n) }
来源：http://zgm.havefunace.top

[T20] Swift：数组操作
来源：http://yoj.chenzaomai.com

var a = [1, 2, 3];  a.append(4)
来源：http://gma.yvedp.cn

[T21] Swift：遍历
来源：http://ntx.zhengqikj.top

for x in a { print(x) }
来源：http://dav.cucudq.cn

[T22] Swift：字典
来源：http://syp.chenzaomai.com

var d = ["a": 1];  d["b"] = 2
来源：http://ozn.ydzc1.top

[T23] Swift：函数
来源：http://zvp.smart0.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vzb.yuanzhike.top

[T24] Swift：闭包
来源：http://uhr.xuanzx.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://dxc.shangyingyoupin.top

[T25] Swift：结构体
来源：http://acm.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://xji.nwbrower.top

[T26] Swift：类与重写
来源：http://fes.nwbrower.top

class A: Base { override func f() {} }
来源：http://fdk.yj20258888.top

[T27] Swift：错误处理
来源：http://cyh.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://tgg.hywenlv.cn

[T28] Swift：枚举
来源：http://kbw.gzhubu.top

enum Color { case red, green }
来源：http://yac.guowangkeji.top

[T29] Swift：guard 提前返回
来源：http://abi.birdmap.top

guard let x = opt else { return }
来源：http://sqm.cqqwz.cn

[T30] Swift：协议
来源：http://jjq.jinqigfzy.top

protocol Shape { func area() -> Double }
来源：http://gtx.gogol.net.cn

[T31] Lua：Hello World
来源：http://smf.shanyushiyangkeji.top

print("Hello")
来源：http://iip.jianghu66.top

[T32] Lua：局部变量
来源：http://eih.jinghuilouyu.cn

local a = 1
来源：http://jmd.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://vgc.zhoulong.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://bwf.shanyushiyangkeji.top

[T34] Lua：遍历表
来源：http://ajd.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rao.cheryme.top

[T35] Lua：字典表
来源：http://uuu.zhengqikj.top

local d = { a = 1 };  d.b = 2
来源：http://ehy.nwbrower.top

[T36] Lua：函数
来源：http://xny.hesvh.cn

function add(a, b) return a + b end
来源：http://dwk.feifeiyinyue.top

[T37] Lua：字符串拼接
来源：http://tzf.ppjwa.cn

"a" .. "b"
来源：http://mvw.ywan-chungtsiang.top

[T38] Lua：条件
来源：http://yhb.yj202588.top

if x > 0 then print("正") end
来源：http://vij.ctjpmb.com

[T39] Lua：模式匹配
来源：http://oqf.snrcjt.cn

string.find(s, "%d+")
来源：http://ufl.epnwcf.com

[T40] Lua：元表
来源：http://fno.cucudq.cn

setmetatable({}, { __index = base })
来源：http://yey.dianchejie.cn

[T41] Perl：Hello World
来源：http://rhs.guannengcc.top

print "Hello\n";
来源：http://rug.gzhubu.top

[T42] Perl：变量类型
来源：http://oih.jinghuilouyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qwl.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://npf.jlsjyb.cn

"值: $a"
来源：http://zau.hfpthk.cn

[T44] Perl：条件
来源：http://mqk.ybcxt.top

if ($a > 0) { print "正"; }
来源：http://ozh.hnxiangtu.top

[T45] Perl：数组遍历
来源：http://rwm.tarul.cn

for my $x (@arr) { print $x; }
来源：http://iql.ctjpmb.com

[T46] Perl：哈希操作
来源：http://rte.hnxiangtu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gjj.bbcook.cn

[T47] Perl：正则捕获
来源：http://lob.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gqe.daria6918.cn

[T48] Perl：正则替换
来源：http://ylt.hesvh.cn

$s =~ s/old/new/g;
来源：http://hgr.hongshengwenyu.top

[T49] Perl：函数
来源：http://avg.xylfe.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lcp.wangdashe.top

[T50] Perl：逐行读文件
来源：http://uxi.yanxiufei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cdj.jinqigfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://fec.c1oappe.top

[T51] Scala：Hello World
来源：http://fwt.zhiwuduotai.top

println("Hello")
来源：http://ewg.zycfv.cn

[T52] Scala：变量
来源：http://kkz.cheryme.top


<!-- 参考信息 -->