代发 wailian999

cmd >/dev/null 2>&1
来源：http://nlp.ehwqpu.com

[R42] 输入重定向
来源：http://jwe.hongshengwenyu.top

wc -l < a.txt
来源：http://ufi.havefunace.top

[R43] 按名字查找文件
来源：http://ekh.jlsjyb.cn

find . -name "*.log" -type f
来源：http://wkl.hnqzz.top

[R44] 按修改时间查找
来源：http://dxt.zycfv.cn

find . -mtime -7 -type f
来源：http://wgi.dianchejie.cn

[R45] 批量删除
来源：http://gup.mhx1999.top

find . -name "*.tmp" -delete
来源：http://ldw.xuanzx.com

[R46] 递归替换文件内容
来源：http://owi.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://env.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://chy.cucudq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ecz.havefunace.top

[R48] awk 取指定列
来源：http://rgz.zdbjq.cn

awk '{print $1, $3}' a.txt
来源：http://vlx.jianghu66.top

[R49] awk 带条件
来源：http://jir.jianghu66.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tnl.shzxlz.cn

[R50] awk 求和
来源：http://acz.52xcode.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ruf.zdqjudy.top

[R51] 排序去重取前几
来源：http://bwr.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://vpa.zdbjq.cn

[R52] 统计行数
来源：http://nqx.chenzaomai.com

wc -l a.txt
来源：http://llw.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://ill.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bsh.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://aoi.mhx1999.top

diff a.txt b.txt
来源：http://bry.zhengqikj.top

[R55] 压缩与解压
来源：http://zed.sweek.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://egh.guowangkeji.top

[R56] 远程拷贝
来源：http://vxm.xuanzx.com

scp file user@host:/path/
来源：http://nhi.xingfuxueyuan.xyz

[R57] 远程执行命令
来源：http://iqc.gogol.net.cn

ssh user@host 'uptime'
来源：http://akq.feifeiyinyue.top

[R58] 下载文件
来源：http://hbl.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://myu.pycfn.com

[R59] 发 POST JSON
来源：http://voh.ywan-chungtsiang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://knb.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://boa.fengsongda.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yab.hongshengwenyu.top

[R61] 磁盘占用
来源：http://cbw.yvedp.cn

df -h;  du -sh *
来源：http://boc.zdqjudy.top

[R62] 找最占空间的文件
来源：http://xau.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://xzr.nwbrower.top

[R63] 内存与进程
来源：http://wkr.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://tva.snrcjt.cn

[R64] 结束进程
来源：http://tuy.svipenyu.cn

kill -9 $(pgrep -f app.py)
来源：http://wyt.fktsv.cn

[R65] 查看端口占用
来源：http://uxy.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jxk.jinyuanbaomall.cn

[R66] 定时任务
来源：http://lra.sufxvd.cn

crontab -e;  crontab -l
来源：http://ezr.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://xrg.aibaodan.cn

openssl rand -hex 16
来源：http://kuu.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://zoz.zhongyouzk.top

sha256sum a.txt;  md5sum a.txt
来源：http://vis.xuetiantiany.cn

[R69] 生成随机密码
来源：http://fmn.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://gai.tian-w.cn

[R70] 时间戳与互转
来源：http://vjg.jinqigufen.top

date +%s;  date -d @1700000000
来源：http://zmk.guannengcc.top

[R71] 日期格式化
来源：http://zkp.fzhhl.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tcy.hfpthk.cn

[R72] 等待端口就绪
来源：http://api.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://big.hongshengwenyu.top

[R73] 分割大日志
来源：http://amc.vqdsnc.cn

split -l 1000 big.log part_
来源：http://nba.yuanzhike.top

[R74] 批量重命名
来源：http://ylk.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ukx.hnxiangtu.top

[R75] 导出环境变量
来源：http://alj.gaohongyu789.top

export PATH="$HOME/bin:$PATH"
来源：http://djn.sxryk.cn

[R76] 使用临时文件
来源：http://bhw.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ndy.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://nvy.svipenyu.cn

read -rp "请输入: " ans
来源：http://ofn.zhiwuduotai.top

