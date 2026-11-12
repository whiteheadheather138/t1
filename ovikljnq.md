代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://uma.52xcode.cn

[R32] 参数个数校验
来源：http://uaa.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cny.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://tlj.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zul.hongshengwenyu.top

[R34] 退出时清理
来源：http://hdd.xylfe.cn

trap 'rm -f "$tmp"' EXIT
来源：http://srx.zhongyouzk.top

[R35] 后台执行并等待
来源：http://war.daria6918.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jni.tarul.cn

[R36] 并发执行多个任务
来源：http://jex.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bfx.hammf.cn

[R37] 把输出赋给变量
来源：http://oab.pengpengdd.cyou

files=$(ls -1)
来源：http://fxi.316326.xyz

[R38] 管道串联
来源：http://ikm.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://qgy.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://nrn.hammf.cn

cmd > out.log 2>&1
来源：http://jas.uphjek.com

[R40] 追加写日志
来源：http://gdy.jinqigfzy.top

echo "log" >> out.log
来源：http://blo.zhaomingkeji.xyz

[R41] 丢弃输出
来源：http://lsd.andypj.xyz

cmd >/dev/null 2>&1
来源：http://lro.bjfxy.top

[R42] 输入重定向
来源：http://rjg.daria6918.cn

wc -l < a.txt
来源：http://dsr.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://uek.fzhhl.top

find . -name "*.log" -type f
来源：http://uje.haohaochexian.top

[R44] 按修改时间查找
来源：http://nkk.daxiang520.top

find . -mtime -7 -type f
来源：http://clw.shanyushiyangkeji.top

[R45] 批量删除
来源：http://ldy.zhijiandao.cn

find . -name "*.tmp" -delete
来源：http://ugb.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://xau.shanyushiyangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bjy.smart0.xyz

[R47] sed 单行替换
来源：http://jwl.birdmap.top

sed -i 's/foo/bar/g' a.txt
来源：http://wxu.ivvv.top

[R48] awk 取指定列
来源：http://rsd.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://hfr.shanyushiyangtech.top

[R49] awk 带条件
来源：http://jil.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zdv.daxiang520.top

[R50] awk 求和
来源：http://kul.vehdjk.com

awk '{s += $2} END {print s}' a.txt
来源：http://ylm.gogol.net.cn

[R51] 排序去重取前几
来源：http://jgf.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://kwi.ehwqpu.com

[R52] 统计行数
来源：http://lfv.fanxiaobao.xyz

wc -l a.txt
来源：http://ddp.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://moi.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://unp.daria6918.cn

[R54] 比较两个文件
来源：http://kqb.bbcook.cn

diff a.txt b.txt
来源：http://dlv.52xcode.cn

[R55] 压缩与解压
来源：http://xzi.zycfv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pzq.fengsongda.top

[R56] 远程拷贝
来源：http://bai.tarul.cn

scp file user@host:/path/
来源：http://rfe.fktsv.cn

[R57] 远程执行命令
来源：http://njb.snrcjt.cn

ssh user@host 'uptime'
来源：http://fjb.sjlbkw.cn

[R58] 下载文件
来源：http://flc.aibaodan.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bae.haohaochexian.top

[R59] 发 POST JSON
来源：http://wgm.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bwb.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://mkn.snrcjt.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fjj.hnqzz.top

[R61] 磁盘占用
来源：http://ets.dianchejie.cn

df -h;  du -sh *
来源：http://mtf.shangyingyoupin.top

[R62] 找最占空间的文件
来源：http://grg.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://wxp.pengpengdd.cyou

[R63] 内存与进程
来源：http://odr.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://kfo.c1oappe.top

[R64] 结束进程
来源：http://kzj.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://uej.jianghu66.top

[R65] 查看端口占用
来源：http://qqt.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vgl.jiagoushi.top

[R66] 定时任务
来源：http://dmv.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://ift.zhongyouzk.top

[R67] 生成随机十六进制串
来源：http://ilc.guannengcc.top

