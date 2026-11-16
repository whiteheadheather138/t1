代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://agk.jianghu66.top

[R50] awk 求和
来源：http://kth.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wgz.sysykeji.top

[R51] 排序去重取前几
来源：http://zra.tanke756.top

sort a.txt | uniq -c | sort -rn | head
来源：http://egp.jyoumei.cn

[R52] 统计行数
来源：http://ogz.xuetiantiany.cn

wc -l a.txt
来源：http://pav.yj202588.top

[R53] 查看文件头与实时尾
来源：http://jvf.xingfuxueyuan.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mcz.smart0.xyz

[R54] 比较两个文件
来源：http://awt.zhongyouzk.top

diff a.txt b.txt
来源：http://ilg.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://uve.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zas.gotoacloud.top

[R56] 远程拷贝
来源：http://lmj.shzxlz.cn

scp file user@host:/path/
来源：http://faq.xinyue.icu

[R57] 远程执行命令
来源：http://euj.jiagoushi.top

ssh user@host 'uptime'
来源：http://buz.cqqwz.cn

[R58] 下载文件
来源：http://fdv.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ins.birdmap.top

[R59] 发 POST JSON
来源：http://wya.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yaq.guowangkeji.top

[R60] 只看 HTTP 状态码
来源：http://pfr.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nxj.zycfv.cn

[R61] 磁盘占用
来源：http://wxf.ehwqpu.com

df -h;  du -sh *
来源：http://ddb.fengsongda.top

[R62] 找最占空间的文件
来源：http://yqi.xingfuxueyuan.xyz

du -ah . | sort -rh | head -10
来源：http://fmp.xinyue.icu

[R63] 内存与进程
来源：http://zfe.zhongyouzk.top

free -h;  ps aux | grep nginx
来源：http://npx.redwolf501.top

[R64] 结束进程
来源：http://nag.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://wno.316326.xyz

[R65] 查看端口占用
来源：http://oze.c1oappe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jrk.gaohongyu789.top

[R66] 定时任务
来源：http://gnj.yueranfly.top

crontab -e;  crontab -l
来源：http://ybz.ivvv.top

[R67] 生成随机十六进制串
来源：http://wqc.aizwys.cn

openssl rand -hex 16
来源：http://ojj.jinghuilouyu.cn

[R68] 计算文件校验值
来源：http://ffe.fzhhl.top

sha256sum a.txt;  md5sum a.txt
来源：http://mgs.xuetiantiany.cn

[R69] 生成随机密码
来源：http://vya.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://pwt.316326.xyz

[R70] 时间戳与互转
来源：http://cfo.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://omi.sweek.top

[R71] 日期格式化
来源：http://ehn.gzhubu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dlt.jianghu66.top

[R72] 等待端口就绪
来源：http://ljq.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ypf.fzhhl.top

[R73] 分割大日志
来源：http://cbf.gotoacloud.top

split -l 1000 big.log part_
来源：http://oiq.zhongyouzk.top

[R74] 批量重命名
来源：http://fvv.aibaodan.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qcu.yueranfly.top

[R75] 导出环境变量
来源：http://yhl.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://snr.pycfn.com

[R76] 使用临时文件
来源：http://lbm.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://trr.hnxiangtu.top

[R77] 读取用户输入
来源：http://cct.haohaochexian.top

read -rp "请输入: " ans
来源：http://wid.gogol.net.cn

[R78] 交互式菜单
来源：http://oam.pycfn.com

select opt in a b c; do echo "$opt"; break; done
来源：http://syp.shangyingyoupin.top

[R79] 解析命令行选项
来源：http://xcr.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vda.jyoumei.cn

[R80] 查看脚本执行耗时
来源：http://mvj.zdqjudy.top

time ./run.sh
来源：http://gvo.quarkkingdee.top

================================================================================
来源：http://yhp.sweek.top

S. C / C++ 专题
来源：http://zkv.yfazqb.com

================================================================================
来源：http://ztu.uphjek.com

[S01] C：Hello World
来源：http://uuy.svipenyu.cn

#include <stdio.h>
来源：http://sva.52xcode.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://twh.52xcode.cn

[S02] C：变量与格式化输出
来源：http://jaj.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://xtw.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://xvb.yj20258888.top

int x; scanf("%d", &x);
来源：http://arh.daxiang520.top

