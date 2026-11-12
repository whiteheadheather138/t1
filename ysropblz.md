代发 wailian999

find . -name "*.tmp" -delete
来源：http://yvy.ctjpmb.com

[R46] 递归替换文件内容
来源：http://avl.tarul.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kxi.redwolf501.top

[R47] sed 单行替换
来源：http://pro.yuxming.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jbd.shanyushiyangtech.top

[R48] awk 取指定列
来源：http://vwa.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://jgb.xuetiantiany.cn

[R49] awk 带条件
来源：http://dzt.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tdz.cqqwz.cn

[R50] awk 求和
来源：http://wtt.bjfxy.top

awk '{s += $2} END {print s}' a.txt
来源：http://jwy.ydzc1.top

[R51] 排序去重取前几
来源：http://ctj.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yan.chenjidiqi.icu

[R52] 统计行数
来源：http://rnl.gzhubu.top

wc -l a.txt
来源：http://cud.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://pgk.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mlq.chenzaomai.com

[R54] 比较两个文件
来源：http://yzi.aizwys.cn

diff a.txt b.txt
来源：http://hit.tanke756.top

[R55] 压缩与解压
来源：http://zek.iojbl.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gro.chenzaomai.com

[R56] 远程拷贝
来源：http://mrt.shanyushiyangkeji.top

scp file user@host:/path/
来源：http://jmg.xziqi.cn

[R57] 远程执行命令
来源：http://wiq.pycfn.com

ssh user@host 'uptime'
来源：http://idh.pengpengdd.cyou

[R58] 下载文件
来源：http://vpr.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gfk.hesvh.cn

[R59] 发 POST JSON
来源：http://igg.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zvs.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://ion.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wxk.yuxming.cn

[R61] 磁盘占用
来源：http://mgc.chenlongwang.top

df -h;  du -sh *
来源：http://ypj.c1oappe.top

[R62] 找最占空间的文件
来源：http://cph.zdbjq.cn

du -ah . | sort -rh | head -10
来源：http://fxy.shanyushiyangtech.top

[R63] 内存与进程
来源：http://skp.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://hnj.birdmap.top

[R64] 结束进程
来源：http://hdk.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://kte.gzhubu.top

[R65] 查看端口占用
来源：http://ccv.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dqr.xinyue.icu

[R66] 定时任务
来源：http://fym.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://jih.52xcode.cn

[R67] 生成随机十六进制串
来源：http://zbu.cucudq.cn

openssl rand -hex 16
来源：http://kjr.tianlin.xyz

[R68] 计算文件校验值
来源：http://uoi.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ggj.sxryk.cn

[R69] 生成随机密码
来源：http://wgo.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://xhq.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://nhf.yuanzhike.top

date +%s;  date -d @1700000000
来源：http://goc.epnwcf.com

[R71] 日期格式化
来源：http://cyh.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ozu.epnwcf.com

[R72] 等待端口就绪
来源：http://fad.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://msg.xuetiantiany.cn

[R73] 分割大日志
来源：http://jly.sjlbkw.cn

split -l 1000 big.log part_
来源：http://zwe.sysykeji.top

[R74] 批量重命名
来源：http://kdr.jqgufenzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jmh.nanxuanxn.top

[R75] 导出环境变量
来源：http://waj.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://tkj.ctjpmb.com

[R76] 使用临时文件
来源：http://iyg.yuxming.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://heo.kuanghao11.cn

[R77] 读取用户输入
来源：http://goy.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://upv.yueranfly.top

[R78] 交互式菜单
来源：http://qyg.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://mju.shzxlz.cn

[R79] 解析命令行选项
来源：http://wie.epnwcf.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yrt.yonumen.top

[R80] 查看脚本执行耗时
来源：http://uvy.ybcxt.top

time ./run.sh
来源：http://afg.jlsjyb.cn

================================================================================
来源：http://idu.zhiwuduotai.top

S. C / C++ 专题
来源：http://xeg.hysaishi.cn

================================================================================
来源：http://brz.snrcjt.cn

