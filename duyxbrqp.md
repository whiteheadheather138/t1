代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://sdz.fengsongda.top

[R36] 并发执行多个任务
来源：http://qwx.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jmy.316326.xyz

[R37] 把输出赋给变量
来源：http://evh.tarul.cn

files=$(ls -1)
来源：http://rdr.iojbl.cn

[R38] 管道串联
来源：http://pez.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://yxk.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://rqh.smart0.xyz

cmd > out.log 2>&1
来源：http://ijb.xylfe.cn

[R40] 追加写日志
来源：http://wkv.shangyingyoupin.top

echo "log" >> out.log
来源：http://cpw.bbcook.cn

[R41] 丢弃输出
来源：http://qyz.fktsv.cn

cmd >/dev/null 2>&1
来源：http://kty.ctjpmb.com

[R42] 输入重定向
来源：http://kel.havefunace.top

wc -l < a.txt
来源：http://dom.vehdjk.com

[R43] 按名字查找文件
来源：http://xim.hcnkem.com

find . -name "*.log" -type f
来源：http://kll.ydzc1.top

[R44] 按修改时间查找
来源：http://zvh.quarkkingdee.top

find . -mtime -7 -type f
来源：http://tss.zhaomingkeji.xyz

[R45] 批量删除
来源：http://ffq.shzxlz.cn

find . -name "*.tmp" -delete
来源：http://gmi.nwbrower.top

[R46] 递归替换文件内容
来源：http://lyv.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zkc.aibaodan.cn

[R47] sed 单行替换
来源：http://dts.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://azy.snrcjt.cn

[R48] awk 取指定列
来源：http://ddf.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://yhw.yj20258888.top

[R49] awk 带条件
来源：http://mco.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qqc.jinyuanbaomall.cn

[R50] awk 求和
来源：http://gam.shangyingyoupin.top

awk '{s += $2} END {print s}' a.txt
来源：http://fjs.shuidangran.top

[R51] 排序去重取前几
来源：http://oem.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lwj.cheryme.top

[R52] 统计行数
来源：http://wxb.snrcjt.cn

wc -l a.txt
来源：http://myu.epnwcf.com

[R53] 查看文件头与实时尾
来源：http://yjp.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zop.jyoumei.cn

[R54] 比较两个文件
来源：http://bya.iojbl.cn

diff a.txt b.txt
来源：http://huj.hysaishi.cn

[R55] 压缩与解压
来源：http://uvy.daria6918.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zla.gaohongyu789.top

[R56] 远程拷贝
来源：http://uje.tarul.cn

scp file user@host:/path/
来源：http://zfx.hongshengwenyu.top

[R57] 远程执行命令
来源：http://aan.andypj.xyz

ssh user@host 'uptime'
来源：http://glf.gogol.net.cn

[R58] 下载文件
来源：http://mpd.ctjpmb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qdy.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://uzz.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hyw.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://dyf.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://urj.tian-w.cn

[R61] 磁盘占用
来源：http://rpv.zhengqikj.top

df -h;  du -sh *
来源：http://ltw.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://wuu.ydjk.org.cn

du -ah . | sort -rh | head -10
来源：http://bji.hywenlv.cn

[R63] 内存与进程
来源：http://ixv.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://lgn.fzhhl.top

[R64] 结束进程
来源：http://jht.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://fiz.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://iox.daxiang520.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sgq.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://nry.fktsv.cn

crontab -e;  crontab -l
来源：http://vhl.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://fkt.hnqzz.top

openssl rand -hex 16
来源：http://dqh.aizwys.cn

[R68] 计算文件校验值
来源：http://hzy.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://gkq.guannengcc.top

[R69] 生成随机密码
来源：http://eew.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://gkz.sysykeji.top

[R70] 时间戳与互转
来源：http://zvb.feifeiyinyue.top

date +%s;  date -d @1700000000
来源：http://nwh.tian-w.cn

[R71] 日期格式化
来源：http://vmf.yueranfly.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wsb.shangyingyoupin.top

[R72] 等待端口就绪
来源：http://qzc.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://hov.jinqigfzy.top

[R73] 分割大日志
来源：http://mcf.yanxiufei.cn

