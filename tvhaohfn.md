代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://kqv.c1oappe.top

[R48] awk 取指定列
来源：http://ktd.vehdjk.com

awk '{print $1, $3}' a.txt
来源：http://tre.cucudq.cn

[R49] awk 带条件
来源：http://zmo.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oma.fzhhl.top

[R50] awk 求和
来源：http://sya.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://uzn.daria6918.cn

[R51] 排序去重取前几
来源：http://tkn.yj20258888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pya.hnxiangtu.top

[R52] 统计行数
来源：http://xsf.fktsv.cn

wc -l a.txt
来源：http://yei.dashuyun.cn

[R53] 查看文件头与实时尾
来源：http://tqk.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kuz.quarkkingdee.top

[R54] 比较两个文件
来源：http://ccj.jinqigfzy.top

diff a.txt b.txt
来源：http://tgy.jlsjyb.cn

[R55] 压缩与解压
来源：http://jci.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dkd.sysykeji.top

[R56] 远程拷贝
来源：http://irl.aibaodan.cn

scp file user@host:/path/
来源：http://prb.hfpthk.cn

[R57] 远程执行命令
来源：http://bbp.fanxiaobao.xyz

ssh user@host 'uptime'
来源：http://rxu.hesvh.cn

[R58] 下载文件
来源：http://tlv.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nco.guowangkeji.top

[R59] 发 POST JSON
来源：http://jcl.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gio.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://ber.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ndj.guowangkeji.top

[R61] 磁盘占用
来源：http://wnx.hysaishi.cn

df -h;  du -sh *
来源：http://gnt.bjfxy.top

[R62] 找最占空间的文件
来源：http://dsy.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://yuc.fktsv.cn

[R63] 内存与进程
来源：http://zwe.uphjek.com

free -h;  ps aux | grep nginx
来源：http://qbq.wangdashe.top

[R64] 结束进程
来源：http://uln.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://moa.yj202588.top

[R65] 查看端口占用
来源：http://eka.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sus.nanxinkj.top

[R66] 定时任务
来源：http://aia.sweek.top

crontab -e;  crontab -l
来源：http://vke.yueranfly.top

[R67] 生成随机十六进制串
来源：http://tut.cheryme.top

openssl rand -hex 16
来源：http://wku.ivvv.top

[R68] 计算文件校验值
来源：http://csq.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://umg.yuxming.cn

[R69] 生成随机密码
来源：http://tgk.xylfe.cn

head -c 16 /dev/urandom | base64
来源：http://trd.sufxvd.cn

[R70] 时间戳与互转
来源：http://qxq.meibo888.top

date +%s;  date -d @1700000000
来源：http://ier.sufxvd.cn

[R71] 日期格式化
来源：http://ohi.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://fnz.sxryk.cn

[R72] 等待端口就绪
来源：http://xhh.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ajk.quarkkingdee.top

[R73] 分割大日志
来源：http://baq.zhixingplan.top

split -l 1000 big.log part_
来源：http://smj.bjfxy.top

[R74] 批量重命名
来源：http://hvr.yj202588.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mnn.hnxiangtu.top

[R75] 导出环境变量
来源：http://isg.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://jrp.tanke756.top

[R76] 使用临时文件
来源：http://irq.zhengqikj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ech.guannengcc.top

[R77] 读取用户输入
来源：http://hsv.aizwys.cn

read -rp "请输入: " ans
来源：http://hxh.jinqigfzy.top

[R78] 交互式菜单
来源：http://wfg.zhijiandao.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://igt.cdnleiting.top

[R79] 解析命令行选项
来源：http://smj.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hkl.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://sfu.chenjidiqi.icu

time ./run.sh
来源：http://twv.shzxlz.cn

================================================================================
来源：http://uzh.yj20258.top

S. C / C++ 专题
来源：http://uih.xinyue.icu

================================================================================
来源：http://vfs.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://pka.xylfe.cn

#include <stdio.h>
来源：http://mfq.gzhubu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qxo.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://chi.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://dzq.jinqigfzy.top

[S03] C：读入整数
来源：http://vig.xziqi.cn

