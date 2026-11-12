代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pqj.zhongyouzk.top

[R34] 退出时清理
来源：http://mfi.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ujc.pycfn.com

[R35] 后台执行并等待
来源：http://ows.shanyushiyangtech.top

sleep 5 & pid=$!; wait "$pid"
来源：http://iko.jyoumei.cn

[R36] 并发执行多个任务
来源：http://usq.yj202588.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://skv.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://cvl.meibo888.top

files=$(ls -1)
来源：http://dxb.shangyingyoupin.top

[R38] 管道串联
来源：http://gbp.shanyushiyangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://rzi.yonumen.top

[R39] 重定向标准输出与错误
来源：http://xvr.iojbl.cn

cmd > out.log 2>&1
来源：http://doo.nwbrower.top

[R40] 追加写日志
来源：http://gls.redwolf501.top

echo "log" >> out.log
来源：http://pvw.316326.xyz

[R41] 丢弃输出
来源：http://nwu.zycfv.cn

cmd >/dev/null 2>&1
来源：http://qhp.jqgufenzy.top

[R42] 输入重定向
来源：http://cbh.daxiang520.top

wc -l < a.txt
来源：http://hmw.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://dmv.hnxiangtu.top

find . -name "*.log" -type f
来源：http://agk.jianghu66.top

[R44] 按修改时间查找
来源：http://slu.tianlin.xyz

find . -mtime -7 -type f
来源：http://ppb.ywan-chungtsiang.top

[R45] 批量删除
来源：http://mpw.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://wtd.yueranfly.top

[R46] 递归替换文件内容
来源：http://hpr.jinqigufen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ktm.xuanzx.com

[R47] sed 单行替换
来源：http://hdj.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://usr.vqdsnc.cn

[R48] awk 取指定列
来源：http://ajr.cheryme.top

awk '{print $1, $3}' a.txt
来源：http://ezk.hnqzz.top

[R49] awk 带条件
来源：http://qtn.hnqzz.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aqr.dashuyun.cn

[R50] awk 求和
来源：http://acw.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://kdn.chenjidiqi.icu

[R51] 排序去重取前几
来源：http://qnj.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xzp.nwbrower.top

[R52] 统计行数
来源：http://gre.yuanzhike.top

wc -l a.txt
来源：http://dge.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://zwl.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ucq.jinqigufen.top

[R54] 比较两个文件
来源：http://pbb.chenzaomai.com

diff a.txt b.txt
来源：http://vdl.yfazqb.com

[R55] 压缩与解压
来源：http://tdq.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ujh.jqgfzy.top

[R56] 远程拷贝
来源：http://sel.hysaishi.cn

scp file user@host:/path/
来源：http://afj.jlsjyb.cn

[R57] 远程执行命令
来源：http://api.hnxiangtu.top

ssh user@host 'uptime'
来源：http://uhn.bbcook.cn

[R58] 下载文件
来源：http://jzo.chenjidiqi.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qlp.gotoacloud.top

[R59] 发 POST JSON
来源：http://dtw.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yqu.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://ymb.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://izp.yuxming.cn

[R61] 磁盘占用
来源：http://uhy.haohaochexian.top

df -h;  du -sh *
来源：http://wty.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://pkf.yongpay.top

du -ah . | sort -rh | head -10
来源：http://hpm.ydjk.org.cn

[R63] 内存与进程
来源：http://exz.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://qta.redwolf501.top

[R64] 结束进程
来源：http://dhg.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://xlj.pengpengdd.cyou

[R65] 查看端口占用
来源：http://suf.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://csi.hysaishi.cn

[R66] 定时任务
来源：http://yln.cucudq.cn

crontab -e;  crontab -l
来源：http://pcm.guannengcc.top

[R67] 生成随机十六进制串
来源：http://nia.nanxinkj.top

openssl rand -hex 16
来源：http://sjc.haohaochexian.top

[R68] 计算文件校验值
来源：http://gki.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://xcd.yonumen.top

[R69] 生成随机密码
来源：http://nia.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://zzg.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://ccm.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://dsp.yfazqb.com

