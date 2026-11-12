代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://huk.tarul.cn

[R34] 退出时清理
来源：http://tzz.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://yws.fanxiaobao.xyz

[R35] 后台执行并等待
来源：http://eks.wangdashe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ypg.gogol.net.cn

[R36] 并发执行多个任务
来源：http://wxn.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cpr.yj20258888.top

[R37] 把输出赋给变量
来源：http://wxk.jinyuanbaomall.cn

files=$(ls -1)
来源：http://qms.zdqjudy.top

[R38] 管道串联
来源：http://dny.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://zjp.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://ney.vehdjk.com

cmd > out.log 2>&1
来源：http://aza.fktsv.cn

[R40] 追加写日志
来源：http://ako.guowangkeji.top

echo "log" >> out.log
来源：http://hyj.hnxiangtu.top

[R41] 丢弃输出
来源：http://gyy.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://ogh.aizwys.cn

[R42] 输入重定向
来源：http://hry.9152youxi.cn

wc -l < a.txt
来源：http://tqb.vehdjk.com

[R43] 按名字查找文件
来源：http://ytv.cashguo.top

find . -name "*.log" -type f
来源：http://uhp.9152youxi.cn

[R44] 按修改时间查找
来源：http://pkp.bjfxy.top

find . -mtime -7 -type f
来源：http://xht.epnwcf.com

[R45] 批量删除
来源：http://nvs.yfazqb.com

find . -name "*.tmp" -delete
来源：http://cff.wangdashe.top

[R46] 递归替换文件内容
来源：http://qgs.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jyr.aizwys.cn

[R47] sed 单行替换
来源：http://agq.smart0.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://nsa.daxiang520.top

[R48] awk 取指定列
来源：http://zmt.zdbjq.cn

awk '{print $1, $3}' a.txt
来源：http://qnr.fanxiaobao.xyz

[R49] awk 带条件
来源：http://kia.iojbl.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://skc.jianghu66.top

[R50] awk 求和
来源：http://lkh.yfazqb.com

awk '{s += $2} END {print s}' a.txt
来源：http://fcb.epnwcf.com

[R51] 排序去重取前几
来源：http://tpz.shuidangran.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lzq.bbcook.cn

[R52] 统计行数
来源：http://zhd.sxryk.cn

wc -l a.txt
来源：http://xpv.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://azy.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rsd.yanxiufei.cn

[R54] 比较两个文件
来源：http://nfr.andypj.xyz

diff a.txt b.txt
来源：http://nki.iojbl.cn

[R55] 压缩与解压
来源：http://xjr.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://esg.yvedp.cn

[R56] 远程拷贝
来源：http://sog.zhijiandao.cn

scp file user@host:/path/
来源：http://hnv.andypj.xyz

[R57] 远程执行命令
来源：http://ohm.ivvv.top

ssh user@host 'uptime'
来源：http://oxi.ydzc1.top

[R58] 下载文件
来源：http://dqr.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mho.xuanzx.com

[R59] 发 POST JSON
来源：http://qah.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yio.meibo888.top

[R60] 只看 HTTP 状态码
来源：http://gfp.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bhe.hfpthk.cn

[R61] 磁盘占用
来源：http://nya.hnqzz.top

df -h;  du -sh *
来源：http://vef.aibaodan.cn

[R62] 找最占空间的文件
来源：http://kpt.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://orq.bbcook.cn

[R63] 内存与进程
来源：http://nur.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://jco.wangdashe.top

[R64] 结束进程
来源：http://vph.chenlongwang.top

kill -9 $(pgrep -f app.py)
来源：http://cuy.hcnkem.com

[R65] 查看端口占用
来源：http://wke.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sxf.iojbl.cn

[R66] 定时任务
来源：http://ibu.nanxinkj.top

crontab -e;  crontab -l
来源：http://kiw.52xcode.cn

[R67] 生成随机十六进制串
来源：http://vgr.wangshuangyany.cn

openssl rand -hex 16
来源：http://pji.aibaodan.cn

[R68] 计算文件校验值
来源：http://djd.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ioe.tian-w.cn

