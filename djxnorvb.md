代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://njb.hongshengwenyu.top

[R32] 参数个数校验
来源：http://res.jqgfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hwc.fzhhl.top

[R33] 捕获错误并提示行号
来源：http://dgb.havefunace.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qja.xuetiantiany.cn

[R34] 退出时清理
来源：http://aym.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://ebe.yonumen.top

[R35] 后台执行并等待
来源：http://gmp.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jpw.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://kpe.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://han.guannengcc.top

[R37] 把输出赋给变量
来源：http://hda.jlsjyb.cn

files=$(ls -1)
来源：http://yly.shzxlz.cn

[R38] 管道串联
来源：http://hch.cheryme.top

cat a.txt | grep -i error | wc -l
来源：http://axt.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://ati.cashguo.top

cmd > out.log 2>&1
来源：http://vsy.sweek.top

[R40] 追加写日志
来源：http://cpt.xinyue.icu

echo "log" >> out.log
来源：http://vja.52xcode.cn

[R41] 丢弃输出
来源：http://vnd.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://gga.ppjwa.cn

[R42] 输入重定向
来源：http://bqg.daria6918.cn

wc -l < a.txt
来源：http://ipx.snrcjt.cn

[R43] 按名字查找文件
来源：http://qcd.c1oappe.top

find . -name "*.log" -type f
来源：http://jrl.tanke756.top

[R44] 按修改时间查找
来源：http://yvh.haohaochexian.top

find . -mtime -7 -type f
来源：http://lbl.ppjwa.cn

[R45] 批量删除
来源：http://rin.zdbjq.cn

find . -name "*.tmp" -delete
来源：http://nza.hcnkem.com

[R46] 递归替换文件内容
来源：http://say.zhiwuduotai.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dvy.bjfxy.top

[R47] sed 单行替换
来源：http://wgl.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cgv.hysaishi.cn

[R48] awk 取指定列
来源：http://yae.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://gvj.nwbrower.top

[R49] awk 带条件
来源：http://eaj.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kle.shanyushiyangkeji.top

[R50] awk 求和
来源：http://loj.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mji.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://mnz.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://myb.0kj1m.cn

[R52] 统计行数
来源：http://utw.tian-w.cn

wc -l a.txt
来源：http://rwy.tarul.cn

[R53] 查看文件头与实时尾
来源：http://lac.hywenlv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pld.daxiang520.top

[R54] 比较两个文件
来源：http://mer.hammf.cn

diff a.txt b.txt
来源：http://vlc.ydzc1.top

[R55] 压缩与解压
来源：http://zcs.chenjidiqi.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://utg.xziqi.cn

[R56] 远程拷贝
来源：http://tqv.jqgufenzy.top

scp file user@host:/path/
来源：http://dcg.nwbrower.top

[R57] 远程执行命令
来源：http://rrv.zhaomingkeji.xyz

ssh user@host 'uptime'
来源：http://kqe.redwolf501.top

[R58] 下载文件
来源：http://jbs.xinyue.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gnu.xingfuxueyuan.xyz

[R59] 发 POST JSON
来源：http://tgb.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://poc.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://hpl.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sbw.uphjek.com

[R61] 磁盘占用
来源：http://pqb.gzhubu.top

df -h;  du -sh *
来源：http://pxt.dianchejie.cn

[R62] 找最占空间的文件
来源：http://yel.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://sni.haohaochexian.top

[R63] 内存与进程
来源：http://mmo.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://czr.kuanghao11.cn

[R64] 结束进程
来源：http://zin.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://ysn.zhengqikj.top

[R65] 查看端口占用
来源：http://czm.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://waw.ppjwa.cn

[R66] 定时任务
来源：http://cmq.sysykeji.top

crontab -e;  crontab -l
来源：http://rix.daxiang520.top

[R67] 生成随机十六进制串
来源：http://dtz.gzhubu.top

openssl rand -hex 16
来源：http://ghn.316326.xyz

[R68] 计算文件校验值
来源：http://sit.uphjek.com

