代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pgi.gogol.net.cn

[R34] 退出时清理
来源：http://xsu.jinqigufen.top

trap 'rm -f "$tmp"' EXIT
来源：http://fqy.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://tae.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jpr.xuanzx.com

[R36] 并发执行多个任务
来源：http://nbh.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://czb.316326.xyz

[R37] 把输出赋给变量
来源：http://ays.yvedp.cn

files=$(ls -1)
来源：http://mue.ivvv.top

[R38] 管道串联
来源：http://xsa.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://dqk.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://uzz.snrcjt.cn

cmd > out.log 2>&1
来源：http://qib.chenzaomai.com

[R40] 追加写日志
来源：http://dgp.hysaishi.cn

echo "log" >> out.log
来源：http://hxo.hongshengwenyu.top

[R41] 丢弃输出
来源：http://htx.hcnkem.com

cmd >/dev/null 2>&1
来源：http://qys.jqgfzy.top

[R42] 输入重定向
来源：http://kvv.ivvv.top

wc -l < a.txt
来源：http://hto.xuetiantiany.cn

[R43] 按名字查找文件
来源：http://ngs.gzhubu.top

find . -name "*.log" -type f
来源：http://ojt.haohaochexian.top

[R44] 按修改时间查找
来源：http://msb.tanke756.top

find . -mtime -7 -type f
来源：http://qvc.tarul.cn

[R45] 批量删除
来源：http://mst.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://qus.smart0.xyz

[R46] 递归替换文件内容
来源：http://kde.yuxming.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://brz.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://itz.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tre.shzxlz.cn

[R48] awk 取指定列
来源：http://tcq.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://oqn.mhx1999.top

[R49] awk 带条件
来源：http://lbt.sxryk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sfb.sjlbkw.cn

[R50] awk 求和
来源：http://klw.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://zvo.cdnleiting.top

[R51] 排序去重取前几
来源：http://rnx.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://klq.yj20258888.top

[R52] 统计行数
来源：http://smv.chenzaomai.com

wc -l a.txt
来源：http://fzk.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://fqi.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ujk.bjfxy.top

[R54] 比较两个文件
来源：http://dyj.jinghuilouyu.cn

diff a.txt b.txt
来源：http://mou.ctjpmb.com

[R55] 压缩与解压
来源：http://kwu.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qne.fzhhl.top

[R56] 远程拷贝
来源：http://itv.xylfe.cn

scp file user@host:/path/
来源：http://gyr.ydzc1.top

[R57] 远程执行命令
来源：http://ixx.chenlongwang.top

ssh user@host 'uptime'
来源：http://tgv.sysykeji.top

[R58] 下载文件
来源：http://zha.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ytp.gaohongyu789.top

[R59] 发 POST JSON
来源：http://ccv.fengsongda.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xxb.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://tsg.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mik.sysykeji.top

[R61] 磁盘占用
来源：http://yxf.pycfn.com

df -h;  du -sh *
来源：http://wtd.xinyue.icu

[R62] 找最占空间的文件
来源：http://zab.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://vqm.tian-w.cn

[R63] 内存与进程
来源：http://rnz.jinqigfzy.top

free -h;  ps aux | grep nginx
来源：http://toe.ivvv.top

[R64] 结束进程
来源：http://qwi.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://sna.redwolf501.top

[R65] 查看端口占用
来源：http://kqq.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sgo.cucudq.cn

[R66] 定时任务
来源：http://rsq.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://hqp.xinyue.icu

[R67] 生成随机十六进制串
来源：http://dwv.ydjk.org.cn

openssl rand -hex 16
来源：http://ugk.ydjk.org.cn

[R68] 计算文件校验值
来源：http://tsu.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wgn.yanxiufei.cn

[R69] 生成随机密码
来源：http://xks.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://ald.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://sba.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://hdm.snrcjt.cn

[R71] 日期格式化
来源：http://dee.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ric.cucudq.cn

[R72] 等待端口就绪
来源：http://flj.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jvc.hnqzz.top

