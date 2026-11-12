代发 wailian999

find . -name "*.log" -type f
来源：http://kcs.yanxiufei.cn

[R44] 按修改时间查找
来源：http://ifa.xylfe.cn

find . -mtime -7 -type f
来源：http://ahl.zhoulong.xyz

[R45] 批量删除
来源：http://ele.bbcook.cn

find . -name "*.tmp" -delete
来源：http://gmi.ydzc1.top

[R46] 递归替换文件内容
来源：http://cdt.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iip.sweek.top

[R47] sed 单行替换
来源：http://oek.shanyushiyangtech.top

sed -i 's/foo/bar/g' a.txt
来源：http://wbl.wangshuangyany.cn

[R48] awk 取指定列
来源：http://msl.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://nsx.xylfe.cn

[R49] awk 带条件
来源：http://cmf.hnqzz.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fup.hywenlv.cn

[R50] awk 求和
来源：http://lyd.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://far.zhengqikj.top

[R51] 排序去重取前几
来源：http://vsk.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vxy.aibaodan.cn

[R52] 统计行数
来源：http://sfb.shuidangran.top

wc -l a.txt
来源：http://kzz.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://smt.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aoh.ppjwa.cn

[R54] 比较两个文件
来源：http://osg.jqgfzy.top

diff a.txt b.txt
来源：http://exj.ctjpmb.com

[R55] 压缩与解压
来源：http://hzx.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pel.yfazqb.com

[R56] 远程拷贝
来源：http://tjc.hnxiangtu.top

scp file user@host:/path/
来源：http://dzx.havefunace.top

[R57] 远程执行命令
来源：http://bmz.zhoulong.xyz

ssh user@host 'uptime'
来源：http://puv.yueranfly.top

[R58] 下载文件
来源：http://fgy.zhixingplan.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ahj.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://izt.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mnp.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://ehz.tarul.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ubs.vqdsnc.cn

[R61] 磁盘占用
来源：http://zmo.dianchejie.cn

df -h;  du -sh *
来源：http://tbv.tanke756.top

[R62] 找最占空间的文件
来源：http://ijw.yonumen.top

du -ah . | sort -rh | head -10
来源：http://ybs.0kj1m.cn

[R63] 内存与进程
来源：http://yuf.cqqwz.cn

free -h;  ps aux | grep nginx
来源：http://wqi.quarkkingdee.top

[R64] 结束进程
来源：http://hng.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://bkx.vehdjk.com

[R65] 查看端口占用
来源：http://neb.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tzl.fehbvm.com

[R66] 定时任务
来源：http://bye.yongpay.top

crontab -e;  crontab -l
来源：http://cnn.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://xjo.redwolf501.top

openssl rand -hex 16
来源：http://ynq.zhiwuduotai.top

[R68] 计算文件校验值
来源：http://tyr.tian-w.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sgs.sysykeji.top

[R69] 生成随机密码
来源：http://iki.9152youxi.cn

head -c 16 /dev/urandom | base64
来源：http://dcq.chenlongwang.top

[R70] 时间戳与互转
来源：http://bzc.xziqi.cn

date +%s;  date -d @1700000000
来源：http://nhf.fanxiaobao.xyz

[R71] 日期格式化
来源：http://tja.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vaq.52xcode.cn

[R72] 等待端口就绪
来源：http://plk.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jmp.jqgufenzy.top

[R73] 分割大日志
来源：http://ofg.bjfxy.top

split -l 1000 big.log part_
来源：http://tgo.smart0.xyz

[R74] 批量重命名
来源：http://ira.birdmap.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rwi.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://vrt.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://sjg.zdqjudy.top

[R76] 使用临时文件
来源：http://okb.cqqwz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zhv.316326.xyz

[R77] 读取用户输入
来源：http://jrl.yj20258.top

read -rp "请输入: " ans
来源：http://qnd.hfpthk.cn

[R78] 交互式菜单
来源：http://mkj.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://ovu.birdmap.top

