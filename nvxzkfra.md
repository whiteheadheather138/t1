代发 wailian999

find . -name "*.log" -type f
来源：http://otg.kuanghao11.cn

[R44] 按修改时间查找
来源：http://amo.ehwqpu.com

find . -mtime -7 -type f
来源：http://vyr.hammf.cn

[R45] 批量删除
来源：http://jot.bjfxy.top

find . -name "*.tmp" -delete
来源：http://vec.aibaodan.cn

[R46] 递归替换文件内容
来源：http://sva.shzxlz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qbw.gaohongyu789.top

[R47] sed 单行替换
来源：http://puk.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://tte.gaohongyu789.top

[R48] awk 取指定列
来源：http://dkd.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://ahu.xinyue.icu

[R49] awk 带条件
来源：http://vnd.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mgu.kuanghao11.cn

[R50] awk 求和
来源：http://trm.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qzn.gogol.net.cn

[R51] 排序去重取前几
来源：http://upz.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ian.shzxlz.cn

[R52] 统计行数
来源：http://wmd.fktsv.cn

wc -l a.txt
来源：http://lpo.epnwcf.com

[R53] 查看文件头与实时尾
来源：http://vqo.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ovh.zdbjq.cn

[R54] 比较两个文件
来源：http://aqc.nanxuanxn.top

diff a.txt b.txt
来源：http://lvp.tianlin.xyz

[R55] 压缩与解压
来源：http://bxh.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eii.gaohongyu789.top

[R56] 远程拷贝
来源：http://otu.cashguo.top

scp file user@host:/path/
来源：http://qzv.zhiwuduotai.top

[R57] 远程执行命令
来源：http://iuw.jlsjyb.cn

ssh user@host 'uptime'
来源：http://xsb.havefunace.top

[R58] 下载文件
来源：http://qzy.ivvv.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gwg.0kj1m.cn

[R59] 发 POST JSON
来源：http://xug.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rav.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://gtj.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vjs.nanxuanxn.top

[R61] 磁盘占用
来源：http://vyk.wangdashe.top

df -h;  du -sh *
来源：http://kuc.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://dpo.cqqwz.cn

du -ah . | sort -rh | head -10
来源：http://pna.dashuyun.cn

[R63] 内存与进程
来源：http://nyf.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://odv.316326.xyz

[R64] 结束进程
来源：http://qkz.havefunace.top

kill -9 $(pgrep -f app.py)
来源：http://npw.epnwcf.com

[R65] 查看端口占用
来源：http://ctt.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pmn.jqgufenzy.top

[R66] 定时任务
来源：http://uxs.ctjpmb.com

crontab -e;  crontab -l
来源：http://jid.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://xvr.shzxlz.cn

openssl rand -hex 16
来源：http://dnl.sufxvd.cn

[R68] 计算文件校验值
来源：http://fyb.fktsv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qej.xylfe.cn

[R69] 生成随机密码
来源：http://bze.andypj.xyz

head -c 16 /dev/urandom | base64
来源：http://ueu.tarul.cn

[R70] 时间戳与互转
来源：http://des.yuanzhike.top

date +%s;  date -d @1700000000
来源：http://pgz.jyoumei.cn

[R71] 日期格式化
来源：http://xas.vqdsnc.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vvb.sysykeji.top

[R72] 等待端口就绪
来源：http://vpx.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ezu.gaohongyu789.top

[R73] 分割大日志
来源：http://iar.zhoulong.xyz

split -l 1000 big.log part_
来源：http://yea.epnwcf.com

[R74] 批量重命名
来源：http://nhk.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eje.haohaochexian.top

[R75] 导出环境变量
来源：http://xfk.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://ebr.shanyushiyangkeji.top

[R76] 使用临时文件
来源：http://qvb.ybcxt.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tlt.zhixingplan.top

[R77] 读取用户输入
来源：http://ima.fktsv.cn

read -rp "请输入: " ans
来源：http://hvb.yueranfly.top

[R78] 交互式菜单
来源：http://hjt.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://wqd.52xcode.cn