[R71] 日期格式化
来源：http://sgc.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nbw.hywenlv.cn

[R72] 等待端口就绪
来源：http://nxv.shuidangran.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dzn.yangfankeji.com

[R73] 分割大日志
来源：http://tiw.epnwcf.com

split -l 1000 big.log part_
来源：http://cyo.jiagoushi.top

[R74] 批量重命名
来源：http://htv.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dpv.jiagoushi.top

[R75] 导出环境变量
来源：http://fgd.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://dtq.ydjk.org.cn

[R76] 使用临时文件
来源：http://qco.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ozr.yangfankeji.com

[R77] 读取用户输入
来源：http://jnj.sxryk.cn

read -rp "请输入: " ans
来源：http://prk.nwbrower.top

[R78] 交互式菜单
来源：http://mlb.zhiwuduotai.top

select opt in a b c; do echo "$opt"; break; done
来源：http://azq.zhongyouzk.top

[R79] 解析命令行选项
来源：http://vwh.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://koq.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://kdb.hongshengwenyu.top

time ./run.sh
来源：http://pqq.cdnleiting.top

================================================================================
来源：http://pwo.zhiwuduotai.top

S. C / C++ 专题
来源：http://lfk.hcnkem.com

================================================================================
来源：http://oyy.xinyue.icu

[S01] C：Hello World
来源：http://nzz.hnxiangtu.top

#include <stdio.h>
来源：http://dwn.jiagoushi.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://aka.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://jrp.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://fxl.xziqi.cn

[S03] C：读入整数
来源：http://dic.iojbl.cn

int x; scanf("%d", &x);
来源：http://uns.shzxlz.cn

[S04] C：字符串复制
来源：http://tiw.chenzaomai.com

char dst[32]; strcpy(dst, "hi");
来源：http://rie.jinyuanbaomall.cn

[S05] C：字符串长度
来源：http://xau.cqqwz.cn

strlen(s)
来源：http://dms.quarkkingdee.top

[S06] C：字符串比较
来源：http://hmx.jinqigfzy.top

strcmp(a, b) == 0
来源：http://kef.cucudq.cn

[S07] C：数组遍历求和
来源：http://esm.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rsd.sufxvd.cn

[S08] C：动态内存分配与释放
来源：http://hed.fanxiaobao.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://air.uphjek.com

[S09] C：结构体定义与初始化
来源：http://pky.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jmx.dianchejie.cn

[S10] C：指针与解引用
来源：http://lbz.vehdjk.com

int *p = &a;  *p = 5;
来源：http://baz.gzhubu.top

[S11] C：逐行读文件
来源：http://apw.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "r");
来源：http://mye.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dcd.jinqigfzy.top

fclose(f);
来源：http://xkz.svipenyu.cn

[S12] C：写文件
来源：http://xtu.xinyue.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tda.cucudq.cn

[S13] C：宏定义
来源：http://oso.haohaochexian.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kqb.zhijiandao.cn

[S14] C：枚举
来源：http://yxo.yj20258.top

enum Color { RED, GREEN, BLUE };
来源：http://pxy.jianghu66.top

[S15] C：类型转换
来源：http://vxr.daria6918.cn

(double) a / b
来源：http://rxo.sxryk.cn

[S16] C：位操作置位
来源：http://gie.xziqi.cn

x |= (1 << 3);
来源：http://xwf.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://zwn.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qts.yuanzhike.top

[S18] C：命令行参数
来源：http://dqe.xinyue.icu

int main(int argc, char **argv)
来源：http://wck.gzhubu.top

[S19] C：快速排序
来源：http://eqz.sxryk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pec.nanxuanxn.top

[S20] C：二分查找
来源：http://jbp.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ksn.gzhubu.top

[S21] C：字符类别判断
来源：http://qsn.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://biy.jinghuilouyu.cn

[S22] C：字符串转数字
来源：http://nou.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://ikx.hcnkem.com

[S23] C：随机数
来源：http://wdd.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dax.cheryme.top