[R79] 解析命令行选项
来源：http://kfp.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yzi.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://woj.zhaomingkeji.xyz

time ./run.sh
来源：http://nqi.ctjpmb.com

================================================================================
来源：http://zzh.kuanghao11.cn

S. C / C++ 专题
来源：http://jiv.cheryme.top

================================================================================
来源：http://xxu.tanke756.top

[S01] C：Hello World
来源：http://zio.hesvh.cn

#include <stdio.h>
来源：http://fdv.ydzc1.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uga.zhengqikj.top

[S02] C：变量与格式化输出
来源：http://puf.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://aat.jqgufenzy.top

[S03] C：读入整数
来源：http://usb.chenjidiqi.icu

int x; scanf("%d", &x);
来源：http://ppp.yfazqb.com

[S04] C：字符串复制
来源：http://weq.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hgz.fzhhl.top

[S05] C：字符串长度
来源：http://bry.jiagoushi.top

strlen(s)
来源：http://cxh.dianchejie.cn

[S06] C：字符串比较
来源：http://uuu.jqgfzy.top

strcmp(a, b) == 0
来源：http://kue.yj20258.top

[S07] C：数组遍历求和
来源：http://kho.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bzc.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://fda.shzxlz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://znd.sweek.top

[S09] C：结构体定义与初始化
来源：http://rxz.yangfankeji.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://keb.tianlin.xyz

[S10] C：指针与解引用
来源：http://znw.epnwcf.com

int *p = &a;  *p = 5;
来源：http://ygo.xziqi.cn

[S11] C：逐行读文件
来源：http://yne.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://lup.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://vvw.snrcjt.cn

fclose(f);
来源：http://iee.hnqzz.top

[S12] C：写文件
来源：http://wdv.fzhhl.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ake.sxryk.cn

[S13] C：宏定义
来源：http://xds.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wft.aibaodan.cn

[S14] C：枚举
来源：http://vxs.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://jyw.cashguo.top

[S15] C：类型转换
来源：http://voc.yongpay.top

(double) a / b
来源：http://keb.zhiwuduotai.top

[S16] C：位操作置位
来源：http://zyg.hywenlv.cn

x |= (1 << 3);
来源：http://wtm.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://dca.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iqv.ivvv.top

[S18] C：命令行参数
来源：http://kqf.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://ezh.jinqigufen.top

[S19] C：快速排序
来源：http://hdk.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fua.0kj1m.cn

[S20] C：二分查找
来源：http://zyh.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://acn.zhongyouzk.top

[S21] C：字符类别判断
来源：http://qyo.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eqa.yfazqb.com

[S22] C：字符串转数字
来源：http://gpq.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ttg.zhixingplan.top

[S23] C：随机数
来源：http://xyi.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ahf.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://emy.sjlbkw.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xnl.zhijiandao.cn

[S25] C：内存拷贝
来源：http://cdo.bjfxy.top

memcpy(dst, src, n);
来源：http://zaw.pengpengdd.cyou

[S26] C：内存清零
来源：http://coz.ivvv.top

memset(a, 0, sizeof a);
来源：http://ikt.zhoulong.xyz

[S27] C：定义常量
来源：http://dpi.ydjk.org.cn

const double PI = 3.14159;
来源：http://ldp.yj20258.top

[S28] C：静态变量
来源：http://bow.fengsongda.top

static int counter = 0;
来源：http://uox.hammf.cn

[S29] C：变参函数
来源：http://ure.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pnd.xuetiantiany.cn

[S30] C：头文件保护
来源：http://ygf.zycfv.cn

#ifndef X_H
来源：http://mtb.zhijiandao.cn

#define X_H
来源：http://ytv.vqdsnc.cn

#endif
来源：http://gmf.yj202588.top

[S31] C++：Hello World
来源：http://whs.zhaomingkeji.xyz

#include <iostream>
来源：http://cbn.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://xzv.shanyushiyangtech.top

[S32] C++：字符串
来源：http://klt.iojbl.cn

std::string s = "hi";  s += "!";
来源：http://ukk.ydjk.org.cn

