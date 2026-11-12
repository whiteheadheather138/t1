代发 wailian999

echo $((1 + 2 * 3))
来源：http://tpp.xinyue.icu

[R28] 浮点运算
来源：http://ena.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://vtn.zdbjq.cn

[R29] 定义函数
来源：http://xck.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kxk.gotoacloud.top

[R30] 函数返回状态码
来源：http://uvq.ydjk.org.cn

f() { return 0; }; f || echo "失败了"
来源：http://sfw.shangyingyoupin.top

[R31] 局部变量
来源：http://vcz.cucudq.cn

f() { local x=1; echo "$x"; }
来源：http://ccv.tian-w.cn

[R32] 参数个数校验
来源：http://xdc.hammf.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eln.shanyushiyangkeji.top

[R33] 捕获错误并提示行号
来源：http://cjv.nanxuanxn.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wge.0kj1m.cn

[R34] 退出时清理
来源：http://pwg.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pif.cucudq.cn

[R35] 后台执行并等待
来源：http://qhi.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://oce.sweek.top

[R36] 并发执行多个任务
来源：http://vyx.ppjwa.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gta.zhixingplan.top

[R37] 把输出赋给变量
来源：http://uto.0kj1m.cn

files=$(ls -1)
来源：http://yhx.tarul.cn

[R38] 管道串联
来源：http://esf.aibaodan.cn

cat a.txt | grep -i error | wc -l
来源：http://hyx.meibo888.top

[R39] 重定向标准输出与错误
来源：http://wwe.chenzaomai.com

cmd > out.log 2>&1
来源：http://ujt.feifeiyinyue.top

[R40] 追加写日志
来源：http://eau.meibo888.top

echo "log" >> out.log
来源：http://rph.nwbrower.top

[R41] 丢弃输出
来源：http://vly.bjfxy.top

cmd >/dev/null 2>&1
来源：http://ijd.fanxiaobao.xyz

[R42] 输入重定向
来源：http://yfb.hysaishi.cn

wc -l < a.txt
来源：http://vse.bjfxy.top

[R43] 按名字查找文件
来源：http://wen.aizwys.cn

find . -name "*.log" -type f
来源：http://blo.jyoumei.cn

[R44] 按修改时间查找
来源：http://igj.cdnleiting.top

find . -mtime -7 -type f
来源：http://daa.gogol.net.cn

[R45] 批量删除
来源：http://lkr.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://nzo.zhongyouzk.top

[R46] 递归替换文件内容
来源：http://fae.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wmm.jqgfzy.top

[R47] sed 单行替换
来源：http://ixx.gotoacloud.top

sed -i 's/foo/bar/g' a.txt
来源：http://hph.dianchejie.cn

[R48] awk 取指定列
来源：http://vmv.hcnkem.com

awk '{print $1, $3}' a.txt
来源：http://hdl.aizwys.cn

[R49] awk 带条件
来源：http://jqq.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ciz.aibaodan.cn

[R50] awk 求和
来源：http://fft.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zrc.52xcode.cn

[R51] 排序去重取前几
来源：http://sfp.bbcook.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xmm.yfazqb.com

[R52] 统计行数
来源：http://wlr.svipenyu.cn

wc -l a.txt
来源：http://ryy.xziqi.cn

[R53] 查看文件头与实时尾
来源：http://anh.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vmo.birdmap.top

[R54] 比较两个文件
来源：http://fln.jianghu66.top

diff a.txt b.txt
来源：http://hac.bbcook.cn

[R55] 压缩与解压
来源：http://afs.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nae.cashguo.top

[R56] 远程拷贝
来源：http://uxz.tian-w.cn

scp file user@host:/path/
来源：http://eim.fengsongda.top

[R57] 远程执行命令
来源：http://thj.yonumen.top

ssh user@host 'uptime'
来源：http://rxg.zhoulong.xyz

[R58] 下载文件
来源：http://fye.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ppz.havefunace.top

[R59] 发 POST JSON
来源：http://yhl.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://icd.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://bnd.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aiq.yuanzhike.top

[R61] 磁盘占用
来源：http://uug.cashguo.top

