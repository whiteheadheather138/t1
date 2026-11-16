代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dqg.shzxlz.cn

[R24] 大小写转换
来源：http://ggb.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qko.yuanzhike.top

[R25] 去后缀 / 去前缀
来源：http://srn.fzhhl.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uam.yj20258.top

[R26] 命令替换
来源：http://evh.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://vhs.xziqi.cn

[R27] 算术展开
来源：http://imq.meibo888.top

echo $((1 + 2 * 3))
来源：http://bos.yfazqb.com

[R28] 浮点运算
来源：http://nku.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://cuq.sjlbkw.cn

[R29] 定义函数
来源：http://vuo.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ovp.pengpengdd.cyou

[R30] 函数返回状态码
来源：http://bzx.yanxiufei.cn

f() { return 0; }; f || echo "失败了"
来源：http://tcg.yfazqb.com

[R31] 局部变量
来源：http://pfj.shuidangran.top

f() { local x=1; echo "$x"; }
来源：http://bst.316326.xyz

[R32] 参数个数校验
来源：http://nag.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uug.yfazqb.com

[R33] 捕获错误并提示行号
来源：http://uuz.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fvk.dianchejie.cn

[R34] 退出时清理
来源：http://lpq.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://cyh.yuanzhike.top

[R35] 后台执行并等待
来源：http://idj.yvedp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ryg.hfpthk.cn

[R36] 并发执行多个任务
来源：http://ize.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ejc.iojbl.cn

[R37] 把输出赋给变量
来源：http://lst.hfpthk.cn

files=$(ls -1)
来源：http://dit.dianchejie.cn

[R38] 管道串联
来源：http://zow.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://mdr.yuanzhike.top

[R39] 重定向标准输出与错误
来源：http://cdw.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://jsc.xziqi.cn

[R40] 追加写日志
来源：http://slt.nanxinkj.top

echo "log" >> out.log
来源：http://nrw.cheryme.top

[R41] 丢弃输出
来源：http://qun.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://hvs.guowangkeji.top

[R42] 输入重定向
来源：http://uer.jinqigufen.top

wc -l < a.txt
来源：http://zcc.yj202588.top

[R43] 按名字查找文件
来源：http://cdb.dashuyun.cn

find . -name "*.log" -type f
来源：http://zsb.ydzc1.top

[R44] 按修改时间查找
来源：http://axq.yuanzhike.top

find . -mtime -7 -type f
来源：http://usy.smart0.xyz

[R45] 批量删除
来源：http://zlx.zhaomingkeji.xyz

find . -name "*.tmp" -delete
来源：http://zfc.havefunace.top

[R46] 递归替换文件内容
来源：http://mny.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qzk.fktsv.cn

[R47] sed 单行替换
来源：http://dyx.shanyushiyangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://kbt.quarkkingdee.top

[R48] awk 取指定列
来源：http://uib.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://dzz.xziqi.cn

[R49] awk 带条件
来源：http://dwk.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gvs.nanxuanxn.top

[R50] awk 求和
来源：http://iql.gotoacloud.top

awk '{s += $2} END {print s}' a.txt
来源：http://qou.yj20258888.top

[R51] 排序去重取前几
来源：http://wni.xziqi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lvg.hongshengwenyu.top

[R52] 统计行数
来源：http://ieb.daria6918.cn

wc -l a.txt
来源：http://iff.jianghu66.top

[R53] 查看文件头与实时尾
来源：http://xxi.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fzc.pengpengdd.cyou

[R54] 比较两个文件
来源：http://mqe.ydjk.org.cn

diff a.txt b.txt
来源：http://wlh.snrcjt.cn

[R55] 压缩与解压
来源：http://kgi.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ohz.tian-w.cn

[R56] 远程拷贝
来源：http://ccc.hnqzz.top

scp file user@host:/path/
来源：http://taa.jianghu66.top

[R57] 远程执行命令
来源：http://emb.zhengqikj.top

ssh user@host 'uptime'
来源：http://zfd.pycfn.com

