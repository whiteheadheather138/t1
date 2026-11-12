代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://ugh.yuxming.cn

[R26] 命令替换
来源：http://gbw.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://jmv.bbcook.cn

[R27] 算术展开
来源：http://znx.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://tmv.ppjwa.cn

[R28] 浮点运算
来源：http://rvj.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://wso.jinyuanbaomall.cn

[R29] 定义函数
来源：http://jgy.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://shd.zdbjq.cn

[R30] 函数返回状态码
来源：http://xvx.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://sfq.ehwqpu.com

[R31] 局部变量
来源：http://roo.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://lqz.bjfxy.top

[R32] 参数个数校验
来源：http://qwb.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zso.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://aus.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ojb.sysykeji.top

[R34] 退出时清理
来源：http://jdx.xziqi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jjs.bbcook.cn

[R35] 后台执行并等待
来源：http://tue.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jlw.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://npc.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qqp.yj202588.top

[R37] 把输出赋给变量
来源：http://mqr.yueranfly.top

files=$(ls -1)
来源：http://gpp.hnxiangtu.top

[R38] 管道串联
来源：http://boa.aibaodan.cn

cat a.txt | grep -i error | wc -l
来源：http://thd.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://zxc.jqgfzy.top

cmd > out.log 2>&1
来源：http://wsk.jinghuilouyu.cn

[R40] 追加写日志
来源：http://sqe.yj202588.top

echo "log" >> out.log
来源：http://xpy.bbcook.cn

[R41] 丢弃输出
来源：http://kco.cqqwz.cn

cmd >/dev/null 2>&1
来源：http://jzu.xuanzx.com

[R42] 输入重定向
来源：http://wrj.ywan-chungtsiang.top

wc -l < a.txt
来源：http://bjq.zhoulong.xyz

[R43] 按名字查找文件
来源：http://smw.haohaochexian.top

find . -name "*.log" -type f
来源：http://uxz.gaohongyu789.top

[R44] 按修改时间查找
来源：http://eek.snrcjt.cn

find . -mtime -7 -type f
来源：http://nvz.jqgfzy.top

[R45] 批量删除
来源：http://hqz.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://bcg.birdmap.top

[R46] 递归替换文件内容
来源：http://rvb.zdbjq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lue.meibo888.top

[R47] sed 单行替换
来源：http://pzu.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xnv.pycfn.com

[R48] awk 取指定列
来源：http://sgi.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://mjn.zycfv.cn

[R49] awk 带条件
来源：http://gxx.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ujt.tianlin.xyz

[R50] awk 求和
来源：http://mnh.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://jbs.jinqigufen.top

[R51] 排序去重取前几
来源：http://dup.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zdj.52xcode.cn

[R52] 统计行数
来源：http://wqm.shzxlz.cn

wc -l a.txt
来源：http://gme.c1oappe.top

[R53] 查看文件头与实时尾
来源：http://ykb.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qfa.yongpay.top

[R54] 比较两个文件
来源：http://jhd.jinqigfzy.top

diff a.txt b.txt
来源：http://jmr.cashguo.top

[R55] 压缩与解压
来源：http://qzu.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fnz.jinqigfzy.top

[R56] 远程拷贝
来源：http://tyd.gaohongyu789.top

scp file user@host:/path/
来源：http://lpb.gzhubu.top

[R57] 远程执行命令
来源：http://wqn.sufxvd.cn

ssh user@host 'uptime'
来源：http://jdn.fehbvm.com

[R58] 下载文件
来源：http://jjr.uphjek.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fhr.havefunace.top

[R59] 发 POST JSON
来源：http://ahe.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yzv.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://dgb.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://syz.jyoumei.cn

[R61] 磁盘占用
来源：http://puc.cqqwz.cn

df -h;  du -sh *
来源：http://qqy.yuxming.cn

[R62] 找最占空间的文件
来源：http://yjn.cqqwz.cn

du -ah . | sort -rh | head -10
来源：http://hzn.gaohongyu789.top

[R63] 内存与进程
来源：http://xlz.yuxming.cn