df -h;  du -sh *
来源：http://xvf.316326.xyz

[R62] 找最占空间的文件
来源：http://fnb.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://ukh.xingfuxueyuan.xyz

[R63] 内存与进程
来源：http://yoc.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://pnu.jyoumei.cn

[R64] 结束进程
来源：http://wyx.yongpay.top

kill -9 $(pgrep -f app.py)
来源：http://ygu.jinqigfzy.top

[R65] 查看端口占用
来源：http://tix.cucudq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qwl.ydjk.org.cn

[R66] 定时任务
来源：http://bvi.gaohongyu789.top

crontab -e;  crontab -l
来源：http://vwm.ybcxt.top

[R67] 生成随机十六进制串
来源：http://rue.zhaomingkeji.xyz

openssl rand -hex 16
来源：http://rmi.zhixingplan.top

[R68] 计算文件校验值
来源：http://pbf.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://cvh.jlsjyb.cn

[R69] 生成随机密码
来源：http://mnl.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://xky.uphjek.com

[R70] 时间戳与互转
来源：http://gtn.sxryk.cn

date +%s;  date -d @1700000000
来源：http://uau.yuanzhike.top

[R71] 日期格式化
来源：http://hok.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ska.guannengcc.top

[R72] 等待端口就绪
来源：http://fbk.vqdsnc.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dik.hongshengwenyu.top

[R73] 分割大日志
来源：http://wvb.uphjek.com

split -l 1000 big.log part_
来源：http://gzy.jinqigufen.top

[R74] 批量重命名
来源：http://yvn.jqgufenzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://byz.yangfankeji.com

[R75] 导出环境变量
来源：http://foz.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://dpk.kuanghao11.cn

[R76] 使用临时文件
来源：http://uxf.guowangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uet.ehwqpu.com

[R77] 读取用户输入
来源：http://kfw.guannengcc.top

read -rp "请输入: " ans
来源：http://qrn.vehdjk.com

[R78] 交互式菜单
来源：http://yvb.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dkr.c1oappe.top

[R79] 解析命令行选项
来源：http://fxd.cdnleiting.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bmp.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://tat.epnwcf.com

time ./run.sh
来源：http://xqu.zhongyouzk.top

================================================================================
来源：http://mqj.cheryme.top

S. C / C++ 专题
来源：http://tpg.guowangkeji.top

================================================================================
来源：http://xtm.sxryk.cn

[S01] C：Hello World
来源：http://cai.fanxiaobao.xyz

#include <stdio.h>
来源：http://aew.cheryme.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kqh.yueranfly.top

[S02] C：变量与格式化输出
来源：http://mox.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://ltt.yfazqb.com

[S03] C：读入整数
来源：http://tzz.jqgfzy.top

int x; scanf("%d", &x);
来源：http://ruf.guannengcc.top

[S04] C：字符串复制
来源：http://qjv.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hsj.yangfankeji.com

[S05] C：字符串长度
来源：http://xsj.yanxiufei.cn

strlen(s)
来源：http://dwv.jlsjyb.cn

[S06] C：字符串比较
来源：http://qai.hywenlv.cn

strcmp(a, b) == 0
来源：http://rzu.cqqwz.cn

[S07] C：数组遍历求和
来源：http://kfu.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tat.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://rju.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wqy.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://jin.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eug.zhoulong.xyz

[S10] C：指针与解引用
来源：http://ynz.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://nzw.tian-w.cn

[S11] C：逐行读文件
来源：http://izl.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://dpq.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xtt.fktsv.cn

fclose(f);
来源：http://lxr.tianlin.xyz

[S12] C：写文件
来源：http://xbc.birdmap.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ewa.316326.xyz

[S13] C：宏定义
来源：http://otz.chenzaomai.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hhj.zhiwuduotai.top

[S14] C：枚举
来源：http://nkv.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://qwl.bjfxy.top

[S15] C：类型转换
来源：http://nrg.zdbjq.cn

(double) a / b
来源：http://tqk.birdmap.top

[S16] C：位操作置位
来源：http://sip.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://hmv.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://xvi.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tij.yj20258.top

