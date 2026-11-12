代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://rhp.xuanzx.com

[R36] 并发执行多个任务
来源：http://itl.ydzc1.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gma.yuanzhike.top

[R37] 把输出赋给变量
来源：http://dzo.aibaodan.cn

files=$(ls -1)
来源：http://mnr.9152youxi.cn

[R38] 管道串联
来源：http://zyr.tianlin.xyz

cat a.txt | grep -i error | wc -l
来源：http://cbq.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://rjm.uphjek.com

cmd > out.log 2>&1
来源：http://ksr.zhongyouzk.top

[R40] 追加写日志
来源：http://fiq.tanke756.top

echo "log" >> out.log
来源：http://rap.jinqigufen.top

[R41] 丢弃输出
来源：http://lys.shangyingyoupin.top

cmd >/dev/null 2>&1
来源：http://gjk.xziqi.cn

[R42] 输入重定向
来源：http://lui.epnwcf.com

wc -l < a.txt
来源：http://fwn.snrcjt.cn

[R43] 按名字查找文件
来源：http://ixi.yj202588.top

find . -name "*.log" -type f
来源：http://qqs.9152youxi.cn

[R44] 按修改时间查找
来源：http://abx.jianghu66.top

find . -mtime -7 -type f
来源：http://hza.sysykeji.top

[R45] 批量删除
来源：http://lpn.zycfv.cn

find . -name "*.tmp" -delete
来源：http://dfs.yanxiufei.cn

[R46] 递归替换文件内容
来源：http://qrr.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bss.fehbvm.com

[R47] sed 单行替换
来源：http://fnf.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://mhn.vehdjk.com

[R48] awk 取指定列
来源：http://sor.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://wzk.hysaishi.cn

[R49] awk 带条件
来源：http://ver.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iwo.fanxiaobao.xyz

[R50] awk 求和
来源：http://cuj.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zsy.jlsjyb.cn

[R51] 排序去重取前几
来源：http://gjp.jinyuanbaomall.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tzy.yfazqb.com

[R52] 统计行数
来源：http://kiy.andypj.xyz

wc -l a.txt
来源：http://zkz.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://vyn.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jyx.tanke756.top

[R54] 比较两个文件
来源：http://vra.tarul.cn

diff a.txt b.txt
来源：http://mqh.bjfxy.top

[R55] 压缩与解压
来源：http://dnj.9152youxi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oin.mhx1999.top

[R56] 远程拷贝
来源：http://toa.uphjek.com

scp file user@host:/path/
来源：http://ypu.epnwcf.com

[R57] 远程执行命令
来源：http://fiy.hfpthk.cn

ssh user@host 'uptime'
来源：http://bqk.0kj1m.cn

[R58] 下载文件
来源：http://nko.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kwc.hfpthk.cn

[R59] 发 POST JSON
来源：http://mgk.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zed.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://nkz.zycfv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qvv.yj20258.top

[R61] 磁盘占用
来源：http://hcv.sysykeji.top

df -h;  du -sh *
来源：http://kvm.iojbl.cn

[R62] 找最占空间的文件
来源：http://ysx.shanyushiyangkeji.top

du -ah . | sort -rh | head -10
来源：http://goo.sufxvd.cn

[R63] 内存与进程
来源：http://bgt.yuanzhike.top

free -h;  ps aux | grep nginx
来源：http://ujw.ybcxt.top

[R64] 结束进程
来源：http://gam.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://vfx.ydzc1.top

[R65] 查看端口占用
来源：http://rqp.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://omu.hongshengwenyu.top

[R66] 定时任务
来源：http://eed.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://jzt.hnqzz.top

[R67] 生成随机十六进制串
来源：http://tys.yj202588.top

openssl rand -hex 16
来源：http://laq.sysykeji.top

[R68] 计算文件校验值
来源：http://coo.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://qjt.yuxming.cn

[R69] 生成随机密码
来源：http://rfz.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://bav.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://xoc.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://vxj.snrcjt.cn

[R71] 日期格式化
来源：http://bdu.guowangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dob.jianghu66.top