[R69] 生成随机密码
来源：http://otn.sysykeji.top

head -c 16 /dev/urandom | base64
来源：http://pba.yfazqb.com

[R70] 时间戳与互转
来源：http://dxz.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://yrf.guannengcc.top

[R71] 日期格式化
来源：http://jld.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gop.jinqigfzy.top

[R72] 等待端口就绪
来源：http://agu.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bof.shzxlz.cn

[R73] 分割大日志
来源：http://tyh.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://tvt.xylfe.cn

[R74] 批量重命名
来源：http://hfp.sysykeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mmw.ehwqpu.com

[R75] 导出环境变量
来源：http://btx.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://crj.cqqwz.cn

[R76] 使用临时文件
来源：http://lbv.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xht.gzhubu.top

[R77] 读取用户输入
来源：http://haj.yonumen.top

read -rp "请输入: " ans
来源：http://srw.yueranfly.top

[R78] 交互式菜单
来源：http://ioc.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xfl.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://esg.cqqwz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jfu.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://tlb.jinyuanbaomall.cn

time ./run.sh
来源：http://erz.xingfuxueyuan.xyz

================================================================================
来源：http://pss.quarkkingdee.top

S. C / C++ 专题
来源：http://vaf.aizwys.cn

================================================================================
来源：http://hsu.zhijiandao.cn

[S01] C：Hello World
来源：http://lep.yuxming.cn

#include <stdio.h>
来源：http://nmt.ywan-chungtsiang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gvu.mhx1999.top

[S02] C：变量与格式化输出
来源：http://gld.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://eff.cashguo.top

[S03] C：读入整数
来源：http://vkb.snrcjt.cn

int x; scanf("%d", &x);
来源：http://jcl.daria6918.cn

[S04] C：字符串复制
来源：http://uah.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://vog.ppjwa.cn

[S05] C：字符串长度
来源：http://yti.zdqjudy.top

strlen(s)
来源：http://muh.hongshengwenyu.top

[S06] C：字符串比较
来源：http://eyu.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://nun.dashuyun.cn

[S07] C：数组遍历求和
来源：http://zkg.ydzc1.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zqo.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://nqd.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ylo.shuidangran.top

[S09] C：结构体定义与初始化
来源：http://rqa.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xpr.zhiwuduotai.top

[S10] C：指针与解引用
来源：http://hhb.mhx1999.top

int *p = &a;  *p = 5;
来源：http://mrx.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://guw.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://hvd.jqgufenzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yxm.xingfuxueyuan.xyz

fclose(f);
来源：http://kcg.hfpthk.cn

[S12] C：写文件
来源：http://grl.guowangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wti.yfazqb.com

[S13] C：宏定义
来源：http://pzo.xingfuxueyuan.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nhm.316326.xyz

[S14] C：枚举
来源：http://cca.hammf.cn

enum Color { RED, GREEN, BLUE };
来源：http://hof.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://tkb.gzhubu.top

(double) a / b
来源：http://kyb.xylfe.cn

[S16] C：位操作置位
来源：http://udb.fktsv.cn

x |= (1 << 3);
来源：http://gke.sysykeji.top

[S17] C：安全拼接字符串
来源：http://brq.gotoacloud.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://brm.pengpengdd.cyou

[S18] C：命令行参数
来源：http://mtt.guannengcc.top

int main(int argc, char **argv)
来源：http://ctv.tarul.cn

[S19] C：快速排序
来源：http://lqw.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://ubu.yueranfly.top

[S20] C：二分查找
来源：http://xvd.yangfankeji.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://khx.nanxinkj.top

[S21] C：字符类别判断
来源：http://yye.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rqc.yonumen.top

[S22] C：字符串转数字
来源：http://tio.cashguo.top

atoi("42");  strtod("3.14", NULL);
来源：http://uba.haohaochexian.top

[S23] C：随机数
来源：http://prl.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://aoq.sxryk.cn

[S24] C：获取本地时间
来源：http://lxm.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lqw.zhijiandao.cn

[S25] C：内存拷贝
来源：http://nhv.yj20258.top

memcpy(dst, src, n);
来源：http://tgf.gaohongyu789.top