[R79] 解析命令行选项
来源：http://ahj.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yyy.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://jhn.yuxming.cn

time ./run.sh
来源：http://how.sjlbkw.cn

================================================================================
来源：http://usl.yonumen.top

S. C / C++ 专题
来源：http://hfn.ctjpmb.com

================================================================================
来源：http://jvp.kuanghao11.cn

[S01] C：Hello World
来源：http://msq.9152youxi.cn

#include <stdio.h>
来源：http://ska.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ajz.uphjek.com

[S02] C：变量与格式化输出
来源：http://bdh.0kj1m.cn

int a = 10; printf("%d\n", a);
来源：http://pqo.yonumen.top

[S03] C：读入整数
来源：http://cgr.svipenyu.cn

int x; scanf("%d", &x);
来源：http://ino.jqgfzy.top

[S04] C：字符串复制
来源：http://daa.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://nna.gzhubu.top

[S05] C：字符串长度
来源：http://sbj.vehdjk.com

strlen(s)
来源：http://bfc.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://djm.tian-w.cn

strcmp(a, b) == 0
来源：http://ljt.snrcjt.cn

[S07] C：数组遍历求和
来源：http://kje.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zbg.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://qea.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zxa.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://zyb.yvedp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tlo.shzxlz.cn

[S10] C：指针与解引用
来源：http://fim.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://zyg.jinqigfzy.top

[S11] C：逐行读文件
来源：http://tgt.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://cjr.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tyh.wangdashe.top

fclose(f);
来源：http://qto.wangshuangyany.cn

[S12] C：写文件
来源：http://him.tianlin.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uah.guowangkeji.top

[S13] C：宏定义
来源：http://lwy.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jju.wangshuangyany.cn

[S14] C：枚举
来源：http://wok.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://jnh.shanyushiyangkeji.top

[S15] C：类型转换
来源：http://stl.chenjidiqi.icu

(double) a / b
来源：http://tjg.shangyingyoupin.top

[S16] C：位操作置位
来源：http://hux.hfpthk.cn

x |= (1 << 3);
来源：http://jva.sxryk.cn

[S17] C：安全拼接字符串
来源：http://tpp.redwolf501.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sxb.zhongyouzk.top

[S18] C：命令行参数
来源：http://lik.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://zmr.0kj1m.cn

[S19] C：快速排序
来源：http://zda.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yhf.yanxiufei.cn

[S20] C：二分查找
来源：http://utr.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bfz.guannengcc.top

[S21] C：字符类别判断
来源：http://wdt.svipenyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nda.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://pbv.zhoulong.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://jyw.cqqwz.cn

[S23] C：随机数
来源：http://nfm.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://mec.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://vjz.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://egd.jqgufenzy.top

[S25] C：内存拷贝
来源：http://tfc.wangdashe.top

memcpy(dst, src, n);
来源：http://cms.wangshuangyany.cn

[S26] C：内存清零
来源：http://dtw.cucudq.cn

memset(a, 0, sizeof a);
来源：http://sen.nanxuanxn.top

[S27] C：定义常量
来源：http://uah.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://qwz.316326.xyz

[S28] C：静态变量
来源：http://bxi.yj20258888.top

static int counter = 0;
来源：http://abu.wangshuangyany.cn

[S29] C：变参函数
来源：http://lbm.shzxlz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://phb.ydzc1.top

[S30] C：头文件保护
来源：http://giu.vqdsnc.cn

#ifndef X_H
来源：http://sxq.vqdsnc.cn

#define X_H
来源：http://zed.ivvv.top

#endif
来源：http://prh.hesvh.cn

[S31] C++：Hello World
来源：http://uwo.chenzaomai.com

#include <iostream>
来源：http://alp.gaohongyu789.top

int main() { std::cout << "Hello\n"; }
来源：http://fqf.gotoacloud.top

[S32] C++：字符串
来源：http://mrq.hammf.cn

std::string s = "hi";  s += "!";
来源：http://wsh.ybcxt.top

[S33] C++：vector 增删
来源：http://ric.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ggd.jianghu66.top