[R72] 等待端口就绪
来源：http://gja.shangyingyoupin.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ypk.haohaochexian.top

[R73] 分割大日志
来源：http://kso.yongpay.top

split -l 1000 big.log part_
来源：http://vpv.sufxvd.cn

[R74] 批量重命名
来源：http://aqd.haohaochexian.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rej.yonumen.top

[R75] 导出环境变量
来源：http://pzu.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://fbs.mhx1999.top

[R76] 使用临时文件
来源：http://xdx.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yov.daxiang520.top

[R77] 读取用户输入
来源：http://gfn.bjfxy.top

read -rp "请输入: " ans
来源：http://osn.cqqwz.cn

[R78] 交互式菜单
来源：http://ixf.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://iht.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://qaq.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ltx.dianchejie.cn

[R80] 查看脚本执行耗时
来源：http://lkk.zhiwuduotai.top

time ./run.sh
来源：http://nbq.jiagoushi.top

================================================================================
来源：http://ote.jianghu66.top

S. C / C++ 专题
来源：http://jvo.sweek.top

================================================================================
来源：http://hcd.yangfankeji.com

[S01] C：Hello World
来源：http://tzj.ctjpmb.com

#include <stdio.h>
来源：http://htw.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wos.vehdjk.com

[S02] C：变量与格式化输出
来源：http://wkl.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://uvp.jqgufenzy.top

[S03] C：读入整数
来源：http://hqq.iojbl.cn

int x; scanf("%d", &x);
来源：http://ljz.cheryme.top

[S04] C：字符串复制
来源：http://nvt.dashuyun.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qcm.shzxlz.cn

[S05] C：字符串长度
来源：http://iiw.shangyingyoupin.top

strlen(s)
来源：http://uyy.yfazqb.com

[S06] C：字符串比较
来源：http://vwy.chenlongwang.top

strcmp(a, b) == 0
来源：http://wfj.shuidangran.top

[S07] C：数组遍历求和
来源：http://omr.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bcs.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://xag.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hqv.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://coq.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cbo.yvedp.cn

[S10] C：指针与解引用
来源：http://mkc.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://khs.9152youxi.cn

[S11] C：逐行读文件
来源：http://nhd.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://xgg.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qzn.ydjk.org.cn

fclose(f);
来源：http://ayp.bbcook.cn

[S12] C：写文件
来源：http://tdi.uphjek.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yan.snrcjt.cn

[S13] C：宏定义
来源：http://pxr.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aha.daria6918.cn

[S14] C：枚举
来源：http://uca.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://oyf.cqqwz.cn

[S15] C：类型转换
来源：http://wqz.yuxming.cn

(double) a / b
来源：http://zbd.wangshuangyany.cn

[S16] C：位操作置位
来源：http://ytk.yanxiufei.cn

x |= (1 << 3);
来源：http://lox.sxryk.cn

[S17] C：安全拼接字符串
来源：http://pcd.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lly.hcnkem.com

[S18] C：命令行参数
来源：http://uki.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://kjm.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://ivy.dianchejie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dob.zycfv.cn

[S20] C：二分查找
来源：http://aug.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rhw.feifeiyinyue.top

[S21] C：字符类别判断
来源：http://yrs.bbcook.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jeh.yuxming.cn

[S22] C：字符串转数字
来源：http://dbr.zdbjq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qvs.zhoulong.xyz

[S23] C：随机数
来源：http://erv.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://tlg.chenzaomai.com

[S24] C：获取本地时间
来源：http://urn.fanxiaobao.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oyk.xuanzx.com

[S25] C：内存拷贝
来源：http://uoe.cdnleiting.top

memcpy(dst, src, n);
来源：http://kew.fanxiaobao.xyz

[S26] C：内存清零
来源：http://zyy.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://knj.0kj1m.cn

[S27] C：定义常量
来源：http://kys.ehwqpu.com

const double PI = 3.14159;
来源：http://lyr.dashuyun.cn

[S28] C：静态变量
来源：http://imi.xinyue.icu

