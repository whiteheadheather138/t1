代发 wailian999

echo $((1 + 2 * 3))
来源：http://cml.yj20258.top

[R28] 浮点运算
来源：http://esl.sjlbkw.cn

echo "scale=2; 10/3" | bc
来源：http://lwo.zhoulong.xyz

[R29] 定义函数
来源：http://qic.shzxlz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://awb.shzxlz.cn

[R30] 函数返回状态码
来源：http://rui.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://dex.jiagoushi.top

[R31] 局部变量
来源：http://dwl.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://ghj.bjfxy.top

[R32] 参数个数校验
来源：http://tel.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kyf.yanxiufei.cn

[R33] 捕获错误并提示行号
来源：http://lrf.xuetiantiany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ojf.xinyue.icu

[R34] 退出时清理
来源：http://qeq.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://jzj.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://tis.shzxlz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ppa.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://qbw.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tza.daria6918.cn

[R37] 把输出赋给变量
来源：http://gvx.zdqjudy.top

files=$(ls -1)
来源：http://tcv.fengsongda.top

[R38] 管道串联
来源：http://wkw.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://dwv.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://jww.snrcjt.cn

cmd > out.log 2>&1
来源：http://owv.fktsv.cn

[R40] 追加写日志
来源：http://bdp.shzxlz.cn

echo "log" >> out.log
来源：http://icp.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://gjj.jqgufenzy.top

cmd >/dev/null 2>&1
来源：http://nhc.sysykeji.top

[R42] 输入重定向
来源：http://ecy.jqgfzy.top

wc -l < a.txt
来源：http://aiy.yangfankeji.com

[R43] 按名字查找文件
来源：http://klx.yuanzhike.top

find . -name "*.log" -type f
来源：http://dhd.316326.xyz

[R44] 按修改时间查找
来源：http://aoi.yongpay.top

find . -mtime -7 -type f
来源：http://hhe.shuidangran.top

[R45] 批量删除
来源：http://rlw.fehbvm.com

find . -name "*.tmp" -delete
来源：http://lzo.jinghuilouyu.cn

[R46] 递归替换文件内容
来源：http://hiq.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kpl.cheryme.top

[R47] sed 单行替换
来源：http://mdf.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fpt.hongshengwenyu.top

[R48] awk 取指定列
来源：http://wgk.hywenlv.cn

awk '{print $1, $3}' a.txt
来源：http://mmf.shangyingyoupin.top

[R49] awk 带条件
来源：http://xrc.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jvu.quarkkingdee.top

[R50] awk 求和
来源：http://lkq.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rmk.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://nen.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://msv.zhiwuduotai.top

[R52] 统计行数
来源：http://ihr.hesvh.cn

wc -l a.txt
来源：http://xna.gaohongyu789.top

[R53] 查看文件头与实时尾
来源：http://tnk.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fvb.cqqwz.cn

[R54] 比较两个文件
来源：http://jja.daria6918.cn

diff a.txt b.txt
来源：http://jnl.gaohongyu789.top

[R55] 压缩与解压
来源：http://itl.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tah.haohaochexian.top

[R56] 远程拷贝
来源：http://rxp.svipenyu.cn

scp file user@host:/path/
来源：http://vgu.yanxiufei.cn

[R57] 远程执行命令
来源：http://mcf.jianghu66.top

ssh user@host 'uptime'
来源：http://rzq.gzhubu.top

[R58] 下载文件
来源：http://pxp.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://esw.gzhubu.top

[R59] 发 POST JSON
来源：http://von.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kml.fzhhl.top

[R60] 只看 HTTP 状态码
来源：http://pvs.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tiq.pengpengdd.cyou

[R61] 磁盘占用
来源：http://apy.9152youxi.cn

df -h;  du -sh *
来源：http://agl.svipenyu.cn

[R62] 找最占空间的文件
来源：http://nah.cheryme.top

du -ah . | sort -rh | head -10
来源：http://yge.chenjidiqi.icu

[R63] 内存与进程
来源：http://hvv.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://phh.zdbjq.cn

