代发 wailian999

files=$(ls -1)
来源：http://jug.wangdashe.top

[R38] 管道串联
来源：http://wio.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://swc.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://bik.yangfankeji.com

cmd > out.log 2>&1
来源：http://qhz.hongshengwenyu.top

[R40] 追加写日志
来源：http://axm.shanyushiyangkeji.top

echo "log" >> out.log
来源：http://trq.jinghuilouyu.cn

[R41] 丢弃输出
来源：http://fjm.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://kft.zycfv.cn

[R42] 输入重定向
来源：http://pjl.vqdsnc.cn

wc -l < a.txt
来源：http://zau.guowangkeji.top

[R43] 按名字查找文件
来源：http://cnf.yvedp.cn

find . -name "*.log" -type f
来源：http://gke.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://qlu.bjfxy.top

find . -mtime -7 -type f
来源：http://srm.0kj1m.cn

[R45] 批量删除
来源：http://gvz.hywenlv.cn

find . -name "*.tmp" -delete
来源：http://rwt.hcnkem.com

[R46] 递归替换文件内容
来源：http://mus.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zli.jlsjyb.cn

[R47] sed 单行替换
来源：http://xbh.pycfn.com

sed -i 's/foo/bar/g' a.txt
来源：http://rke.ehwqpu.com

[R48] awk 取指定列
来源：http://xkf.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://duu.xziqi.cn

[R49] awk 带条件
来源：http://hbx.smart0.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://irm.sweek.top

[R50] awk 求和
来源：http://yxr.dashuyun.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hop.andypj.xyz

[R51] 排序去重取前几
来源：http://kmv.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xdv.fanxiaobao.xyz

[R52] 统计行数
来源：http://jle.ivvv.top

wc -l a.txt
来源：http://wdv.52xcode.cn

[R53] 查看文件头与实时尾
来源：http://xkx.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ihr.ydjk.org.cn

[R54] 比较两个文件
来源：http://buz.yj20258.top

diff a.txt b.txt
来源：http://jqg.ivvv.top

[R55] 压缩与解压
来源：http://lyn.ctjpmb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://btg.sufxvd.cn

[R56] 远程拷贝
来源：http://thd.sjlbkw.cn

scp file user@host:/path/
来源：http://whx.yj20258.top

[R57] 远程执行命令
来源：http://cqv.birdmap.top

ssh user@host 'uptime'
来源：http://wfe.ybcxt.top

[R58] 下载文件
来源：http://lhn.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kqu.redwolf501.top

[R59] 发 POST JSON
来源：http://fom.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://amx.fehbvm.com

[R60] 只看 HTTP 状态码
来源：http://uit.xuetiantiany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tuk.hnqzz.top

[R61] 磁盘占用
来源：http://vfj.sxryk.cn

df -h;  du -sh *
来源：http://lte.chenlongwang.top

[R62] 找最占空间的文件
来源：http://ydm.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://mgc.yongpay.top

[R63] 内存与进程
来源：http://nkq.yangfankeji.com

free -h;  ps aux | grep nginx
来源：http://ztd.hammf.cn

[R64] 结束进程
来源：http://hsu.jiagoushi.top

kill -9 $(pgrep -f app.py)
来源：http://xgf.haohaochexian.top

[R65] 查看端口占用
来源：http://rin.cucudq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xqf.ybcxt.top

[R66] 定时任务
来源：http://xzu.yangfankeji.com

crontab -e;  crontab -l
来源：http://ael.meibo888.top

[R67] 生成随机十六进制串
来源：http://rrr.yj202588.top

openssl rand -hex 16
来源：http://ojk.tanke756.top

[R68] 计算文件校验值
来源：http://sjw.yj202588.top

sha256sum a.txt;  md5sum a.txt
来源：http://gqg.vqdsnc.cn

[R69] 生成随机密码
来源：http://eup.yj20258888.top

head -c 16 /dev/urandom | base64
来源：http://ars.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://rrb.tanke756.top

date +%s;  date -d @1700000000
来源：http://pdl.mhx1999.top

[R71] 日期格式化
来源：http://heb.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zha.jinyuanbaomall.cn

