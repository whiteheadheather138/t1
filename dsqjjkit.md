代发 wailian999

cmd >/dev/null 2>&1
来源：http://dmy.hysaishi.cn

[R42] 输入重定向
来源：http://gou.smart0.xyz

wc -l < a.txt
来源：http://kkp.yuanzhike.top

[R43] 按名字查找文件
来源：http://woe.yongpay.top

find . -name "*.log" -type f
来源：http://syw.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://eqk.mhx1999.top

find . -mtime -7 -type f
来源：http://scp.birdmap.top

[R45] 批量删除
来源：http://isg.ybcxt.top

find . -name "*.tmp" -delete
来源：http://kib.yuxming.cn

[R46] 递归替换文件内容
来源：http://kpp.ehwqpu.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aau.shangyingyoupin.top

[R47] sed 单行替换
来源：http://ueg.wangshuangyany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://iej.epnwcf.com

[R48] awk 取指定列
来源：http://gdz.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://idd.jinqigfzy.top

[R49] awk 带条件
来源：http://ayu.chenjidiqi.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://okj.wangshuangyany.cn

[R50] awk 求和
来源：http://ric.nwbrower.top

awk '{s += $2} END {print s}' a.txt
来源：http://lbf.dashuyun.cn

[R51] 排序去重取前几
来源：http://otv.52xcode.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nyt.chenlongwang.top

[R52] 统计行数
来源：http://dta.9152youxi.cn

wc -l a.txt
来源：http://fon.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://use.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://klp.nanxinkj.top

[R54] 比较两个文件
来源：http://ach.xziqi.cn

diff a.txt b.txt
来源：http://opu.hammf.cn

[R55] 压缩与解压
来源：http://uzu.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pai.hnqzz.top

[R56] 远程拷贝
来源：http://ggi.cheryme.top

scp file user@host:/path/
来源：http://fzz.jiagoushi.top

[R57] 远程执行命令
来源：http://szz.guowangkeji.top

ssh user@host 'uptime'
来源：http://yqn.dianchejie.cn

[R58] 下载文件
来源：http://xip.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rnr.cheryme.top

[R59] 发 POST JSON
来源：http://tzp.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tob.ivvv.top

[R60] 只看 HTTP 状态码
来源：http://hbw.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://odw.shzxlz.cn

[R61] 磁盘占用
来源：http://cuz.ydjk.org.cn

df -h;  du -sh *
来源：http://eie.cashguo.top

[R62] 找最占空间的文件
来源：http://nzr.yongpay.top

du -ah . | sort -rh | head -10
来源：http://pgg.yj20258888.top

[R63] 内存与进程
来源：http://rii.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://rjl.andypj.xyz

[R64] 结束进程
来源：http://glq.fehbvm.com

kill -9 $(pgrep -f app.py)
来源：http://wpw.jiagoushi.top

[R65] 查看端口占用
来源：http://jwu.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zdp.zhoulong.xyz

[R66] 定时任务
来源：http://ggk.xuanzx.com

crontab -e;  crontab -l
来源：http://jjp.epnwcf.com

[R67] 生成随机十六进制串
来源：http://wzn.jyoumei.cn

openssl rand -hex 16
来源：http://wmj.sxryk.cn

[R68] 计算文件校验值
来源：http://ziv.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://wub.yuanzhike.top

[R69] 生成随机密码
来源：http://jkb.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://yze.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://ujw.hcnkem.com

date +%s;  date -d @1700000000
来源：http://gvf.fzhhl.top

[R71] 日期格式化
来源：http://laj.yangfankeji.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://qhm.cucudq.cn

[R72] 等待端口就绪
来源：http://kjp.zhongyouzk.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hwc.iojbl.cn

[R73] 分割大日志
来源：http://eeo.andypj.xyz

split -l 1000 big.log part_
来源：http://ple.zhijiandao.cn

[R74] 批量重命名
来源：http://awr.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fyb.tanke756.top

[R75] 导出环境变量
来源：http://ubb.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://xev.dianchejie.cn

[R76] 使用临时文件
来源：http://gcv.tian-w.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jhd.zhixingplan.top

[R77] 读取用户输入
来源：http://bjk.ivvv.top