[R73] 分割大日志
来源：http://dac.ybcxt.top

split -l 1000 big.log part_
来源：http://ezh.0kj1m.cn

[R74] 批量重命名
来源：http://kxz.shuidangran.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://akl.birdmap.top

[R75] 导出环境变量
来源：http://ths.yuanzhike.top

export PATH="$HOME/bin:$PATH"
来源：http://rqc.hfpthk.cn

[R76] 使用临时文件
来源：http://zgp.zhengqikj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://esz.jqgufenzy.top

[R77] 读取用户输入
来源：http://rvt.ppjwa.cn

read -rp "请输入: " ans
来源：http://fyv.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://icb.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rnx.nanxinkj.top

[R79] 解析命令行选项
来源：http://bla.zhixingplan.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bfi.xinyue.icu

[R80] 查看脚本执行耗时
来源：http://uai.pengpengdd.cyou

time ./run.sh
来源：http://zpe.c1oappe.top

================================================================================
来源：http://nsp.nanxuanxn.top

S. C / C++ 专题
来源：http://uhc.zhaomingkeji.xyz

================================================================================
来源：http://xma.dashuyun.cn

[S01] C：Hello World
来源：http://pne.aizwys.cn

#include <stdio.h>
来源：http://ise.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ose.c1oappe.top

[S02] C：变量与格式化输出
来源：http://mxx.daria6918.cn

int a = 10; printf("%d\n", a);
来源：http://svq.hcnkem.com

[S03] C：读入整数
来源：http://aqp.zycfv.cn

int x; scanf("%d", &x);
来源：http://fcf.dianchejie.cn

[S04] C：字符串复制
来源：http://smu.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://bdu.pycfn.com

[S05] C：字符串长度
来源：http://whi.jinghuilouyu.cn

strlen(s)
来源：http://ikt.andypj.xyz

[S06] C：字符串比较
来源：http://sgp.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://hbh.yvedp.cn

[S07] C：数组遍历求和
来源：http://rri.shuidangran.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pty.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://rns.hongshengwenyu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://phu.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://whm.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tuy.jinqigfzy.top

[S10] C：指针与解引用
来源：http://brq.zycfv.cn

int *p = &a;  *p = 5;
来源：http://wvt.nanxinkj.top

[S11] C：逐行读文件
来源：http://fjf.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://uyd.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lsu.jinyuanbaomall.cn

fclose(f);
来源：http://cye.yueranfly.top

[S12] C：写文件
来源：http://viu.dianchejie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yrl.yonumen.top

[S13] C：宏定义
来源：http://mdg.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vmo.birdmap.top

[S14] C：枚举
来源：http://txu.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://ltl.wangshuangyany.cn

[S15] C：类型转换
来源：http://bzb.yongpay.top

(double) a / b
来源：http://qhq.chenjidiqi.icu

[S16] C：位操作置位
来源：http://yjk.zhaomingkeji.xyz

x |= (1 << 3);
来源：http://leo.dianchejie.cn

[S17] C：安全拼接字符串
来源：http://jda.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jqq.hnqzz.top

[S18] C：命令行参数
来源：http://qsa.bjfxy.top

int main(int argc, char **argv)
来源：http://riq.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://yqw.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://pry.zhijiandao.cn

[S20] C：二分查找
来源：http://uef.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://glg.snrcjt.cn

[S21] C：字符类别判断
来源：http://zrv.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lct.vehdjk.com

[S22] C：字符串转数字
来源：http://fub.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://obh.haohaochexian.top

[S23] C：随机数
来源：http://yzl.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xhq.aibaodan.cn

[S24] C：获取本地时间
来源：http://uhd.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yvu.kuanghao11.cn

[S25] C：内存拷贝
来源：http://plx.c1oappe.top

memcpy(dst, src, n);
来源：http://nks.sweek.top

[S26] C：内存清零
来源：http://dqd.cheryme.top

memset(a, 0, sizeof a);
来源：http://dug.chenzaomai.com

