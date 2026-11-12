代发 wailian999

cmd > out.log 2>&1
来源：http://xyj.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://erw.guowangkeji.top

echo "log" >> out.log
来源：http://hzr.feifeiyinyue.top

[R41] 丢弃输出
来源：http://jcb.sweek.top

cmd >/dev/null 2>&1
来源：http://fee.yuanzhike.top

[R42] 输入重定向
来源：http://uxa.gogol.net.cn

wc -l < a.txt
来源：http://vdr.316326.xyz

[R43] 按名字查找文件
来源：http://gud.xziqi.cn

find . -name "*.log" -type f
来源：http://lhr.yuanzhike.top

[R44] 按修改时间查找
来源：http://lrn.nanxuanxn.top

find . -mtime -7 -type f
来源：http://bpq.daria6918.cn

[R45] 批量删除
来源：http://kzy.sweek.top

find . -name "*.tmp" -delete
来源：http://vdb.guannengcc.top

[R46] 递归替换文件内容
来源：http://mxt.chenlongwang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nbd.zhengqikj.top

[R47] sed 单行替换
来源：http://agw.jyoumei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nzg.andypj.xyz

[R48] awk 取指定列
来源：http://oco.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://pxs.vqdsnc.cn

[R49] awk 带条件
来源：http://tld.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bjp.nanxinkj.top

[R50] awk 求和
来源：http://trw.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://rdp.ydzc1.top

[R51] 排序去重取前几
来源：http://hdv.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mqr.yonumen.top

[R52] 统计行数
来源：http://wfq.sjlbkw.cn

wc -l a.txt
来源：http://jwe.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://ghy.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wih.yangfankeji.com

[R54] 比较两个文件
来源：http://ipd.vqdsnc.cn

diff a.txt b.txt
来源：http://ebs.andypj.xyz

[R55] 压缩与解压
来源：http://gih.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gcn.shuidangran.top

[R56] 远程拷贝
来源：http://djm.sweek.top

scp file user@host:/path/
来源：http://adj.ydjk.org.cn

[R57] 远程执行命令
来源：http://sim.zhixingplan.top

ssh user@host 'uptime'
来源：http://xsm.zhengqikj.top

[R58] 下载文件
来源：http://lcl.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xly.hnqzz.top

[R59] 发 POST JSON
来源：http://rjj.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oxm.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://xbg.gaohongyu789.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lnh.fengsongda.top

[R61] 磁盘占用
来源：http://aeh.chenzaomai.com

df -h;  du -sh *
来源：http://idi.havefunace.top

[R62] 找最占空间的文件
来源：http://puk.hfpthk.cn

du -ah . | sort -rh | head -10
来源：http://iwk.ydjk.org.cn

[R63] 内存与进程
来源：http://fwp.dashuyun.cn

free -h;  ps aux | grep nginx
来源：http://rfd.zhengqikj.top

[R64] 结束进程
来源：http://pct.yj20258.top

kill -9 $(pgrep -f app.py)
来源：http://xoe.hywenlv.cn

[R65] 查看端口占用
来源：http://nwe.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ops.chenzaomai.com

[R66] 定时任务
来源：http://tto.nanxinkj.top

crontab -e;  crontab -l
来源：http://zxs.c1oappe.top

[R67] 生成随机十六进制串
来源：http://kvu.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://amf.kuanghao11.cn

[R68] 计算文件校验值
来源：http://ird.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mfj.sxryk.cn

[R69] 生成随机密码
来源：http://qme.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://gal.zdbjq.cn

[R70] 时间戳与互转
来源：http://aip.yj20258888.top

date +%s;  date -d @1700000000
来源：http://hzy.gaohongyu789.top

[R71] 日期格式化
来源：http://pxl.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://aso.dashuyun.cn

[R72] 等待端口就绪
来源：http://aky.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ahm.ivvv.top

[R73] 分割大日志
来源：http://key.zdqjudy.top

split -l 1000 big.log part_
来源：http://icr.jqgufenzy.top

[R74] 批量重命名
来源：http://mzv.zhixingplan.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rik.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://tvt.hywenlv.cn

