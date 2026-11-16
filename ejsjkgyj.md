代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://txb.jinqigufen.top

[R36] 并发执行多个任务
来源：http://och.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://svm.haohaochexian.top

[R37] 把输出赋给变量
来源：http://jyh.yj20258.top

files=$(ls -1)
来源：http://lac.ybcxt.top

[R38] 管道串联
来源：http://fum.ehwqpu.com

cat a.txt | grep -i error | wc -l
来源：http://wcu.yj202588.top

[R39] 重定向标准输出与错误
来源：http://yha.guowangkeji.top

cmd > out.log 2>&1
来源：http://scr.sxryk.cn

[R40] 追加写日志
来源：http://ggp.bbcook.cn

echo "log" >> out.log
来源：http://mgo.yj202588.top

[R41] 丢弃输出
来源：http://tee.smart0.xyz

cmd >/dev/null 2>&1
来源：http://nfz.xuanzx.com

[R42] 输入重定向
来源：http://ucg.ydzc1.top

wc -l < a.txt
来源：http://tfj.ppjwa.cn

[R43] 按名字查找文件
来源：http://odl.shanyushiyangtech.top

find . -name "*.log" -type f
来源：http://atq.yangfankeji.com

[R44] 按修改时间查找
来源：http://iam.ybcxt.top

find . -mtime -7 -type f
来源：http://twg.zdqjudy.top

[R45] 批量删除
来源：http://upc.xuanzx.com

find . -name "*.tmp" -delete
来源：http://wld.iojbl.cn

[R46] 递归替换文件内容
来源：http://eog.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://abi.xuanzx.com

[R47] sed 单行替换
来源：http://yoe.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tvm.epnwcf.com

[R48] awk 取指定列
来源：http://cbd.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://xlu.yonumen.top

[R49] awk 带条件
来源：http://hcg.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rfx.jqgfzy.top

[R50] awk 求和
来源：http://iem.sysykeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://cso.fehbvm.com

[R51] 排序去重取前几
来源：http://dzt.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://utc.hesvh.cn

[R52] 统计行数
来源：http://box.zdqjudy.top

wc -l a.txt
来源：http://jur.cashguo.top

[R53] 查看文件头与实时尾
来源：http://vet.hywenlv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zmi.iojbl.cn

[R54] 比较两个文件
来源：http://uog.nanxuanxn.top

diff a.txt b.txt
来源：http://ffn.sjlbkw.cn

[R55] 压缩与解压
来源：http://bzm.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qug.yueranfly.top

[R56] 远程拷贝
来源：http://bdo.cashguo.top

scp file user@host:/path/
来源：http://dgu.yj202588.top

[R57] 远程执行命令
来源：http://lju.cashguo.top

ssh user@host 'uptime'
来源：http://wdc.zhongyouzk.top

[R58] 下载文件
来源：http://ecd.jinqigfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yty.sufxvd.cn

[R59] 发 POST JSON
来源：http://bsm.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ymw.gogol.net.cn

[R60] 只看 HTTP 状态码
来源：http://ldd.epnwcf.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cly.guowangkeji.top

[R61] 磁盘占用
来源：http://hcw.nanxuanxn.top

df -h;  du -sh *
来源：http://jdw.jianghu66.top

[R62] 找最占空间的文件
来源：http://xrk.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://qau.jqgfzy.top

[R63] 内存与进程
来源：http://hdf.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://sfl.zhaomingkeji.xyz

[R64] 结束进程
来源：http://lnv.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://otr.zhijiandao.cn

[R65] 查看端口占用
来源：http://cnb.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zmx.iojbl.cn

[R66] 定时任务
来源：http://vsg.aibaodan.cn

crontab -e;  crontab -l
来源：http://ppr.hammf.cn

[R67] 生成随机十六进制串
来源：http://ohr.sweek.top

openssl rand -hex 16
来源：http://lva.jyoumei.cn

[R68] 计算文件校验值
来源：http://kar.yfazqb.com

sha256sum a.txt;  md5sum a.txt
来源：http://oed.hysaishi.cn

[R69] 生成随机密码
来源：http://cyv.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://rkn.xuanzx.com

[R70] 时间戳与互转
来源：http://iqf.fanxiaobao.xyz

