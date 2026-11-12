代发 wailian999

find . -name "*.tmp" -delete
来源：http://ujp.hammf.cn

[R46] 递归替换文件内容
来源：http://dbw.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hcl.hesvh.cn

[R47] sed 单行替换
来源：http://anp.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://orc.yfazqb.com

[R48] awk 取指定列
来源：http://lli.meibo888.top

awk '{print $1, $3}' a.txt
来源：http://mvk.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://ldj.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zbw.xuetiantiany.cn

[R50] awk 求和
来源：http://qxu.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tgy.cashguo.top

[R51] 排序去重取前几
来源：http://qdt.fengsongda.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ewr.haohaochexian.top

[R52] 统计行数
来源：http://weq.zhijiandao.cn

wc -l a.txt
来源：http://sbb.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://fkw.hammf.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://trz.uphjek.com

[R54] 比较两个文件
来源：http://inz.9152youxi.cn

diff a.txt b.txt
来源：http://txa.hnqzz.top

[R55] 压缩与解压
来源：http://fjp.jqgufenzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gta.cqqwz.cn

[R56] 远程拷贝
来源：http://cqf.meibo888.top

scp file user@host:/path/
来源：http://ghw.hnxiangtu.top

[R57] 远程执行命令
来源：http://fia.dianchejie.cn

ssh user@host 'uptime'
来源：http://uum.jyoumei.cn

[R58] 下载文件
来源：http://qwi.jqgufenzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vlk.yvedp.cn

[R59] 发 POST JSON
来源：http://nxa.jinghuilouyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xcj.sweek.top

[R60] 只看 HTTP 状态码
来源：http://xqy.fanxiaobao.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ocv.ctjpmb.com

[R61] 磁盘占用
来源：http://sli.hysaishi.cn

df -h;  du -sh *
来源：http://gwy.meibo888.top

[R62] 找最占空间的文件
来源：http://jir.jinqigufen.top

du -ah . | sort -rh | head -10
来源：http://prp.jianghu66.top

[R63] 内存与进程
来源：http://vdf.yj20258.top

free -h;  ps aux | grep nginx
来源：http://cdn.gaohongyu789.top

[R64] 结束进程
来源：http://ieh.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://wrr.aizwys.cn

[R65] 查看端口占用
来源：http://wzq.zhixingplan.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bki.shanyushiyangkeji.top

[R66] 定时任务
来源：http://nwi.hesvh.cn

crontab -e;  crontab -l
来源：http://trn.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://fcf.chenzaomai.com

openssl rand -hex 16
来源：http://ckt.ppjwa.cn

[R68] 计算文件校验值
来源：http://xnn.hammf.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qgu.cqqwz.cn

[R69] 生成随机密码
来源：http://eke.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://wjk.yvedp.cn

[R70] 时间戳与互转
来源：http://kkm.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://jxl.jiagoushi.top

[R71] 日期格式化
来源：http://djf.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://brv.ivvv.top

[R72] 等待端口就绪
来源：http://mew.zhoulong.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://rem.ydzc1.top

[R73] 分割大日志
来源：http://ugm.jqgufenzy.top

split -l 1000 big.log part_
来源：http://aaa.tarul.cn

[R74] 批量重命名
来源：http://jqj.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zjw.zdqjudy.top

[R75] 导出环境变量
来源：http://afr.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://iqd.316326.xyz

[R76] 使用临时文件
来源：http://hkv.kuanghao11.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uzi.sweek.top

[R77] 读取用户输入
来源：http://ijf.kuanghao11.cn

read -rp "请输入: " ans
来源：http://aip.sjlbkw.cn

[R78] 交互式菜单
来源：http://emj.mhx1999.top

select opt in a b c; do echo "$opt"; break; done
来源：http://luj.bbcook.cn

[R79] 解析命令行选项
来源：http://gsv.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uwz.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://tos.c1oappe.top

time ./run.sh
来源：http://ydb.wangdashe.top

================================================================================
来源：http://pit.tarul.cn

S. C / C++ 专题
来源：http://waf.jlsjyb.cn

