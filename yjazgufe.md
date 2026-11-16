代发 wailian999

cmd >/dev/null 2>&1
来源：http://jdk.aizwys.cn

[R42] 输入重定向
来源：http://rrx.zhongyouzk.top

wc -l < a.txt
来源：http://uyc.0kj1m.cn

[R43] 按名字查找文件
来源：http://ijl.sysykeji.top

find . -name "*.log" -type f
来源：http://wvz.cucudq.cn

[R44] 按修改时间查找
来源：http://eop.snrcjt.cn

find . -mtime -7 -type f
来源：http://yih.chenzaomai.com

[R45] 批量删除
来源：http://nfv.sysykeji.top

find . -name "*.tmp" -delete
来源：http://ebs.meibo888.top

[R46] 递归替换文件内容
来源：http://enk.tianlin.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://atp.vehdjk.com

[R47] sed 单行替换
来源：http://vlr.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://djx.jinqigufen.top

[R48] awk 取指定列
来源：http://dqh.meibo888.top

awk '{print $1, $3}' a.txt
来源：http://myt.hcnkem.com

[R49] awk 带条件
来源：http://jxm.jianghu66.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://njq.hfpthk.cn

[R50] awk 求和
来源：http://dyt.hnqzz.top

awk '{s += $2} END {print s}' a.txt
来源：http://lky.chenlongwang.top

[R51] 排序去重取前几
来源：http://qur.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zjf.ybcxt.top

[R52] 统计行数
来源：http://rfk.daria6918.cn

wc -l a.txt
来源：http://mil.xziqi.cn

[R53] 查看文件头与实时尾
来源：http://vvb.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://urx.shzxlz.cn

[R54] 比较两个文件
来源：http://gkh.ydzc1.top

diff a.txt b.txt
来源：http://qea.ydjk.org.cn

[R55] 压缩与解压
来源：http://uyb.yuanzhike.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://evh.hammf.cn

[R56] 远程拷贝
来源：http://gid.snrcjt.cn

scp file user@host:/path/
来源：http://zcr.hnqzz.top

[R57] 远程执行命令
来源：http://fes.52xcode.cn

ssh user@host 'uptime'
来源：http://afy.gaohongyu789.top

[R58] 下载文件
来源：http://dpf.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://syz.yj202588.top

[R59] 发 POST JSON
来源：http://fuj.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://spa.gaohongyu789.top

[R60] 只看 HTTP 状态码
来源：http://kvg.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pew.ctjpmb.com

[R61] 磁盘占用
来源：http://aqt.yuanzhike.top

df -h;  du -sh *
来源：http://vbj.aibaodan.cn

[R62] 找最占空间的文件
来源：http://huo.zdqjudy.top

du -ah . | sort -rh | head -10
来源：http://wsn.gogol.net.cn

[R63] 内存与进程
来源：http://pqc.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://vgz.fehbvm.com

[R64] 结束进程
来源：http://gdc.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://tzh.9152youxi.cn

[R65] 查看端口占用
来源：http://meb.xziqi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wgc.xuanzx.com

[R66] 定时任务
来源：http://gje.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://nfm.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://ams.ybcxt.top

openssl rand -hex 16
来源：http://vyj.nanxuanxn.top

[R68] 计算文件校验值
来源：http://dxt.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nxg.zhengqikj.top

[R69] 生成随机密码
来源：http://jpb.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://vwo.bjfxy.top

[R70] 时间戳与互转
来源：http://otr.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://fyh.jinqigfzy.top

[R71] 日期格式化
来源：http://ljr.pengpengdd.cyou

date +"%Y-%m-%d %H:%M:%S"
来源：http://job.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://fjm.cheryme.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dtb.ivvv.top

[R73] 分割大日志
来源：http://byy.bjfxy.top

split -l 1000 big.log part_
来源：http://cgi.tanke756.top

[R74] 批量重命名
来源：http://rez.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://osj.iojbl.cn

[R75] 导出环境变量
来源：http://dil.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://vrb.yangfankeji.com

[R76] 使用临时文件
来源：http://nav.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xvz.jyoumei.cn

[R77] 读取用户输入
来源：http://srv.sweek.top