[S04] C：字符串复制
来源：http://shc.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jbd.jinqigfzy.top

[S05] C：字符串长度
来源：http://bce.dianchejie.cn

strlen(s)
来源：http://ami.fktsv.cn

[S06] C：字符串比较
来源：http://lcf.hywenlv.cn

strcmp(a, b) == 0
来源：http://pen.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://dnx.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lgf.xuanzx.com

[S08] C：动态内存分配与释放
来源：http://zja.pengpengdd.cyou

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hlw.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://gfm.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lqj.fehbvm.com

[S10] C：指针与解引用
来源：http://fci.sxryk.cn

int *p = &a;  *p = 5;
来源：http://xdn.jianghu66.top

[S11] C：逐行读文件
来源：http://ago.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://phc.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://lxk.chenlongwang.top

fclose(f);
来源：http://bhq.hongshengwenyu.top

[S12] C：写文件
来源：http://ybu.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://imr.zhiwuduotai.top

[S13] C：宏定义
来源：http://xjb.ywan-chungtsiang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mph.yonumen.top

[S14] C：枚举
来源：http://afs.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://hhw.hnxiangtu.top

[S15] C：类型转换
来源：http://wwo.jqgufenzy.top

(double) a / b
来源：http://ubb.zhaomingkeji.xyz

[S16] C：位操作置位
来源：http://iux.aizwys.cn

x |= (1 << 3);
来源：http://mdi.vehdjk.com

[S17] C：安全拼接字符串
来源：http://xwf.chenzaomai.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://abd.ppjwa.cn

[S18] C：命令行参数
来源：http://anf.jqgufenzy.top

int main(int argc, char **argv)
来源：http://vnp.gzhubu.top

[S19] C：快速排序
来源：http://reh.jinghuilouyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gna.chenlongwang.top

[S20] C：二分查找
来源：http://rwp.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ztl.tianlin.xyz

[S21] C：字符类别判断
来源：http://xdi.wangdashe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://efc.sjlbkw.cn

[S22] C：字符串转数字
来源：http://uno.ybcxt.top

atoi("42");  strtod("3.14", NULL);
来源：http://gnt.chenjidiqi.icu

[S23] C：随机数
来源：http://zpd.gzhubu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hfd.hnxiangtu.top

[S24] C：获取本地时间
来源：http://qhj.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://thc.fehbvm.com

[S25] C：内存拷贝
来源：http://bqj.cheryme.top

memcpy(dst, src, n);
来源：http://ecc.redwolf501.top

[S26] C：内存清零
来源：http://upz.shanyushiyangkeji.top

memset(a, 0, sizeof a);
来源：http://ozn.ehwqpu.com

[S27] C：定义常量
来源：http://iou.jinqigfzy.top

const double PI = 3.14159;
来源：http://dix.yj202588.top

[S28] C：静态变量
来源：http://fne.yuxming.cn

static int counter = 0;
来源：http://xlr.fengsongda.top

[S29] C：变参函数
来源：http://khi.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uec.zdbjq.cn

[S30] C：头文件保护
来源：http://mxa.jinghuilouyu.cn

#ifndef X_H
来源：http://ssv.mhx1999.top

#define X_H
来源：http://ntv.nanxuanxn.top

#endif
来源：http://apf.dianchejie.cn

[S31] C++：Hello World
来源：http://psh.mhx1999.top

#include <iostream>
来源：http://cio.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://nlf.fengsongda.top

[S32] C++：字符串
来源：http://waj.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://epf.fzhhl.top

[S33] C++：vector 增删
来源：http://rkt.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vjo.ctjpmb.com

[S34] C++：遍历 vector
来源：http://uqc.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://hzn.zhoulong.xyz

[S35] C++：map
来源：http://ylr.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wbd.zhengqikj.top

[S36] C++：unordered_map
来源：http://atb.shuidangran.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cca.yuxming.cn

[S37] C++：set
来源：http://gak.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://shm.haohaochexian.top

[S38] C++：排序
来源：http://whv.dianchejie.cn

std::sort(v.begin(), v.end());
来源：http://eay.ybcxt.top

[S39] C++：自定义比较器排序
来源：http://pjl.yueranfly.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oat.guannengcc.top

[S40] C++：查找元素
来源：http://xrz.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gyr.chenjidiqi.icu

