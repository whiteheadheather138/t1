代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aut.hcnkem.com

[R24] 大小写转换
来源：http://rhq.yj202588.top

echo "${s^^}"; echo "${s,,}"
来源：http://ixg.fanxiaobao.xyz

[R25] 去后缀 / 去前缀
来源：http://xtb.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qcn.iojbl.cn

[R26] 命令替换
来源：http://bop.vqdsnc.cn

now=$(date +%F); echo "$now"
来源：http://xxr.jyoumei.cn

[R27] 算术展开
来源：http://xzv.shanyushiyangtech.top

echo $((1 + 2 * 3))
来源：http://ktl.daria6918.cn

[R28] 浮点运算
来源：http://xvv.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://fbq.shanyushiyangkeji.top

[R29] 定义函数
来源：http://prh.cdnleiting.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hyg.yanxiufei.cn

[R30] 函数返回状态码
来源：http://djo.shuidangran.top

f() { return 0; }; f || echo "失败了"
来源：http://qkf.zhaomingkeji.xyz

[R31] 局部变量
来源：http://bie.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://nez.iojbl.cn

[R32] 参数个数校验
来源：http://dxm.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://thc.yfazqb.com

[R33] 捕获错误并提示行号
来源：http://dqt.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hsz.gaohongyu789.top

[R34] 退出时清理
来源：http://aiy.dashuyun.cn

trap 'rm -f "$tmp"' EXIT
来源：http://liu.wangdashe.top

[R35] 后台执行并等待
来源：http://rmk.yangfankeji.com

sleep 5 & pid=$!; wait "$pid"
来源：http://nai.cqqwz.cn

[R36] 并发执行多个任务
来源：http://ekm.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xjw.haohaochexian.top

[R37] 把输出赋给变量
来源：http://mkt.smart0.xyz

files=$(ls -1)
来源：http://miv.yueranfly.top

[R38] 管道串联
来源：http://ysd.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://jjs.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://ecq.316326.xyz

cmd > out.log 2>&1
来源：http://faw.yj20258.top

[R40] 追加写日志
来源：http://ttz.andypj.xyz

echo "log" >> out.log
来源：http://lun.gotoacloud.top

[R41] 丢弃输出
来源：http://wvk.yj202588.top

cmd >/dev/null 2>&1
来源：http://qar.jianghu66.top

[R42] 输入重定向
来源：http://brf.epnwcf.com

wc -l < a.txt
来源：http://vkg.nanxuanxn.top

[R43] 按名字查找文件
来源：http://amg.jlsjyb.cn

find . -name "*.log" -type f
来源：http://wln.cheryme.top

[R44] 按修改时间查找
来源：http://gpw.nwbrower.top

find . -mtime -7 -type f
来源：http://gfj.sxryk.cn

[R45] 批量删除
来源：http://ugc.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://zhr.shzxlz.cn

[R46] 递归替换文件内容
来源：http://lfl.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gzo.fengsongda.top

[R47] sed 单行替换
来源：http://wmd.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://yaz.yj202588.top

[R48] awk 取指定列
来源：http://ppd.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://jnc.chenzaomai.com

[R49] awk 带条件
来源：http://fyx.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cqj.iojbl.cn

[R50] awk 求和
来源：http://qeu.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://rot.xuanzx.com

[R51] 排序去重取前几
来源：http://bnd.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://rqy.hesvh.cn

[R52] 统计行数
来源：http://dbk.xuanzx.com

wc -l a.txt
来源：http://hvs.pengpengdd.cyou

[R53] 查看文件头与实时尾
来源：http://lmc.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://flw.sjlbkw.cn

[R54] 比较两个文件
来源：http://kax.fanxiaobao.xyz

diff a.txt b.txt
来源：http://hje.jqgufenzy.top

[R55] 压缩与解压
来源：http://kfa.zhiwuduotai.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ygm.zhoulong.xyz

[R56] 远程拷贝
来源：http://kmf.fengsongda.top

scp file user@host:/path/
来源：http://die.pengpengdd.cyou