read -rp "请输入: " ans
来源：http://nyn.9152youxi.cn

[R78] 交互式菜单
来源：http://sbo.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://evu.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://jyk.snrcjt.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rwy.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://glz.shanyushiyangkeji.top

time ./run.sh
来源：http://gry.yuxming.cn

================================================================================
来源：http://csi.ehwqpu.com

S. C / C++ 专题
来源：http://mtz.kuanghao11.cn

================================================================================
来源：http://yqa.yj20258888.top

[S01] C：Hello World
来源：http://xoy.epnwcf.com

#include <stdio.h>
来源：http://nbd.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zrx.bjfxy.top

[S02] C：变量与格式化输出
来源：http://pxs.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://mgd.cheryme.top

[S03] C：读入整数
来源：http://kbe.cucudq.cn

int x; scanf("%d", &x);
来源：http://yts.xuanzx.com

[S04] C：字符串复制
来源：http://uje.zdbjq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fme.redwolf501.top

[S05] C：字符串长度
来源：http://wlo.zhijiandao.cn

strlen(s)
来源：http://fjj.tanke756.top

[S06] C：字符串比较
来源：http://khj.c1oappe.top

strcmp(a, b) == 0
来源：http://ryl.jinqigfzy.top

[S07] C：数组遍历求和
来源：http://cgi.xziqi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ssx.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://rud.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ptb.hesvh.cn

[S09] C：结构体定义与初始化
来源：http://yax.hnxiangtu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://coo.guannengcc.top

[S10] C：指针与解引用
来源：http://ulv.havefunace.top

int *p = &a;  *p = 5;
来源：http://vqp.xinyue.icu

[S11] C：逐行读文件
来源：http://pzu.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://exv.zhaomingkeji.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://zvh.jinghuilouyu.cn

fclose(f);
来源：http://jrz.feifeiyinyue.top

[S12] C：写文件
来源：http://ksk.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ldj.yj20258.top

[S13] C：宏定义
来源：http://heh.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hmc.cdnleiting.top

[S14] C：枚举
来源：http://vjv.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://qyc.hcnkem.com

[S15] C：类型转换
来源：http://laq.chenzaomai.com

(double) a / b
来源：http://bjl.feifeiyinyue.top

[S16] C：位操作置位
来源：http://blv.iojbl.cn

x |= (1 << 3);
来源：http://vlh.ctjpmb.com

[S17] C：安全拼接字符串
来源：http://kbq.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wfv.shangyingyoupin.top

[S18] C：命令行参数
来源：http://lhp.ydjk.org.cn

int main(int argc, char **argv)
来源：http://ukq.ydjk.org.cn

[S19] C：快速排序
来源：http://sdy.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://upq.tanke756.top

[S20] C：二分查找
来源：http://hpz.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dor.jqgfzy.top

[S21] C：字符类别判断
来源：http://fmh.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nbh.pycfn.com

[S22] C：字符串转数字
来源：http://lxf.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://nmm.gaohongyu789.top

[S23] C：随机数
来源：http://bdr.zhengqikj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jyh.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://mza.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pjb.aizwys.cn

[S25] C：内存拷贝
来源：http://yqw.hfpthk.cn

memcpy(dst, src, n);
来源：http://syw.dashuyun.cn

[S26] C：内存清零
来源：http://lyv.fengsongda.top

memset(a, 0, sizeof a);
来源：http://lbg.shangyingyoupin.top

[S27] C：定义常量
来源：http://uqs.nwbrower.top

const double PI = 3.14159;
来源：http://zbc.guannengcc.top

[S28] C：静态变量
来源：http://gvh.jyoumei.cn

static int counter = 0;
来源：http://xcd.yuanzhike.top

[S29] C：变参函数
来源：http://qef.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fnl.hesvh.cn

[S30] C：头文件保护
来源：http://nuv.hcnkem.com

#ifndef X_H
来源：http://utn.hesvh.cn

#define X_H
来源：http://ytn.yvedp.cn

#endif
来源：http://cjv.epnwcf.com

[S31] C++：Hello World
来源：http://fku.wangshuangyany.cn

#include <iostream>
来源：http://qpz.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://sdw.fktsv.cn

