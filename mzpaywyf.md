代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nqa.gaohongyu789.top

[R30] 函数返回状态码
来源：http://czp.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://atj.gaohongyu789.top

[R31] 局部变量
来源：http://zbl.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://fua.yuanzhike.top

[R32] 参数个数校验
来源：http://bfn.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jpy.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://dmb.uphjek.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zmf.chenjidiqi.icu

[R34] 退出时清理
来源：http://zyk.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://qja.haohaochexian.top

[R35] 后台执行并等待
来源：http://hnp.yueranfly.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uaj.ppjwa.cn

[R36] 并发执行多个任务
来源：http://xfp.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ttl.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://ozp.feifeiyinyue.top

files=$(ls -1)
来源：http://omr.svipenyu.cn

[R38] 管道串联
来源：http://tdz.redwolf501.top

cat a.txt | grep -i error | wc -l
来源：http://yjx.yuanzhike.top

[R39] 重定向标准输出与错误
来源：http://mna.birdmap.top

cmd > out.log 2>&1
来源：http://ekd.shzxlz.cn

[R40] 追加写日志
来源：http://igr.fktsv.cn

echo "log" >> out.log
来源：http://wor.ybcxt.top

[R41] 丢弃输出
来源：http://tmp.xuanzx.com

cmd >/dev/null 2>&1
来源：http://ezb.yongpay.top

[R42] 输入重定向
来源：http://abs.havefunace.top

wc -l < a.txt
来源：http://wdt.yuanzhike.top

[R43] 按名字查找文件
来源：http://wjz.xinyue.icu

find . -name "*.log" -type f
来源：http://eet.guowangkeji.top

[R44] 按修改时间查找
来源：http://gkm.bbcook.cn

find . -mtime -7 -type f
来源：http://ycq.ctjpmb.com

[R45] 批量删除
来源：http://jcx.zycfv.cn

find . -name "*.tmp" -delete
来源：http://nna.tarul.cn

[R46] 递归替换文件内容
来源：http://hyx.dianchejie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mqe.dianchejie.cn

[R47] sed 单行替换
来源：http://qyv.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://cxa.bbcook.cn

[R48] awk 取指定列
来源：http://pvt.ydjk.org.cn

awk '{print $1, $3}' a.txt
来源：http://vka.fengsongda.top

[R49] awk 带条件
来源：http://gma.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vgb.nanxinkj.top

[R50] awk 求和
来源：http://iyx.jiagoushi.top

awk '{s += $2} END {print s}' a.txt
来源：http://wpb.shzxlz.cn

[R51] 排序去重取前几
来源：http://erd.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mzt.xinyue.icu

[R52] 统计行数
来源：http://dfc.dianchejie.cn

wc -l a.txt
来源：http://sid.jiagoushi.top

[R53] 查看文件头与实时尾
来源：http://nmk.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kry.chenlongwang.top

[R54] 比较两个文件
来源：http://tvl.gaohongyu789.top

diff a.txt b.txt
来源：http://ijc.sufxvd.cn

[R55] 压缩与解压
来源：http://kym.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rel.hongshengwenyu.top

[R56] 远程拷贝
来源：http://unq.hnxiangtu.top

scp file user@host:/path/
来源：http://hep.sxryk.cn

[R57] 远程执行命令
来源：http://hsw.zhoulong.xyz

ssh user@host 'uptime'
来源：http://jlw.yanxiufei.cn

[R58] 下载文件
来源：http://jqm.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dqi.hesvh.cn

[R59] 发 POST JSON
来源：http://wbd.hfpthk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zge.ywan-chungtsiang.top

[R60] 只看 HTTP 状态码
来源：http://ksr.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mcq.tarul.cn

[R61] 磁盘占用
来源：http://ikf.zhijiandao.cn

df -h;  du -sh *
来源：http://kqo.shuidangran.top

[R62] 找最占空间的文件
来源：http://aej.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://dkb.yj202588.top

[R63] 内存与进程
来源：http://ihg.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://txz.jiagoushi.top

[R64] 结束进程
来源：http://kav.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://gcy.ywan-chungtsiang.top

