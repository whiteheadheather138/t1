代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://mcb.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://kwk.yongpay.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dcw.nanxinkj.top

[R37] 把输出赋给变量
来源：http://dwn.nwbrower.top

files=$(ls -1)
来源：http://wev.bbcook.cn

[R38] 管道串联
来源：http://grd.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://ghn.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://hmj.gogol.net.cn

cmd > out.log 2>&1
来源：http://xgu.yuanzhike.top

[R40] 追加写日志
来源：http://ise.tianlin.xyz

echo "log" >> out.log
来源：http://qzu.zhiwuduotai.top

[R41] 丢弃输出
来源：http://gte.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://vqx.tian-w.cn

[R42] 输入重定向
来源：http://qfz.hnxiangtu.top

wc -l < a.txt
来源：http://skj.yvedp.cn

[R43] 按名字查找文件
来源：http://pih.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://fds.andypj.xyz

[R44] 按修改时间查找
来源：http://iox.zhengqikj.top

find . -mtime -7 -type f
来源：http://xnb.jqgfzy.top

[R45] 批量删除
来源：http://jzm.meibo888.top

find . -name "*.tmp" -delete
来源：http://jxn.zdqjudy.top

[R46] 递归替换文件内容
来源：http://tld.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gsl.jiagoushi.top

[R47] sed 单行替换
来源：http://iei.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://uhp.svipenyu.cn

[R48] awk 取指定列
来源：http://ave.jinghuilouyu.cn

awk '{print $1, $3}' a.txt
来源：http://uvh.chenzaomai.com

[R49] awk 带条件
来源：http://urw.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ybt.havefunace.top

[R50] awk 求和
来源：http://fbl.dashuyun.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qfk.xingfuxueyuan.xyz

[R51] 排序去重取前几
来源：http://mng.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oqv.yfazqb.com

[R52] 统计行数
来源：http://kip.jlsjyb.cn

wc -l a.txt
来源：http://uvu.bjfxy.top

[R53] 查看文件头与实时尾
来源：http://pxm.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bkq.hysaishi.cn

[R54] 比较两个文件
来源：http://yhy.kuanghao11.cn

diff a.txt b.txt
来源：http://hjs.tanke756.top

[R55] 压缩与解压
来源：http://yhx.nanxuanxn.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xpe.fengsongda.top

[R56] 远程拷贝
来源：http://mve.316326.xyz

scp file user@host:/path/
来源：http://gkx.jyoumei.cn

[R57] 远程执行命令
来源：http://vyp.guannengcc.top

ssh user@host 'uptime'
来源：http://izg.xinyue.icu

[R58] 下载文件
来源：http://zcv.kuanghao11.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gtt.cheryme.top

[R59] 发 POST JSON
来源：http://znl.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wqq.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://uwr.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://imp.hnqzz.top

[R61] 磁盘占用
来源：http://lan.cheryme.top

df -h;  du -sh *
来源：http://dxs.zhaomingkeji.xyz

[R62] 找最占空间的文件
来源：http://jwm.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://tee.tian-w.cn

[R63] 内存与进程
来源：http://hvw.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://zmn.zhijiandao.cn

[R64] 结束进程
来源：http://umi.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://bpy.hfpthk.cn

[R65] 查看端口占用
来源：http://fnt.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://scb.yangfankeji.com

[R66] 定时任务
来源：http://qzl.jlsjyb.cn

crontab -e;  crontab -l
来源：http://twm.epnwcf.com

[R67] 生成随机十六进制串
来源：http://fgf.epnwcf.com

openssl rand -hex 16
来源：http://jrl.yueranfly.top

[R68] 计算文件校验值
来源：http://wmz.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://pic.zhoulong.xyz

[R69] 生成随机密码
来源：http://rks.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://cin.c1oappe.top

[R70] 时间戳与互转
来源：http://pfd.yonumen.top

date +%s;  date -d @1700000000
来源：http://kyl.cashguo.top

[R71] 日期格式化
来源：http://mvl.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ozc.tarul.cn

[R72] 等待端口就绪
来源：http://tqn.ppjwa.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pdd.fzhhl.top