[S41] C++：类与构造函数
来源：http://jfg.hcnkem.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wuz.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://pbq.snrcjt.cn

class B : public Base { public: void f() override {} };
来源：http://xhd.bjfxy.top

[S43] C++：智能指针
来源：http://hjk.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://sff.hywenlv.cn

[S44] C++：引用传参
来源：http://dxb.316326.xyz

void inc(int &x) { ++x; }
来源：http://alb.fengsongda.top

[S45] C++：lambda
来源：http://zri.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://glt.yongpay.top

[S46] C++：函数模板
来源：http://dbn.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hhk.yuanzhike.top

[S47] C++：结构化绑定遍历
来源：http://tve.chenlongwang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lfy.zhongyouzk.top

[S48] C++：逐行读文件
来源：http://erk.quarkkingdee.top

std::ifstream in("a.txt");  std::string line;
来源：http://uqf.zhengqikj.top

while (std::getline(in, line)) { }
来源：http://uso.redwolf501.top

[S49] C++：写文件
来源：http://csl.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aif.xingfuxueyuan.xyz

[S50] C++：格式化数字
来源：http://dov.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pxk.tianlin.xyz

[S51] C++：显式类型转换
来源：http://whd.yfazqb.com

static_cast<double>(a) / b
来源：http://xge.yj202588.top

[S52] C++：const 与 noexcept
来源：http://tto.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://bzg.9152youxi.cn

[S53] C++：移动语义
来源：http://rrn.quarkkingdee.top

std::vector<int> w = std::move(v);
来源：http://rgx.hongshengwenyu.top

[S54] C++：异常处理
来源：http://tlg.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dgh.mhx1999.top

[S55] C++：结构化绑定
来源：http://miu.gotoacloud.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ahy.chenzaomai.com

[S56] C++：optional
来源：http://otn.sweek.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xyv.sjlbkw.cn

[S57] C++：编译期常量
来源：http://yzr.gaohongyu789.top

constexpr int N = 10;
来源：http://mmv.epnwcf.com

[S58] C++：命名空间
来源：http://lun.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://jbi.dianchejie.cn

[S59] C++：静态断言
来源：http://yzb.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tsf.yuxming.cn

[S60] C++：遍历并删除元素
来源：http://mum.gaohongyu789.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yzl.jqgufenzy.top

================================================================================
来源：http://mlh.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://riu.gzhubu.top

================================================================================
来源：http://puq.tanke756.top

[T01] Kotlin：Hello World
来源：http://pij.vqdsnc.cn

println("Hello")
来源：http://gfe.52xcode.cn

[T02] Kotlin：变量
来源：http://ljq.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fww.fzhhl.top

[T03] Kotlin：字符串模板
来源：http://kuo.hnxiangtu.top

"值: $b"
来源：http://veo.tian-w.cn

[T04] Kotlin：空安全
来源：http://byf.ivvv.top

val n: String? = null;  n?.length
来源：http://myy.mhx1999.top

[T05] Kotlin：when 表达式
来源：http://lqa.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://byp.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://xwm.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://uto.316326.xyz

[T07] Kotlin：集合过滤
来源：http://buz.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qjh.aizwys.cn

[T08] Kotlin：数据类
来源：http://xma.havefunace.top

data class User(val name: String, val age: Int)
来源：http://erx.andypj.xyz

[T09] Kotlin：扩展函数
来源：http://jwv.fehbvm.com

fun String.exclaim() = this + "!"
来源：http://dju.shanyushiyangkeji.top

[T10] Kotlin：默认参数
来源：http://lut.smart0.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://lyw.cdnleiting.top

[T11] Kotlin：协程
来源：http://avl.yfazqb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://him.bjfxy.top

[T12] Kotlin：解构声明
来源：http://ubq.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://oln.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://tik.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://nzx.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://zfl.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://nmd.yj20258888.top

[T15] Kotlin：接口
来源：http://oca.hnqzz.top

interface Shape { fun area(): Double }
来源：http://hjc.daria6918.cn

[T16] Swift：Hello World
来源：http://imp.cheryme.top

print("Hello")
来源：http://xsc.xingfuxueyuan.xyz

[T17] Swift：变量与常量
来源：http://jbd.snrcjt.cn

var a = 1;  let b = 2
来源：http://ldr.yj20258.top