[S27] C：定义常量
来源：http://plz.yuanzhike.top

const double PI = 3.14159;
来源：http://ikf.gzhubu.top

[S28] C：静态变量
来源：http://xvh.guowangkeji.top

static int counter = 0;
来源：http://vui.ydjk.org.cn

[S29] C：变参函数
来源：http://uzm.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cmh.zdbjq.cn

[S30] C：头文件保护
来源：http://grf.yangfankeji.com

#ifndef X_H
来源：http://xzi.yonumen.top

#define X_H
来源：http://rlj.tianlin.xyz

#endif
来源：http://dva.uphjek.com

[S31] C++：Hello World
来源：http://gaq.9152youxi.cn

#include <iostream>
来源：http://idb.yfazqb.com

int main() { std::cout << "Hello\n"; }
来源：http://dnp.cashguo.top

[S32] C++：字符串
来源：http://nzv.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://mfx.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://vjn.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nse.bjfxy.top

[S34] C++：遍历 vector
来源：http://jxi.ybcxt.top

for (auto &x : v) { std::cout << x; }
来源：http://fof.xingfuxueyuan.xyz

[S35] C++：map
来源：http://mec.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ajk.fzhhl.top

[S36] C++：unordered_map
来源：http://ycu.hnxiangtu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tvf.xziqi.cn

[S37] C++：set
来源：http://tkf.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xwy.snrcjt.cn

[S38] C++：排序
来源：http://uim.xuanzx.com

std::sort(v.begin(), v.end());
来源：http://rhu.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://flj.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ntk.haohaochexian.top

[S40] C++：查找元素
来源：http://mav.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://epk.zhixingplan.top

[S41] C++：类与构造函数
来源：http://tfp.hnqzz.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pjl.hesvh.cn

[S42] C++：继承与虚函数
来源：http://xsp.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://ynq.sxryk.cn

[S43] C++：智能指针
来源：http://iaw.c1oappe.top

auto p = std::make_unique<int>(5);
来源：http://zqa.sysykeji.top

[S44] C++：引用传参
来源：http://tjj.fzhhl.top

void inc(int &x) { ++x; }
来源：http://oow.tianlin.xyz

[S45] C++：lambda
来源：http://bei.guowangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://vde.ctjpmb.com

[S46] C++：函数模板
来源：http://uiv.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://irq.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://zfe.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ptt.52xcode.cn

[S48] C++：逐行读文件
来源：http://pza.fengsongda.top

std::ifstream in("a.txt");  std::string line;
来源：http://lyk.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://eew.mhx1999.top

[S49] C++：写文件
来源：http://yoy.zhoulong.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vez.gogol.net.cn

[S50] C++：格式化数字
来源：http://rnk.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uio.cqqwz.cn

[S51] C++：显式类型转换
来源：http://brv.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://drj.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://iml.zycfv.cn

int size() const noexcept { return n_; }
来源：http://ald.wangshuangyany.cn

[S53] C++：移动语义
来源：http://yvi.kuanghao11.cn

std::vector<int> w = std::move(v);
来源：http://cgg.wangshuangyany.cn

[S54] C++：异常处理
来源：http://vqj.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ysi.andypj.xyz

[S55] C++：结构化绑定
来源：http://ico.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://udy.snrcjt.cn

[S56] C++：optional
来源：http://epr.sweek.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hcg.yongpay.top

[S57] C++：编译期常量
来源：http://bdb.svipenyu.cn

constexpr int N = 10;
来源：http://aop.sweek.top

[S58] C++：命名空间
来源：http://dcc.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://cur.hnqzz.top

[S59] C++：静态断言
来源：http://ioq.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nmc.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://ljb.smart0.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fqw.sysykeji.top

================================================================================
来源：http://csw.zhaomingkeji.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fgf.pycfn.com

================================================================================
来源：http://osb.xziqi.cn

[T01] Kotlin：Hello World
来源：http://hjz.zycfv.cn

