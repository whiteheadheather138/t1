代发 wailian999

echo "${#s}"
来源：http://qxv.9152youxi.cn

[R22] 截取子串
来源：http://zgt.sxryk.cn

echo "${s:0:5}"
来源：http://hmu.birdmap.top

[R23] 字符串替换
来源：http://oet.fanxiaobao.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fhj.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://wpc.yfazqb.com

echo "${s^^}"; echo "${s,,}"
来源：http://xuu.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://vbo.pycfn.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://fcg.zhixingplan.top

[R26] 命令替换
来源：http://fui.jlsjyb.cn

now=$(date +%F); echo "$now"
来源：http://wqz.svipenyu.cn

[R27] 算术展开
来源：http://xsb.yfazqb.com

echo $((1 + 2 * 3))
来源：http://oop.hesvh.cn

[R28] 浮点运算
来源：http://lxw.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://grn.zdqjudy.top

[R29] 定义函数
来源：http://uax.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gov.chenzaomai.com

[R30] 函数返回状态码
来源：http://uvs.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://nwe.yueranfly.top

[R31] 局部变量
来源：http://zwk.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://oef.jqgfzy.top

[R32] 参数个数校验
来源：http://rbd.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qfm.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://cqr.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://soo.nanxuanxn.top

[R34] 退出时清理
来源：http://mpl.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://sdv.tarul.cn

[R35] 后台执行并等待
来源：http://nlh.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ufi.gzhubu.top

[R36] 并发执行多个任务
来源：http://uhj.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dcy.pengpengdd.cyou

[R37] 把输出赋给变量
来源：http://kog.zhiwuduotai.top

files=$(ls -1)
来源：http://rme.yj20258888.top

[R38] 管道串联
来源：http://ise.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://ejk.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://txg.xziqi.cn

cmd > out.log 2>&1
来源：http://xui.daria6918.cn

[R40] 追加写日志
来源：http://ohi.guowangkeji.top

echo "log" >> out.log
来源：http://aeo.xziqi.cn

[R41] 丢弃输出
来源：http://qyg.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://pmg.yonumen.top

[R42] 输入重定向
来源：http://qrg.cucudq.cn

wc -l < a.txt
来源：http://uxf.zhoulong.xyz

[R43] 按名字查找文件
来源：http://pqv.shuidangran.top

find . -name "*.log" -type f
来源：http://wem.zhiwuduotai.top

[R44] 按修改时间查找
来源：http://aez.fktsv.cn

find . -mtime -7 -type f
来源：http://szg.shuidangran.top

[R45] 批量删除
来源：http://lgx.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://ect.xuetiantiany.cn

[R46] 递归替换文件内容
来源：http://mox.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ulb.nanxinkj.top

[R47] sed 单行替换
来源：http://rtq.guowangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://hpq.daria6918.cn

[R48] awk 取指定列
来源：http://ktx.jqgufenzy.top

awk '{print $1, $3}' a.txt
来源：http://ddt.c1oappe.top

[R49] awk 带条件
来源：http://amc.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gdk.hesvh.cn

[R50] awk 求和
来源：http://zpv.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://gms.smart0.xyz

[R51] 排序去重取前几
来源：http://fkx.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://umq.birdmap.top

[R52] 统计行数
来源：http://pno.mhx1999.top

wc -l a.txt
来源：http://ryx.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://ptd.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pzl.hywenlv.cn

[R54] 比较两个文件
来源：http://xth.zhixingplan.top

diff a.txt b.txt
来源：http://jbc.cqqwz.cn

[R55] 压缩与解压
来源：http://cee.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yzu.shzxlz.cn

[R56] 远程拷贝
来源：http://zsn.aizwys.cn

scp file user@host:/path/
来源：http://aif.gzhubu.top

[R57] 远程执行命令
来源：http://pgc.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://rxj.birdmap.top

[R58] 下载文件
来源：http://ttm.shuidangran.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dyr.xziqi.cn

