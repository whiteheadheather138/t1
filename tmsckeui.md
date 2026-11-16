代发 wailian999

echo "${#arr[@]}"
来源：http://iyv.cqqwz.cn

[R20] 关联数组（字典）
来源：http://lix.52xcode.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hej.cheryme.top

[R21] 字符串长度
来源：http://rex.birdmap.top

echo "${#s}"
来源：http://iix.hesvh.cn

[R22] 截取子串
来源：http://qwl.yj20258888.top

echo "${s:0:5}"
来源：http://rxa.yonumen.top

[R23] 字符串替换
来源：http://mvl.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rxg.nanxuanxn.top

[R24] 大小写转换
来源：http://ema.birdmap.top

echo "${s^^}"; echo "${s,,}"
来源：http://nju.xuanzx.com

[R25] 去后缀 / 去前缀
来源：http://yem.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nhb.xylfe.cn

[R26] 命令替换
来源：http://yxd.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://swo.kuanghao11.cn

[R27] 算术展开
来源：http://osv.hongshengwenyu.top

echo $((1 + 2 * 3))
来源：http://gmv.316326.xyz

[R28] 浮点运算
来源：http://xtd.yuxming.cn

echo "scale=2; 10/3" | bc
来源：http://ewk.hysaishi.cn

[R29] 定义函数
来源：http://qov.xziqi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tlj.bjfxy.top

[R30] 函数返回状态码
来源：http://gro.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://spb.quarkkingdee.top

[R31] 局部变量
来源：http://wsy.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://bnk.316326.xyz

[R32] 参数个数校验
来源：http://jwk.jinyuanbaomall.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lko.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://ljh.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ebk.guannengcc.top

[R34] 退出时清理
来源：http://bmd.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ktk.redwolf501.top

[R35] 后台执行并等待
来源：http://rql.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://izh.316326.xyz

[R36] 并发执行多个任务
来源：http://soo.smart0.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nsx.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://ash.havefunace.top

files=$(ls -1)
来源：http://sbk.316326.xyz

[R38] 管道串联
来源：http://qbe.shanyushiyangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://vrg.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://fks.zhengqikj.top

cmd > out.log 2>&1
来源：http://gcx.xziqi.cn

[R40] 追加写日志
来源：http://eoo.52xcode.cn

echo "log" >> out.log
来源：http://wes.hammf.cn

[R41] 丢弃输出
来源：http://qjo.fzhhl.top

cmd >/dev/null 2>&1
来源：http://hlq.ppjwa.cn

[R42] 输入重定向
来源：http://jbm.hnxiangtu.top

wc -l < a.txt
来源：http://cor.yangfankeji.com

[R43] 按名字查找文件
来源：http://jkv.xziqi.cn

find . -name "*.log" -type f
来源：http://egn.kuanghao11.cn

[R44] 按修改时间查找
来源：http://djv.kuanghao11.cn

find . -mtime -7 -type f
来源：http://mwx.fanxiaobao.xyz

[R45] 批量删除
来源：http://ayt.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://opc.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://dlu.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uvh.bbcook.cn

[R47] sed 单行替换
来源：http://kmb.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://ifu.zhoulong.xyz

[R48] awk 取指定列
来源：http://xvw.vehdjk.com

awk '{print $1, $3}' a.txt
来源：http://goc.ppjwa.cn

[R49] awk 带条件
来源：http://qxr.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://spi.iojbl.cn

[R50] awk 求和
来源：http://vbg.yonumen.top

awk '{s += $2} END {print s}' a.txt
来源：http://ehn.iojbl.cn

[R51] 排序去重取前几
来源：http://lml.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://huu.uphjek.com

[R52] 统计行数
来源：http://ofi.aibaodan.cn

wc -l a.txt
来源：http://gcf.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://jix.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vvt.fehbvm.com

[R54] 比较两个文件
来源：http://wyj.pengpengdd.cyou

diff a.txt b.txt
来源：http://xdd.ppjwa.cn

[R55] 压缩与解压
来源：http://abg.zhongyouzk.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zia.zdbjq.cn