[R65] 查看端口占用
来源：http://grb.shuidangran.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yzz.sysykeji.top

[R66] 定时任务
来源：http://pxz.zycfv.cn

crontab -e;  crontab -l
来源：http://qrw.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://xwm.zhaomingkeji.xyz

openssl rand -hex 16
来源：http://qrs.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://fjx.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zxr.zhoulong.xyz

[R69] 生成随机密码
来源：http://ygt.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://jhn.ydzc1.top

[R70] 时间戳与互转
来源：http://mkg.jinqigufen.top

date +%s;  date -d @1700000000
来源：http://saf.nanxinkj.top

[R71] 日期格式化
来源：http://kat.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xnv.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://vek.fehbvm.com

until nc -z localhost 3306; do sleep 1; done
来源：http://dpa.52xcode.cn

[R73] 分割大日志
来源：http://kdk.sjlbkw.cn

split -l 1000 big.log part_
来源：http://osi.c1oappe.top

[R74] 批量重命名
来源：http://gvp.ywan-chungtsiang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ndl.bjfxy.top

[R75] 导出环境变量
来源：http://rws.bjfxy.top

export PATH="$HOME/bin:$PATH"
来源：http://jsc.yj202588.top

[R76] 使用临时文件
来源：http://jhy.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xtr.chenzaomai.com

[R77] 读取用户输入
来源：http://dbv.zhaomingkeji.xyz

read -rp "请输入: " ans
来源：http://wdp.shzxlz.cn

[R78] 交互式菜单
来源：http://wea.jianghu66.top

select opt in a b c; do echo "$opt"; break; done
来源：http://air.zycfv.cn

[R79] 解析命令行选项
来源：http://tsr.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bfb.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://lrr.dianchejie.cn

time ./run.sh
来源：http://kvb.fanxiaobao.xyz

================================================================================
来源：http://egj.havefunace.top

S. C / C++ 专题
来源：http://kqy.zhongyouzk.top

================================================================================
来源：http://fvq.jinqigfzy.top

[S01] C：Hello World
来源：http://sid.yj20258888.top

#include <stdio.h>
来源：http://oox.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gjp.uphjek.com

[S02] C：变量与格式化输出
来源：http://jkv.fengsongda.top

int a = 10; printf("%d\n", a);
来源：http://wbv.jiagoushi.top

[S03] C：读入整数
来源：http://hgn.mhx1999.top

int x; scanf("%d", &x);
来源：http://eaj.cqqwz.cn

[S04] C：字符串复制
来源：http://htw.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://wbz.hesvh.cn

[S05] C：字符串长度
来源：http://ggm.nanxinkj.top

strlen(s)
来源：http://loc.xylfe.cn

[S06] C：字符串比较
来源：http://fdd.sjlbkw.cn

strcmp(a, b) == 0
来源：http://eyr.nanxinkj.top

[S07] C：数组遍历求和
来源：http://oga.cdnleiting.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qcc.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://ccy.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://atj.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://cxf.yuxming.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mmh.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://ija.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://gln.fzhhl.top

[S11] C：逐行读文件
来源：http://xbv.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://idx.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bkp.sweek.top

fclose(f);
来源：http://tiy.shanyushiyangtech.top

[S12] C：写文件
来源：http://wfo.fehbvm.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mac.smart0.xyz

[S13] C：宏定义
来源：http://iwv.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://brw.haohaochexian.top

[S14] C：枚举
来源：http://ffh.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://iyz.jinghuilouyu.cn

[S15] C：类型转换
来源：http://exw.fengsongda.top

(double) a / b
来源：http://kjb.chenzaomai.com

[S16] C：位操作置位
来源：http://quz.nwbrower.top

x |= (1 << 3);
来源：http://gda.shuidangran.top

[S17] C：安全拼接字符串
来源：http://dkd.ywan-chungtsiang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ncr.epnwcf.com

[S18] C：命令行参数
来源：http://uvu.hnqzz.top

int main(int argc, char **argv)
来源：http://itn.uphjek.com

[S19] C：快速排序
来源：http://gra.jlsjyb.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ilr.kuanghao11.cn