[S24] C：获取本地时间
来源：http://rxd.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cuv.meibo888.top

[S25] C：内存拷贝
来源：http://qgc.quarkkingdee.top

memcpy(dst, src, n);
来源：http://isz.yongpay.top

[S26] C：内存清零
来源：http://gip.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://qmv.aibaodan.cn

[S27] C：定义常量
来源：http://sum.316326.xyz

const double PI = 3.14159;
来源：http://vsg.fzhhl.top

[S28] C：静态变量
来源：http://wpe.pengpengdd.cyou

static int counter = 0;
来源：http://ynk.ivvv.top

[S29] C：变参函数
来源：http://jsq.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://veu.yj20258.top

[S30] C：头文件保护
来源：http://ujv.ivvv.top

#ifndef X_H
来源：http://ytu.tarul.cn

#define X_H
来源：http://wlv.yj20258888.top

#endif
来源：http://ull.epnwcf.com

[S31] C++：Hello World
来源：http://ckq.xinyue.icu

#include <iostream>
来源：http://asn.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://ynn.meibo888.top

[S32] C++：字符串
来源：http://gnz.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://mjj.xinyue.icu

[S33] C++：vector 增删
来源：http://jmf.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fck.jyoumei.cn

[S34] C++：遍历 vector
来源：http://pge.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://vtn.cheryme.top

[S35] C++：map
来源：http://qcw.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wzw.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://yza.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pws.zdqjudy.top

[S37] C++：set
来源：http://yrs.andypj.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nsm.fanxiaobao.xyz

[S38] C++：排序
来源：http://rxt.snrcjt.cn

std::sort(v.begin(), v.end());
来源：http://djv.pycfn.com

[S39] C++：自定义比较器排序
来源：http://qab.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rvp.dashuyun.cn

[S40] C++：查找元素
来源：http://ncm.zdqjudy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kjk.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://ffl.yonumen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kli.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://zfq.sweek.top

class B : public Base { public: void f() override {} };
来源：http://ylq.wangdashe.top

[S43] C++：智能指针
来源：http://tzy.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://xjp.fanxiaobao.xyz

[S44] C++：引用传参
来源：http://bih.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://twn.hcnkem.com

[S45] C++：lambda
来源：http://dmw.pycfn.com

auto add = [](int a, int b) { return a + b; };
来源：http://ljk.ydzc1.top

[S46] C++：函数模板
来源：http://klu.pycfn.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uiw.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://ncf.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bma.hesvh.cn

[S48] C++：逐行读文件
来源：http://vwt.aibaodan.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rgx.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://wyz.vehdjk.com

[S49] C++：写文件
来源：http://sjr.sxryk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aie.yangfankeji.com

[S50] C++：格式化数字
来源：http://ykh.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ndm.jiagoushi.top

[S51] C++：显式类型转换
来源：http://nlm.zhongyouzk.top

static_cast<double>(a) / b
来源：http://evt.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://njk.316326.xyz

int size() const noexcept { return n_; }
来源：http://eeu.fehbvm.com

[S53] C++：移动语义
来源：http://jgt.hesvh.cn

std::vector<int> w = std::move(v);
来源：http://pbr.sjlbkw.cn

[S54] C++：异常处理
来源：http://qiv.haohaochexian.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://auu.cheryme.top

[S55] C++：结构化绑定
来源：http://yjj.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://kpm.birdmap.top

[S56] C++：optional
来源：http://fls.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://axt.andypj.xyz

[S57] C++：编译期常量
来源：http://rwe.vqdsnc.cn

constexpr int N = 10;
来源：http://iza.quarkkingdee.top

[S58] C++：命名空间
来源：http://syh.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://wje.hfpthk.cn

[S59] C++：静态断言
来源：http://efh.hesvh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nre.ydzc1.top

[S60] C++：遍历并删除元素
来源：http://pgs.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lid.shangyingyoupin.top

================================================================================
来源：http://npc.sweek.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://usv.xuetiantiany.cn

================================================================================
来源：http://zgt.fzhhl.top

[T01] Kotlin：Hello World
来源：http://vjy.epnwcf.com