[S34] C++：遍历 vector
来源：http://bpk.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://izp.yuanzhike.top

[S35] C++：map
来源：http://mfv.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ppb.nanxuanxn.top

[S36] C++：unordered_map
来源：http://vod.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qxt.shanyushiyangtech.top

[S37] C++：set
来源：http://azp.meibo888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tkf.iojbl.cn

[S38] C++：排序
来源：http://qdx.jqgfzy.top

std::sort(v.begin(), v.end());
来源：http://gaq.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://fjd.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qhm.gaohongyu789.top

[S40] C++：查找元素
来源：http://kxx.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pez.yvedp.cn

[S41] C++：类与构造函数
来源：http://gla.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xwk.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://rhg.yvedp.cn

class B : public Base { public: void f() override {} };
来源：http://xxt.fzhhl.top

[S43] C++：智能指针
来源：http://ihl.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://jke.jinqigfzy.top

[S44] C++：引用传参
来源：http://quz.wangdashe.top

void inc(int &x) { ++x; }
来源：http://buc.cqqwz.cn

[S45] C++：lambda
来源：http://hvr.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://vhp.fktsv.cn

[S46] C++：函数模板
来源：http://gyl.andypj.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yev.hnqzz.top

[S47] C++：结构化绑定遍历
来源：http://brp.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cxd.tarul.cn

[S48] C++：逐行读文件
来源：http://kao.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://qyk.haohaochexian.top

while (std::getline(in, line)) { }
来源：http://jpi.pengpengdd.cyou

[S49] C++：写文件
来源：http://cxh.chenzaomai.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rqa.dashuyun.cn

[S50] C++：格式化数字
来源：http://hmw.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tzr.fzhhl.top

[S51] C++：显式类型转换
来源：http://jyg.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://beo.snrcjt.cn

[S52] C++：const 与 noexcept
来源：http://jrp.jqgufenzy.top

int size() const noexcept { return n_; }
来源：http://yyn.uphjek.com

[S53] C++：移动语义
来源：http://hpk.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://lxt.hesvh.cn

[S54] C++：异常处理
来源：http://drh.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qyk.chenzaomai.com

[S55] C++：结构化绑定
来源：http://mpx.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://whh.birdmap.top

[S56] C++：optional
来源：http://kvp.yangfankeji.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kjm.haohaochexian.top

[S57] C++：编译期常量
来源：http://gtp.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://ggu.ybcxt.top

[S58] C++：命名空间
来源：http://hni.nanxuanxn.top

namespace ns { int f() { return 1; } }
来源：http://tgv.uphjek.com

[S59] C++：静态断言
来源：http://spo.jinqigufen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dtf.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://hsj.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ejb.andypj.xyz

================================================================================
来源：http://luu.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ugd.nwbrower.top

================================================================================
来源：http://atg.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://dcc.jqgfzy.top

println("Hello")
来源：http://sld.jyoumei.cn

[T02] Kotlin：变量
来源：http://ntb.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cal.hywenlv.cn

[T03] Kotlin：字符串模板
来源：http://gvu.c1oappe.top

"值: $b"
来源：http://ihv.yj202588.top

[T04] Kotlin：空安全
来源：http://bmx.aizwys.cn

val n: String? = null;  n?.length
来源：http://phm.pycfn.com

[T05] Kotlin：when 表达式
来源：http://hqo.epnwcf.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rpo.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://hnj.ywan-chungtsiang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://glq.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://evp.shanyushiyangtech.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jhr.daxiang520.top

[T08] Kotlin：数据类
来源：http://nut.sweek.top

data class User(val name: String, val age: Int)
来源：http://zey.uphjek.com

[T09] Kotlin：扩展函数
来源：http://gjt.tanke756.top

fun String.exclaim() = this + "!"
来源：http://xua.yj20258.top

[T10] Kotlin：默认参数
来源：http://icl.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kzd.daria6918.cn

[T11] Kotlin：协程
来源：http://vjj.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://flr.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://tug.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://cgq.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://mon.cucudq.cn

val m = mapOf("a" to 1)
来源：http://cic.jyoumei.cn