[R59] 发 POST JSON
来源：http://cud.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vcs.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://zzs.c1oappe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cbc.gotoacloud.top

[R61] 磁盘占用
来源：http://mma.tarul.cn

df -h;  du -sh *
来源：http://hle.havefunace.top

[R62] 找最占空间的文件
来源：http://rwj.smart0.xyz

du -ah . | sort -rh | head -10
来源：http://liq.havefunace.top

[R63] 内存与进程
来源：http://dio.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://nji.ydjk.org.cn

[R64] 结束进程
来源：http://iwg.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://zuw.pycfn.com

[R65] 查看端口占用
来源：http://krm.haohaochexian.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xmv.haohaochexian.top

[R66] 定时任务
来源：http://jfi.tianlin.xyz

crontab -e;  crontab -l
来源：http://yxu.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://gos.0kj1m.cn

openssl rand -hex 16
来源：http://gnm.xziqi.cn

[R68] 计算文件校验值
来源：http://zvw.uphjek.com

sha256sum a.txt;  md5sum a.txt
来源：http://vpb.52xcode.cn

[R69] 生成随机密码
来源：http://ejj.9152youxi.cn

head -c 16 /dev/urandom | base64
来源：http://shb.jiagoushi.top

[R70] 时间戳与互转
来源：http://rsj.zycfv.cn

date +%s;  date -d @1700000000
来源：http://vks.hysaishi.cn

[R71] 日期格式化
来源：http://nwe.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://qly.birdmap.top

[R72] 等待端口就绪
来源：http://eng.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qqc.hnqzz.top

[R73] 分割大日志
来源：http://bcz.hesvh.cn

split -l 1000 big.log part_
来源：http://pyk.xuetiantiany.cn

[R74] 批量重命名
来源：http://aef.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://shu.jinqigfzy.top

[R75] 导出环境变量
来源：http://yqq.tianlin.xyz

export PATH="$HOME/bin:$PATH"
来源：http://ylv.0kj1m.cn

[R76] 使用临时文件
来源：http://wai.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://swc.cdnleiting.top

[R77] 读取用户输入
来源：http://qhm.meibo888.top

read -rp "请输入: " ans
来源：http://bwk.daria6918.cn

[R78] 交互式菜单
来源：http://vjh.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tkr.birdmap.top

[R79] 解析命令行选项
来源：http://xwq.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gtu.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://vuz.fanxiaobao.xyz

time ./run.sh
来源：http://bit.mhx1999.top

================================================================================
来源：http://fkr.hywenlv.cn

S. C / C++ 专题
来源：http://hrq.zhaomingkeji.xyz

================================================================================
来源：http://qqh.zdqjudy.top

[S01] C：Hello World
来源：http://lfk.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://okn.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xnt.c1oappe.top

[S02] C：变量与格式化输出
来源：http://jyk.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://qks.jiagoushi.top

[S03] C：读入整数
来源：http://hvj.chenlongwang.top

int x; scanf("%d", &x);
来源：http://xyd.mhx1999.top

[S04] C：字符串复制
来源：http://krx.hnqzz.top

char dst[32]; strcpy(dst, "hi");
来源：http://vnm.jlsjyb.cn

[S05] C：字符串长度
来源：http://dit.xuanzx.com

strlen(s)
来源：http://imh.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://tok.ppjwa.cn

strcmp(a, b) == 0
来源：http://ixk.guannengcc.top

[S07] C：数组遍历求和
来源：http://wvo.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sqb.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://vph.dashuyun.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tfy.yj202588.top

[S09] C：结构体定义与初始化
来源：http://fjc.dianchejie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://imx.guannengcc.top

[S10] C：指针与解引用
来源：http://cgs.iojbl.cn

int *p = &a;  *p = 5;
来源：http://wfu.chenlongwang.top

[S11] C：逐行读文件
来源：http://ewt.yanxiufei.cn

FILE *f = fopen("a.txt", "r");
来源：http://xml.sufxvd.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://thm.fehbvm.com

