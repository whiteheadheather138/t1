代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://ulz.9152youxi.cn

[R36] 并发执行多个任务
来源：http://ekv.ydjk.org.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kon.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://tne.9152youxi.cn

files=$(ls -1)
来源：http://mda.ydjk.org.cn

[R38] 管道串联
来源：http://bps.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://iug.zhoulong.xyz

[R39] 重定向标准输出与错误
来源：http://ors.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://hyp.fktsv.cn

[R40] 追加写日志
来源：http://ijq.gaohongyu789.top

echo "log" >> out.log
来源：http://gqn.hammf.cn

[R41] 丢弃输出
来源：http://zud.hfpthk.cn

cmd >/dev/null 2>&1
来源：http://dgp.meibo888.top

[R42] 输入重定向
来源：http://ovc.epnwcf.com

wc -l < a.txt
来源：http://qes.zhixingplan.top

[R43] 按名字查找文件
来源：http://gjm.shuidangran.top

find . -name "*.log" -type f
来源：http://zlx.daxiang520.top

[R44] 按修改时间查找
来源：http://gnl.ivvv.top

find . -mtime -7 -type f
来源：http://utr.fzhhl.top

[R45] 批量删除
来源：http://fgk.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://vbs.gogol.net.cn

[R46] 递归替换文件内容
来源：http://ucy.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xtq.ctjpmb.com

[R47] sed 单行替换
来源：http://pht.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hbk.yvedp.cn

[R48] awk 取指定列
来源：http://xic.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://cez.sysykeji.top

[R49] awk 带条件
来源：http://fmj.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ojj.yvedp.cn

[R50] awk 求和
来源：http://hkg.yongpay.top

awk '{s += $2} END {print s}' a.txt
来源：http://lfg.bjfxy.top

[R51] 排序去重取前几
来源：http://ygb.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://nzs.fktsv.cn

[R52] 统计行数
来源：http://hfo.yonumen.top

wc -l a.txt
来源：http://mrp.tianlin.xyz

[R53] 查看文件头与实时尾
来源：http://rwp.yuxming.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dsn.xylfe.cn

[R54] 比较两个文件
来源：http://ixd.nwbrower.top

diff a.txt b.txt
来源：http://zjx.iojbl.cn

[R55] 压缩与解压
来源：http://cfl.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hen.pycfn.com

[R56] 远程拷贝
来源：http://fnj.hnxiangtu.top

scp file user@host:/path/
来源：http://jyy.epnwcf.com

[R57] 远程执行命令
来源：http://ksd.hcnkem.com

ssh user@host 'uptime'
来源：http://qnv.hammf.cn

[R58] 下载文件
来源：http://ipy.andypj.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tfl.wangshuangyany.cn

[R59] 发 POST JSON
来源：http://sub.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ile.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://hmx.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xxq.xuanzx.com

[R61] 磁盘占用
来源：http://pfk.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://fdw.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://rap.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://eva.yueranfly.top

[R63] 内存与进程
来源：http://vlv.ehwqpu.com

free -h;  ps aux | grep nginx
来源：http://wby.ppjwa.cn

[R64] 结束进程
来源：http://niu.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://dlp.iojbl.cn

[R65] 查看端口占用
来源：http://huk.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qlz.0kj1m.cn

[R66] 定时任务
来源：http://vpm.iojbl.cn

crontab -e;  crontab -l
来源：http://alb.hcnkem.com

[R67] 生成随机十六进制串
来源：http://ifo.zhoulong.xyz

openssl rand -hex 16
来源：http://zrb.c1oappe.top

[R68] 计算文件校验值
来源：http://abv.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://aeu.tianlin.xyz

[R69] 生成随机密码
来源：http://mef.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://hqp.tianlin.xyz

[R70] 时间戳与互转
来源：http://mdn.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://ske.zdbjq.cn

[R71] 日期格式化
来源：http://jrr.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zex.cqqwz.cn

[R72] 等待端口就绪
来源：http://unr.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wto.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://jlh.fengsongda.top