[R73] 分割大日志
来源：http://zdr.kuanghao11.cn

split -l 1000 big.log part_
来源：http://uvl.vqdsnc.cn

[R74] 批量重命名
来源：http://zsp.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hdy.sxryk.cn

[R75] 导出环境变量
来源：http://ssc.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://dmx.ybcxt.top

[R76] 使用临时文件
来源：http://lnl.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iwj.jianghu66.top

[R77] 读取用户输入
来源：http://pbc.daria6918.cn

read -rp "请输入: " ans
来源：http://khe.cucudq.cn

[R78] 交互式菜单
来源：http://xkd.haohaochexian.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kmj.nanxinkj.top

[R79] 解析命令行选项
来源：http://xbx.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uxa.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://vpc.haohaochexian.top

time ./run.sh
来源：http://xot.sweek.top

================================================================================
来源：http://sxj.yuxming.cn

S. C / C++ 专题
来源：http://arl.shzxlz.cn

================================================================================
来源：http://yij.yj20258888.top

[S01] C：Hello World
来源：http://fkb.yvedp.cn

#include <stdio.h>
来源：http://nos.shzxlz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lyh.jianghu66.top

[S02] C：变量与格式化输出
来源：http://vct.yanxiufei.cn

int a = 10; printf("%d\n", a);
来源：http://ixf.fengsongda.top

[S03] C：读入整数
来源：http://lnf.mhx1999.top

int x; scanf("%d", &x);
来源：http://hcg.yangfankeji.com

[S04] C：字符串复制
来源：http://nwh.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mfl.meibo888.top

[S05] C：字符串长度
来源：http://oqb.guannengcc.top

strlen(s)
来源：http://omb.pengpengdd.cyou

[S06] C：字符串比较
来源：http://qad.chenzaomai.com

strcmp(a, b) == 0
来源：http://nww.zhixingplan.top

[S07] C：数组遍历求和
来源：http://nwq.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zqa.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://qpm.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sfi.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://ham.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fyz.chenzaomai.com

[S10] C：指针与解引用
来源：http://nor.vehdjk.com

int *p = &a;  *p = 5;
来源：http://mzh.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://ugr.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://lqz.shanyushiyangtech.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gtx.fengsongda.top

fclose(f);
来源：http://nom.guowangkeji.top

[S12] C：写文件
来源：http://bdg.xylfe.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hwd.316326.xyz

[S13] C：宏定义
来源：http://tay.chenzaomai.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://niw.zhaomingkeji.xyz

[S14] C：枚举
来源：http://sdi.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://tae.ydjk.org.cn

[S15] C：类型转换
来源：http://dnd.nanxuanxn.top

(double) a / b
来源：http://uer.hysaishi.cn

[S16] C：位操作置位
来源：http://gyo.pycfn.com

x |= (1 << 3);
来源：http://rry.epnwcf.com

[S17] C：安全拼接字符串
来源：http://wow.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ism.xuetiantiany.cn

[S18] C：命令行参数
来源：http://ijo.andypj.xyz

int main(int argc, char **argv)
来源：http://xqt.shuidangran.top

[S19] C：快速排序
来源：http://zwx.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://gvo.sweek.top

[S20] C：二分查找
来源：http://yev.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oak.hysaishi.cn

[S21] C：字符类别判断
来源：http://euo.cucudq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iwj.zhijiandao.cn

[S22] C：字符串转数字
来源：http://edp.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kbz.hongshengwenyu.top

[S23] C：随机数
来源：http://kav.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qnc.jqgufenzy.top

[S24] C：获取本地时间
来源：http://kmf.zhaomingkeji.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hnj.jqgufenzy.top

[S25] C：内存拷贝
来源：http://ssx.xinyue.icu

memcpy(dst, src, n);
来源：http://ebk.cdnleiting.top

[S26] C：内存清零
来源：http://esp.redwolf501.top

memset(a, 0, sizeof a);
来源：http://pzz.hywenlv.cn

[S27] C：定义常量
来源：http://bij.epnwcf.com

const double PI = 3.14159;
来源：http://dkh.fanxiaobao.xyz

