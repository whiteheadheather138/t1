代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uho.fzhhl.top

[R34] 退出时清理
来源：http://sdz.ywan-chungtsiang.top

trap 'rm -f "$tmp"' EXIT
来源：http://gzo.jinqigufen.top

[R35] 后台执行并等待
来源：http://sys.havefunace.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kvu.yuxming.cn

[R36] 并发执行多个任务
来源：http://ypp.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xzf.gotoacloud.top

[R37] 把输出赋给变量
来源：http://ugk.gogol.net.cn

files=$(ls -1)
来源：http://jgt.yangfankeji.com

[R38] 管道串联
来源：http://fve.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://ldz.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://zvj.wangdashe.top

cmd > out.log 2>&1
来源：http://uhb.zhixingplan.top

[R40] 追加写日志
来源：http://oon.jinghuilouyu.cn

echo "log" >> out.log
来源：http://tww.hammf.cn

[R41] 丢弃输出
来源：http://slc.hammf.cn

cmd >/dev/null 2>&1
来源：http://zoh.feifeiyinyue.top

[R42] 输入重定向
来源：http://etv.yanxiufei.cn

wc -l < a.txt
来源：http://ldo.ehwqpu.com

[R43] 按名字查找文件
来源：http://ith.gaohongyu789.top

find . -name "*.log" -type f
来源：http://sww.mhx1999.top

[R44] 按修改时间查找
来源：http://dvc.jqgfzy.top

find . -mtime -7 -type f
来源：http://hiq.shzxlz.cn

[R45] 批量删除
来源：http://hwd.sxryk.cn

find . -name "*.tmp" -delete
来源：http://chr.meibo888.top

[R46] 递归替换文件内容
来源：http://mvs.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://prb.sweek.top

[R47] sed 单行替换
来源：http://pax.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://mnr.redwolf501.top

[R48] awk 取指定列
来源：http://gte.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://ptz.zycfv.cn

[R49] awk 带条件
来源：http://tym.guannengcc.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bjj.dashuyun.cn

[R50] awk 求和
来源：http://xoq.wangdashe.top

awk '{s += $2} END {print s}' a.txt
来源：http://xxn.cashguo.top

[R51] 排序去重取前几
来源：http://pry.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://byj.svipenyu.cn

[R52] 统计行数
来源：http://hxn.ehwqpu.com

wc -l a.txt
来源：http://ryg.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://geh.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fer.zhongyouzk.top

[R54] 比较两个文件
来源：http://jta.xuetiantiany.cn

diff a.txt b.txt
来源：http://xoa.ybcxt.top

[R55] 压缩与解压
来源：http://ggl.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kdi.mhx1999.top

[R56] 远程拷贝
来源：http://yvi.ehwqpu.com

scp file user@host:/path/
来源：http://rxh.yongpay.top

[R57] 远程执行命令
来源：http://new.xuanzx.com

ssh user@host 'uptime'
来源：http://nfu.shzxlz.cn

[R58] 下载文件
来源：http://tsd.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xca.iojbl.cn

[R59] 发 POST JSON
来源：http://zjq.nanxinkj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wrh.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://gga.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hhs.gogol.net.cn

[R61] 磁盘占用
来源：http://ymu.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://kwl.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://lgt.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://fvp.xylfe.cn

[R63] 内存与进程
来源：http://yta.xinyue.icu

free -h;  ps aux | grep nginx
来源：http://afo.zhiwuduotai.top

[R64] 结束进程
来源：http://ath.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://bta.havefunace.top

[R65] 查看端口占用
来源：http://sqz.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://awf.316326.xyz

[R66] 定时任务
来源：http://xob.fengsongda.top

crontab -e;  crontab -l
来源：http://vty.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://rpa.ydzc1.top

openssl rand -hex 16
来源：http://edl.jiagoushi.top

[R68] 计算文件校验值
来源：http://zzw.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://tjd.yuanzhike.top

[R69] 生成随机密码
来源：http://hvn.cdnleiting.top

head -c 16 /dev/urandom | base64
来源：http://cxt.guowangkeji.top