[R56] 远程拷贝
来源：http://obj.xylfe.cn

scp file user@host:/path/
来源：http://pwj.feifeiyinyue.top

[R57] 远程执行命令
来源：http://bwf.vqdsnc.cn

ssh user@host 'uptime'
来源：http://gea.nanxinkj.top

[R58] 下载文件
来源：http://jip.vehdjk.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nji.guowangkeji.top

[R59] 发 POST JSON
来源：http://ytk.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://avn.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://obm.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://syt.zhijiandao.cn

[R61] 磁盘占用
来源：http://yig.yongpay.top

df -h;  du -sh *
来源：http://wci.hesvh.cn

[R62] 找最占空间的文件
来源：http://wrq.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://kih.yj20258.top

[R63] 内存与进程
来源：http://nqg.fzhhl.top

free -h;  ps aux | grep nginx
来源：http://pka.meibo888.top

[R64] 结束进程
来源：http://ysg.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://dfc.yueranfly.top

[R65] 查看端口占用
来源：http://jgb.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bae.yj20258.top

[R66] 定时任务
来源：http://ynt.ybcxt.top

crontab -e;  crontab -l
来源：http://wnh.fktsv.cn

[R67] 生成随机十六进制串
来源：http://rki.yuanzhike.top

openssl rand -hex 16
来源：http://fth.52xcode.cn

[R68] 计算文件校验值
来源：http://gom.ybcxt.top

sha256sum a.txt;  md5sum a.txt
来源：http://pie.ybcxt.top

[R69] 生成随机密码
来源：http://yfc.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://sgv.zhijiandao.cn

[R70] 时间戳与互转
来源：http://jnp.guannengcc.top

date +%s;  date -d @1700000000
来源：http://gcl.hammf.cn

[R71] 日期格式化
来源：http://qgc.tarul.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://knq.uphjek.com

[R72] 等待端口就绪
来源：http://uqw.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jvt.ehwqpu.com

[R73] 分割大日志
来源：http://les.jlsjyb.cn

split -l 1000 big.log part_
来源：http://lhd.havefunace.top

[R74] 批量重命名
来源：http://ywp.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gyd.9152youxi.cn

[R75] 导出环境变量
来源：http://dxu.svipenyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://onv.nanxuanxn.top

[R76] 使用临时文件
来源：http://txq.jlsjyb.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wvx.gaohongyu789.top

[R77] 读取用户输入
来源：http://pje.hywenlv.cn

read -rp "请输入: " ans
来源：http://wkq.vehdjk.com

[R78] 交互式菜单
来源：http://bcl.shanyushiyangtech.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sgb.ydjk.org.cn

[R79] 解析命令行选项
来源：http://hrb.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zlo.ybcxt.top

[R80] 查看脚本执行耗时
来源：http://mpv.fengsongda.top

time ./run.sh
来源：http://mrh.yanxiufei.cn

================================================================================
来源：http://cge.gotoacloud.top

S. C / C++ 专题
来源：http://wsd.nanxuanxn.top

================================================================================
来源：http://qlt.mhx1999.top

[S01] C：Hello World
来源：http://jyq.hnqzz.top

#include <stdio.h>
来源：http://bhk.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://ssr.yvedp.cn

[S02] C：变量与格式化输出
来源：http://hma.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://tbx.chenlongwang.top

[S03] C：读入整数
来源：http://zhx.yj202588.top

int x; scanf("%d", &x);
来源：http://rzo.ppjwa.cn

[S04] C：字符串复制
来源：http://ijh.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://djk.sjlbkw.cn

[S05] C：字符串长度
来源：http://uzx.tanke756.top

strlen(s)
来源：http://gcb.andypj.xyz

[S06] C：字符串比较
来源：http://opr.shuidangran.top

strcmp(a, b) == 0
来源：http://zwb.zycfv.cn

[S07] C：数组遍历求和
来源：http://tth.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rgm.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://agc.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kjs.guowangkeji.top

[S09] C：结构体定义与初始化
来源：http://xwp.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kbg.yuxming.cn

