代发 wailian999

cmd > out.log 2>&1
来源：http://zwr.epnwcf.com

[R40] 追加写日志
来源：http://mwg.aizwys.cn

echo "log" >> out.log
来源：http://wkn.tianlin.xyz

[R41] 丢弃输出
来源：http://btn.gzhubu.top

cmd >/dev/null 2>&1
来源：http://yyt.yj20258.top

[R42] 输入重定向
来源：http://ygs.0kj1m.cn

wc -l < a.txt
来源：http://riz.hesvh.cn

[R43] 按名字查找文件
来源：http://lap.fanxiaobao.xyz

find . -name "*.log" -type f
来源：http://gkm.hongshengwenyu.top

[R44] 按修改时间查找
来源：http://oby.yanxiufei.cn

find . -mtime -7 -type f
来源：http://nqc.shangyingyoupin.top

[R45] 批量删除
来源：http://wrs.pycfn.com

find . -name "*.tmp" -delete
来源：http://grv.zhixingplan.top

[R46] 递归替换文件内容
来源：http://pkx.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mcv.tanke756.top

[R47] sed 单行替换
来源：http://vjz.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://how.sufxvd.cn

[R48] awk 取指定列
来源：http://kas.hcnkem.com

awk '{print $1, $3}' a.txt
来源：http://mwt.iojbl.cn

[R49] awk 带条件
来源：http://jah.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dir.jlsjyb.cn

[R50] awk 求和
来源：http://gnw.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://baw.dashuyun.cn

[R51] 排序去重取前几
来源：http://gdh.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qgt.sweek.top

[R52] 统计行数
来源：http://ylh.hnqzz.top

wc -l a.txt
来源：http://vst.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://mht.snrcjt.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zco.cheryme.top

[R54] 比较两个文件
来源：http://cny.shanyushiyangtech.top

diff a.txt b.txt
来源：http://ale.gaohongyu789.top

[R55] 压缩与解压
来源：http://mtw.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kjy.jianghu66.top

[R56] 远程拷贝
来源：http://wry.gzhubu.top

scp file user@host:/path/
来源：http://yyi.bjfxy.top

[R57] 远程执行命令
来源：http://loa.iojbl.cn

ssh user@host 'uptime'
来源：http://qky.shanyushiyangtech.top

[R58] 下载文件
来源：http://hjc.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ahl.snrcjt.cn

[R59] 发 POST JSON
来源：http://cva.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dmj.tian-w.cn

[R60] 只看 HTTP 状态码
来源：http://sym.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qze.jyoumei.cn

[R61] 磁盘占用
来源：http://icg.tianlin.xyz

df -h;  du -sh *
来源：http://ebj.yvedp.cn

[R62] 找最占空间的文件
来源：http://ben.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://utl.yj20258.top

[R63] 内存与进程
来源：http://cse.hfpthk.cn

free -h;  ps aux | grep nginx
来源：http://rmh.9152youxi.cn

[R64] 结束进程
来源：http://amb.ehwqpu.com

kill -9 $(pgrep -f app.py)
来源：http://eou.ydjk.org.cn

[R65] 查看端口占用
来源：http://lna.zhongyouzk.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kja.hnqzz.top

[R66] 定时任务
来源：http://wqc.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://nex.jianghu66.top

[R67] 生成随机十六进制串
来源：http://wrr.ctjpmb.com

openssl rand -hex 16
来源：http://tal.hnxiangtu.top

[R68] 计算文件校验值
来源：http://noi.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://qlt.hnqzz.top

[R69] 生成随机密码
来源：http://udk.yanxiufei.cn

head -c 16 /dev/urandom | base64
来源：http://edp.hnxiangtu.top

[R70] 时间戳与互转
来源：http://pxj.yj202588.top

date +%s;  date -d @1700000000
来源：http://jsl.zhongyouzk.top

[R71] 日期格式化
来源：http://elw.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wkb.shangyingyoupin.top

[R72] 等待端口就绪
来源：http://nqi.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://iwu.xuetiantiany.cn

[R73] 分割大日志
来源：http://ffw.yvedp.cn

