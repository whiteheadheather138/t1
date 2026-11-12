代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://sow.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://sqj.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iok.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://oll.zhoulong.xyz

files=$(ls -1)
来源：http://jhs.0kj1m.cn

[R38] 管道串联
来源：http://dsy.tianlin.xyz

cat a.txt | grep -i error | wc -l
来源：http://ozy.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://dcx.chenzaomai.com

cmd > out.log 2>&1
来源：http://ase.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://ran.jqgfzy.top

echo "log" >> out.log
来源：http://hme.zhixingplan.top

[R41] 丢弃输出
来源：http://ucs.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://jdd.yj202588.top

[R42] 输入重定向
来源：http://kip.zhiwuduotai.top

wc -l < a.txt
来源：http://xmv.havefunace.top

[R43] 按名字查找文件
来源：http://mnj.nanxinkj.top

find . -name "*.log" -type f
来源：http://eez.vehdjk.com

[R44] 按修改时间查找
来源：http://rhi.jqgufenzy.top

find . -mtime -7 -type f
来源：http://swb.tarul.cn

[R45] 批量删除
来源：http://xsm.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://bpf.svipenyu.cn

[R46] 递归替换文件内容
来源：http://qyq.snrcjt.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://btz.cheryme.top

[R47] sed 单行替换
来源：http://huc.yvedp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jdu.meibo888.top

[R48] awk 取指定列
来源：http://ple.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://sbb.zhoulong.xyz

[R49] awk 带条件
来源：http://vzg.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sjs.chenjidiqi.icu

[R50] awk 求和
来源：http://ggi.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lxa.yuanzhike.top

[R51] 排序去重取前几
来源：http://gfw.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ulo.yfazqb.com

[R52] 统计行数
来源：http://qzq.sysykeji.top

wc -l a.txt
来源：http://qao.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://yyl.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vxc.tianlin.xyz

[R54] 比较两个文件
来源：http://soi.fehbvm.com

diff a.txt b.txt
来源：http://ugv.52xcode.cn

[R55] 压缩与解压
来源：http://fqk.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pdj.gaohongyu789.top

[R56] 远程拷贝
来源：http://rhn.xuetiantiany.cn

scp file user@host:/path/
来源：http://tvz.zhixingplan.top

[R57] 远程执行命令
来源：http://mqr.fengsongda.top

ssh user@host 'uptime'
来源：http://xns.guowangkeji.top

[R58] 下载文件
来源：http://paa.pengpengdd.cyou

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ena.vqdsnc.cn

[R59] 发 POST JSON
来源：http://sra.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gvd.zdqjudy.top

[R60] 只看 HTTP 状态码
来源：http://zge.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nwq.uphjek.com

[R61] 磁盘占用
来源：http://wvy.0kj1m.cn

df -h;  du -sh *
来源：http://deq.shuidangran.top

[R62] 找最占空间的文件
来源：http://ovm.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://zot.gaohongyu789.top

[R63] 内存与进程
来源：http://zzc.fengsongda.top

free -h;  ps aux | grep nginx
来源：http://efa.svipenyu.cn

[R64] 结束进程
来源：http://gxg.daxiang520.top

kill -9 $(pgrep -f app.py)
来源：http://xpl.xinyue.icu

[R65] 查看端口占用
来源：http://pfg.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uod.tarul.cn

[R66] 定时任务
来源：http://lzu.cashguo.top

crontab -e;  crontab -l
来源：http://zge.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://rji.hywenlv.cn

openssl rand -hex 16
来源：http://hvy.wangdashe.top

[R68] 计算文件校验值
来源：http://nuq.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://ixm.yangfankeji.com

[R69] 生成随机密码
来源：http://tbj.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://zvg.chenzaomai.com

[R70] 时间戳与互转
来源：http://xqc.yvedp.cn

date +%s;  date -d @1700000000
来源：http://die.52xcode.cn

[R71] 日期格式化
来源：http://xup.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://thi.xinyue.icu

