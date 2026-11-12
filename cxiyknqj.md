代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://bck.shuidangran.top

[R32] 参数个数校验
来源：http://tyg.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zsf.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://mzg.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qnt.cucudq.cn

[R34] 退出时清理
来源：http://sbp.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vph.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://zjn.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bum.zycfv.cn

[R36] 并发执行多个任务
来源：http://nvc.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tsa.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://wjv.yvedp.cn

files=$(ls -1)
来源：http://iei.xuetiantiany.cn

[R38] 管道串联
来源：http://tir.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://laf.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://las.yfazqb.com

cmd > out.log 2>&1
来源：http://ptn.shuidangran.top

[R40] 追加写日志
来源：http://ugj.yj202588.top

echo "log" >> out.log
来源：http://ejt.vehdjk.com

[R41] 丢弃输出
来源：http://mgj.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://yim.chenzaomai.com

[R42] 输入重定向
来源：http://sdn.yuxming.cn

wc -l < a.txt
来源：http://wlh.xziqi.cn

[R43] 按名字查找文件
来源：http://ysg.bbcook.cn

find . -name "*.log" -type f
来源：http://uhb.jyoumei.cn

[R44] 按修改时间查找
来源：http://yew.jqgfzy.top

find . -mtime -7 -type f
来源：http://ghe.hfpthk.cn

[R45] 批量删除
来源：http://uzj.zdbjq.cn

find . -name "*.tmp" -delete
来源：http://bhs.zdqjudy.top

[R46] 递归替换文件内容
来源：http://zsq.dashuyun.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://goz.xuanzx.com

[R47] sed 单行替换
来源：http://mii.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vtw.tian-w.cn

[R48] awk 取指定列
来源：http://rfg.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://omq.yongpay.top

[R49] awk 带条件
来源：http://wns.cucudq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xqq.yvedp.cn

[R50] awk 求和
来源：http://ifl.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://rcc.jinqigfzy.top

[R51] 排序去重取前几
来源：http://sqc.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://sgx.aizwys.cn

[R52] 统计行数
来源：http://rrh.iojbl.cn

wc -l a.txt
来源：http://jwy.52xcode.cn

[R53] 查看文件头与实时尾
来源：http://hjm.sysykeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tky.ctjpmb.com

[R54] 比较两个文件
来源：http://xim.pycfn.com

diff a.txt b.txt
来源：http://iab.fengsongda.top

[R55] 压缩与解压
来源：http://xrz.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ftx.aibaodan.cn

[R56] 远程拷贝
来源：http://wcy.ywan-chungtsiang.top

scp file user@host:/path/
来源：http://rrr.9152youxi.cn

[R57] 远程执行命令
来源：http://pfk.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://tnc.sysykeji.top

[R58] 下载文件
来源：http://sty.shuidangran.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xho.dianchejie.cn

[R59] 发 POST JSON
来源：http://hws.nanxuanxn.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fgq.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://ofw.ywan-chungtsiang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://utp.yangfankeji.com

[R61] 磁盘占用
来源：http://qpl.gzhubu.top

df -h;  du -sh *
来源：http://wcu.52xcode.cn

[R62] 找最占空间的文件
来源：http://skz.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://ztx.jianghu66.top

[R63] 内存与进程
来源：http://prx.bbcook.cn

free -h;  ps aux | grep nginx
来源：http://bcr.cqqwz.cn

[R64] 结束进程
来源：http://ceu.hammf.cn

kill -9 $(pgrep -f app.py)
来源：http://wvw.fengsongda.top

[R65] 查看端口占用
来源：http://gha.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://glp.fzhhl.top

[R66] 定时任务
来源：http://hol.zhengqikj.top

crontab -e;  crontab -l
来源：http://dba.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://lja.sysykeji.top

openssl rand -hex 16
来源：http://sez.havefunace.top

[R68] 计算文件校验值
来源：http://rsk.aizwys.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ydo.xingfuxueyuan.xyz

[R69] 生成随机密码
来源：http://pku.zhiwuduotai.top