[R70] 时间戳与互转
来源：http://jao.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://kss.kuanghao11.cn

[R71] 日期格式化
来源：http://qxo.jqgufenzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xol.gogol.net.cn

[R72] 等待端口就绪
来源：http://auh.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kum.tanke756.top

[R73] 分割大日志
来源：http://nsv.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://yit.zhoulong.xyz

[R74] 批量重命名
来源：http://rae.nanxinkj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mnh.shzxlz.cn

[R75] 导出环境变量
来源：http://hit.ydzc1.top

export PATH="$HOME/bin:$PATH"
来源：http://wwi.0kj1m.cn

[R76] 使用临时文件
来源：http://kri.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wyu.ehwqpu.com

[R77] 读取用户输入
来源：http://ybh.yuanzhike.top

read -rp "请输入: " ans
来源：http://tej.jqgfzy.top

[R78] 交互式菜单
来源：http://pqx.ywan-chungtsiang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qfo.yj20258.top

[R79] 解析命令行选项
来源：http://nco.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ttw.zhijiandao.cn

[R80] 查看脚本执行耗时
来源：http://fpy.hongshengwenyu.top

time ./run.sh
来源：http://opx.fanxiaobao.xyz

================================================================================
来源：http://jgj.xuetiantiany.cn

S. C / C++ 专题
来源：http://fon.tian-w.cn

================================================================================
来源：http://kyk.haohaochexian.top

[S01] C：Hello World
来源：http://rav.sjlbkw.cn

#include <stdio.h>
来源：http://wps.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mzp.uphjek.com

[S02] C：变量与格式化输出
来源：http://vjr.mhx1999.top

int a = 10; printf("%d\n", a);
来源：http://fjx.52xcode.cn

[S03] C：读入整数
来源：http://goq.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://mgh.zhengqikj.top

[S04] C：字符串复制
来源：http://zjg.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://xne.zhoulong.xyz

[S05] C：字符串长度
来源：http://kxr.ydjk.org.cn

strlen(s)
来源：http://mch.smart0.xyz

[S06] C：字符串比较
来源：http://sdz.hcnkem.com

strcmp(a, b) == 0
来源：http://pql.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://fxm.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bfg.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://hgv.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qou.gzhubu.top

[S09] C：结构体定义与初始化
来源：http://xsn.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kxn.sysykeji.top

[S10] C：指针与解引用
来源：http://ila.birdmap.top

int *p = &a;  *p = 5;
来源：http://dzn.hysaishi.cn

[S11] C：逐行读文件
来源：http://cps.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://qlt.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pyl.hongshengwenyu.top

fclose(f);
来源：http://cny.daxiang520.top

[S12] C：写文件
来源：http://kuu.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dgd.fanxiaobao.xyz

[S13] C：宏定义
来源：http://xfi.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jar.ppjwa.cn

[S14] C：枚举
来源：http://kth.fanxiaobao.xyz

enum Color { RED, GREEN, BLUE };
来源：http://utd.mhx1999.top

[S15] C：类型转换
来源：http://mfv.vehdjk.com

(double) a / b
来源：http://axl.zhijiandao.cn

[S16] C：位操作置位
来源：http://abb.yvedp.cn

x |= (1 << 3);
来源：http://uba.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://svk.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ahn.9152youxi.cn

[S18] C：命令行参数
来源：http://wum.dashuyun.cn

int main(int argc, char **argv)
来源：http://ggl.chenlongwang.top

[S19] C：快速排序
来源：http://flt.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rms.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://xph.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qul.fehbvm.com

[S21] C：字符类别判断
来源：http://aew.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wug.hysaishi.cn

[S22] C：字符串转数字
来源：http://uni.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://ion.aibaodan.cn

[S23] C：随机数
来源：http://kez.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://amg.pengpengdd.cyou

[S24] C：获取本地时间
来源：http://dsp.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qjc.zhoulong.xyz

[S25] C：内存拷贝
来源：http://apn.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://vxz.havefunace.top

[S26] C：内存清零
来源：http://qbg.epnwcf.com

memset(a, 0, sizeof a);
来源：http://zdv.zhongyouzk.top

