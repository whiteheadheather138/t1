代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://yng.sufxvd.cn

[R26] 命令替换
来源：http://nje.ydzc1.top

now=$(date +%F); echo "$now"
来源：http://nal.ydzc1.top

[R27] 算术展开
来源：http://lmd.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://fty.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://gem.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://ivg.xuetiantiany.cn

[R29] 定义函数
来源：http://kdh.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qfj.jinqigufen.top

[R30] 函数返回状态码
来源：http://yiz.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://qfi.zhengqikj.top

[R31] 局部变量
来源：http://ney.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://uoy.fehbvm.com

[R32] 参数个数校验
来源：http://ogp.epnwcf.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mas.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://ggm.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ovd.hongshengwenyu.top

[R34] 退出时清理
来源：http://eit.bjfxy.top

trap 'rm -f "$tmp"' EXIT
来源：http://vyu.andypj.xyz

[R35] 后台执行并等待
来源：http://nwh.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://umq.bbcook.cn

[R36] 并发执行多个任务
来源：http://sdv.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qoj.xziqi.cn

[R37] 把输出赋给变量
来源：http://mep.nanxinkj.top

files=$(ls -1)
来源：http://kdw.yueranfly.top

[R38] 管道串联
来源：http://sdx.xuetiantiany.cn

cat a.txt | grep -i error | wc -l
来源：http://ucv.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://ljd.hysaishi.cn

cmd > out.log 2>&1
来源：http://vlf.sysykeji.top

[R40] 追加写日志
来源：http://lhn.jyoumei.cn

echo "log" >> out.log
来源：http://rey.9152youxi.cn

[R41] 丢弃输出
来源：http://ftb.zdqjudy.top

cmd >/dev/null 2>&1
来源：http://svj.gzhubu.top

[R42] 输入重定向
来源：http://mht.zhixingplan.top

wc -l < a.txt
来源：http://nal.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://bjn.yfazqb.com

find . -name "*.log" -type f
来源：http://tgl.tianlin.xyz

[R44] 按修改时间查找
来源：http://acv.sxryk.cn

find . -mtime -7 -type f
来源：http://gur.jqgufenzy.top

[R45] 批量删除
来源：http://fyb.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://jfq.snrcjt.cn

[R46] 递归替换文件内容
来源：http://axv.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iql.sxryk.cn

[R47] sed 单行替换
来源：http://hmf.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rhk.gaohongyu789.top

[R48] awk 取指定列
来源：http://mvs.cashguo.top

awk '{print $1, $3}' a.txt
来源：http://bqp.yuanzhike.top

[R49] awk 带条件
来源：http://rph.jyoumei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gpd.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://nxb.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://iiw.zhijiandao.cn

[R51] 排序去重取前几
来源：http://avp.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mwn.birdmap.top

[R52] 统计行数
来源：http://zmm.sufxvd.cn

wc -l a.txt
来源：http://qcw.yj202588.top

[R53] 查看文件头与实时尾
来源：http://woc.yuanzhike.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://toi.quarkkingdee.top

[R54] 比较两个文件
来源：http://pno.9152youxi.cn

diff a.txt b.txt
来源：http://mex.chenjidiqi.icu

[R55] 压缩与解压
来源：http://hxf.aibaodan.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jek.nanxinkj.top

[R56] 远程拷贝
来源：http://vcu.zhengqikj.top

scp file user@host:/path/
来源：http://ykw.epnwcf.com

[R57] 远程执行命令
来源：http://sox.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://nzz.ybcxt.top

[R58] 下载文件
来源：http://mgt.hysaishi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mnj.vqdsnc.cn

[R59] 发 POST JSON
来源：http://cxc.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://moh.gaohongyu789.top

[R60] 只看 HTTP 状态码
来源：http://ukb.ppjwa.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hbt.nanxinkj.top

[R61] 磁盘占用
来源：http://pir.feifeiyinyue.top

df -h;  du -sh *
来源：http://paf.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://hpz.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://xjg.quarkkingdee.top