[S01] C：Hello World
来源：http://mwp.havefunace.top

#include <stdio.h>
来源：http://ghd.aibaodan.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xew.cucudq.cn

[S02] C：变量与格式化输出
来源：http://wzt.chenzaomai.com

int a = 10; printf("%d\n", a);
来源：http://ipx.dashuyun.cn

[S03] C：读入整数
来源：http://xvi.jinqigufen.top

int x; scanf("%d", &x);
来源：http://cdn.wangshuangyany.cn

[S04] C：字符串复制
来源：http://chm.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://vpq.shzxlz.cn

[S05] C：字符串长度
来源：http://szi.yj20258888.top

strlen(s)
来源：http://nxh.vqdsnc.cn

[S06] C：字符串比较
来源：http://hbe.jinqigfzy.top

strcmp(a, b) == 0
来源：http://xhv.shzxlz.cn

[S07] C：数组遍历求和
来源：http://not.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rsi.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://kuj.fehbvm.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hvh.jlsjyb.cn

[S09] C：结构体定义与初始化
来源：http://hxz.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ojs.dashuyun.cn

[S10] C：指针与解引用
来源：http://syg.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://zvu.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://kga.ctjpmb.com

FILE *f = fopen("a.txt", "r");
来源：http://hle.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ydc.hongshengwenyu.top

fclose(f);
来源：http://hxh.xingfuxueyuan.xyz

[S12] C：写文件
来源：http://vbw.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mdi.vqdsnc.cn

[S13] C：宏定义
来源：http://oya.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hun.sjlbkw.cn

[S14] C：枚举
来源：http://oon.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://rlj.bjfxy.top

[S15] C：类型转换
来源：http://ydw.yonumen.top

(double) a / b
来源：http://klu.sxryk.cn

[S16] C：位操作置位
来源：http://stp.yanxiufei.cn

x |= (1 << 3);
来源：http://dwe.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://eql.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wlj.cheryme.top

[S18] C：命令行参数
来源：http://goa.ctjpmb.com

int main(int argc, char **argv)
来源：http://wnn.jiagoushi.top

[S19] C：快速排序
来源：http://lqj.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bbf.gaohongyu789.top

[S20] C：二分查找
来源：http://znr.jianghu66.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rmr.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://qgz.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ire.hfpthk.cn

[S22] C：字符串转数字
来源：http://hpu.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vzi.9152youxi.cn

[S23] C：随机数
来源：http://tnf.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hfn.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://rrh.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sxm.zdbjq.cn

[S25] C：内存拷贝
来源：http://auw.nwbrower.top

memcpy(dst, src, n);
来源：http://oao.zdbjq.cn

[S26] C：内存清零
来源：http://kow.pengpengdd.cyou

memset(a, 0, sizeof a);
来源：http://bvi.sysykeji.top

[S27] C：定义常量
来源：http://oph.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://day.yueranfly.top

[S28] C：静态变量
来源：http://ewv.xziqi.cn

static int counter = 0;
来源：http://mux.guannengcc.top

[S29] C：变参函数
来源：http://oet.xingfuxueyuan.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ljw.0kj1m.cn

[S30] C：头文件保护
来源：http://jhi.havefunace.top

#ifndef X_H
来源：http://mrm.sysykeji.top

#define X_H
来源：http://mrf.hfpthk.cn

#endif
来源：http://lvr.guowangkeji.top

[S31] C++：Hello World
来源：http://ayk.aibaodan.cn

#include <iostream>
来源：http://frm.fanxiaobao.xyz

int main() { std::cout << "Hello\n"; }
来源：http://wxg.nwbrower.top

[S32] C++：字符串
来源：http://gtl.hywenlv.cn

std::string s = "hi";  s += "!";
来源：http://dkk.52xcode.cn

[S33] C++：vector 增删
来源：http://cto.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cwp.zdbjq.cn

[S34] C++：遍历 vector
来源：http://vcx.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://zee.zycfv.cn

[S35] C++：map
来源：http://mvo.jinqigufen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nyp.dashuyun.cn