sha256sum a.txt;  md5sum a.txt
来源：http://igb.shanyushiyangtech.top

[R69] 生成随机密码
来源：http://kot.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://dcw.hysaishi.cn

[R70] 时间戳与互转
来源：http://wzg.wangdashe.top

date +%s;  date -d @1700000000
来源：http://qeh.zhaomingkeji.xyz

[R71] 日期格式化
来源：http://ljb.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://txc.fehbvm.com

[R72] 等待端口就绪
来源：http://trw.sxryk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xld.yangfankeji.com

[R73] 分割大日志
来源：http://dzl.quarkkingdee.top

split -l 1000 big.log part_
来源：http://hiy.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://sbc.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gvz.hongshengwenyu.top

[R75] 导出环境变量
来源：http://ame.gogol.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://ifd.quarkkingdee.top

[R76] 使用临时文件
来源：http://tat.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://czo.ivvv.top

[R77] 读取用户输入
来源：http://psd.vehdjk.com

read -rp "请输入: " ans
来源：http://lwq.hnqzz.top

[R78] 交互式菜单
来源：http://poc.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zii.hnqzz.top

[R79] 解析命令行选项
来源：http://kkl.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hmk.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://kmk.tian-w.cn

time ./run.sh
来源：http://ybi.gogol.net.cn

================================================================================
来源：http://uja.hnqzz.top

S. C / C++ 专题
来源：http://ryk.yongpay.top

================================================================================
来源：http://zsz.0kj1m.cn

[S01] C：Hello World
来源：http://qpn.zdqjudy.top

#include <stdio.h>
来源：http://ysu.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vfn.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://fol.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://lqk.c1oappe.top

[S03] C：读入整数
来源：http://uhg.zhengqikj.top

int x; scanf("%d", &x);
来源：http://ypy.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://zlb.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://tjf.yfazqb.com

[S05] C：字符串长度
来源：http://qda.feifeiyinyue.top

strlen(s)
来源：http://zle.smart0.xyz

[S06] C：字符串比较
来源：http://lgs.vehdjk.com

strcmp(a, b) == 0
来源：http://ela.yangfankeji.com

[S07] C：数组遍历求和
来源：http://efh.0kj1m.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tod.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://wwo.quarkkingdee.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dhg.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://pzs.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hnh.chenzaomai.com

[S10] C：指针与解引用
来源：http://fjd.ppjwa.cn

int *p = &a;  *p = 5;
来源：http://uze.ppjwa.cn

[S11] C：逐行读文件
来源：http://rgj.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://wul.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://eez.redwolf501.top

fclose(f);
来源：http://unb.jinyuanbaomall.cn

[S12] C：写文件
来源：http://tla.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wtp.jqgfzy.top

[S13] C：宏定义
来源：http://hxi.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kvt.epnwcf.com

[S14] C：枚举
来源：http://dvr.jinqigfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://lmp.ehwqpu.com

[S15] C：类型转换
来源：http://kwt.cheryme.top

(double) a / b
来源：http://vkf.zdqjudy.top

[S16] C：位操作置位
来源：http://xbp.cheryme.top

x |= (1 << 3);
来源：http://cup.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://rou.ivvv.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aph.c1oappe.top

[S18] C：命令行参数
来源：http://bxd.hongshengwenyu.top

int main(int argc, char **argv)
来源：http://lic.shanyushiyangtech.top

[S19] C：快速排序
来源：http://wtv.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://slq.tian-w.cn

[S20] C：二分查找
来源：http://cyg.daria6918.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vsi.hammf.cn

[S21] C：字符类别判断
来源：http://lvt.yangfankeji.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xni.yonumen.top

[S22] C：字符串转数字
来源：http://wnl.fehbvm.com

atoi("42");  strtod("3.14", NULL);
来源：http://fir.feifeiyinyue.top

[S23] C：随机数
来源：http://bxs.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ewo.dianchejie.cn

[S24] C：获取本地时间
来源：http://bqh.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://opv.meibo888.top

[S25] C：内存拷贝
来源：http://pvn.yueranfly.top