free -h;  ps aux | grep nginx
来源：http://hnx.vqdsnc.cn

[R64] 结束进程
来源：http://iti.havefunace.top

kill -9 $(pgrep -f app.py)
来源：http://krm.zhijiandao.cn

[R65] 查看端口占用
来源：http://rql.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rzj.pengpengdd.cyou

[R66] 定时任务
来源：http://pru.yj202588.top

crontab -e;  crontab -l
来源：http://gdl.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://pvc.0kj1m.cn

openssl rand -hex 16
来源：http://gce.mhx1999.top

[R68] 计算文件校验值
来源：http://pxq.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://ebq.zhongyouzk.top

[R69] 生成随机密码
来源：http://aft.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://twf.0kj1m.cn

[R70] 时间戳与互转
来源：http://emq.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://qdm.jlsjyb.cn

[R71] 日期格式化
来源：http://lpo.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wzh.hesvh.cn

[R72] 等待端口就绪
来源：http://fub.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://khs.yj20258888.top

[R73] 分割大日志
来源：http://gcr.redwolf501.top

split -l 1000 big.log part_
来源：http://gfa.birdmap.top

[R74] 批量重命名
来源：http://ltm.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ulo.zhiwuduotai.top

[R75] 导出环境变量
来源：http://efe.nwbrower.top

export PATH="$HOME/bin:$PATH"
来源：http://hkt.zhijiandao.cn

[R76] 使用临时文件
来源：http://eho.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eiw.zhoulong.xyz

[R77] 读取用户输入
来源：http://tnt.hammf.cn

read -rp "请输入: " ans
来源：http://hfz.xylfe.cn

[R78] 交互式菜单
来源：http://xfx.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tir.tarul.cn

[R79] 解析命令行选项
来源：http://zcd.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dsm.quarkkingdee.top

[R80] 查看脚本执行耗时
来源：http://mlb.hnqzz.top

time ./run.sh
来源：http://dce.52xcode.cn

================================================================================
来源：http://fze.jianghu66.top

S. C / C++ 专题
来源：http://enu.zhoulong.xyz

================================================================================
来源：http://rln.fktsv.cn

[S01] C：Hello World
来源：http://zqw.zhaomingkeji.xyz

#include <stdio.h>
来源：http://xnp.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nzx.chenzaomai.com

[S02] C：变量与格式化输出
来源：http://xvm.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://vbr.jinqigfzy.top

[S03] C：读入整数
来源：http://geb.jyoumei.cn

int x; scanf("%d", &x);
来源：http://wht.ppjwa.cn

[S04] C：字符串复制
来源：http://ffr.hfpthk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vvl.nanxuanxn.top

[S05] C：字符串长度
来源：http://ssc.sxryk.cn

strlen(s)
来源：http://efx.shangyingyoupin.top

[S06] C：字符串比较
来源：http://jcm.hnqzz.top

strcmp(a, b) == 0
来源：http://xkn.hfpthk.cn

[S07] C：数组遍历求和
来源：http://ltc.havefunace.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wkx.haohaochexian.top

[S08] C：动态内存分配与释放
来源：http://uui.zycfv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ktf.yuxming.cn

[S09] C：结构体定义与初始化
来源：http://dkz.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gtr.yanxiufei.cn

[S10] C：指针与解引用
来源：http://imd.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://qkf.ydzc1.top

[S11] C：逐行读文件
来源：http://hvh.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://nwp.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ksg.gaohongyu789.top

fclose(f);
来源：http://kwm.cqqwz.cn

[S12] C：写文件
来源：http://edc.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wyo.zhixingplan.top

[S13] C：宏定义
来源：http://czr.ywan-chungtsiang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zog.epnwcf.com

[S14] C：枚举
来源：http://djy.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://eny.zycfv.cn

[S15] C：类型转换
来源：http://eda.pycfn.com

(double) a / b
来源：http://swv.jlsjyb.cn

[S16] C：位操作置位
来源：http://hrn.jinqigufen.top

x |= (1 << 3);
来源：http://xaw.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://ojw.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jbp.aizwys.cn

