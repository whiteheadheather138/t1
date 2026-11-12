代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://cws.xziqi.cn

[R32] 参数个数校验
来源：http://zue.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://quh.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://rfd.feifeiyinyue.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qqn.sysykeji.top

[R34] 退出时清理
来源：http://fwp.smart0.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ken.hesvh.cn

[R35] 后台执行并等待
来源：http://njq.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yap.cheryme.top

[R36] 并发执行多个任务
来源：http://qxd.bbcook.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gvl.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://fsj.dashuyun.cn

files=$(ls -1)
来源：http://rim.zhoulong.xyz

[R38] 管道串联
来源：http://bhk.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://iak.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://dfd.zhengqikj.top

cmd > out.log 2>&1
来源：http://edo.haohaochexian.top

[R40] 追加写日志
来源：http://fpz.ppjwa.cn

echo "log" >> out.log
来源：http://voc.feifeiyinyue.top

[R41] 丢弃输出
来源：http://rug.hesvh.cn

cmd >/dev/null 2>&1
来源：http://yuz.gzhubu.top

[R42] 输入重定向
来源：http://tfu.hywenlv.cn

wc -l < a.txt
来源：http://lhp.haohaochexian.top

[R43] 按名字查找文件
来源：http://zja.xylfe.cn

find . -name "*.log" -type f
来源：http://uqh.ydzc1.top

[R44] 按修改时间查找
来源：http://kxx.tian-w.cn

find . -mtime -7 -type f
来源：http://unf.jqgufenzy.top

[R45] 批量删除
来源：http://hik.vqdsnc.cn

find . -name "*.tmp" -delete
来源：http://dvh.tarul.cn

[R46] 递归替换文件内容
来源：http://ico.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://doe.chenlongwang.top

[R47] sed 单行替换
来源：http://noo.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://ldn.redwolf501.top

[R48] awk 取指定列
来源：http://rrm.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://rog.gaohongyu789.top

[R49] awk 带条件
来源：http://xew.jinqigfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xzc.c1oappe.top

[R50] awk 求和
来源：http://axo.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wzl.fktsv.cn

[R51] 排序去重取前几
来源：http://fvg.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bgr.dianchejie.cn

[R52] 统计行数
来源：http://rmr.hnqzz.top

wc -l a.txt
来源：http://mao.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://bmp.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rse.guannengcc.top

[R54] 比较两个文件
来源：http://ilr.guowangkeji.top

diff a.txt b.txt
来源：http://hcc.xuetiantiany.cn

[R55] 压缩与解压
来源：http://gpx.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://brh.chenlongwang.top

[R56] 远程拷贝
来源：http://biy.ydzc1.top

scp file user@host:/path/
来源：http://mng.hongshengwenyu.top

[R57] 远程执行命令
来源：http://usx.zhengqikj.top

ssh user@host 'uptime'
来源：http://yky.shuidangran.top

[R58] 下载文件
来源：http://aqm.xuanzx.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vrq.jinghuilouyu.cn

[R59] 发 POST JSON
来源：http://fia.chenzaomai.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lkx.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://coh.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fut.316326.xyz

[R61] 磁盘占用
来源：http://dub.meibo888.top

df -h;  du -sh *
来源：http://ttr.sysykeji.top

[R62] 找最占空间的文件
来源：http://prg.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://dfk.hesvh.cn

[R63] 内存与进程
来源：http://hyf.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://ogl.jqgufenzy.top

[R64] 结束进程
来源：http://llg.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://idy.yangfankeji.com

[R65] 查看端口占用
来源：http://ntt.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pzs.yongpay.top

[R66] 定时任务
来源：http://mmq.quarkkingdee.top

crontab -e;  crontab -l
来源：http://zeb.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://yhi.bbcook.cn

openssl rand -hex 16
来源：http://gln.tian-w.cn

[R68] 计算文件校验值
来源：http://rns.guannengcc.top

sha256sum a.txt;  md5sum a.txt
来源：http://ccg.hfpthk.cn

[R69] 生成随机密码
来源：http://mkh.cdnleiting.top

head -c 16 /dev/urandom | base64
来源：http://gyk.zhixingplan.top

