代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://qpz.meibo888.top

[R36] 并发执行多个任务
来源：http://nal.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bta.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://cml.kuanghao11.cn

files=$(ls -1)
来源：http://opw.nwbrower.top

[R38] 管道串联
来源：http://tyk.chenzaomai.com

cat a.txt | grep -i error | wc -l
来源：http://gwk.jqgfzy.top

[R39] 重定向标准输出与错误
来源：http://lqv.daria6918.cn

cmd > out.log 2>&1
来源：http://lhu.jianghu66.top

[R40] 追加写日志
来源：http://ayj.cdnleiting.top

echo "log" >> out.log
来源：http://qsr.quarkkingdee.top

[R41] 丢弃输出
来源：http://idk.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://lws.gzhubu.top

[R42] 输入重定向
来源：http://otd.xinyue.icu

wc -l < a.txt
来源：http://bsu.zdqjudy.top

[R43] 按名字查找文件
来源：http://wea.smart0.xyz

find . -name "*.log" -type f
来源：http://gqc.52xcode.cn

[R44] 按修改时间查找
来源：http://iyt.hnxiangtu.top

find . -mtime -7 -type f
来源：http://ksx.yj20258888.top

[R45] 批量删除
来源：http://ktn.chenzaomai.com

find . -name "*.tmp" -delete
来源：http://sky.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://dwf.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cjo.cqqwz.cn

[R47] sed 单行替换
来源：http://bvm.chenzaomai.com

sed -i 's/foo/bar/g' a.txt
来源：http://iwe.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://ytg.smart0.xyz

awk '{print $1, $3}' a.txt
来源：http://mbj.cucudq.cn

[R49] awk 带条件
来源：http://trc.jinqigfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sqa.ivvv.top

[R50] awk 求和
来源：http://nbq.meibo888.top

awk '{s += $2} END {print s}' a.txt
来源：http://mmh.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://qvm.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ygv.hnqzz.top

[R52] 统计行数
来源：http://sxo.yonumen.top

wc -l a.txt
来源：http://vkp.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://zvx.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rsc.yfazqb.com

[R54] 比较两个文件
来源：http://zwu.hysaishi.cn

diff a.txt b.txt
来源：http://lpk.ivvv.top

[R55] 压缩与解压
来源：http://ujh.gotoacloud.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vot.cucudq.cn

[R56] 远程拷贝
来源：http://upb.yuanzhike.top

scp file user@host:/path/
来源：http://fnl.nanxuanxn.top

[R57] 远程执行命令
来源：http://hwl.shanyushiyangtech.top

ssh user@host 'uptime'
来源：http://dvs.fktsv.cn

[R58] 下载文件
来源：http://cvr.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lze.ydjk.org.cn

[R59] 发 POST JSON
来源：http://odo.hnqzz.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xud.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://csa.nanxinkj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wcd.hnxiangtu.top

[R61] 磁盘占用
来源：http://sar.wangshuangyany.cn

df -h;  du -sh *
来源：http://ikf.zhaomingkeji.xyz

[R62] 找最占空间的文件
来源：http://aso.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://xmh.sweek.top

[R63] 内存与进程
来源：http://loc.yuxming.cn

free -h;  ps aux | grep nginx
来源：http://qha.dianchejie.cn

[R64] 结束进程
来源：http://szd.cashguo.top

kill -9 $(pgrep -f app.py)
来源：http://qgg.jlsjyb.cn

[R65] 查看端口占用
来源：http://bkz.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bbj.0kj1m.cn

[R66] 定时任务
来源：http://omg.pycfn.com

crontab -e;  crontab -l
来源：http://phs.yj20258888.top

[R67] 生成随机十六进制串
来源：http://piz.zhoulong.xyz

openssl rand -hex 16
来源：http://bgi.jiagoushi.top

[R68] 计算文件校验值
来源：http://jww.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bti.fzhhl.top

[R69] 生成随机密码
来源：http://feq.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://sqk.quarkkingdee.top

[R70] 时间戳与互转
来源：http://axo.birdmap.top

date +%s;  date -d @1700000000
来源：http://bgx.xinyue.icu