[R78] 交互式菜单
来源：http://wfb.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://idl.zhoulong.xyz

[R79] 解析命令行选项
来源：http://jpw.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://usf.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://gme.bbcook.cn

time ./run.sh
来源：http://rqw.hnxiangtu.top

================================================================================
来源：http://zck.yuanzhike.top

S. C / C++ 专题
来源：http://iis.9152youxi.cn

================================================================================
来源：http://eev.xylfe.cn

[S01] C：Hello World
来源：http://hvn.hnxiangtu.top

#include <stdio.h>
来源：http://qrv.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fxd.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://lxm.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://tyg.vqdsnc.cn

[S03] C：读入整数
来源：http://rbn.guannengcc.top

int x; scanf("%d", &x);
来源：http://vfi.jiagoushi.top

[S04] C：字符串复制
来源：http://ymp.birdmap.top

char dst[32]; strcpy(dst, "hi");
来源：http://fwm.cdnleiting.top

[S05] C：字符串长度
来源：http://nue.svipenyu.cn

strlen(s)
来源：http://fbm.yj20258.top

[S06] C：字符串比较
来源：http://bcu.gzhubu.top

strcmp(a, b) == 0
来源：http://fsq.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://ikt.jianghu66.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hbv.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://toc.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://frf.ydjk.org.cn

[S09] C：结构体定义与初始化
来源：http://nov.havefunace.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xhp.aibaodan.cn

[S10] C：指针与解引用
来源：http://hqx.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://psm.dashuyun.cn

[S11] C：逐行读文件
来源：http://vpl.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://hqx.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zgc.redwolf501.top

fclose(f);
来源：http://ngj.jinqigfzy.top

[S12] C：写文件
来源：http://rkx.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ubk.feifeiyinyue.top

[S13] C：宏定义
来源：http://oox.yj20258888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kyz.aizwys.cn

[S14] C：枚举
来源：http://rsr.zhoulong.xyz

enum Color { RED, GREEN, BLUE };
来源：http://wje.hongshengwenyu.top

[S15] C：类型转换
来源：http://byk.hesvh.cn

(double) a / b
来源：http://hsi.sysykeji.top

[S16] C：位操作置位
来源：http://xad.jqgfzy.top

x |= (1 << 3);
来源：http://ggm.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://xou.bjfxy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yts.snrcjt.cn

[S18] C：命令行参数
来源：http://vqa.sjlbkw.cn

int main(int argc, char **argv)
来源：http://gpt.fzhhl.top

[S19] C：快速排序
来源：http://zze.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oen.yueranfly.top

[S20] C：二分查找
来源：http://iqb.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rjv.hnqzz.top

[S21] C：字符类别判断
来源：http://muo.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://buq.zhijiandao.cn

[S22] C：字符串转数字
来源：http://itb.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oii.jianghu66.top

[S23] C：随机数
来源：http://ets.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://diq.ivvv.top

[S24] C：获取本地时间
来源：http://gfi.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ihj.yvedp.cn

[S25] C：内存拷贝
来源：http://vcr.kuanghao11.cn

memcpy(dst, src, n);
来源：http://yrq.chenzaomai.com

[S26] C：内存清零
来源：http://xrd.52xcode.cn

memset(a, 0, sizeof a);
来源：http://wqo.hcnkem.com

[S27] C：定义常量
来源：http://kht.yonumen.top

const double PI = 3.14159;
来源：http://zqi.jianghu66.top

[S28] C：静态变量
来源：http://ego.yanxiufei.cn

static int counter = 0;
来源：http://tqs.zdbjq.cn

[S29] C：变参函数
来源：http://mnt.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xjj.ybcxt.top

[S30] C：头文件保护
来源：http://kmy.iojbl.cn

#ifndef X_H
来源：http://zeg.shanyushiyangtech.top

#define X_H
来源：http://ajm.tian-w.cn

#endif
来源：http://zqi.hesvh.cn

[S31] C++：Hello World
来源：http://vcu.aibaodan.cn

#include <iostream>
来源：http://gpg.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://svf.tian-w.cn