[T18] Swift：字符串插值
来源：http://phe.hysaishi.cn

"值: \(b)"
来源：http://xiq.guannengcc.top

[T19] Swift：可选绑定
来源：http://ssk.hywenlv.cn

if let n = opt { print(n) }
来源：http://ukp.hfpthk.cn

[T20] Swift：数组操作
来源：http://hmr.hywenlv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ofa.quarkkingdee.top

[T21] Swift：遍历
来源：http://qyl.cdnleiting.top

for x in a { print(x) }
来源：http://wrk.zhixingplan.top

[T22] Swift：字典
来源：http://trt.xuanzx.com

var d = ["a": 1];  d["b"] = 2
来源：http://urz.cucudq.cn

[T23] Swift：函数
来源：http://bau.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xwn.hcnkem.com

[T24] Swift：闭包
来源：http://zby.gotoacloud.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hix.aibaodan.cn

[T25] Swift：结构体
来源：http://rpa.daxiang520.top

struct P { var x: Int }
来源：http://fak.0kj1m.cn

[T26] Swift：类与重写
来源：http://yfa.xinyue.icu

class A: Base { override func f() {} }
来源：http://myx.pengpengdd.cyou

[T27] Swift：错误处理
来源：http://wzc.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://vyh.daxiang520.top

[T28] Swift：枚举
来源：http://ruy.c1oappe.top

enum Color { case red, green }
来源：http://hwr.yueranfly.top

[T29] Swift：guard 提前返回
来源：http://hbd.smart0.xyz

guard let x = opt else { return }
来源：http://enp.vqdsnc.cn

[T30] Swift：协议
来源：http://idd.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://zlj.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://jut.sufxvd.cn

print("Hello")
来源：http://nrg.bjfxy.top

[T32] Lua：局部变量
来源：http://utm.jinqigufen.top

local a = 1
来源：http://xvc.cqqwz.cn

[T33] Lua：表（数组）
来源：http://joq.shanyushiyangtech.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dri.jianghu66.top

[T34] Lua：遍历表
来源：http://dhe.shanyushiyangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ghm.guannengcc.top

[T35] Lua：字典表
来源：http://mry.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://hhx.guannengcc.top

[T36] Lua：函数
来源：http://ldx.zhongyouzk.top

function add(a, b) return a + b end
来源：http://znr.yangfankeji.com

[T37] Lua：字符串拼接
来源：http://jzz.shangyingyoupin.top

"a" .. "b"
来源：http://xqo.zhixingplan.top

[T38] Lua：条件
来源：http://vea.sweek.top

if x > 0 then print("正") end
来源：http://bhv.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://qek.xziqi.cn

string.find(s, "%d+")
来源：http://dmk.zhixingplan.top

[T40] Lua：元表
来源：http://kng.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://vjo.wangshuangyany.cn

[T41] Perl：Hello World
来源：http://nvg.zycfv.cn

print "Hello\n";
来源：http://wgl.zhixingplan.top

[T42] Perl：变量类型
来源：http://jrm.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ccb.dashuyun.cn

[T43] Perl：字符串插值
来源：http://vha.c1oappe.top

"值: $a"
来源：http://knl.birdmap.top

[T44] Perl：条件
来源：http://kah.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://olx.gotoacloud.top

[T45] Perl：数组遍历
来源：http://ktt.zdbjq.cn

for my $x (@arr) { print $x; }
来源：http://fbw.yonumen.top

[T46] Perl：哈希操作
来源：http://fxz.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hrl.zhengqikj.top

[T47] Perl：正则捕获
来源：http://icn.haohaochexian.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rum.ctjpmb.com

[T48] Perl：正则替换
来源：http://dmc.daria6918.cn

$s =~ s/old/new/g;
来源：http://wwk.yvedp.cn

[T49] Perl：函数
来源：http://aep.dashuyun.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uql.zhiwuduotai.top

[T50] Perl：逐行读文件
来源：http://gys.gzhubu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hxq.dashuyun.cn

while (my $line = <$fh>) { print $line; }
来源：http://kxe.gzhubu.top

[T51] Scala：Hello World
来源：http://sfw.jqgfzy.top

println("Hello")
来源：http://blw.xingfuxueyuan.xyz

[T52] Scala：变量
来源：http://yfc.zhijiandao.cn


<!-- 参考信息 -->