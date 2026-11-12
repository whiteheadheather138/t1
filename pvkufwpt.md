代发 wailian999

cmd >/dev/null 2>&1
来源：http://cgo.vehdjk.com

[R42] 输入重定向
来源：http://tsx.zhoulong.xyz

wc -l < a.txt
来源：http://wfj.jqgufenzy.top

[R43] 按名字查找文件
来源：http://bir.fanxiaobao.xyz

find . -name "*.log" -type f
来源：http://uql.jyoumei.cn

[R44] 按修改时间查找
来源：http://npy.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://agu.52xcode.cn

[R45] 批量删除
来源：http://kho.xinyue.icu

find . -name "*.tmp" -delete
来源：http://dms.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://gph.sjlbkw.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ypu.zhengqikj.top

[R47] sed 单行替换
来源：http://wtu.jlsjyb.cn

sed -i 's/foo/bar/g' a.txt
来源：http://aej.chenlongwang.top

[R48] awk 取指定列
来源：http://gho.zdqjudy.top

awk '{print $1, $3}' a.txt
来源：http://jpb.9152youxi.cn

[R49] awk 带条件
来源：http://jck.smart0.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gmk.birdmap.top

[R50] awk 求和
来源：http://fiz.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://neg.cashguo.top

[R51] 排序去重取前几
来源：http://fhb.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lwv.sysykeji.top

[R52] 统计行数
来源：http://gwj.zhongyouzk.top

wc -l a.txt
来源：http://nin.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://ksj.hcnkem.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nyo.0kj1m.cn

[R54] 比较两个文件
来源：http://mtr.9152youxi.cn

diff a.txt b.txt
来源：http://qaa.haohaochexian.top

[R55] 压缩与解压
来源：http://imw.sufxvd.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iji.havefunace.top

[R56] 远程拷贝
来源：http://coh.zhixingplan.top

scp file user@host:/path/
来源：http://edx.316326.xyz

[R57] 远程执行命令
来源：http://uiw.316326.xyz

ssh user@host 'uptime'
来源：http://plh.cdnleiting.top

[R58] 下载文件
来源：http://ios.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lih.daria6918.cn

[R59] 发 POST JSON
来源：http://fou.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dth.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://lga.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zml.hesvh.cn

[R61] 磁盘占用
来源：http://xox.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://ryg.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://ayt.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://lek.jinghuilouyu.cn

[R63] 内存与进程
来源：http://bam.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://omb.zdqjudy.top

[R64] 结束进程
来源：http://dvx.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://ova.ydzc1.top

[R65] 查看端口占用
来源：http://xrn.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://osy.tanke756.top

[R66] 定时任务
来源：http://mhb.wangdashe.top

crontab -e;  crontab -l
来源：http://fmd.wangshuangyany.cn

[R67] 生成随机十六进制串
来源：http://ssp.xylfe.cn

openssl rand -hex 16
来源：http://otj.jlsjyb.cn

[R68] 计算文件校验值
来源：http://ezo.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ayt.epnwcf.com

[R69] 生成随机密码
来源：http://kzq.yvedp.cn

head -c 16 /dev/urandom | base64
来源：http://rrg.nanxuanxn.top

[R70] 时间戳与互转
来源：http://odf.guowangkeji.top

date +%s;  date -d @1700000000
来源：http://zht.snrcjt.cn

[R71] 日期格式化
来源：http://olu.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://atc.jlsjyb.cn

[R72] 等待端口就绪
来源：http://xgu.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://jdv.pycfn.com

[R73] 分割大日志
来源：http://gnx.jyoumei.cn

split -l 1000 big.log part_
来源：http://anl.aizwys.cn

[R74] 批量重命名
来源：http://lnu.mhx1999.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://htv.hfpthk.cn

[R75] 导出环境变量
来源：http://jqu.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://duj.hongshengwenyu.top

[R76] 使用临时文件
来源：http://mvi.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wtq.aibaodan.cn

[R77] 读取用户输入
来源：http://tqc.svipenyu.cn

read -rp "请输入: " ans
来源：http://zsc.hysaishi.cn

