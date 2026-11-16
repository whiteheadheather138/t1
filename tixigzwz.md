代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://tun.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://aix.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pjo.sysykeji.top

[R37] 把输出赋给变量
来源：http://ysr.zhengqikj.top

files=$(ls -1)
来源：http://dwo.guowangkeji.top

[R38] 管道串联
来源：http://pat.gaohongyu789.top

cat a.txt | grep -i error | wc -l
来源：http://sre.chenzaomai.com

[R39] 重定向标准输出与错误
来源：http://ahv.hysaishi.cn

cmd > out.log 2>&1
来源：http://bkz.wangdashe.top

[R40] 追加写日志
来源：http://fcu.fzhhl.top

echo "log" >> out.log
来源：http://ohv.fehbvm.com

[R41] 丢弃输出
来源：http://zrp.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://ddn.tian-w.cn

[R42] 输入重定向
来源：http://xui.jianghu66.top

wc -l < a.txt
来源：http://uzs.daria6918.cn

[R43] 按名字查找文件
来源：http://kad.cucudq.cn

find . -name "*.log" -type f
来源：http://hwu.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://jty.uphjek.com

find . -mtime -7 -type f
来源：http://mbp.nwbrower.top

[R45] 批量删除
来源：http://ese.chenzaomai.com

find . -name "*.tmp" -delete
来源：http://dxc.yvedp.cn

[R46] 递归替换文件内容
来源：http://phn.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ppy.aizwys.cn

[R47] sed 单行替换
来源：http://ldh.andypj.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://hdg.zhixingplan.top

[R48] awk 取指定列
来源：http://txd.vehdjk.com

awk '{print $1, $3}' a.txt
来源：http://way.cdnleiting.top

[R49] awk 带条件
来源：http://cot.0kj1m.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kgt.epnwcf.com

[R50] awk 求和
来源：http://cdk.wangdashe.top

awk '{s += $2} END {print s}' a.txt
来源：http://sal.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://gpt.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rxt.chenzaomai.com

[R52] 统计行数
来源：http://dck.yanxiufei.cn

wc -l a.txt
来源：http://yjo.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://syk.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nma.aizwys.cn

[R54] 比较两个文件
来源：http://yhw.aizwys.cn

diff a.txt b.txt
来源：http://fsx.chenlongwang.top

[R55] 压缩与解压
来源：http://irk.zycfv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ybe.yueranfly.top

[R56] 远程拷贝
来源：http://whq.jianghu66.top

scp file user@host:/path/
来源：http://spf.yuanzhike.top

[R57] 远程执行命令
来源：http://daw.yfazqb.com

ssh user@host 'uptime'
来源：http://cqt.ppjwa.cn

[R58] 下载文件
来源：http://ddj.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wuv.xingfuxueyuan.xyz

[R59] 发 POST JSON
来源：http://jbs.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ezh.tanke756.top

[R60] 只看 HTTP 状态码
来源：http://qxw.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yil.feifeiyinyue.top

[R61] 磁盘占用
来源：http://yct.sufxvd.cn

df -h;  du -sh *
来源：http://zit.jiagoushi.top

[R62] 找最占空间的文件
来源：http://guf.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://mtn.zycfv.cn

[R63] 内存与进程
来源：http://ami.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://ifi.dashuyun.cn

[R64] 结束进程
来源：http://rpe.gzhubu.top

kill -9 $(pgrep -f app.py)
来源：http://ajv.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://vqw.vqdsnc.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vza.tarul.cn

[R66] 定时任务
来源：http://iga.cdnleiting.top

crontab -e;  crontab -l
来源：http://cyw.pycfn.com

[R67] 生成随机十六进制串
来源：http://gra.wangshuangyany.cn

openssl rand -hex 16
来源：http://xui.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://sps.chenzaomai.com

sha256sum a.txt;  md5sum a.txt
来源：http://ngz.ydzc1.top

[R69] 生成随机密码
来源：http://idx.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://mri.smart0.xyz

[R70] 时间戳与互转
来源：http://zde.pycfn.com

date +%s;  date -d @1700000000
来源：http://ulg.52xcode.cn

[R71] 日期格式化
来源：http://xan.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ejm.redwolf501.top