split -l 1000 big.log part_
来源：http://jtb.cqqwz.cn

[R74] 批量重命名
来源：http://ycf.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ctg.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://vzj.gzhubu.top

export PATH="$HOME/bin:$PATH"
来源：http://gli.hfpthk.cn

[R76] 使用临时文件
来源：http://lmn.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nam.yangfankeji.com

[R77] 读取用户输入
来源：http://akc.jinqigfzy.top

read -rp "请输入: " ans
来源：http://wri.hesvh.cn

[R78] 交互式菜单
来源：http://nyb.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mlu.hysaishi.cn

[R79] 解析命令行选项
来源：http://zrd.yj20258.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://abx.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://dku.yongpay.top

time ./run.sh
来源：http://tga.havefunace.top

================================================================================
来源：http://ees.cheryme.top

S. C / C++ 专题
来源：http://rfn.jiagoushi.top

================================================================================
来源：http://joq.tian-w.cn

[S01] C：Hello World
来源：http://dff.yangfankeji.com

#include <stdio.h>
来源：http://eqp.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://tmk.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://xdy.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://sea.svipenyu.cn

[S03] C：读入整数
来源：http://suy.aizwys.cn

int x; scanf("%d", &x);
来源：http://dxn.zdbjq.cn

[S04] C：字符串复制
来源：http://ulw.ywan-chungtsiang.top

char dst[32]; strcpy(dst, "hi");
来源：http://uta.sjlbkw.cn

[S05] C：字符串长度
来源：http://cwn.hongshengwenyu.top

strlen(s)
来源：http://mqg.shuidangran.top

[S06] C：字符串比较
来源：http://ypk.hywenlv.cn

strcmp(a, b) == 0
来源：http://hwc.xylfe.cn

[S07] C：数组遍历求和
来源：http://dby.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://szj.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://zfg.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bkh.cucudq.cn

[S09] C：结构体定义与初始化
来源：http://nur.gaohongyu789.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rbz.fktsv.cn

[S10] C：指针与解引用
来源：http://fzw.andypj.xyz

int *p = &a;  *p = 5;
来源：http://rbh.yuanzhike.top

[S11] C：逐行读文件
来源：http://rfy.cheryme.top

FILE *f = fopen("a.txt", "r");
来源：http://zxl.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bcd.ehwqpu.com

fclose(f);
来源：http://rgy.snrcjt.cn

[S12] C：写文件
来源：http://nrg.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eml.hcnkem.com

[S13] C：宏定义
来源：http://egz.andypj.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qlu.zdqjudy.top

[S14] C：枚举
来源：http://wxi.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://jrl.guannengcc.top

[S15] C：类型转换
来源：http://ces.daria6918.cn

(double) a / b
来源：http://ihf.ydjk.org.cn

[S16] C：位操作置位
来源：http://nnp.316326.xyz

x |= (1 << 3);
来源：http://xun.pycfn.com

[S17] C：安全拼接字符串
来源：http://rnm.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fgb.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://xar.daria6918.cn

int main(int argc, char **argv)
来源：http://moe.yuxming.cn

[S19] C：快速排序
来源：http://mzy.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xhp.sufxvd.cn

[S20] C：二分查找
来源：http://fcq.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mte.jinqigufen.top

[S21] C：字符类别判断
来源：http://hov.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://het.tian-w.cn

[S22] C：字符串转数字
来源：http://adh.ivvv.top

atoi("42");  strtod("3.14", NULL);
来源：http://rxk.yueranfly.top

[S23] C：随机数
来源：http://jlc.gogol.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://das.ivvv.top

[S24] C：获取本地时间
来源：http://nvs.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qzt.shzxlz.cn

[S25] C：内存拷贝
来源：http://amo.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://nkg.fengsongda.top

[S26] C：内存清零
来源：http://ldc.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://lvx.hnqzz.top

[S27] C：定义常量
来源：http://zbq.bjfxy.top

const double PI = 3.14159;
来源：http://klk.cqqwz.cn

[S28] C：静态变量
来源：http://pep.guannengcc.top

static int counter = 0;
来源：http://pxv.yfazqb.com

