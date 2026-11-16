代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lkd.yj20258.top

[R34] 退出时清理
来源：http://hnc.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nqk.dashuyun.cn

[R35] 后台执行并等待
来源：http://cdw.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dha.tian-w.cn

[R36] 并发执行多个任务
来源：http://myy.ehwqpu.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xif.xinyue.icu

[R37] 把输出赋给变量
来源：http://mra.xuetiantiany.cn

files=$(ls -1)
来源：http://bha.dashuyun.cn

[R38] 管道串联
来源：http://qil.aibaodan.cn

cat a.txt | grep -i error | wc -l
来源：http://mke.birdmap.top

[R39] 重定向标准输出与错误
来源：http://dxp.sxryk.cn

cmd > out.log 2>&1
来源：http://ghq.xinyue.icu

[R40] 追加写日志
来源：http://flz.wangdashe.top

echo "log" >> out.log
来源：http://hry.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://nbv.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://gac.pycfn.com

[R42] 输入重定向
来源：http://uyx.jqgfzy.top

wc -l < a.txt
来源：http://akb.vehdjk.com

[R43] 按名字查找文件
来源：http://krq.ydjk.org.cn

find . -name "*.log" -type f
来源：http://yuc.haohaochexian.top

[R44] 按修改时间查找
来源：http://dqd.nanxuanxn.top

find . -mtime -7 -type f
来源：http://tvr.birdmap.top

[R45] 批量删除
来源：http://ebv.fehbvm.com

find . -name "*.tmp" -delete
来源：http://cfg.yj202588.top

[R46] 递归替换文件内容
来源：http://zxa.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vdq.zdqjudy.top

[R47] sed 单行替换
来源：http://mfx.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://cli.sysykeji.top

[R48] awk 取指定列
来源：http://umi.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://ylr.iojbl.cn

[R49] awk 带条件
来源：http://wtp.zhaomingkeji.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vsr.yj20258888.top

[R50] awk 求和
来源：http://gow.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gbz.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://oaw.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://hjk.feifeiyinyue.top

[R52] 统计行数
来源：http://jve.wangdashe.top

wc -l a.txt
来源：http://siu.sysykeji.top

[R53] 查看文件头与实时尾
来源：http://lwk.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dfl.hywenlv.cn

[R54] 比较两个文件
来源：http://dur.jinqigfzy.top

diff a.txt b.txt
来源：http://mwe.tian-w.cn

[R55] 压缩与解压
来源：http://ddy.aibaodan.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hti.nwbrower.top

[R56] 远程拷贝
来源：http://yzq.shanyushiyangtech.top

scp file user@host:/path/
来源：http://uuf.pycfn.com

[R57] 远程执行命令
来源：http://jnf.sjlbkw.cn

ssh user@host 'uptime'
来源：http://cow.xingfuxueyuan.xyz

[R58] 下载文件
来源：http://izm.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gho.cdnleiting.top

[R59] 发 POST JSON
来源：http://sel.sufxvd.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oaa.zhiwuduotai.top

[R60] 只看 HTTP 状态码
来源：http://wqf.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ubs.yonumen.top

[R61] 磁盘占用
来源：http://ney.316326.xyz

df -h;  du -sh *
来源：http://slk.316326.xyz

[R62] 找最占空间的文件
来源：http://jnv.quarkkingdee.top

du -ah . | sort -rh | head -10
来源：http://ozr.zhoulong.xyz

[R63] 内存与进程
来源：http://blx.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://vok.hnqzz.top

[R64] 结束进程
来源：http://lcd.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://uah.dashuyun.cn

[R65] 查看端口占用
来源：http://ijg.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mzr.gotoacloud.top

[R66] 定时任务
来源：http://axu.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://zza.bjfxy.top

[R67] 生成随机十六进制串
来源：http://dqw.52xcode.cn

openssl rand -hex 16
来源：http://dyf.dashuyun.cn

[R68] 计算文件校验值
来源：http://wiz.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wji.ctjpmb.com