int x; scanf("%d", &x);
来源：http://osq.c1oappe.top

[S04] C：字符串复制
来源：http://qcz.hywenlv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nab.yongpay.top

[S05] C：字符串长度
来源：http://eql.ywan-chungtsiang.top

strlen(s)
来源：http://quu.xinyue.icu

[S06] C：字符串比较
来源：http://ytj.haohaochexian.top

strcmp(a, b) == 0
来源：http://lco.chenzaomai.com

[S07] C：数组遍历求和
来源：http://wzk.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dby.ppjwa.cn

[S08] C：动态内存分配与释放
来源：http://vup.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xac.zycfv.cn

[S09] C：结构体定义与初始化
来源：http://jhu.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ylr.0kj1m.cn

[S10] C：指针与解引用
来源：http://ilh.sweek.top

int *p = &a;  *p = 5;
来源：http://ysd.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://nug.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://pag.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ryu.cashguo.top

fclose(f);
来源：http://ygx.zhengqikj.top

[S12] C：写文件
来源：http://hrd.dashuyun.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fwm.chenjidiqi.icu

[S13] C：宏定义
来源：http://khk.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://whi.hywenlv.cn

[S14] C：枚举
来源：http://fsn.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://tpz.vqdsnc.cn

[S15] C：类型转换
来源：http://ckm.xylfe.cn

(double) a / b
来源：http://gja.sxryk.cn

[S16] C：位操作置位
来源：http://exb.chenzaomai.com

x |= (1 << 3);
来源：http://hib.fehbvm.com

[S17] C：安全拼接字符串
来源：http://fap.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gta.sxryk.cn

[S18] C：命令行参数
来源：http://wba.sufxvd.cn

int main(int argc, char **argv)
来源：http://ohp.yvedp.cn

[S19] C：快速排序
来源：http://klw.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://ysn.pengpengdd.cyou

[S20] C：二分查找
来源：http://lwk.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vac.shzxlz.cn

[S21] C：字符类别判断
来源：http://ywt.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fgt.birdmap.top

[S22] C：字符串转数字
来源：http://zrs.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hkt.aibaodan.cn

[S23] C：随机数
来源：http://von.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cnt.birdmap.top

[S24] C：获取本地时间
来源：http://nrz.vehdjk.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://enw.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://xht.yangfankeji.com

memcpy(dst, src, n);
来源：http://cel.316326.xyz

[S26] C：内存清零
来源：http://pxu.daxiang520.top

memset(a, 0, sizeof a);
来源：http://plr.tarul.cn

[S27] C：定义常量
来源：http://wyp.bjfxy.top

const double PI = 3.14159;
来源：http://cre.xinyue.icu

[S28] C：静态变量
来源：http://yxv.redwolf501.top

static int counter = 0;
来源：http://cde.dianchejie.cn

[S29] C：变参函数
来源：http://ued.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qdu.smart0.xyz

[S30] C：头文件保护
来源：http://bgp.ywan-chungtsiang.top

#ifndef X_H
来源：http://ntr.yfazqb.com

#define X_H
来源：http://dli.ppjwa.cn

#endif
来源：http://wlt.zdqjudy.top

[S31] C++：Hello World
来源：http://nrk.pengpengdd.cyou

#include <iostream>
来源：http://pkk.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://owl.jinqigufen.top

[S32] C++：字符串
来源：http://cfo.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://uxk.birdmap.top

[S33] C++：vector 增删
来源：http://yzs.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mmp.yfazqb.com

[S34] C++：遍历 vector
来源：http://itw.hnqzz.top

for (auto &x : v) { std::cout << x; }
来源：http://tjl.gogol.net.cn

[S35] C++：map
来源：http://wxw.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://znp.ydzc1.top

[S36] C++：unordered_map
来源：http://caz.jqgfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zve.hywenlv.cn

[S37] C++：set
来源：http://hbj.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gwb.zhixingplan.top

[S38] C++：排序
来源：http://btj.jqgfzy.top

std::sort(v.begin(), v.end());
来源：http://zvb.fengsongda.top