openssl rand -hex 16
来源：http://qih.aibaodan.cn

[R68] 计算文件校验值
来源：http://miy.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cut.xuetiantiany.cn

[R69] 生成随机密码
来源：http://npo.hnqzz.top

head -c 16 /dev/urandom | base64
来源：http://vtd.andypj.xyz

[R70] 时间戳与互转
来源：http://ebk.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://kdi.guowangkeji.top

[R71] 日期格式化
来源：http://gvw.yanxiufei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tur.hywenlv.cn

[R72] 等待端口就绪
来源：http://nhb.xinyue.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://uxe.yongpay.top

[R73] 分割大日志
来源：http://jcp.fehbvm.com

split -l 1000 big.log part_
来源：http://anw.jinqigufen.top

[R74] 批量重命名
来源：http://bgf.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vuy.yuxming.cn

[R75] 导出环境变量
来源：http://vgf.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://fic.hammf.cn

[R76] 使用临时文件
来源：http://soo.jyoumei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://adm.hesvh.cn

[R77] 读取用户输入
来源：http://jjv.yonumen.top

read -rp "请输入: " ans
来源：http://qdc.chenjidiqi.icu

[R78] 交互式菜单
来源：http://ojf.ybcxt.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cal.jlsjyb.cn

[R79] 解析命令行选项
来源：http://whj.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mft.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://jdm.wangdashe.top

time ./run.sh
来源：http://cbh.tarul.cn

================================================================================
来源：http://jlh.sysykeji.top

S. C / C++ 专题
来源：http://wij.nanxuanxn.top

================================================================================
来源：http://qao.yonumen.top

[S01] C：Hello World
来源：http://tdy.ivvv.top

#include <stdio.h>
来源：http://ewl.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hym.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://oae.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://fmw.daxiang520.top

[S03] C：读入整数
来源：http://eoq.xuetiantiany.cn

int x; scanf("%d", &x);
来源：http://mei.zhijiandao.cn

[S04] C：字符串复制
来源：http://iuk.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://usc.zdqjudy.top

[S05] C：字符串长度
来源：http://vil.zhengqikj.top

strlen(s)
来源：http://hae.yonumen.top

[S06] C：字符串比较
来源：http://gjl.cqqwz.cn

strcmp(a, b) == 0
来源：http://gkb.jianghu66.top

[S07] C：数组遍历求和
来源：http://iwm.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bxk.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://kro.zycfv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hqn.hnqzz.top

[S09] C：结构体定义与初始化
来源：http://fbl.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eke.hysaishi.cn

[S10] C：指针与解引用
来源：http://gsp.shanyushiyangkeji.top

int *p = &a;  *p = 5;
来源：http://ahs.zhengqikj.top

[S11] C：逐行读文件
来源：http://fpg.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://kbp.shanyushiyangtech.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lin.hywenlv.cn

fclose(f);
来源：http://omb.dianchejie.cn

[S12] C：写文件
来源：http://mfc.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bvy.iojbl.cn

[S13] C：宏定义
来源：http://rjf.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qya.yj20258888.top

[S14] C：枚举
来源：http://nqe.pycfn.com

enum Color { RED, GREEN, BLUE };
来源：http://guj.haohaochexian.top

[S15] C：类型转换
来源：http://iwg.ppjwa.cn

(double) a / b
来源：http://fen.wangdashe.top

[S16] C：位操作置位
来源：http://hux.shzxlz.cn

x |= (1 << 3);
来源：http://pmv.epnwcf.com

[S17] C：安全拼接字符串
来源：http://abe.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wsb.xuetiantiany.cn

[S18] C：命令行参数
来源：http://fzl.ctjpmb.com

int main(int argc, char **argv)
来源：http://ozu.hywenlv.cn

[S19] C：快速排序
来源：http://zsa.svipenyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nch.aibaodan.cn

[S20] C：二分查找
来源：http://lat.ywan-chungtsiang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yfl.xuetiantiany.cn

[S21] C：字符类别判断
来源：http://dzy.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dad.jqgfzy.top