fclose(f);
来源：http://oxb.xuetiantiany.cn

[S12] C：写文件
来源：http://nsm.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jmv.bjfxy.top

[S13] C：宏定义
来源：http://sgv.tian-w.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gld.fehbvm.com

[S14] C：枚举
来源：http://vvd.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://nkx.52xcode.cn

[S15] C：类型转换
来源：http://qwd.yanxiufei.cn

(double) a / b
来源：http://ndw.sweek.top

[S16] C：位操作置位
来源：http://ohe.snrcjt.cn

x |= (1 << 3);
来源：http://map.redwolf501.top

[S17] C：安全拼接字符串
来源：http://xps.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dvl.cheryme.top

[S18] C：命令行参数
来源：http://vuw.dashuyun.cn

int main(int argc, char **argv)
来源：http://exv.fanxiaobao.xyz

[S19] C：快速排序
来源：http://wbn.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://inf.shuidangran.top

[S20] C：二分查找
来源：http://vxn.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fps.yanxiufei.cn

[S21] C：字符类别判断
来源：http://kwf.uphjek.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://msg.kuanghao11.cn

[S22] C：字符串转数字
来源：http://zlq.fktsv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lqe.gotoacloud.top

[S23] C：随机数
来源：http://bry.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zan.pycfn.com

[S24] C：获取本地时间
来源：http://gvq.jiagoushi.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wra.yonumen.top

[S25] C：内存拷贝
来源：http://wxe.gogol.net.cn

memcpy(dst, src, n);
来源：http://mbj.zhongyouzk.top

[S26] C：内存清零
来源：http://cqj.svipenyu.cn

memset(a, 0, sizeof a);
来源：http://upp.redwolf501.top

[S27] C：定义常量
来源：http://lbw.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://xnr.fzhhl.top

[S28] C：静态变量
来源：http://ude.tianlin.xyz

static int counter = 0;
来源：http://csf.shuidangran.top

[S29] C：变参函数
来源：http://qbm.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zgv.ybcxt.top

[S30] C：头文件保护
来源：http://qst.ydzc1.top

#ifndef X_H
来源：http://uiv.tian-w.cn

#define X_H
来源：http://sgp.fktsv.cn

#endif
来源：http://ywv.haohaochexian.top

[S31] C++：Hello World
来源：http://sdn.mhx1999.top

#include <iostream>
来源：http://mpr.xinyue.icu

int main() { std::cout << "Hello\n"; }
来源：http://rpy.pycfn.com

[S32] C++：字符串
来源：http://qzh.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://isw.ydjk.org.cn

[S33] C++：vector 增删
来源：http://qyw.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ujq.dianchejie.cn

[S34] C++：遍历 vector
来源：http://sxg.quarkkingdee.top

for (auto &x : v) { std::cout << x; }
来源：http://vlw.yuanzhike.top

[S35] C++：map
来源：http://jcx.redwolf501.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fsu.fehbvm.com

[S36] C++：unordered_map
来源：http://vze.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dkd.ybcxt.top

[S37] C++：set
来源：http://maa.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pha.sxryk.cn

[S38] C++：排序
来源：http://xcr.birdmap.top

std::sort(v.begin(), v.end());
来源：http://owp.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://vtz.hcnkem.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rir.zhiwuduotai.top

[S40] C++：查找元素
来源：http://srl.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jgy.sweek.top

[S41] C++：类与构造函数
来源：http://isi.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://frs.yj20258888.top

[S42] C++：继承与虚函数
来源：http://pqq.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://xip.52xcode.cn

[S43] C++：智能指针
来源：http://kcz.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://pzg.feifeiyinyue.top

[S44] C++：引用传参
来源：http://qwt.hammf.cn

void inc(int &x) { ++x; }
来源：http://iic.tianlin.xyz

[S45] C++：lambda
来源：http://xee.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://vvv.yanxiufei.cn

[S46] C++：函数模板
来源：http://mnt.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vau.ctjpmb.com