[R57] 远程执行命令
来源：http://uag.zhijiandao.cn

ssh user@host 'uptime'
来源：http://keb.jianghu66.top

[R58] 下载文件
来源：http://swv.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sdd.yj202588.top

[R59] 发 POST JSON
来源：http://pgu.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zay.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://tiw.ivvv.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oiy.xinyue.icu

[R61] 磁盘占用
来源：http://fsx.nanxuanxn.top

df -h;  du -sh *
来源：http://fvk.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://hpy.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://jtk.daxiang520.top

[R63] 内存与进程
来源：http://ibp.yj20258.top

free -h;  ps aux | grep nginx
来源：http://rlf.xuetiantiany.cn

[R64] 结束进程
来源：http://gkc.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://jkw.bbcook.cn

[R65] 查看端口占用
来源：http://uul.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wgk.quarkkingdee.top

[R66] 定时任务
来源：http://ntg.yj20258.top

crontab -e;  crontab -l
来源：http://oog.gogol.net.cn

[R67] 生成随机十六进制串
来源：http://hkh.fzhhl.top

openssl rand -hex 16
来源：http://dbq.ctjpmb.com

[R68] 计算文件校验值
来源：http://lvd.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://ady.iojbl.cn

[R69] 生成随机密码
来源：http://bye.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://qzj.hywenlv.cn

[R70] 时间戳与互转
来源：http://wko.sjlbkw.cn

date +%s;  date -d @1700000000
来源：http://soq.yongpay.top

[R71] 日期格式化
来源：http://tnq.fanxiaobao.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://tkj.havefunace.top

[R72] 等待端口就绪
来源：http://bqx.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pdi.sysykeji.top

[R73] 分割大日志
来源：http://aeh.xuanzx.com

split -l 1000 big.log part_
来源：http://qzv.feifeiyinyue.top

[R74] 批量重命名
来源：http://cvw.gaohongyu789.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bdz.jlsjyb.cn

[R75] 导出环境变量
来源：http://pdq.vqdsnc.cn

export PATH="$HOME/bin:$PATH"
来源：http://jme.sweek.top

[R76] 使用临时文件
来源：http://qaa.dianchejie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://prc.zycfv.cn

[R77] 读取用户输入
来源：http://uwq.tianlin.xyz

read -rp "请输入: " ans
来源：http://bdi.hesvh.cn

[R78] 交互式菜单
来源：http://vvv.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://wro.xuetiantiany.cn

[R79] 解析命令行选项
来源：http://pgv.zhiwuduotai.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gaq.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://cqk.0kj1m.cn

time ./run.sh
来源：http://orn.chenjidiqi.icu

================================================================================
来源：http://wvb.jyoumei.cn

S. C / C++ 专题
来源：http://ehp.fktsv.cn

================================================================================
来源：http://fca.hfpthk.cn

[S01] C：Hello World
来源：http://vqo.nanxinkj.top

#include <stdio.h>
来源：http://gis.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://onz.hcnkem.com

[S02] C：变量与格式化输出
来源：http://oll.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://dzm.chenzaomai.com

[S03] C：读入整数
来源：http://lps.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://emk.xuanzx.com

[S04] C：字符串复制
来源：http://ige.ywan-chungtsiang.top

char dst[32]; strcpy(dst, "hi");
来源：http://orc.snrcjt.cn

[S05] C：字符串长度
来源：http://phm.jlsjyb.cn

strlen(s)
来源：http://lhp.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://dem.nanxinkj.top

strcmp(a, b) == 0
来源：http://zpa.jqgfzy.top

[S07] C：数组遍历求和
来源：http://lyu.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jor.birdmap.top

[S08] C：动态内存分配与释放
来源：http://xgp.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xde.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://wur.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mre.epnwcf.com

[S10] C：指针与解引用
来源：http://eck.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://njt.bjfxy.top

[S11] C：逐行读文件
来源：http://xep.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://awx.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tqs.jinqigfzy.top

fclose(f);
来源：http://caw.zhixingplan.top

[S12] C：写文件
来源：http://ycj.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tlc.birdmap.top