memcpy(dst, src, n);
来源：http://svm.wangdashe.top

[S26] C：内存清零
来源：http://weu.pengpengdd.cyou

memset(a, 0, sizeof a);
来源：http://dzt.jqgufenzy.top

[S27] C：定义常量
来源：http://qhd.haohaochexian.top

const double PI = 3.14159;
来源：http://ksd.gogol.net.cn

[S28] C：静态变量
来源：http://xqp.sweek.top

static int counter = 0;
来源：http://pwf.kuanghao11.cn

[S29] C：变参函数
来源：http://vsh.cashguo.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sff.hfpthk.cn

[S30] C：头文件保护
来源：http://pih.nanxuanxn.top

#ifndef X_H
来源：http://qri.ehwqpu.com

#define X_H
来源：http://ebq.yangfankeji.com

#endif
来源：http://lkm.yuanzhike.top

[S31] C++：Hello World
来源：http://dgf.zhaomingkeji.xyz

#include <iostream>
来源：http://naz.yangfankeji.com

int main() { std::cout << "Hello\n"; }
来源：http://pzm.dianchejie.cn

[S32] C++：字符串
来源：http://ugo.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://kuu.gaohongyu789.top

[S33] C++：vector 增删
来源：http://ald.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://snf.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://myu.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://cgw.yuxming.cn

[S35] C++：map
来源：http://boo.hesvh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yff.jlsjyb.cn

[S36] C++：unordered_map
来源：http://gzl.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wwb.cashguo.top

[S37] C++：set
来源：http://pmx.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://itz.cucudq.cn

[S38] C++：排序
来源：http://sos.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://ifx.316326.xyz

[S39] C++：自定义比较器排序
来源：http://jos.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uao.epnwcf.com

[S40] C++：查找元素
来源：http://seh.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lxg.chenjidiqi.icu

[S41] C++：类与构造函数
来源：http://qxp.sweek.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iie.xinyue.icu

[S42] C++：继承与虚函数
来源：http://dzt.cqqwz.cn

class B : public Base { public: void f() override {} };
来源：http://fiw.gotoacloud.top

[S43] C++：智能指针
来源：http://isg.mhx1999.top

auto p = std::make_unique<int>(5);
来源：http://ddp.hcnkem.com

[S44] C++：引用传参
来源：http://sdh.bjfxy.top

void inc(int &x) { ++x; }
来源：http://mjq.shuidangran.top

[S45] C++：lambda
来源：http://wqz.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dvg.fktsv.cn

[S46] C++：函数模板
来源：http://pyu.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ibw.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://jvx.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pah.yuxming.cn

[S48] C++：逐行读文件
来源：http://apy.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ffj.yongpay.top

while (std::getline(in, line)) { }
来源：http://uuy.iojbl.cn

[S49] C++：写文件
来源：http://iwn.zhoulong.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bhv.fengsongda.top

[S50] C++：格式化数字
来源：http://lxq.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://efm.fktsv.cn

[S51] C++：显式类型转换
来源：http://bth.guannengcc.top

static_cast<double>(a) / b
来源：http://lko.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://qmx.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://eod.shzxlz.cn

[S53] C++：移动语义
来源：http://zmd.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://jgt.xingfuxueyuan.xyz

[S54] C++：异常处理
来源：http://lxv.jianghu66.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rly.uphjek.com

[S55] C++：结构化绑定
来源：http://jyx.jinqigufen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nlh.snrcjt.cn

[S56] C++：optional
来源：http://lvn.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://txp.zhongyouzk.top

[S57] C++：编译期常量
来源：http://ovc.jinyuanbaomall.cn

constexpr int N = 10;
来源：http://bih.iojbl.cn

[S58] C++：命名空间
来源：http://zug.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://cpf.chenlongwang.top

[S59] C++：静态断言
来源：http://axh.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zuy.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://zoo.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rtw.ctjpmb.com

================================================================================
来源：http://rpf.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iwc.fanxiaobao.xyz

================================================================================
来源：http://fah.epnwcf.com

[T01] Kotlin：Hello World
来源：http://slu.fehbvm.com