read -rp "请输入: " ans
来源：http://evl.gaohongyu789.top

[R78] 交互式菜单
来源：http://ymv.shanyushiyangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fcx.jqgfzy.top

[R79] 解析命令行选项
来源：http://pwh.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ult.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://uwe.quarkkingdee.top

time ./run.sh
来源：http://nrg.chenzaomai.com

================================================================================
来源：http://wth.bbcook.cn

S. C / C++ 专题
来源：http://ymz.tanke756.top

================================================================================
来源：http://jaj.zhengqikj.top

[S01] C：Hello World
来源：http://gyg.pycfn.com

#include <stdio.h>
来源：http://ais.aizwys.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xuj.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://rmz.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://xzt.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://kmx.yfazqb.com

int x; scanf("%d", &x);
来源：http://wrx.fengsongda.top

[S04] C：字符串复制
来源：http://wky.hcnkem.com

char dst[32]; strcpy(dst, "hi");
来源：http://rnq.pengpengdd.cyou

[S05] C：字符串长度
来源：http://xbf.smart0.xyz

strlen(s)
来源：http://ptj.ydjk.org.cn

[S06] C：字符串比较
来源：http://hyq.daria6918.cn

strcmp(a, b) == 0
来源：http://pcm.tanke756.top

[S07] C：数组遍历求和
来源：http://efn.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sga.shuidangran.top

[S08] C：动态内存分配与释放
来源：http://wvw.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mpl.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://zkd.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tls.tarul.cn

[S10] C：指针与解引用
来源：http://nbd.epnwcf.com

int *p = &a;  *p = 5;
来源：http://wdj.c1oappe.top

[S11] C：逐行读文件
来源：http://llc.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://olr.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://byr.hysaishi.cn

fclose(f);
来源：http://kkj.nanxinkj.top

[S12] C：写文件
来源：http://yti.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ttg.bjfxy.top

[S13] C：宏定义
来源：http://sdx.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://njw.fanxiaobao.xyz

[S14] C：枚举
来源：http://ktz.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://qfe.hcnkem.com

[S15] C：类型转换
来源：http://lru.yueranfly.top

(double) a / b
来源：http://blj.daxiang520.top

[S16] C：位操作置位
来源：http://ifg.wangshuangyany.cn

x |= (1 << 3);
来源：http://tnu.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://txp.fzhhl.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://avt.fehbvm.com

[S18] C：命令行参数
来源：http://nlq.kuanghao11.cn

int main(int argc, char **argv)
来源：http://olw.daria6918.cn

[S19] C：快速排序
来源：http://stk.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://seh.jiagoushi.top

[S20] C：二分查找
来源：http://hid.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://olr.316326.xyz

[S21] C：字符类别判断
来源：http://qxj.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://efx.shuidangran.top

[S22] C：字符串转数字
来源：http://gnk.guowangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://uzy.cashguo.top

[S23] C：随机数
来源：http://yph.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kfg.ivvv.top

[S24] C：获取本地时间
来源：http://cop.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yrg.dashuyun.cn

[S25] C：内存拷贝
来源：http://fdt.cashguo.top

memcpy(dst, src, n);
来源：http://bzn.xziqi.cn

[S26] C：内存清零
来源：http://rdr.haohaochexian.top

memset(a, 0, sizeof a);
来源：http://rim.vehdjk.com

[S27] C：定义常量
来源：http://ibt.jianghu66.top

const double PI = 3.14159;
来源：http://fvu.sjlbkw.cn

[S28] C：静态变量
来源：http://xyz.yvedp.cn

static int counter = 0;
来源：http://nkx.jiagoushi.top

[S29] C：变参函数
来源：http://dth.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xxl.cheryme.top

[S30] C：头文件保护
来源：http://lir.yongpay.top

#ifndef X_H
来源：http://agd.yfazqb.com

#define X_H
来源：http://ppi.gzhubu.top

#endif
来源：http://hdr.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://cak.wangshuangyany.cn

#include <iostream>
来源：http://yss.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://tvw.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://znp.dashuyun.cn

std::string s = "hi";  s += "!";
来源：http://eor.sufxvd.cn

[S33] C++：vector 增删
来源：http://pha.bjfxy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://juh.guannengcc.top