[R72] 等待端口就绪
来源：http://qqg.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://plm.shangyingyoupin.top

[R73] 分割大日志
来源：http://djk.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://iyd.hcnkem.com

[R74] 批量重命名
来源：http://rca.nanxinkj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gdg.ctjpmb.com

[R75] 导出环境变量
来源：http://tcy.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://osg.nanxinkj.top

[R76] 使用临时文件
来源：http://zdb.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qpw.pengpengdd.cyou

[R77] 读取用户输入
来源：http://thc.cdnleiting.top

read -rp "请输入: " ans
来源：http://xzp.jinghuilouyu.cn

[R78] 交互式菜单
来源：http://vtw.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kdz.sjlbkw.cn

[R79] 解析命令行选项
来源：http://arq.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jio.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://jse.c1oappe.top

time ./run.sh
来源：http://gnw.meibo888.top

================================================================================
来源：http://sox.yongpay.top

S. C / C++ 专题
来源：http://jfr.yvedp.cn

================================================================================
来源：http://weo.chenjidiqi.icu

[S01] C：Hello World
来源：http://cti.hesvh.cn

#include <stdio.h>
来源：http://nzn.hnxiangtu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://oyy.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://qdd.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://hnz.yueranfly.top

[S03] C：读入整数
来源：http://aou.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://nff.cheryme.top

[S04] C：字符串复制
来源：http://cby.hywenlv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hdz.jiagoushi.top

[S05] C：字符串长度
来源：http://obc.0kj1m.cn

strlen(s)
来源：http://yht.gaohongyu789.top

[S06] C：字符串比较
来源：http://zce.ppjwa.cn

strcmp(a, b) == 0
来源：http://dax.9152youxi.cn

[S07] C：数组遍历求和
来源：http://rve.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://don.jyoumei.cn

[S08] C：动态内存分配与释放
来源：http://hxu.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qfr.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://xob.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mtp.andypj.xyz

[S10] C：指针与解引用
来源：http://kri.dashuyun.cn

int *p = &a;  *p = 5;
来源：http://mqu.nwbrower.top

[S11] C：逐行读文件
来源：http://ulr.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://lms.zycfv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ooy.zycfv.cn

fclose(f);
来源：http://cir.hfpthk.cn

[S12] C：写文件
来源：http://nnk.redwolf501.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://epv.gogol.net.cn

[S13] C：宏定义
来源：http://voe.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xnt.yanxiufei.cn

[S14] C：枚举
来源：http://kcg.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://unf.hnxiangtu.top

[S15] C：类型转换
来源：http://fnp.chenjidiqi.icu

(double) a / b
来源：http://mia.ivvv.top

[S16] C：位操作置位
来源：http://bsq.0kj1m.cn

x |= (1 << 3);
来源：http://cqz.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://sqk.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://isn.epnwcf.com

[S18] C：命令行参数
来源：http://hww.fzhhl.top

int main(int argc, char **argv)
来源：http://wcj.zhoulong.xyz

[S19] C：快速排序
来源：http://uyi.jlsjyb.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fjh.tarul.cn

[S20] C：二分查找
来源：http://ahh.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ucy.fktsv.cn

[S21] C：字符类别判断
来源：http://duw.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yzl.cdnleiting.top

[S22] C：字符串转数字
来源：http://khi.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://thn.zhaomingkeji.xyz

[S23] C：随机数
来源：http://ryk.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mqk.kuanghao11.cn

[S24] C：获取本地时间
来源：http://zcs.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ymt.yj20258888.top

[S25] C：内存拷贝
来源：http://tkp.hongshengwenyu.top

memcpy(dst, src, n);
来源：http://xex.zhoulong.xyz

[S26] C：内存清零
来源：http://lwm.daria6918.cn

memset(a, 0, sizeof a);
来源：http://elp.kuanghao11.cn

[S27] C：定义常量
来源：http://yvu.tianlin.xyz

