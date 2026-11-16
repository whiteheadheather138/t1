代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://cdt.ywan-chungtsiang.top

[R26] 命令替换
来源：http://nga.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://nxg.daxiang520.top

[R27] 算术展开
来源：http://jlz.smart0.xyz

echo $((1 + 2 * 3))
来源：http://ent.epnwcf.com

[R28] 浮点运算
来源：http://nzp.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://mpf.guannengcc.top

[R29] 定义函数
来源：http://pcz.vehdjk.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fah.cdnleiting.top

[R30] 函数返回状态码
来源：http://kxx.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://jeg.feifeiyinyue.top

[R31] 局部变量
来源：http://slu.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://wpv.shzxlz.cn

[R32] 参数个数校验
来源：http://vxi.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aqi.jinghuilouyu.cn

[R33] 捕获错误并提示行号
来源：http://oev.nanxinkj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jah.zhongyouzk.top

[R34] 退出时清理
来源：http://tgo.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://ozv.0kj1m.cn

[R35] 后台执行并等待
来源：http://jzv.tanke756.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xsl.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://ksb.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xkc.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://gux.kuanghao11.cn

files=$(ls -1)
来源：http://wlp.cdnleiting.top

[R38] 管道串联
来源：http://edu.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://yks.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://mma.316326.xyz

cmd > out.log 2>&1
来源：http://cqx.shanyushiyangtech.top

[R40] 追加写日志
来源：http://xdq.jinqigufen.top

echo "log" >> out.log
来源：http://imm.jqgfzy.top

[R41] 丢弃输出
来源：http://sag.dashuyun.cn

cmd >/dev/null 2>&1
来源：http://fhm.dianchejie.cn

[R42] 输入重定向
来源：http://xel.jqgfzy.top

wc -l < a.txt
来源：http://ahr.ppjwa.cn

[R43] 按名字查找文件
来源：http://keb.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://vfv.daxiang520.top

[R44] 按修改时间查找
来源：http://cbl.sufxvd.cn

find . -mtime -7 -type f
来源：http://oip.316326.xyz

[R45] 批量删除
来源：http://evg.xingfuxueyuan.xyz

find . -name "*.tmp" -delete
来源：http://ogk.birdmap.top

[R46] 递归替换文件内容
来源：http://lhs.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pgn.gzhubu.top

[R47] sed 单行替换
来源：http://hiv.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tqo.jianghu66.top

[R48] awk 取指定列
来源：http://pzv.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://xtb.316326.xyz

[R49] awk 带条件
来源：http://pzl.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pem.uphjek.com

[R50] awk 求和
来源：http://jrr.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sxc.c1oappe.top

[R51] 排序去重取前几
来源：http://khi.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://mut.nanxinkj.top

[R52] 统计行数
来源：http://xqf.fanxiaobao.xyz

wc -l a.txt
来源：http://afp.hnqzz.top

[R53] 查看文件头与实时尾
来源：http://ccu.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qyc.gzhubu.top

[R54] 比较两个文件
来源：http://drr.hnxiangtu.top

diff a.txt b.txt
来源：http://lkh.316326.xyz

[R55] 压缩与解压
来源：http://ctf.daxiang520.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://izb.sysykeji.top

[R56] 远程拷贝
来源：http://lvm.bjfxy.top

scp file user@host:/path/
来源：http://som.zhengqikj.top

[R57] 远程执行命令
来源：http://mmg.yj20258888.top

ssh user@host 'uptime'
来源：http://rzw.xinyue.icu

[R58] 下载文件
来源：http://zia.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://esq.ybcxt.top

[R59] 发 POST JSON
来源：http://xwb.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pcn.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://kec.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yzy.sweek.top

[R61] 磁盘占用
来源：http://saw.dianchejie.cn

df -h;  du -sh *
来源：http://xos.ctjpmb.com

[R62] 找最占空间的文件
来源：http://tbs.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://kbq.quarkkingdee.top

[R63] 内存与进程
来源：http://jou.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://erz.zhaomingkeji.xyz

[R64] 结束进程
来源：http://rvs.zhoulong.xyz

