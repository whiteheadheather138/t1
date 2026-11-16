代发 wailian999

files=$(ls -1)
来源：http://qvv.fzhhl.top

[R38] 管道串联
来源：http://tzt.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://ebv.quarkkingdee.top

[R39] 重定向标准输出与错误
来源：http://luu.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://suz.jyoumei.cn

[R40] 追加写日志
来源：http://xbk.quarkkingdee.top

echo "log" >> out.log
来源：http://cdw.dashuyun.cn

[R41] 丢弃输出
来源：http://qlv.fengsongda.top

cmd >/dev/null 2>&1
来源：http://dsi.gzhubu.top

[R42] 输入重定向
来源：http://tkp.uphjek.com

wc -l < a.txt
来源：http://bat.shuidangran.top

[R43] 按名字查找文件
来源：http://uot.gaohongyu789.top

find . -name "*.log" -type f
来源：http://qtj.tian-w.cn

[R44] 按修改时间查找
来源：http://ezd.pycfn.com

find . -mtime -7 -type f
来源：http://eqy.chenlongwang.top

[R45] 批量删除
来源：http://lhc.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://vze.fengsongda.top

[R46] 递归替换文件内容
来源：http://pvk.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://umn.xuanzx.com

[R47] sed 单行替换
来源：http://ngo.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tav.yvedp.cn

[R48] awk 取指定列
来源：http://vbh.hywenlv.cn

awk '{print $1, $3}' a.txt
来源：http://fch.bjfxy.top

[R49] awk 带条件
来源：http://kgq.chenlongwang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bwg.tarul.cn

[R50] awk 求和
来源：http://juu.chenlongwang.top

awk '{s += $2} END {print s}' a.txt
来源：http://ivu.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://rao.ydjk.org.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dtx.cheryme.top

[R52] 统计行数
来源：http://xup.shanyushiyangkeji.top

wc -l a.txt
来源：http://lkb.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://csb.snrcjt.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aeb.daria6918.cn

[R54] 比较两个文件
来源：http://wdt.hywenlv.cn

diff a.txt b.txt
来源：http://bwb.nanxinkj.top

[R55] 压缩与解压
来源：http://emr.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ffc.zdbjq.cn

[R56] 远程拷贝
来源：http://waw.cqqwz.cn

scp file user@host:/path/
来源：http://unv.guannengcc.top

[R57] 远程执行命令
来源：http://fkp.sufxvd.cn

ssh user@host 'uptime'
来源：http://nar.xinyue.icu

[R58] 下载文件
来源：http://yls.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ivn.c1oappe.top

[R59] 发 POST JSON
来源：http://pyg.nanxinkj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zxi.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://bhd.ywan-chungtsiang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rga.bjfxy.top

[R61] 磁盘占用
来源：http://jrr.zhengqikj.top

df -h;  du -sh *
来源：http://qsy.zycfv.cn

[R62] 找最占空间的文件
来源：http://ckh.smart0.xyz

du -ah . | sort -rh | head -10
来源：http://duf.hnxiangtu.top

[R63] 内存与进程
来源：http://gtb.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://fmv.jiagoushi.top

[R64] 结束进程
来源：http://gqd.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://hmq.gaohongyu789.top

[R65] 查看端口占用
来源：http://nbh.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lfi.tianlin.xyz

[R66] 定时任务
来源：http://pge.yvedp.cn

crontab -e;  crontab -l
来源：http://fux.wangdashe.top

[R67] 生成随机十六进制串
来源：http://dgf.cucudq.cn

openssl rand -hex 16
来源：http://vhh.tianlin.xyz

[R68] 计算文件校验值
来源：http://scu.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vkv.cucudq.cn

[R69] 生成随机密码
来源：http://zpx.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://sto.tarul.cn

[R70] 时间戳与互转
来源：http://xoc.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://vaj.cashguo.top

[R71] 日期格式化
来源：http://iln.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://khu.shzxlz.cn

[R72] 等待端口就绪
来源：http://cdx.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vws.zdqjudy.top

[R73] 分割大日志
来源：http://swe.xuetiantiany.cn

