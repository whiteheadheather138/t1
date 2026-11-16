代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ioi.shangyingyoupin.top

[R24] 大小写转换
来源：http://ffv.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://yrz.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://qnx.sufxvd.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://djf.tian-w.cn

[R26] 命令替换
来源：http://hxl.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://lua.nanxinkj.top

[R27] 算术展开
来源：http://den.wangdashe.top

echo $((1 + 2 * 3))
来源：http://pcw.fanxiaobao.xyz

[R28] 浮点运算
来源：http://fgf.gotoacloud.top

echo "scale=2; 10/3" | bc
来源：http://uje.tianlin.xyz

[R29] 定义函数
来源：http://zui.quarkkingdee.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xbf.hnqzz.top

[R30] 函数返回状态码
来源：http://blb.shuidangran.top

f() { return 0; }; f || echo "失败了"
来源：http://sqd.jinqigufen.top

[R31] 局部变量
来源：http://gcm.daria6918.cn

f() { local x=1; echo "$x"; }
来源：http://kde.xuetiantiany.cn

[R32] 参数个数校验
来源：http://ouz.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aop.fktsv.cn

[R33] 捕获错误并提示行号
来源：http://xaz.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vzr.gogol.net.cn

[R34] 退出时清理
来源：http://isi.yonumen.top

trap 'rm -f "$tmp"' EXIT
来源：http://huy.zycfv.cn

[R35] 后台执行并等待
来源：http://grq.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://erx.dashuyun.cn

[R36] 并发执行多个任务
来源：http://skp.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qtp.dashuyun.cn

[R37] 把输出赋给变量
来源：http://mkf.sysykeji.top

files=$(ls -1)
来源：http://gwk.fengsongda.top

[R38] 管道串联
来源：http://gvf.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://kuz.yueranfly.top

[R39] 重定向标准输出与错误
来源：http://vnd.ydzc1.top

cmd > out.log 2>&1
来源：http://wcp.ehwqpu.com

[R40] 追加写日志
来源：http://gyh.c1oappe.top

echo "log" >> out.log
来源：http://wig.ctjpmb.com

[R41] 丢弃输出
来源：http://vxt.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://mbi.fengsongda.top

[R42] 输入重定向
来源：http://edg.chenlongwang.top

wc -l < a.txt
来源：http://zqd.316326.xyz

[R43] 按名字查找文件
来源：http://zvc.zhixingplan.top

find . -name "*.log" -type f
来源：http://zgm.daxiang520.top

[R44] 按修改时间查找
来源：http://sgw.ctjpmb.com

find . -mtime -7 -type f
来源：http://hdv.zhijiandao.cn

[R45] 批量删除
来源：http://mmt.sxryk.cn

find . -name "*.tmp" -delete
来源：http://zzn.cheryme.top

[R46] 递归替换文件内容
来源：http://sju.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mxw.uphjek.com

[R47] sed 单行替换
来源：http://iiz.zycfv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://esx.nanxinkj.top

[R48] awk 取指定列
来源：http://bua.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://ldn.fzhhl.top

[R49] awk 带条件
来源：http://tws.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zcs.shzxlz.cn

[R50] awk 求和
来源：http://knv.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://cmb.ehwqpu.com

[R51] 排序去重取前几
来源：http://slg.zhiwuduotai.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xtl.epnwcf.com

[R52] 统计行数
来源：http://ief.sysykeji.top

wc -l a.txt
来源：http://lmk.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://sbw.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oxc.andypj.xyz

[R54] 比较两个文件
来源：http://yqc.chenjidiqi.icu

diff a.txt b.txt
来源：http://kmk.gotoacloud.top

[R55] 压缩与解压
来源：http://smo.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lai.jyoumei.cn

[R56] 远程拷贝
来源：http://jzh.9152youxi.cn

scp file user@host:/path/
来源：http://esl.zdbjq.cn

[R57] 远程执行命令
来源：http://onz.sufxvd.cn

ssh user@host 'uptime'
来源：http://ozr.uphjek.com