kill -9 $(pgrep -f app.py)
来源：http://dbx.9152youxi.cn

[R65] 查看端口占用
来源：http://bue.zhongyouzk.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hxt.zhijiandao.cn

[R66] 定时任务
来源：http://uwu.yj20258.top

crontab -e;  crontab -l
来源：http://vie.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://fwt.fengsongda.top

openssl rand -hex 16
来源：http://atx.snrcjt.cn

[R68] 计算文件校验值
来源：http://nyg.chenzaomai.com

sha256sum a.txt;  md5sum a.txt
来源：http://kzi.ydjk.org.cn

[R69] 生成随机密码
来源：http://ati.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://raz.sjlbkw.cn

[R70] 时间戳与互转
来源：http://osq.andypj.xyz

date +%s;  date -d @1700000000
来源：http://qdh.wangshuangyany.cn

[R71] 日期格式化
来源：http://twz.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://cdb.mhx1999.top

[R72] 等待端口就绪
来源：http://ypt.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://snf.sxryk.cn

[R73] 分割大日志
来源：http://xjr.shangyingyoupin.top

split -l 1000 big.log part_
来源：http://eyr.yonumen.top

[R74] 批量重命名
来源：http://gcn.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rjr.meibo888.top

[R75] 导出环境变量
来源：http://chu.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://zbn.shangyingyoupin.top

[R76] 使用临时文件
来源：http://zrk.aizwys.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fap.yfazqb.com

[R77] 读取用户输入
来源：http://psb.ydjk.org.cn

read -rp "请输入: " ans
来源：http://obj.jqgfzy.top

[R78] 交互式菜单
来源：http://qro.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://aqt.yfazqb.com

[R79] 解析命令行选项
来源：http://ryt.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gtu.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://nlh.yuanzhike.top

time ./run.sh
来源：http://sgc.gogol.net.cn

================================================================================
来源：http://qim.gotoacloud.top

S. C / C++ 专题
来源：http://uwk.chenlongwang.top

================================================================================
来源：http://vgb.jlsjyb.cn

[S01] C：Hello World
来源：http://fgj.zhijiandao.cn

#include <stdio.h>
来源：http://yvg.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://adm.jianghu66.top

[S02] C：变量与格式化输出
来源：http://ayi.gotoacloud.top

int a = 10; printf("%d\n", a);
来源：http://ead.zhongyouzk.top

[S03] C：读入整数
来源：http://eev.sweek.top

int x; scanf("%d", &x);
来源：http://ivb.zycfv.cn

[S04] C：字符串复制
来源：http://kfx.zhaomingkeji.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://hpl.vehdjk.com

[S05] C：字符串长度
来源：http://tyi.nwbrower.top

strlen(s)
来源：http://cgx.cucudq.cn

[S06] C：字符串比较
来源：http://lij.zhixingplan.top

strcmp(a, b) == 0
来源：http://mat.hesvh.cn

[S07] C：数组遍历求和
来源：http://ghq.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bba.haohaochexian.top

[S08] C：动态内存分配与释放
来源：http://ibi.0kj1m.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hfm.meibo888.top

[S09] C：结构体定义与初始化
来源：http://kvk.gaohongyu789.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tna.jianghu66.top

[S10] C：指针与解引用
来源：http://njy.316326.xyz

int *p = &a;  *p = 5;
来源：http://cke.fzhhl.top

[S11] C：逐行读文件
来源：http://vpj.aibaodan.cn

FILE *f = fopen("a.txt", "r");
来源：http://dtl.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://tar.vehdjk.com

fclose(f);
来源：http://azt.cashguo.top

[S12] C：写文件
来源：http://nve.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tvv.gzhubu.top

[S13] C：宏定义
来源：http://mdh.xylfe.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mkc.bbcook.cn

[S14] C：枚举
来源：http://wqd.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://uql.zhijiandao.cn

[S15] C：类型转换
来源：http://dia.tarul.cn

(double) a / b
来源：http://wqn.yonumen.top

[S16] C：位操作置位
来源：http://xkl.epnwcf.com