date +%s;  date -d @1700000000
来源：http://dvk.sufxvd.cn

[R71] 日期格式化
来源：http://ojc.redwolf501.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://aky.vqdsnc.cn

[R72] 等待端口就绪
来源：http://lgt.ppjwa.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://okn.smart0.xyz

[R73] 分割大日志
来源：http://niz.yfazqb.com

split -l 1000 big.log part_
来源：http://mrz.c1oappe.top

[R74] 批量重命名
来源：http://eyc.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dpm.yuanzhike.top

[R75] 导出环境变量
来源：http://isk.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://rxw.fengsongda.top

[R76] 使用临时文件
来源：http://lfb.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lep.dashuyun.cn

[R77] 读取用户输入
来源：http://vis.tian-w.cn

read -rp "请输入: " ans
来源：http://xzk.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://bdb.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cvb.wangdashe.top

[R79] 解析命令行选项
来源：http://pvi.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vnd.52xcode.cn

[R80] 查看脚本执行耗时
来源：http://fvk.cashguo.top

time ./run.sh
来源：http://itj.iojbl.cn

================================================================================
来源：http://fog.yj202588.top

S. C / C++ 专题
来源：http://ftv.hnqzz.top

================================================================================
来源：http://coo.jyoumei.cn

[S01] C：Hello World
来源：http://uer.cashguo.top

#include <stdio.h>
来源：http://hng.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://exk.jianghu66.top

[S02] C：变量与格式化输出
来源：http://ejn.9152youxi.cn

int a = 10; printf("%d\n", a);
来源：http://umj.tarul.cn

[S03] C：读入整数
来源：http://evk.tanke756.top

int x; scanf("%d", &x);
来源：http://nxz.snrcjt.cn

[S04] C：字符串复制
来源：http://enu.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://kwm.cqqwz.cn

[S05] C：字符串长度
来源：http://gux.epnwcf.com

strlen(s)
来源：http://bpz.yj20258888.top

[S06] C：字符串比较
来源：http://ppu.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://mmp.yuxming.cn

[S07] C：数组遍历求和
来源：http://ziu.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qag.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://ahu.0kj1m.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yei.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://zcd.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ifk.hesvh.cn

[S10] C：指针与解引用
来源：http://srr.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://zta.tanke756.top

[S11] C：逐行读文件
来源：http://fxu.fktsv.cn

FILE *f = fopen("a.txt", "r");
来源：http://ryg.bjfxy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xpz.xylfe.cn

fclose(f);
来源：http://vqj.ivvv.top

[S12] C：写文件
来源：http://myt.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tyz.aibaodan.cn

[S13] C：宏定义
来源：http://mii.jinyuanbaomall.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kbs.epnwcf.com

[S14] C：枚举
来源：http://szf.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://lqn.ivvv.top

[S15] C：类型转换
来源：http://stc.fengsongda.top

(double) a / b
来源：http://xod.guowangkeji.top

[S16] C：位操作置位
来源：http://htz.yonumen.top

x |= (1 << 3);
来源：http://inr.zdbjq.cn

[S17] C：安全拼接字符串
来源：http://lxt.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://puz.zhongyouzk.top

[S18] C：命令行参数
来源：http://nmh.mhx1999.top

int main(int argc, char **argv)
来源：http://ymk.epnwcf.com

[S19] C：快速排序
来源：http://ozw.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://xuq.tarul.cn

[S20] C：二分查找
来源：http://hvn.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uma.gogol.net.cn

[S21] C：字符类别判断
来源：http://hwu.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zwt.xylfe.cn

[S22] C：字符串转数字
来源：http://uxu.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://tqe.ydjk.org.cn

[S23] C：随机数
来源：http://xpf.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://uze.nanxuanxn.top

[S24] C：获取本地时间
来源：http://vdw.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://luq.feifeiyinyue.top

[S25] C：内存拷贝
来源：http://run.quarkkingdee.top

memcpy(dst, src, n);
来源：http://grd.xuetiantiany.cn

[S26] C：内存清零
来源：http://eey.jianghu66.top

memset(a, 0, sizeof a);
来源：http://xqg.316326.xyz

[S27] C：定义常量
来源：http://fpl.aizwys.cn

const double PI = 3.14159;
来源：http://tvw.316326.xyz

