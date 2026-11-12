代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://qqz.gogol.net.cn

[R32] 参数个数校验
来源：http://gts.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kyv.yanxiufei.cn

[R33] 捕获错误并提示行号
来源：http://ily.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ccr.zdqjudy.top

[R34] 退出时清理
来源：http://cug.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://imx.yangfankeji.com

[R35] 后台执行并等待
来源：http://uep.hnxiangtu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://emi.tianlin.xyz

[R36] 并发执行多个任务
来源：http://glg.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pgz.guannengcc.top

[R37] 把输出赋给变量
来源：http://nga.ydjk.org.cn

files=$(ls -1)
来源：http://ply.xuetiantiany.cn

[R38] 管道串联
来源：http://wbi.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://hee.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://zid.c1oappe.top

cmd > out.log 2>&1
来源：http://vor.sjlbkw.cn

[R40] 追加写日志
来源：http://dvz.zhoulong.xyz

echo "log" >> out.log
来源：http://kdf.tian-w.cn

[R41] 丢弃输出
来源：http://qjm.haohaochexian.top

cmd >/dev/null 2>&1
来源：http://dfr.sysykeji.top

[R42] 输入重定向
来源：http://mlq.52xcode.cn

wc -l < a.txt
来源：http://esh.jinqigufen.top

[R43] 按名字查找文件
来源：http://qdk.zycfv.cn

find . -name "*.log" -type f
来源：http://ueo.birdmap.top

[R44] 按修改时间查找
来源：http://ysv.jqgufenzy.top

find . -mtime -7 -type f
来源：http://uqn.yonumen.top

[R45] 批量删除
来源：http://smx.jqgfzy.top

find . -name "*.tmp" -delete
来源：http://vmu.jyoumei.cn

[R46] 递归替换文件内容
来源：http://twf.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://biq.yueranfly.top

[R47] sed 单行替换
来源：http://amd.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://qky.cdnleiting.top

[R48] awk 取指定列
来源：http://qyo.xuanzx.com

awk '{print $1, $3}' a.txt
来源：http://vgu.ctjpmb.com

[R49] awk 带条件
来源：http://vfq.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cco.xuetiantiany.cn

[R50] awk 求和
来源：http://fem.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mty.bjfxy.top

[R51] 排序去重取前几
来源：http://azm.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eow.vehdjk.com

[R52] 统计行数
来源：http://vjf.cheryme.top

wc -l a.txt
来源：http://kqk.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://gyj.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://too.zhongyouzk.top

[R54] 比较两个文件
来源：http://rej.sxryk.cn

diff a.txt b.txt
来源：http://oiw.ivvv.top

[R55] 压缩与解压
来源：http://lbg.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kzv.zhoulong.xyz

[R56] 远程拷贝
来源：http://vno.gaohongyu789.top

scp file user@host:/path/
来源：http://lqi.jianghu66.top

[R57] 远程执行命令
来源：http://kux.yueranfly.top

ssh user@host 'uptime'
来源：http://xff.cucudq.cn

[R58] 下载文件
来源：http://gik.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ppe.hnqzz.top

[R59] 发 POST JSON
来源：http://ofx.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://okp.zdbjq.cn

[R60] 只看 HTTP 状态码
来源：http://ngo.zhiwuduotai.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ofl.xylfe.cn

[R61] 磁盘占用
来源：http://eop.9152youxi.cn

df -h;  du -sh *
来源：http://how.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://bil.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://jha.smart0.xyz

[R63] 内存与进程
来源：http://kdj.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://pqw.yfazqb.com

[R64] 结束进程
来源：http://pbr.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://epi.kuanghao11.cn

[R65] 查看端口占用
来源：http://rxd.redwolf501.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vfb.feifeiyinyue.top

[R66] 定时任务
来源：http://tic.feifeiyinyue.top

crontab -e;  crontab -l
来源：http://lag.zycfv.cn

[R67] 生成随机十六进制串
来源：http://mgg.bbcook.cn

openssl rand -hex 16
来源：http://qsu.gotoacloud.top