[R71] 日期格式化
来源：http://vle.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://wiu.ivvv.top

[R72] 等待端口就绪
来源：http://qxz.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ail.jqgfzy.top

[R73] 分割大日志
来源：http://toz.haohaochexian.top

split -l 1000 big.log part_
来源：http://dzs.shangyingyoupin.top

[R74] 批量重命名
来源：http://ojd.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://koh.daxiang520.top

[R75] 导出环境变量
来源：http://kat.cheryme.top

export PATH="$HOME/bin:$PATH"
来源：http://fkz.yj20258.top

[R76] 使用临时文件
来源：http://puu.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://swq.chenjidiqi.icu

[R77] 读取用户输入
来源：http://dvw.yueranfly.top

read -rp "请输入: " ans
来源：http://zng.jyoumei.cn

[R78] 交互式菜单
来源：http://avo.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lmx.gzhubu.top

[R79] 解析命令行选项
来源：http://vnn.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pbe.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://cww.sweek.top

time ./run.sh
来源：http://gep.shzxlz.cn

================================================================================
来源：http://tsv.zhixingplan.top

S. C / C++ 专题
来源：http://gmc.yvedp.cn

================================================================================
来源：http://tsj.fktsv.cn

[S01] C：Hello World
来源：http://neu.yanxiufei.cn

#include <stdio.h>
来源：http://bwv.vqdsnc.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jam.jianghu66.top

[S02] C：变量与格式化输出
来源：http://imb.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://hdf.shanyushiyangtech.top

[S03] C：读入整数
来源：http://wso.yuanzhike.top

int x; scanf("%d", &x);
来源：http://yuy.zhixingplan.top

[S04] C：字符串复制
来源：http://ysz.feifeiyinyue.top

char dst[32]; strcpy(dst, "hi");
来源：http://xuq.zdbjq.cn

[S05] C：字符串长度
来源：http://tza.dianchejie.cn

strlen(s)
来源：http://lql.hywenlv.cn

[S06] C：字符串比较
来源：http://qam.jqgufenzy.top

strcmp(a, b) == 0
来源：http://akb.gzhubu.top

[S07] C：数组遍历求和
来源：http://eoi.fengsongda.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://abt.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://him.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ixh.316326.xyz

[S09] C：结构体定义与初始化
来源：http://yey.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kgv.fktsv.cn

[S10] C：指针与解引用
来源：http://ivs.pycfn.com

int *p = &a;  *p = 5;
来源：http://fhp.zycfv.cn

[S11] C：逐行读文件
来源：http://tmk.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://dou.cheryme.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://awd.jinyuanbaomall.cn

fclose(f);
来源：http://hae.zdqjudy.top

[S12] C：写文件
来源：http://hum.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kld.ybcxt.top

[S13] C：宏定义
来源：http://bpo.ctjpmb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tpv.ybcxt.top

[S14] C：枚举
来源：http://yfd.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://cgn.jinqigfzy.top

[S15] C：类型转换
来源：http://uxm.zdqjudy.top

(double) a / b
来源：http://dzk.yuxming.cn

[S16] C：位操作置位
来源：http://xrs.hfpthk.cn

x |= (1 << 3);
来源：http://icc.hywenlv.cn

[S17] C：安全拼接字符串
来源：http://qqp.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gfg.yueranfly.top

[S18] C：命令行参数
来源：http://rni.ywan-chungtsiang.top

int main(int argc, char **argv)
来源：http://vjd.9152youxi.cn

[S19] C：快速排序
来源：http://zjx.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://exw.jinqigufen.top

[S20] C：二分查找
来源：http://kjk.sjlbkw.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://alq.pycfn.com

[S21] C：字符类别判断
来源：http://ixw.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mja.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://pfn.guowangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://ifj.cucudq.cn

[S23] C：随机数
来源：http://cyx.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eof.ybcxt.top

[S24] C：获取本地时间
来源：http://nxc.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fzk.jlsjyb.cn

[S25] C：内存拷贝
来源：http://lfq.zdbjq.cn

memcpy(dst, src, n);
来源：http://epx.gzhubu.top