[S32] C++：字符串
来源：http://xgj.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://zir.hfpthk.cn

[S33] C++：vector 增删
来源：http://aac.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://saz.yongpay.top

[S34] C++：遍历 vector
来源：http://gxc.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://yvs.c1oappe.top

[S35] C++：map
来源：http://tkq.vqdsnc.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kqs.hfpthk.cn

[S36] C++：unordered_map
来源：http://nkv.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eat.yuxming.cn

[S37] C++：set
来源：http://tsy.hongshengwenyu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kgs.cheryme.top

[S38] C++：排序
来源：http://lfh.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://tmj.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://ijo.jinyuanbaomall.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bmp.cheryme.top

[S40] C++：查找元素
来源：http://egz.aizwys.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yde.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://guy.yj202588.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uwx.shanyushiyangtech.top

[S42] C++：继承与虚函数
来源：http://xly.xinyue.icu

class B : public Base { public: void f() override {} };
来源：http://ncm.cqqwz.cn

[S43] C++：智能指针
来源：http://ohn.ydjk.org.cn

auto p = std::make_unique<int>(5);
来源：http://umf.tian-w.cn

[S44] C++：引用传参
来源：http://jyk.cashguo.top

void inc(int &x) { ++x; }
来源：http://fey.tanke756.top

[S45] C++：lambda
来源：http://mnw.ppjwa.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mhc.cqqwz.cn

[S46] C++：函数模板
来源：http://eho.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eoz.yongpay.top

[S47] C++：结构化绑定遍历
来源：http://oeq.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rmv.yuxming.cn

[S48] C++：逐行读文件
来源：http://wxt.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://qby.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://lfd.zhixingplan.top

[S49] C++：写文件
来源：http://nfc.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mfo.yonumen.top

[S50] C++：格式化数字
来源：http://ipe.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://stt.tian-w.cn

[S51] C++：显式类型转换
来源：http://dph.yj202588.top

static_cast<double>(a) / b
来源：http://riq.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://xwt.316326.xyz

int size() const noexcept { return n_; }
来源：http://usb.zdqjudy.top

[S53] C++：移动语义
来源：http://yvp.chenlongwang.top

std::vector<int> w = std::move(v);
来源：http://ijp.kuanghao11.cn

[S54] C++：异常处理
来源：http://dao.jianghu66.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eee.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://yfj.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fdx.svipenyu.cn

[S56] C++：optional
来源：http://gfi.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ydf.hcnkem.com

[S57] C++：编译期常量
来源：http://cas.yonumen.top

constexpr int N = 10;
来源：http://fpo.pengpengdd.cyou

[S58] C++：命名空间
来源：http://dqq.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://vro.guowangkeji.top

[S59] C++：静态断言
来源：http://tix.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mdq.yfazqb.com

[S60] C++：遍历并删除元素
来源：http://aza.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ube.hongshengwenyu.top

================================================================================
来源：http://dvv.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fok.kuanghao11.cn

================================================================================
来源：http://bbo.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://jgf.chenjidiqi.icu

println("Hello")
来源：http://ktn.ppjwa.cn

[T02] Kotlin：变量
来源：http://buy.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ajm.tarul.cn

[T03] Kotlin：字符串模板
来源：http://ntp.tian-w.cn

"值: $b"
来源：http://cet.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://ehn.jinqigfzy.top

val n: String? = null;  n?.length
来源：http://ija.sweek.top

[T05] Kotlin：when 表达式
来源：http://lnj.hcnkem.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ice.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://rha.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://feg.316326.xyz

[T07] Kotlin：集合过滤
来源：http://gvb.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wiu.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://igj.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://jem.chenlongwang.top

[T09] Kotlin：扩展函数
来源：http://qwc.hammf.cn

fun String.exclaim() = this + "!"
来源：http://lal.316326.xyz

[T10] Kotlin：默认参数
来源：http://yxg.fehbvm.com

fun greet(name: String = "World") = "Hi $name"
来源：http://jrr.jinghuilouyu.cn