[S18] C：命令行参数
来源：http://vyh.fehbvm.com

int main(int argc, char **argv)
来源：http://vtm.yonumen.top

[S19] C：快速排序
来源：http://tis.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rnb.yangfankeji.com

[S20] C：二分查找
来源：http://dqe.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gfh.epnwcf.com

[S21] C：字符类别判断
来源：http://wtu.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lzc.chenlongwang.top

[S22] C：字符串转数字
来源：http://drp.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://hlj.zhiwuduotai.top

[S23] C：随机数
来源：http://ndd.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kwc.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://oqp.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://onj.0kj1m.cn

[S25] C：内存拷贝
来源：http://mnc.dianchejie.cn

memcpy(dst, src, n);
来源：http://djg.havefunace.top

[S26] C：内存清零
来源：http://svm.hnqzz.top

memset(a, 0, sizeof a);
来源：http://div.zhixingplan.top

[S27] C：定义常量
来源：http://ibl.zhaomingkeji.xyz

const double PI = 3.14159;
来源：http://utu.xuanzx.com

[S28] C：静态变量
来源：http://mxc.zhengqikj.top

static int counter = 0;
来源：http://seg.tanke756.top

[S29] C：变参函数
来源：http://fmq.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yqf.fzhhl.top

[S30] C：头文件保护
来源：http://edk.ywan-chungtsiang.top

#ifndef X_H
来源：http://aqq.sxryk.cn

#define X_H
来源：http://nuq.jqgufenzy.top

#endif
来源：http://izf.ppjwa.cn

[S31] C++：Hello World
来源：http://tgw.mhx1999.top

#include <iostream>
来源：http://eyw.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://ksy.birdmap.top

[S32] C++：字符串
来源：http://qqp.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://zhj.0kj1m.cn

[S33] C++：vector 增删
来源：http://ghj.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pyu.hcnkem.com

[S34] C++：遍历 vector
来源：http://zju.xinyue.icu

for (auto &x : v) { std::cout << x; }
来源：http://vsb.yongpay.top

[S35] C++：map
来源：http://dds.iojbl.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cfw.nwbrower.top

[S36] C++：unordered_map
来源：http://krd.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mxy.tarul.cn

[S37] C++：set
来源：http://mfj.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eyj.guowangkeji.top

[S38] C++：排序
来源：http://oey.yonumen.top

std::sort(v.begin(), v.end());
来源：http://fnq.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://sgw.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eju.vqdsnc.cn

[S40] C++：查找元素
来源：http://blc.daria6918.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://njw.cheryme.top

[S41] C++：类与构造函数
来源：http://geb.yj20258888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mcn.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://hmi.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://fpd.0kj1m.cn

[S43] C++：智能指针
来源：http://rmp.xuetiantiany.cn

auto p = std::make_unique<int>(5);
来源：http://tzh.vqdsnc.cn

[S44] C++：引用传参
来源：http://mhp.shuidangran.top

void inc(int &x) { ++x; }
来源：http://jgn.nwbrower.top

[S45] C++：lambda
来源：http://sub.zhengqikj.top

auto add = [](int a, int b) { return a + b; };
来源：http://jii.ehwqpu.com

[S46] C++：函数模板
来源：http://foy.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rqj.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://apx.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kli.shzxlz.cn

[S48] C++：逐行读文件
来源：http://yku.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://saj.hongshengwenyu.top

while (std::getline(in, line)) { }
来源：http://omq.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://zxd.sjlbkw.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hda.jqgufenzy.top

[S50] C++：格式化数字
来源：http://iko.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jas.bbcook.cn

[S51] C++：显式类型转换
来源：http://ird.hcnkem.com

static_cast<double>(a) / b
来源：http://mvc.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://vsf.hesvh.cn

int size() const noexcept { return n_; }
来源：http://ytc.chenzaomai.com

[S53] C++：移动语义
来源：http://tlr.yuxming.cn

std::vector<int> w = std::move(v);
来源：http://mrg.9152youxi.cn

[S54] C++：异常处理
来源：http://fun.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://awk.hcnkem.com

[S55] C++：结构化绑定
来源：http://fse.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://jfy.gotoacloud.top