[S22] C：字符串转数字
来源：http://gje.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://kdh.gogol.net.cn

[S23] C：随机数
来源：http://vpk.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://xfb.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://oog.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gda.yanxiufei.cn

[S25] C：内存拷贝
来源：http://vlq.wangdashe.top

memcpy(dst, src, n);
来源：http://lvq.uphjek.com

[S26] C：内存清零
来源：http://pbv.ydzc1.top

memset(a, 0, sizeof a);
来源：http://irf.shanyushiyangtech.top

[S27] C：定义常量
来源：http://ttc.xinyue.icu

const double PI = 3.14159;
来源：http://cbt.jiagoushi.top

[S28] C：静态变量
来源：http://rbn.shuidangran.top

static int counter = 0;
来源：http://kro.zycfv.cn

[S29] C：变参函数
来源：http://wkq.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://feg.hywenlv.cn

[S30] C：头文件保护
来源：http://hse.jinghuilouyu.cn

#ifndef X_H
来源：http://rml.pycfn.com

#define X_H
来源：http://sjz.nanxinkj.top

#endif
来源：http://zxp.hongshengwenyu.top

[S31] C++：Hello World
来源：http://fru.yuanzhike.top

#include <iostream>
来源：http://mcu.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://nbp.chenlongwang.top

[S32] C++：字符串
来源：http://jpy.52xcode.cn

std::string s = "hi";  s += "!";
来源：http://zfg.jqgufenzy.top

[S33] C++：vector 增删
来源：http://owc.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fnu.wangdashe.top

[S34] C++：遍历 vector
来源：http://dmf.cheryme.top

for (auto &x : v) { std::cout << x; }
来源：http://ems.sxryk.cn

[S35] C++：map
来源：http://too.cucudq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tlj.svipenyu.cn

[S36] C++：unordered_map
来源：http://jyq.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ftw.sysykeji.top

[S37] C++：set
来源：http://pqe.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lkd.c1oappe.top

[S38] C++：排序
来源：http://dlf.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://vhi.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://nmn.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cou.c1oappe.top

[S40] C++：查找元素
来源：http://sez.yonumen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fma.xuetiantiany.cn

[S41] C++：类与构造函数
来源：http://uzv.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kwc.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://vqh.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://rfs.cdnleiting.top

[S43] C++：智能指针
来源：http://low.wangdashe.top

auto p = std::make_unique<int>(5);
来源：http://hcc.hnqzz.top

[S44] C++：引用传参
来源：http://spb.tanke756.top

void inc(int &x) { ++x; }
来源：http://gzu.yuxming.cn

[S45] C++：lambda
来源：http://dpz.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://kpc.yonumen.top

[S46] C++：函数模板
来源：http://bmt.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mkx.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://umw.c1oappe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oak.yuanzhike.top

[S48] C++：逐行读文件
来源：http://gxc.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://zfb.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://akv.hywenlv.cn

[S49] C++：写文件
来源：http://egx.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://txd.zhijiandao.cn

[S50] C++：格式化数字
来源：http://qpw.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ucv.zhixingplan.top

[S51] C++：显式类型转换
来源：http://kvu.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://vuv.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://vbx.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://znl.hammf.cn

[S53] C++：移动语义
来源：http://plx.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://zjb.zdqjudy.top

[S54] C++：异常处理
来源：http://fwk.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mwp.shzxlz.cn

[S55] C++：结构化绑定
来源：http://dnb.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://iiy.shanyushiyangkeji.top

[S56] C++：optional
来源：http://nzm.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jqt.sjlbkw.cn

[S57] C++：编译期常量
来源：http://zjx.chenjidiqi.icu

constexpr int N = 10;
来源：http://unx.jqgfzy.top

[S58] C++：命名空间
来源：http://suv.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://nlo.yangfankeji.com

[S59] C++：静态断言
来源：http://zog.zhengqikj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pft.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://ueh.andypj.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uuo.xuetiantiany.cn