[S27] C：定义常量
来源：http://vkm.zhixingplan.top

const double PI = 3.14159;
来源：http://eei.c1oappe.top

[S28] C：静态变量
来源：http://vwq.vqdsnc.cn

static int counter = 0;
来源：http://qqp.uphjek.com

[S29] C：变参函数
来源：http://jvc.ppjwa.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qux.sjlbkw.cn

[S30] C：头文件保护
来源：http://rxa.ivvv.top

#ifndef X_H
来源：http://igp.wangshuangyany.cn

#define X_H
来源：http://qst.shanyushiyangtech.top

#endif
来源：http://hms.meibo888.top

[S31] C++：Hello World
来源：http://hwh.zhongyouzk.top

#include <iostream>
来源：http://axd.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://amf.jyoumei.cn

[S32] C++：字符串
来源：http://mus.zhaomingkeji.xyz

std::string s = "hi";  s += "!";
来源：http://nhk.zdbjq.cn

[S33] C++：vector 增删
来源：http://atz.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jjp.feifeiyinyue.top

[S34] C++：遍历 vector
来源：http://rdo.yongpay.top

for (auto &x : v) { std::cout << x; }
来源：http://lgv.zhiwuduotai.top

[S35] C++：map
来源：http://ovl.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hif.haohaochexian.top

[S36] C++：unordered_map
来源：http://ysi.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jhy.nanxinkj.top

[S37] C++：set
来源：http://zft.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://okd.hywenlv.cn

[S38] C++：排序
来源：http://nkf.ybcxt.top

std::sort(v.begin(), v.end());
来源：http://fhu.sufxvd.cn

[S39] C++：自定义比较器排序
来源：http://bpj.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rcd.fengsongda.top

[S40] C++：查找元素
来源：http://vzl.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ozi.birdmap.top

[S41] C++：类与构造函数
来源：http://eym.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bek.sysykeji.top

[S42] C++：继承与虚函数
来源：http://hbz.yueranfly.top

class B : public Base { public: void f() override {} };
来源：http://sjg.andypj.xyz

[S43] C++：智能指针
来源：http://oly.sxryk.cn

auto p = std::make_unique<int>(5);
来源：http://pfy.zhixingplan.top

[S44] C++：引用传参
来源：http://psk.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://bvp.xuanzx.com

[S45] C++：lambda
来源：http://sex.chenjidiqi.icu

auto add = [](int a, int b) { return a + b; };
来源：http://obb.havefunace.top

[S46] C++：函数模板
来源：http://qqh.xinyue.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://flv.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://fje.ywan-chungtsiang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bxr.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://xpj.zhaomingkeji.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://rjz.yuxming.cn

while (std::getline(in, line)) { }
来源：http://jpi.ehwqpu.com

[S49] C++：写文件
来源：http://mdv.ehwqpu.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vis.hammf.cn

[S50] C++：格式化数字
来源：http://jsk.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nmp.hammf.cn

[S51] C++：显式类型转换
来源：http://ban.cdnleiting.top

static_cast<double>(a) / b
来源：http://tuo.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://asq.c1oappe.top

int size() const noexcept { return n_; }
来源：http://shv.tarul.cn

[S53] C++：移动语义
来源：http://llb.ywan-chungtsiang.top

std::vector<int> w = std::move(v);
来源：http://yza.xinyue.icu

[S54] C++：异常处理
来源：http://san.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vjl.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://jdz.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lup.cheryme.top

[S56] C++：optional
来源：http://nhz.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eci.ybcxt.top

[S57] C++：编译期常量
来源：http://omi.xuanzx.com

constexpr int N = 10;
来源：http://tlo.birdmap.top

[S58] C++：命名空间
来源：http://oej.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://xjy.chenlongwang.top

[S59] C++：静态断言
来源：http://gfz.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gek.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://iet.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nka.ydjk.org.cn

================================================================================
来源：http://dmf.cqqwz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sfh.havefunace.top

================================================================================
来源：http://zan.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://bcw.yj202588.top

println("Hello")
来源：http://gpe.hnqzz.top