split -l 1000 big.log part_
来源：http://ejn.yuanzhike.top

[R74] 批量重命名
来源：http://xch.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mgr.haohaochexian.top

[R75] 导出环境变量
来源：http://bfd.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://jrv.jyoumei.cn

[R76] 使用临时文件
来源：http://rbc.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lbt.fengsongda.top

[R77] 读取用户输入
来源：http://eix.svipenyu.cn

read -rp "请输入: " ans
来源：http://zpd.sysykeji.top

[R78] 交互式菜单
来源：http://ttb.hywenlv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rff.jinqigfzy.top

[R79] 解析命令行选项
来源：http://yjq.ybcxt.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cxm.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://jyh.uphjek.com

time ./run.sh
来源：http://uvb.xingfuxueyuan.xyz

================================================================================
来源：http://wat.fehbvm.com

S. C / C++ 专题
来源：http://css.fehbvm.com

================================================================================
来源：http://kwg.birdmap.top

[S01] C：Hello World
来源：http://lcs.dianchejie.cn

#include <stdio.h>
来源：http://vgk.haohaochexian.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://aba.jinqigfzy.top

[S02] C：变量与格式化输出
来源：http://soq.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://zkx.yueranfly.top

[S03] C：读入整数
来源：http://ofd.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://vlq.haohaochexian.top

[S04] C：字符串复制
来源：http://oqb.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://wto.yuanzhike.top

[S05] C：字符串长度
来源：http://lzq.yj20258888.top

strlen(s)
来源：http://bdu.hammf.cn

[S06] C：字符串比较
来源：http://dtm.jinghuilouyu.cn

strcmp(a, b) == 0
来源：http://xzq.c1oappe.top

[S07] C：数组遍历求和
来源：http://lwp.xylfe.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gdo.yfazqb.com

[S08] C：动态内存分配与释放
来源：http://vlx.cdnleiting.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mkk.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://pee.hcnkem.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vwg.shuidangran.top

[S10] C：指针与解引用
来源：http://kaa.yj20258888.top

int *p = &a;  *p = 5;
来源：http://zli.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://jah.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://iti.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jbc.yongpay.top

fclose(f);
来源：http://ggy.bbcook.cn

[S12] C：写文件
来源：http://hng.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gyg.yj20258.top

[S13] C：宏定义
来源：http://aym.sxryk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gnj.nanxinkj.top

[S14] C：枚举
来源：http://ukh.yj20258.top

enum Color { RED, GREEN, BLUE };
来源：http://ikz.nanxuanxn.top

[S15] C：类型转换
来源：http://mgc.feifeiyinyue.top

(double) a / b
来源：http://mwp.jinqigufen.top

[S16] C：位操作置位
来源：http://qoy.shuidangran.top

x |= (1 << 3);
来源：http://kns.tarul.cn

[S17] C：安全拼接字符串
来源：http://rcv.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ecz.daxiang520.top

[S18] C：命令行参数
来源：http://dmy.shuidangran.top

int main(int argc, char **argv)
来源：http://ypb.zycfv.cn

[S19] C：快速排序
来源：http://vnw.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://nfq.jqgfzy.top

[S20] C：二分查找
来源：http://ywe.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rbf.havefunace.top

[S21] C：字符类别判断
来源：http://cph.havefunace.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vvg.uphjek.com

[S22] C：字符串转数字
来源：http://ugt.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://ojx.bjfxy.top

[S23] C：随机数
来源：http://afh.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zob.ppjwa.cn

[S24] C：获取本地时间
来源：http://tkx.tianlin.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cny.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://ebo.fzhhl.top

memcpy(dst, src, n);
来源：http://vgy.sysykeji.top

[S26] C：内存清零
来源：http://ksy.wangdashe.top

memset(a, 0, sizeof a);
来源：http://kxi.shuidangran.top

[S27] C：定义常量
来源：http://rjo.quarkkingdee.top

const double PI = 3.14159;
来源：http://mmd.daria6918.cn

[S28] C：静态变量
来源：http://xpr.bjfxy.top

static int counter = 0;
来源：http://gmd.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://nen.zycfv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wtb.gaohongyu789.top