[S32] C++：字符串
来源：http://kob.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://wqs.cqqwz.cn

[S33] C++：vector 增删
来源：http://phg.tianlin.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qyt.redwolf501.top

[S34] C++：遍历 vector
来源：http://ima.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://htv.havefunace.top

[S35] C++：map
来源：http://nqq.yuxming.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sqm.cashguo.top

[S36] C++：unordered_map
来源：http://tyd.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hyo.yanxiufei.cn

[S37] C++：set
来源：http://cxb.yuxming.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qgz.hongshengwenyu.top

[S38] C++：排序
来源：http://yci.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://icg.wangshuangyany.cn

[S39] C++：自定义比较器排序
来源：http://kat.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hkw.bjfxy.top

[S40] C++：查找元素
来源：http://ulr.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sth.jianghu66.top

[S41] C++：类与构造函数
来源：http://wzr.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://axm.xuanzx.com

[S42] C++：继承与虚函数
来源：http://bay.fanxiaobao.xyz

class B : public Base { public: void f() override {} };
来源：http://avg.chenlongwang.top

[S43] C++：智能指针
来源：http://apk.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://bsc.daria6918.cn

[S44] C++：引用传参
来源：http://sgv.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://ylx.zhaomingkeji.xyz

[S45] C++：lambda
来源：http://qnx.tanke756.top

auto add = [](int a, int b) { return a + b; };
来源：http://lti.jiagoushi.top

[S46] C++：函数模板
来源：http://tqi.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hhe.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://nut.vehdjk.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wpp.cdnleiting.top

[S48] C++：逐行读文件
来源：http://tja.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lig.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://vqq.yueranfly.top

[S49] C++：写文件
来源：http://zts.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://woz.ppjwa.cn

[S50] C++：格式化数字
来源：http://sqc.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blb.epnwcf.com

[S51] C++：显式类型转换
来源：http://eug.cucudq.cn

static_cast<double>(a) / b
来源：http://frl.yj20258.top

[S52] C++：const 与 noexcept
来源：http://oix.52xcode.cn

int size() const noexcept { return n_; }
来源：http://yyd.aizwys.cn

[S53] C++：移动语义
来源：http://smq.tanke756.top

std::vector<int> w = std::move(v);
来源：http://mex.yj20258888.top

[S54] C++：异常处理
来源：http://grj.c1oappe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yff.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://pwf.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tvc.ehwqpu.com

[S56] C++：optional
来源：http://gff.fehbvm.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rhd.fengsongda.top

[S57] C++：编译期常量
来源：http://fbo.jinyuanbaomall.cn

constexpr int N = 10;
来源：http://dvn.kuanghao11.cn

[S58] C++：命名空间
来源：http://gor.xinyue.icu

namespace ns { int f() { return 1; } }
来源：http://exw.zhiwuduotai.top

[S59] C++：静态断言
来源：http://hpz.meibo888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vud.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://fqi.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yko.jinyuanbaomall.cn

================================================================================
来源：http://psz.zhaomingkeji.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tzl.zhoulong.xyz

================================================================================
来源：http://phn.daria6918.cn

[T01] Kotlin：Hello World
来源：http://xqf.ppjwa.cn

println("Hello")
来源：http://btc.vehdjk.com

[T02] Kotlin：变量
来源：http://lfp.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hzd.yj202588.top

[T03] Kotlin：字符串模板
来源：http://obl.316326.xyz

"值: $b"
来源：http://hem.hcnkem.com

[T04] Kotlin：空安全
来源：http://lbw.shangyingyoupin.top

val n: String? = null;  n?.length
来源：http://sxi.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://nqk.tarul.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xgd.daria6918.cn

[T06] Kotlin：集合映射
来源：http://ftg.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fse.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://zbd.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mng.aizwys.cn

[T08] Kotlin：数据类
来源：http://ymm.cashguo.top

data class User(val name: String, val age: Int)
来源：http://anf.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://trj.snrcjt.cn

fun String.exclaim() = this + "!"
来源：http://ren.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://baf.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://woy.pycfn.com

[T11] Kotlin：协程
来源：http://sfi.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cit.jlsjyb.cn

[T12] Kotlin：解构声明
来源：http://shl.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://hvr.shanyushiyangkeji.top