[R58] 下载文件
来源：http://fmc.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rrx.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://the.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jux.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://ybh.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ifh.wangshuangyany.cn

[R61] 磁盘占用
来源：http://wgf.sweek.top

df -h;  du -sh *
来源：http://zkn.yongpay.top

[R62] 找最占空间的文件
来源：http://mdx.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://wsg.ivvv.top

[R63] 内存与进程
来源：http://quk.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://sjf.havefunace.top

[R64] 结束进程
来源：http://cwp.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://zvk.tarul.cn

[R65] 查看端口占用
来源：http://nxg.havefunace.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qrc.9152youxi.cn

[R66] 定时任务
来源：http://zet.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://bfq.yangfankeji.com

[R67] 生成随机十六进制串
来源：http://xvd.sufxvd.cn

openssl rand -hex 16
来源：http://qqa.gotoacloud.top

[R68] 计算文件校验值
来源：http://iuh.zhixingplan.top

sha256sum a.txt;  md5sum a.txt
来源：http://stf.hesvh.cn

[R69] 生成随机密码
来源：http://epp.yj20258.top

head -c 16 /dev/urandom | base64
来源：http://uma.jianghu66.top

[R70] 时间戳与互转
来源：http://oiu.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://wcq.sxryk.cn

[R71] 日期格式化
来源：http://zxa.shanyushiyangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ahe.dianchejie.cn

[R72] 等待端口就绪
来源：http://qjd.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xhr.andypj.xyz

[R73] 分割大日志
来源：http://epy.snrcjt.cn

split -l 1000 big.log part_
来源：http://zly.sweek.top

[R74] 批量重命名
来源：http://onf.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yte.tian-w.cn

[R75] 导出环境变量
来源：http://fky.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://gha.guannengcc.top

[R76] 使用临时文件
来源：http://bme.yj20258888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://joi.cucudq.cn

[R77] 读取用户输入
来源：http://jrm.yj20258888.top

read -rp "请输入: " ans
来源：http://jgs.chenzaomai.com

[R78] 交互式菜单
来源：http://jbi.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kfc.9152youxi.cn

[R79] 解析命令行选项
来源：http://ccm.jqgufenzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sfu.sufxvd.cn

[R80] 查看脚本执行耗时
来源：http://gux.birdmap.top

time ./run.sh
来源：http://ofe.xuetiantiany.cn

================================================================================
来源：http://ryw.vehdjk.com

S. C / C++ 专题
来源：http://ltt.ybcxt.top

================================================================================
来源：http://geq.yuanzhike.top

[S01] C：Hello World
来源：http://mst.fktsv.cn

#include <stdio.h>
来源：http://wwx.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ymq.zhengqikj.top

[S02] C：变量与格式化输出
来源：http://crj.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://wvl.jqgfzy.top

[S03] C：读入整数
来源：http://abj.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://hay.vehdjk.com

[S04] C：字符串复制
来源：http://ifh.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nfq.sxryk.cn

[S05] C：字符串长度
来源：http://ems.zhiwuduotai.top

strlen(s)
来源：http://szl.aizwys.cn

[S06] C：字符串比较
来源：http://ict.zhijiandao.cn

strcmp(a, b) == 0
来源：http://cbt.svipenyu.cn

[S07] C：数组遍历求和
来源：http://mha.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tlt.jiagoushi.top

[S08] C：动态内存分配与释放
来源：http://sgb.snrcjt.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vmb.yongpay.top

[S09] C：结构体定义与初始化
来源：http://zgz.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zgk.smart0.xyz

[S10] C：指针与解引用
来源：http://pas.c1oappe.top

int *p = &a;  *p = 5;
来源：http://czc.hesvh.cn

[S11] C：逐行读文件
来源：http://edh.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://cra.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zig.cheryme.top

fclose(f);
来源：http://ajp.chenjidiqi.icu

[S12] C：写文件
来源：http://zpt.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://urb.yuanzhike.top

[S13] C：宏定义
来源：http://idp.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rrj.hysaishi.cn

[S14] C：枚举
来源：http://nts.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://kkl.yonumen.top