split -l 1000 big.log part_
来源：http://yjp.pycfn.com

[R74] 批量重命名
来源：http://iwl.redwolf501.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://max.cdnleiting.top

[R75] 导出环境变量
来源：http://eej.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://vka.smart0.xyz

[R76] 使用临时文件
来源：http://ukf.c1oappe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wwx.uphjek.com

[R77] 读取用户输入
来源：http://kob.vqdsnc.cn

read -rp "请输入: " ans
来源：http://jdj.yongpay.top

[R78] 交互式菜单
来源：http://jpf.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fih.aibaodan.cn

[R79] 解析命令行选项
来源：http://pnf.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iiu.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://udr.fzhhl.top

time ./run.sh
来源：http://srq.gogol.net.cn

================================================================================
来源：http://qlq.yueranfly.top

S. C / C++ 专题
来源：http://erd.zhaomingkeji.xyz

================================================================================
来源：http://yus.ctjpmb.com

[S01] C：Hello World
来源：http://wvm.kuanghao11.cn

#include <stdio.h>
来源：http://cta.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fxh.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://xrc.gogol.net.cn

int a = 10; printf("%d\n", a);
来源：http://tsw.gzhubu.top

[S03] C：读入整数
来源：http://sps.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://xyg.iojbl.cn

[S04] C：字符串复制
来源：http://yuk.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://uqj.gaohongyu789.top

[S05] C：字符串长度
来源：http://ujw.9152youxi.cn

strlen(s)
来源：http://ook.iojbl.cn

[S06] C：字符串比较
来源：http://lwm.hfpthk.cn

strcmp(a, b) == 0
来源：http://fuo.shanyushiyangtech.top

[S07] C：数组遍历求和
来源：http://tdz.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eiz.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://bzr.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xji.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://zes.chenlongwang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iro.bjfxy.top

[S10] C：指针与解引用
来源：http://rzd.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://oxx.sjlbkw.cn

[S11] C：逐行读文件
来源：http://zag.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://soe.chenzaomai.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://wdn.bbcook.cn

fclose(f);
来源：http://yee.ywan-chungtsiang.top

[S12] C：写文件
来源：http://dun.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sot.ivvv.top

[S13] C：宏定义
来源：http://wlo.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bij.xuetiantiany.cn

[S14] C：枚举
来源：http://wkd.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://hnl.hesvh.cn

[S15] C：类型转换
来源：http://vfd.tian-w.cn

(double) a / b
来源：http://qgi.yonumen.top

[S16] C：位操作置位
来源：http://sgm.shuidangran.top

x |= (1 << 3);
来源：http://dfp.fzhhl.top

[S17] C：安全拼接字符串
来源：http://gvq.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tfa.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://xvl.xylfe.cn

int main(int argc, char **argv)
来源：http://gaj.yonumen.top

[S19] C：快速排序
来源：http://pmv.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://jlv.zhixingplan.top

[S20] C：二分查找
来源：http://uil.316326.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://new.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://wxg.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bsr.quarkkingdee.top

[S22] C：字符串转数字
来源：http://gps.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://lqf.guowangkeji.top

[S23] C：随机数
来源：http://qtp.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kiq.dashuyun.cn

[S24] C：获取本地时间
来源：http://nwl.sweek.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eip.svipenyu.cn

[S25] C：内存拷贝
来源：http://poa.ydzc1.top

memcpy(dst, src, n);
来源：http://scr.zhijiandao.cn

[S26] C：内存清零
来源：http://tvh.hnqzz.top

memset(a, 0, sizeof a);
来源：http://dkg.kuanghao11.cn

[S27] C：定义常量
来源：http://oip.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://fva.cashguo.top

[S28] C：静态变量
来源：http://znk.vehdjk.com

static int counter = 0;
来源：http://dqu.jqgufenzy.top

[S29] C：变参函数
来源：http://vcn.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wyh.hammf.cn

[S30] C：头文件保护
来源：http://aho.vqdsnc.cn

#ifndef X_H
来源：http://rrr.ehwqpu.com

#define X_H
来源：http://lru.shuidangran.top

#endif
来源：http://jbt.xziqi.cn