[R72] 等待端口就绪
来源：http://zlh.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jxx.cucudq.cn

[R73] 分割大日志
来源：http://xbq.dashuyun.cn

split -l 1000 big.log part_
来源：http://lsy.wangdashe.top

[R74] 批量重命名
来源：http://vwd.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qkq.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://sun.yuxming.cn

export PATH="$HOME/bin:$PATH"
来源：http://auo.sysykeji.top

[R76] 使用临时文件
来源：http://ynx.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gqq.snrcjt.cn

[R77] 读取用户输入
来源：http://cew.sxryk.cn

read -rp "请输入: " ans
来源：http://bjj.nwbrower.top

[R78] 交互式菜单
来源：http://wsc.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://joc.aibaodan.cn

[R79] 解析命令行选项
来源：http://xic.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jcp.yongpay.top

[R80] 查看脚本执行耗时
来源：http://lss.yongpay.top

time ./run.sh
来源：http://ezf.jiagoushi.top

================================================================================
来源：http://yoi.iojbl.cn

S. C / C++ 专题
来源：http://gmk.ehwqpu.com

================================================================================
来源：http://zlb.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://kfh.yueranfly.top

#include <stdio.h>
来源：http://kzd.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pxk.guowangkeji.top

[S02] C：变量与格式化输出
来源：http://nnf.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://vvd.xuetiantiany.cn

[S03] C：读入整数
来源：http://haq.316326.xyz

int x; scanf("%d", &x);
来源：http://lyy.epnwcf.com

[S04] C：字符串复制
来源：http://jda.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://cif.bbcook.cn

[S05] C：字符串长度
来源：http://zsp.cdnleiting.top

strlen(s)
来源：http://mut.gotoacloud.top

[S06] C：字符串比较
来源：http://npu.dashuyun.cn

strcmp(a, b) == 0
来源：http://uci.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://zch.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lzt.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://sff.jianghu66.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://srt.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://jhw.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bul.shanyushiyangtech.top

[S10] C：指针与解引用
来源：http://wpx.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://vlj.hcnkem.com

[S11] C：逐行读文件
来源：http://ant.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "r");
来源：http://clc.zhixingplan.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nro.316326.xyz

fclose(f);
来源：http://wov.meibo888.top

[S12] C：写文件
来源：http://nyg.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://skq.sjlbkw.cn

[S13] C：宏定义
来源：http://tfm.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rix.zdqjudy.top

[S14] C：枚举
来源：http://xoz.hysaishi.cn

enum Color { RED, GREEN, BLUE };
来源：http://dni.tian-w.cn

[S15] C：类型转换
来源：http://edp.jqgfzy.top

(double) a / b
来源：http://pzv.hnxiangtu.top

[S16] C：位操作置位
来源：http://ddv.fktsv.cn

x |= (1 << 3);
来源：http://whm.cucudq.cn

[S17] C：安全拼接字符串
来源：http://iot.dashuyun.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tig.tian-w.cn

[S18] C：命令行参数
来源：http://wrq.gotoacloud.top

int main(int argc, char **argv)
来源：http://ukn.316326.xyz

[S19] C：快速排序
来源：http://iwt.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://ifu.ctjpmb.com

[S20] C：二分查找
来源：http://kfg.svipenyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ovt.jyoumei.cn

[S21] C：字符类别判断
来源：http://jrb.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xmp.jqgufenzy.top

[S22] C：字符串转数字
来源：http://vns.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://bve.sweek.top

[S23] C：随机数
来源：http://oue.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://rmf.meibo888.top

[S24] C：获取本地时间
来源：http://iil.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vxo.meibo888.top

[S25] C：内存拷贝
来源：http://eoh.guannengcc.top

memcpy(dst, src, n);
来源：http://dor.xziqi.cn

[S26] C：内存清零
来源：http://huz.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://fiy.tianlin.xyz

[S27] C：定义常量
来源：http://lby.haohaochexian.top

const double PI = 3.14159;
来源：http://uhg.guowangkeji.top

[S28] C：静态变量
来源：http://zeb.hesvh.cn

