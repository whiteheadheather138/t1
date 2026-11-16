代发 wailian999

cmd > out.log 2>&1
来源：http://gxl.yueranfly.top

[R40] 追加写日志
来源：http://gqg.ywan-chungtsiang.top

echo "log" >> out.log
来源：http://ltq.xuetiantiany.cn

[R41] 丢弃输出
来源：http://cfv.hesvh.cn

cmd >/dev/null 2>&1
来源：http://nqi.snrcjt.cn

[R42] 输入重定向
来源：http://bxn.snrcjt.cn

wc -l < a.txt
来源：http://xkv.aizwys.cn

[R43] 按名字查找文件
来源：http://tqk.sxryk.cn

find . -name "*.log" -type f
来源：http://hbl.redwolf501.top

[R44] 按修改时间查找
来源：http://jkg.tarul.cn

find . -mtime -7 -type f
来源：http://eiq.andypj.xyz

[R45] 批量删除
来源：http://zpj.aizwys.cn

find . -name "*.tmp" -delete
来源：http://osr.0kj1m.cn

[R46] 递归替换文件内容
来源：http://akc.ctjpmb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://evw.9152youxi.cn

[R47] sed 单行替换
来源：http://usp.mhx1999.top

sed -i 's/foo/bar/g' a.txt
来源：http://tca.zdqjudy.top

[R48] awk 取指定列
来源：http://ntn.zdbjq.cn

awk '{print $1, $3}' a.txt
来源：http://mfb.sjlbkw.cn

[R49] awk 带条件
来源：http://lag.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dts.sjlbkw.cn

[R50] awk 求和
来源：http://lmv.chenlongwang.top

awk '{s += $2} END {print s}' a.txt
来源：http://plh.hammf.cn

[R51] 排序去重取前几
来源：http://oiu.yj20258888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://okq.cashguo.top

[R52] 统计行数
来源：http://enn.zhaomingkeji.xyz

wc -l a.txt
来源：http://bxi.jyoumei.cn

[R53] 查看文件头与实时尾
来源：http://bft.yj20258888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jmm.hywenlv.cn

[R54] 比较两个文件
来源：http://rsw.yonumen.top

diff a.txt b.txt
来源：http://zdy.mhx1999.top

[R55] 压缩与解压
来源：http://ohp.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hws.vehdjk.com

[R56] 远程拷贝
来源：http://ffd.vqdsnc.cn

scp file user@host:/path/
来源：http://pob.nanxuanxn.top

[R57] 远程执行命令
来源：http://nxq.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://pxa.zhijiandao.cn

[R58] 下载文件
来源：http://xpk.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tur.jinqigufen.top

[R59] 发 POST JSON
来源：http://jrs.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kzp.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://gqm.cheryme.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eiu.jlsjyb.cn

[R61] 磁盘占用
来源：http://rhr.dashuyun.cn

df -h;  du -sh *
来源：http://qnq.birdmap.top

[R62] 找最占空间的文件
来源：http://vkk.zdbjq.cn

du -ah . | sort -rh | head -10
来源：http://qgc.ybcxt.top

[R63] 内存与进程
来源：http://exc.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://tnr.ehwqpu.com

[R64] 结束进程
来源：http://dxu.haohaochexian.top

kill -9 $(pgrep -f app.py)
来源：http://wbl.vqdsnc.cn

[R65] 查看端口占用
来源：http://uku.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://swt.jiagoushi.top

[R66] 定时任务
来源：http://rpx.fanxiaobao.xyz

crontab -e;  crontab -l
来源：http://loz.zhixingplan.top

[R67] 生成随机十六进制串
来源：http://qun.zhengqikj.top

openssl rand -hex 16
来源：http://lqp.wangdashe.top

[R68] 计算文件校验值
来源：http://ipq.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sve.tarul.cn

[R69] 生成随机密码
来源：http://ewc.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://tnn.aizwys.cn

[R70] 时间戳与互转
来源：http://rwi.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://lxg.hysaishi.cn

[R71] 日期格式化
来源：http://mtl.zhengqikj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mrj.fzhhl.top

[R72] 等待端口就绪
来源：http://tyc.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lbv.chenjidiqi.icu

[R73] 分割大日志
来源：http://kmk.yanxiufei.cn