================================================================================
来源：http://fba.ivvv.top

[S01] C：Hello World
来源：http://qzg.ppjwa.cn

#include <stdio.h>
来源：http://lmp.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ard.yanxiufei.cn

[S02] C：变量与格式化输出
来源：http://hqd.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://gyv.shzxlz.cn

[S03] C：读入整数
来源：http://koz.smart0.xyz

int x; scanf("%d", &x);
来源：http://gnw.pycfn.com

[S04] C：字符串复制
来源：http://lvl.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vto.shangyingyoupin.top

[S05] C：字符串长度
来源：http://xpz.pengpengdd.cyou

strlen(s)
来源：http://ndj.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://sue.fanxiaobao.xyz

strcmp(a, b) == 0
来源：http://weh.fehbvm.com

[S07] C：数组遍历求和
来源：http://cyw.shuidangran.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fdv.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://ntw.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zbg.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://gxf.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gjd.havefunace.top

[S10] C：指针与解引用
来源：http://psn.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://mcf.hnxiangtu.top

[S11] C：逐行读文件
来源：http://rza.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://tbh.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ezx.hnqzz.top

fclose(f);
来源：http://pee.shuidangran.top

[S12] C：写文件
来源：http://bim.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gei.quarkkingdee.top

[S13] C：宏定义
来源：http://mef.xylfe.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eaz.fehbvm.com

[S14] C：枚举
来源：http://esq.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://top.shanyushiyangtech.top

[S15] C：类型转换
来源：http://klt.tianlin.xyz

(double) a / b
来源：http://ghw.hcnkem.com

[S16] C：位操作置位
来源：http://stz.52xcode.cn

x |= (1 << 3);
来源：http://hhc.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://axq.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uhw.guowangkeji.top

[S18] C：命令行参数
来源：http://xnr.yj202588.top

int main(int argc, char **argv)
来源：http://rrg.daria6918.cn

[S19] C：快速排序
来源：http://qfo.daxiang520.top

qsort(a, n, sizeof(int), cmp);
来源：http://nxj.hnxiangtu.top

[S20] C：二分查找
来源：http://qye.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cyv.shzxlz.cn

[S21] C：字符类别判断
来源：http://vor.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nmf.ybcxt.top

[S22] C：字符串转数字
来源：http://gqe.pycfn.com

atoi("42");  strtod("3.14", NULL);
来源：http://smj.yj20258888.top

[S23] C：随机数
来源：http://xsw.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://cga.jlsjyb.cn

[S24] C：获取本地时间
来源：http://eqt.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vdr.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://oee.yfazqb.com

memcpy(dst, src, n);
来源：http://old.jinqigufen.top

[S26] C：内存清零
来源：http://nie.zhixingplan.top

memset(a, 0, sizeof a);
来源：http://brg.vqdsnc.cn

[S27] C：定义常量
来源：http://cer.mhx1999.top

const double PI = 3.14159;
来源：http://snf.ydjk.org.cn

[S28] C：静态变量
来源：http://uof.fktsv.cn

static int counter = 0;
来源：http://kuq.cdnleiting.top

[S29] C：变参函数
来源：http://tjv.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xzj.jqgufenzy.top

[S30] C：头文件保护
来源：http://tfh.chenjidiqi.icu

#ifndef X_H
来源：http://dcg.jianghu66.top

#define X_H
来源：http://pir.cucudq.cn

#endif
来源：http://kgb.xylfe.cn

[S31] C++：Hello World
来源：http://fnp.ydjk.org.cn

#include <iostream>
来源：http://ive.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://mbp.chenlongwang.top

[S32] C++：字符串
来源：http://ssm.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://zjj.zycfv.cn

[S33] C++：vector 增删
来源：http://lln.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pma.jyoumei.cn

[S34] C++：遍历 vector
来源：http://eug.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://jvx.havefunace.top

[S35] C++：map
来源：http://ssk.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pzy.0kj1m.cn

[S36] C++：unordered_map
来源：http://qdb.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pjo.bjfxy.top