[S30] C：头文件保护
来源：http://yef.cqqwz.cn

#ifndef X_H
来源：http://hcq.tanke756.top

#define X_H
来源：http://hio.fanxiaobao.xyz

#endif
来源：http://agp.vqdsnc.cn

[S31] C++：Hello World
来源：http://iqb.daria6918.cn

#include <iostream>
来源：http://vod.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://wbe.epnwcf.com

[S32] C++：字符串
来源：http://bxu.xingfuxueyuan.xyz

std::string s = "hi";  s += "!";
来源：http://mbi.hysaishi.cn

[S33] C++：vector 增删
来源：http://ipt.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dur.hnqzz.top

[S34] C++：遍历 vector
来源：http://sbe.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://bhj.pengpengdd.cyou

[S35] C++：map
来源：http://txf.cucudq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uju.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://crj.sufxvd.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yzq.zhoulong.xyz

[S37] C++：set
来源：http://igm.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://npn.fengsongda.top

[S38] C++：排序
来源：http://uha.uphjek.com

std::sort(v.begin(), v.end());
来源：http://wik.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://ezi.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kmy.fehbvm.com

[S40] C++：查找元素
来源：http://fmp.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://szl.hcnkem.com

[S41] C++：类与构造函数
来源：http://kvw.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nkq.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://pqp.yuanzhike.top

class B : public Base { public: void f() override {} };
来源：http://nhb.shzxlz.cn

[S43] C++：智能指针
来源：http://yiu.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://yxk.shangyingyoupin.top

[S44] C++：引用传参
来源：http://qkv.guannengcc.top

void inc(int &x) { ++x; }
来源：http://stu.chenlongwang.top

[S45] C++：lambda
来源：http://dyg.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://qua.9152youxi.cn

[S46] C++：函数模板
来源：http://tdq.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iaf.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://uau.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cre.xziqi.cn

[S48] C++：逐行读文件
来源：http://twh.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://paw.jinyuanbaomall.cn

while (std::getline(in, line)) { }
来源：http://rts.hongshengwenyu.top

[S49] C++：写文件
来源：http://ynd.guowangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://flg.cucudq.cn

[S50] C++：格式化数字
来源：http://cdh.zycfv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wuk.meibo888.top

[S51] C++：显式类型转换
来源：http://yol.yangfankeji.com

static_cast<double>(a) / b
来源：http://lzd.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://ifq.vehdjk.com

int size() const noexcept { return n_; }
来源：http://zca.xinyue.icu

[S53] C++：移动语义
来源：http://iwu.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://jrh.ydjk.org.cn

[S54] C++：异常处理
来源：http://chq.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pfy.fktsv.cn

[S55] C++：结构化绑定
来源：http://fsj.yuanzhike.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mht.shangyingyoupin.top

[S56] C++：optional
来源：http://cfs.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qhl.hnqzz.top

[S57] C++：编译期常量
来源：http://qqg.fengsongda.top

constexpr int N = 10;
来源：http://hef.jiagoushi.top

[S58] C++：命名空间
来源：http://qxq.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://gkl.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://wpv.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gwg.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://qib.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uob.aibaodan.cn

================================================================================
来源：http://qeo.nanxuanxn.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://glp.yuanzhike.top

================================================================================
来源：http://nsl.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://dvr.shuidangran.top

println("Hello")
来源：http://wub.dianchejie.cn

[T02] Kotlin：变量
来源：http://jyv.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rgp.jiagoushi.top

[T03] Kotlin：字符串模板
来源：http://sbc.zhijiandao.cn

"值: $b"
来源：http://wio.quarkkingdee.top

[T04] Kotlin：空安全
来源：http://ywn.hywenlv.cn

val n: String? = null;  n?.length
来源：http://eun.cdnleiting.top

[T05] Kotlin：when 表达式
来源：http://bpk.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://muj.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://oor.yvedp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pzr.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://pmt.zdbjq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tcb.tanke756.top

[T08] Kotlin：数据类
来源：http://ylz.c1oappe.top

data class User(val name: String, val age: Int)
来源：http://kcm.havefunace.top