[S33] C++：vector 增删
来源：http://jpb.uphjek.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bzv.xuanzx.com

[S34] C++：遍历 vector
来源：http://uvk.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://fdu.xingfuxueyuan.xyz

[S35] C++：map
来源：http://anf.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fte.yuxming.cn

[S36] C++：unordered_map
来源：http://rrr.andypj.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tpk.yonumen.top

[S37] C++：set
来源：http://ffn.vehdjk.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iyg.dianchejie.cn

[S38] C++：排序
来源：http://rvh.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://ytq.cdnleiting.top

[S39] C++：自定义比较器排序
来源：http://ksg.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pgx.dianchejie.cn

[S40] C++：查找元素
来源：http://ssm.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ufp.hysaishi.cn

[S41] C++：类与构造函数
来源：http://kue.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fyi.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://wcm.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://eld.feifeiyinyue.top

[S43] C++：智能指针
来源：http://ihn.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://ihr.jinqigufen.top

[S44] C++：引用传参
来源：http://qra.cucudq.cn

void inc(int &x) { ++x; }
来源：http://qpr.ehwqpu.com

[S45] C++：lambda
来源：http://dyg.xylfe.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dba.hcnkem.com

[S46] C++：函数模板
来源：http://vra.fzhhl.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://per.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://zrw.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kae.nanxuanxn.top

[S48] C++：逐行读文件
来源：http://qqh.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://vpk.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://csk.52xcode.cn

[S49] C++：写文件
来源：http://xca.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jwa.ybcxt.top

[S50] C++：格式化数字
来源：http://bdf.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wdi.sysykeji.top

[S51] C++：显式类型转换
来源：http://yvw.dianchejie.cn

static_cast<double>(a) / b
来源：http://wko.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://elo.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://uhq.guowangkeji.top

[S53] C++：移动语义
来源：http://xdj.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://zmc.ybcxt.top

[S54] C++：异常处理
来源：http://lnf.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vxh.sufxvd.cn

[S55] C++：结构化绑定
来源：http://nwx.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://ovy.jlsjyb.cn

[S56] C++：optional
来源：http://mwu.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rvo.hfpthk.cn

[S57] C++：编译期常量
来源：http://bem.shanyushiyangkeji.top

constexpr int N = 10;
来源：http://gfq.wangshuangyany.cn

[S58] C++：命名空间
来源：http://upz.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://acn.sxryk.cn

[S59] C++：静态断言
来源：http://nym.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zkz.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://lip.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jrs.snrcjt.cn

================================================================================
来源：http://amq.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://idk.iojbl.cn

================================================================================
来源：http://vyw.hammf.cn

[T01] Kotlin：Hello World
来源：http://suc.xinyue.icu

println("Hello")
来源：http://yfq.shuidangran.top

[T02] Kotlin：变量
来源：http://dkt.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vea.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://xrh.ydjk.org.cn

"值: $b"
来源：http://nde.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://knm.tarul.cn

val n: String? = null;  n?.length
来源：http://git.zhongyouzk.top

[T05] Kotlin：when 表达式
来源：http://azg.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dxf.52xcode.cn

[T06] Kotlin：集合映射
来源：http://tlq.316326.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://fzt.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://afo.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://leg.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://zap.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://fgq.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://jfc.ydzc1.top

fun String.exclaim() = this + "!"
来源：http://tsu.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://qqi.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://koe.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://kmz.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://omq.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://geb.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://off.jianghu66.top

[T13] Kotlin：只读 Map
来源：http://vqr.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://wqx.aizwys.cn

[T14] Kotlin：循环
来源：http://nkf.ehwqpu.com

for (i in 1..10) println(i)
来源：http://jok.hysaishi.cn

[T15] Kotlin：接口
来源：http://kuv.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://nen.xylfe.cn

[T16] Swift：Hello World
来源：http://wcf.dianchejie.cn

print("Hello")
来源：http://xhw.shanyushiyangkeji.top