println("Hello")
来源：http://pzo.9152youxi.cn

[T02] Kotlin：变量
来源：http://mfn.zycfv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hgr.yongpay.top

[T03] Kotlin：字符串模板
来源：http://apx.yvedp.cn

"值: $b"
来源：http://uhu.jinqigufen.top

[T04] Kotlin：空安全
来源：http://fwv.zycfv.cn

val n: String? = null;  n?.length
来源：http://cmx.tianlin.xyz

[T05] Kotlin：when 表达式
来源：http://nma.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mte.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://lyr.haohaochexian.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hft.cqqwz.cn

[T07] Kotlin：集合过滤
来源：http://zbk.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://xbs.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://ogd.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://ofy.pengpengdd.cyou

[T09] Kotlin：扩展函数
来源：http://jvd.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://mls.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://mrp.jyoumei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wpv.cashguo.top

[T11] Kotlin：协程
来源：http://chh.yfazqb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://wpn.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://akb.bjfxy.top

val (a, b) = Pair(1, 2)
来源：http://bgs.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://fvs.aizwys.cn

val m = mapOf("a" to 1)
来源：http://szu.xylfe.cn

[T14] Kotlin：循环
来源：http://qhc.gaohongyu789.top

for (i in 1..10) println(i)
来源：http://ldy.tanke756.top

[T15] Kotlin：接口
来源：http://czq.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://iec.sweek.top

[T16] Swift：Hello World
来源：http://hme.zhengqikj.top

print("Hello")
来源：http://dcq.pengpengdd.cyou

[T17] Swift：变量与常量
来源：http://qvc.aibaodan.cn

var a = 1;  let b = 2
来源：http://lrc.sxryk.cn

[T18] Swift：字符串插值
来源：http://lto.52xcode.cn

"值: \(b)"
来源：http://ufz.zycfv.cn

[T19] Swift：可选绑定
来源：http://wow.xziqi.cn

if let n = opt { print(n) }
来源：http://gnq.xinyue.icu

[T20] Swift：数组操作
来源：http://juk.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://ogp.zhoulong.xyz

[T21] Swift：遍历
来源：http://ymi.ctjpmb.com

for x in a { print(x) }
来源：http://owl.fktsv.cn

[T22] Swift：字典
来源：http://uyc.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://kby.yj20258.top

[T23] Swift：函数
来源：http://wre.gotoacloud.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wws.cdnleiting.top

[T24] Swift：闭包
来源：http://seu.chenjidiqi.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://vmx.feifeiyinyue.top

[T25] Swift：结构体
来源：http://joi.uphjek.com

struct P { var x: Int }
来源：http://nmf.uphjek.com

[T26] Swift：类与重写
来源：http://yxi.zhixingplan.top

class A: Base { override func f() {} }
来源：http://ddz.xuanzx.com

[T27] Swift：错误处理
来源：http://zge.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://kjk.gotoacloud.top

[T28] Swift：枚举
来源：http://qfc.zhengqikj.top

enum Color { case red, green }
来源：http://woo.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://vnz.dianchejie.cn

guard let x = opt else { return }
来源：http://lmd.xuanzx.com

[T30] Swift：协议
来源：http://ibl.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://qnv.hysaishi.cn

[T31] Lua：Hello World
来源：http://lyn.tarul.cn

print("Hello")
来源：http://nmr.epnwcf.com

[T32] Lua：局部变量
来源：http://cua.sjlbkw.cn

local a = 1
来源：http://lga.sjlbkw.cn

[T33] Lua：表（数组）
来源：http://ngj.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://qsj.xziqi.cn

[T34] Lua：遍历表
来源：http://sij.jinqigufen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rws.sweek.top

[T35] Lua：字典表
来源：http://xlx.bjfxy.top

local d = { a = 1 };  d.b = 2
来源：http://woj.chenjidiqi.icu

[T36] Lua：函数
来源：http://xsg.xingfuxueyuan.xyz

function add(a, b) return a + b end
来源：http://cyg.yvedp.cn


<!-- 参考信息 -->