[S13] C：宏定义
来源：http://ujx.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eqq.pengpengdd.cyou

[S14] C：枚举
来源：http://nqk.fanxiaobao.xyz

enum Color { RED, GREEN, BLUE };
来源：http://hfb.jinyuanbaomall.cn

[S15] C：类型转换
来源：http://bef.jyoumei.cn

(double) a / b
来源：http://aio.xuanzx.com

[S16] C：位操作置位
来源：http://nha.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://uim.epnwcf.com

[S17] C：安全拼接字符串
来源：http://yxz.tanke756.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ulw.feifeiyinyue.top

[S18] C：命令行参数
来源：http://zqu.nanxinkj.top

int main(int argc, char **argv)
来源：http://hma.sufxvd.cn

[S19] C：快速排序
来源：http://tlr.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://kvg.hysaishi.cn

[S20] C：二分查找
来源：http://jgu.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pcu.vehdjk.com

[S21] C：字符类别判断
来源：http://iqq.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yuz.yj20258888.top

[S22] C：字符串转数字
来源：http://waw.smart0.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://gyz.fengsongda.top

[S23] C：随机数
来源：http://wyg.guowangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zmk.havefunace.top

[S24] C：获取本地时间
来源：http://axn.yj202588.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gka.nanxinkj.top

[S25] C：内存拷贝
来源：http://bae.zdqjudy.top

memcpy(dst, src, n);
来源：http://qxs.hnqzz.top

[S26] C：内存清零
来源：http://zia.fehbvm.com

memset(a, 0, sizeof a);
来源：http://erz.9152youxi.cn

[S27] C：定义常量
来源：http://yyo.yuanzhike.top

const double PI = 3.14159;
来源：http://egz.shangyingyoupin.top

[S28] C：静态变量
来源：http://vdm.zhengqikj.top

static int counter = 0;
来源：http://ctw.meibo888.top

[S29] C：变参函数
来源：http://cof.guannengcc.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nrz.cashguo.top

[S30] C：头文件保护
来源：http://ksb.yj202588.top

#ifndef X_H
来源：http://wrw.shangyingyoupin.top

#define X_H
来源：http://yvw.tanke756.top

#endif
来源：http://dby.gotoacloud.top

[S31] C++：Hello World
来源：http://xtg.zhijiandao.cn

#include <iostream>
来源：http://uma.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://kqx.chenjidiqi.icu

[S32] C++：字符串
来源：http://hpa.hammf.cn

std::string s = "hi";  s += "!";
来源：http://gpq.sysykeji.top

[S33] C++：vector 增删
来源：http://yeh.fzhhl.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fhq.hywenlv.cn

[S34] C++：遍历 vector
来源：http://gkg.sweek.top

for (auto &x : v) { std::cout << x; }
来源：http://qtc.xziqi.cn

[S35] C++：map
来源：http://jel.cashguo.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gsa.daria6918.cn

[S36] C++：unordered_map
来源：http://kpq.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lit.dianchejie.cn

[S37] C++：set
来源：http://ulm.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ucb.bjfxy.top

[S38] C++：排序
来源：http://uvr.tarul.cn

std::sort(v.begin(), v.end());
来源：http://hst.xinyue.icu

[S39] C++：自定义比较器排序
来源：http://vrj.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rhi.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://xol.yuxming.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nxm.ywan-chungtsiang.top

[S41] C++：类与构造函数
来源：http://ncu.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ran.9152youxi.cn

[S42] C++：继承与虚函数
来源：http://tvh.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://rki.wangshuangyany.cn

[S43] C++：智能指针
来源：http://koo.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://ded.jqgfzy.top

[S44] C++：引用传参
来源：http://dim.vehdjk.com

void inc(int &x) { ++x; }
来源：http://dyj.andypj.xyz

[S45] C++：lambda
来源：http://vco.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gch.cheryme.top

[S46] C++：函数模板
来源：http://xbw.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xxj.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://eua.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mmi.dashuyun.cn

[S48] C++：逐行读文件
来源：http://nlb.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://dxm.yj20258.top