[R63] 内存与进程
来源：http://nhb.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://dhf.wangdashe.top

[R64] 结束进程
来源：http://evc.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://oty.sjlbkw.cn

[R65] 查看端口占用
来源：http://guw.shangyingyoupin.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hss.hysaishi.cn

[R66] 定时任务
来源：http://nqv.tarul.cn

crontab -e;  crontab -l
来源：http://lty.daria6918.cn

[R67] 生成随机十六进制串
来源：http://tok.cdnleiting.top

openssl rand -hex 16
来源：http://kqa.fehbvm.com

[R68] 计算文件校验值
来源：http://eck.cqqwz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://upx.dianchejie.cn

[R69] 生成随机密码
来源：http://gyk.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://myt.yj20258.top

[R70] 时间戳与互转
来源：http://rid.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://bvo.aibaodan.cn

[R71] 日期格式化
来源：http://gdg.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ewq.hfpthk.cn

[R72] 等待端口就绪
来源：http://rxr.chenjidiqi.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://uio.jqgufenzy.top

[R73] 分割大日志
来源：http://jvq.xinyue.icu

split -l 1000 big.log part_
来源：http://tij.chenlongwang.top

[R74] 批量重命名
来源：http://qbt.cashguo.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wnm.hysaishi.cn

[R75] 导出环境变量
来源：http://zwj.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://sbx.zhixingplan.top

[R76] 使用临时文件
来源：http://xkt.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bfa.fktsv.cn

[R77] 读取用户输入
来源：http://utq.yonumen.top

read -rp "请输入: " ans
来源：http://vmc.zhoulong.xyz

[R78] 交互式菜单
来源：http://tuu.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gbg.redwolf501.top

[R79] 解析命令行选项
来源：http://bda.dashuyun.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sjt.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://bah.ehwqpu.com

time ./run.sh
来源：http://ehb.316326.xyz

================================================================================
来源：http://ctg.haohaochexian.top

S. C / C++ 专题
来源：http://kkc.xingfuxueyuan.xyz

================================================================================
来源：http://aqg.sweek.top

[S01] C：Hello World
来源：http://snz.jianghu66.top

#include <stdio.h>
来源：http://fvp.xuanzx.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://eyf.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://vci.shangyingyoupin.top

int a = 10; printf("%d\n", a);
来源：http://fyv.0kj1m.cn

[S03] C：读入整数
来源：http://fga.zycfv.cn

int x; scanf("%d", &x);
来源：http://hry.fzhhl.top

[S04] C：字符串复制
来源：http://jea.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://xor.wangshuangyany.cn

[S05] C：字符串长度
来源：http://fgy.ybcxt.top

strlen(s)
来源：http://noi.fehbvm.com

[S06] C：字符串比较
来源：http://lwi.xuanzx.com

strcmp(a, b) == 0
来源：http://wzz.ywan-chungtsiang.top

[S07] C：数组遍历求和
来源：http://pfh.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uts.quarkkingdee.top

[S08] C：动态内存分配与释放
来源：http://ckr.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rbq.birdmap.top

[S09] C：结构体定义与初始化
来源：http://ovu.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nwg.havefunace.top

[S10] C：指针与解引用
来源：http://lpk.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://iax.zdqjudy.top

[S11] C：逐行读文件
来源：http://mar.wangshuangyany.cn

FILE *f = fopen("a.txt", "r");
来源：http://rmp.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ptd.9152youxi.cn

fclose(f);
来源：http://rso.hnqzz.top

[S12] C：写文件
来源：http://pgg.hnqzz.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uoy.zhongyouzk.top

[S13] C：宏定义
来源：http://obc.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tgb.cheryme.top

[S14] C：枚举
来源：http://swa.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://ycz.svipenyu.cn

[S15] C：类型转换
来源：http://vho.iojbl.cn

(double) a / b
来源：http://axl.zhoulong.xyz

[S16] C：位操作置位
来源：http://eyx.snrcjt.cn

x |= (1 << 3);
来源：http://njf.zhixingplan.top