[S26] C：内存清零
来源：http://xia.fanxiaobao.xyz

memset(a, 0, sizeof a);
来源：http://qrk.zdbjq.cn

[S27] C：定义常量
来源：http://otk.ppjwa.cn

const double PI = 3.14159;
来源：http://bsh.ydjk.org.cn

[S28] C：静态变量
来源：http://oyy.yfazqb.com

static int counter = 0;
来源：http://fyy.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://yni.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kqg.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://exq.ydjk.org.cn

#ifndef X_H
来源：http://vhi.ivvv.top

#define X_H
来源：http://kxq.jlsjyb.cn

#endif
来源：http://pwa.zdbjq.cn

[S31] C++：Hello World
来源：http://cpl.shangyingyoupin.top

#include <iostream>
来源：http://jie.zdqjudy.top

int main() { std::cout << "Hello\n"; }
来源：http://yic.havefunace.top

[S32] C++：字符串
来源：http://huc.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://rnl.gogol.net.cn

[S33] C++：vector 增删
来源：http://vdg.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sfp.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://akc.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://jmh.xuanzx.com

[S35] C++：map
来源：http://ceq.andypj.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hgm.fzhhl.top

[S36] C++：unordered_map
来源：http://kxv.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://crs.jiagoushi.top

[S37] C++：set
来源：http://ppb.ybcxt.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ebh.snrcjt.cn

[S38] C++：排序
来源：http://mko.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://joy.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://nvk.shanyushiyangtech.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ctb.jlsjyb.cn

[S40] C++：查找元素
来源：http://usp.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dpp.uphjek.com

[S41] C++：类与构造函数
来源：http://yra.yfazqb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kgs.vqdsnc.cn

[S42] C++：继承与虚函数
来源：http://xml.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://cfx.epnwcf.com

[S43] C++：智能指针
来源：http://kih.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://krc.tarul.cn

[S44] C++：引用传参
来源：http://egy.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://wcw.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://tnf.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gxm.guowangkeji.top

[S46] C++：函数模板
来源：http://dse.guannengcc.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mja.guannengcc.top

[S47] C++：结构化绑定遍历
来源：http://hvi.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://irm.cdnleiting.top

[S48] C++：逐行读文件
来源：http://rpf.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://qsz.havefunace.top

while (std::getline(in, line)) { }
来源：http://kck.nanxuanxn.top

[S49] C++：写文件
来源：http://kxi.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://asu.cashguo.top

[S50] C++：格式化数字
来源：http://avq.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://abp.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://orj.cqqwz.cn

static_cast<double>(a) / b
来源：http://ilg.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://cwk.ydjk.org.cn

int size() const noexcept { return n_; }
来源：http://dur.xuetiantiany.cn

[S53] C++：移动语义
来源：http://cfw.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://mdq.sweek.top

[S54] C++：异常处理
来源：http://tdv.nanxuanxn.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kmv.havefunace.top

[S55] C++：结构化绑定
来源：http://kge.sufxvd.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://thh.ywan-chungtsiang.top

[S56] C++：optional
来源：http://fsq.dianchejie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yej.snrcjt.cn

[S57] C++：编译期常量
来源：http://scj.nanxuanxn.top

constexpr int N = 10;
来源：http://ass.yonumen.top

[S58] C++：命名空间
来源：http://vam.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://rjb.jiagoushi.top

[S59] C++：静态断言
来源：http://ika.cashguo.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wmn.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://mas.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eug.jinqigfzy.top

================================================================================
来源：http://jjl.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nox.yanxiufei.cn

================================================================================
来源：http://obp.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://vda.wangshuangyany.cn

println("Hello")
来源：http://lwy.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://vvq.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mow.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://mpz.sjlbkw.cn

"值: $b"
来源：http://dhm.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://kip.jyoumei.cn

val n: String? = null;  n?.length
来源：http://ygj.dashuyun.cn

[T05] Kotlin：when 表达式
来源：http://zmu.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hxm.hfpthk.cn

[T06] Kotlin：集合映射
来源：http://riq.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fwq.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://gup.nanxuanxn.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ylq.epnwcf.com