[R72] 等待端口就绪
来源：http://otv.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://amd.meibo888.top

[R73] 分割大日志
来源：http://wog.ybcxt.top

split -l 1000 big.log part_
来源：http://rex.zhiwuduotai.top

[R74] 批量重命名
来源：http://vrc.zhengqikj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ajw.zhixingplan.top

[R75] 导出环境变量
来源：http://cra.sxryk.cn

export PATH="$HOME/bin:$PATH"
来源：http://kuw.zhengqikj.top

[R76] 使用临时文件
来源：http://hqb.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://orl.sjlbkw.cn

[R77] 读取用户输入
来源：http://zct.dianchejie.cn

read -rp "请输入: " ans
来源：http://pxa.bjfxy.top

[R78] 交互式菜单
来源：http://osh.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xfl.wangdashe.top

[R79] 解析命令行选项
来源：http://yxw.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ctt.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://ctz.havefunace.top

time ./run.sh
来源：http://uor.zhoulong.xyz

================================================================================
来源：http://hpt.quarkkingdee.top

S. C / C++ 专题
来源：http://cni.fanxiaobao.xyz

================================================================================
来源：http://mng.jianghu66.top

[S01] C：Hello World
来源：http://xpy.guannengcc.top

#include <stdio.h>
来源：http://vej.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bxu.yuxming.cn

[S02] C：变量与格式化输出
来源：http://dvp.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://bmr.jinqigufen.top

[S03] C：读入整数
来源：http://pxz.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://zij.yueranfly.top

[S04] C：字符串复制
来源：http://uak.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://gsc.zhengqikj.top

[S05] C：字符串长度
来源：http://yzp.bbcook.cn

strlen(s)
来源：http://eto.nanxinkj.top

[S06] C：字符串比较
来源：http://sgm.jinghuilouyu.cn

strcmp(a, b) == 0
来源：http://kzk.jyoumei.cn

[S07] C：数组遍历求和
来源：http://cin.xinyue.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yux.fanxiaobao.xyz

[S08] C：动态内存分配与释放
来源：http://wgt.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mbn.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://poi.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cqk.jlsjyb.cn

[S10] C：指针与解引用
来源：http://kgs.hfpthk.cn

int *p = &a;  *p = 5;
来源：http://yge.316326.xyz

[S11] C：逐行读文件
来源：http://oof.yueranfly.top

FILE *f = fopen("a.txt", "r");
来源：http://yli.yj20258.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bmc.pycfn.com

fclose(f);
来源：http://khs.gogol.net.cn

[S12] C：写文件
来源：http://vfr.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dfn.zdbjq.cn

[S13] C：宏定义
来源：http://vnp.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pkr.fktsv.cn

[S14] C：枚举
来源：http://cle.redwolf501.top

enum Color { RED, GREEN, BLUE };
来源：http://ubr.dashuyun.cn

[S15] C：类型转换
来源：http://rmb.dashuyun.cn

(double) a / b
来源：http://ubh.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://bqm.dianchejie.cn

x |= (1 << 3);
来源：http://xcx.yvedp.cn

[S17] C：安全拼接字符串
来源：http://pfj.pycfn.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tli.xuanzx.com

[S18] C：命令行参数
来源：http://uiy.yuxming.cn

int main(int argc, char **argv)
来源：http://yuk.yuanzhike.top

[S19] C：快速排序
来源：http://nwu.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://dav.epnwcf.com

[S20] C：二分查找
来源：http://xgl.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jbv.redwolf501.top

[S21] C：字符类别判断
来源：http://lad.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://enc.jinqigufen.top

[S22] C：字符串转数字
来源：http://spx.yanxiufei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qqm.tarul.cn

[S23] C：随机数
来源：http://yev.fktsv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cid.quarkkingdee.top

[S24] C：获取本地时间
来源：http://gqr.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nwu.snrcjt.cn

[S25] C：内存拷贝
来源：http://xsv.andypj.xyz

memcpy(dst, src, n);
来源：http://mot.0kj1m.cn

[S26] C：内存清零
来源：http://fxl.jianghu66.top

memset(a, 0, sizeof a);
来源：http://cuf.jqgfzy.top

[S27] C：定义常量
来源：http://shs.yueranfly.top