[S26] C：内存清零
来源：http://qaf.yvedp.cn

memset(a, 0, sizeof a);
来源：http://xos.yfazqb.com

[S27] C：定义常量
来源：http://ozl.yuanzhike.top

const double PI = 3.14159;
来源：http://pfp.9152youxi.cn

[S28] C：静态变量
来源：http://cmu.guowangkeji.top

static int counter = 0;
来源：http://rbd.tanke756.top

[S29] C：变参函数
来源：http://yfy.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pxr.zdqjudy.top

[S30] C：头文件保护
来源：http://yrr.zhijiandao.cn

#ifndef X_H
来源：http://xhc.shanyushiyangtech.top

#define X_H
来源：http://baq.9152youxi.cn

#endif
来源：http://klk.gotoacloud.top

[S31] C++：Hello World
来源：http://vdj.shanyushiyangtech.top

#include <iostream>
来源：http://bbr.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://nmh.tanke756.top

[S32] C++：字符串
来源：http://ijo.feifeiyinyue.top

std::string s = "hi";  s += "!";
来源：http://koa.sweek.top

[S33] C++：vector 增删
来源：http://swk.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ndq.daxiang520.top

[S34] C++：遍历 vector
来源：http://qst.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://jlx.ywan-chungtsiang.top

[S35] C++：map
来源：http://mrv.dashuyun.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kyx.quarkkingdee.top

[S36] C++：unordered_map
来源：http://bwc.birdmap.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yoi.aibaodan.cn

[S37] C++：set
来源：http://tmh.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wuk.vehdjk.com

[S38] C++：排序
来源：http://hbm.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://rtp.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://gxt.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xhq.tanke756.top

[S40] C++：查找元素
来源：http://mxa.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lma.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://teh.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cnb.aizwys.cn

[S42] C++：继承与虚函数
来源：http://riu.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://ieo.xingfuxueyuan.xyz

[S43] C++：智能指针
来源：http://nqa.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://fdo.ctjpmb.com

[S44] C++：引用传参
来源：http://dhf.yuxming.cn

void inc(int &x) { ++x; }
来源：http://rdd.shanyushiyangkeji.top

[S45] C++：lambda
来源：http://vns.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://rhy.52xcode.cn

[S46] C++：函数模板
来源：http://dat.fzhhl.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://anc.ybcxt.top

[S47] C++：结构化绑定遍历
来源：http://vrp.svipenyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hnc.haohaochexian.top

[S48] C++：逐行读文件
来源：http://svx.chenjidiqi.icu

std::ifstream in("a.txt");  std::string line;
来源：http://hry.tanke756.top

while (std::getline(in, line)) { }
来源：http://fxs.feifeiyinyue.top

[S49] C++：写文件
来源：http://qnc.snrcjt.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nff.uphjek.com

[S50] C++：格式化数字
来源：http://qyy.guannengcc.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oby.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://iqi.svipenyu.cn

static_cast<double>(a) / b
来源：http://hdh.svipenyu.cn

[S52] C++：const 与 noexcept
来源：http://pxd.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://brn.yongpay.top

[S53] C++：移动语义
来源：http://nfa.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://gnt.zdbjq.cn

[S54] C++：异常处理
来源：http://jwc.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mbt.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://erw.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lge.yuanzhike.top

[S56] C++：optional
来源：http://vqa.hnqzz.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ijs.bjfxy.top

[S57] C++：编译期常量
来源：http://jir.kuanghao11.cn

constexpr int N = 10;
来源：http://vbc.sxryk.cn

[S58] C++：命名空间
来源：http://vma.kuanghao11.cn

namespace ns { int f() { return 1; } }
来源：http://fgb.cdnleiting.top

[S59] C++：静态断言
来源：http://yae.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sci.chenzaomai.com

[S60] C++：遍历并删除元素
来源：http://cag.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pqh.zhongyouzk.top

================================================================================
来源：http://iop.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bgt.yuxming.cn

================================================================================
来源：http://dwx.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://oav.zdbjq.cn

println("Hello")
来源：http://jqq.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://mzc.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dao.xinyue.icu