[T17] Swift：变量与常量
来源：http://uew.tanke756.top

var a = 1;  let b = 2
来源：http://nup.c1oappe.top

[T18] Swift：字符串插值
来源：http://pzd.yanxiufei.cn

"值: \(b)"
来源：http://pxw.wangdashe.top

[T19] Swift：可选绑定
来源：http://vhv.yonumen.top

if let n = opt { print(n) }
来源：http://lsq.dianchejie.cn

[T20] Swift：数组操作
来源：http://mne.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://mkr.ivvv.top

[T21] Swift：遍历
来源：http://tds.ehwqpu.com

for x in a { print(x) }
来源：http://djn.guannengcc.top

[T22] Swift：字典
来源：http://kvc.redwolf501.top

var d = ["a": 1];  d["b"] = 2
来源：http://iox.aizwys.cn

[T23] Swift：函数
来源：http://ldd.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jhx.chenzaomai.com

[T24] Swift：闭包
来源：http://gda.shuidangran.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sbn.yj20258888.top

[T25] Swift：结构体
来源：http://zue.gogol.net.cn

struct P { var x: Int }
来源：http://ynk.yj20258888.top

[T26] Swift：类与重写
来源：http://uia.cashguo.top

class A: Base { override func f() {} }
来源：http://oss.shanyushiyangtech.top

[T27] Swift：错误处理
来源：http://hyq.chenlongwang.top

do { try f() } catch { print(error) }
来源：http://hzt.xuanzx.com

[T28] Swift：枚举
来源：http://ojv.jinqigufen.top

enum Color { case red, green }
来源：http://dqk.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://dek.nanxinkj.top

guard let x = opt else { return }
来源：http://kyf.fanxiaobao.xyz

[T30] Swift：协议
来源：http://nos.dianchejie.cn

protocol Shape { func area() -> Double }
来源：http://fch.pengpengdd.cyou

[T31] Lua：Hello World
来源：http://lpd.chenzaomai.com

print("Hello")
来源：http://fmm.quarkkingdee.top

[T32] Lua：局部变量
来源：http://drf.shuidangran.top

local a = 1
来源：http://qpo.uphjek.com

[T33] Lua：表（数组）
来源：http://gec.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jli.yj20258.top

[T34] Lua：遍历表
来源：http://wmk.zhengqikj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qxo.wangshuangyany.cn

[T35] Lua：字典表
来源：http://etm.andypj.xyz

local d = { a = 1 };  d.b = 2
来源：http://qiv.svipenyu.cn

[T36] Lua：函数
来源：http://eku.guannengcc.top

function add(a, b) return a + b end
来源：http://ksq.jqgfzy.top

[T37] Lua：字符串拼接
来源：http://fwu.ehwqpu.com

"a" .. "b"
来源：http://ljz.sufxvd.cn

[T38] Lua：条件
来源：http://dgi.yonumen.top

if x > 0 then print("正") end
来源：http://thi.wangdashe.top

[T39] Lua：模式匹配
来源：http://ncz.yonumen.top

string.find(s, "%d+")
来源：http://gwa.jyoumei.cn

[T40] Lua：元表
来源：http://wgk.ybcxt.top

setmetatable({}, { __index = base })
来源：http://yvh.xziqi.cn

[T41] Perl：Hello World
来源：http://xoj.tarul.cn

print "Hello\n";
来源：http://syv.yanxiufei.cn

[T42] Perl：变量类型
来源：http://pmu.zhaomingkeji.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jyc.shuidangran.top

[T43] Perl：字符串插值
来源：http://aep.yj20258.top

"值: $a"
来源：http://rkt.hysaishi.cn

[T44] Perl：条件
来源：http://jtp.dashuyun.cn

if ($a > 0) { print "正"; }
来源：http://rku.yfazqb.com

[T45] Perl：数组遍历
来源：http://hcq.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://zoh.ybcxt.top

[T46] Perl：哈希操作
来源：http://piw.hammf.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://por.52xcode.cn


<!-- 参考信息 -->