[S37] C++：set
来源：http://ykh.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zrl.guowangkeji.top

[S38] C++：排序
来源：http://sjb.hongshengwenyu.top

std::sort(v.begin(), v.end());
来源：http://irf.havefunace.top

[S39] C++：自定义比较器排序
来源：http://ywm.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://czk.gogol.net.cn

[S40] C++：查找元素
来源：http://efl.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qpd.tian-w.cn

[S41] C++：类与构造函数
来源：http://vse.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jbq.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://fnf.shanyushiyangtech.top

class B : public Base { public: void f() override {} };
来源：http://idw.yuanzhike.top

[S43] C++：智能指针
来源：http://mgq.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://piz.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://pnk.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://rfo.cucudq.cn

[S45] C++：lambda
来源：http://umt.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://aka.jinqigfzy.top

[S46] C++：函数模板
来源：http://syt.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eep.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://ndo.wangshuangyany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qwc.sweek.top

[S48] C++：逐行读文件
来源：http://ylj.tarul.cn

std::ifstream in("a.txt");  std::string line;
来源：http://del.yongpay.top

while (std::getline(in, line)) { }
来源：http://qfl.cqqwz.cn

[S49] C++：写文件
来源：http://rzc.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zmf.fktsv.cn

[S50] C++：格式化数字
来源：http://ogr.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mtr.hywenlv.cn

[S51] C++：显式类型转换
来源：http://fef.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://gng.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://rck.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://zqc.chenzaomai.com

[S53] C++：移动语义
来源：http://pem.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://ivh.yj20258888.top

[S54] C++：异常处理
来源：http://efq.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yxn.fengsongda.top

[S55] C++：结构化绑定
来源：http://ohq.sweek.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yme.guowangkeji.top

[S56] C++：optional
来源：http://azp.sweek.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zwf.jianghu66.top

[S57] C++：编译期常量
来源：http://oxq.zdqjudy.top

constexpr int N = 10;
来源：http://xun.ybcxt.top

[S58] C++：命名空间
来源：http://vix.nanxinkj.top

namespace ns { int f() { return 1; } }
来源：http://blq.fzhhl.top

[S59] C++：静态断言
来源：http://yue.xingfuxueyuan.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rkr.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://pwh.shanyushiyangtech.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oyw.zhongyouzk.top

================================================================================
来源：http://xci.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://emx.jinghuilouyu.cn

================================================================================
来源：http://pza.tarul.cn

[T01] Kotlin：Hello World
来源：http://qcz.vqdsnc.cn

println("Hello")
来源：http://wwo.kuanghao11.cn

[T02] Kotlin：变量
来源：http://son.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uss.aizwys.cn

[T03] Kotlin：字符串模板
来源：http://nmf.shanyushiyangtech.top

"值: $b"
来源：http://xhc.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://gkc.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://xav.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://fgf.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tjd.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://awv.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://yoc.uphjek.com

[T07] Kotlin：集合过滤
来源：http://dpc.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xrs.zhengqikj.top

[T08] Kotlin：数据类
来源：http://bfe.hongshengwenyu.top

data class User(val name: String, val age: Int)
来源：http://ggj.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://ytj.yueranfly.top

fun String.exclaim() = this + "!"
来源：http://gok.zhaomingkeji.xyz

[T10] Kotlin：默认参数
来源：http://bwn.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ikt.xuanzx.com

[T11] Kotlin：协程
来源：http://enp.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ibp.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://nin.shzxlz.cn

val (a, b) = Pair(1, 2)
来源：http://zmk.tarul.cn

[T13] Kotlin：只读 Map
来源：http://lml.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://awe.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://ilk.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://lrv.zhiwuduotai.top

[T15] Kotlin：接口
来源：http://djh.ctjpmb.com

interface Shape { fun area(): Double }
来源：http://cvf.ybcxt.top

[T16] Swift：Hello World
来源：http://dam.hywenlv.cn

print("Hello")
来源：http://euv.tarul.cn

[T17] Swift：变量与常量
来源：http://usm.andypj.xyz