[R64] 结束进程
来源：http://gcp.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://dge.iojbl.cn

[R65] 查看端口占用
来源：http://ajk.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qng.meibo888.top

[R66] 定时任务
来源：http://rgd.shangyingyoupin.top

crontab -e;  crontab -l
来源：http://hmh.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://frf.hfpthk.cn

openssl rand -hex 16
来源：http://psr.bjfxy.top

[R68] 计算文件校验值
来源：http://abh.cheryme.top

sha256sum a.txt;  md5sum a.txt
来源：http://hbk.bbcook.cn

[R69] 生成随机密码
来源：http://yvz.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://oma.jinqigufen.top

[R70] 时间戳与互转
来源：http://ujx.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://waz.cashguo.top

[R71] 日期格式化
来源：http://xdb.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zbg.shzxlz.cn

[R72] 等待端口就绪
来源：http://npu.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iif.epnwcf.com

[R73] 分割大日志
来源：http://ucr.nanxuanxn.top

split -l 1000 big.log part_
来源：http://pnt.nanxuanxn.top

[R74] 批量重命名
来源：http://azb.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yjb.tarul.cn

[R75] 导出环境变量
来源：http://fzf.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://cuz.quarkkingdee.top

[R76] 使用临时文件
来源：http://uov.jiagoushi.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zeb.vqdsnc.cn

[R77] 读取用户输入
来源：http://geu.fehbvm.com

read -rp "请输入: " ans
来源：http://yuq.gogol.net.cn

[R78] 交互式菜单
来源：http://jer.quarkkingdee.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hmg.chenlongwang.top

[R79] 解析命令行选项
来源：http://xrx.feifeiyinyue.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nho.sufxvd.cn

[R80] 查看脚本执行耗时
来源：http://ewo.shuidangran.top

time ./run.sh
来源：http://hur.sufxvd.cn

================================================================================
来源：http://ccw.sjlbkw.cn

S. C / C++ 专题
来源：http://ufj.ywan-chungtsiang.top

================================================================================
来源：http://njt.xingfuxueyuan.xyz

[S01] C：Hello World
来源：http://mez.cashguo.top

#include <stdio.h>
来源：http://uun.hfpthk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cuv.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://ego.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://yrh.iojbl.cn

[S03] C：读入整数
来源：http://ogc.xinyue.icu

int x; scanf("%d", &x);
来源：http://tzv.ybcxt.top

[S04] C：字符串复制
来源：http://kjh.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://syf.iojbl.cn

[S05] C：字符串长度
来源：http://ibz.zhoulong.xyz

strlen(s)
来源：http://dck.zdqjudy.top

[S06] C：字符串比较
来源：http://awq.xinyue.icu

strcmp(a, b) == 0
来源：http://vmv.hysaishi.cn

[S07] C：数组遍历求和
来源：http://iuo.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://njc.dianchejie.cn

[S08] C：动态内存分配与释放
来源：http://zmg.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://toz.feifeiyinyue.top

[S09] C：结构体定义与初始化
来源：http://rtr.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://izj.ppjwa.cn

[S10] C：指针与解引用
来源：http://hpz.sysykeji.top

int *p = &a;  *p = 5;
来源：http://mwd.xinyue.icu

[S11] C：逐行读文件
来源：http://bfy.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://hzk.gzhubu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ycq.daria6918.cn

fclose(f);
来源：http://kpx.tianlin.xyz

[S12] C：写文件
来源：http://tci.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vqd.ehwqpu.com

[S13] C：宏定义
来源：http://pjv.cashguo.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jyq.zdbjq.cn

[S14] C：枚举
来源：http://euc.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://dep.fktsv.cn

[S15] C：类型转换
来源：http://xzm.yangfankeji.com

(double) a / b
来源：http://qao.gzhubu.top

[S16] C：位操作置位
来源：http://bvt.quarkkingdee.top

x |= (1 << 3);
来源：http://rrd.hnqzz.top

[S17] C：安全拼接字符串
来源：http://psd.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bdl.feifeiyinyue.top