[S17] C：安全拼接字符串
来源：http://fji.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jrp.daria6918.cn

[S18] C：命令行参数
来源：http://osu.cqqwz.cn

int main(int argc, char **argv)
来源：http://gdp.shanyushiyangtech.top

[S19] C：快速排序
来源：http://lrj.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fki.andypj.xyz

[S20] C：二分查找
来源：http://rcb.yj20258888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zsl.fehbvm.com

[S21] C：字符类别判断
来源：http://aie.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ish.zhongyouzk.top

[S22] C：字符串转数字
来源：http://vjj.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ztk.gogol.net.cn

[S23] C：随机数
来源：http://spc.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://obo.shuidangran.top

[S24] C：获取本地时间
来源：http://xby.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://apv.hywenlv.cn

[S25] C：内存拷贝
来源：http://jdx.sufxvd.cn

memcpy(dst, src, n);
来源：http://hla.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://vze.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://izp.yj20258888.top

[S27] C：定义常量
来源：http://kbs.cucudq.cn

const double PI = 3.14159;
来源：http://mhr.nanxuanxn.top

[S28] C：静态变量
来源：http://ioi.vqdsnc.cn

static int counter = 0;
来源：http://ckv.ppjwa.cn

[S29] C：变参函数
来源：http://gnj.guowangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://srg.tianlin.xyz

[S30] C：头文件保护
来源：http://rwr.vehdjk.com

#ifndef X_H
来源：http://axb.yangfankeji.com

#define X_H
来源：http://vrq.jlsjyb.cn

#endif
来源：http://muw.yvedp.cn

[S31] C++：Hello World
来源：http://ebh.svipenyu.cn

#include <iostream>
来源：http://zbw.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://xwz.chenlongwang.top

[S32] C++：字符串
来源：http://gen.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://shv.chenjidiqi.icu

[S33] C++：vector 增删
来源：http://qel.shanyushiyangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dqy.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://asn.aizwys.cn

for (auto &x : v) { std::cout << x; }
来源：http://tpz.nwbrower.top

[S35] C++：map
来源：http://sem.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dcf.9152youxi.cn

[S36] C++：unordered_map
来源：http://fcz.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kow.bbcook.cn

[S37] C++：set
来源：http://lhc.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://szu.cheryme.top

[S38] C++：排序
来源：http://ibi.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://mrb.hesvh.cn

[S39] C++：自定义比较器排序
来源：http://hmr.zdbjq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ndc.sweek.top

[S40] C++：查找元素
来源：http://kgb.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nxi.hammf.cn

[S41] C++：类与构造函数
来源：http://kzg.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wms.dashuyun.cn

[S42] C++：继承与虚函数
来源：http://xch.ywan-chungtsiang.top

class B : public Base { public: void f() override {} };
来源：http://azo.havefunace.top

[S43] C++：智能指针
来源：http://gdn.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://qkx.kuanghao11.cn

[S44] C++：引用传参
来源：http://crj.sufxvd.cn

void inc(int &x) { ++x; }
来源：http://mhy.wangdashe.top

[S45] C++：lambda
来源：http://fmw.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://evh.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://gyf.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://heh.shangyingyoupin.top

[S47] C++：结构化绑定遍历
来源：http://tyr.vqdsnc.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://anj.jinqigfzy.top

[S48] C++：逐行读文件
来源：http://mgk.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://zdo.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://bsn.xziqi.cn

[S49] C++：写文件
来源：http://ajw.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pwi.ybcxt.top

[S50] C++：格式化数字
来源：http://kmt.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bxl.aibaodan.cn

[S51] C++：显式类型转换
来源：http://jug.hesvh.cn

static_cast<double>(a) / b
来源：http://far.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://aqf.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://hlj.jlsjyb.cn

[S53] C++：移动语义
来源：http://gom.shzxlz.cn

std::vector<int> w = std::move(v);
来源：http://lra.dashuyun.cn

[S54] C++：异常处理
来源：http://cpw.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bgs.gotoacloud.top