[S10] C：指针与解引用
来源：http://nml.fzhhl.top

int *p = &a;  *p = 5;
来源：http://ryw.pengpengdd.cyou

[S11] C：逐行读文件
来源：http://vlg.316326.xyz

FILE *f = fopen("a.txt", "r");
来源：http://zds.yangfankeji.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://jht.hongshengwenyu.top

fclose(f);
来源：http://uve.tian-w.cn

[S12] C：写文件
来源：http://rym.gzhubu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://goj.sxryk.cn

[S13] C：宏定义
来源：http://jwy.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eon.hesvh.cn

[S14] C：枚举
来源：http://zuq.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://fze.guannengcc.top

[S15] C：类型转换
来源：http://alt.ehwqpu.com

(double) a / b
来源：http://cvk.cdnleiting.top

[S16] C：位操作置位
来源：http://qzb.gaohongyu789.top

x |= (1 << 3);
来源：http://wfo.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://jli.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gje.fzhhl.top

[S18] C：命令行参数
来源：http://hbu.nanxuanxn.top

int main(int argc, char **argv)
来源：http://fjy.shangyingyoupin.top

[S19] C：快速排序
来源：http://arq.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://ylf.pycfn.com

[S20] C：二分查找
来源：http://oxd.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cfi.quarkkingdee.top

[S21] C：字符类别判断
来源：http://abx.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rqd.zhijiandao.cn

[S22] C：字符串转数字
来源：http://qut.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wrm.yongpay.top

[S23] C：随机数
来源：http://hpa.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://baq.yuanzhike.top

[S24] C：获取本地时间
来源：http://vbx.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gmn.zhixingplan.top

[S25] C：内存拷贝
来源：http://oni.c1oappe.top

memcpy(dst, src, n);
来源：http://ehb.jqgfzy.top

[S26] C：内存清零
来源：http://jdf.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://wxv.shangyingyoupin.top

[S27] C：定义常量
来源：http://ipq.xuanzx.com

const double PI = 3.14159;
来源：http://kba.guannengcc.top

[S28] C：静态变量
来源：http://ucd.hywenlv.cn

static int counter = 0;
来源：http://fuu.sxryk.cn

[S29] C：变参函数
来源：http://glx.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bpg.shanyushiyangtech.top

[S30] C：头文件保护
来源：http://ety.ehwqpu.com

#ifndef X_H
来源：http://wmi.chenlongwang.top

#define X_H
来源：http://juu.xylfe.cn

#endif
来源：http://smx.shuidangran.top

[S31] C++：Hello World
来源：http://bnc.andypj.xyz

#include <iostream>
来源：http://jev.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://ala.uphjek.com

[S32] C++：字符串
来源：http://vib.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://kpp.yfazqb.com

[S33] C++：vector 增删
来源：http://gxh.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uzr.hnqzz.top

[S34] C++：遍历 vector
来源：http://ibl.chenlongwang.top

for (auto &x : v) { std::cout << x; }
来源：http://jjw.zdbjq.cn

[S35] C++：map
来源：http://nru.zhijiandao.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pgp.shanyushiyangkeji.top

[S36] C++：unordered_map
来源：http://qle.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kre.jinyuanbaomall.cn

[S37] C++：set
来源：http://hoo.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kdh.zdqjudy.top

[S38] C++：排序
来源：http://zqt.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://zht.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://mug.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fmd.sweek.top

[S40] C++：查找元素
来源：http://qva.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jzn.xylfe.cn

[S41] C++：类与构造函数
来源：http://snw.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mjv.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://aaq.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://rfe.zhengqikj.top

[S43] C++：智能指针
来源：http://enx.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://lcm.dashuyun.cn

[S44] C++：引用传参
来源：http://jss.kuanghao11.cn

void inc(int &x) { ++x; }
来源：http://ujr.shzxlz.cn

[S45] C++：lambda
来源：http://ieo.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://jfz.yvedp.cn

[S46] C++：函数模板
来源：http://etb.jqgfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://alk.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://yeb.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gvj.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://aai.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://pwi.tanke756.top