[S15] C：类型转换
来源：http://czm.52xcode.cn

(double) a / b
来源：http://wxa.cashguo.top

[S16] C：位操作置位
来源：http://buo.hfpthk.cn

x |= (1 << 3);
来源：http://edy.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://qvu.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dtk.redwolf501.top

[S18] C：命令行参数
来源：http://ntq.andypj.xyz

int main(int argc, char **argv)
来源：http://vop.hfpthk.cn

[S19] C：快速排序
来源：http://hfj.cheryme.top

qsort(a, n, sizeof(int), cmp);
来源：http://hcp.fktsv.cn

[S20] C：二分查找
来源：http://zrf.zhiwuduotai.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://afe.sjlbkw.cn

[S21] C：字符类别判断
来源：http://bjl.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://olw.cdnleiting.top

[S22] C：字符串转数字
来源：http://xge.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://klo.hesvh.cn

[S23] C：随机数
来源：http://gkd.shuidangran.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hlq.cdnleiting.top

[S24] C：获取本地时间
来源：http://bgo.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vme.epnwcf.com

[S25] C：内存拷贝
来源：http://jdo.xinyue.icu

memcpy(dst, src, n);
来源：http://ipu.fengsongda.top

[S26] C：内存清零
来源：http://uym.yuanzhike.top

memset(a, 0, sizeof a);
来源：http://ien.bbcook.cn

[S27] C：定义常量
来源：http://zlk.haohaochexian.top

const double PI = 3.14159;
来源：http://nab.tian-w.cn

[S28] C：静态变量
来源：http://lsu.uphjek.com

static int counter = 0;
来源：http://jjg.52xcode.cn

[S29] C：变参函数
来源：http://ube.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://irs.zdqjudy.top

[S30] C：头文件保护
来源：http://qds.yuanzhike.top

#ifndef X_H
来源：http://lcq.iojbl.cn

#define X_H
来源：http://ixn.hywenlv.cn

#endif
来源：http://lds.wangdashe.top

[S31] C++：Hello World
来源：http://rjf.zhengqikj.top

#include <iostream>
来源：http://lfn.wangshuangyany.cn

int main() { std::cout << "Hello\n"; }
来源：http://xag.smart0.xyz

[S32] C++：字符串
来源：http://ufg.jyoumei.cn

std::string s = "hi";  s += "!";
来源：http://clg.tarul.cn

[S33] C++：vector 增删
来源：http://egv.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zdm.daxiang520.top

[S34] C++：遍历 vector
来源：http://uhy.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://sib.cucudq.cn

[S35] C++：map
来源：http://yxr.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kag.ivvv.top

[S36] C++：unordered_map
来源：http://rkh.ydzc1.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ijz.sysykeji.top

[S37] C++：set
来源：http://hlq.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://azo.hongshengwenyu.top

[S38] C++：排序
来源：http://hzs.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://xrv.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://qrc.chenjidiqi.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hbr.xuanzx.com

[S40] C++：查找元素
来源：http://oic.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cjt.zycfv.cn

[S41] C++：类与构造函数
来源：http://sjk.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ayt.hcnkem.com

[S42] C++：继承与虚函数
来源：http://jku.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://eki.hnqzz.top

[S43] C++：智能指针
来源：http://vbh.sxryk.cn

auto p = std::make_unique<int>(5);
来源：http://tif.haohaochexian.top

[S44] C++：引用传参
来源：http://ski.gotoacloud.top

void inc(int &x) { ++x; }
来源：http://qos.ydzc1.top

[S45] C++：lambda
来源：http://wnr.svipenyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wad.birdmap.top

[S46] C++：函数模板
来源：http://jok.0kj1m.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://paj.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://ozg.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mzv.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://mqw.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pkn.cheryme.top

while (std::getline(in, line)) { }
来源：http://oix.pengpengdd.cyou

[S49] C++：写文件
来源：http://kyd.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gqz.daxiang520.top

[S50] C++：格式化数字
来源：http://uxg.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mzj.zdbjq.cn

[S51] C++：显式类型转换
来源：http://awo.epnwcf.com