[T11] Kotlin：协程
来源：http://trb.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cby.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://iyn.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://ypk.meibo888.top

[T13] Kotlin：只读 Map
来源：http://vqt.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://btj.zhoulong.xyz

[T14] Kotlin：循环
来源：http://qld.fanxiaobao.xyz

for (i in 1..10) println(i)
来源：http://zle.jyoumei.cn

[T15] Kotlin：接口
来源：http://pnh.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://pgc.hcnkem.com

[T16] Swift：Hello World
来源：http://kxg.vehdjk.com

print("Hello")
来源：http://oka.gaohongyu789.top

[T17] Swift：变量与常量
来源：http://bad.hnqzz.top

var a = 1;  let b = 2
来源：http://bfc.ivvv.top

[T18] Swift：字符串插值
来源：http://lat.zdbjq.cn

"值: \(b)"
来源：http://kfm.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://cax.epnwcf.com

if let n = opt { print(n) }
来源：http://ptp.jqgufenzy.top

[T20] Swift：数组操作
来源：http://gim.jlsjyb.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qhk.shuidangran.top

[T21] Swift：遍历
来源：http://beb.jiagoushi.top

for x in a { print(x) }
来源：http://sod.tian-w.cn

[T22] Swift：字典
来源：http://mzn.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kvl.yj202588.top

[T23] Swift：函数
来源：http://ngh.yj20258.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ekn.jlsjyb.cn

[T24] Swift：闭包
来源：http://usf.shanyushiyangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xlv.havefunace.top

[T25] Swift：结构体
来源：http://qfq.tianlin.xyz

struct P { var x: Int }
来源：http://qmv.tarul.cn

[T26] Swift：类与重写
来源：http://csw.xylfe.cn

class A: Base { override func f() {} }
来源：http://hks.yfazqb.com

[T27] Swift：错误处理
来源：http://ons.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://cts.hnxiangtu.top

[T28] Swift：枚举
来源：http://pte.ydzc1.top

enum Color { case red, green }
来源：http://fkj.ywan-chungtsiang.top

[T29] Swift：guard 提前返回
来源：http://adk.xuetiantiany.cn

guard let x = opt else { return }
来源：http://yvo.ybcxt.top

[T30] Swift：协议
来源：http://kov.cheryme.top

protocol Shape { func area() -> Double }
来源：http://sew.xingfuxueyuan.xyz

[T31] Lua：Hello World
来源：http://zhz.xuetiantiany.cn

print("Hello")
来源：http://njw.uphjek.com

[T32] Lua：局部变量
来源：http://vcs.aizwys.cn

local a = 1
来源：http://auw.xuanzx.com

[T33] Lua：表（数组）
来源：http://uch.316326.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://els.xziqi.cn

[T34] Lua：遍历表
来源：http://rkv.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xoo.aibaodan.cn

[T35] Lua：字典表
来源：http://mgl.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://jtp.shuidangran.top

[T36] Lua：函数
来源：http://vfj.shuidangran.top

function add(a, b) return a + b end
来源：http://zbj.nwbrower.top

[T37] Lua：字符串拼接
来源：http://cuu.snrcjt.cn

"a" .. "b"
来源：http://zqv.jlsjyb.cn

[T38] Lua：条件
来源：http://gmv.havefunace.top

if x > 0 then print("正") end
来源：http://pua.birdmap.top

[T39] Lua：模式匹配
来源：http://mvw.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://zmp.cqqwz.cn

[T40] Lua：元表
来源：http://gtp.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://xzy.hnxiangtu.top

[T41] Perl：Hello World
来源：http://bue.xylfe.cn

print "Hello\n";
来源：http://jwi.kuanghao11.cn

[T42] Perl：变量类型
来源：http://rmp.zdqjudy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ekb.ctjpmb.com

[T43] Perl：字符串插值
来源：http://ofu.hesvh.cn

"值: $a"
来源：http://npy.zhaomingkeji.xyz

[T44] Perl：条件
来源：http://rqa.birdmap.top

if ($a > 0) { print "正"; }
来源：http://ppt.cashguo.top


<!-- 参考信息 -->