const double PI = 3.14159;
来源：http://vke.gzhubu.top

[S28] C：静态变量
来源：http://tge.ywan-chungtsiang.top

static int counter = 0;
来源：http://ico.yangfankeji.com

[S29] C：变参函数
来源：http://jve.zycfv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xeo.zhiwuduotai.top

[S30] C：头文件保护
来源：http://vas.dashuyun.cn

#ifndef X_H
来源：http://dub.nanxinkj.top

#define X_H
来源：http://dmj.shangyingyoupin.top

#endif
来源：http://wfk.tarul.cn

[S31] C++：Hello World
来源：http://gkx.jinqigufen.top

#include <iostream>
来源：http://mui.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://qio.tarul.cn

[S32] C++：字符串
来源：http://obz.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://rkr.fehbvm.com

[S33] C++：vector 增删
来源：http://wkb.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cyn.xziqi.cn

[S34] C++：遍历 vector
来源：http://frg.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://vse.dianchejie.cn

[S35] C++：map
来源：http://ygt.yonumen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hda.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://obo.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zyc.cashguo.top

[S37] C++：set
来源：http://cmk.xinyue.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lim.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://cqk.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://otm.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://pjf.jqgufenzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xog.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://yxw.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lqx.smart0.xyz

[S41] C++：类与构造函数
来源：http://acd.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://per.dashuyun.cn

[S42] C++：继承与虚函数
来源：http://tbo.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://ylr.pycfn.com

[S43] C++：智能指针
来源：http://rtq.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://pzk.jqgfzy.top

[S44] C++：引用传参
来源：http://rar.tarul.cn

void inc(int &x) { ++x; }
来源：http://ftb.tianlin.xyz

[S45] C++：lambda
来源：http://zef.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://qiu.jlsjyb.cn

[S46] C++：函数模板
来源：http://ssr.dianchejie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mpg.dianchejie.cn

[S47] C++：结构化绑定遍历
来源：http://fqc.zdqjudy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ydk.tanke756.top

[S48] C++：逐行读文件
来源：http://elo.xylfe.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pzb.daria6918.cn

while (std::getline(in, line)) { }
来源：http://cds.hongshengwenyu.top

[S49] C++：写文件
来源：http://zbk.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iob.jqgufenzy.top

[S50] C++：格式化数字
来源：http://dyj.yanxiufei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sfp.dianchejie.cn

[S51] C++：显式类型转换
来源：http://igt.yonumen.top

static_cast<double>(a) / b
来源：http://gfa.quarkkingdee.top

[S52] C++：const 与 noexcept
来源：http://akk.hcnkem.com

int size() const noexcept { return n_; }
来源：http://grz.shzxlz.cn

[S53] C++：移动语义
来源：http://khh.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://vwp.hfpthk.cn

[S54] C++：异常处理
来源：http://ojk.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hlg.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://iec.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://psu.jinghuilouyu.cn

[S56] C++：optional
来源：http://sya.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kkm.ppjwa.cn

[S57] C++：编译期常量
来源：http://dlj.tanke756.top

constexpr int N = 10;
来源：http://mmb.chenjidiqi.icu

[S58] C++：命名空间
来源：http://aui.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://gwy.quarkkingdee.top

[S59] C++：静态断言
来源：http://qrs.shzxlz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zbu.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://wtv.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sty.xingfuxueyuan.xyz

================================================================================
来源：http://mxy.daria6918.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wug.tian-w.cn

================================================================================
来源：http://qzy.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://vsg.52xcode.cn

println("Hello")
来源：http://tec.yj20258.top

[T02] Kotlin：变量
来源：http://lym.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://exd.yanxiufei.cn

[T03] Kotlin：字符串模板
来源：http://iyj.fktsv.cn

"值: $b"
来源：http://ehx.meibo888.top

[T04] Kotlin：空安全
来源：http://kys.nanxinkj.top