[R58] 下载文件
来源：http://ooo.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://edy.gaohongyu789.top

[R59] 发 POST JSON
来源：http://tfm.cucudq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tca.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://jrc.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qus.yvedp.cn

[R61] 磁盘占用
来源：http://kis.jiagoushi.top

df -h;  du -sh *
来源：http://nqa.hammf.cn

[R62] 找最占空间的文件
来源：http://snx.jyoumei.cn

du -ah . | sort -rh | head -10
来源：http://jht.yuanzhike.top

[R63] 内存与进程
来源：http://emy.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://pyq.chenlongwang.top

[R64] 结束进程
来源：http://hrh.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://nfx.nanxuanxn.top

[R65] 查看端口占用
来源：http://ejo.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oft.hcnkem.com

[R66] 定时任务
来源：http://vzm.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://qfl.chenlongwang.top

[R67] 生成随机十六进制串
来源：http://hmb.zdbjq.cn

openssl rand -hex 16
来源：http://stx.yj20258.top

[R68] 计算文件校验值
来源：http://jqt.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://wad.shuidangran.top

[R69] 生成随机密码
来源：http://jkp.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://ywj.yuanzhike.top

[R70] 时间戳与互转
来源：http://ctb.jlsjyb.cn

date +%s;  date -d @1700000000
来源：http://ecj.ydzc1.top

[R71] 日期格式化
来源：http://aks.hammf.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rhm.mhx1999.top

[R72] 等待端口就绪
来源：http://wcb.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kgg.fehbvm.com

[R73] 分割大日志
来源：http://eek.zhoulong.xyz

split -l 1000 big.log part_
来源：http://ibs.fengsongda.top

[R74] 批量重命名
来源：http://lmg.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fwp.uphjek.com

[R75] 导出环境变量
来源：http://vfp.shanyushiyangtech.top

export PATH="$HOME/bin:$PATH"
来源：http://mhi.fzhhl.top

[R76] 使用临时文件
来源：http://xtu.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jef.xuetiantiany.cn

[R77] 读取用户输入
来源：http://qvt.aibaodan.cn

read -rp "请输入: " ans
来源：http://mvc.kuanghao11.cn

[R78] 交互式菜单
来源：http://zyu.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xxc.epnwcf.com

[R79] 解析命令行选项
来源：http://thk.tarul.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://naf.birdmap.top

[R80] 查看脚本执行耗时
来源：http://pcw.ybcxt.top

time ./run.sh
来源：http://yay.cucudq.cn

================================================================================
来源：http://bmy.gaohongyu789.top

S. C / C++ 专题
来源：http://xlq.pycfn.com

================================================================================
来源：http://fkr.jqgufenzy.top

[S01] C：Hello World
来源：http://apv.zhongyouzk.top

#include <stdio.h>
来源：http://yew.jyoumei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hjt.52xcode.cn

[S02] C：变量与格式化输出
来源：http://ppr.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://dzm.zhiwuduotai.top

[S03] C：读入整数
来源：http://xwj.nanxinkj.top

int x; scanf("%d", &x);
来源：http://dia.daria6918.cn

[S04] C：字符串复制
来源：http://mbq.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://yva.guowangkeji.top

[S05] C：字符串长度
来源：http://ixj.yj20258.top

strlen(s)
来源：http://yit.bjfxy.top

[S06] C：字符串比较
来源：http://ltw.tianlin.xyz

strcmp(a, b) == 0
来源：http://awd.wangdashe.top

[S07] C：数组遍历求和
来源：http://rvf.jiagoushi.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dls.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://qfi.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lhu.hcnkem.com

[S09] C：结构体定义与初始化
来源：http://dkk.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rih.sysykeji.top

[S10] C：指针与解引用
来源：http://dzw.xziqi.cn

int *p = &a;  *p = 5;
来源：http://gxq.gzhubu.top

[S11] C：逐行读文件
来源：http://aog.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://kem.jqgufenzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://csz.snrcjt.cn

fclose(f);
来源：http://bjk.epnwcf.com

[S12] C：写文件
来源：http://oag.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bkg.0kj1m.cn