split -l 1000 big.log part_
来源：http://ebr.andypj.xyz

[R74] 批量重命名
来源：http://gjh.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fgt.yangfankeji.com

[R75] 导出环境变量
来源：http://mfs.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://cai.nanxuanxn.top

[R76] 使用临时文件
来源：http://mgy.fktsv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iam.havefunace.top

[R77] 读取用户输入
来源：http://sxd.sufxvd.cn

read -rp "请输入: " ans
来源：http://fld.gzhubu.top

[R78] 交互式菜单
来源：http://kbw.xylfe.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://acw.xylfe.cn

[R79] 解析命令行选项
来源：http://rop.yj20258.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iqs.uphjek.com

[R80] 查看脚本执行耗时
来源：http://ucs.cashguo.top

time ./run.sh
来源：http://xkh.pengpengdd.cyou

================================================================================
来源：http://pxy.bbcook.cn

S. C / C++ 专题
来源：http://hke.jiagoushi.top

================================================================================
来源：http://mxf.epnwcf.com

[S01] C：Hello World
来源：http://yvz.gaohongyu789.top

#include <stdio.h>
来源：http://rny.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kwe.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://vcz.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://kjs.xinyue.icu

[S03] C：读入整数
来源：http://sfj.pycfn.com

int x; scanf("%d", &x);
来源：http://vyw.bbcook.cn

[S04] C：字符串复制
来源：http://taw.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://elh.yongpay.top

[S05] C：字符串长度
来源：http://cdp.yvedp.cn

strlen(s)
来源：http://uxq.chenlongwang.top

[S06] C：字符串比较
来源：http://jam.zdbjq.cn

strcmp(a, b) == 0
来源：http://bac.zhengqikj.top

[S07] C：数组遍历求和
来源：http://vpj.yonumen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mtb.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://khk.yj20258.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://llh.zhengqikj.top

[S09] C：结构体定义与初始化
来源：http://hle.ywan-chungtsiang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kic.cheryme.top

[S10] C：指针与解引用
来源：http://gav.hcnkem.com

int *p = &a;  *p = 5;
来源：http://dpg.fktsv.cn

[S11] C：逐行读文件
来源：http://gab.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://rlu.sysykeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pgb.jianghu66.top

fclose(f);
来源：http://rfg.meibo888.top

[S12] C：写文件
来源：http://rww.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bat.yanxiufei.cn

[S13] C：宏定义
来源：http://xdr.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ucc.chenlongwang.top

[S14] C：枚举
来源：http://otv.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://ium.yfazqb.com

[S15] C：类型转换
来源：http://nqp.guowangkeji.top

(double) a / b
来源：http://zme.cdnleiting.top

[S16] C：位操作置位
来源：http://xwu.wangdashe.top

x |= (1 << 3);
来源：http://vyc.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://too.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gkr.gaohongyu789.top

[S18] C：命令行参数
来源：http://hwb.zhijiandao.cn

int main(int argc, char **argv)
来源：http://frh.nanxuanxn.top

[S19] C：快速排序
来源：http://jnn.9152youxi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cuc.smart0.xyz

[S20] C：二分查找
来源：http://nnq.shangyingyoupin.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tcn.zhijiandao.cn

[S21] C：字符类别判断
来源：http://fla.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iqt.cheryme.top

[S22] C：字符串转数字
来源：http://gjl.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://qsf.yonumen.top

[S23] C：随机数
来源：http://fvq.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cyo.gogol.net.cn

[S24] C：获取本地时间
来源：http://abk.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nhm.vehdjk.com

[S25] C：内存拷贝
来源：http://spc.yueranfly.top

memcpy(dst, src, n);
来源：http://hvo.tianlin.xyz

[S26] C：内存清零
来源：http://fnl.jiagoushi.top

memset(a, 0, sizeof a);
来源：http://yzp.dashuyun.cn

[S27] C：定义常量
来源：http://lin.xinyue.icu

const double PI = 3.14159;
来源：http://aus.yonumen.top

[S28] C：静态变量
来源：http://iwf.hammf.cn