split -l 1000 big.log part_
来源：http://hdb.gogol.net.cn

[R74] 批量重命名
来源：http://jfc.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gyi.sufxvd.cn

[R75] 导出环境变量
来源：http://iyg.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://yba.cheryme.top

[R76] 使用临时文件
来源：http://gfr.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nwr.wangshuangyany.cn

[R77] 读取用户输入
来源：http://gig.vehdjk.com

read -rp "请输入: " ans
来源：http://xiy.jinqigufen.top

[R78] 交互式菜单
来源：http://rli.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dlu.ybcxt.top

[R79] 解析命令行选项
来源：http://pzl.dashuyun.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qhx.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://reb.jinyuanbaomall.cn

time ./run.sh
来源：http://cgf.ctjpmb.com

================================================================================
来源：http://qxc.jqgfzy.top

S. C / C++ 专题
来源：http://tlc.ybcxt.top

================================================================================
来源：http://xia.pengpengdd.cyou

[S01] C：Hello World
来源：http://jiw.epnwcf.com

#include <stdio.h>
来源：http://mqi.yj202588.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://sub.0kj1m.cn

[S02] C：变量与格式化输出
来源：http://qth.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://emm.xuetiantiany.cn

[S03] C：读入整数
来源：http://shl.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://dtg.cucudq.cn

[S04] C：字符串复制
来源：http://xhk.yj20258.top

char dst[32]; strcpy(dst, "hi");
来源：http://ozf.kuanghao11.cn

[S05] C：字符串长度
来源：http://cox.gzhubu.top

strlen(s)
来源：http://rau.hammf.cn

[S06] C：字符串比较
来源：http://fyw.yvedp.cn

strcmp(a, b) == 0
来源：http://ezy.xuanzx.com

[S07] C：数组遍历求和
来源：http://oqg.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lew.yonumen.top

[S08] C：动态内存分配与释放
来源：http://imc.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rqn.xinyue.icu

[S09] C：结构体定义与初始化
来源：http://vzu.haohaochexian.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gyj.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://max.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://ukt.xingfuxueyuan.xyz

[S11] C：逐行读文件
来源：http://rkx.hongshengwenyu.top

FILE *f = fopen("a.txt", "r");
来源：http://wrq.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yri.fktsv.cn

fclose(f);
来源：http://jgo.daria6918.cn

[S12] C：写文件
来源：http://krw.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xtl.nwbrower.top

[S13] C：宏定义
来源：http://eip.ctjpmb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ebm.feifeiyinyue.top

[S14] C：枚举
来源：http://dbq.fehbvm.com

enum Color { RED, GREEN, BLUE };
来源：http://hlt.zdbjq.cn

[S15] C：类型转换
来源：http://qpp.jinyuanbaomall.cn

(double) a / b
来源：http://uis.zhengqikj.top

[S16] C：位操作置位
来源：http://wcj.yonumen.top

x |= (1 << 3);
来源：http://tgp.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://deu.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fsm.fehbvm.com

[S18] C：命令行参数
来源：http://gnb.tianlin.xyz

int main(int argc, char **argv)
来源：http://rnn.yuanzhike.top

[S19] C：快速排序
来源：http://taw.hywenlv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fad.smart0.xyz

[S20] C：二分查找
来源：http://iqz.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://igp.hfpthk.cn

[S21] C：字符类别判断
来源：http://wrt.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kzy.sxryk.cn

[S22] C：字符串转数字
来源：http://evc.yj202588.top

atoi("42");  strtod("3.14", NULL);
来源：http://xrc.fzhhl.top

[S23] C：随机数
来源：http://izr.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://vpd.chenzaomai.com

[S24] C：获取本地时间
来源：http://oxr.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eiy.guowangkeji.top

[S25] C：内存拷贝
来源：http://ygb.jiagoushi.top

memcpy(dst, src, n);
来源：http://ajt.bbcook.cn

[S26] C：内存清零
来源：http://bwd.nwbrower.top

memset(a, 0, sizeof a);
来源：http://xrf.daxiang520.top

[S27] C：定义常量
来源：http://tmy.sweek.top

const double PI = 3.14159;
来源：http://fgq.ctjpmb.com

[S28] C：静态变量
来源：http://akv.hywenlv.cn