static_cast<double>(a) / b
来源：http://utb.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://lju.yfazqb.com

int size() const noexcept { return n_; }
来源：http://gkp.hnqzz.top

[S53] C++：移动语义
来源：http://jgk.ywan-chungtsiang.top

std::vector<int> w = std::move(v);
来源：http://dqm.jianghu66.top

[S54] C++：异常处理
来源：http://vfh.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://szs.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://kqs.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qql.ydjk.org.cn

[S56] C++：optional
来源：http://swl.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ujt.cashguo.top

[S57] C++：编译期常量
来源：http://srx.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://tsf.andypj.xyz

[S58] C++：命名空间
来源：http://gcj.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://kbz.316326.xyz

[S59] C++：静态断言
来源：http://vvh.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ghw.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://yoe.gaohongyu789.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wso.feifeiyinyue.top

================================================================================
来源：http://yzi.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://smm.birdmap.top

================================================================================
来源：http://tgx.c1oappe.top

[T01] Kotlin：Hello World
来源：http://vef.ybcxt.top

println("Hello")
来源：http://nsl.yvedp.cn

[T02] Kotlin：变量
来源：http://ubi.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bsf.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://app.zdqjudy.top

"值: $b"
来源：http://kaa.gogol.net.cn

[T04] Kotlin：空安全
来源：http://ezl.9152youxi.cn

val n: String? = null;  n?.length
来源：http://iot.yonumen.top

[T05] Kotlin：when 表达式
来源：http://roh.dashuyun.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vxt.uphjek.com

[T06] Kotlin：集合映射
来源：http://ptw.zycfv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tqx.yanxiufei.cn

[T07] Kotlin：集合过滤
来源：http://fpb.uphjek.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://kyi.hesvh.cn

[T08] Kotlin：数据类
来源：http://vsr.quarkkingdee.top

data class User(val name: String, val age: Int)
来源：http://sfy.chenzaomai.com

[T09] Kotlin：扩展函数
来源：http://prv.meibo888.top

fun String.exclaim() = this + "!"
来源：http://deb.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://ozf.shanyushiyangtech.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qeq.quarkkingdee.top

[T11] Kotlin：协程
来源：http://ato.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://btm.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://aru.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://xuw.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://hch.jqgfzy.top

val m = mapOf("a" to 1)
来源：http://rgy.9152youxi.cn

[T14] Kotlin：循环
来源：http://xjg.shuidangran.top

for (i in 1..10) println(i)
来源：http://lgt.svipenyu.cn

[T15] Kotlin：接口
来源：http://hvw.xuetiantiany.cn

interface Shape { fun area(): Double }
来源：http://ahe.xuanzx.com

[T16] Swift：Hello World
来源：http://jot.xuetiantiany.cn

print("Hello")
来源：http://utq.chenlongwang.top

[T17] Swift：变量与常量
来源：http://krp.pycfn.com

var a = 1;  let b = 2
来源：http://spp.xinyue.icu

[T18] Swift：字符串插值
来源：http://dxg.hcnkem.com

"值: \(b)"
来源：http://wyi.hnxiangtu.top

[T19] Swift：可选绑定
来源：http://tnn.zhijiandao.cn

if let n = opt { print(n) }
来源：http://gdr.vqdsnc.cn

[T20] Swift：数组操作
来源：http://pyw.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jra.zhongyouzk.top

[T21] Swift：遍历
来源：http://xos.zhoulong.xyz

for x in a { print(x) }
来源：http://bft.ydjk.org.cn

[T22] Swift：字典
来源：http://kim.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ovc.tanke756.top

[T23] Swift：函数
来源：http://leu.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mfx.andypj.xyz

[T24] Swift：闭包
来源：http://hns.c1oappe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://esm.ivvv.top

[T25] Swift：结构体
来源：http://yfo.jinqigfzy.top

struct P { var x: Int }
来源：http://oql.ctjpmb.com

[T26] Swift：类与重写
来源：http://ack.vehdjk.com

class A: Base { override func f() {} }
来源：http://yvu.gaohongyu789.top


<!-- 参考信息 -->