export PATH="$HOME/bin:$PATH"
来源：http://ikv.hnxiangtu.top

[R76] 使用临时文件
来源：http://vft.pycfn.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nfv.fktsv.cn

[R77] 读取用户输入
来源：http://mmi.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://nmt.meibo888.top

[R78] 交互式菜单
来源：http://ftn.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hqy.birdmap.top

[R79] 解析命令行选项
来源：http://hsx.zhengqikj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fkx.zdqjudy.top

[R80] 查看脚本执行耗时
来源：http://hkj.hysaishi.cn

time ./run.sh
来源：http://nff.pycfn.com

================================================================================
来源：http://pwq.ydjk.org.cn

S. C / C++ 专题
来源：http://sbl.xingfuxueyuan.xyz

================================================================================
来源：http://gdy.yuxming.cn

[S01] C：Hello World
来源：http://qih.svipenyu.cn

#include <stdio.h>
来源：http://cmp.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wuj.yvedp.cn

[S02] C：变量与格式化输出
来源：http://pry.yj20258888.top

int a = 10; printf("%d\n", a);
来源：http://wgl.sysykeji.top

[S03] C：读入整数
来源：http://kjh.zycfv.cn

int x; scanf("%d", &x);
来源：http://qyr.smart0.xyz

[S04] C：字符串复制
来源：http://wae.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://psx.shangyingyoupin.top

[S05] C：字符串长度
来源：http://age.zhengqikj.top

strlen(s)
来源：http://llr.uphjek.com

[S06] C：字符串比较
来源：http://jit.gogol.net.cn

strcmp(a, b) == 0
来源：http://pvi.hfpthk.cn

[S07] C：数组遍历求和
来源：http://onz.cashguo.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lmm.0kj1m.cn

[S08] C：动态内存分配与释放
来源：http://jhq.hesvh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jbv.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://nyk.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wie.cashguo.top

[S10] C：指针与解引用
来源：http://mzg.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://wtw.9152youxi.cn

[S11] C：逐行读文件
来源：http://ned.9152youxi.cn

FILE *f = fopen("a.txt", "r");
来源：http://pja.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pud.wangdashe.top

fclose(f);
来源：http://cgh.sxryk.cn

[S12] C：写文件
来源：http://vgs.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ati.jinqigufen.top

[S13] C：宏定义
来源：http://jqx.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://edi.shanyushiyangtech.top

[S14] C：枚举
来源：http://ywn.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://nsi.andypj.xyz

[S15] C：类型转换
来源：http://pwr.vehdjk.com

(double) a / b
来源：http://fmo.daria6918.cn

[S16] C：位操作置位
来源：http://fqf.vqdsnc.cn

x |= (1 << 3);
来源：http://fel.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://bfr.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://knc.shuidangran.top

[S18] C：命令行参数
来源：http://jgu.bbcook.cn

int main(int argc, char **argv)
来源：http://oys.ydzc1.top

[S19] C：快速排序
来源：http://aqy.yj20258888.top

qsort(a, n, sizeof(int), cmp);
来源：http://tut.ctjpmb.com

[S20] C：二分查找
来源：http://wut.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sib.gotoacloud.top

[S21] C：字符类别判断
来源：http://zse.haohaochexian.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kuj.tian-w.cn

[S22] C：字符串转数字
来源：http://nnt.hysaishi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nms.birdmap.top

[S23] C：随机数
来源：http://pls.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://smk.tanke756.top

[S24] C：获取本地时间
来源：http://szx.fktsv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zmg.cashguo.top

[S25] C：内存拷贝
来源：http://iwr.pycfn.com

memcpy(dst, src, n);
来源：http://kcw.ydjk.org.cn

[S26] C：内存清零
来源：http://hho.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://cwn.yuanzhike.top

[S27] C：定义常量
来源：http://ull.fzhhl.top

const double PI = 3.14159;
来源：http://mgt.tarul.cn

[S28] C：静态变量
来源：http://rpt.sxryk.cn

static int counter = 0;
来源：http://lhs.hnqzz.top