[R68] 计算文件校验值
来源：http://ewp.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://jzn.shanyushiyangkeji.top

[R69] 生成随机密码
来源：http://ejd.jinqigfzy.top

head -c 16 /dev/urandom | base64
来源：http://rhq.haohaochexian.top

[R70] 时间戳与互转
来源：http://uat.zhongyouzk.top

date +%s;  date -d @1700000000
来源：http://ran.jinqigfzy.top

[R71] 日期格式化
来源：http://aqn.yangfankeji.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://bni.shzxlz.cn

[R72] 等待端口就绪
来源：http://vfp.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://grw.bjfxy.top

[R73] 分割大日志
来源：http://ups.chenjidiqi.icu

split -l 1000 big.log part_
来源：http://ved.yonumen.top

[R74] 批量重命名
来源：http://cxc.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ppe.zhengqikj.top

[R75] 导出环境变量
来源：http://nma.yuxming.cn

export PATH="$HOME/bin:$PATH"
来源：http://etf.pengpengdd.cyou

[R76] 使用临时文件
来源：http://jja.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xki.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://lir.zhengqikj.top

read -rp "请输入: " ans
来源：http://vnz.jinqigufen.top

[R78] 交互式菜单
来源：http://fky.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jvs.xuanzx.com

[R79] 解析命令行选项
来源：http://bkx.yonumen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sso.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://zon.gzhubu.top

time ./run.sh
来源：http://jgn.ywan-chungtsiang.top

================================================================================
来源：http://ift.zdqjudy.top

S. C / C++ 专题
来源：http://mrs.jqgufenzy.top

================================================================================
来源：http://gpk.dianchejie.cn

[S01] C：Hello World
来源：http://sjl.zycfv.cn

#include <stdio.h>
来源：http://fpc.nanxinkj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fxk.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://stq.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://oho.andypj.xyz

[S03] C：读入整数
来源：http://xiz.fktsv.cn

int x; scanf("%d", &x);
来源：http://ewh.pycfn.com

[S04] C：字符串复制
来源：http://agw.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mnx.jyoumei.cn

[S05] C：字符串长度
来源：http://twf.zhaomingkeji.xyz

strlen(s)
来源：http://xxm.cqqwz.cn

[S06] C：字符串比较
来源：http://tdq.zhengqikj.top

strcmp(a, b) == 0
来源：http://mhs.zdqjudy.top

[S07] C：数组遍历求和
来源：http://wme.guowangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oxb.fanxiaobao.xyz

[S08] C：动态内存分配与释放
来源：http://uch.gaohongyu789.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://crt.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://vdm.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gyf.nanxinkj.top

[S10] C：指针与解引用
来源：http://iwx.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://mrf.jlsjyb.cn

[S11] C：逐行读文件
来源：http://mqe.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://xrz.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fpk.smart0.xyz

fclose(f);
来源：http://nia.aizwys.cn

[S12] C：写文件
来源：http://bce.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xiw.hcnkem.com

[S13] C：宏定义
来源：http://eaa.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yfv.xylfe.cn

[S14] C：枚举
来源：http://gwe.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://twm.gaohongyu789.top

[S15] C：类型转换
来源：http://lzv.epnwcf.com

(double) a / b
来源：http://hje.0kj1m.cn

[S16] C：位操作置位
来源：http://uys.tarul.cn

x |= (1 << 3);
来源：http://axm.nwbrower.top

[S17] C：安全拼接字符串
来源：http://jio.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ldy.shangyingyoupin.top

[S18] C：命令行参数
来源：http://jrd.cdnleiting.top

int main(int argc, char **argv)
来源：http://ock.jinqigfzy.top

[S19] C：快速排序
来源：http://ekz.jinghuilouyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://how.nanxuanxn.top

[S20] C：二分查找
来源：http://kif.hfpthk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nmk.tarul.cn

[S21] C：字符类别判断
来源：http://ruf.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jzr.zhengqikj.top

[S22] C：字符串转数字
来源：http://zaz.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://vhm.tanke756.top

[S23] C：随机数
来源：http://apr.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cpj.cheryme.top