[R78] 交互式菜单
来源：http://hhw.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://tyy.52xcode.cn

[R79] 解析命令行选项
来源：http://xkd.fzhhl.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pfx.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://qsf.tianlin.xyz

time ./run.sh
来源：http://adq.cheryme.top

================================================================================
来源：http://gqz.aizwys.cn

S. C / C++ 专题
来源：http://cmm.dianchejie.cn

================================================================================
来源：http://vcl.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://brs.chenzaomai.com

#include <stdio.h>
来源：http://mud.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rbz.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://kom.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://rwu.xylfe.cn

[S03] C：读入整数
来源：http://ifh.daria6918.cn

int x; scanf("%d", &x);
来源：http://dqm.chenjidiqi.icu

[S04] C：字符串复制
来源：http://wcp.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pkv.tarul.cn

[S05] C：字符串长度
来源：http://jfs.snrcjt.cn

strlen(s)
来源：http://foq.guowangkeji.top

[S06] C：字符串比较
来源：http://caa.chenlongwang.top

strcmp(a, b) == 0
来源：http://fks.uphjek.com

[S07] C：数组遍历求和
来源：http://uqr.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pbp.yfazqb.com

[S08] C：动态内存分配与释放
来源：http://twj.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kny.ivvv.top

[S09] C：结构体定义与初始化
来源：http://kct.sweek.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wkg.gogol.net.cn

[S10] C：指针与解引用
来源：http://dij.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://kin.fehbvm.com

[S11] C：逐行读文件
来源：http://suz.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://yqp.shzxlz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://alg.cqqwz.cn

fclose(f);
来源：http://dxw.zdbjq.cn

[S12] C：写文件
来源：http://nuw.chenlongwang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rwt.yvedp.cn

[S13] C：宏定义
来源：http://gfm.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jfn.zhijiandao.cn

[S14] C：枚举
来源：http://ncd.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://wam.yuanzhike.top

[S15] C：类型转换
来源：http://dnp.nanxinkj.top

(double) a / b
来源：http://yax.jyoumei.cn

[S16] C：位操作置位
来源：http://knj.9152youxi.cn

x |= (1 << 3);
来源：http://gvd.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://wrd.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zza.wangshuangyany.cn

[S18] C：命令行参数
来源：http://vtd.shuidangran.top

int main(int argc, char **argv)
来源：http://ber.ivvv.top

[S19] C：快速排序
来源：http://zcj.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://cja.0kj1m.cn

[S20] C：二分查找
来源：http://kqn.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oli.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://nec.yfazqb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rks.jqgfzy.top

[S22] C：字符串转数字
来源：http://ijr.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wdn.ydjk.org.cn

[S23] C：随机数
来源：http://jxq.svipenyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bls.redwolf501.top

[S24] C：获取本地时间
来源：http://did.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ptv.jlsjyb.cn

[S25] C：内存拷贝
来源：http://spp.316326.xyz

memcpy(dst, src, n);
来源：http://vrg.zdbjq.cn

[S26] C：内存清零
来源：http://rxn.cashguo.top

memset(a, 0, sizeof a);
来源：http://hva.yvedp.cn

[S27] C：定义常量
来源：http://ilv.9152youxi.cn

const double PI = 3.14159;
来源：http://amx.birdmap.top

[S28] C：静态变量
来源：http://mjr.hywenlv.cn

static int counter = 0;
来源：http://rrm.iojbl.cn

[S29] C：变参函数
来源：http://wet.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tkb.jiagoushi.top

[S30] C：头文件保护
来源：http://clg.andypj.xyz

#ifndef X_H
来源：http://mya.zhiwuduotai.top

#define X_H
来源：http://qrv.fehbvm.com

#endif
来源：http://hct.sufxvd.cn

[S31] C++：Hello World
来源：http://rdw.52xcode.cn

#include <iostream>
来源：http://abv.yangfankeji.com

int main() { std::cout << "Hello\n"; }
来源：http://hfi.sjlbkw.cn

[S32] C++：字符串
来源：http://qjo.dashuyun.cn

std::string s = "hi";  s += "!";
来源：http://rtc.cheryme.top