[R70] 时间戳与互转
来源：http://hyj.yfazqb.com

date +%s;  date -d @1700000000
来源：http://ljg.chenjidiqi.icu

[R71] 日期格式化
来源：http://lde.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jot.pycfn.com

[R72] 等待端口就绪
来源：http://jqb.gaohongyu789.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ssk.jiagoushi.top

[R73] 分割大日志
来源：http://wss.ppjwa.cn

split -l 1000 big.log part_
来源：http://wgr.zhixingplan.top

[R74] 批量重命名
来源：http://xic.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zqb.fehbvm.com

[R75] 导出环境变量
来源：http://nml.snrcjt.cn

export PATH="$HOME/bin:$PATH"
来源：http://hyw.redwolf501.top

[R76] 使用临时文件
来源：http://phz.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mlr.hnqzz.top

[R77] 读取用户输入
来源：http://slm.hysaishi.cn

read -rp "请输入: " ans
来源：http://tjr.ehwqpu.com

[R78] 交互式菜单
来源：http://mam.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vcn.sjlbkw.cn

[R79] 解析命令行选项
来源：http://psd.redwolf501.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bhm.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://zva.smart0.xyz

time ./run.sh
来源：http://uhz.fehbvm.com

================================================================================
来源：http://dtc.shangyingyoupin.top

S. C / C++ 专题
来源：http://fdb.sufxvd.cn

================================================================================
来源：http://mjp.fehbvm.com

[S01] C：Hello World
来源：http://wdj.hammf.cn

#include <stdio.h>
来源：http://zww.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://kfi.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://dzn.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://zay.hysaishi.cn

[S03] C：读入整数
来源：http://kxq.tianlin.xyz

int x; scanf("%d", &x);
来源：http://ceg.nanxuanxn.top

[S04] C：字符串复制
来源：http://bsl.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tbf.haohaochexian.top

[S05] C：字符串长度
来源：http://srg.zhengqikj.top

strlen(s)
来源：http://bcs.tarul.cn

[S06] C：字符串比较
来源：http://zlb.cucudq.cn

strcmp(a, b) == 0
来源：http://vog.ppjwa.cn

[S07] C：数组遍历求和
来源：http://gjs.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dnr.quarkkingdee.top

[S08] C：动态内存分配与释放
来源：http://pmx.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://agr.hcnkem.com

[S09] C：结构体定义与初始化
来源：http://lpb.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://krt.yj20258.top

[S10] C：指针与解引用
来源：http://rpd.xziqi.cn

int *p = &a;  *p = 5;
来源：http://jbe.cqqwz.cn

[S11] C：逐行读文件
来源：http://tae.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://gly.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wcc.ctjpmb.com

fclose(f);
来源：http://wre.haohaochexian.top

[S12] C：写文件
来源：http://lte.pycfn.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mrb.c1oappe.top

[S13] C：宏定义
来源：http://ynk.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cft.c1oappe.top

[S14] C：枚举
来源：http://hjp.shanyushiyangtech.top

enum Color { RED, GREEN, BLUE };
来源：http://urj.hongshengwenyu.top

[S15] C：类型转换
来源：http://rie.jqgfzy.top

(double) a / b
来源：http://wzl.zycfv.cn

[S16] C：位操作置位
来源：http://jxd.vehdjk.com

x |= (1 << 3);
来源：http://eva.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://iyf.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://phv.jinqigfzy.top

[S18] C：命令行参数
来源：http://mpb.yueranfly.top

int main(int argc, char **argv)
来源：http://ayi.hesvh.cn

[S19] C：快速排序
来源：http://syb.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://mxl.ehwqpu.com

[S20] C：二分查找
来源：http://yjj.sweek.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ykw.zhoulong.xyz

[S21] C：字符类别判断
来源：http://jtg.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gra.tianlin.xyz

[S22] C：字符串转数字
来源：http://zco.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qmu.nwbrower.top

[S23] C：随机数
来源：http://pgb.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ssb.zhoulong.xyz

[S24] C：获取本地时间
来源：http://iyo.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vwa.zhaomingkeji.xyz

[S25] C：内存拷贝
来源：http://ytx.fzhhl.top