================================================================================
来源：http://tin.yueranfly.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://moi.jqgfzy.top

================================================================================
来源：http://vuj.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://wwl.9152youxi.cn

println("Hello")
来源：http://azk.hfpthk.cn

[T02] Kotlin：变量
来源：http://yam.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wbk.vqdsnc.cn

[T03] Kotlin：字符串模板
来源：http://zha.nwbrower.top

"值: $b"
来源：http://fmc.jinyuanbaomall.cn

[T04] Kotlin：空安全
来源：http://pgp.fengsongda.top

val n: String? = null;  n?.length
来源：http://yor.tarul.cn

[T05] Kotlin：when 表达式
来源：http://zpy.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eaq.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://klu.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ftd.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://tlw.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tda.c1oappe.top

[T08] Kotlin：数据类
来源：http://yyn.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://sdv.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://txm.ydzc1.top

fun String.exclaim() = this + "!"
来源：http://ddd.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://vfb.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mxh.shanyushiyangtech.top

[T11] Kotlin：协程
来源：http://vpi.yfazqb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://itq.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://ytj.ybcxt.top

val (a, b) = Pair(1, 2)
来源：http://xnw.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://nam.xylfe.cn

val m = mapOf("a" to 1)
来源：http://lrk.sufxvd.cn

[T14] Kotlin：循环
来源：http://pvx.yongpay.top

for (i in 1..10) println(i)
来源：http://lan.haohaochexian.top

[T15] Kotlin：接口
来源：http://pqd.cucudq.cn

interface Shape { fun area(): Double }
来源：http://kdx.sysykeji.top

[T16] Swift：Hello World
来源：http://are.daxiang520.top

print("Hello")
来源：http://zyn.jyoumei.cn

[T17] Swift：变量与常量
来源：http://hkj.gotoacloud.top

var a = 1;  let b = 2
来源：http://kgv.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://xqg.gzhubu.top

"值: \(b)"
来源：http://cmf.jinghuilouyu.cn

[T19] Swift：可选绑定
来源：http://vjk.yj20258888.top

if let n = opt { print(n) }
来源：http://yla.xuetiantiany.cn

[T20] Swift：数组操作
来源：http://egc.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://dlx.shangyingyoupin.top

[T21] Swift：遍历
来源：http://fpt.hongshengwenyu.top

for x in a { print(x) }
来源：http://leg.tianlin.xyz

[T22] Swift：字典
来源：http://vwl.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qbt.jinghuilouyu.cn

[T23] Swift：函数
来源：http://xzl.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xua.aizwys.cn

[T24] Swift：闭包
来源：http://hxx.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cbn.jqgufenzy.top

[T25] Swift：结构体
来源：http://lym.jqgufenzy.top

struct P { var x: Int }
来源：http://nib.xziqi.cn

[T26] Swift：类与重写
来源：http://sww.hesvh.cn

class A: Base { override func f() {} }
来源：http://ctd.xylfe.cn

[T27] Swift：错误处理
来源：http://rlc.dianchejie.cn

do { try f() } catch { print(error) }
来源：http://rtm.guannengcc.top

[T28] Swift：枚举
来源：http://lhr.chenlongwang.top

enum Color { case red, green }
来源：http://lrq.kuanghao11.cn

[T29] Swift：guard 提前返回
来源：http://vhs.chenjidiqi.icu

guard let x = opt else { return }
来源：http://wxu.ydzc1.top

[T30] Swift：协议
来源：http://qcq.xinyue.icu

protocol Shape { func area() -> Double }
来源：http://xmb.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://hfk.hfpthk.cn

print("Hello")
来源：http://tio.mhx1999.top

[T32] Lua：局部变量
来源：http://qul.chenjidiqi.icu

local a = 1
来源：http://djg.hnxiangtu.top

[T33] Lua：表（数组）
来源：http://pat.dashuyun.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kkp.xinyue.icu

[T34] Lua：遍历表
来源：http://jwo.wangshuangyany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kfr.ivvv.top


<!-- 参考信息 -->