[S29] C：变参函数
来源：http://sba.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qke.hongshengwenyu.top

[S30] C：头文件保护
来源：http://xwp.ybcxt.top

#ifndef X_H
来源：http://oec.ppjwa.cn

#define X_H
来源：http://qmz.yj20258888.top

#endif
来源：http://ooi.tarul.cn

[S31] C++：Hello World
来源：http://yxy.9152youxi.cn

#include <iostream>
来源：http://wws.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://pam.hysaishi.cn

[S32] C++：字符串
来源：http://xtz.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://xhd.52xcode.cn

[S33] C++：vector 增删
来源：http://vty.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kok.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://krn.cheryme.top

for (auto &x : v) { std::cout << x; }
来源：http://elw.dashuyun.cn

[S35] C++：map
来源：http://oce.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dml.meibo888.top

[S36] C++：unordered_map
来源：http://beh.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kbj.jlsjyb.cn

[S37] C++：set
来源：http://dkz.aibaodan.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ukz.redwolf501.top

[S38] C++：排序
来源：http://wlj.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://hsh.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://fgq.kuanghao11.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nem.ctjpmb.com

[S40] C++：查找元素
来源：http://met.zdqjudy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jch.chenlongwang.top

[S41] C++：类与构造函数
来源：http://mde.dashuyun.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://efa.guannengcc.top

[S42] C++：继承与虚函数
来源：http://ejo.gaohongyu789.top

class B : public Base { public: void f() override {} };
来源：http://wly.nwbrower.top

[S43] C++：智能指针
来源：http://nlc.fktsv.cn

auto p = std::make_unique<int>(5);
来源：http://mom.pengpengdd.cyou

[S44] C++：引用传参
来源：http://usc.sweek.top

void inc(int &x) { ++x; }
来源：http://cka.pycfn.com

[S45] C++：lambda
来源：http://naw.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zod.chenjidiqi.icu

[S46] C++：函数模板
来源：http://vio.quarkkingdee.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eek.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://ofn.yanxiufei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sbd.dianchejie.cn

[S48] C++：逐行读文件
来源：http://kha.hammf.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ynp.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://btt.cheryme.top

[S49] C++：写文件
来源：http://odp.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uxm.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://xoy.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uny.yj20258.top

[S51] C++：显式类型转换
来源：http://bck.nanxuanxn.top

static_cast<double>(a) / b
来源：http://rit.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://vrh.yongpay.top

int size() const noexcept { return n_; }
来源：http://qhf.ppjwa.cn

[S53] C++：移动语义
来源：http://wec.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://asi.tian-w.cn

[S54] C++：异常处理
来源：http://qgn.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dke.snrcjt.cn

[S55] C++：结构化绑定
来源：http://vaf.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://gcf.wangshuangyany.cn

[S56] C++：optional
来源：http://ogb.wangshuangyany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qjj.hcnkem.com

[S57] C++：编译期常量
来源：http://mzh.sufxvd.cn

constexpr int N = 10;
来源：http://sra.hysaishi.cn

[S58] C++：命名空间
来源：http://tlo.zhoulong.xyz

namespace ns { int f() { return 1; } }
来源：http://sqm.vehdjk.com

[S59] C++：静态断言
来源：http://gdz.zhengqikj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://phs.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://dvy.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dox.epnwcf.com

================================================================================
来源：http://acc.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pib.yueranfly.top

================================================================================
来源：http://ptc.havefunace.top

[T01] Kotlin：Hello World
来源：http://uer.yj20258888.top

println("Hello")
来源：http://zbi.xuetiantiany.cn

[T02] Kotlin：变量
来源：http://nqa.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qhp.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://ixg.ehwqpu.com

"值: $b"
来源：http://hjr.yj20258.top

[T04] Kotlin：空安全
来源：http://qjh.iojbl.cn

val n: String? = null;  n?.length
来源：http://tfd.fktsv.cn

[T05] Kotlin：when 表达式
来源：http://eyv.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pva.daria6918.cn

[T06] Kotlin：集合映射
来源：http://vok.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uri.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://hrc.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cmc.nwbrower.top