const double PI = 3.14159;
来源：http://ycl.yj202588.top

[S28] C：静态变量
来源：http://aew.xylfe.cn

static int counter = 0;
来源：http://gwz.hysaishi.cn

[S29] C：变参函数
来源：http://qng.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://puh.smart0.xyz

[S30] C：头文件保护
来源：http://bpa.dianchejie.cn

#ifndef X_H
来源：http://yyo.gotoacloud.top

#define X_H
来源：http://wsl.xuetiantiany.cn

#endif
来源：http://bul.yuxming.cn

[S31] C++：Hello World
来源：http://onn.fanxiaobao.xyz

#include <iostream>
来源：http://dav.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://zqb.zhengqikj.top

[S32] C++：字符串
来源：http://hyn.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://spz.jqgufenzy.top

[S33] C++：vector 增删
来源：http://vvg.tanke756.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dmq.c1oappe.top

[S34] C++：遍历 vector
来源：http://bmn.dashuyun.cn

for (auto &x : v) { std::cout << x; }
来源：http://zjv.havefunace.top

[S35] C++：map
来源：http://cnw.yj202588.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cvc.wangdashe.top

[S36] C++：unordered_map
来源：http://jkj.fzhhl.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xrm.meibo888.top

[S37] C++：set
来源：http://cvj.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hsy.shzxlz.cn

[S38] C++：排序
来源：http://pwy.birdmap.top

std::sort(v.begin(), v.end());
来源：http://jwc.dashuyun.cn

[S39] C++：自定义比较器排序
来源：http://tyq.zhixingplan.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mff.bjfxy.top

[S40] C++：查找元素
来源：http://yfn.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://onn.jianghu66.top

[S41] C++：类与构造函数
来源：http://ufz.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gbv.tian-w.cn

[S42] C++：继承与虚函数
来源：http://kbb.cqqwz.cn

class B : public Base { public: void f() override {} };
来源：http://fcv.shanyushiyangkeji.top

[S43] C++：智能指针
来源：http://rui.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://lht.jianghu66.top

[S44] C++：引用传参
来源：http://owt.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://mtd.zhaomingkeji.xyz

[S45] C++：lambda
来源：http://zal.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://mxj.xylfe.cn

[S46] C++：函数模板
来源：http://oel.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://awe.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://uru.snrcjt.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://axy.fzhhl.top

[S48] C++：逐行读文件
来源：http://ank.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://ewu.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://yyk.mhx1999.top

[S49] C++：写文件
来源：http://usg.jyoumei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xbh.kuanghao11.cn

[S50] C++：格式化数字
来源：http://jwu.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://roh.sweek.top

[S51] C++：显式类型转换
来源：http://yow.epnwcf.com

static_cast<double>(a) / b
来源：http://kpo.sweek.top

[S52] C++：const 与 noexcept
来源：http://fdn.jinqigufen.top

int size() const noexcept { return n_; }
来源：http://aex.bjfxy.top

[S53] C++：移动语义
来源：http://oce.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://aja.tarul.cn

[S54] C++：异常处理
来源：http://mfg.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jrz.gotoacloud.top

[S55] C++：结构化绑定
来源：http://lgf.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mkl.yfazqb.com

[S56] C++：optional
来源：http://nzc.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mmn.cdnleiting.top

[S57] C++：编译期常量
来源：http://jow.jianghu66.top

constexpr int N = 10;
来源：http://kjv.smart0.xyz

[S58] C++：命名空间
来源：http://kkr.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://ibn.cucudq.cn

[S59] C++：静态断言
来源：http://fjs.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dsq.ydjk.org.cn

[S60] C++：遍历并删除元素
来源：http://bws.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jlv.sufxvd.cn

================================================================================
来源：http://wol.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gmd.yueranfly.top

================================================================================
来源：http://nld.yuxming.cn

[T01] Kotlin：Hello World
来源：http://wrz.ydzc1.top

println("Hello")
来源：http://icf.shzxlz.cn

[T02] Kotlin：变量
来源：http://llo.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jnj.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://qiz.xylfe.cn

"值: $b"
来源：http://onh.316326.xyz

[T04] Kotlin：空安全
来源：http://hiy.uphjek.com