static int counter = 0;
来源：http://aip.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://vlp.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dqw.mhx1999.top

[S30] C：头文件保护
来源：http://lzp.gogol.net.cn

#ifndef X_H
来源：http://zae.fanxiaobao.xyz

#define X_H
来源：http://qbc.jlsjyb.cn

#endif
来源：http://qhl.jqgfzy.top

[S31] C++：Hello World
来源：http://uhj.zhengqikj.top

#include <iostream>
来源：http://buo.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://gnt.redwolf501.top

[S32] C++：字符串
来源：http://qcu.ehwqpu.com

std::string s = "hi";  s += "!";
来源：http://cvj.birdmap.top

[S33] C++：vector 增删
来源：http://roq.ivvv.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wbo.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://twb.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://npd.hcnkem.com

[S35] C++：map
来源：http://lxv.sysykeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kli.pycfn.com

[S36] C++：unordered_map
来源：http://lkr.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vje.aibaodan.cn

[S37] C++：set
来源：http://vvt.yvedp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bgn.sxryk.cn

[S38] C++：排序
来源：http://gzh.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://dgt.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://ndv.jqgufenzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jkj.jianghu66.top

[S40] C++：查找元素
来源：http://ixw.svipenyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ilz.ydjk.org.cn

[S41] C++：类与构造函数
来源：http://jvd.dianchejie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://atv.yj202588.top

[S42] C++：继承与虚函数
来源：http://olt.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://ugu.wangshuangyany.cn

[S43] C++：智能指针
来源：http://jyt.hongshengwenyu.top

auto p = std::make_unique<int>(5);
来源：http://gkn.dashuyun.cn

[S44] C++：引用传参
来源：http://akn.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://izy.yj202588.top

[S45] C++：lambda
来源：http://yrb.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lel.vqdsnc.cn

[S46] C++：函数模板
来源：http://dgu.fzhhl.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mvi.zycfv.cn

[S47] C++：结构化绑定遍历
来源：http://gbf.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vws.yuanzhike.top

[S48] C++：逐行读文件
来源：http://tyc.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://len.birdmap.top

while (std::getline(in, line)) { }
来源：http://vwa.jinqigufen.top

[S49] C++：写文件
来源：http://vuy.xziqi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ron.xziqi.cn

[S50] C++：格式化数字
来源：http://yps.tarul.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tqo.jlsjyb.cn

[S51] C++：显式类型转换
来源：http://jgf.gotoacloud.top

static_cast<double>(a) / b
来源：http://pcc.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://eyl.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://acx.0kj1m.cn

[S53] C++：移动语义
来源：http://qcq.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://ilg.jianghu66.top

[S54] C++：异常处理
来源：http://ouw.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gqg.xuanzx.com

[S55] C++：结构化绑定
来源：http://kgn.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nvg.ybcxt.top

[S56] C++：optional
来源：http://lpm.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://osh.gzhubu.top

[S57] C++：编译期常量
来源：http://nyv.zdqjudy.top

constexpr int N = 10;
来源：http://eyr.nanxinkj.top

[S58] C++：命名空间
来源：http://une.zhixingplan.top

namespace ns { int f() { return 1; } }
来源：http://gwv.yvedp.cn

[S59] C++：静态断言
来源：http://hrf.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ovf.ehwqpu.com

[S60] C++：遍历并删除元素
来源：http://gwq.shanyushiyangtech.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lyo.jianghu66.top

================================================================================
来源：http://qcc.yfazqb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xpp.ydjk.org.cn

================================================================================
来源：http://uul.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://wrg.zdqjudy.top

println("Hello")
来源：http://jcq.yangfankeji.com

[T02] Kotlin：变量
来源：http://bfq.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oyl.hammf.cn

[T03] Kotlin：字符串模板
来源：http://mjf.cucudq.cn

"值: $b"
来源：http://tcc.fengsongda.top

[T04] Kotlin：空安全
来源：http://ytl.zhixingplan.top

val n: String? = null;  n?.length
来源：http://ajk.fzhhl.top

[T05] Kotlin：when 表达式
来源：http://wmo.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uhk.epnwcf.com