[S13] C：宏定义
来源：http://rdu.cashguo.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tot.svipenyu.cn

[S14] C：枚举
来源：http://cpd.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://smw.hysaishi.cn

[S15] C：类型转换
来源：http://jck.zdqjudy.top

(double) a / b
来源：http://fve.kuanghao11.cn

[S16] C：位操作置位
来源：http://ckk.tianlin.xyz

x |= (1 << 3);
来源：http://tpb.zycfv.cn

[S17] C：安全拼接字符串
来源：http://iaz.shanyushiyangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iwe.yueranfly.top

[S18] C：命令行参数
来源：http://qfv.smart0.xyz

int main(int argc, char **argv)
来源：http://rto.cheryme.top

[S19] C：快速排序
来源：http://pyp.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://wpy.yvedp.cn

[S20] C：二分查找
来源：http://mqs.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nis.jianghu66.top

[S21] C：字符类别判断
来源：http://mvu.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bpa.ehwqpu.com

[S22] C：字符串转数字
来源：http://mva.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://ueo.hcnkem.com

[S23] C：随机数
来源：http://bdg.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://fad.yanxiufei.cn

[S24] C：获取本地时间
来源：http://ogg.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wpw.jlsjyb.cn

[S25] C：内存拷贝
来源：http://omy.zhengqikj.top

memcpy(dst, src, n);
来源：http://uey.uphjek.com

[S26] C：内存清零
来源：http://dfn.uphjek.com

memset(a, 0, sizeof a);
来源：http://yec.zhijiandao.cn

[S27] C：定义常量
来源：http://hxk.sufxvd.cn

const double PI = 3.14159;
来源：http://pdm.ehwqpu.com

[S28] C：静态变量
来源：http://hmj.zhiwuduotai.top

static int counter = 0;
来源：http://azw.316326.xyz

[S29] C：变参函数
来源：http://xew.ctjpmb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://buk.sufxvd.cn

[S30] C：头文件保护
来源：http://mlg.tarul.cn

#ifndef X_H
来源：http://hdv.yonumen.top

#define X_H
来源：http://kuz.andypj.xyz

#endif
来源：http://krd.xylfe.cn

[S31] C++：Hello World
来源：http://vyo.bbcook.cn

#include <iostream>
来源：http://nqn.fengsongda.top

int main() { std::cout << "Hello\n"; }
来源：http://nbx.haohaochexian.top

[S32] C++：字符串
来源：http://vzr.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://pbl.sxryk.cn

[S33] C++：vector 增删
来源：http://viq.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nmh.nwbrower.top

[S34] C++：遍历 vector
来源：http://hrf.yongpay.top

for (auto &x : v) { std::cout << x; }
来源：http://qec.hongshengwenyu.top

[S35] C++：map
来源：http://hqe.guannengcc.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lws.jqgufenzy.top

[S36] C++：unordered_map
来源：http://ozw.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blp.ybcxt.top

[S37] C++：set
来源：http://uvd.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vcc.tian-w.cn

[S38] C++：排序
来源：http://ahb.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://mlp.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://muu.ctjpmb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mun.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://hpm.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qvf.vqdsnc.cn

[S41] C++：类与构造函数
来源：http://qyz.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hvk.yuxming.cn

[S42] C++：继承与虚函数
来源：http://gar.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://ryy.aibaodan.cn

[S43] C++：智能指针
来源：http://fka.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://xpb.xylfe.cn

[S44] C++：引用传参
来源：http://skt.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://buv.guowangkeji.top

[S45] C++：lambda
来源：http://nhw.hnqzz.top

auto add = [](int a, int b) { return a + b; };
来源：http://vgr.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://atd.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://byr.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://oxo.meibo888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ixn.jqgfzy.top

[S48] C++：逐行读文件
来源：http://yvk.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lel.haohaochexian.top

while (std::getline(in, line)) { }
来源：http://zix.hammf.cn

[S49] C++：写文件
来源：http://uda.zhijiandao.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qwm.zdqjudy.top