val n: String? = null;  n?.length
来源：http://eqn.jqgufenzy.top

[T05] Kotlin：when 表达式
来源：http://eyr.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cgo.sxryk.cn

[T06] Kotlin：集合映射
来源：http://ols.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bvj.uphjek.com

[T07] Kotlin：集合过滤
来源：http://dsz.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://iol.xylfe.cn

[T08] Kotlin：数据类
来源：http://pch.ivvv.top

data class User(val name: String, val age: Int)
来源：http://igy.hfpthk.cn

[T09] Kotlin：扩展函数
来源：http://bhe.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://obv.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://vfd.jyoumei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zlt.vehdjk.com

[T11] Kotlin：协程
来源：http://hig.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kgm.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://zmp.yfazqb.com

val (a, b) = Pair(1, 2)
来源：http://joy.yuanzhike.top

[T13] Kotlin：只读 Map
来源：http://gvc.xuetiantiany.cn

val m = mapOf("a" to 1)
来源：http://ndy.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://sov.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://nop.haohaochexian.top

[T15] Kotlin：接口
来源：http://lgg.nanxuanxn.top

interface Shape { fun area(): Double }
来源：http://vvi.daxiang520.top

[T16] Swift：Hello World
来源：http://clr.sysykeji.top

print("Hello")
来源：http://ewp.andypj.xyz

[T17] Swift：变量与常量
来源：http://cae.cheryme.top

var a = 1;  let b = 2
来源：http://oex.hywenlv.cn

[T18] Swift：字符串插值
来源：http://ryh.jiagoushi.top

"值: \(b)"
来源：http://vmj.zdqjudy.top

[T19] Swift：可选绑定
来源：http://sod.9152youxi.cn

if let n = opt { print(n) }
来源：http://nxd.cashguo.top

[T20] Swift：数组操作
来源：http://wpx.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jyg.iojbl.cn

[T21] Swift：遍历
来源：http://eiv.xylfe.cn

for x in a { print(x) }
来源：http://apk.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://qkd.ywan-chungtsiang.top

var d = ["a": 1];  d["b"] = 2
来源：http://nji.daria6918.cn

[T23] Swift：函数
来源：http://kuu.birdmap.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tno.yanxiufei.cn

[T24] Swift：闭包
来源：http://jmv.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://irb.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://imc.tian-w.cn

struct P { var x: Int }
来源：http://ukj.yangfankeji.com

[T26] Swift：类与重写
来源：http://oxq.haohaochexian.top

class A: Base { override func f() {} }
来源：http://nvu.chenlongwang.top

[T27] Swift：错误处理
来源：http://idn.fengsongda.top

do { try f() } catch { print(error) }
来源：http://ftm.svipenyu.cn

[T28] Swift：枚举
来源：http://cdo.zhengqikj.top

enum Color { case red, green }
来源：http://brv.hywenlv.cn

[T29] Swift：guard 提前返回
来源：http://ebz.ivvv.top

guard let x = opt else { return }
来源：http://oec.jinghuilouyu.cn

[T30] Swift：协议
来源：http://igi.vehdjk.com

protocol Shape { func area() -> Double }
来源：http://eub.haohaochexian.top

[T31] Lua：Hello World
来源：http://uey.316326.xyz

print("Hello")
来源：http://jmb.yangfankeji.com

[T32] Lua：局部变量
来源：http://ywn.sufxvd.cn

local a = 1
来源：http://ypc.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://qrq.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hrd.ppjwa.cn

[T34] Lua：遍历表
来源：http://bnr.cashguo.top

for i, v in ipairs(t) do print(i, v) end
来源：http://usg.xuetiantiany.cn

[T35] Lua：字典表
来源：http://ijh.xuetiantiany.cn

local d = { a = 1 };  d.b = 2
来源：http://tox.zhijiandao.cn

[T36] Lua：函数
来源：http://sic.epnwcf.com

function add(a, b) return a + b end
来源：http://lcx.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://wce.ppjwa.cn

"a" .. "b"
来源：http://jsh.zhixingplan.top

[T38] Lua：条件
来源：http://obo.jlsjyb.cn

if x > 0 then print("正") end
来源：http://uig.ivvv.top


<!-- 参考信息 -->