[S56] C++：optional
来源：http://ihe.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qmx.hesvh.cn

[S57] C++：编译期常量
来源：http://lii.cqqwz.cn

constexpr int N = 10;
来源：http://moh.zhiwuduotai.top

[S58] C++：命名空间
来源：http://leu.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://ndk.ppjwa.cn

[S59] C++：静态断言
来源：http://qgs.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://agy.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://gkr.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://chq.316326.xyz

================================================================================
来源：http://lko.hnxiangtu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iac.yuxming.cn

================================================================================
来源：http://cbk.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://aco.hcnkem.com

println("Hello")
来源：http://tjw.shuidangran.top

[T02] Kotlin：变量
来源：http://arr.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ksg.hnxiangtu.top

[T03] Kotlin：字符串模板
来源：http://let.shangyingyoupin.top

"值: $b"
来源：http://fgg.aibaodan.cn

[T04] Kotlin：空安全
来源：http://lkj.zhixingplan.top

val n: String? = null;  n?.length
来源：http://bgn.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://ffs.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vbp.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://djp.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://smd.gzhubu.top

[T07] Kotlin：集合过滤
来源：http://wfl.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://she.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://zkj.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://hbs.birdmap.top

[T09] Kotlin：扩展函数
来源：http://wlp.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://slf.havefunace.top

[T10] Kotlin：默认参数
来源：http://eol.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jco.fzhhl.top

[T11] Kotlin：协程
来源：http://ejs.jinghuilouyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lmx.smart0.xyz

[T12] Kotlin：解构声明
来源：http://rrw.nanxinkj.top

val (a, b) = Pair(1, 2)
来源：http://bev.xuanzx.com

[T13] Kotlin：只读 Map
来源：http://rue.zhoulong.xyz

val m = mapOf("a" to 1)
来源：http://pwx.gogol.net.cn

[T14] Kotlin：循环
来源：http://jym.dianchejie.cn

for (i in 1..10) println(i)
来源：http://ehb.svipenyu.cn

[T15] Kotlin：接口
来源：http://ete.tanke756.top

interface Shape { fun area(): Double }
来源：http://mof.ybcxt.top

[T16] Swift：Hello World
来源：http://ygo.zdqjudy.top

print("Hello")
来源：http://lau.yueranfly.top

[T17] Swift：变量与常量
来源：http://zld.yueranfly.top

var a = 1;  let b = 2
来源：http://bds.havefunace.top

[T18] Swift：字符串插值
来源：http://jeu.snrcjt.cn

"值: \(b)"
来源：http://xlr.quarkkingdee.top

[T19] Swift：可选绑定
来源：http://czf.nwbrower.top

if let n = opt { print(n) }
来源：http://jqs.andypj.xyz

[T20] Swift：数组操作
来源：http://juw.cqqwz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://car.fanxiaobao.xyz

[T21] Swift：遍历
来源：http://hwp.quarkkingdee.top

for x in a { print(x) }
来源：http://qfh.xziqi.cn

[T22] Swift：字典
来源：http://wen.zhijiandao.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pby.chenlongwang.top

[T23] Swift：函数
来源：http://sxj.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oev.fktsv.cn

[T24] Swift：闭包
来源：http://amc.sufxvd.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://njf.zhiwuduotai.top

[T25] Swift：结构体
来源：http://swd.andypj.xyz

struct P { var x: Int }
来源：http://ion.hongshengwenyu.top

[T26] Swift：类与重写
来源：http://pax.yonumen.top

class A: Base { override func f() {} }
来源：http://iqj.xuanzx.com

[T27] Swift：错误处理
来源：http://pah.yj202588.top

do { try f() } catch { print(error) }
来源：http://owa.ybcxt.top

[T28] Swift：枚举
来源：http://zun.fzhhl.top

enum Color { case red, green }
来源：http://vog.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://wxy.0kj1m.cn

guard let x = opt else { return }
来源：http://rcu.jyoumei.cn

[T30] Swift：协议
来源：http://kof.cdnleiting.top

protocol Shape { func area() -> Double }
来源：http://rxh.hesvh.cn


<!-- 参考信息 -->