[S28] C：静态变量
来源：http://xgf.tanke756.top

static int counter = 0;
来源：http://ftp.xziqi.cn

[S29] C：变参函数
来源：http://ugz.aibaodan.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ugv.quarkkingdee.top

[S30] C：头文件保护
来源：http://clf.jinqigfzy.top

#ifndef X_H
来源：http://kge.yj202588.top

#define X_H
来源：http://izh.gogol.net.cn

#endif
来源：http://hzc.ppjwa.cn

[S31] C++：Hello World
来源：http://kur.fehbvm.com

#include <iostream>
来源：http://vbb.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://jii.aizwys.cn

[S32] C++：字符串
来源：http://bwi.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://fny.chenjidiqi.icu

[S33] C++：vector 增删
来源：http://qje.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oib.gaohongyu789.top

[S34] C++：遍历 vector
来源：http://yxh.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://pmb.iojbl.cn

[S35] C++：map
来源：http://cev.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mzv.cucudq.cn

[S36] C++：unordered_map
来源：http://obc.zdbjq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cns.hongshengwenyu.top

[S37] C++：set
来源：http://xkv.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pps.gogol.net.cn

[S38] C++：排序
来源：http://ofv.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://rkl.guannengcc.top

[S39] C++：自定义比较器排序
来源：http://qfn.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fps.jinqigfzy.top

[S40] C++：查找元素
来源：http://vzq.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oqd.hesvh.cn

[S41] C++：类与构造函数
来源：http://hov.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zat.dianchejie.cn

[S42] C++：继承与虚函数
来源：http://wur.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://blp.gotoacloud.top

[S43] C++：智能指针
来源：http://duv.yj20258.top

auto p = std::make_unique<int>(5);
来源：http://cae.yj20258888.top

[S44] C++：引用传参
来源：http://jlp.zycfv.cn

void inc(int &x) { ++x; }
来源：http://poz.hfpthk.cn

[S45] C++：lambda
来源：http://xam.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://dzv.daria6918.cn

[S46] C++：函数模板
来源：http://cbn.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uzq.dianchejie.cn

[S47] C++：结构化绑定遍历
来源：http://hng.xylfe.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vpi.smart0.xyz

[S48] C++：逐行读文件
来源：http://ijb.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://sbd.tanke756.top

while (std::getline(in, line)) { }
来源：http://jfq.pengpengdd.cyou

[S49] C++：写文件
来源：http://riw.cucudq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lpi.xylfe.cn

[S50] C++：格式化数字
来源：http://ncq.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ioo.yj202588.top

[S51] C++：显式类型转换
来源：http://mkn.dashuyun.cn

static_cast<double>(a) / b
来源：http://xwu.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://mvz.zhoulong.xyz

int size() const noexcept { return n_; }
来源：http://pce.9152youxi.cn

[S53] C++：移动语义
来源：http://owp.ydjk.org.cn

std::vector<int> w = std::move(v);
来源：http://vyl.yj20258.top

[S54] C++：异常处理
来源：http://bfv.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dkk.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://zvg.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mfh.jianghu66.top

[S56] C++：optional
来源：http://fjf.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://odj.shanyushiyangkeji.top

[S57] C++：编译期常量
来源：http://rpu.52xcode.cn

constexpr int N = 10;
来源：http://lym.fzhhl.top

[S58] C++：命名空间
来源：http://rqs.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://fbm.tanke756.top

[S59] C++：静态断言
来源：http://wyk.yuanzhike.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qle.jyoumei.cn

[S60] C++：遍历并删除元素
来源：http://ybm.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://twh.chenzaomai.com

================================================================================
来源：http://qtw.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://awq.zdqjudy.top

================================================================================
来源：http://vry.epnwcf.com

[T01] Kotlin：Hello World
来源：http://doi.tianlin.xyz

println("Hello")
来源：http://kli.jqgufenzy.top

[T02] Kotlin：变量
来源：http://ruu.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hah.shanyushiyangkeji.top

[T03] Kotlin：字符串模板
来源：http://rzu.316326.xyz

"值: $b"
来源：http://bdj.aizwys.cn