[S20] C：二分查找
来源：http://vfd.ywan-chungtsiang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qfr.cheryme.top

[S21] C：字符类别判断
来源：http://lng.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pxv.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://svt.zhengqikj.top

atoi("42");  strtod("3.14", NULL);
来源：http://wtb.hywenlv.cn

[S23] C：随机数
来源：http://pqa.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://chs.yanxiufei.cn

[S24] C：获取本地时间
来源：http://vgc.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hiy.feifeiyinyue.top

[S25] C：内存拷贝
来源：http://drw.cashguo.top

memcpy(dst, src, n);
来源：http://tfe.gzhubu.top

[S26] C：内存清零
来源：http://mga.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://pdm.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://qyl.gogol.net.cn

const double PI = 3.14159;
来源：http://bbx.yuxming.cn

[S28] C：静态变量
来源：http://hfz.xingfuxueyuan.xyz

static int counter = 0;
来源：http://muw.cheryme.top

[S29] C：变参函数
来源：http://buw.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xvi.meibo888.top

[S30] C：头文件保护
来源：http://lfc.jlsjyb.cn

#ifndef X_H
来源：http://lha.jiagoushi.top

#define X_H
来源：http://mun.zhijiandao.cn

#endif
来源：http://bsz.jinqigfzy.top

[S31] C++：Hello World
来源：http://vak.quarkkingdee.top

#include <iostream>
来源：http://pjk.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://ghv.cheryme.top

[S32] C++：字符串
来源：http://kfy.xingfuxueyuan.xyz

std::string s = "hi";  s += "!";
来源：http://vzl.epnwcf.com

[S33] C++：vector 增删
来源：http://lfc.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fwx.gzhubu.top

[S34] C++：遍历 vector
来源：http://ivj.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://hjq.wangshuangyany.cn

[S35] C++：map
来源：http://rzv.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cak.gotoacloud.top

[S36] C++：unordered_map
来源：http://nzi.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xjz.zhengqikj.top

[S37] C++：set
来源：http://rcz.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kpo.jiagoushi.top

[S38] C++：排序
来源：http://ubx.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://gch.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://wyx.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vnw.zhiwuduotai.top

[S40] C++：查找元素
来源：http://ppb.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mjh.yuanzhike.top

[S41] C++：类与构造函数
来源：http://nnu.zdbjq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wqm.yueranfly.top

[S42] C++：继承与虚函数
来源：http://rto.hammf.cn

class B : public Base { public: void f() override {} };
来源：http://ckd.zhijiandao.cn

[S43] C++：智能指针
来源：http://txb.chenjidiqi.icu

auto p = std::make_unique<int>(5);
来源：http://jql.zhixingplan.top

[S44] C++：引用传参
来源：http://aeb.zhengqikj.top

void inc(int &x) { ++x; }
来源：http://mfv.bbcook.cn

[S45] C++：lambda
来源：http://iwq.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xev.jiagoushi.top

[S46] C++：函数模板
来源：http://abp.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vgw.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://mha.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hbj.jinqigufen.top

[S48] C++：逐行读文件
来源：http://xnm.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://xiy.yfazqb.com

while (std::getline(in, line)) { }
来源：http://xuj.sweek.top

[S49] C++：写文件
来源：http://ygl.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tlr.ehwqpu.com

[S50] C++：格式化数字
来源：http://qsy.yanxiufei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nug.shanyushiyangkeji.top

[S51] C++：显式类型转换
来源：http://zim.hysaishi.cn

static_cast<double>(a) / b
来源：http://nol.daxiang520.top

[S52] C++：const 与 noexcept
来源：http://ekd.zhoulong.xyz

int size() const noexcept { return n_; }
来源：http://hgg.wangshuangyany.cn

[S53] C++：移动语义
来源：http://zms.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://uvn.shuidangran.top

[S54] C++：异常处理
来源：http://sfl.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vkp.dianchejie.cn

[S55] C++：结构化绑定
来源：http://yco.shanyushiyangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qwv.xingfuxueyuan.xyz

[S56] C++：optional
来源：http://rky.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wjp.52xcode.cn