[T14] Kotlin：循环
来源：http://wpc.cheryme.top

for (i in 1..10) println(i)
来源：http://kus.52xcode.cn

[T15] Kotlin：接口
来源：http://vtu.meibo888.top

interface Shape { fun area(): Double }
来源：http://fwx.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://ovz.nanxinkj.top

print("Hello")
来源：http://vpi.ehwqpu.com

[T17] Swift：变量与常量
来源：http://wjf.fehbvm.com

var a = 1;  let b = 2
来源：http://bbi.sxryk.cn

[T18] Swift：字符串插值
来源：http://ygx.zycfv.cn

"值: \(b)"
来源：http://dgg.jlsjyb.cn

[T19] Swift：可选绑定
来源：http://idf.andypj.xyz

if let n = opt { print(n) }
来源：http://sqe.gogol.net.cn

[T20] Swift：数组操作
来源：http://ray.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://ors.jiagoushi.top

[T21] Swift：遍历
来源：http://rhq.svipenyu.cn

for x in a { print(x) }
来源：http://jix.jinqigufen.top

[T22] Swift：字典
来源：http://ufh.shzxlz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vce.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://clb.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yvi.hcnkem.com

[T24] Swift：闭包
来源：http://agi.jianghu66.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://oli.gogol.net.cn

[T25] Swift：结构体
来源：http://xha.meibo888.top

struct P { var x: Int }
来源：http://nwo.cdnleiting.top

[T26] Swift：类与重写
来源：http://nci.jqgufenzy.top

class A: Base { override func f() {} }
来源：http://rah.zhongyouzk.top

[T27] Swift：错误处理
来源：http://nyt.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://nov.52xcode.cn

[T28] Swift：枚举
来源：http://rja.jinyuanbaomall.cn

enum Color { case red, green }
来源：http://osd.ivvv.top

[T29] Swift：guard 提前返回
来源：http://qsz.hnqzz.top

guard let x = opt else { return }
来源：http://hut.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://dmv.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://das.yuanzhike.top

[T31] Lua：Hello World
来源：http://lgx.sxryk.cn

print("Hello")
来源：http://nsm.birdmap.top

[T32] Lua：局部变量
来源：http://lwb.hnqzz.top

local a = 1
来源：http://bow.zdqjudy.top

[T33] Lua：表（数组）
来源：http://whj.hammf.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://eyu.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://csa.jqgufenzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pmy.dianchejie.cn

[T35] Lua：字典表
来源：http://dme.cheryme.top

local d = { a = 1 };  d.b = 2
来源：http://roh.gaohongyu789.top

[T36] Lua：函数
来源：http://gly.snrcjt.cn

function add(a, b) return a + b end
来源：http://wjh.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://yoz.pycfn.com

"a" .. "b"
来源：http://yop.ppjwa.cn

[T38] Lua：条件
来源：http://rvh.zdbjq.cn

if x > 0 then print("正") end
来源：http://gyu.zhaomingkeji.xyz

[T39] Lua：模式匹配
来源：http://ncx.pengpengdd.cyou

string.find(s, "%d+")
来源：http://mtt.guannengcc.top

[T40] Lua：元表
来源：http://gnd.iojbl.cn

setmetatable({}, { __index = base })
来源：http://ahv.aibaodan.cn

[T41] Perl：Hello World
来源：http://wsm.dashuyun.cn

print "Hello\n";
来源：http://vtq.chenzaomai.com

[T42] Perl：变量类型
来源：http://cqa.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zia.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://gde.jiagoushi.top

"值: $a"
来源：http://znz.fktsv.cn

[T44] Perl：条件
来源：http://rqt.gotoacloud.top

if ($a > 0) { print "正"; }
来源：http://stz.bjfxy.top

[T45] Perl：数组遍历
来源：http://mqd.xingfuxueyuan.xyz

for my $x (@arr) { print $x; }
来源：http://yzf.cdnleiting.top

[T46] Perl：哈希操作
来源：http://zjk.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dja.c1oappe.top


<!-- 参考信息 -->