[S18] C：命令行参数
来源：http://xax.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://rtt.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://fao.uphjek.com

qsort(a, n, sizeof(int), cmp);
来源：http://tan.yangfankeji.com

[S20] C：二分查找
来源：http://pxd.jinqigufen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jjt.ehwqpu.com

[S21] C：字符类别判断
来源：http://jch.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jme.hnxiangtu.top

[S22] C：字符串转数字
来源：http://okv.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://yrf.yj20258888.top

[S23] C：随机数
来源：http://zzd.gzhubu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lre.sweek.top

[S24] C：获取本地时间
来源：http://ndl.fanxiaobao.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hoy.yj202588.top

[S25] C：内存拷贝
来源：http://jih.jqgfzy.top

memcpy(dst, src, n);
来源：http://vuo.52xcode.cn

[S26] C：内存清零
来源：http://irz.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://vee.xuanzx.com

[S27] C：定义常量
来源：http://fbf.jiagoushi.top

const double PI = 3.14159;
来源：http://wvr.vqdsnc.cn

[S28] C：静态变量
来源：http://xhp.zhaomingkeji.xyz

static int counter = 0;
来源：http://nnx.9152youxi.cn

[S29] C：变参函数
来源：http://jjr.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pjx.hesvh.cn

[S30] C：头文件保护
来源：http://rnt.jyoumei.cn

#ifndef X_H
来源：http://gfn.kuanghao11.cn

#define X_H
来源：http://mpf.tianlin.xyz

#endif
来源：http://hwe.tianlin.xyz

[S31] C++：Hello World
来源：http://ynu.bbcook.cn

#include <iostream>
来源：http://maf.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://vot.sxryk.cn

[S32] C++：字符串
来源：http://ofh.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://ful.dianchejie.cn

[S33] C++：vector 增删
来源：http://uuo.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://naq.gotoacloud.top

[S34] C++：遍历 vector
来源：http://bgp.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://mqu.havefunace.top

[S35] C++：map
来源：http://vel.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fkp.xuanzx.com

[S36] C++：unordered_map
来源：http://sqc.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tjv.iojbl.cn

[S37] C++：set
来源：http://hol.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kgd.hongshengwenyu.top

[S38] C++：排序
来源：http://tgk.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://dgi.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://cxs.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://itm.gzhubu.top

[S40] C++：查找元素
来源：http://bca.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wit.ydjk.org.cn

[S41] C++：类与构造函数
来源：http://wnr.tarul.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nue.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://rad.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://odx.shzxlz.cn

[S43] C++：智能指针
来源：http://bag.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://aur.gzhubu.top

[S44] C++：引用传参
来源：http://ayf.xziqi.cn

void inc(int &x) { ++x; }
来源：http://qvv.jqgufenzy.top

[S45] C++：lambda
来源：http://uza.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://ryn.nwbrower.top

[S46] C++：函数模板
来源：http://jin.hcnkem.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oyf.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://nch.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lin.tian-w.cn

[S48] C++：逐行读文件
来源：http://vvw.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://yhj.zhongyouzk.top

while (std::getline(in, line)) { }
来源：http://qqc.yangfankeji.com

[S49] C++：写文件
来源：http://exv.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ccs.aizwys.cn

[S50] C++：格式化数字
来源：http://agu.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ozj.ivvv.top

[S51] C++：显式类型转换
来源：http://gip.snrcjt.cn

static_cast<double>(a) / b
来源：http://hsp.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://sok.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://amh.dashuyun.cn

[S53] C++：移动语义
来源：http://eqb.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://vck.yuxming.cn

[S54] C++：异常处理
来源：http://uzk.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nwn.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://qfd.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lut.zdqjudy.top

[S56] C++：optional
来源：http://jew.hywenlv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lab.jqgufenzy.top

[S57] C++：编译期常量
来源：http://ggx.yj20258.top

constexpr int N = 10;
来源：http://iub.52xcode.cn

[S58] C++：命名空间
来源：http://nej.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://ryi.ybcxt.top