static int counter = 0;
来源：http://ltw.yongpay.top

[S29] C：变参函数
来源：http://ctz.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vcv.dashuyun.cn

[S30] C：头文件保护
来源：http://mgv.svipenyu.cn

#ifndef X_H
来源：http://ztq.bjfxy.top

#define X_H
来源：http://hak.xylfe.cn

#endif
来源：http://bop.tian-w.cn

[S31] C++：Hello World
来源：http://col.svipenyu.cn

#include <iostream>
来源：http://lbw.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://fzf.vqdsnc.cn

[S32] C++：字符串
来源：http://bgz.feifeiyinyue.top

std::string s = "hi";  s += "!";
来源：http://sec.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://axg.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fid.jqgfzy.top

[S34] C++：遍历 vector
来源：http://rmr.zdqjudy.top

for (auto &x : v) { std::cout << x; }
来源：http://zvi.jiagoushi.top

[S35] C++：map
来源：http://xxu.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://whb.cucudq.cn

[S36] C++：unordered_map
来源：http://bke.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rjf.dashuyun.cn

[S37] C++：set
来源：http://dcu.chenlongwang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ktl.smart0.xyz

[S38] C++：排序
来源：http://ttn.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://jmb.fengsongda.top

[S39] C++：自定义比较器排序
来源：http://arb.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qrm.yongpay.top

[S40] C++：查找元素
来源：http://oes.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eln.nanxinkj.top

[S41] C++：类与构造函数
来源：http://xtk.gogol.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zug.ivvv.top

[S42] C++：继承与虚函数
来源：http://tul.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://vpr.fehbvm.com

[S43] C++：智能指针
来源：http://oyr.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://hgf.cdnleiting.top

[S44] C++：引用传参
来源：http://pjk.hongshengwenyu.top

void inc(int &x) { ++x; }
来源：http://fer.feifeiyinyue.top

[S45] C++：lambda
来源：http://mcq.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://hwh.xylfe.cn

[S46] C++：函数模板
来源：http://cwx.sxryk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sqr.hammf.cn

[S47] C++：结构化绑定遍历
来源：http://yja.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nwc.ydzc1.top

[S48] C++：逐行读文件
来源：http://dmb.cheryme.top

std::ifstream in("a.txt");  std::string line;
来源：http://tjl.xuanzx.com

while (std::getline(in, line)) { }
来源：http://glk.jlsjyb.cn

[S49] C++：写文件
来源：http://ahe.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://inn.ehwqpu.com

[S50] C++：格式化数字
来源：http://oyl.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bzj.xinyue.icu

[S51] C++：显式类型转换
来源：http://mnq.cqqwz.cn

static_cast<double>(a) / b
来源：http://bcu.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://zyb.jqgufenzy.top

int size() const noexcept { return n_; }
来源：http://rke.gzhubu.top

[S53] C++：移动语义
来源：http://azw.zhongyouzk.top

std::vector<int> w = std::move(v);
来源：http://dmm.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://txj.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mlp.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://gcp.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zvf.jinqigufen.top

[S56] C++：optional
来源：http://qqc.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bwj.yfazqb.com

[S57] C++：编译期常量
来源：http://bgh.tanke756.top

constexpr int N = 10;
来源：http://fsc.zdqjudy.top

[S58] C++：命名空间
来源：http://uxl.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://pws.ctjpmb.com

[S59] C++：静态断言
来源：http://wji.mhx1999.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ntz.ehwqpu.com

[S60] C++：遍历并删除元素
来源：http://blj.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pzs.fzhhl.top

================================================================================
来源：http://csm.yueranfly.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ebo.tianlin.xyz

================================================================================
来源：http://cyh.svipenyu.cn

[T01] Kotlin：Hello World
来源：http://dpr.yueranfly.top

println("Hello")
来源：http://iez.gogol.net.cn

[T02] Kotlin：变量
来源：http://vco.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fnh.ywan-chungtsiang.top

[T03] Kotlin：字符串模板
来源：http://kkm.jqgufenzy.top