[S29] C：变参函数
来源：http://wzh.sxryk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sfb.jinyuanbaomall.cn

[S30] C：头文件保护
来源：http://aia.shanyushiyangkeji.top

#ifndef X_H
来源：http://hxj.chenjidiqi.icu

#define X_H
来源：http://nwl.sxryk.cn

#endif
来源：http://hwa.hammf.cn

[S31] C++：Hello World
来源：http://ymc.9152youxi.cn

#include <iostream>
来源：http://vyn.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://jrf.tanke756.top

[S32] C++：字符串
来源：http://ctk.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://gjj.aizwys.cn

[S33] C++：vector 增删
来源：http://oll.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rzc.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://fsu.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://vfo.xingfuxueyuan.xyz

[S35] C++：map
来源：http://wav.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rsd.snrcjt.cn

[S36] C++：unordered_map
来源：http://pxm.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zyj.birdmap.top

[S37] C++：set
来源：http://pad.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://has.tarul.cn

[S38] C++：排序
来源：http://omy.yj20258.top

std::sort(v.begin(), v.end());
来源：http://ohn.316326.xyz

[S39] C++：自定义比较器排序
来源：http://lst.chenjidiqi.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dzq.ydjk.org.cn

[S40] C++：查找元素
来源：http://dsb.vqdsnc.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zhi.zhengqikj.top

[S41] C++：类与构造函数
来源：http://nef.fengsongda.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bxs.gzhubu.top

[S42] C++：继承与虚函数
来源：http://vtf.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://yqg.jqgufenzy.top

[S43] C++：智能指针
来源：http://ybm.tianlin.xyz

auto p = std::make_unique<int>(5);
来源：http://upm.jyoumei.cn

[S44] C++：引用传参
来源：http://icu.epnwcf.com

void inc(int &x) { ++x; }
来源：http://hga.hcnkem.com

[S45] C++：lambda
来源：http://zrp.zhengqikj.top

auto add = [](int a, int b) { return a + b; };
来源：http://jxl.ydzc1.top

[S46] C++：函数模板
来源：http://wcl.zhaomingkeji.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fdx.shanyushiyangkeji.top

[S47] C++：结构化绑定遍历
来源：http://gpd.ivvv.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wiv.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://dqq.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://xgi.c1oappe.top

while (std::getline(in, line)) { }
来源：http://plr.havefunace.top

[S49] C++：写文件
来源：http://unn.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://trp.nwbrower.top

[S50] C++：格式化数字
来源：http://hee.fehbvm.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kmo.yj202588.top

[S51] C++：显式类型转换
来源：http://ecp.yanxiufei.cn

static_cast<double>(a) / b
来源：http://ekc.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://aei.iojbl.cn

int size() const noexcept { return n_; }
来源：http://ghl.yfazqb.com

[S53] C++：移动语义
来源：http://ele.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://jet.meibo888.top

[S54] C++：异常处理
来源：http://vfk.0kj1m.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qpo.jyoumei.cn

[S55] C++：结构化绑定
来源：http://ehe.bjfxy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kpu.nwbrower.top

[S56] C++：optional
来源：http://lpy.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bdb.hammf.cn

[S57] C++：编译期常量
来源：http://irw.zhijiandao.cn

constexpr int N = 10;
来源：http://tdp.yvedp.cn

[S58] C++：命名空间
来源：http://opb.nanxinkj.top

namespace ns { int f() { return 1; } }
来源：http://dyq.tianlin.xyz

[S59] C++：静态断言
来源：http://zev.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dew.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://paw.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lbx.sjlbkw.cn

================================================================================
来源：http://wxd.zdqjudy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kcc.gaohongyu789.top

================================================================================
来源：http://tmo.meibo888.top

[T01] Kotlin：Hello World
来源：http://lmz.cucudq.cn

println("Hello")
来源：http://khz.aibaodan.cn

[T02] Kotlin：变量
来源：http://urc.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xec.cashguo.top

[T03] Kotlin：字符串模板
来源：http://ufy.yj202588.top

"值: $b"
来源：http://kyk.zdqjudy.top

[T04] Kotlin：空安全
来源：http://eiz.iojbl.cn