[S28] C：静态变量
来源：http://wtv.daria6918.cn

static int counter = 0;
来源：http://ogf.yuxming.cn

[S29] C：变参函数
来源：http://eot.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://emp.xuanzx.com

[S30] C：头文件保护
来源：http://quf.daria6918.cn

#ifndef X_H
来源：http://jqt.yuxming.cn

#define X_H
来源：http://gdt.yongpay.top

#endif
来源：http://pnq.fktsv.cn

[S31] C++：Hello World
来源：http://zmz.havefunace.top

#include <iostream>
来源：http://dho.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://rlt.dianchejie.cn

[S32] C++：字符串
来源：http://mlh.daria6918.cn

std::string s = "hi";  s += "!";
来源：http://ajc.sweek.top

[S33] C++：vector 增删
来源：http://cej.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qoa.uphjek.com

[S34] C++：遍历 vector
来源：http://bhu.hnqzz.top

for (auto &x : v) { std::cout << x; }
来源：http://fxr.zycfv.cn

[S35] C++：map
来源：http://dya.quarkkingdee.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qnk.smart0.xyz

[S36] C++：unordered_map
来源：http://elu.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wlq.meibo888.top

[S37] C++：set
来源：http://rat.hongshengwenyu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mqb.hammf.cn

[S38] C++：排序
来源：http://vvc.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://daq.havefunace.top

[S39] C++：自定义比较器排序
来源：http://qyy.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://peq.epnwcf.com

[S40] C++：查找元素
来源：http://hli.sweek.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rwy.cdnleiting.top

[S41] C++：类与构造函数
来源：http://lll.yonumen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qps.ybcxt.top

[S42] C++：继承与虚函数
来源：http://yfj.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://qrp.hysaishi.cn

[S43] C++：智能指针
来源：http://vzb.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://mpo.jinghuilouyu.cn

[S44] C++：引用传参
来源：http://xmw.yj20258.top

void inc(int &x) { ++x; }
来源：http://see.vqdsnc.cn

[S45] C++：lambda
来源：http://mjy.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ylg.xziqi.cn

[S46] C++：函数模板
来源：http://kxe.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xad.dianchejie.cn

[S47] C++：结构化绑定遍历
来源：http://aac.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zdq.xziqi.cn

[S48] C++：逐行读文件
来源：http://pet.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://knl.ywan-chungtsiang.top

while (std::getline(in, line)) { }
来源：http://vwe.ydjk.org.cn

[S49] C++：写文件
来源：http://zbx.zdqjudy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cwy.yueranfly.top

[S50] C++：格式化数字
来源：http://onx.zhiwuduotai.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wdh.hysaishi.cn

[S51] C++：显式类型转换
来源：http://dsj.yj20258.top

static_cast<double>(a) / b
来源：http://dqx.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://gbn.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://bim.sxryk.cn

[S53] C++：移动语义
来源：http://sji.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://uqs.xingfuxueyuan.xyz

[S54] C++：异常处理
来源：http://pra.fktsv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pri.chenzaomai.com

[S55] C++：结构化绑定
来源：http://gdg.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cwe.feifeiyinyue.top

[S56] C++：optional
来源：http://lxg.pengpengdd.cyou

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eyt.bjfxy.top

[S57] C++：编译期常量
来源：http://isq.zdbjq.cn

constexpr int N = 10;
来源：http://ggm.0kj1m.cn

[S58] C++：命名空间
来源：http://jne.xinyue.icu

namespace ns { int f() { return 1; } }
来源：http://wcz.yj20258.top

[S59] C++：静态断言
来源：http://zum.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://usz.ydjk.org.cn

[S60] C++：遍历并删除元素
来源：http://bpo.dashuyun.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gsm.hesvh.cn

================================================================================
来源：http://ghf.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hzt.andypj.xyz

================================================================================
来源：http://gbx.fengsongda.top

[T01] Kotlin：Hello World
来源：http://jce.smart0.xyz

println("Hello")
来源：http://dbd.shuidangran.top

[T02] Kotlin：变量
来源：http://gkh.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fal.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://zca.fehbvm.com

"值: $b"
来源：http://rad.meibo888.top