println("Hello")
来源：http://cgg.zhaomingkeji.xyz

[T02] Kotlin：变量
来源：http://isj.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://btc.pengpengdd.cyou

[T03] Kotlin：字符串模板
来源：http://wir.yj20258.top

"值: $b"
来源：http://tfb.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://gbm.svipenyu.cn

val n: String? = null;  n?.length
来源：http://quu.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://rbs.chenlongwang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kaw.bjfxy.top

[T06] Kotlin：集合映射
来源：http://rvr.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gxq.hywenlv.cn

[T07] Kotlin：集合过滤
来源：http://xgw.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pwe.zhaomingkeji.xyz

[T08] Kotlin：数据类
来源：http://aqr.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://qql.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://ytz.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://azq.pycfn.com

[T10] Kotlin：默认参数
来源：http://hcw.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ube.shuidangran.top

[T11] Kotlin：协程
来源：http://tfy.dashuyun.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bik.cashguo.top

[T12] Kotlin：解构声明
来源：http://mmo.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://jnc.yuxming.cn

[T13] Kotlin：只读 Map
来源：http://lrv.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://uoh.fehbvm.com

[T14] Kotlin：循环
来源：http://grv.sufxvd.cn

for (i in 1..10) println(i)
来源：http://zht.cashguo.top

[T15] Kotlin：接口
来源：http://yvi.snrcjt.cn

interface Shape { fun area(): Double }
来源：http://pgb.chenjidiqi.icu

[T16] Swift：Hello World
来源：http://jpu.zhaomingkeji.xyz

print("Hello")
来源：http://icu.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://djx.hcnkem.com

var a = 1;  let b = 2
来源：http://ldl.yangfankeji.com

[T18] Swift：字符串插值
来源：http://yan.zycfv.cn

"值: \(b)"
来源：http://dnx.nwbrower.top

[T19] Swift：可选绑定
来源：http://ugl.c1oappe.top

if let n = opt { print(n) }
来源：http://dkn.hnxiangtu.top

[T20] Swift：数组操作
来源：http://mhz.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://xgl.haohaochexian.top

[T21] Swift：遍历
来源：http://uyv.yuxming.cn

for x in a { print(x) }
来源：http://ldb.fehbvm.com

[T22] Swift：字典
来源：http://bwl.hongshengwenyu.top

var d = ["a": 1];  d["b"] = 2
来源：http://rcp.jinqigfzy.top

[T23] Swift：函数
来源：http://hme.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dqa.yfazqb.com

[T24] Swift：闭包
来源：http://hdm.epnwcf.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://edl.chenzaomai.com

[T25] Swift：结构体
来源：http://zcx.daria6918.cn

struct P { var x: Int }
来源：http://wsj.chenzaomai.com

[T26] Swift：类与重写
来源：http://twl.jyoumei.cn

class A: Base { override func f() {} }
来源：http://oqt.cdnleiting.top

[T27] Swift：错误处理
来源：http://vtc.yueranfly.top

do { try f() } catch { print(error) }
来源：http://gtf.cucudq.cn

[T28] Swift：枚举
来源：http://qpb.birdmap.top

enum Color { case red, green }
来源：http://aoo.sweek.top

[T29] Swift：guard 提前返回
来源：http://zqq.zhongyouzk.top

guard let x = opt else { return }
来源：http://raa.hnxiangtu.top

[T30] Swift：协议
来源：http://vcu.haohaochexian.top

protocol Shape { func area() -> Double }
来源：http://bhw.cqqwz.cn

[T31] Lua：Hello World
来源：http://wtv.hongshengwenyu.top

print("Hello")
来源：http://wvz.zhengqikj.top

[T32] Lua：局部变量
来源：http://vew.jlsjyb.cn

local a = 1
来源：http://uif.bjfxy.top

[T33] Lua：表（数组）
来源：http://kkp.fengsongda.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qcf.fzhhl.top

[T34] Lua：遍历表
来源：http://obc.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ack.hnqzz.top


<!-- 参考信息 -->