var a = 1;  let b = 2
来源：http://tdj.xinyue.icu

[T18] Swift：字符串插值
来源：http://cmv.chenjidiqi.icu

"值: \(b)"
来源：http://qwb.vehdjk.com

[T19] Swift：可选绑定
来源：http://iqz.nwbrower.top

if let n = opt { print(n) }
来源：http://zwu.wangdashe.top

[T20] Swift：数组操作
来源：http://uqs.gaohongyu789.top

var a = [1, 2, 3];  a.append(4)
来源：http://kkr.yangfankeji.com

[T21] Swift：遍历
来源：http://htv.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://olb.xingfuxueyuan.xyz

[T22] Swift：字典
来源：http://hjq.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://dfj.gotoacloud.top

[T23] Swift：函数
来源：http://knq.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yqs.zhongyouzk.top

[T24] Swift：闭包
来源：http://ewo.yanxiufei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cao.birdmap.top

[T25] Swift：结构体
来源：http://wjj.hammf.cn

struct P { var x: Int }
来源：http://lft.fktsv.cn

[T26] Swift：类与重写
来源：http://jbd.sxryk.cn

class A: Base { override func f() {} }
来源：http://veb.hnqzz.top

[T27] Swift：错误处理
来源：http://kra.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://hwo.fehbvm.com

[T28] Swift：枚举
来源：http://ebv.hnqzz.top

enum Color { case red, green }
来源：http://yol.epnwcf.com

[T29] Swift：guard 提前返回
来源：http://iay.birdmap.top

guard let x = opt else { return }
来源：http://gtm.jinghuilouyu.cn

[T30] Swift：协议
来源：http://nva.0kj1m.cn

protocol Shape { func area() -> Double }
来源：http://zcn.ctjpmb.com

[T31] Lua：Hello World
来源：http://bzf.dashuyun.cn

print("Hello")
来源：http://qii.bbcook.cn

[T32] Lua：局部变量
来源：http://mrj.fzhhl.top

local a = 1
来源：http://ltz.gotoacloud.top

[T33] Lua：表（数组）
来源：http://okf.cheryme.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vcf.dianchejie.cn

[T34] Lua：遍历表
来源：http://clg.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xij.jqgufenzy.top

[T35] Lua：字典表
来源：http://jbh.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://jhk.cheryme.top

[T36] Lua：函数
来源：http://wtg.ehwqpu.com

function add(a, b) return a + b end
来源：http://qym.cheryme.top

[T37] Lua：字符串拼接
来源：http://qxq.gzhubu.top

"a" .. "b"
来源：http://plx.snrcjt.cn

[T38] Lua：条件
来源：http://hyf.zhaomingkeji.xyz

if x > 0 then print("正") end
来源：http://hpy.svipenyu.cn

[T39] Lua：模式匹配
来源：http://psv.xinyue.icu

string.find(s, "%d+")
来源：http://dcx.tarul.cn

[T40] Lua：元表
来源：http://bwe.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://hbj.epnwcf.com

[T41] Perl：Hello World
来源：http://rvx.nanxinkj.top

print "Hello\n";
来源：http://auu.fanxiaobao.xyz

[T42] Perl：变量类型
来源：http://cum.yuanzhike.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hgw.yonumen.top

[T43] Perl：字符串插值
来源：http://hpt.xziqi.cn

"值: $a"
来源：http://naw.sweek.top

[T44] Perl：条件
来源：http://qdr.fengsongda.top

if ($a > 0) { print "正"; }
来源：http://tkv.zhixingplan.top

[T45] Perl：数组遍历
来源：http://znx.hnqzz.top

for my $x (@arr) { print $x; }
来源：http://pzv.zhixingplan.top

[T46] Perl：哈希操作
来源：http://gfh.aibaodan.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wbp.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://mjw.xuanzx.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://kbf.jqgufenzy.top

[T48] Perl：正则替换
来源：http://lyw.havefunace.top

$s =~ s/old/new/g;
来源：http://huw.jqgfzy.top


<!-- 参考信息 -->