val n: String? = null;  n?.length
来源：http://yen.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://flm.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jii.haohaochexian.top

[T06] Kotlin：集合映射
来源：http://tga.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://xqc.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://nzx.jlsjyb.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tix.xinyue.icu

[T08] Kotlin：数据类
来源：http://emm.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://gaw.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://nfp.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://lvl.ybcxt.top

[T10] Kotlin：默认参数
来源：http://axe.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ugw.zdbjq.cn

[T11] Kotlin：协程
来源：http://hzp.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ryr.bbcook.cn

[T12] Kotlin：解构声明
来源：http://fjd.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://flc.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://acv.jinqigufen.top

val m = mapOf("a" to 1)
来源：http://zng.yj20258.top

[T14] Kotlin：循环
来源：http://jwj.xuanzx.com

for (i in 1..10) println(i)
来源：http://fqd.pycfn.com

[T15] Kotlin：接口
来源：http://djd.cashguo.top

interface Shape { fun area(): Double }
来源：http://cso.smart0.xyz

[T16] Swift：Hello World
来源：http://vwv.vehdjk.com

print("Hello")
来源：http://twt.zhongyouzk.top

[T17] Swift：变量与常量
来源：http://uya.aibaodan.cn

var a = 1;  let b = 2
来源：http://lje.hcnkem.com

[T18] Swift：字符串插值
来源：http://qzh.wangshuangyany.cn

"值: \(b)"
来源：http://dtm.nwbrower.top

[T19] Swift：可选绑定
来源：http://lfd.xuanzx.com

if let n = opt { print(n) }
来源：http://adf.kuanghao11.cn

[T20] Swift：数组操作
来源：http://jlr.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://skw.hnqzz.top

[T21] Swift：遍历
来源：http://afz.bjfxy.top

for x in a { print(x) }
来源：http://aei.ybcxt.top

[T22] Swift：字典
来源：http://mwb.gogol.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vgj.jqgufenzy.top

[T23] Swift：函数
来源：http://ibm.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cuv.dashuyun.cn

[T24] Swift：闭包
来源：http://onj.fehbvm.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://nqs.daria6918.cn

[T25] Swift：结构体
来源：http://osc.yvedp.cn

struct P { var x: Int }
来源：http://dig.sjlbkw.cn

[T26] Swift：类与重写
来源：http://xei.xinyue.icu

class A: Base { override func f() {} }
来源：http://qod.jinyuanbaomall.cn

[T27] Swift：错误处理
来源：http://rve.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://qxd.nanxinkj.top

[T28] Swift：枚举
来源：http://kuq.316326.xyz

enum Color { case red, green }
来源：http://fwz.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://mqf.zhiwuduotai.top

guard let x = opt else { return }
来源：http://ybq.daria6918.cn

[T30] Swift：协议
来源：http://cjx.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://ide.jqgfzy.top

[T31] Lua：Hello World
来源：http://doa.shangyingyoupin.top

print("Hello")
来源：http://xbc.hnxiangtu.top

[T32] Lua：局部变量
来源：http://gal.zhengqikj.top

local a = 1
来源：http://ncg.bbcook.cn

[T33] Lua：表（数组）
来源：http://inj.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gjc.shzxlz.cn

[T34] Lua：遍历表
来源：http://kil.vehdjk.com

for i, v in ipairs(t) do print(i, v) end
来源：http://jkz.yuanzhike.top

[T35] Lua：字典表
来源：http://uol.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://ckt.hcnkem.com

[T36] Lua：函数
来源：http://sns.jyoumei.cn

function add(a, b) return a + b end
来源：http://qnr.uphjek.com

[T37] Lua：字符串拼接
来源：http://ota.tian-w.cn

"a" .. "b"
来源：http://hbj.hesvh.cn

[T38] Lua：条件
来源：http://cum.zhoulong.xyz

if x > 0 then print("正") end
来源：http://gcg.yuxming.cn


<!-- 参考信息 -->