[T04] Kotlin：空安全
来源：http://jqh.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://vtd.shanyushiyangtech.top

[T05] Kotlin：when 表达式
来源：http://dkl.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jez.jinqigufen.top

[T06] Kotlin：集合映射
来源：http://ekh.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://khn.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://uvv.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vrf.nwbrower.top

[T08] Kotlin：数据类
来源：http://ezs.hfpthk.cn

data class User(val name: String, val age: Int)
来源：http://tks.jianghu66.top

[T09] Kotlin：扩展函数
来源：http://uhg.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://khb.vehdjk.com

[T10] Kotlin：默认参数
来源：http://eoq.dashuyun.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://joz.zycfv.cn

[T11] Kotlin：协程
来源：http://uum.chenlongwang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://eeo.hammf.cn

[T12] Kotlin：解构声明
来源：http://baq.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://qxf.ybcxt.top

[T13] Kotlin：只读 Map
来源：http://oti.sufxvd.cn

val m = mapOf("a" to 1)
来源：http://pay.nanxinkj.top

[T14] Kotlin：循环
来源：http://oob.dashuyun.cn

for (i in 1..10) println(i)
来源：http://szy.hysaishi.cn

[T15] Kotlin：接口
来源：http://vuo.vehdjk.com

interface Shape { fun area(): Double }
来源：http://fzw.havefunace.top

[T16] Swift：Hello World
来源：http://iom.yonumen.top

print("Hello")
来源：http://qsp.shuidangran.top

[T17] Swift：变量与常量
来源：http://zfy.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://gws.ivvv.top

[T18] Swift：字符串插值
来源：http://ygp.cheryme.top

"值: \(b)"
来源：http://lhl.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://iul.tian-w.cn

if let n = opt { print(n) }
来源：http://koz.yj20258.top

[T20] Swift：数组操作
来源：http://wxk.ppjwa.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kud.jlsjyb.cn

[T21] Swift：遍历
来源：http://zep.wangdashe.top

for x in a { print(x) }
来源：http://uyr.shuidangran.top

[T22] Swift：字典
来源：http://wma.zdqjudy.top

var d = ["a": 1];  d["b"] = 2
来源：http://sbw.gaohongyu789.top

[T23] Swift：函数
来源：http://cxr.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lrj.cqqwz.cn

[T24] Swift：闭包
来源：http://nbe.ppjwa.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lkc.9152youxi.cn

[T25] Swift：结构体
来源：http://wex.hcnkem.com

struct P { var x: Int }
来源：http://guh.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://qlx.jinqigfzy.top

class A: Base { override func f() {} }
来源：http://usc.0kj1m.cn

[T27] Swift：错误处理
来源：http://ahw.gotoacloud.top

do { try f() } catch { print(error) }
来源：http://dbx.shangyingyoupin.top

[T28] Swift：枚举
来源：http://yhb.meibo888.top

enum Color { case red, green }
来源：http://rje.jqgufenzy.top

[T29] Swift：guard 提前返回
来源：http://hha.zhaomingkeji.xyz

guard let x = opt else { return }
来源：http://ppe.zhengqikj.top

[T30] Swift：协议
来源：http://twl.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://ncz.snrcjt.cn

[T31] Lua：Hello World
来源：http://xnf.cashguo.top

print("Hello")
来源：http://qlu.hcnkem.com

[T32] Lua：局部变量
来源：http://qfb.andypj.xyz

local a = 1
来源：http://nku.aibaodan.cn

[T33] Lua：表（数组）
来源：http://omg.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lar.shanyushiyangkeji.top

[T34] Lua：遍历表
来源：http://ykx.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rpd.hnqzz.top

[T35] Lua：字典表
来源：http://vrc.cqqwz.cn

local d = { a = 1 };  d.b = 2
来源：http://eea.xinyue.icu

[T36] Lua：函数
来源：http://jwq.nanxuanxn.top

function add(a, b) return a + b end
来源：http://vkb.hesvh.cn

[T37] Lua：字符串拼接
来源：http://xpd.zhengqikj.top

"a" .. "b"
来源：http://tti.jinqigufen.top

[T38] Lua：条件
来源：http://qeg.epnwcf.com

if x > 0 then print("正") end
来源：http://ecs.52xcode.cn


<!-- 参考信息 -->