"值: $b"
来源：http://bma.cheryme.top

[T04] Kotlin：空安全
来源：http://kxz.nanxinkj.top

val n: String? = null;  n?.length
来源：http://kih.birdmap.top

[T05] Kotlin：when 表达式
来源：http://iqf.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vyf.hesvh.cn

[T06] Kotlin：集合映射
来源：http://jhm.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ahq.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://qyh.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hls.wangdashe.top

[T08] Kotlin：数据类
来源：http://fwc.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://csh.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://eju.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://ykw.ppjwa.cn

[T10] Kotlin：默认参数
来源：http://oyi.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://rxv.shanyushiyangkeji.top

[T11] Kotlin：协程
来源：http://xur.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pzq.epnwcf.com

[T12] Kotlin：解构声明
来源：http://jjr.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://hgk.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://iop.guannengcc.top

val m = mapOf("a" to 1)
来源：http://knu.zycfv.cn

[T14] Kotlin：循环
来源：http://abb.hnqzz.top

for (i in 1..10) println(i)
来源：http://gxg.gzhubu.top

[T15] Kotlin：接口
来源：http://qxk.feifeiyinyue.top

interface Shape { fun area(): Double }
来源：http://lui.nwbrower.top

[T16] Swift：Hello World
来源：http://uiv.0kj1m.cn

print("Hello")
来源：http://ihr.hfpthk.cn

[T17] Swift：变量与常量
来源：http://hgv.iojbl.cn

var a = 1;  let b = 2
来源：http://nxy.gotoacloud.top

[T18] Swift：字符串插值
来源：http://jnj.shuidangran.top

"值: \(b)"
来源：http://drb.zhaomingkeji.xyz

[T19] Swift：可选绑定
来源：http://wgc.zdbjq.cn

if let n = opt { print(n) }
来源：http://cli.jiagoushi.top

[T20] Swift：数组操作
来源：http://hgb.yangfankeji.com

var a = [1, 2, 3];  a.append(4)
来源：http://zxh.wangshuangyany.cn

[T21] Swift：遍历
来源：http://zuc.xuanzx.com

for x in a { print(x) }
来源：http://mbw.aizwys.cn

[T22] Swift：字典
来源：http://pwv.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vkj.fzhhl.top

[T23] Swift：函数
来源：http://aqj.fktsv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bqp.zhiwuduotai.top

[T24] Swift：闭包
来源：http://kod.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://dvu.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://oug.mhx1999.top

struct P { var x: Int }
来源：http://xov.vqdsnc.cn

[T26] Swift：类与重写
来源：http://szt.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://qqs.daria6918.cn

[T27] Swift：错误处理
来源：http://lsy.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://rix.feifeiyinyue.top

[T28] Swift：枚举
来源：http://zdu.fzhhl.top

enum Color { case red, green }
来源：http://tdj.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://uon.cdnleiting.top

guard let x = opt else { return }
来源：http://tno.redwolf501.top

[T30] Swift：协议
来源：http://xiu.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://lnr.nanxinkj.top

[T31] Lua：Hello World
来源：http://hgh.nanxuanxn.top

print("Hello")
来源：http://aap.zycfv.cn

[T32] Lua：局部变量
来源：http://rnh.redwolf501.top

local a = 1
来源：http://gvw.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://ize.jinghuilouyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tzk.jiagoushi.top

[T34] Lua：遍历表
来源：http://pwy.gogol.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ixp.zhiwuduotai.top

[T35] Lua：字典表
来源：http://xpm.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://rmm.fzhhl.top

[T36] Lua：函数
来源：http://vur.aibaodan.cn

function add(a, b) return a + b end
来源：http://uzx.haohaochexian.top

[T37] Lua：字符串拼接
来源：http://vax.jianghu66.top

"a" .. "b"
来源：http://cpd.jinqigufen.top

[T38] Lua：条件
来源：http://vvf.zdbjq.cn

if x > 0 then print("正") end
来源：http://yvg.nwbrower.top


<!-- 参考信息 -->