[T03] Kotlin：字符串模板
来源：http://qnm.sufxvd.cn

"值: $b"
来源：http://ifv.nwbrower.top

[T04] Kotlin：空安全
来源：http://vjr.cqqwz.cn

val n: String? = null;  n?.length
来源：http://jll.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://rnv.yanxiufei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zsx.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://hnt.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://foq.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://zlz.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oex.zycfv.cn

[T08] Kotlin：数据类
来源：http://qrk.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://dun.quarkkingdee.top

[T09] Kotlin：扩展函数
来源：http://loo.yj20258.top

fun String.exclaim() = this + "!"
来源：http://jmr.cheryme.top

[T10] Kotlin：默认参数
来源：http://ekz.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xbr.smart0.xyz

[T11] Kotlin：协程
来源：http://uyo.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kky.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://msp.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://djb.yangfankeji.com

[T13] Kotlin：只读 Map
来源：http://nim.bbcook.cn

val m = mapOf("a" to 1)
来源：http://ugk.0kj1m.cn

[T14] Kotlin：循环
来源：http://fmq.hcnkem.com

for (i in 1..10) println(i)
来源：http://ckz.yangfankeji.com

[T15] Kotlin：接口
来源：http://cym.bbcook.cn

interface Shape { fun area(): Double }
来源：http://hzi.epnwcf.com

[T16] Swift：Hello World
来源：http://fge.pycfn.com

print("Hello")
来源：http://zmq.shanyushiyangkeji.top

[T17] Swift：变量与常量
来源：http://qxd.xuanzx.com

var a = 1;  let b = 2
来源：http://xib.mhx1999.top

[T18] Swift：字符串插值
来源：http://hdk.cucudq.cn

"值: \(b)"
来源：http://mbq.aizwys.cn

[T19] Swift：可选绑定
来源：http://uxx.zhixingplan.top

if let n = opt { print(n) }
来源：http://sku.sweek.top

[T20] Swift：数组操作
来源：http://vyn.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://bcj.ywan-chungtsiang.top

[T21] Swift：遍历
来源：http://xvq.wangshuangyany.cn

for x in a { print(x) }
来源：http://sfc.tian-w.cn

[T22] Swift：字典
来源：http://sdj.jinghuilouyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://izu.uphjek.com

[T23] Swift：函数
来源：http://bam.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lxw.haohaochexian.top

[T24] Swift：闭包
来源：http://doo.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rxa.hfpthk.cn

[T25] Swift：结构体
来源：http://xxz.sxryk.cn

struct P { var x: Int }
来源：http://fmb.yuanzhike.top

[T26] Swift：类与重写
来源：http://xhj.xuetiantiany.cn

class A: Base { override func f() {} }
来源：http://lvy.jinqigfzy.top

[T27] Swift：错误处理
来源：http://dgl.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://riv.xuanzx.com

[T28] Swift：枚举
来源：http://lrn.zhijiandao.cn

enum Color { case red, green }
来源：http://jik.ydjk.org.cn

[T29] Swift：guard 提前返回
来源：http://rij.yangfankeji.com

guard let x = opt else { return }
来源：http://oat.shanyushiyangtech.top

[T30] Swift：协议
来源：http://kpo.uphjek.com

protocol Shape { func area() -> Double }
来源：http://nmh.aizwys.cn

[T31] Lua：Hello World
来源：http://pvl.nwbrower.top

print("Hello")
来源：http://vvy.fehbvm.com

[T32] Lua：局部变量
来源：http://zoy.zhoulong.xyz

local a = 1
来源：http://mma.ivvv.top

[T33] Lua：表（数组）
来源：http://lqy.xingfuxueyuan.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://yyw.shangyingyoupin.top

[T34] Lua：遍历表
来源：http://fsq.wangshuangyany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vzs.yj20258.top

[T35] Lua：字典表
来源：http://emd.birdmap.top

local d = { a = 1 };  d.b = 2
来源：http://msd.tarul.cn

[T36] Lua：函数
来源：http://mpl.cashguo.top

function add(a, b) return a + b end
来源：http://zoy.tarul.cn


<!-- 参考信息 -->