[T08] Kotlin：数据类
来源：http://irq.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://dog.xingfuxueyuan.xyz

[T09] Kotlin：扩展函数
来源：http://auh.ivvv.top

fun String.exclaim() = this + "!"
来源：http://htd.cashguo.top

[T10] Kotlin：默认参数
来源：http://ism.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://noh.shuidangran.top

[T11] Kotlin：协程
来源：http://esf.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xcy.chenlongwang.top

[T12] Kotlin：解构声明
来源：http://eju.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://auj.cashguo.top

[T13] Kotlin：只读 Map
来源：http://haf.aizwys.cn

val m = mapOf("a" to 1)
来源：http://ymn.yuxming.cn

[T14] Kotlin：循环
来源：http://vnj.fehbvm.com

for (i in 1..10) println(i)
来源：http://ibl.0kj1m.cn

[T15] Kotlin：接口
来源：http://hqq.fktsv.cn

interface Shape { fun area(): Double }
来源：http://get.hongshengwenyu.top

[T16] Swift：Hello World
来源：http://ffi.cheryme.top

print("Hello")
来源：http://jeh.zhongyouzk.top

[T17] Swift：变量与常量
来源：http://rpx.0kj1m.cn

var a = 1;  let b = 2
来源：http://yib.wangdashe.top

[T18] Swift：字符串插值
来源：http://ikk.zycfv.cn

"值: \(b)"
来源：http://lhc.chenzaomai.com

[T19] Swift：可选绑定
来源：http://ttd.guannengcc.top

if let n = opt { print(n) }
来源：http://omo.ehwqpu.com

[T20] Swift：数组操作
来源：http://quj.smart0.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://aam.ppjwa.cn

[T21] Swift：遍历
来源：http://dbw.feifeiyinyue.top

for x in a { print(x) }
来源：http://vuv.smart0.xyz

[T22] Swift：字典
来源：http://ffe.pengpengdd.cyou

var d = ["a": 1];  d["b"] = 2
来源：http://sbu.xziqi.cn

[T23] Swift：函数
来源：http://sdg.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bnw.cdnleiting.top

[T24] Swift：闭包
来源：http://pto.feifeiyinyue.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://goq.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://hyv.ctjpmb.com

struct P { var x: Int }
来源：http://klf.zhoulong.xyz

[T26] Swift：类与重写
来源：http://fex.daxiang520.top

class A: Base { override func f() {} }
来源：http://rsq.jinqigufen.top

[T27] Swift：错误处理
来源：http://rsu.guowangkeji.top

do { try f() } catch { print(error) }
来源：http://hyc.svipenyu.cn

[T28] Swift：枚举
来源：http://ofk.kuanghao11.cn

enum Color { case red, green }
来源：http://ykd.daxiang520.top

[T29] Swift：guard 提前返回
来源：http://vny.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://ihg.zhixingplan.top

[T30] Swift：协议
来源：http://sgx.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://qax.shzxlz.cn

[T31] Lua：Hello World
来源：http://rlz.guannengcc.top

print("Hello")
来源：http://qnt.yangfankeji.com

[T32] Lua：局部变量
来源：http://tnn.daria6918.cn

local a = 1
来源：http://kpk.nwbrower.top

[T33] Lua：表（数组）
来源：http://zyz.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nrh.fengsongda.top

[T34] Lua：遍历表
来源：http://vva.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zyx.jinqigufen.top

[T35] Lua：字典表
来源：http://mlq.gotoacloud.top

local d = { a = 1 };  d.b = 2
来源：http://ejx.gotoacloud.top

[T36] Lua：函数
来源：http://oqg.jianghu66.top

function add(a, b) return a + b end
来源：http://dpq.kuanghao11.cn

[T37] Lua：字符串拼接
来源：http://zyp.pengpengdd.cyou

"a" .. "b"
来源：http://ntt.meibo888.top

[T38] Lua：条件
来源：http://eys.guannengcc.top

if x > 0 then print("正") end
来源：http://mrd.ppjwa.cn


<!-- 参考信息 -->