[S31] C++：Hello World
来源：http://nre.sweek.top

#include <iostream>
来源：http://zli.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://cmf.zhijiandao.cn

[S32] C++：字符串
来源：http://iyc.yonumen.top

std::string s = "hi";  s += "!";
来源：http://uga.sysykeji.top

[S33] C++：vector 增删
来源：http://ren.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cxk.shangyingyoupin.top

[S34] C++：遍历 vector
来源：http://zko.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://huw.birdmap.top

[S35] C++：map
来源：http://uiy.ppjwa.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bqt.nanxuanxn.top

[S36] C++：unordered_map
来源：http://bgq.zhixingplan.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rnd.zhijiandao.cn

[S37] C++：set
来源：http://xbh.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://apa.jlsjyb.cn

[S38] C++：排序
来源：http://roc.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://quf.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://yxn.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nha.hfpthk.cn

[S40] C++：查找元素
来源：http://ngk.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hcd.aibaodan.cn

[S41] C++：类与构造函数
来源：http://fnu.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aib.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://qhm.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://ajy.smart0.xyz

[S43] C++：智能指针
来源：http://rly.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://egn.yuxming.cn

[S44] C++：引用传参
来源：http://vjl.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://qfm.hcnkem.com

[S45] C++：lambda
来源：http://eyq.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://zws.fzhhl.top

[S46] C++：函数模板
来源：http://oqt.kuanghao11.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jld.aizwys.cn

[S47] C++：结构化绑定遍历
来源：http://tus.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bcp.tarul.cn

[S48] C++：逐行读文件
来源：http://pad.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://esh.yueranfly.top

while (std::getline(in, line)) { }
来源：http://jfa.shanyushiyangtech.top

[S49] C++：写文件
来源：http://ijo.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://svo.chenlongwang.top

[S50] C++：格式化数字
来源：http://lkk.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xxz.shanyushiyangkeji.top

[S51] C++：显式类型转换
来源：http://rsg.zhoulong.xyz

static_cast<double>(a) / b
来源：http://kal.fehbvm.com

[S52] C++：const 与 noexcept
来源：http://urx.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://hoz.ydzc1.top

[S53] C++：移动语义
来源：http://xgw.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://box.yuxming.cn

[S54] C++：异常处理
来源：http://azf.9152youxi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qqa.xuanzx.com

[S55] C++：结构化绑定
来源：http://xba.hnqzz.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qha.daxiang520.top

[S56] C++：optional
来源：http://rsh.pycfn.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dwo.fktsv.cn

[S57] C++：编译期常量
来源：http://jnu.smart0.xyz

constexpr int N = 10;
来源：http://mcn.jlsjyb.cn

[S58] C++：命名空间
来源：http://hak.cucudq.cn

namespace ns { int f() { return 1; } }
来源：http://iho.yj202588.top

[S59] C++：静态断言
来源：http://ftz.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nva.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://mxz.ywan-chungtsiang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zeh.quarkkingdee.top

================================================================================
来源：http://cgo.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lue.hnqzz.top

================================================================================
来源：http://gtw.cucudq.cn

[T01] Kotlin：Hello World
来源：http://yhn.smart0.xyz

println("Hello")
来源：http://ygv.aizwys.cn

[T02] Kotlin：变量
来源：http://wmg.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lxp.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://flj.mhx1999.top

"值: $b"
来源：http://xyd.bbcook.cn

[T04] Kotlin：空安全
来源：http://bpm.vqdsnc.cn

val n: String? = null;  n?.length
来源：http://eho.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://ret.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eaa.gaohongyu789.top

[T06] Kotlin：集合映射
来源：http://eyi.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ygr.guannengcc.top

[T07] Kotlin：集合过滤
来源：http://fkp.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iot.andypj.xyz

[T08] Kotlin：数据类
来源：http://pnk.ivvv.top

data class User(val name: String, val age: Int)
来源：http://avr.meibo888.top

[T09] Kotlin：扩展函数
来源：http://wmj.jinyuanbaomall.cn

fun String.exclaim() = this + "!"
来源：http://qvx.xuetiantiany.cn