x |= (1 << 3);
来源：http://lgn.jianghu66.top

[S17] C：安全拼接字符串
来源：http://nxi.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://grf.hnxiangtu.top

[S18] C：命令行参数
来源：http://cks.iojbl.cn

int main(int argc, char **argv)
来源：http://ovm.shuidangran.top

[S19] C：快速排序
来源：http://wkk.sjlbkw.cn

qsort(a, n, sizeof(int), cmp);
来源：http://usa.jinghuilouyu.cn

[S20] C：二分查找
来源：http://tqv.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xoj.cucudq.cn

[S21] C：字符类别判断
来源：http://pae.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nwz.redwolf501.top

[S22] C：字符串转数字
来源：http://uzp.9152youxi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://utb.xinyue.icu

[S23] C：随机数
来源：http://rup.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jke.yj20258888.top

[S24] C：获取本地时间
来源：http://ywm.cdnleiting.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://chb.nanxinkj.top

[S25] C：内存拷贝
来源：http://fvi.zhongyouzk.top

memcpy(dst, src, n);
来源：http://sof.haohaochexian.top

[S26] C：内存清零
来源：http://zes.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://svb.xylfe.cn

[S27] C：定义常量
来源：http://yaw.jlsjyb.cn

const double PI = 3.14159;
来源：http://fhj.yfazqb.com

[S28] C：静态变量
来源：http://stq.snrcjt.cn

static int counter = 0;
来源：http://tqr.tian-w.cn

[S29] C：变参函数
来源：http://def.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ode.shuidangran.top

[S30] C：头文件保护
来源：http://ryj.haohaochexian.top

#ifndef X_H
来源：http://vjs.shzxlz.cn

#define X_H
来源：http://prw.jinghuilouyu.cn

#endif
来源：http://avj.aibaodan.cn

[S31] C++：Hello World
来源：http://htq.quarkkingdee.top

#include <iostream>
来源：http://wbo.redwolf501.top

int main() { std::cout << "Hello\n"; }
来源：http://qov.daxiang520.top

[S32] C++：字符串
来源：http://rrg.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://wcl.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://wfs.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ell.jqgfzy.top

[S34] C++：遍历 vector
来源：http://nhy.zdqjudy.top

for (auto &x : v) { std::cout << x; }
来源：http://lpw.quarkkingdee.top

[S35] C++：map
来源：http://utb.shanyushiyangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://luf.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://pdw.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://otw.wangdashe.top

[S37] C++：set
来源：http://nqg.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xcy.xinyue.icu

[S38] C++：排序
来源：http://ylh.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://evs.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://vef.0kj1m.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fpb.fanxiaobao.xyz

[S40] C++：查找元素
来源：http://efh.jinyuanbaomall.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qpy.fengsongda.top

[S41] C++：类与构造函数
来源：http://huk.zhijiandao.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://avj.fehbvm.com

[S42] C++：继承与虚函数
来源：http://yko.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://jiy.uphjek.com

[S43] C++：智能指针
来源：http://xpc.shzxlz.cn

auto p = std::make_unique<int>(5);
来源：http://njf.zhongyouzk.top

[S44] C++：引用传参
来源：http://fgf.svipenyu.cn

void inc(int &x) { ++x; }
来源：http://gqq.316326.xyz

[S45] C++：lambda
来源：http://btc.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://jlg.andypj.xyz

[S46] C++：函数模板
来源：http://xho.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pyt.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://pgh.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cek.redwolf501.top

[S48] C++：逐行读文件
来源：http://rlc.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://nsf.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://ijf.jianghu66.top

[S49] C++：写文件
来源：http://prk.feifeiyinyue.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rza.fzhhl.top

[S50] C++：格式化数字
来源：http://yzo.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rtz.fanxiaobao.xyz

[S51] C++：显式类型转换
来源：http://blo.snrcjt.cn

static_cast<double>(a) / b
来源：http://rjd.kuanghao11.cn

[S52] C++：const 与 noexcept
来源：http://gdp.ybcxt.top

int size() const noexcept { return n_; }
来源：http://eyb.cheryme.top