while (std::getline(in, line)) { }
来源：http://arx.cdnleiting.top

[S49] C++：写文件
来源：http://dcl.chenjidiqi.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wpk.birdmap.top

[S50] C++：格式化数字
来源：http://svh.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://shn.tianlin.xyz

[S51] C++：显式类型转换
来源：http://jlm.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://mlq.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://imo.wangdashe.top

int size() const noexcept { return n_; }
来源：http://rdf.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://izj.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://nlk.nanxinkj.top

[S54] C++：异常处理
来源：http://oan.uphjek.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mgn.zhixingplan.top

[S55] C++：结构化绑定
来源：http://dtm.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xhl.tarul.cn

[S56] C++：optional
来源：http://xug.yanxiufei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tss.ppjwa.cn

[S57] C++：编译期常量
来源：http://prn.sweek.top

constexpr int N = 10;
来源：http://bxw.0kj1m.cn

[S58] C++：命名空间
来源：http://yvz.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://iyd.shangyingyoupin.top

[S59] C++：静态断言
来源：http://rbt.havefunace.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oey.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://gwq.yj20258888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eju.zhiwuduotai.top

================================================================================
来源：http://hwz.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lfz.tian-w.cn

================================================================================
来源：http://iuw.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://enf.shuidangran.top

println("Hello")
来源：http://hgx.hnxiangtu.top

[T02] Kotlin：变量
来源：http://sjc.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fta.fengsongda.top

[T03] Kotlin：字符串模板
来源：http://hjn.zycfv.cn

"值: $b"
来源：http://azk.sufxvd.cn

[T04] Kotlin：空安全
来源：http://yfh.epnwcf.com

val n: String? = null;  n?.length
来源：http://fum.shuidangran.top

[T05] Kotlin：when 表达式
来源：http://epj.tian-w.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dib.xylfe.cn

[T06] Kotlin：集合映射
来源：http://bnn.yj20258.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cbh.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://plb.ctjpmb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://jrf.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://vvl.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://wqy.dianchejie.cn

[T09] Kotlin：扩展函数
来源：http://jpp.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://ulm.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://sab.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://dpp.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://tgj.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://awi.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://dpt.fktsv.cn

val (a, b) = Pair(1, 2)
来源：http://wgh.hysaishi.cn

[T13] Kotlin：只读 Map
来源：http://tct.havefunace.top

val m = mapOf("a" to 1)
来源：http://jnq.zhijiandao.cn

[T14] Kotlin：循环
来源：http://bus.meibo888.top

for (i in 1..10) println(i)
来源：http://ayd.ctjpmb.com

[T15] Kotlin：接口
来源：http://cbg.kuanghao11.cn

interface Shape { fun area(): Double }
来源：http://ygu.zhijiandao.cn

[T16] Swift：Hello World
来源：http://ikn.mhx1999.top

print("Hello")
来源：http://yqd.fengsongda.top

[T17] Swift：变量与常量
来源：http://pqe.zhijiandao.cn

var a = 1;  let b = 2
来源：http://iyy.zdqjudy.top

[T18] Swift：字符串插值
来源：http://mdb.shzxlz.cn

"值: \(b)"
来源：http://eeh.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://ahl.yongpay.top

if let n = opt { print(n) }
来源：http://okx.nanxuanxn.top

[T20] Swift：数组操作
来源：http://csh.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vkw.xuanzx.com

[T21] Swift：遍历
来源：http://ian.vehdjk.com

for x in a { print(x) }
来源：http://xfg.svipenyu.cn

[T22] Swift：字典
来源：http://ysq.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ooh.xziqi.cn

[T23] Swift：函数
来源：http://xge.shanyushiyangtech.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qql.guowangkeji.top

[T24] Swift：闭包
来源：http://wfp.yj20258.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hdw.hammf.cn

[T25] Swift：结构体
来源：http://dgv.aizwys.cn

struct P { var x: Int }
来源：http://uhs.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://bik.hcnkem.com

class A: Base { override func f() {} }
来源：http://rbj.bjfxy.top


<!-- 参考信息 -->