[S18] C：命令行参数
来源：http://dnx.zhongyouzk.top

int main(int argc, char **argv)
来源：http://kdp.jinqigufen.top

[S19] C：快速排序
来源：http://dvz.hongshengwenyu.top

qsort(a, n, sizeof(int), cmp);
来源：http://crp.guowangkeji.top

[S20] C：二分查找
来源：http://gwo.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ovt.yangfankeji.com

[S21] C：字符类别判断
来源：http://ixr.c1oappe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mta.pycfn.com

[S22] C：字符串转数字
来源：http://jdh.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://hje.cdnleiting.top

[S23] C：随机数
来源：http://vvh.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xak.cashguo.top

[S24] C：获取本地时间
来源：http://wdy.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vyx.gzhubu.top

[S25] C：内存拷贝
来源：http://ewm.jqgfzy.top

memcpy(dst, src, n);
来源：http://wgk.tianlin.xyz

[S26] C：内存清零
来源：http://bex.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://sxf.smart0.xyz

[S27] C：定义常量
来源：http://zke.chenjidiqi.icu

const double PI = 3.14159;
来源：http://dcn.tianlin.xyz

[S28] C：静态变量
来源：http://uql.yuxming.cn

static int counter = 0;
来源：http://ddn.guowangkeji.top

[S29] C：变参函数
来源：http://nde.ehwqpu.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dnd.zhoulong.xyz

[S30] C：头文件保护
来源：http://ksv.sweek.top

#ifndef X_H
来源：http://fcr.wangshuangyany.cn

#define X_H
来源：http://ige.chenzaomai.com

#endif
来源：http://fax.ppjwa.cn

[S31] C++：Hello World
来源：http://oal.smart0.xyz

#include <iostream>
来源：http://nyw.jyoumei.cn

int main() { std::cout << "Hello\n"; }
来源：http://bzg.yonumen.top

[S32] C++：字符串
来源：http://ufb.zhaomingkeji.xyz

std::string s = "hi";  s += "!";
来源：http://byf.meibo888.top

[S33] C++：vector 增删
来源：http://ray.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://spa.nwbrower.top

[S34] C++：遍历 vector
来源：http://lij.fanxiaobao.xyz

for (auto &x : v) { std::cout << x; }
来源：http://iiu.ydzc1.top

[S35] C++：map
来源：http://jij.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jdc.dashuyun.cn

[S36] C++：unordered_map
来源：http://oqx.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fny.xziqi.cn

[S37] C++：set
来源：http://suk.zhixingplan.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://heu.jqgfzy.top

[S38] C++：排序
来源：http://vse.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://ndo.hysaishi.cn

[S39] C++：自定义比较器排序
来源：http://lwx.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nfe.epnwcf.com

[S40] C++：查找元素
来源：http://tvu.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sly.yj202588.top

[S41] C++：类与构造函数
来源：http://xdw.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pqg.zhixingplan.top

[S42] C++：继承与虚函数
来源：http://ywr.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://biu.andypj.xyz

[S43] C++：智能指针
来源：http://inl.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://iof.guowangkeji.top

[S44] C++：引用传参
来源：http://flx.daria6918.cn

void inc(int &x) { ++x; }
来源：http://sia.tianlin.xyz

[S45] C++：lambda
来源：http://yhn.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jsa.yonumen.top

[S46] C++：函数模板
来源：http://fby.jinqigufen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wxj.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://erz.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eoq.yonumen.top

[S48] C++：逐行读文件
来源：http://tsb.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://qrr.aizwys.cn

while (std::getline(in, line)) { }
来源：http://qfp.jinghuilouyu.cn

[S49] C++：写文件
来源：http://gcm.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hkc.zhongyouzk.top

[S50] C++：格式化数字
来源：http://pej.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rag.yfazqb.com

[S51] C++：显式类型转换
来源：http://tks.pycfn.com

static_cast<double>(a) / b
来源：http://lhc.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://cuv.c1oappe.top

int size() const noexcept { return n_; }
来源：http://nvv.hnqzz.top

[S53] C++：移动语义
来源：http://nbh.yj202588.top