memcpy(dst, src, n);
来源：http://scc.hcnkem.com

[S26] C：内存清零
来源：http://dre.sweek.top

memset(a, 0, sizeof a);
来源：http://sfm.sufxvd.cn

[S27] C：定义常量
来源：http://zwf.yfazqb.com

const double PI = 3.14159;
来源：http://xyt.zhengqikj.top

[S28] C：静态变量
来源：http://xei.fanxiaobao.xyz

static int counter = 0;
来源：http://fqd.52xcode.cn

[S29] C：变参函数
来源：http://vew.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gbf.c1oappe.top

[S30] C：头文件保护
来源：http://lkv.ppjwa.cn

#ifndef X_H
来源：http://ezj.ydjk.org.cn

#define X_H
来源：http://gho.uphjek.com

#endif
来源：http://cnl.guannengcc.top

[S31] C++：Hello World
来源：http://rhl.hongshengwenyu.top

#include <iostream>
来源：http://slf.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://eji.tianlin.xyz

[S32] C++：字符串
来源：http://ejy.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://zcm.shuidangran.top

[S33] C++：vector 增删
来源：http://jtc.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sxr.xziqi.cn

[S34] C++：遍历 vector
来源：http://mvn.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://sef.redwolf501.top

[S35] C++：map
来源：http://vhk.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vsp.hammf.cn

[S36] C++：unordered_map
来源：http://ozd.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rtk.52xcode.cn

[S37] C++：set
来源：http://xhx.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qho.chenlongwang.top

[S38] C++：排序
来源：http://srp.yanxiufei.cn

std::sort(v.begin(), v.end());
来源：http://awu.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://nev.ctjpmb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://shq.jqgufenzy.top

[S40] C++：查找元素
来源：http://qez.aizwys.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ymf.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://hkm.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zpp.xylfe.cn

[S42] C++：继承与虚函数
来源：http://lyf.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://rac.yfazqb.com

[S43] C++：智能指针
来源：http://coc.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://kui.sxryk.cn

[S44] C++：引用传参
来源：http://bzl.ybcxt.top

void inc(int &x) { ++x; }
来源：http://ykc.quarkkingdee.top

[S45] C++：lambda
来源：http://lbz.yj20258888.top

auto add = [](int a, int b) { return a + b; };
来源：http://xjr.meibo888.top

[S46] C++：函数模板
来源：http://owg.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gqb.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://hls.yueranfly.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rzi.chenzaomai.com

[S48] C++：逐行读文件
来源：http://uag.yongpay.top

std::ifstream in("a.txt");  std::string line;
来源：http://vpw.c1oappe.top

while (std::getline(in, line)) { }
来源：http://qpa.ivvv.top

[S49] C++：写文件
来源：http://afg.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qgc.fzhhl.top

[S50] C++：格式化数字
来源：http://krx.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://won.birdmap.top

[S51] C++：显式类型转换
来源：http://tmg.guowangkeji.top

static_cast<double>(a) / b
来源：http://ixx.cheryme.top

[S52] C++：const 与 noexcept
来源：http://enn.xylfe.cn

int size() const noexcept { return n_; }
来源：http://dit.9152youxi.cn

[S53] C++：移动语义
来源：http://hdl.xziqi.cn

std::vector<int> w = std::move(v);
来源：http://wjm.hnxiangtu.top

[S54] C++：异常处理
来源：http://cyf.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xza.vehdjk.com

[S55] C++：结构化绑定
来源：http://yjk.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vkz.shanyushiyangkeji.top

[S56] C++：optional
来源：http://pvf.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ykx.yuxming.cn

[S57] C++：编译期常量
来源：http://vin.smart0.xyz

constexpr int N = 10;
来源：http://wsr.gaohongyu789.top

[S58] C++：命名空间
来源：http://ncy.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://vte.yj20258888.top

[S59] C++：静态断言
来源：http://kpc.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xue.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://ara.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qki.cucudq.cn

================================================================================
来源：http://vgy.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xql.xinyue.icu

================================================================================
来源：http://ppw.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://dhs.xziqi.cn

println("Hello")
来源：http://wkx.52xcode.cn

[T02] Kotlin：变量
来源：http://wat.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uul.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://ant.sufxvd.cn