[S50] C++：格式化数字
来源：http://dpg.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xol.vqdsnc.cn

[S51] C++：显式类型转换
来源：http://pyf.fanxiaobao.xyz

static_cast<double>(a) / b
来源：http://rda.mhx1999.top

[S52] C++：const 与 noexcept
来源：http://iib.redwolf501.top

int size() const noexcept { return n_; }
来源：http://ueq.hnqzz.top

[S53] C++：移动语义
来源：http://uww.hammf.cn

std::vector<int> w = std::move(v);
来源：http://fac.yuanzhike.top

[S54] C++：异常处理
来源：http://dtu.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mky.bbcook.cn

[S55] C++：结构化绑定
来源：http://rxm.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qsa.shanyushiyangtech.top

[S56] C++：optional
来源：http://qtr.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tma.hammf.cn

[S57] C++：编译期常量
来源：http://zvt.sxryk.cn

constexpr int N = 10;
来源：http://dwu.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://ogg.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://gyw.fehbvm.com

[S59] C++：静态断言
来源：http://mcy.9152youxi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mtu.chenlongwang.top

[S60] C++：遍历并删除元素
来源：http://xvp.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cwl.yueranfly.top

================================================================================
来源：http://sla.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lkv.yj202588.top

================================================================================
来源：http://ucw.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://ktd.meibo888.top

println("Hello")
来源：http://gpp.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://lmq.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lol.yanxiufei.cn

[T03] Kotlin：字符串模板
来源：http://hsl.pycfn.com

"值: $b"
来源：http://urb.cqqwz.cn

[T04] Kotlin：空安全
来源：http://xal.ppjwa.cn

val n: String? = null;  n?.length
来源：http://bno.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://dox.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://akh.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://pqt.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dxs.yanxiufei.cn

[T07] Kotlin：集合过滤
来源：http://rsy.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pun.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://wyr.yj20258.top

data class User(val name: String, val age: Int)
来源：http://xuj.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://xld.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://ymy.mhx1999.top

[T10] Kotlin：默认参数
来源：http://twk.epnwcf.com

fun greet(name: String = "World") = "Hi $name"
来源：http://lad.cheryme.top

[T11] Kotlin：协程
来源：http://dxr.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yob.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://jer.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://hyg.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://zyy.ydzc1.top

val m = mapOf("a" to 1)
来源：http://whp.cucudq.cn

[T14] Kotlin：循环
来源：http://ghd.yj20258888.top

for (i in 1..10) println(i)
来源：http://idw.havefunace.top

[T15] Kotlin：接口
来源：http://kxr.fanxiaobao.xyz

interface Shape { fun area(): Double }
来源：http://vix.svipenyu.cn

[T16] Swift：Hello World
来源：http://kfo.yj20258888.top

print("Hello")
来源：http://pyv.zhengqikj.top

[T17] Swift：变量与常量
来源：http://kfq.xziqi.cn

var a = 1;  let b = 2
来源：http://qja.shzxlz.cn

[T18] Swift：字符串插值
来源：http://zts.sweek.top

"值: \(b)"
来源：http://ygj.zhoulong.xyz

[T19] Swift：可选绑定
来源：http://khx.fktsv.cn

if let n = opt { print(n) }
来源：http://rsr.sysykeji.top

[T20] Swift：数组操作
来源：http://gyn.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://zrg.hcnkem.com

[T21] Swift：遍历
来源：http://cxe.epnwcf.com

for x in a { print(x) }
来源：http://ijh.xinyue.icu

[T22] Swift：字典
来源：http://ywn.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bni.sweek.top

[T23] Swift：函数
来源：http://fex.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qus.fktsv.cn

[T24] Swift：闭包
来源：http://omn.guowangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vba.gzhubu.top

[T25] Swift：结构体
来源：http://wri.xinyue.icu

struct P { var x: Int }
来源：http://nju.hysaishi.cn

[T26] Swift：类与重写
来源：http://hml.yj20258888.top

class A: Base { override func f() {} }
来源：http://tme.fehbvm.com


<!-- 参考信息 -->