std::vector<int> w = std::move(v);
来源：http://mln.dianchejie.cn

[S54] C++：异常处理
来源：http://uik.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://knh.pycfn.com

[S55] C++：结构化绑定
来源：http://eqs.sweek.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qbl.yvedp.cn

[S56] C++：optional
来源：http://prb.tian-w.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vhc.shuidangran.top

[S57] C++：编译期常量
来源：http://mqq.fengsongda.top

constexpr int N = 10;
来源：http://ywj.chenlongwang.top

[S58] C++：命名空间
来源：http://hzp.xziqi.cn

namespace ns { int f() { return 1; } }
来源：http://mlw.pengpengdd.cyou

[S59] C++：静态断言
来源：http://pwy.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mwb.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://zlf.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xxo.yuxming.cn

================================================================================
来源：http://mlq.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://czz.hnxiangtu.top

================================================================================
来源：http://efz.yj20258888.top

[T01] Kotlin：Hello World
来源：http://cxh.daria6918.cn

println("Hello")
来源：http://dpp.hnqzz.top

[T02] Kotlin：变量
来源：http://wrr.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ytv.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://ope.gzhubu.top

"值: $b"
来源：http://qea.svipenyu.cn

[T04] Kotlin：空安全
来源：http://xfp.gzhubu.top

val n: String? = null;  n?.length
来源：http://xya.pycfn.com

[T05] Kotlin：when 表达式
来源：http://yxq.zdqjudy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qdr.tarul.cn

[T06] Kotlin：集合映射
来源：http://kzf.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://fje.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://wsk.xingfuxueyuan.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://jpf.jinqigufen.top

[T08] Kotlin：数据类
来源：http://iow.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://hdf.nwbrower.top

[T09] Kotlin：扩展函数
来源：http://rnf.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://ugl.nwbrower.top

[T10] Kotlin：默认参数
来源：http://kxf.cdnleiting.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uiu.ydjk.org.cn

[T11] Kotlin：协程
来源：http://pdk.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://zry.tanke756.top

[T12] Kotlin：解构声明
来源：http://sfj.bbcook.cn

val (a, b) = Pair(1, 2)
来源：http://gko.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://frp.fktsv.cn

val m = mapOf("a" to 1)
来源：http://sal.gogol.net.cn

[T14] Kotlin：循环
来源：http://ozp.xuanzx.com

for (i in 1..10) println(i)
来源：http://hti.andypj.xyz

[T15] Kotlin：接口
来源：http://hbq.jiagoushi.top

interface Shape { fun area(): Double }
来源：http://ppk.ivvv.top

[T16] Swift：Hello World
来源：http://fxm.haohaochexian.top

print("Hello")
来源：http://dkm.jiagoushi.top

[T17] Swift：变量与常量
来源：http://uqi.jinqigfzy.top

var a = 1;  let b = 2
来源：http://mrn.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://jot.sxryk.cn

"值: \(b)"
来源：http://djb.yj202588.top

[T19] Swift：可选绑定
来源：http://vzc.yj202588.top

if let n = opt { print(n) }
来源：http://ddm.yanxiufei.cn

[T20] Swift：数组操作
来源：http://kcr.kuanghao11.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mkf.aizwys.cn

[T21] Swift：遍历
来源：http://lsx.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://lgy.hongshengwenyu.top

[T22] Swift：字典
来源：http://obz.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://woy.chenjidiqi.icu

[T23] Swift：函数
来源：http://uzg.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wgo.xuetiantiany.cn

[T24] Swift：闭包
来源：http://jkl.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://gru.xinyue.icu

[T25] Swift：结构体
来源：http://wgv.zdbjq.cn

struct P { var x: Int }
来源：http://dga.ydjk.org.cn

[T26] Swift：类与重写
来源：http://jya.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://exx.uphjek.com

[T27] Swift：错误处理
来源：http://voo.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://rrv.nwbrower.top

[T28] Swift：枚举
来源：http://snz.yuanzhike.top

enum Color { case red, green }
来源：http://cro.xingfuxueyuan.xyz


<!-- 参考信息 -->