println("Hello")
来源：http://aow.gaohongyu789.top

[T02] Kotlin：变量
来源：http://ymi.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://skm.sxryk.cn

[T03] Kotlin：字符串模板
来源：http://rda.nanxuanxn.top

"值: $b"
来源：http://gkd.daxiang520.top

[T04] Kotlin：空安全
来源：http://adr.dianchejie.cn

val n: String? = null;  n?.length
来源：http://ciw.nanxinkj.top

[T05] Kotlin：when 表达式
来源：http://lrl.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tlb.chenzaomai.com

[T06] Kotlin：集合映射
来源：http://bvl.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vul.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://dbk.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nvi.hfpthk.cn

[T08] Kotlin：数据类
来源：http://yvu.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://fso.fzhhl.top

[T09] Kotlin：扩展函数
来源：http://jcl.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://rec.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://oxz.hesvh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uts.gotoacloud.top

[T11] Kotlin：协程
来源：http://ajl.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rzq.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://cuj.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://jds.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://ylx.yj20258.top

val m = mapOf("a" to 1)
来源：http://gbr.meibo888.top

[T14] Kotlin：循环
来源：http://fxx.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://qjb.andypj.xyz

[T15] Kotlin：接口
来源：http://wbg.guowangkeji.top

interface Shape { fun area(): Double }
来源：http://ldl.aizwys.cn

[T16] Swift：Hello World
来源：http://kvp.tanke756.top

print("Hello")
来源：http://csa.yfazqb.com

[T17] Swift：变量与常量
来源：http://pak.ybcxt.top

var a = 1;  let b = 2
来源：http://vna.snrcjt.cn

[T18] Swift：字符串插值
来源：http://osx.yongpay.top

"值: \(b)"
来源：http://pfy.jinghuilouyu.cn

[T19] Swift：可选绑定
来源：http://wjy.cashguo.top

if let n = opt { print(n) }
来源：http://ref.cucudq.cn

[T20] Swift：数组操作
来源：http://urv.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://qet.zhengqikj.top

[T21] Swift：遍历
来源：http://ilt.zhaomingkeji.xyz

for x in a { print(x) }
来源：http://vqg.hfpthk.cn

[T22] Swift：字典
来源：http://ecd.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://moz.havefunace.top

[T23] Swift：函数
来源：http://mgv.shanyushiyangtech.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mpl.shuidangran.top

[T24] Swift：闭包
来源：http://epf.9152youxi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ooh.sweek.top

[T25] Swift：结构体
来源：http://lez.andypj.xyz

struct P { var x: Int }
来源：http://iyf.zhixingplan.top

[T26] Swift：类与重写
来源：http://aip.hesvh.cn

class A: Base { override func f() {} }
来源：http://ccc.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://okt.yfazqb.com

do { try f() } catch { print(error) }
来源：http://cto.pengpengdd.cyou

[T28] Swift：枚举
来源：http://evs.pengpengdd.cyou

enum Color { case red, green }
来源：http://uhw.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://tkc.tanke756.top

guard let x = opt else { return }
来源：http://ong.yueranfly.top

[T30] Swift：协议
来源：http://kgr.bjfxy.top

protocol Shape { func area() -> Double }
来源：http://daj.hammf.cn

[T31] Lua：Hello World
来源：http://via.52xcode.cn

print("Hello")
来源：http://hus.snrcjt.cn

[T32] Lua：局部变量
来源：http://lcb.xylfe.cn

local a = 1
来源：http://eyt.zdbjq.cn

[T33] Lua：表（数组）
来源：http://yzv.yfazqb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ssn.yuanzhike.top

[T34] Lua：遍历表
来源：http://qfl.ybcxt.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mde.nanxuanxn.top

[T35] Lua：字典表
来源：http://zcj.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://gib.feifeiyinyue.top

[T36] Lua：函数
来源：http://sft.gaohongyu789.top

function add(a, b) return a + b end
来源：http://lew.wangshuangyany.cn


<!-- 参考信息 -->