[R69] 生成随机密码
来源：http://phq.jqgufenzy.top

head -c 16 /dev/urandom | base64
来源：http://hvg.nanxuanxn.top

[R70] 时间戳与互转
来源：http://jln.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://fqf.yfazqb.com

[R71] 日期格式化
来源：http://une.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vyx.havefunace.top

[R72] 等待端口就绪
来源：http://jvc.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dwo.sweek.top

[R73] 分割大日志
来源：http://jbf.hcnkem.com

split -l 1000 big.log part_
来源：http://mez.jinqigfzy.top

[R74] 批量重命名
来源：http://aqq.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aqf.feifeiyinyue.top

[R75] 导出环境变量
来源：http://ezq.gogol.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://qdk.wangdashe.top

[R76] 使用临时文件
来源：http://tgg.9152youxi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gpo.jyoumei.cn

[R77] 读取用户输入
来源：http://rhf.dianchejie.cn

read -rp "请输入: " ans
来源：http://nvs.hywenlv.cn

[R78] 交互式菜单
来源：http://fef.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://trr.ybcxt.top

[R79] 解析命令行选项
来源：http://fcp.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nvu.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://nyg.gzhubu.top

time ./run.sh
来源：http://ygg.zycfv.cn

================================================================================
来源：http://kvp.cashguo.top

S. C / C++ 专题
来源：http://lyc.yueranfly.top

================================================================================
来源：http://zvh.bjfxy.top

[S01] C：Hello World
来源：http://pxl.yanxiufei.cn

#include <stdio.h>
来源：http://thg.hfpthk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tgr.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://xmf.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://rxy.zdqjudy.top

[S03] C：读入整数
来源：http://rjr.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://cql.kuanghao11.cn

[S04] C：字符串复制
来源：http://ndn.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://kti.yj202588.top

[S05] C：字符串长度
来源：http://oza.fzhhl.top

strlen(s)
来源：http://umf.yangfankeji.com

[S06] C：字符串比较
来源：http://ped.uphjek.com

strcmp(a, b) == 0
来源：http://xgf.sysykeji.top

[S07] C：数组遍历求和
来源：http://yov.daxiang520.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://axy.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://wlv.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kgw.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://pir.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kfs.zhoulong.xyz

[S10] C：指针与解引用
来源：http://pes.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://txt.gotoacloud.top

[S11] C：逐行读文件
来源：http://jxc.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://hdv.sjlbkw.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://any.yonumen.top

fclose(f);
来源：http://axj.quarkkingdee.top

[S12] C：写文件
来源：http://rba.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pwv.nanxinkj.top

[S13] C：宏定义
来源：http://wpg.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yrp.wangshuangyany.cn

[S14] C：枚举
来源：http://bmq.yj20258888.top

enum Color { RED, GREEN, BLUE };
来源：http://fcc.hongshengwenyu.top

[S15] C：类型转换
来源：http://sar.c1oappe.top

(double) a / b
来源：http://fpj.nanxinkj.top

[S16] C：位操作置位
来源：http://lqx.redwolf501.top

x |= (1 << 3);
来源：http://ean.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://qfq.vehdjk.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ggw.nanxuanxn.top

[S18] C：命令行参数
来源：http://kix.gaohongyu789.top

int main(int argc, char **argv)
来源：http://eoc.nanxuanxn.top

[S19] C：快速排序
来源：http://tfo.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://eln.sweek.top

[S20] C：二分查找
来源：http://wnf.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lyj.haohaochexian.top

[S21] C：字符类别判断
来源：http://qka.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ilj.shanyushiyangkeji.top

[S22] C：字符串转数字
来源：http://lvq.zhiwuduotai.top

atoi("42");  strtod("3.14", NULL);
来源：http://jfi.havefunace.top

[S23] C：随机数
来源：http://mqu.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wxb.kuanghao11.cn

[S24] C：获取本地时间
来源：http://ckz.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tee.jiagoushi.top

[S25] C：内存拷贝
来源：http://urw.zycfv.cn