head -c 16 /dev/urandom | base64
来源：http://iyo.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://tzi.nwbrower.top

date +%s;  date -d @1700000000
来源：http://qfu.fehbvm.com

[R71] 日期格式化
来源：http://pek.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://gle.quarkkingdee.top

[R72] 等待端口就绪
来源：http://vlr.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://tyh.iojbl.cn

[R73] 分割大日志
来源：http://ttu.ybcxt.top

split -l 1000 big.log part_
来源：http://pkw.yfazqb.com

[R74] 批量重命名
来源：http://wtw.yongpay.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://auw.haohaochexian.top

[R75] 导出环境变量
来源：http://rrz.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://mht.fengsongda.top

[R76] 使用临时文件
来源：http://xef.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dbe.shuidangran.top

[R77] 读取用户输入
来源：http://tpu.sysykeji.top

read -rp "请输入: " ans
来源：http://orv.xuanzx.com

[R78] 交互式菜单
来源：http://kvp.yanxiufei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://foi.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://ijk.dashuyun.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cjr.hnxiangtu.top

[R80] 查看脚本执行耗时
来源：http://dca.fanxiaobao.xyz

time ./run.sh
来源：http://ipa.zhixingplan.top

================================================================================
来源：http://abt.ppjwa.cn

S. C / C++ 专题
来源：http://lll.9152youxi.cn

================================================================================
来源：http://edt.zycfv.cn

[S01] C：Hello World
来源：http://ztw.kuanghao11.cn

#include <stdio.h>
来源：http://kxh.zhongyouzk.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lnf.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://kjl.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://cet.smart0.xyz

[S03] C：读入整数
来源：http://tjy.xinyue.icu

int x; scanf("%d", &x);
来源：http://gul.vehdjk.com

[S04] C：字符串复制
来源：http://lzv.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gdd.yj20258888.top

[S05] C：字符串长度
来源：http://poh.fzhhl.top

strlen(s)
来源：http://zwb.yuanzhike.top

[S06] C：字符串比较
来源：http://ket.cdnleiting.top

strcmp(a, b) == 0
来源：http://zee.uphjek.com

[S07] C：数组遍历求和
来源：http://xwc.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zsi.wangdashe.top

[S08] C：动态内存分配与释放
来源：http://ijb.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jmr.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://osg.sjlbkw.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sav.havefunace.top

[S10] C：指针与解引用
来源：http://jhv.shuidangran.top

int *p = &a;  *p = 5;
来源：http://zyb.yj20258.top

[S11] C：逐行读文件
来源：http://hmz.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "r");
来源：http://klt.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://rjz.xziqi.cn

fclose(f);
来源：http://gqt.vehdjk.com

[S12] C：写文件
来源：http://dte.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ucg.meibo888.top

[S13] C：宏定义
来源：http://rgl.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zgn.sxryk.cn

[S14] C：枚举
来源：http://wuq.gaohongyu789.top

enum Color { RED, GREEN, BLUE };
来源：http://saj.jqgfzy.top

[S15] C：类型转换
来源：http://edn.sweek.top

(double) a / b
来源：http://fpi.cqqwz.cn

[S16] C：位操作置位
来源：http://rku.jyoumei.cn

x |= (1 << 3);
来源：http://rcu.hesvh.cn

[S17] C：安全拼接字符串
来源：http://dcp.hysaishi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vao.hnqzz.top

[S18] C：命令行参数
来源：http://xdi.daria6918.cn

int main(int argc, char **argv)
来源：http://pul.fktsv.cn

[S19] C：快速排序
来源：http://yir.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://dow.redwolf501.top

[S20] C：二分查找
来源：http://zjk.chenzaomai.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://izb.zhongyouzk.top

[S21] C：字符类别判断
来源：http://irv.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lrx.zhoulong.xyz

[S22] C：字符串转数字
来源：http://kni.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bnv.cqqwz.cn

[S23] C：随机数
来源：http://qcu.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zzv.haohaochexian.top