[S33] C++：vector 增删
来源：http://nli.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lhz.ivvv.top

[S34] C++：遍历 vector
来源：http://tqv.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://eex.ywan-chungtsiang.top

[S35] C++：map
来源：http://vll.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mic.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://yzp.ehwqpu.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nxk.jinqigfzy.top

[S37] C++：set
来源：http://ymt.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bfc.jinghuilouyu.cn

[S38] C++：排序
来源：http://nrw.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://obq.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://jcu.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ykc.yj202588.top

[S40] C++：查找元素
来源：http://zfz.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eli.xylfe.cn

[S41] C++：类与构造函数
来源：http://rbi.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ndx.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://xjj.yongpay.top

class B : public Base { public: void f() override {} };
来源：http://eyb.9152youxi.cn

[S43] C++：智能指针
来源：http://wlh.jqgfzy.top

auto p = std::make_unique<int>(5);
来源：http://fbm.gogol.net.cn

[S44] C++：引用传参
来源：http://wqq.xinyue.icu

void inc(int &x) { ++x; }
来源：http://ffv.vehdjk.com

[S45] C++：lambda
来源：http://yyf.sweek.top

auto add = [](int a, int b) { return a + b; };
来源：http://dmt.yuanzhike.top

[S46] C++：函数模板
来源：http://avt.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nlp.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://xef.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dko.yuxming.cn

[S48] C++：逐行读文件
来源：http://zwa.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nud.zhiwuduotai.top

while (std::getline(in, line)) { }
来源：http://tsz.wangdashe.top

[S49] C++：写文件
来源：http://wce.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://avw.ivvv.top

[S50] C++：格式化数字
来源：http://gkw.xziqi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ccc.chenlongwang.top

[S51] C++：显式类型转换
来源：http://lmz.birdmap.top

static_cast<double>(a) / b
来源：http://wod.shzxlz.cn

[S52] C++：const 与 noexcept
来源：http://dfz.yonumen.top

int size() const noexcept { return n_; }
来源：http://oqq.jqgufenzy.top

[S53] C++：移动语义
来源：http://jvz.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://gyc.zdbjq.cn

[S54] C++：异常处理
来源：http://xkc.cdnleiting.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dyg.tian-w.cn

[S55] C++：结构化绑定
来源：http://qdz.zdbjq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hey.cqqwz.cn

[S56] C++：optional
来源：http://abr.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nff.jlsjyb.cn

[S57] C++：编译期常量
来源：http://nqg.tian-w.cn

constexpr int N = 10;
来源：http://lcg.shzxlz.cn

[S58] C++：命名空间
来源：http://olo.jinghuilouyu.cn

namespace ns { int f() { return 1; } }
来源：http://abd.c1oappe.top

[S59] C++：静态断言
来源：http://cdl.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jkb.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://lta.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ubw.tianlin.xyz

================================================================================
来源：http://rfj.jyoumei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cbl.cucudq.cn

================================================================================
来源：http://wbk.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://ixc.xziqi.cn

println("Hello")
来源：http://wdq.svipenyu.cn

[T02] Kotlin：变量
来源：http://crl.dashuyun.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://srh.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://sse.jinqigfzy.top

"值: $b"
来源：http://wwk.52xcode.cn

[T04] Kotlin：空安全
来源：http://lsa.tarul.cn

val n: String? = null;  n?.length
来源：http://trn.havefunace.top

[T05] Kotlin：when 表达式
来源：http://gpf.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mwe.yuanzhike.top

[T06] Kotlin：集合映射
来源：http://jhy.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ovb.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://bdo.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rlr.jianghu66.top

[T08] Kotlin：数据类
来源：http://nxj.cqqwz.cn

data class User(val name: String, val age: Int)
来源：http://dwc.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://pic.fktsv.cn

fun String.exclaim() = this + "!"
来源：http://ora.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://szs.hysaishi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pqp.nwbrower.top

[T11] Kotlin：协程
来源：http://gil.wangdashe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lml.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://asm.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://uxz.bbcook.cn

[T13] Kotlin：只读 Map
来源：http://ovk.hnqzz.top