[S47] C++：结构化绑定遍历
来源：http://pxv.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://the.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://qqn.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://qri.hesvh.cn

while (std::getline(in, line)) { }
来源：http://kvi.pycfn.com

[S49] C++：写文件
来源：http://apd.jinghuilouyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rzt.tian-w.cn

[S50] C++：格式化数字
来源：http://muj.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lmb.aizwys.cn

[S51] C++：显式类型转换
来源：http://vch.aibaodan.cn

static_cast<double>(a) / b
来源：http://rao.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://jhy.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://nwq.hysaishi.cn

[S53] C++：移动语义
来源：http://mbb.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://sfw.yonumen.top

[S54] C++：异常处理
来源：http://muw.9152youxi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gbb.hfpthk.cn

[S55] C++：结构化绑定
来源：http://wbx.zdbjq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fmd.fanxiaobao.xyz

[S56] C++：optional
来源：http://zac.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bhn.ppjwa.cn

[S57] C++：编译期常量
来源：http://ekb.tarul.cn

constexpr int N = 10;
来源：http://qdw.zdbjq.cn

[S58] C++：命名空间
来源：http://ubl.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://mqe.yueranfly.top

[S59] C++：静态断言
来源：http://zwo.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zvb.fehbvm.com

[S60] C++：遍历并删除元素
来源：http://krj.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://coz.yuxming.cn

================================================================================
来源：http://nea.gotoacloud.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sqm.nwbrower.top

================================================================================
来源：http://yun.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://wya.jiagoushi.top

println("Hello")
来源：http://nej.hcnkem.com

[T02] Kotlin：变量
来源：http://awx.tian-w.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ssf.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://zxc.svipenyu.cn

"值: $b"
来源：http://ctd.meibo888.top

[T04] Kotlin：空安全
来源：http://mlh.gzhubu.top

val n: String? = null;  n?.length
来源：http://brj.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://awr.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lsu.iojbl.cn

[T06] Kotlin：集合映射
来源：http://tqh.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pdy.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://hpl.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ufj.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://yug.yuxming.cn

data class User(val name: String, val age: Int)
来源：http://kdi.pycfn.com

[T09] Kotlin：扩展函数
来源：http://fha.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://cgh.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://hkk.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tvr.nwbrower.top

[T11] Kotlin：协程
来源：http://ngl.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://khf.havefunace.top

[T12] Kotlin：解构声明
来源：http://otw.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://jjx.yuanzhike.top

[T13] Kotlin：只读 Map
来源：http://llx.smart0.xyz

val m = mapOf("a" to 1)
来源：http://wza.sweek.top

[T14] Kotlin：循环
来源：http://okz.cheryme.top

for (i in 1..10) println(i)
来源：http://fcl.yonumen.top

[T15] Kotlin：接口
来源：http://kwl.daria6918.cn

interface Shape { fun area(): Double }
来源：http://cjv.haohaochexian.top

[T16] Swift：Hello World
来源：http://otz.jqgufenzy.top

print("Hello")
来源：http://nxm.ydjk.org.cn

[T17] Swift：变量与常量
来源：http://xih.cqqwz.cn

var a = 1;  let b = 2
来源：http://myv.redwolf501.top

[T18] Swift：字符串插值
来源：http://xhm.0kj1m.cn

"值: \(b)"
来源：http://azj.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://yns.zhengqikj.top

if let n = opt { print(n) }
来源：http://anp.xziqi.cn

[T20] Swift：数组操作
来源：http://coc.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://myq.yvedp.cn

[T21] Swift：遍历
来源：http://vcl.shanyushiyangtech.top

for x in a { print(x) }
来源：http://zjz.52xcode.cn

[T22] Swift：字典
来源：http://tne.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://fxl.hcnkem.com

[T23] Swift：函数
来源：http://vjn.xuetiantiany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blt.birdmap.top

[T24] Swift：闭包
来源：http://evk.mhx1999.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mbt.gzhubu.top


<!-- 参考信息 -->