[S55] C++：结构化绑定
来源：http://oup.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gaf.quarkkingdee.top

[S56] C++：optional
来源：http://wqq.dashuyun.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cwt.ctjpmb.com

[S57] C++：编译期常量
来源：http://rzy.jianghu66.top

constexpr int N = 10;
来源：http://get.zhiwuduotai.top

[S58] C++：命名空间
来源：http://rtu.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://btv.ivvv.top

[S59] C++：静态断言
来源：http://mns.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://naq.ydzc1.top

[S60] C++：遍历并删除元素
来源：http://ean.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qza.shangyingyoupin.top

================================================================================
来源：http://eiy.mhx1999.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vef.chenjidiqi.icu

================================================================================
来源：http://uyd.meibo888.top

[T01] Kotlin：Hello World
来源：http://zko.jiagoushi.top

println("Hello")
来源：http://dtf.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://xuk.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://reg.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://tiu.hesvh.cn

"值: $b"
来源：http://qfc.yj20258.top

[T04] Kotlin：空安全
来源：http://zub.daxiang520.top

val n: String? = null;  n?.length
来源：http://mdd.yvedp.cn

[T05] Kotlin：when 表达式
来源：http://zzd.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pme.hesvh.cn

[T06] Kotlin：集合映射
来源：http://qgb.gaohongyu789.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zus.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://bmr.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cnh.ehwqpu.com

[T08] Kotlin：数据类
来源：http://wfv.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://sjz.yuanzhike.top

[T09] Kotlin：扩展函数
来源：http://drs.xylfe.cn

fun String.exclaim() = this + "!"
来源：http://ehv.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://ikf.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yvz.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://lcx.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://iyn.ehwqpu.com

[T12] Kotlin：解构声明
来源：http://mey.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://cyx.svipenyu.cn

[T13] Kotlin：只读 Map
来源：http://mks.ybcxt.top

val m = mapOf("a" to 1)
来源：http://ayv.vqdsnc.cn

[T14] Kotlin：循环
来源：http://gfx.shzxlz.cn

for (i in 1..10) println(i)
来源：http://wxn.zhengqikj.top

[T15] Kotlin：接口
来源：http://huj.yongpay.top

interface Shape { fun area(): Double }
来源：http://tuy.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://xcd.mhx1999.top

print("Hello")
来源：http://hbt.daxiang520.top

[T17] Swift：变量与常量
来源：http://jlq.hysaishi.cn

var a = 1;  let b = 2
来源：http://kvq.316326.xyz

[T18] Swift：字符串插值
来源：http://zks.shanyushiyangkeji.top

"值: \(b)"
来源：http://qax.xuanzx.com

[T19] Swift：可选绑定
来源：http://cku.cheryme.top

if let n = opt { print(n) }
来源：http://asj.xuanzx.com

[T20] Swift：数组操作
来源：http://suk.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://usu.9152youxi.cn

[T21] Swift：遍历
来源：http://cnj.chenjidiqi.icu

for x in a { print(x) }
来源：http://aje.tianlin.xyz

[T22] Swift：字典
来源：http://kdn.birdmap.top

var d = ["a": 1];  d["b"] = 2
来源：http://qma.guannengcc.top

[T23] Swift：函数
来源：http://otk.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://txr.ywan-chungtsiang.top

[T24] Swift：闭包
来源：http://qet.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dfx.ppjwa.cn

[T25] Swift：结构体
来源：http://mnt.shanyushiyangtech.top

struct P { var x: Int }
来源：http://pyq.zhengqikj.top

[T26] Swift：类与重写
来源：http://eau.dianchejie.cn

class A: Base { override func f() {} }
来源：http://mhh.zhongyouzk.top

[T27] Swift：错误处理
来源：http://dja.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://rzx.tianlin.xyz

[T28] Swift：枚举
来源：http://cox.zhiwuduotai.top

enum Color { case red, green }
来源：http://edr.316326.xyz


<!-- 参考信息 -->