[S24] C：获取本地时间
来源：http://enq.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ixi.316326.xyz

[S25] C：内存拷贝
来源：http://ydg.fehbvm.com

memcpy(dst, src, n);
来源：http://mdd.nanxuanxn.top

[S26] C：内存清零
来源：http://lsl.sjlbkw.cn

memset(a, 0, sizeof a);
来源：http://ets.havefunace.top

[S27] C：定义常量
来源：http://uyb.sweek.top

const double PI = 3.14159;
来源：http://qce.sjlbkw.cn

[S28] C：静态变量
来源：http://ezu.jinghuilouyu.cn

static int counter = 0;
来源：http://lcc.zhijiandao.cn

[S29] C：变参函数
来源：http://fyw.dashuyun.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rfa.shanyushiyangtech.top

[S30] C：头文件保护
来源：http://csl.zhengqikj.top

#ifndef X_H
来源：http://sio.ivvv.top

#define X_H
来源：http://ffy.pycfn.com

#endif
来源：http://krq.c1oappe.top

[S31] C++：Hello World
来源：http://gos.yvedp.cn

#include <iostream>
来源：http://fty.fanxiaobao.xyz

int main() { std::cout << "Hello\n"; }
来源：http://auf.tanke756.top

[S32] C++：字符串
来源：http://wvv.xuanzx.com

std::string s = "hi";  s += "!";
来源：http://cok.fktsv.cn

[S33] C++：vector 增删
来源：http://mnn.uphjek.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bbr.zhixingplan.top

[S34] C++：遍历 vector
来源：http://rbv.sjlbkw.cn

for (auto &x : v) { std::cout << x; }
来源：http://nhh.mhx1999.top

[S35] C++：map
来源：http://oqx.sweek.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://atf.yongpay.top

[S36] C++：unordered_map
来源：http://vvi.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qzj.gotoacloud.top

[S37] C++：set
来源：http://fkw.bbcook.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pgq.316326.xyz

[S38] C++：排序
来源：http://jzn.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://cfw.yj20258.top

[S39] C++：自定义比较器排序
来源：http://txo.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://drk.hcnkem.com

[S40] C++：查找元素
来源：http://our.zhengqikj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pbm.gotoacloud.top

[S41] C++：类与构造函数
来源：http://dnh.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vod.feifeiyinyue.top

[S42] C++：继承与虚函数
来源：http://szi.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://plj.shzxlz.cn

[S43] C++：智能指针
来源：http://cwd.xuetiantiany.cn

auto p = std::make_unique<int>(5);
来源：http://yua.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://owk.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://opt.yueranfly.top

[S45] C++：lambda
来源：http://gkf.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://xhy.nanxuanxn.top

[S46] C++：函数模板
来源：http://hcc.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://itw.cdnleiting.top

[S47] C++：结构化绑定遍历
来源：http://gjv.wangshuangyany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sqz.yangfankeji.com

[S48] C++：逐行读文件
来源：http://mdp.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://ohd.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://lfb.daxiang520.top

[S49] C++：写文件
来源：http://fcr.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vxd.yvedp.cn

[S50] C++：格式化数字
来源：http://lxr.redwolf501.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zup.xinyue.icu

[S51] C++：显式类型转换
来源：http://ppe.sjlbkw.cn

static_cast<double>(a) / b
来源：http://ziz.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://ajv.zycfv.cn

int size() const noexcept { return n_; }
来源：http://fvd.0kj1m.cn

[S53] C++：移动语义
来源：http://hpt.birdmap.top

std::vector<int> w = std::move(v);
来源：http://wkj.haohaochexian.top

[S54] C++：异常处理
来源：http://zea.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zct.guannengcc.top

[S55] C++：结构化绑定
来源：http://bfa.smart0.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://npx.chenlongwang.top

[S56] C++：optional
来源：http://gry.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oma.svipenyu.cn

[S57] C++：编译期常量
来源：http://uby.shzxlz.cn

constexpr int N = 10;
来源：http://xcd.vehdjk.com

[S58] C++：命名空间
来源：http://vct.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://gjt.yuanzhike.top