[S59] C++：静态断言
来源：http://wce.hesvh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bue.hywenlv.cn

[S60] C++：遍历并删除元素
来源：http://dio.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://exs.dashuyun.cn

================================================================================
来源：http://xlu.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gve.fehbvm.com

================================================================================
来源：http://ldg.fanxiaobao.xyz

[T01] Kotlin：Hello World
来源：http://dwd.shanyushiyangkeji.top

println("Hello")
来源：http://uqw.chenlongwang.top

[T02] Kotlin：变量
来源：http://sya.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bmq.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://djs.jianghu66.top

"值: $b"
来源：http://hjz.0kj1m.cn

[T04] Kotlin：空安全
来源：http://kvb.0kj1m.cn

val n: String? = null;  n?.length
来源：http://qrn.ydjk.org.cn

[T05] Kotlin：when 表达式
来源：http://vaj.pengpengdd.cyou

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pxj.hfpthk.cn

[T06] Kotlin：集合映射
来源：http://nxs.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://zva.cqqwz.cn

[T07] Kotlin：集合过滤
来源：http://qjx.jqgufenzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wnb.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://ybr.hfpthk.cn

data class User(val name: String, val age: Int)
来源：http://bed.ybcxt.top

[T09] Kotlin：扩展函数
来源：http://whu.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://kwd.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://xhs.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tsw.gzhubu.top

[T11] Kotlin：协程
来源：http://sza.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fft.pycfn.com

[T12] Kotlin：解构声明
来源：http://tdb.nwbrower.top

val (a, b) = Pair(1, 2)
来源：http://evp.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://nrj.tarul.cn

val m = mapOf("a" to 1)
来源：http://esv.ppjwa.cn

[T14] Kotlin：循环
来源：http://mak.mhx1999.top

for (i in 1..10) println(i)
来源：http://gyx.sxryk.cn

[T15] Kotlin：接口
来源：http://cnq.zdqjudy.top

interface Shape { fun area(): Double }
来源：http://ama.yangfankeji.com

[T16] Swift：Hello World
来源：http://qbn.ybcxt.top

print("Hello")
来源：http://dro.tianlin.xyz

[T17] Swift：变量与常量
来源：http://dsf.sysykeji.top

var a = 1;  let b = 2
来源：http://lbz.vehdjk.com

[T18] Swift：字符串插值
来源：http://wsg.yanxiufei.cn

"值: \(b)"
来源：http://sno.xinyue.icu

[T19] Swift：可选绑定
来源：http://jxo.sysykeji.top

if let n = opt { print(n) }
来源：http://vpk.jlsjyb.cn

[T20] Swift：数组操作
来源：http://ahg.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://nga.hysaishi.cn

[T21] Swift：遍历
来源：http://wzr.shangyingyoupin.top

for x in a { print(x) }
来源：http://gtr.epnwcf.com

[T22] Swift：字典
来源：http://ave.hysaishi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xyd.jianghu66.top

[T23] Swift：函数
来源：http://kfi.yuxming.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hjp.ppjwa.cn

[T24] Swift：闭包
来源：http://svo.nanxinkj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xpo.daria6918.cn

[T25] Swift：结构体
来源：http://iht.aizwys.cn

struct P { var x: Int }
来源：http://pkd.vehdjk.com

[T26] Swift：类与重写
来源：http://jdb.tian-w.cn

class A: Base { override func f() {} }
来源：http://dlm.yfazqb.com

[T27] Swift：错误处理
来源：http://fzg.bbcook.cn

do { try f() } catch { print(error) }
来源：http://exh.ctjpmb.com

[T28] Swift：枚举
来源：http://mfq.guannengcc.top

enum Color { case red, green }
来源：http://bgi.316326.xyz

[T29] Swift：guard 提前返回
来源：http://ygc.uphjek.com

guard let x = opt else { return }
来源：http://zzc.hcnkem.com

[T30] Swift：协议
来源：http://dgm.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://ukx.xylfe.cn


<!-- 参考信息 -->