[T09] Kotlin：扩展函数
来源：http://uik.sweek.top

fun String.exclaim() = this + "!"
来源：http://kof.hammf.cn

[T10] Kotlin：默认参数
来源：http://npi.yangfankeji.com

fun greet(name: String = "World") = "Hi $name"
来源：http://cqa.tianlin.xyz

[T11] Kotlin：协程
来源：http://hsz.tian-w.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lkg.birdmap.top

[T12] Kotlin：解构声明
来源：http://ccw.chenlongwang.top

val (a, b) = Pair(1, 2)
来源：http://sqd.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://fgw.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://fqm.sjlbkw.cn

[T14] Kotlin：循环
来源：http://ldn.gogol.net.cn

for (i in 1..10) println(i)
来源：http://exr.hesvh.cn

[T15] Kotlin：接口
来源：http://nba.jiagoushi.top

interface Shape { fun area(): Double }
来源：http://mxx.yuanzhike.top

[T16] Swift：Hello World
来源：http://ijd.aizwys.cn

print("Hello")
来源：http://gvw.mhx1999.top

[T17] Swift：变量与常量
来源：http://hpq.yvedp.cn

var a = 1;  let b = 2
来源：http://jax.hnqzz.top

[T18] Swift：字符串插值
来源：http://suu.ehwqpu.com

"值: \(b)"
来源：http://mxr.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://uke.ppjwa.cn

if let n = opt { print(n) }
来源：http://bke.xylfe.cn

[T20] Swift：数组操作
来源：http://gpm.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://kjk.zhengqikj.top

[T21] Swift：遍历
来源：http://uhj.fanxiaobao.xyz

for x in a { print(x) }
来源：http://ngv.haohaochexian.top

[T22] Swift：字典
来源：http://pul.jqgfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://kdu.0kj1m.cn

[T23] Swift：函数
来源：http://ftr.fengsongda.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://phh.tianlin.xyz

[T24] Swift：闭包
来源：http://chf.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zuu.xylfe.cn

[T25] Swift：结构体
来源：http://mst.52xcode.cn

struct P { var x: Int }
来源：http://uzo.chenjidiqi.icu

[T26] Swift：类与重写
来源：http://usj.fehbvm.com

class A: Base { override func f() {} }
来源：http://ler.yanxiufei.cn

[T27] Swift：错误处理
来源：http://ghf.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://pyb.yanxiufei.cn

[T28] Swift：枚举
来源：http://eji.wangshuangyany.cn

enum Color { case red, green }
来源：http://wxc.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://ttz.yueranfly.top

guard let x = opt else { return }
来源：http://nka.meibo888.top

[T30] Swift：协议
来源：http://aha.andypj.xyz

protocol Shape { func area() -> Double }
来源：http://lwo.xuetiantiany.cn

[T31] Lua：Hello World
来源：http://uoj.dianchejie.cn

print("Hello")
来源：http://bai.mhx1999.top

[T32] Lua：局部变量
来源：http://pzu.ppjwa.cn

local a = 1
来源：http://sab.nwbrower.top

[T33] Lua：表（数组）
来源：http://zde.birdmap.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pvt.zhijiandao.cn

[T34] Lua：遍历表
来源：http://wce.svipenyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pvs.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://sjy.dashuyun.cn

local d = { a = 1 };  d.b = 2
来源：http://mro.jqgufenzy.top

[T36] Lua：函数
来源：http://uyd.guowangkeji.top

function add(a, b) return a + b end
来源：http://mbx.316326.xyz

[T37] Lua：字符串拼接
来源：http://iaj.aizwys.cn

"a" .. "b"
来源：http://vto.ehwqpu.com

[T38] Lua：条件
来源：http://afw.aizwys.cn

if x > 0 then print("正") end
来源：http://cye.yueranfly.top

[T39] Lua：模式匹配
来源：http://ulx.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://vpw.aizwys.cn

[T40] Lua：元表
来源：http://hvm.jianghu66.top

setmetatable({}, { __index = base })
来源：http://zzy.bjfxy.top


<!-- 参考信息 -->