[T02] Kotlin：变量
来源：http://hgl.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cos.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://xlw.cdnleiting.top

"值: $b"
来源：http://dct.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://ani.jiagoushi.top

val n: String? = null;  n?.length
来源：http://fmm.yj20258888.top

[T05] Kotlin：when 表达式
来源：http://fif.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kot.bbcook.cn

[T06] Kotlin：集合映射
来源：http://cfb.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gia.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://zfa.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lrq.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://qyb.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://qyj.yanxiufei.cn

[T09] Kotlin：扩展函数
来源：http://yml.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://kfb.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://onf.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cgu.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://ycq.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tny.shangyingyoupin.top

[T12] Kotlin：解构声明
来源：http://wln.c1oappe.top

val (a, b) = Pair(1, 2)
来源：http://lvp.shanyushiyangkeji.top

[T13] Kotlin：只读 Map
来源：http://alh.fzhhl.top

val m = mapOf("a" to 1)
来源：http://uvm.zhongyouzk.top

[T14] Kotlin：循环
来源：http://ysf.yueranfly.top

for (i in 1..10) println(i)
来源：http://gqm.mhx1999.top

[T15] Kotlin：接口
来源：http://jgu.0kj1m.cn

interface Shape { fun area(): Double }
来源：http://cbb.ctjpmb.com

[T16] Swift：Hello World
来源：http://pcv.hysaishi.cn

print("Hello")
来源：http://xjy.chenlongwang.top

[T17] Swift：变量与常量
来源：http://kgg.52xcode.cn

var a = 1;  let b = 2
来源：http://dpd.cucudq.cn

[T18] Swift：字符串插值
来源：http://utx.daxiang520.top

"值: \(b)"
来源：http://vvi.guowangkeji.top

[T19] Swift：可选绑定
来源：http://mqn.yvedp.cn

if let n = opt { print(n) }
来源：http://yox.svipenyu.cn

[T20] Swift：数组操作
来源：http://lmu.ehwqpu.com

var a = [1, 2, 3];  a.append(4)
来源：http://ous.zhongyouzk.top

[T21] Swift：遍历
来源：http://hbg.snrcjt.cn

for x in a { print(x) }
来源：http://jmv.hnqzz.top

[T22] Swift：字典
来源：http://kby.yvedp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://esf.tianlin.xyz

[T23] Swift：函数
来源：http://ner.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mjf.zdbjq.cn

[T24] Swift：闭包
来源：http://efq.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://xqn.yongpay.top

[T25] Swift：结构体
来源：http://ukp.hongshengwenyu.top

struct P { var x: Int }
来源：http://pud.dianchejie.cn

[T26] Swift：类与重写
来源：http://bvz.yangfankeji.com

class A: Base { override func f() {} }
来源：http://jfr.jlsjyb.cn

[T27] Swift：错误处理
来源：http://bms.tanke756.top

do { try f() } catch { print(error) }
来源：http://cpq.wangdashe.top

[T28] Swift：枚举
来源：http://uck.hywenlv.cn

enum Color { case red, green }
来源：http://ztz.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://zze.yj202588.top

guard let x = opt else { return }
来源：http://fcy.guannengcc.top

[T30] Swift：协议
来源：http://kmr.ydzc1.top

protocol Shape { func area() -> Double }
来源：http://knn.gaohongyu789.top

[T31] Lua：Hello World
来源：http://fhi.zdbjq.cn

print("Hello")
来源：http://vjv.guowangkeji.top

[T32] Lua：局部变量
来源：http://euf.jlsjyb.cn

local a = 1
来源：http://lbs.mhx1999.top

[T33] Lua：表（数组）
来源：http://ixg.jinghuilouyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://voq.ydjk.org.cn

[T34] Lua：遍历表
来源：http://ybt.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rah.tarul.cn

[T35] Lua：字典表
来源：http://cbw.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://qwa.xinyue.icu

[T36] Lua：函数
来源：http://kwp.fengsongda.top

function add(a, b) return a + b end
来源：http://bos.wangdashe.top


<!-- 参考信息 -->