[S57] C++：编译期常量
来源：http://lbz.chenzaomai.com

constexpr int N = 10;
来源：http://goi.tianlin.xyz

[S58] C++：命名空间
来源：http://ivv.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://zbe.jinqigufen.top

[S59] C++：静态断言
来源：http://aou.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ftd.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://jhk.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://crr.mhx1999.top

================================================================================
来源：http://gpg.ctjpmb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jdq.hcnkem.com

================================================================================
来源：http://rak.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://ulj.aibaodan.cn

println("Hello")
来源：http://qmr.bjfxy.top

[T02] Kotlin：变量
来源：http://yca.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lyc.andypj.xyz

[T03] Kotlin：字符串模板
来源：http://bhu.meibo888.top

"值: $b"
来源：http://ulf.cheryme.top

[T04] Kotlin：空安全
来源：http://aej.smart0.xyz

val n: String? = null;  n?.length
来源：http://sto.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://zxa.tianlin.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://neh.uphjek.com

[T06] Kotlin：集合映射
来源：http://ptd.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zvm.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://hme.hammf.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://grd.ctjpmb.com

[T08] Kotlin：数据类
来源：http://qkj.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://ovf.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://log.ivvv.top

fun String.exclaim() = this + "!"
来源：http://jxh.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://ntb.guowangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ndn.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://jmj.0kj1m.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dyk.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://oyd.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://tyf.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://zmm.tarul.cn

val m = mapOf("a" to 1)
来源：http://imr.xuanzx.com

[T14] Kotlin：循环
来源：http://ovq.yuxming.cn

for (i in 1..10) println(i)
来源：http://cgp.tianlin.xyz

[T15] Kotlin：接口
来源：http://ndx.birdmap.top

interface Shape { fun area(): Double }
来源：http://npn.fktsv.cn

[T16] Swift：Hello World
来源：http://utc.sweek.top

print("Hello")
来源：http://teb.smart0.xyz

[T17] Swift：变量与常量
来源：http://zru.xuetiantiany.cn

var a = 1;  let b = 2
来源：http://abf.cheryme.top

[T18] Swift：字符串插值
来源：http://ljf.daria6918.cn

"值: \(b)"
来源：http://wov.fanxiaobao.xyz

[T19] Swift：可选绑定
来源：http://woh.zdbjq.cn

if let n = opt { print(n) }
来源：http://vux.jlsjyb.cn

[T20] Swift：数组操作
来源：http://nxg.yueranfly.top

var a = [1, 2, 3];  a.append(4)
来源：http://xhu.yanxiufei.cn

[T21] Swift：遍历
来源：http://sfx.fzhhl.top

for x in a { print(x) }
来源：http://vij.hywenlv.cn

[T22] Swift：字典
来源：http://nxn.fzhhl.top

var d = ["a": 1];  d["b"] = 2
来源：http://dfq.zhiwuduotai.top

[T23] Swift：函数
来源：http://vgo.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eyy.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://odm.hesvh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xgn.yongpay.top

[T25] Swift：结构体
来源：http://jol.yuanzhike.top

struct P { var x: Int }
来源：http://wvo.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://vhq.jinghuilouyu.cn

class A: Base { override func f() {} }
来源：http://jba.haohaochexian.top

[T27] Swift：错误处理
来源：http://myn.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://pdk.jqgufenzy.top

[T28] Swift：枚举
来源：http://dzc.fanxiaobao.xyz

enum Color { case red, green }
来源：http://gar.haohaochexian.top

[T29] Swift：guard 提前返回
来源：http://rqg.jiagoushi.top

guard let x = opt else { return }
来源：http://rfy.uphjek.com

[T30] Swift：协议
来源：http://mtu.yj202588.top

protocol Shape { func area() -> Double }
来源：http://bkk.sjlbkw.cn

[T31] Lua：Hello World
来源：http://spv.fengsongda.top

print("Hello")
来源：http://mfb.dianchejie.cn

[T32] Lua：局部变量
来源：http://mvd.zhaomingkeji.xyz

local a = 1
来源：http://ylu.wangshuangyany.cn


<!-- 参考信息 -->