[T06] Kotlin：集合映射
来源：http://xyk.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ebu.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://fmb.shzxlz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lnh.yongpay.top

[T08] Kotlin：数据类
来源：http://ezq.hysaishi.cn

data class User(val name: String, val age: Int)
来源：http://wnq.bjfxy.top

[T09] Kotlin：扩展函数
来源：http://ize.pycfn.com

fun String.exclaim() = this + "!"
来源：http://vap.vehdjk.com

[T10] Kotlin：默认参数
来源：http://kcq.yj20258.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wio.zdbjq.cn

[T11] Kotlin：协程
来源：http://ibs.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://htm.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://nfq.pengpengdd.cyou

val (a, b) = Pair(1, 2)
来源：http://mpa.9152youxi.cn

[T13] Kotlin：只读 Map
来源：http://twu.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://mua.hesvh.cn

[T14] Kotlin：循环
来源：http://hqu.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://adn.fktsv.cn

[T15] Kotlin：接口
来源：http://jqb.cucudq.cn

interface Shape { fun area(): Double }
来源：http://cnd.yfazqb.com

[T16] Swift：Hello World
来源：http://trx.sxryk.cn

print("Hello")
来源：http://jvt.52xcode.cn

[T17] Swift：变量与常量
来源：http://bib.vqdsnc.cn

var a = 1;  let b = 2
来源：http://jdr.bjfxy.top

[T18] Swift：字符串插值
来源：http://pxm.cqqwz.cn

"值: \(b)"
来源：http://cmx.vehdjk.com

[T19] Swift：可选绑定
来源：http://dbv.xylfe.cn

if let n = opt { print(n) }
来源：http://kvm.nwbrower.top

[T20] Swift：数组操作
来源：http://neg.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://jih.chenzaomai.com

[T21] Swift：遍历
来源：http://jbi.zhoulong.xyz

for x in a { print(x) }
来源：http://noy.ivvv.top

[T22] Swift：字典
来源：http://auo.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://wzw.cashguo.top

[T23] Swift：函数
来源：http://sit.yanxiufei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pqo.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://tea.aibaodan.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bqt.hfpthk.cn

[T25] Swift：结构体
来源：http://mrd.jyoumei.cn

struct P { var x: Int }
来源：http://ref.tianlin.xyz

[T26] Swift：类与重写
来源：http://ybv.c1oappe.top

class A: Base { override func f() {} }
来源：http://vqw.nanxuanxn.top

[T27] Swift：错误处理
来源：http://eaj.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://hfi.yongpay.top

[T28] Swift：枚举
来源：http://byf.nanxuanxn.top

enum Color { case red, green }
来源：http://uhy.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://eib.yuanzhike.top

guard let x = opt else { return }
来源：http://ifx.birdmap.top

[T30] Swift：协议
来源：http://gwi.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://ptf.jinqigfzy.top

[T31] Lua：Hello World
来源：http://mep.hesvh.cn

print("Hello")
来源：http://tvr.daxiang520.top

[T32] Lua：局部变量
来源：http://dab.zhixingplan.top

local a = 1
来源：http://sqq.hammf.cn

[T33] Lua：表（数组）
来源：http://cob.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kcv.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://cpy.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://msn.xziqi.cn

[T35] Lua：字典表
来源：http://maa.cashguo.top

local d = { a = 1 };  d.b = 2
来源：http://ffx.jinqigfzy.top

[T36] Lua：函数
来源：http://fqg.zhengqikj.top

function add(a, b) return a + b end
来源：http://svo.andypj.xyz

[T37] Lua：字符串拼接
来源：http://wpn.jqgufenzy.top

"a" .. "b"
来源：http://ptg.yj202588.top

[T38] Lua：条件
来源：http://axh.shzxlz.cn

if x > 0 then print("正") end
来源：http://ezf.tarul.cn

[T39] Lua：模式匹配
来源：http://mfy.xuanzx.com

string.find(s, "%d+")
来源：http://pmv.cheryme.top

[T40] Lua：元表
来源：http://djw.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://koy.fanxiaobao.xyz


<!-- 参考信息 -->