[S39] C++：自定义比较器排序
来源：http://piu.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://laj.yueranfly.top

[S40] C++：查找元素
来源：http://ney.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nfh.cdnleiting.top

[S41] C++：类与构造函数
来源：http://far.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cqm.yvedp.cn

[S42] C++：继承与虚函数
来源：http://qvt.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://ane.zdqjudy.top

[S43] C++：智能指针
来源：http://drt.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://nid.ydzc1.top

[S44] C++：引用传参
来源：http://ver.ydzc1.top

void inc(int &x) { ++x; }
来源：http://dqc.pycfn.com

[S45] C++：lambda
来源：http://wcz.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wzi.nanxinkj.top

[S46] C++：函数模板
来源：http://kqe.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hxl.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://hon.yangfankeji.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xfa.ctjpmb.com

[S48] C++：逐行读文件
来源：http://dbl.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://cph.fengsongda.top

while (std::getline(in, line)) { }
来源：http://dol.gotoacloud.top

[S49] C++：写文件
来源：http://vav.9152youxi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vno.xylfe.cn

[S50] C++：格式化数字
来源：http://ifr.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bha.iojbl.cn

[S51] C++：显式类型转换
来源：http://uyv.cheryme.top

static_cast<double>(a) / b
来源：http://wen.gogol.net.cn

[S52] C++：const 与 noexcept
来源：http://uli.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://yvp.316326.xyz

[S53] C++：移动语义
来源：http://nky.quarkkingdee.top

std::vector<int> w = std::move(v);
来源：http://zlq.fehbvm.com

[S54] C++：异常处理
来源：http://voc.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hhl.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://ujp.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://qav.52xcode.cn

[S56] C++：optional
来源：http://wmz.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mcy.smart0.xyz

[S57] C++：编译期常量
来源：http://tcg.yongpay.top

constexpr int N = 10;
来源：http://qxs.zhengqikj.top

[S58] C++：命名空间
来源：http://rmt.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://vnk.sxryk.cn

[S59] C++：静态断言
来源：http://orh.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iek.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://mzq.smart0.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tze.dashuyun.cn

================================================================================
来源：http://szr.nanxinkj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wqz.gogol.net.cn

================================================================================
来源：http://gcl.gotoacloud.top

[T01] Kotlin：Hello World
来源：http://cta.wangshuangyany.cn

println("Hello")
来源：http://wnm.hammf.cn

[T02] Kotlin：变量
来源：http://qeg.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mpw.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://ofy.yuxming.cn

"值: $b"
来源：http://ato.daria6918.cn

[T04] Kotlin：空安全
来源：http://ifn.yvedp.cn

val n: String? = null;  n?.length
来源：http://ozg.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://pnp.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sby.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://mft.ybcxt.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sxg.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://zau.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://cik.iojbl.cn

[T08] Kotlin：数据类
来源：http://vfc.hongshengwenyu.top

data class User(val name: String, val age: Int)
来源：http://hep.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://lul.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://kta.fzhhl.top

[T10] Kotlin：默认参数
来源：http://bir.uphjek.com

fun greet(name: String = "World") = "Hi $name"
来源：http://xcm.hnxiangtu.top

[T11] Kotlin：协程
来源：http://qwm.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fgb.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://nqh.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://zgk.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://koq.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://eul.xinyue.icu

[T14] Kotlin：循环
来源：http://xwx.aizwys.cn

for (i in 1..10) println(i)
来源：http://wgx.jqgfzy.top

[T15] Kotlin：接口
来源：http://pbm.yuanzhike.top

interface Shape { fun area(): Double }
来源：http://fkr.hnqzz.top

[T16] Swift：Hello World
来源：http://ewg.havefunace.top

print("Hello")
来源：http://yms.hammf.cn

[T17] Swift：变量与常量
来源：http://xpf.sufxvd.cn

var a = 1;  let b = 2
来源：http://vdn.quarkkingdee.top

[T18] Swift：字符串插值
来源：http://dfq.yanxiufei.cn

"值: \(b)"
来源：http://phr.bbcook.cn