[S24] C：获取本地时间
来源：http://sre.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yqw.9152youxi.cn

[S25] C：内存拷贝
来源：http://jpi.chenzaomai.com

memcpy(dst, src, n);
来源：http://ovq.havefunace.top

[S26] C：内存清零
来源：http://jjy.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://zwu.cucudq.cn

[S27] C：定义常量
来源：http://gco.ywan-chungtsiang.top

const double PI = 3.14159;
来源：http://gvf.fengsongda.top

[S28] C：静态变量
来源：http://qih.hywenlv.cn

static int counter = 0;
来源：http://jwk.jinqigfzy.top

[S29] C：变参函数
来源：http://isk.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vnn.daxiang520.top

[S30] C：头文件保护
来源：http://pby.ivvv.top

#ifndef X_H
来源：http://yyz.svipenyu.cn

#define X_H
来源：http://wet.chenzaomai.com

#endif
来源：http://fmp.yfazqb.com

[S31] C++：Hello World
来源：http://uaj.yangfankeji.com

#include <iostream>
来源：http://tby.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://vug.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://obi.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://opi.hammf.cn

[S33] C++：vector 增删
来源：http://ylo.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yiq.fehbvm.com

[S34] C++：遍历 vector
来源：http://vkv.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://fel.jiagoushi.top

[S35] C++：map
来源：http://ljf.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gvl.fanxiaobao.xyz

[S36] C++：unordered_map
来源：http://hih.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xdx.aizwys.cn

[S37] C++：set
来源：http://vjr.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vlf.nwbrower.top

[S38] C++：排序
来源：http://cbj.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://swv.aizwys.cn

[S39] C++：自定义比较器排序
来源：http://kys.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pft.tian-w.cn

[S40] C++：查找元素
来源：http://ktc.gotoacloud.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lrl.yuxming.cn

[S41] C++：类与构造函数
来源：http://nfm.guannengcc.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pnz.wangshuangyany.cn

[S42] C++：继承与虚函数
来源：http://vbw.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://iie.zhongyouzk.top

[S43] C++：智能指针
来源：http://saj.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://rpb.shzxlz.cn

[S44] C++：引用传参
来源：http://wtu.xylfe.cn

void inc(int &x) { ++x; }
来源：http://aik.zhijiandao.cn

[S45] C++：lambda
来源：http://tmq.xuanzx.com

auto add = [](int a, int b) { return a + b; };
来源：http://bte.jianghu66.top

[S46] C++：函数模板
来源：http://ivv.hcnkem.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://afq.yj202588.top

[S47] C++：结构化绑定遍历
来源：http://hyv.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://snx.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://uxi.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jur.uphjek.com

while (std::getline(in, line)) { }
来源：http://oac.hfpthk.cn

[S49] C++：写文件
来源：http://jia.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tlp.haohaochexian.top

[S50] C++：格式化数字
来源：http://rlk.316326.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fai.hcnkem.com

[S51] C++：显式类型转换
来源：http://mmz.yonumen.top

static_cast<double>(a) / b
来源：http://oba.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://uru.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://dyy.yfazqb.com

[S53] C++：移动语义
来源：http://yya.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://zjy.havefunace.top

[S54] C++：异常处理
来源：http://jel.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gnx.shuidangran.top

[S55] C++：结构化绑定
来源：http://rhn.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rip.yj20258888.top

[S56] C++：optional
来源：http://ryw.yuxming.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cqd.iojbl.cn

[S57] C++：编译期常量
来源：http://qlf.uphjek.com

constexpr int N = 10;
来源：http://tzv.yuxming.cn

[S58] C++：命名空间
来源：http://cci.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://muo.quarkkingdee.top

[S59] C++：静态断言
来源：http://xba.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cpj.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://uif.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ksu.9152youxi.cn

================================================================================
来源：http://jbz.dashuyun.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://juz.ywan-chungtsiang.top

================================================================================
来源：http://brz.daxiang520.top