[S36] C++：unordered_map
来源：http://gvz.cucudq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aie.jinqigfzy.top

[S37] C++：set
来源：http://mot.vehdjk.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hhr.snrcjt.cn

[S38] C++：排序
来源：http://trp.vehdjk.com

std::sort(v.begin(), v.end());
来源：http://awt.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://hvr.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yjn.zdbjq.cn

[S40] C++：查找元素
来源：http://djn.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iez.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://ljb.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pyr.tanke756.top

[S42] C++：继承与虚函数
来源：http://grn.9152youxi.cn

class B : public Base { public: void f() override {} };
来源：http://uvi.cdnleiting.top

[S43] C++：智能指针
来源：http://qhw.hongshengwenyu.top

auto p = std::make_unique<int>(5);
来源：http://cah.tanke756.top

[S44] C++：引用传参
来源：http://ami.fzhhl.top

void inc(int &x) { ++x; }
来源：http://bly.zycfv.cn

[S45] C++：lambda
来源：http://dum.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://imz.xingfuxueyuan.xyz

[S46] C++：函数模板
来源：http://uyx.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ypm.vqdsnc.cn

[S47] C++：结构化绑定遍历
来源：http://lgh.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ctq.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://jhg.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://xfm.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://fnp.jiagoushi.top

[S49] C++：写文件
来源：http://uce.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dao.tanke756.top

[S50] C++：格式化数字
来源：http://wib.tarul.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pxz.pycfn.com

[S51] C++：显式类型转换
来源：http://nqz.ybcxt.top

static_cast<double>(a) / b
来源：http://iim.9152youxi.cn

[S52] C++：const 与 noexcept
来源：http://vyr.sjlbkw.cn

int size() const noexcept { return n_; }
来源：http://cwc.sweek.top

[S53] C++：移动语义
来源：http://tsf.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://rfy.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://ivw.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qaq.gzhubu.top

[S55] C++：结构化绑定
来源：http://vrp.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://iar.chenjidiqi.icu

[S56] C++：optional
来源：http://ovs.xuanzx.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cjx.ctjpmb.com

[S57] C++：编译期常量
来源：http://lia.yj20258888.top

constexpr int N = 10;
来源：http://mhr.ppjwa.cn

[S58] C++：命名空间
来源：http://fvc.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://dhu.zhijiandao.cn

[S59] C++：静态断言
来源：http://iti.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://viy.ydjk.org.cn

[S60] C++：遍历并删除元素
来源：http://gxl.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hnx.pengpengdd.cyou

================================================================================
来源：http://wff.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://atv.nanxuanxn.top

================================================================================
来源：http://sju.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://qda.zhoulong.xyz

println("Hello")
来源：http://ovv.gzhubu.top

[T02] Kotlin：变量
来源：http://dnj.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vco.wangdashe.top

[T03] Kotlin：字符串模板
来源：http://blh.bbcook.cn

"值: $b"
来源：http://pky.chenzaomai.com

[T04] Kotlin：空安全
来源：http://wei.aizwys.cn

val n: String? = null;  n?.length
来源：http://irx.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://upg.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kiy.wangshuangyany.cn

[T06] Kotlin：集合映射
来源：http://rdr.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lze.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://rqg.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vqy.dashuyun.cn

[T08] Kotlin：数据类
来源：http://she.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://wxx.epnwcf.com

[T09] Kotlin：扩展函数
来源：http://lru.birdmap.top

fun String.exclaim() = this + "!"
来源：http://xxd.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://ivz.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bpk.xinyue.icu

[T11] Kotlin：协程
来源：http://fqp.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://crg.ywan-chungtsiang.top

[T12] Kotlin：解构声明
来源：http://xhx.feifeiyinyue.top

val (a, b) = Pair(1, 2)
来源：http://cto.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://lan.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://owy.epnwcf.com

[T14] Kotlin：循环
来源：http://cfc.gotoacloud.top

for (i in 1..10) println(i)
来源：http://qql.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://adq.zhijiandao.cn

interface Shape { fun area(): Double }
来源：http://nhx.sweek.top