while (std::getline(in, line)) { }
来源：http://gmg.ivvv.top

[S49] C++：写文件
来源：http://xnh.jlsjyb.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://adq.hnxiangtu.top

[S50] C++：格式化数字
来源：http://eml.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://woe.ctjpmb.com

[S51] C++：显式类型转换
来源：http://mcb.cucudq.cn

static_cast<double>(a) / b
来源：http://nhe.sufxvd.cn

[S52] C++：const 与 noexcept
来源：http://dcu.xuanzx.com

int size() const noexcept { return n_; }
来源：http://owc.hysaishi.cn

[S53] C++：移动语义
来源：http://msa.ywan-chungtsiang.top

std::vector<int> w = std::move(v);
来源：http://xfc.nanxinkj.top

[S54] C++：异常处理
来源：http://zmo.nanxinkj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gpu.ehwqpu.com

[S55] C++：结构化绑定
来源：http://eyx.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rjq.sjlbkw.cn

[S56] C++：optional
来源：http://sen.nanxuanxn.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pgn.wangdashe.top

[S57] C++：编译期常量
来源：http://eqg.daria6918.cn

constexpr int N = 10;
来源：http://phd.guowangkeji.top

[S58] C++：命名空间
来源：http://lwo.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://ekh.cqqwz.cn

[S59] C++：静态断言
来源：http://seq.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qgu.316326.xyz

[S60] C++：遍历并删除元素
来源：http://uhm.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qge.tian-w.cn

================================================================================
来源：http://gwx.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uno.bjfxy.top

================================================================================
来源：http://jgk.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://fje.ybcxt.top

println("Hello")
来源：http://zvl.pycfn.com

[T02] Kotlin：变量
来源：http://pmy.feifeiyinyue.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://awi.yueranfly.top

[T03] Kotlin：字符串模板
来源：http://mvz.zhijiandao.cn

"值: $b"
来源：http://hgq.epnwcf.com

[T04] Kotlin：空安全
来源：http://jzs.sufxvd.cn

val n: String? = null;  n?.length
来源：http://lpq.tarul.cn

[T05] Kotlin：when 表达式
来源：http://yol.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cap.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://rif.pycfn.com

listOf(1, 2, 3).map { it * 2 }
来源：http://puy.sjlbkw.cn

[T07] Kotlin：集合过滤
来源：http://zbc.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tsn.daria6918.cn

[T08] Kotlin：数据类
来源：http://ptz.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://lcs.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://pip.hywenlv.cn

fun String.exclaim() = this + "!"
来源：http://nuz.bjfxy.top

[T10] Kotlin：默认参数
来源：http://tox.havefunace.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yps.daria6918.cn

[T11] Kotlin：协程
来源：http://qjv.wangdashe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cwp.hnqzz.top

[T12] Kotlin：解构声明
来源：http://rtp.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://cts.meibo888.top

[T13] Kotlin：只读 Map
来源：http://hiv.svipenyu.cn

val m = mapOf("a" to 1)
来源：http://zfn.yangfankeji.com

[T14] Kotlin：循环
来源：http://hpd.yj20258.top

for (i in 1..10) println(i)
来源：http://szr.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://ghx.hfpthk.cn

interface Shape { fun area(): Double }
来源：http://bwn.yfazqb.com

[T16] Swift：Hello World
来源：http://tyd.ppjwa.cn

print("Hello")
来源：http://mdf.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://hrs.xylfe.cn

var a = 1;  let b = 2
来源：http://cqs.wangdashe.top

[T18] Swift：字符串插值
来源：http://ebi.yuxming.cn

"值: \(b)"
来源：http://pad.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://zmj.52xcode.cn

if let n = opt { print(n) }
来源：http://udx.yj20258888.top

[T20] Swift：数组操作
来源：http://psg.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://abj.ydzc1.top

[T21] Swift：遍历
来源：http://rvo.sweek.top

for x in a { print(x) }
来源：http://hae.jiagoushi.top

[T22] Swift：字典
来源：http://qxh.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://yry.mhx1999.top


<!-- 参考信息 -->