[S53] C++：移动语义
来源：http://uuj.ydjk.org.cn

std::vector<int> w = std::move(v);
来源：http://zlc.52xcode.cn

[S54] C++：异常处理
来源：http://bou.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rbc.9152youxi.cn

[S55] C++：结构化绑定
来源：http://suo.sysykeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jla.ywan-chungtsiang.top

[S56] C++：optional
来源：http://zon.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iii.jyoumei.cn

[S57] C++：编译期常量
来源：http://nsb.hnxiangtu.top

constexpr int N = 10;
来源：http://tvf.vqdsnc.cn

[S58] C++：命名空间
来源：http://yof.zdbjq.cn

namespace ns { int f() { return 1; } }
来源：http://iac.yvedp.cn

[S59] C++：静态断言
来源：http://yxy.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pwl.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://fig.xylfe.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fdg.iojbl.cn

================================================================================
来源：http://lgb.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kur.0kj1m.cn

================================================================================
来源：http://hxa.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://rdp.jyoumei.cn

println("Hello")
来源：http://hur.c1oappe.top

[T02] Kotlin：变量
来源：http://lbm.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fmj.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://zla.daria6918.cn

"值: $b"
来源：http://faw.sxryk.cn

[T04] Kotlin：空安全
来源：http://xym.xziqi.cn

val n: String? = null;  n?.length
来源：http://wbj.hywenlv.cn

[T05] Kotlin：when 表达式
来源：http://daf.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qsi.cucudq.cn

[T06] Kotlin：集合映射
来源：http://fsb.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bfp.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://iew.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yax.cqqwz.cn

[T08] Kotlin：数据类
来源：http://mrx.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://dtj.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://qrd.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://onx.bjfxy.top

[T10] Kotlin：默认参数
来源：http://nao.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qnv.jqgfzy.top

[T11] Kotlin：协程
来源：http://eze.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jnd.fktsv.cn

[T12] Kotlin：解构声明
来源：http://uqa.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://jst.316326.xyz

[T13] Kotlin：只读 Map
来源：http://stj.cashguo.top

val m = mapOf("a" to 1)
来源：http://iyq.fktsv.cn

[T14] Kotlin：循环
来源：http://mvo.dianchejie.cn

for (i in 1..10) println(i)
来源：http://ehx.quarkkingdee.top

[T15] Kotlin：接口
来源：http://gup.nanxinkj.top

interface Shape { fun area(): Double }
来源：http://nao.feifeiyinyue.top

[T16] Swift：Hello World
来源：http://lqy.zhiwuduotai.top

print("Hello")
来源：http://qhn.cqqwz.cn

[T17] Swift：变量与常量
来源：http://qyr.yj202588.top

var a = 1;  let b = 2
来源：http://ktw.0kj1m.cn

[T18] Swift：字符串插值
来源：http://sla.ybcxt.top

"值: \(b)"
来源：http://jyy.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://akx.gotoacloud.top

if let n = opt { print(n) }
来源：http://xrm.yj20258888.top

[T20] Swift：数组操作
来源：http://iey.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uif.sjlbkw.cn

[T21] Swift：遍历
来源：http://lqd.yj20258.top

for x in a { print(x) }
来源：http://hcu.yanxiufei.cn

[T22] Swift：字典
来源：http://zpg.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ruq.hongshengwenyu.top

[T23] Swift：函数
来源：http://kla.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rmk.nanxuanxn.top

[T24] Swift：闭包
来源：http://atu.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mxz.andypj.xyz

[T25] Swift：结构体
来源：http://jdl.jinqigfzy.top

struct P { var x: Int }
来源：http://qfu.sjlbkw.cn

[T26] Swift：类与重写
来源：http://vlb.chenlongwang.top

class A: Base { override func f() {} }
来源：http://dwa.yueranfly.top

[T27] Swift：错误处理
来源：http://sou.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://zyh.yj20258.top

[T28] Swift：枚举
来源：http://wce.ywan-chungtsiang.top

enum Color { case red, green }
来源：http://fid.redwolf501.top


<!-- 参考信息 -->