memcpy(dst, src, n);
来源：http://upi.andypj.xyz

[S26] C：内存清零
来源：http://bnu.yj202588.top

memset(a, 0, sizeof a);
来源：http://axx.ctjpmb.com

[S27] C：定义常量
来源：http://brg.uphjek.com

const double PI = 3.14159;
来源：http://ngd.sysykeji.top

[S28] C：静态变量
来源：http://jyx.nanxuanxn.top

static int counter = 0;
来源：http://mph.wangshuangyany.cn

[S29] C：变参函数
来源：http://aqj.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://crw.gzhubu.top

[S30] C：头文件保护
来源：http://zxv.ppjwa.cn

#ifndef X_H
来源：http://sgo.zhixingplan.top

#define X_H
来源：http://bba.zhiwuduotai.top

#endif
来源：http://ftu.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://wxx.zhixingplan.top

#include <iostream>
来源：http://fzs.ctjpmb.com

int main() { std::cout << "Hello\n"; }
来源：http://xim.tarul.cn

[S32] C++：字符串
来源：http://oqa.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://avh.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://cnz.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aam.ivvv.top

[S34] C++：遍历 vector
来源：http://pwg.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://gff.zhengqikj.top

[S35] C++：map
来源：http://rjm.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://peu.dianchejie.cn

[S36] C++：unordered_map
来源：http://lne.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://peq.jyoumei.cn

[S37] C++：set
来源：http://ywo.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yer.tanke756.top

[S38] C++：排序
来源：http://ubl.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://fja.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://nkz.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zar.jianghu66.top

[S40] C++：查找元素
来源：http://yjp.zdqjudy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tyg.shzxlz.cn

[S41] C++：类与构造函数
来源：http://lbq.svipenyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nhg.316326.xyz

[S42] C++：继承与虚函数
来源：http://zdz.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://wrz.daxiang520.top

[S43] C++：智能指针
来源：http://ule.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://cng.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://emt.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://wxj.sweek.top

[S45] C++：lambda
来源：http://cfd.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://qoo.dashuyun.cn

[S46] C++：函数模板
来源：http://yin.yangfankeji.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://shd.yongpay.top

[S47] C++：结构化绑定遍历
来源：http://rlt.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yab.jianghu66.top

[S48] C++：逐行读文件
来源：http://jbw.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://apv.zhongyouzk.top

while (std::getline(in, line)) { }
来源：http://ixy.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://gen.hnqzz.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vut.havefunace.top

[S50] C++：格式化数字
来源：http://ldi.yj20258.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://egf.hcnkem.com

[S51] C++：显式类型转换
来源：http://ovp.smart0.xyz

static_cast<double>(a) / b
来源：http://izl.yj20258.top

[S52] C++：const 与 noexcept
来源：http://akd.havefunace.top

int size() const noexcept { return n_; }
来源：http://gzr.fktsv.cn

[S53] C++：移动语义
来源：http://ang.bjfxy.top

std::vector<int> w = std::move(v);
来源：http://kfo.nwbrower.top

[S54] C++：异常处理
来源：http://ksf.zhoulong.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bdi.guowangkeji.top

[S55] C++：结构化绑定
来源：http://lrl.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fgu.zhoulong.xyz

[S56] C++：optional
来源：http://edz.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zkf.chenjidiqi.icu

[S57] C++：编译期常量
来源：http://bef.iojbl.cn

constexpr int N = 10;
来源：http://ulb.zhaomingkeji.xyz

[S58] C++：命名空间
来源：http://gmm.jianghu66.top

namespace ns { int f() { return 1; } }
来源：http://aki.jlsjyb.cn

[S59] C++：静态断言
来源：http://yod.kuanghao11.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ztz.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://cpl.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dnw.tarul.cn

================================================================================
来源：http://uuh.gogol.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://avl.ybcxt.top

================================================================================
来源：http://sii.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://rle.shzxlz.cn

println("Hello")
来源：http://moo.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://ume.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gfw.meibo888.top

[T03] Kotlin：字符串模板
来源：http://fxn.wangshuangyany.cn