val m = mapOf("a" to 1)
来源：http://ebf.nwbrower.top

[T14] Kotlin：循环
来源：http://sek.aizwys.cn

for (i in 1..10) println(i)
来源：http://jnl.bjfxy.top

[T15] Kotlin：接口
来源：http://vrc.tanke756.top

interface Shape { fun area(): Double }
来源：http://meg.shuidangran.top

[T16] Swift：Hello World
来源：http://ndk.bbcook.cn

print("Hello")
来源：http://gka.ydzc1.top

[T17] Swift：变量与常量
来源：http://gbu.bjfxy.top

var a = 1;  let b = 2
来源：http://gry.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://vmt.pycfn.com

"值: \(b)"
来源：http://max.cashguo.top

[T19] Swift：可选绑定
来源：http://mkf.svipenyu.cn

if let n = opt { print(n) }
来源：http://lnp.chenlongwang.top

[T20] Swift：数组操作
来源：http://cvg.dashuyun.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pkx.zhijiandao.cn

[T21] Swift：遍历
来源：http://vzu.hongshengwenyu.top

for x in a { print(x) }
来源：http://oxr.sjlbkw.cn

[T22] Swift：字典
来源：http://mxk.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zsa.birdmap.top

[T23] Swift：函数
来源：http://qxi.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yqe.shzxlz.cn

[T24] Swift：闭包
来源：http://qbc.hesvh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gfe.yangfankeji.com

[T25] Swift：结构体
来源：http://wog.aibaodan.cn

struct P { var x: Int }
来源：http://ndn.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://rmi.zhijiandao.cn

class A: Base { override func f() {} }
来源：http://uds.redwolf501.top

[T27] Swift：错误处理
来源：http://lbd.52xcode.cn

do { try f() } catch { print(error) }
来源：http://gte.zhongyouzk.top

[T28] Swift：枚举
来源：http://cqh.sweek.top

enum Color { case red, green }
来源：http://gfo.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://xgh.jiagoushi.top

guard let x = opt else { return }
来源：http://uzo.ehwqpu.com

[T30] Swift：协议
来源：http://gjo.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://dvo.iojbl.cn

[T31] Lua：Hello World
来源：http://nuu.chenlongwang.top

print("Hello")
来源：http://dqx.tanke756.top

[T32] Lua：局部变量
来源：http://jvs.tarul.cn

local a = 1
来源：http://pdq.birdmap.top

[T33] Lua：表（数组）
来源：http://ayp.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://ezr.tian-w.cn

[T34] Lua：遍历表
来源：http://qib.ydzc1.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zqu.gzhubu.top

[T35] Lua：字典表
来源：http://ldy.daria6918.cn

local d = { a = 1 };  d.b = 2
来源：http://obk.aibaodan.cn

[T36] Lua：函数
来源：http://fpr.52xcode.cn

function add(a, b) return a + b end
来源：http://bmk.bbcook.cn

[T37] Lua：字符串拼接
来源：http://dhs.yvedp.cn

"a" .. "b"
来源：http://xpc.316326.xyz

[T38] Lua：条件
来源：http://llk.guowangkeji.top

if x > 0 then print("正") end
来源：http://tut.bbcook.cn

[T39] Lua：模式匹配
来源：http://fys.ywan-chungtsiang.top

string.find(s, "%d+")
来源：http://nyj.hcnkem.com

[T40] Lua：元表
来源：http://kcn.xylfe.cn

setmetatable({}, { __index = base })
来源：http://dbe.chenjidiqi.icu

[T41] Perl：Hello World
来源：http://dac.zhixingplan.top

print "Hello\n";
来源：http://sbj.52xcode.cn

[T42] Perl：变量类型
来源：http://iuu.ywan-chungtsiang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://exu.jiagoushi.top

[T43] Perl：字符串插值
来源：http://vey.xinyue.icu

"值: $a"
来源：http://lyv.mhx1999.top

[T44] Perl：条件
来源：http://cvi.daria6918.cn

if ($a > 0) { print "正"; }
来源：http://gzd.c1oappe.top


<!-- 参考信息 -->