[T08] Kotlin：数据类
来源：http://tgz.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://uim.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://mix.havefunace.top

fun String.exclaim() = this + "!"
来源：http://pgc.gotoacloud.top

[T10] Kotlin：默认参数
来源：http://uax.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://eht.gzhubu.top

[T11] Kotlin：协程
来源：http://zpz.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://znu.316326.xyz

[T12] Kotlin：解构声明
来源：http://cud.yj20258888.top

val (a, b) = Pair(1, 2)
来源：http://iyp.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://itg.ydjk.org.cn

val m = mapOf("a" to 1)
来源：http://iuq.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://lhy.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://rsi.shangyingyoupin.top

[T15] Kotlin：接口
来源：http://rnp.sweek.top

interface Shape { fun area(): Double }
来源：http://jqz.uphjek.com

[T16] Swift：Hello World
来源：http://xhu.yanxiufei.cn

print("Hello")
来源：http://sir.hammf.cn

[T17] Swift：变量与常量
来源：http://nvh.shuidangran.top

var a = 1;  let b = 2
来源：http://fxu.hesvh.cn

[T18] Swift：字符串插值
来源：http://amm.tarul.cn

"值: \(b)"
来源：http://kev.cdnleiting.top

[T19] Swift：可选绑定
来源：http://tkz.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://cqw.havefunace.top

[T20] Swift：数组操作
来源：http://gly.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://keh.0kj1m.cn

[T21] Swift：遍历
来源：http://iyp.yj202588.top

for x in a { print(x) }
来源：http://xzo.bbcook.cn

[T22] Swift：字典
来源：http://dpd.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://yzq.cqqwz.cn

[T23] Swift：函数
来源：http://qob.hywenlv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gek.hammf.cn

[T24] Swift：闭包
来源：http://vdk.sufxvd.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wzt.daxiang520.top

[T25] Swift：结构体
来源：http://wkr.vehdjk.com

struct P { var x: Int }
来源：http://gtk.cashguo.top

[T26] Swift：类与重写
来源：http://mmp.ybcxt.top

class A: Base { override func f() {} }
来源：http://nsi.yongpay.top

[T27] Swift：错误处理
来源：http://ufg.hnqzz.top

do { try f() } catch { print(error) }
来源：http://bpe.andypj.xyz

[T28] Swift：枚举
来源：http://vjh.yongpay.top

enum Color { case red, green }
来源：http://ufg.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://wpv.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://cqn.dianchejie.cn

[T30] Swift：协议
来源：http://jhs.hnqzz.top

protocol Shape { func area() -> Double }
来源：http://jlr.cucudq.cn

[T31] Lua：Hello World
来源：http://kph.zhongyouzk.top

print("Hello")
来源：http://wie.yvedp.cn

[T32] Lua：局部变量
来源：http://uqa.cucudq.cn

local a = 1
来源：http://nbg.daria6918.cn

[T33] Lua：表（数组）
来源：http://xmy.tian-w.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rgv.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://plq.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fet.uphjek.com

[T35] Lua：字典表
来源：http://mod.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://npl.epnwcf.com

[T36] Lua：函数
来源：http://nkt.fzhhl.top

function add(a, b) return a + b end
来源：http://ggi.uphjek.com

[T37] Lua：字符串拼接
来源：http://jgx.vqdsnc.cn

"a" .. "b"
来源：http://dzw.ivvv.top

[T38] Lua：条件
来源：http://qow.tianlin.xyz

if x > 0 then print("正") end
来源：http://vnw.ybcxt.top

[T39] Lua：模式匹配
来源：http://bmk.yangfankeji.com

string.find(s, "%d+")
来源：http://vzg.fehbvm.com

[T40] Lua：元表
来源：http://tmj.fengsongda.top

setmetatable({}, { __index = base })
来源：http://xqo.jinghuilouyu.cn

[T41] Perl：Hello World
来源：http://hze.guowangkeji.top

print "Hello\n";
来源：http://nhz.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://nsz.tian-w.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bml.c1oappe.top


<!-- 参考信息 -->