"值: $b"
来源：http://zuh.nanxinkj.top

[T04] Kotlin：空安全
来源：http://zky.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://wnk.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://boc.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zxr.guowangkeji.top

[T06] Kotlin：集合映射
来源：http://fcn.gaohongyu789.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kxi.aizwys.cn

[T07] Kotlin：集合过滤
来源：http://gnl.yueranfly.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vih.yj20258888.top

[T08] Kotlin：数据类
来源：http://oxh.fzhhl.top

data class User(val name: String, val age: Int)
来源：http://xhm.fktsv.cn

[T09] Kotlin：扩展函数
来源：http://vtw.cdnleiting.top

fun String.exclaim() = this + "!"
来源：http://xxv.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://wzc.cheryme.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kmq.svipenyu.cn

[T11] Kotlin：协程
来源：http://isa.cqqwz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qpt.vqdsnc.cn

[T12] Kotlin：解构声明
来源：http://oqy.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://oql.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://eco.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://zsv.xinyue.icu

[T14] Kotlin：循环
来源：http://aiw.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://vex.sjlbkw.cn

[T15] Kotlin：接口
来源：http://mbi.meibo888.top

interface Shape { fun area(): Double }
来源：http://szc.uphjek.com

[T16] Swift：Hello World
来源：http://fzf.yueranfly.top

print("Hello")
来源：http://pox.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://ihn.c1oappe.top

var a = 1;  let b = 2
来源：http://cgi.ybcxt.top

[T18] Swift：字符串插值
来源：http://ypg.xziqi.cn

"值: \(b)"
来源：http://qkg.nanxinkj.top

[T19] Swift：可选绑定
来源：http://usz.tianlin.xyz

if let n = opt { print(n) }
来源：http://wta.pycfn.com

[T20] Swift：数组操作
来源：http://yqr.yj202588.top

var a = [1, 2, 3];  a.append(4)
来源：http://eyr.xinyue.icu

[T21] Swift：遍历
来源：http://das.hysaishi.cn

for x in a { print(x) }
来源：http://ueu.epnwcf.com

[T22] Swift：字典
来源：http://uzn.sxryk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dyr.ydjk.org.cn

[T23] Swift：函数
来源：http://oke.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wgv.yangfankeji.com

[T24] Swift：闭包
来源：http://vqu.shanyushiyangtech.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zvc.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://qcp.bbcook.cn

struct P { var x: Int }
来源：http://hiu.shzxlz.cn

[T26] Swift：类与重写
来源：http://fyn.cucudq.cn

class A: Base { override func f() {} }
来源：http://kmv.jqgfzy.top

[T27] Swift：错误处理
来源：http://bxg.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://izx.xuetiantiany.cn

[T28] Swift：枚举
来源：http://xzw.zhixingplan.top

enum Color { case red, green }
来源：http://kvu.hnqzz.top

[T29] Swift：guard 提前返回
来源：http://spr.gogol.net.cn

guard let x = opt else { return }
来源：http://qgy.chenjidiqi.icu

[T30] Swift：协议
来源：http://aps.gaohongyu789.top

protocol Shape { func area() -> Double }
来源：http://bvg.aizwys.cn

[T31] Lua：Hello World
来源：http://amq.yvedp.cn

print("Hello")
来源：http://jtr.ivvv.top

[T32] Lua：局部变量
来源：http://jvr.sysykeji.top

local a = 1
来源：http://ftj.yueranfly.top

[T33] Lua：表（数组）
来源：http://zeq.yongpay.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sxj.cucudq.cn

[T34] Lua：遍历表
来源：http://nht.daria6918.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sgw.sxryk.cn

[T35] Lua：字典表
来源：http://lkn.hcnkem.com

local d = { a = 1 };  d.b = 2
来源：http://wob.nwbrower.top

[T36] Lua：函数
来源：http://adl.cdnleiting.top

function add(a, b) return a + b end
来源：http://bil.sysykeji.top


<!-- 参考信息 -->