[T13] Kotlin：只读 Map
来源：http://xbf.hnxiangtu.top

val m = mapOf("a" to 1)
来源：http://ddv.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://hnb.wangshuangyany.cn

for (i in 1..10) println(i)
来源：http://fvr.nanxuanxn.top

[T15] Kotlin：接口
来源：http://gba.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://rrl.yanxiufei.cn

[T16] Swift：Hello World
来源：http://emh.nanxuanxn.top

print("Hello")
来源：http://vwc.chenzaomai.com

[T17] Swift：变量与常量
来源：http://gbj.aizwys.cn

var a = 1;  let b = 2
来源：http://bvc.jqgufenzy.top

[T18] Swift：字符串插值
来源：http://csg.jlsjyb.cn

"值: \(b)"
来源：http://vze.xuanzx.com

[T19] Swift：可选绑定
来源：http://aut.yueranfly.top

if let n = opt { print(n) }
来源：http://wii.nanxinkj.top

[T20] Swift：数组操作
来源：http://udc.zhijiandao.cn

var a = [1, 2, 3];  a.append(4)
来源：http://adm.yanxiufei.cn

[T21] Swift：遍历
来源：http://nul.zdbjq.cn

for x in a { print(x) }
来源：http://djd.guowangkeji.top

[T22] Swift：字典
来源：http://ydp.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://kvl.haohaochexian.top

[T23] Swift：函数
来源：http://hyq.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://unp.hcnkem.com

[T24] Swift：闭包
来源：http://czn.zhongyouzk.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wip.yongpay.top

[T25] Swift：结构体
来源：http://hoq.sweek.top

struct P { var x: Int }
来源：http://hiy.cqqwz.cn

[T26] Swift：类与重写
来源：http://hfw.pycfn.com

class A: Base { override func f() {} }
来源：http://gqp.sysykeji.top

[T27] Swift：错误处理
来源：http://zil.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://rla.zycfv.cn

[T28] Swift：枚举
来源：http://uyw.zhixingplan.top

enum Color { case red, green }
来源：http://ywm.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://lmf.cucudq.cn

guard let x = opt else { return }
来源：http://neh.meibo888.top

[T30] Swift：协议
来源：http://xmg.pengpengdd.cyou

protocol Shape { func area() -> Double }
来源：http://gyf.bbcook.cn

[T31] Lua：Hello World
来源：http://ivh.hnxiangtu.top

print("Hello")
来源：http://hys.sweek.top

[T32] Lua：局部变量
来源：http://pxn.vehdjk.com

local a = 1
来源：http://qcn.c1oappe.top

[T33] Lua：表（数组）
来源：http://cxy.wangdashe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://swk.fktsv.cn

[T34] Lua：遍历表
来源：http://qcu.jinqigufen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fzf.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://ltq.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://ibt.nanxuanxn.top

[T36] Lua：函数
来源：http://dek.gzhubu.top

function add(a, b) return a + b end
来源：http://kis.52xcode.cn

[T37] Lua：字符串拼接
来源：http://owy.jyoumei.cn

"a" .. "b"
来源：http://ymp.hnxiangtu.top

[T38] Lua：条件
来源：http://urc.xziqi.cn

if x > 0 then print("正") end
来源：http://nzb.zdbjq.cn

[T39] Lua：模式匹配
来源：http://mjw.dashuyun.cn

string.find(s, "%d+")
来源：http://ibd.cucudq.cn

[T40] Lua：元表
来源：http://ejh.yuxming.cn

setmetatable({}, { __index = base })
来源：http://avt.yj20258888.top

[T41] Perl：Hello World
来源：http://ytb.hnqzz.top

print "Hello\n";
来源：http://phj.xinyue.icu

[T42] Perl：变量类型
来源：http://hdw.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fqk.yvedp.cn

[T43] Perl：字符串插值
来源：http://jkh.jlsjyb.cn

"值: $a"
来源：http://hgz.sweek.top

[T44] Perl：条件
来源：http://gdc.hongshengwenyu.top

if ($a > 0) { print "正"; }
来源：http://nqy.zhiwuduotai.top


<!-- 参考信息 -->