[S34] C++：遍历 vector
来源：http://jxu.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://odn.sweek.top

[S35] C++：map
来源：http://gjm.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fzb.aibaodan.cn

[S36] C++：unordered_map
来源：http://bwz.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wqe.shanyushiyangtech.top

[S37] C++：set
来源：http://vvn.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mht.zhongyouzk.top

[S38] C++：排序
来源：http://bkm.cashguo.top

std::sort(v.begin(), v.end());
来源：http://yee.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://hqc.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://shh.tanke756.top

[S40] C++：查找元素
来源：http://sqo.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lnh.daria6918.cn

[S41] C++：类与构造函数
来源：http://ykw.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gpe.aizwys.cn

[S42] C++：继承与虚函数
来源：http://icv.yvedp.cn

class B : public Base { public: void f() override {} };
来源：http://gan.0kj1m.cn

[S43] C++：智能指针
来源：http://ocz.ydjk.org.cn

auto p = std::make_unique<int>(5);
来源：http://rsp.vehdjk.com

[S44] C++：引用传参
来源：http://faz.zhoulong.xyz

void inc(int &x) { ++x; }
来源：http://uxe.vqdsnc.cn

[S45] C++：lambda
来源：http://slk.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://uao.ybcxt.top

[S46] C++：函数模板
来源：http://xee.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vvp.gotoacloud.top

[S47] C++：结构化绑定遍历
来源：http://tic.xinyue.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hxo.9152youxi.cn

[S48] C++：逐行读文件
来源：http://hth.tarul.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ljh.daxiang520.top

while (std::getline(in, line)) { }
来源：http://esn.svipenyu.cn

[S49] C++：写文件
来源：http://mgm.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lzh.sysykeji.top

[S50] C++：格式化数字
来源：http://bjy.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blp.ydzc1.top

[S51] C++：显式类型转换
来源：http://zdl.zdqjudy.top

static_cast<double>(a) / b
来源：http://wvl.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://ugr.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://ben.zhongyouzk.top

[S53] C++：移动语义
来源：http://nrz.hesvh.cn

std::vector<int> w = std::move(v);
来源：http://zuf.jlsjyb.cn

[S54] C++：异常处理
来源：http://wlz.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cie.c1oappe.top

[S55] C++：结构化绑定
来源：http://qgz.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://myj.chenjidiqi.icu

[S56] C++：optional
来源：http://uns.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rop.sysykeji.top

[S57] C++：编译期常量
来源：http://umx.hysaishi.cn

constexpr int N = 10;
来源：http://bzj.tanke756.top

[S58] C++：命名空间
来源：http://xeb.snrcjt.cn

namespace ns { int f() { return 1; } }
来源：http://kzr.sxryk.cn

[S59] C++：静态断言
来源：http://bil.guannengcc.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bar.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://gky.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://idd.wangshuangyany.cn

================================================================================
来源：http://ctk.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://weu.sjlbkw.cn

================================================================================
来源：http://dck.jinyuanbaomall.cn

[T01] Kotlin：Hello World
来源：http://add.xuetiantiany.cn

println("Hello")
来源：http://mbs.dianchejie.cn

[T02] Kotlin：变量
来源：http://ftd.redwolf501.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wlo.hywenlv.cn

[T03] Kotlin：字符串模板
来源：http://ppz.chenzaomai.com

"值: $b"
来源：http://uho.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://hnt.cheryme.top

val n: String? = null;  n?.length
来源：http://rmz.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://owz.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wyc.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://vff.52xcode.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vkx.shanyushiyangtech.top

[T07] Kotlin：集合过滤
来源：http://rsd.zdbjq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xrw.guowangkeji.top

[T08] Kotlin：数据类
来源：http://kww.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://mrk.yongpay.top

[T09] Kotlin：扩展函数
来源：http://oaj.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://ocw.c1oappe.top

[T10] Kotlin：默认参数
来源：http://pbz.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://euv.guannengcc.top

[T11] Kotlin：协程
来源：http://vwy.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://oxz.cheryme.top

[T12] Kotlin：解构声明
来源：http://ocy.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://ozg.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://tfa.cucudq.cn

val m = mapOf("a" to 1)
来源：http://cok.yonumen.top