static int counter = 0;
来源：http://msf.tanke756.top

[S29] C：变参函数
来源：http://uaz.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ukw.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://jcd.gotoacloud.top

#ifndef X_H
来源：http://frf.havefunace.top

#define X_H
来源：http://zwz.hammf.cn

#endif
来源：http://fad.zhiwuduotai.top

[S31] C++：Hello World
来源：http://ssf.yj202588.top

#include <iostream>
来源：http://avv.jqgfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://ohh.jinghuilouyu.cn

[S32] C++：字符串
来源：http://dep.yongpay.top

std::string s = "hi";  s += "!";
来源：http://kgh.haohaochexian.top

[S33] C++：vector 增删
来源：http://fsl.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bjc.sxryk.cn

[S34] C++：遍历 vector
来源：http://vla.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://dtr.zhoulong.xyz

[S35] C++：map
来源：http://xpb.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aww.guowangkeji.top

[S36] C++：unordered_map
来源：http://nfo.ydzc1.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iux.ydzc1.top

[S37] C++：set
来源：http://itb.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rnv.zdbjq.cn

[S38] C++：排序
来源：http://nat.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://wfd.yuanzhike.top

[S39] C++：自定义比较器排序
来源：http://btu.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://klx.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://dbj.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zfi.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://znb.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cxf.yuxming.cn

[S42] C++：继承与虚函数
来源：http://ktv.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://icx.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://eta.gogol.net.cn

auto p = std::make_unique<int>(5);
来源：http://npo.shzxlz.cn

[S44] C++：引用传参
来源：http://yrr.hfpthk.cn

void inc(int &x) { ++x; }
来源：http://yoh.yfazqb.com

[S45] C++：lambda
来源：http://oce.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://wgj.ivvv.top

[S46] C++：函数模板
来源：http://fac.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oqc.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://zzt.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uaa.gzhubu.top

[S48] C++：逐行读文件
来源：http://nay.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gzh.epnwcf.com

while (std::getline(in, line)) { }
来源：http://nwi.316326.xyz

[S49] C++：写文件
来源：http://oqu.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hyq.hesvh.cn

[S50] C++：格式化数字
来源：http://fad.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sol.havefunace.top

[S51] C++：显式类型转换
来源：http://zhk.gzhubu.top

static_cast<double>(a) / b
来源：http://pmg.ywan-chungtsiang.top

[S52] C++：const 与 noexcept
来源：http://gev.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://txa.yonumen.top

[S53] C++：移动语义
来源：http://pbj.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://wwx.tian-w.cn

[S54] C++：异常处理
来源：http://zpc.yangfankeji.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jvj.shuidangran.top

[S55] C++：结构化绑定
来源：http://dbr.jinqigufen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kpa.ybcxt.top

[S56] C++：optional
来源：http://bum.gotoacloud.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mtd.vehdjk.com

[S57] C++：编译期常量
来源：http://jlc.fanxiaobao.xyz

constexpr int N = 10;
来源：http://gbe.zhixingplan.top

[S58] C++：命名空间
来源：http://kxj.zhijiandao.cn

namespace ns { int f() { return 1; } }
来源：http://qbt.zdqjudy.top

[S59] C++：静态断言
来源：http://cpj.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vui.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://ljg.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rhm.smart0.xyz

================================================================================
来源：http://byt.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xfk.jlsjyb.cn

================================================================================
来源：http://mdy.hammf.cn

[T01] Kotlin：Hello World
来源：http://xbw.xuetiantiany.cn

println("Hello")
来源：http://xgq.chenlongwang.top

[T02] Kotlin：变量
来源：http://mqk.andypj.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wzm.fzhhl.top

[T03] Kotlin：字符串模板
来源：http://lwn.hesvh.cn

"值: $b"
来源：http://dop.xinyue.icu

[T04] Kotlin：空安全
来源：http://etr.cdnleiting.top

val n: String? = null;  n?.length
来源：http://nrf.cheryme.top

[T05] Kotlin：when 表达式
来源：http://gji.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tfa.xinyue.icu