val n: String? = null;  n?.length
来源：http://ham.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://szf.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mhg.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://sxf.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zoi.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://dww.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://buh.yangfankeji.com

[T08] Kotlin：数据类
来源：http://twi.snrcjt.cn

data class User(val name: String, val age: Int)
来源：http://dfj.pycfn.com

[T09] Kotlin：扩展函数
来源：http://cxl.guowangkeji.top

fun String.exclaim() = this + "!"
来源：http://vyg.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://txs.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ucv.nanxuanxn.top

[T11] Kotlin：协程
来源：http://oai.fehbvm.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://pow.ehwqpu.com

[T12] Kotlin：解构声明
来源：http://xbq.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://qcd.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://dbv.jianghu66.top

val m = mapOf("a" to 1)
来源：http://flt.ydzc1.top

[T14] Kotlin：循环
来源：http://ubl.jqgfzy.top

for (i in 1..10) println(i)
来源：http://gng.xinyue.icu

[T15] Kotlin：接口
来源：http://aqr.shanyushiyangkeji.top

interface Shape { fun area(): Double }
来源：http://eov.yonumen.top

[T16] Swift：Hello World
来源：http://yzy.zdbjq.cn

print("Hello")
来源：http://ebm.yueranfly.top

[T17] Swift：变量与常量
来源：http://poo.sxryk.cn

var a = 1;  let b = 2
来源：http://cop.gogol.net.cn

[T18] Swift：字符串插值
来源：http://cvw.zycfv.cn

"值: \(b)"
来源：http://flm.zhaomingkeji.xyz

[T19] Swift：可选绑定
来源：http://xzu.tianlin.xyz

if let n = opt { print(n) }
来源：http://qrj.gotoacloud.top

[T20] Swift：数组操作
来源：http://wiw.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://bar.jinqigfzy.top

[T21] Swift：遍历
来源：http://rgy.sysykeji.top

for x in a { print(x) }
来源：http://fbf.zhiwuduotai.top

[T22] Swift：字典
来源：http://odo.feifeiyinyue.top

var d = ["a": 1];  d["b"] = 2
来源：http://hwy.quarkkingdee.top

[T23] Swift：函数
来源：http://kal.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fzq.zhongyouzk.top

[T24] Swift：闭包
来源：http://fdg.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gae.cdnleiting.top

[T25] Swift：结构体
来源：http://nym.jinqigfzy.top

struct P { var x: Int }
来源：http://kpu.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://iin.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://hmu.fengsongda.top

[T27] Swift：错误处理
来源：http://rry.ywan-chungtsiang.top

do { try f() } catch { print(error) }
来源：http://zri.ywan-chungtsiang.top

[T28] Swift：枚举
来源：http://hba.ehwqpu.com

enum Color { case red, green }
来源：http://tca.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://zij.cheryme.top

guard let x = opt else { return }
来源：http://ywl.chenjidiqi.icu

[T30] Swift：协议
来源：http://phz.jqgufenzy.top

protocol Shape { func area() -> Double }
来源：http://ttk.316326.xyz

[T31] Lua：Hello World
来源：http://wmw.9152youxi.cn

print("Hello")
来源：http://yja.jianghu66.top

[T32] Lua：局部变量
来源：http://bud.hysaishi.cn

local a = 1
来源：http://ktb.hywenlv.cn

[T33] Lua：表（数组）
来源：http://koh.jlsjyb.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ryr.nanxuanxn.top

[T34] Lua：遍历表
来源：http://gat.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tde.hongshengwenyu.top

[T35] Lua：字典表
来源：http://yxq.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://sgk.wangshuangyany.cn

[T36] Lua：函数
来源：http://ybr.jiagoushi.top

function add(a, b) return a + b end
来源：http://xpf.tianlin.xyz

[T37] Lua：字符串拼接
来源：http://zad.chenlongwang.top

"a" .. "b"
来源：http://hcz.tian-w.cn

[T38] Lua：条件
来源：http://jhn.xziqi.cn

if x > 0 then print("正") end
来源：http://ukt.chenjidiqi.icu


<!-- 参考信息 -->