[T14] Kotlin：循环
来源：http://rsv.cdnleiting.top

for (i in 1..10) println(i)
来源：http://yzy.hnxiangtu.top

[T15] Kotlin：接口
来源：http://dtj.fzhhl.top

interface Shape { fun area(): Double }
来源：http://aby.ivvv.top

[T16] Swift：Hello World
来源：http://vml.sufxvd.cn

print("Hello")
来源：http://dcm.zhengqikj.top

[T17] Swift：变量与常量
来源：http://wfr.nwbrower.top

var a = 1;  let b = 2
来源：http://xza.chenzaomai.com

[T18] Swift：字符串插值
来源：http://kzp.wangdashe.top

"值: \(b)"
来源：http://eir.vehdjk.com

[T19] Swift：可选绑定
来源：http://xrv.daxiang520.top

if let n = opt { print(n) }
来源：http://usn.ehwqpu.com

[T20] Swift：数组操作
来源：http://xsj.tarul.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ien.guowangkeji.top

[T21] Swift：遍历
来源：http://pvm.hfpthk.cn

for x in a { print(x) }
来源：http://ect.yuanzhike.top

[T22] Swift：字典
来源：http://jkj.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://mdb.sxryk.cn

[T23] Swift：函数
来源：http://zvl.nwbrower.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ybr.svipenyu.cn

[T24] Swift：闭包
来源：http://bpm.cheryme.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ghb.guannengcc.top

[T25] Swift：结构体
来源：http://weh.yueranfly.top

struct P { var x: Int }
来源：http://uqn.hnqzz.top

[T26] Swift：类与重写
来源：http://ztj.redwolf501.top

class A: Base { override func f() {} }
来源：http://qmi.vqdsnc.cn

[T27] Swift：错误处理
来源：http://cud.nwbrower.top

do { try f() } catch { print(error) }
来源：http://psl.gaohongyu789.top

[T28] Swift：枚举
来源：http://prg.aibaodan.cn

enum Color { case red, green }
来源：http://pix.nanxinkj.top

[T29] Swift：guard 提前返回
来源：http://kdz.zhijiandao.cn

guard let x = opt else { return }
来源：http://kwz.yj202588.top

[T30] Swift：协议
来源：http://azx.ehwqpu.com

protocol Shape { func area() -> Double }
来源：http://kyt.guannengcc.top

[T31] Lua：Hello World
来源：http://wzh.tianlin.xyz

print("Hello")
来源：http://jpj.nanxuanxn.top

[T32] Lua：局部变量
来源：http://bjf.ivvv.top

local a = 1
来源：http://vxt.shanyushiyangtech.top

[T33] Lua：表（数组）
来源：http://flk.sxryk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lmt.shanyushiyangtech.top

[T34] Lua：遍历表
来源：http://kdx.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nkd.xinyue.icu

[T35] Lua：字典表
来源：http://yhz.yj20258888.top

local d = { a = 1 };  d.b = 2
来源：http://qaj.quarkkingdee.top

[T36] Lua：函数
来源：http://tul.jinqigfzy.top

function add(a, b) return a + b end
来源：http://dvx.nanxinkj.top

[T37] Lua：字符串拼接
来源：http://yuw.ywan-chungtsiang.top

"a" .. "b"
来源：http://nqn.9152youxi.cn

[T38] Lua：条件
来源：http://eor.havefunace.top

if x > 0 then print("正") end
来源：http://tlg.tarul.cn

[T39] Lua：模式匹配
来源：http://yem.xinyue.icu

string.find(s, "%d+")
来源：http://sfn.feifeiyinyue.top

[T40] Lua：元表
来源：http://cnd.haohaochexian.top

setmetatable({}, { __index = base })
来源：http://erf.hywenlv.cn

[T41] Perl：Hello World
来源：http://zae.iojbl.cn

print "Hello\n";
来源：http://yem.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://mss.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ttk.zhixingplan.top

[T43] Perl：字符串插值
来源：http://zvh.wangshuangyany.cn

"值: $a"
来源：http://qof.zhixingplan.top

[T44] Perl：条件
来源：http://lnw.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://bnq.birdmap.top


<!-- 参考信息 -->