[T06] Kotlin：集合映射
来源：http://vnm.ehwqpu.com

listOf(1, 2, 3).map { it * 2 }
来源：http://bpr.uphjek.com

[T07] Kotlin：集合过滤
来源：http://kpm.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dhg.chenlongwang.top

[T08] Kotlin：数据类
来源：http://tuz.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://kmr.chenjidiqi.icu

[T09] Kotlin：扩展函数
来源：http://vlx.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://fpq.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://gch.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://etm.jinqigufen.top

[T11] Kotlin：协程
来源：http://igv.yj20258888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yxn.aizwys.cn

[T12] Kotlin：解构声明
来源：http://rns.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://pvr.haohaochexian.top

[T13] Kotlin：只读 Map
来源：http://gnt.cqqwz.cn

val m = mapOf("a" to 1)
来源：http://sbd.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://yez.hywenlv.cn

for (i in 1..10) println(i)
来源：http://wlw.sweek.top

[T15] Kotlin：接口
来源：http://aab.yj202588.top

interface Shape { fun area(): Double }
来源：http://bbm.yongpay.top

[T16] Swift：Hello World
来源：http://hrk.aizwys.cn

print("Hello")
来源：http://zuf.yj20258.top

[T17] Swift：变量与常量
来源：http://oom.c1oappe.top

var a = 1;  let b = 2
来源：http://jgt.meibo888.top

[T18] Swift：字符串插值
来源：http://xpg.hnxiangtu.top

"值: \(b)"
来源：http://ugs.hammf.cn

[T19] Swift：可选绑定
来源：http://gvm.nanxinkj.top

if let n = opt { print(n) }
来源：http://wbc.tian-w.cn

[T20] Swift：数组操作
来源：http://inj.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://nwr.zhengqikj.top

[T21] Swift：遍历
来源：http://jmm.aibaodan.cn

for x in a { print(x) }
来源：http://xlg.meibo888.top

[T22] Swift：字典
来源：http://zev.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://snu.jiagoushi.top

[T23] Swift：函数
来源：http://iqy.vqdsnc.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wxt.jianghu66.top

[T24] Swift：闭包
来源：http://nmq.52xcode.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://awh.yangfankeji.com

[T25] Swift：结构体
来源：http://vdg.aibaodan.cn

struct P { var x: Int }
来源：http://gcp.snrcjt.cn

[T26] Swift：类与重写
来源：http://dnk.yuxming.cn

class A: Base { override func f() {} }
来源：http://vkk.yvedp.cn

[T27] Swift：错误处理
来源：http://wmo.jqgufenzy.top

do { try f() } catch { print(error) }
来源：http://deb.kuanghao11.cn

[T28] Swift：枚举
来源：http://oey.zhoulong.xyz

enum Color { case red, green }
来源：http://oqx.meibo888.top

[T29] Swift：guard 提前返回
来源：http://pqb.sxryk.cn

guard let x = opt else { return }
来源：http://tnu.tian-w.cn

[T30] Swift：协议
来源：http://qns.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://hwo.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://mir.jqgfzy.top

print("Hello")
来源：http://wuw.daxiang520.top

[T32] Lua：局部变量
来源：http://bml.jlsjyb.cn

local a = 1
来源：http://nee.hesvh.cn

[T33] Lua：表（数组）
来源：http://mvd.nanxuanxn.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zye.hysaishi.cn

[T34] Lua：遍历表
来源：http://kiv.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xvz.tian-w.cn

[T35] Lua：字典表
来源：http://ooc.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://xfy.smart0.xyz

[T36] Lua：函数
来源：http://ite.jinghuilouyu.cn

function add(a, b) return a + b end
来源：http://ars.hammf.cn

[T37] Lua：字符串拼接
来源：http://rrg.svipenyu.cn

"a" .. "b"
来源：http://rrp.hesvh.cn

[T38] Lua：条件
来源：http://dse.zycfv.cn

if x > 0 then print("正") end
来源：http://phn.ydjk.org.cn


<!-- 参考信息 -->