[T01] Kotlin：Hello World
来源：http://bov.gaohongyu789.top

println("Hello")
来源：http://snf.xuetiantiany.cn

[T02] Kotlin：变量
来源：http://rrh.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jpt.vehdjk.com

[T03] Kotlin：字符串模板
来源：http://yhr.pengpengdd.cyou

"值: $b"
来源：http://gdj.daria6918.cn

[T04] Kotlin：空安全
来源：http://wfq.nwbrower.top

val n: String? = null;  n?.length
来源：http://edf.hywenlv.cn

[T05] Kotlin：when 表达式
来源：http://rrr.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qrm.sysykeji.top

[T06] Kotlin：集合映射
来源：http://mdu.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zjg.yj20258.top

[T07] Kotlin：集合过滤
来源：http://xqt.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://roo.jiagoushi.top

[T08] Kotlin：数据类
来源：http://hux.jinghuilouyu.cn

data class User(val name: String, val age: Int)
来源：http://njs.zycfv.cn

[T09] Kotlin：扩展函数
来源：http://pbo.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://umk.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://zrt.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jag.snrcjt.cn

[T11] Kotlin：协程
来源：http://rle.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jnp.xziqi.cn

[T12] Kotlin：解构声明
来源：http://ike.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://vzn.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://nvh.hcnkem.com

val m = mapOf("a" to 1)
来源：http://klm.ehwqpu.com

[T14] Kotlin：循环
来源：http://jqj.shzxlz.cn

for (i in 1..10) println(i)
来源：http://zal.hywenlv.cn

[T15] Kotlin：接口
来源：http://fqi.jlsjyb.cn

interface Shape { fun area(): Double }
来源：http://kua.ppjwa.cn

[T16] Swift：Hello World
来源：http://cdk.c1oappe.top

print("Hello")
来源：http://ivl.andypj.xyz

[T17] Swift：变量与常量
来源：http://qpf.cdnleiting.top

var a = 1;  let b = 2
来源：http://ihs.haohaochexian.top

[T18] Swift：字符串插值
来源：http://onn.tian-w.cn

"值: \(b)"
来源：http://azx.havefunace.top

[T19] Swift：可选绑定
来源：http://tca.wangdashe.top

if let n = opt { print(n) }
来源：http://izh.cucudq.cn

[T20] Swift：数组操作
来源：http://tzf.zhoulong.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://fbv.nanxinkj.top

[T21] Swift：遍历
来源：http://thi.snrcjt.cn

for x in a { print(x) }
来源：http://ywj.havefunace.top

[T22] Swift：字典
来源：http://kzi.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://lxv.ppjwa.cn

[T23] Swift：函数
来源：http://jyw.quarkkingdee.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://agp.9152youxi.cn

[T24] Swift：闭包
来源：http://prd.cashguo.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sim.tarul.cn

[T25] Swift：结构体
来源：http://dba.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://xle.jinyuanbaomall.cn

[T26] Swift：类与重写
来源：http://emp.meibo888.top

class A: Base { override func f() {} }
来源：http://ati.aizwys.cn

[T27] Swift：错误处理
来源：http://ozd.9152youxi.cn

do { try f() } catch { print(error) }
来源：http://mog.gotoacloud.top

[T28] Swift：枚举
来源：http://cwo.hesvh.cn

enum Color { case red, green }
来源：http://jpy.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://luy.yj20258.top

guard let x = opt else { return }
来源：http://htj.cdnleiting.top

[T30] Swift：协议
来源：http://cvj.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://hgg.sweek.top

[T31] Lua：Hello World
来源：http://kgv.yuxming.cn

print("Hello")
来源：http://pvb.hywenlv.cn

[T32] Lua：局部变量
来源：http://xvo.yongpay.top

local a = 1
来源：http://csw.hysaishi.cn

[T33] Lua：表（数组）
来源：http://tzx.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://hfb.ybcxt.top

[T34] Lua：遍历表
来源：http://qbn.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nzm.yanxiufei.cn


<!-- 参考信息 -->