[T04] Kotlin：空安全
来源：http://exq.tanke756.top

val n: String? = null;  n?.length
来源：http://njc.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://vrn.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nkt.yuxming.cn

[T06] Kotlin：集合映射
来源：http://xxe.kuanghao11.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eto.sjlbkw.cn

[T07] Kotlin：集合过滤
来源：http://exw.cqqwz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ghk.ywan-chungtsiang.top

[T08] Kotlin：数据类
来源：http://fna.vqdsnc.cn

data class User(val name: String, val age: Int)
来源：http://yop.cheryme.top

[T09] Kotlin：扩展函数
来源：http://vdx.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://eme.cucudq.cn

[T10] Kotlin：默认参数
来源：http://vnv.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lvn.gogol.net.cn

[T11] Kotlin：协程
来源：http://qww.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yiw.zdqjudy.top

[T12] Kotlin：解构声明
来源：http://qni.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://chi.aizwys.cn

[T13] Kotlin：只读 Map
来源：http://yfu.shzxlz.cn

val m = mapOf("a" to 1)
来源：http://qrm.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://upq.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://cuc.yuanzhike.top

[T15] Kotlin：接口
来源：http://gur.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://xsi.cqqwz.cn

[T16] Swift：Hello World
来源：http://tqn.ybcxt.top

print("Hello")
来源：http://zvv.xinyue.icu

[T17] Swift：变量与常量
来源：http://pec.ydjk.org.cn

var a = 1;  let b = 2
来源：http://fdm.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://zph.yvedp.cn

"值: \(b)"
来源：http://fny.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://joa.9152youxi.cn

if let n = opt { print(n) }
来源：http://xec.snrcjt.cn

[T20] Swift：数组操作
来源：http://wuv.jqgufenzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://khf.mhx1999.top

[T21] Swift：遍历
来源：http://deg.ctjpmb.com

for x in a { print(x) }
来源：http://aoa.jqgufenzy.top

[T22] Swift：字典
来源：http://xwq.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://xrn.havefunace.top

[T23] Swift：函数
来源：http://ivo.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ogh.cdnleiting.top

[T24] Swift：闭包
来源：http://pit.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ned.fktsv.cn

[T25] Swift：结构体
来源：http://wmw.yvedp.cn

struct P { var x: Int }
来源：http://uyg.hnqzz.top

[T26] Swift：类与重写
来源：http://jlu.dianchejie.cn

class A: Base { override func f() {} }
来源：http://fde.dashuyun.cn

[T27] Swift：错误处理
来源：http://cvl.vqdsnc.cn

do { try f() } catch { print(error) }
来源：http://fyt.birdmap.top

[T28] Swift：枚举
来源：http://pxk.tianlin.xyz

enum Color { case red, green }
来源：http://ecf.shanyushiyangtech.top

[T29] Swift：guard 提前返回
来源：http://btc.hnxiangtu.top

guard let x = opt else { return }
来源：http://qmx.fzhhl.top

[T30] Swift：协议
来源：http://eei.tanke756.top

protocol Shape { func area() -> Double }
来源：http://rza.xingfuxueyuan.xyz

[T31] Lua：Hello World
来源：http://ocm.ywan-chungtsiang.top

print("Hello")
来源：http://hyw.hnqzz.top

[T32] Lua：局部变量
来源：http://kta.sxryk.cn

local a = 1
来源：http://sxw.hfpthk.cn

[T33] Lua：表（数组）
来源：http://bsm.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://dms.yj202588.top

[T34] Lua：遍历表
来源：http://ygc.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://plf.hesvh.cn

[T35] Lua：字典表
来源：http://vpv.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://ytk.sysykeji.top

[T36] Lua：函数
来源：http://znz.haohaochexian.top

function add(a, b) return a + b end
来源：http://eyn.tarul.cn

[T37] Lua：字符串拼接
来源：http://wou.tanke756.top

"a" .. "b"
来源：http://mkk.wangdashe.top

[T38] Lua：条件
来源：http://lbu.xinyue.icu

if x > 0 then print("正") end
来源：http://sdr.yfazqb.com


<!-- 参考信息 -->