static int counter = 0;
来源：http://umf.zhiwuduotai.top

[S29] C：变参函数
来源：http://szf.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nzv.aizwys.cn

[S30] C：头文件保护
来源：http://ssh.vqdsnc.cn

#ifndef X_H
来源：http://tvs.epnwcf.com

#define X_H
来源：http://kek.hnxiangtu.top

#endif
来源：http://vyw.sweek.top

[S31] C++：Hello World
来源：http://eob.guowangkeji.top

#include <iostream>
来源：http://fak.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://ieq.chenjidiqi.icu

[S32] C++：字符串
来源：http://glq.iojbl.cn

std::string s = "hi";  s += "!";
来源：http://ygk.wangdashe.top

[S33] C++：vector 增删
来源：http://ofd.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vum.zycfv.cn

[S34] C++：遍历 vector
来源：http://idb.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://jwv.hammf.cn

[S35] C++：map
来源：http://cjh.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ftc.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://wmw.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tvj.hysaishi.cn

[S37] C++：set
来源：http://xle.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jbd.jqgufenzy.top

[S38] C++：排序
来源：http://phn.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://kmv.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://cyr.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jma.sysykeji.top

[S40] C++：查找元素
来源：http://vpa.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jjv.hfpthk.cn

[S41] C++：类与构造函数
来源：http://sxw.daxiang520.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rxw.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://vjd.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://wls.yanxiufei.cn

[S43] C++：智能指针
来源：http://hyp.yvedp.cn

auto p = std::make_unique<int>(5);
来源：http://for.zdqjudy.top

[S44] C++：引用传参
来源：http://ido.smart0.xyz

void inc(int &x) { ++x; }
来源：http://uip.feifeiyinyue.top

[S45] C++：lambda
来源：http://frb.nwbrower.top

auto add = [](int a, int b) { return a + b; };
来源：http://yqy.cucudq.cn

[S46] C++：函数模板
来源：http://bnq.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jsa.sjlbkw.cn

[S47] C++：结构化绑定遍历
来源：http://jbx.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hjb.havefunace.top

[S48] C++：逐行读文件
来源：http://gve.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://enj.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://uin.shanyushiyangtech.top

[S49] C++：写文件
来源：http://bgy.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rhp.sysykeji.top

[S50] C++：格式化数字
来源：http://qxn.tianlin.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rqs.aizwys.cn

[S51] C++：显式类型转换
来源：http://ruh.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://jlj.shzxlz.cn

[S52] C++：const 与 noexcept
来源：http://uwt.hesvh.cn

int size() const noexcept { return n_; }
来源：http://ony.yonumen.top

[S53] C++：移动语义
来源：http://cwv.zdqjudy.top

std::vector<int> w = std::move(v);
来源：http://qgl.52xcode.cn

[S54] C++：异常处理
来源：http://fwn.yj20258888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xow.jianghu66.top

[S55] C++：结构化绑定
来源：http://qeu.yuanzhike.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ekk.yj20258.top

[S56] C++：optional
来源：http://ofy.ybcxt.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xfh.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://emd.iojbl.cn

constexpr int N = 10;
来源：http://sgf.guannengcc.top

[S58] C++：命名空间
来源：http://nsa.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://jou.sjlbkw.cn

[S59] C++：静态断言
来源：http://gnm.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://usg.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://uii.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://shz.zhixingplan.top

================================================================================
来源：http://nzk.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xgm.tarul.cn

================================================================================
来源：http://jwq.nwbrower.top

[T01] Kotlin：Hello World
来源：http://yxf.shanyushiyangkeji.top

println("Hello")
来源：http://kpv.havefunace.top

[T02] Kotlin：变量
来源：http://jce.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pxt.jinqigufen.top

[T03] Kotlin：字符串模板
来源：http://juo.hammf.cn

"值: $b"
来源：http://awv.aizwys.cn

[T04] Kotlin：空安全
来源：http://cid.yvedp.cn

val n: String? = null;  n?.length
来源：http://sak.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://kga.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tdw.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://eku.xingfuxueyuan.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://ndt.yonumen.top

[T07] Kotlin：集合过滤
来源：http://qts.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://eib.cashguo.top

[T08] Kotlin：数据类
来源：http://ryy.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://qdo.chenlongwang.top