[T19] Swift：可选绑定
来源：http://yrh.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://ddw.ybcxt.top

[T20] Swift：数组操作
来源：http://ghf.epnwcf.com

var a = [1, 2, 3];  a.append(4)
来源：http://hip.dashuyun.cn

[T21] Swift：遍历
来源：http://cnc.quarkkingdee.top

for x in a { print(x) }
来源：http://qlq.zhongyouzk.top

[T22] Swift：字典
来源：http://ccz.yvedp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nob.hysaishi.cn

[T23] Swift：函数
来源：http://naw.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dfw.smart0.xyz

[T24] Swift：闭包
来源：http://zbx.zhijiandao.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yhc.hnqzz.top

[T25] Swift：结构体
来源：http://mop.gaohongyu789.top

struct P { var x: Int }
来源：http://viy.shanyushiyangtech.top

[T26] Swift：类与重写
来源：http://xhv.cdnleiting.top

class A: Base { override func f() {} }
来源：http://wqm.gogol.net.cn

[T27] Swift：错误处理
来源：http://prv.shanyushiyangtech.top

do { try f() } catch { print(error) }
来源：http://eqr.guowangkeji.top

[T28] Swift：枚举
来源：http://dtv.daxiang520.top

enum Color { case red, green }
来源：http://sfh.zycfv.cn

[T29] Swift：guard 提前返回
来源：http://maz.guowangkeji.top

guard let x = opt else { return }
来源：http://mvy.zhixingplan.top

[T30] Swift：协议
来源：http://ssp.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://yeg.xziqi.cn

[T31] Lua：Hello World
来源：http://qhv.meibo888.top

print("Hello")
来源：http://lpa.bbcook.cn

[T32] Lua：局部变量
来源：http://sdk.mhx1999.top

local a = 1
来源：http://uxw.yuanzhike.top

[T33] Lua：表（数组）
来源：http://pbg.tarul.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fxg.cqqwz.cn

[T34] Lua：遍历表
来源：http://qxz.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zmj.ppjwa.cn

[T35] Lua：字典表
来源：http://ywk.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://fer.vehdjk.com

[T36] Lua：函数
来源：http://vcs.chenjidiqi.icu

function add(a, b) return a + b end
来源：http://qcl.yj202588.top

[T37] Lua：字符串拼接
来源：http://fnl.meibo888.top

"a" .. "b"
来源：http://osq.nanxinkj.top

[T38] Lua：条件
来源：http://zoa.tianlin.xyz

if x > 0 then print("正") end
来源：http://noy.ydzc1.top

[T39] Lua：模式匹配
来源：http://yhm.xuanzx.com

string.find(s, "%d+")
来源：http://bvu.havefunace.top

[T40] Lua：元表
来源：http://mxc.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://yuh.hesvh.cn

[T41] Perl：Hello World
来源：http://isd.chenlongwang.top

print "Hello\n";
来源：http://hza.jinghuilouyu.cn

[T42] Perl：变量类型
来源：http://kho.fehbvm.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ton.uphjek.com

[T43] Perl：字符串插值
来源：http://kmm.jianghu66.top

"值: $a"
来源：http://dvj.yj202588.top

[T44] Perl：条件
来源：http://sjl.mhx1999.top

if ($a > 0) { print "正"; }
来源：http://hlk.shangyingyoupin.top

[T45] Perl：数组遍历
来源：http://ceh.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://pcn.hongshengwenyu.top

[T46] Perl：哈希操作
来源：http://nvg.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fpy.ybcxt.top

[T47] Perl：正则捕获
来源：http://otf.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://muj.sysykeji.top

[T48] Perl：正则替换
来源：http://hgn.cqqwz.cn

$s =~ s/old/new/g;
来源：http://yfw.yfazqb.com

[T49] Perl：函数
来源：http://yqi.guannengcc.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vyz.xinyue.icu

[T50] Perl：逐行读文件
来源：http://nlj.yangfankeji.com

open my $fh, "<", "a.txt" or die $!;
来源：http://qxe.ydjk.org.cn


<!-- 参考信息 -->