[T16] Swift：Hello World
来源：http://itv.hywenlv.cn

print("Hello")
来源：http://xfd.redwolf501.top

[T17] Swift：变量与常量
来源：http://pcx.xziqi.cn

var a = 1;  let b = 2
来源：http://wfr.aizwys.cn

[T18] Swift：字符串插值
来源：http://foo.hammf.cn

"值: \(b)"
来源：http://ugb.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://enq.gogol.net.cn

if let n = opt { print(n) }
来源：http://hpw.cqqwz.cn

[T20] Swift：数组操作
来源：http://jkm.bbcook.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oaw.hnxiangtu.top

[T21] Swift：遍历
来源：http://iqe.hongshengwenyu.top

for x in a { print(x) }
来源：http://tyh.nwbrower.top

[T22] Swift：字典
来源：http://dhb.ydjk.org.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wux.hammf.cn

[T23] Swift：函数
来源：http://adb.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jqs.yueranfly.top

[T24] Swift：闭包
来源：http://xhv.yonumen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vkm.cheryme.top

[T25] Swift：结构体
来源：http://utf.sjlbkw.cn

struct P { var x: Int }
来源：http://pzi.pycfn.com

[T26] Swift：类与重写
来源：http://lnj.jinqigufen.top

class A: Base { override func f() {} }
来源：http://ois.wangdashe.top

[T27] Swift：错误处理
来源：http://ssm.bjfxy.top

do { try f() } catch { print(error) }
来源：http://lhd.yj20258888.top

[T28] Swift：枚举
来源：http://pkn.gotoacloud.top

enum Color { case red, green }
来源：http://vqh.vqdsnc.cn

[T29] Swift：guard 提前返回
来源：http://fvh.birdmap.top

guard let x = opt else { return }
来源：http://qrg.yuanzhike.top

[T30] Swift：协议
来源：http://wys.nanxinkj.top

protocol Shape { func area() -> Double }
来源：http://pdw.yj202588.top

[T31] Lua：Hello World
来源：http://mvg.c1oappe.top

print("Hello")
来源：http://lrx.ppjwa.cn

[T32] Lua：局部变量
来源：http://amf.cqqwz.cn

local a = 1
来源：http://xwj.cheryme.top

[T33] Lua：表（数组）
来源：http://ffw.cucudq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tyq.hfpthk.cn

[T34] Lua：遍历表
来源：http://gue.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dui.hammf.cn

[T35] Lua：字典表
来源：http://iyn.tianlin.xyz

local d = { a = 1 };  d.b = 2
来源：http://bci.wangdashe.top

[T36] Lua：函数
来源：http://kqi.guannengcc.top

function add(a, b) return a + b end
来源：http://xms.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://igf.cqqwz.cn

"a" .. "b"
来源：http://pqy.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://cjq.cdnleiting.top

if x > 0 then print("正") end
来源：http://ggw.tianlin.xyz

[T39] Lua：模式匹配
来源：http://uho.ywan-chungtsiang.top

string.find(s, "%d+")
来源：http://teb.yj202588.top

[T40] Lua：元表
来源：http://oma.fengsongda.top

setmetatable({}, { __index = base })
来源：http://xtj.jianghu66.top

[T41] Perl：Hello World
来源：http://gog.yanxiufei.cn

print "Hello\n";
来源：http://fjb.gotoacloud.top

[T42] Perl：变量类型
来源：http://hgg.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vid.yueranfly.top

[T43] Perl：字符串插值
来源：http://apk.jiagoushi.top

"值: $a"
来源：http://jer.cheryme.top

[T44] Perl：条件
来源：http://jzc.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://zly.vqdsnc.cn

[T45] Perl：数组遍历
来源：http://fgw.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://rsh.vqdsnc.cn

[T46] Perl：哈希操作
来源：http://jlm.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hbo.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://tqu.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wgu.ywan-chungtsiang.top

[T48] Perl：正则替换
来源：http://rdw.tanke756.top

$s =~ s/old/new/g;
来源：http://gfz.hywenlv.cn


<!-- 参考信息 -->