[S59] C++：静态断言
来源：http://cde.ybcxt.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pgf.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://qvw.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gpn.snrcjt.cn

================================================================================
来源：http://hzx.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ggj.kuanghao11.cn

================================================================================
来源：http://afx.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://omo.jinqigfzy.top

println("Hello")
来源：http://iyt.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://myp.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pmv.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://ezd.hongshengwenyu.top

"值: $b"
来源：http://ysf.quarkkingdee.top

[T04] Kotlin：空安全
来源：http://hur.fengsongda.top

val n: String? = null;  n?.length
来源：http://yax.ivvv.top

[T05] Kotlin：when 表达式
来源：http://bis.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://crg.yj20258.top

[T06] Kotlin：集合映射
来源：http://ctw.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cjv.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://kzs.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xxi.bbcook.cn

[T08] Kotlin：数据类
来源：http://iua.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://dpw.tianlin.xyz

[T09] Kotlin：扩展函数
来源：http://fxp.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://bli.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://jht.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iuu.quarkkingdee.top

[T11] Kotlin：协程
来源：http://dmf.hfpthk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ymh.vehdjk.com

[T12] Kotlin：解构声明
来源：http://ofv.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://kom.ydzc1.top

[T13] Kotlin：只读 Map
来源：http://xsg.dashuyun.cn

val m = mapOf("a" to 1)
来源：http://oub.9152youxi.cn

[T14] Kotlin：循环
来源：http://syf.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://iey.daxiang520.top

[T15] Kotlin：接口
来源：http://ccj.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://gpp.zdqjudy.top

[T16] Swift：Hello World
来源：http://bwy.zycfv.cn

print("Hello")
来源：http://kmi.zycfv.cn

[T17] Swift：变量与常量
来源：http://fsw.yvedp.cn

var a = 1;  let b = 2
来源：http://iqu.kuanghao11.cn

[T18] Swift：字符串插值
来源：http://ste.tianlin.xyz

"值: \(b)"
来源：http://qdp.jiagoushi.top

[T19] Swift：可选绑定
来源：http://szw.fktsv.cn

if let n = opt { print(n) }
来源：http://wta.shanyushiyangtech.top

[T20] Swift：数组操作
来源：http://vxt.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://tsp.zhixingplan.top

[T21] Swift：遍历
来源：http://wls.zhiwuduotai.top

for x in a { print(x) }
来源：http://vzf.gzhubu.top

[T22] Swift：字典
来源：http://bgl.c1oappe.top

var d = ["a": 1];  d["b"] = 2
来源：http://szz.ywan-chungtsiang.top

[T23] Swift：函数
来源：http://vte.316326.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://idd.cdnleiting.top

[T24] Swift：闭包
来源：http://adz.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://ptu.hnxiangtu.top

[T25] Swift：结构体
来源：http://xxl.vqdsnc.cn

struct P { var x: Int }
来源：http://ysq.sxryk.cn

[T26] Swift：类与重写
来源：http://jdp.ppjwa.cn

class A: Base { override func f() {} }
来源：http://ckq.gotoacloud.top

[T27] Swift：错误处理
来源：http://ext.ybcxt.top

do { try f() } catch { print(error) }
来源：http://gpb.gogol.net.cn

[T28] Swift：枚举
来源：http://emg.xuanzx.com

enum Color { case red, green }
来源：http://zdt.zdqjudy.top

[T29] Swift：guard 提前返回
来源：http://wvs.yangfankeji.com

guard let x = opt else { return }
来源：http://zgm.vqdsnc.cn

[T30] Swift：协议
来源：http://kfs.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://dwi.gzhubu.top

[T31] Lua：Hello World
来源：http://nuo.nwbrower.top

print("Hello")
来源：http://uxc.zhiwuduotai.top

[T32] Lua：局部变量
来源：http://dfp.ydjk.org.cn

local a = 1
来源：http://tty.sufxvd.cn

[T33] Lua：表（数组）
来源：http://nac.jqgfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gpn.epnwcf.com

[T34] Lua：遍历表
来源：http://cmw.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dgv.jiagoushi.top


<!-- 参考信息 -->