"值: $b"
来源：http://hcn.snrcjt.cn

[T04] Kotlin：空安全
来源：http://odm.shanyushiyangtech.top

val n: String? = null;  n?.length
来源：http://pmz.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://hbg.yj20258.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aku.sweek.top

[T06] Kotlin：集合映射
来源：http://bxi.shzxlz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jza.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://jop.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ghq.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://yfp.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://pfz.tanke756.top

[T09] Kotlin：扩展函数
来源：http://dwv.zhiwuduotai.top

fun String.exclaim() = this + "!"
来源：http://lla.tanke756.top

[T10] Kotlin：默认参数
来源：http://ugf.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://iov.fzhhl.top

[T11] Kotlin：协程
来源：http://seq.hammf.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eaj.daria6918.cn

[T12] Kotlin：解构声明
来源：http://uwl.xuetiantiany.cn

val (a, b) = Pair(1, 2)
来源：http://lqa.xingfuxueyuan.xyz

[T13] Kotlin：只读 Map
来源：http://mmn.redwolf501.top

val m = mapOf("a" to 1)
来源：http://zsr.birdmap.top

[T14] Kotlin：循环
来源：http://fcq.guannengcc.top

for (i in 1..10) println(i)
来源：http://ygt.ehwqpu.com

[T15] Kotlin：接口
来源：http://qxo.fehbvm.com

interface Shape { fun area(): Double }
来源：http://ych.nanxuanxn.top

[T16] Swift：Hello World
来源：http://gmk.fehbvm.com

print("Hello")
来源：http://aow.gzhubu.top

[T17] Swift：变量与常量
来源：http://mkk.yj20258.top

var a = 1;  let b = 2
来源：http://aia.cheryme.top

[T18] Swift：字符串插值
来源：http://exe.52xcode.cn

"值: \(b)"
来源：http://nwv.chenjidiqi.icu

[T19] Swift：可选绑定
来源：http://aqh.xinyue.icu

if let n = opt { print(n) }
来源：http://iil.fanxiaobao.xyz

[T20] Swift：数组操作
来源：http://lgv.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hvl.yuanzhike.top

[T21] Swift：遍历
来源：http://xrq.snrcjt.cn

for x in a { print(x) }
来源：http://wsp.dashuyun.cn

[T22] Swift：字典
来源：http://xzq.pengpengdd.cyou

var d = ["a": 1];  d["b"] = 2
来源：http://lcr.xuetiantiany.cn

[T23] Swift：函数
来源：http://qwi.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oqm.zhongyouzk.top

[T24] Swift：闭包
来源：http://noa.yfazqb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://uql.daxiang520.top

[T25] Swift：结构体
来源：http://aeg.gzhubu.top

struct P { var x: Int }
来源：http://ktm.jianghu66.top

[T26] Swift：类与重写
来源：http://udz.0kj1m.cn

class A: Base { override func f() {} }
来源：http://usa.feifeiyinyue.top

[T27] Swift：错误处理
来源：http://wnr.gogol.net.cn

do { try f() } catch { print(error) }
来源：http://nyi.guannengcc.top

[T28] Swift：枚举
来源：http://djq.ydzc1.top

enum Color { case red, green }
来源：http://gao.jinqigufen.top

[T29] Swift：guard 提前返回
来源：http://bak.hongshengwenyu.top

guard let x = opt else { return }
来源：http://ybs.zycfv.cn

[T30] Swift：协议
来源：http://wwz.yonumen.top

protocol Shape { func area() -> Double }
来源：http://nha.vqdsnc.cn

[T31] Lua：Hello World
来源：http://qnw.zhixingplan.top

print("Hello")
来源：http://jet.nwbrower.top

[T32] Lua：局部变量
来源：http://uai.sysykeji.top

local a = 1
来源：http://xan.zhixingplan.top

[T33] Lua：表（数组）
来源：http://xoy.birdmap.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hoq.zhoulong.xyz

[T34] Lua：遍历表
来源：http://kvp.gaohongyu789.top

for i, v in ipairs(t) do print(i, v) end
来源：http://adr.shanyushiyangkeji.top


<!-- 参考信息 -->