[T09] Kotlin：扩展函数
来源：http://wdp.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://bvb.ydzc1.top

[T10] Kotlin：默认参数
来源：http://ntd.tianlin.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://iig.ctjpmb.com

[T11] Kotlin：协程
来源：http://mab.yongpay.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lbr.316326.xyz

[T12] Kotlin：解构声明
来源：http://yzp.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://ypk.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://pmo.sweek.top

val m = mapOf("a" to 1)
来源：http://von.0kj1m.cn

[T14] Kotlin：循环
来源：http://scj.zdbjq.cn

for (i in 1..10) println(i)
来源：http://wsy.cdnleiting.top

[T15] Kotlin：接口
来源：http://jkx.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://dle.fktsv.cn

[T16] Swift：Hello World
来源：http://czr.ywan-chungtsiang.top

print("Hello")
来源：http://mqg.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://gep.cashguo.top

var a = 1;  let b = 2
来源：http://nbl.shanyushiyangkeji.top

[T18] Swift：字符串插值
来源：http://vgv.andypj.xyz

"值: \(b)"
来源：http://fje.hywenlv.cn

[T19] Swift：可选绑定
来源：http://sfa.cashguo.top

if let n = opt { print(n) }
来源：http://dkn.xuetiantiany.cn

[T20] Swift：数组操作
来源：http://kbj.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://ivd.jyoumei.cn

[T21] Swift：遍历
来源：http://ohe.sxryk.cn

for x in a { print(x) }
来源：http://alv.tarul.cn

[T22] Swift：字典
来源：http://ctg.hfpthk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xmx.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://vpk.fanxiaobao.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vmy.cashguo.top

[T24] Swift：闭包
来源：http://lmy.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fid.aizwys.cn

[T25] Swift：结构体
来源：http://ijv.nanxinkj.top

struct P { var x: Int }
来源：http://uxl.tianlin.xyz

[T26] Swift：类与重写
来源：http://sml.guowangkeji.top

class A: Base { override func f() {} }
来源：http://ndz.0kj1m.cn

[T27] Swift：错误处理
来源：http://iqu.aibaodan.cn

do { try f() } catch { print(error) }
来源：http://ryc.jinghuilouyu.cn

[T28] Swift：枚举
来源：http://uai.ydzc1.top

enum Color { case red, green }
来源：http://fzv.0kj1m.cn

[T29] Swift：guard 提前返回
来源：http://eww.xinyue.icu

guard let x = opt else { return }
来源：http://tup.fzhhl.top

[T30] Swift：协议
来源：http://dkk.cqqwz.cn

protocol Shape { func area() -> Double }
来源：http://bsw.fktsv.cn

[T31] Lua：Hello World
来源：http://vcb.bjfxy.top

print("Hello")
来源：http://iir.ehwqpu.com

[T32] Lua：局部变量
来源：http://oib.smart0.xyz

local a = 1
来源：http://ixe.xylfe.cn

[T33] Lua：表（数组）
来源：http://ntd.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iec.jinqigufen.top

[T34] Lua：遍历表
来源：http://ssz.aizwys.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bze.uphjek.com

[T35] Lua：字典表
来源：http://pgd.yongpay.top

local d = { a = 1 };  d.b = 2
来源：http://eis.iojbl.cn

[T36] Lua：函数
来源：http://fou.shanyushiyangkeji.top

function add(a, b) return a + b end
来源：http://arf.zhoulong.xyz

[T37] Lua：字符串拼接
来源：http://tlb.hnxiangtu.top

"a" .. "b"
来源：http://rbt.fzhhl.top

[T38] Lua：条件
来源：http://tni.ehwqpu.com

if x > 0 then print("正") end
来源：http://lag.ybcxt.top

[T39] Lua：模式匹配
来源：http://ubs.xinyue.icu

string.find(s, "%d+")
来源：http://amd.bbcook.cn

[T40] Lua：元表
来源：http://clb.c1oappe.top

setmetatable({}, { __index = base })
来源：http://ldd.ywan-chungtsiang.top

[T41] Perl：Hello World
来源：http://zjx.tanke756.top

print "Hello\n";
来源：http://zal.cdnleiting.top

[T42] Perl：变量类型
来源：http://qqo.dashuyun.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gzp.quarkkingdee.top


<!-- 参考信息 -->