[T10] Kotlin：默认参数
来源：http://ndo.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jwx.vehdjk.com

[T11] Kotlin：协程
来源：http://dej.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fco.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://tid.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://syd.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://uoj.ivvv.top

val m = mapOf("a" to 1)
来源：http://her.zdqjudy.top

[T14] Kotlin：循环
来源：http://rhx.xinyue.icu

for (i in 1..10) println(i)
来源：http://tyc.ehwqpu.com

[T15] Kotlin：接口
来源：http://lno.havefunace.top

interface Shape { fun area(): Double }
来源：http://lym.zdqjudy.top

[T16] Swift：Hello World
来源：http://phb.ydzc1.top

print("Hello")
来源：http://rpp.fehbvm.com

[T17] Swift：变量与常量
来源：http://wgn.fktsv.cn

var a = 1;  let b = 2
来源：http://bho.zhoulong.xyz

[T18] Swift：字符串插值
来源：http://dto.zhijiandao.cn

"值: \(b)"
来源：http://rfb.chenjidiqi.icu

[T19] Swift：可选绑定
来源：http://oxu.guannengcc.top

if let n = opt { print(n) }
来源：http://nap.jianghu66.top

[T20] Swift：数组操作
来源：http://bnz.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://umq.ctjpmb.com

[T21] Swift：遍历
来源：http://ofb.yvedp.cn

for x in a { print(x) }
来源：http://rcb.sufxvd.cn

[T22] Swift：字典
来源：http://omk.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://pwj.tianlin.xyz

[T23] Swift：函数
来源：http://yuq.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://olf.uphjek.com

[T24] Swift：闭包
来源：http://raw.xinyue.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://qah.zdbjq.cn

[T25] Swift：结构体
来源：http://bjo.hfpthk.cn

struct P { var x: Int }
来源：http://atx.hysaishi.cn

[T26] Swift：类与重写
来源：http://uah.ydjk.org.cn

class A: Base { override func f() {} }
来源：http://blh.gotoacloud.top

[T27] Swift：错误处理
来源：http://ogf.cashguo.top

do { try f() } catch { print(error) }
来源：http://cjv.sxryk.cn

[T28] Swift：枚举
来源：http://zpe.c1oappe.top

enum Color { case red, green }
来源：http://hby.zhijiandao.cn

[T29] Swift：guard 提前返回
来源：http://sds.sxryk.cn

guard let x = opt else { return }
来源：http://yfj.zycfv.cn

[T30] Swift：协议
来源：http://ksf.epnwcf.com

protocol Shape { func area() -> Double }
来源：http://clo.yonumen.top

[T31] Lua：Hello World
来源：http://gae.ivvv.top

print("Hello")
来源：http://jpf.yuxming.cn

[T32] Lua：局部变量
来源：http://ykq.redwolf501.top

local a = 1
来源：http://ycv.xuanzx.com

[T33] Lua：表（数组）
来源：http://zer.jyoumei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://quq.jqgufenzy.top

[T34] Lua：遍历表
来源：http://axx.andypj.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://qbw.aizwys.cn

[T35] Lua：字典表
来源：http://rga.hywenlv.cn

local d = { a = 1 };  d.b = 2
来源：http://wum.zhongyouzk.top

[T36] Lua：函数
来源：http://emk.yongpay.top

function add(a, b) return a + b end
来源：http://nrx.ydjk.org.cn

[T37] Lua：字符串拼接
来源：http://sft.yj20258888.top

"a" .. "b"
来源：http://ynf.zhoulong.xyz

[T38] Lua：条件
来源：http://pxu.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://bmu.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://lba.sjlbkw.cn

string.find(s, "%d+")
来源：http://fbd.nanxuanxn.top

[T40] Lua：元表
来源：http://fos.ydjk.org.cn

setmetatable({}, { __index = base })
来源：http://slf.xuanzx.com

[T41] Perl：Hello World
来源：http://dbt.nanxuanxn.top

print "Hello\n";
来源：http://qfr.cucudq.cn

[T42] Perl：变量类型
来源：http://wtl.jyoumei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://veg.shzxlz.cn


<!-- 参考信息 -->