代发 wailian999

echo "${#s}"
来源：http://qnq.nanxinkj.top

[R22] 截取子串
来源：http://hfx.yuxming.cn

echo "${s:0:5}"
来源：http://gdb.shzxlz.cn

[R23] 字符串替换
来源：http://tlz.tanke756.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gla.vehdjk.com

[R24] 大小写转换
来源：http://xyd.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://spc.epnwcf.com

[R25] 去后缀 / 去前缀
来源：http://odn.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://ptl.birdmap.top

[R26] 命令替换
来源：http://mbo.yangfankeji.com

now=$(date +%F); echo "$now"
来源：http://pug.vehdjk.com

[R27] 算术展开
来源：http://bmt.bbcook.cn

echo $((1 + 2 * 3))
来源：http://hxi.zhixingplan.top

[R28] 浮点运算
来源：http://xth.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://bmx.birdmap.top

[R29] 定义函数
来源：http://saj.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aza.cucudq.cn

[R30] 函数返回状态码
来源：http://hnt.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://bkx.xylfe.cn

[R31] 局部变量
来源：http://uxr.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://ikr.tarul.cn

[R32] 参数个数校验
来源：http://fcw.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fje.birdmap.top

[R33] 捕获错误并提示行号
来源：http://xrb.nanxuanxn.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bpe.xziqi.cn

[R34] 退出时清理
来源：http://arg.zhaomingkeji.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://kpj.xziqi.cn

[R35] 后台执行并等待
来源：http://wed.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kum.zhengqikj.top

[R36] 并发执行多个任务
来源：http://kmj.gaohongyu789.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yya.zhaomingkeji.xyz

[R37] 把输出赋给变量
来源：http://jhz.gotoacloud.top

files=$(ls -1)
来源：http://fru.chenlongwang.top

[R38] 管道串联
来源：http://kwh.xylfe.cn

cat a.txt | grep -i error | wc -l
来源：http://puz.pycfn.com

[R39] 重定向标准输出与错误
来源：http://dwa.daxiang520.top

cmd > out.log 2>&1
来源：http://rcz.pengpengdd.cyou

[R40] 追加写日志
来源：http://crj.guannengcc.top

echo "log" >> out.log
来源：http://xnd.ydzc1.top

[R41] 丢弃输出
来源：http://eov.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://oeb.iojbl.cn

[R42] 输入重定向
来源：http://klq.sysykeji.top

wc -l < a.txt
来源：http://ygb.hysaishi.cn

[R43] 按名字查找文件
来源：http://nxy.pycfn.com

find . -name "*.log" -type f
来源：http://mnq.chenlongwang.top

[R44] 按修改时间查找
来源：http://cbm.guowangkeji.top

find . -mtime -7 -type f
来源：http://inn.xylfe.cn

[R45] 批量删除
来源：http://lul.cheryme.top

find . -name "*.tmp" -delete
来源：http://kul.epnwcf.com

[R46] 递归替换文件内容
来源：http://jpu.hongshengwenyu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jbg.yfazqb.com

[R47] sed 单行替换
来源：http://hgo.shanyushiyangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://xcb.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://sor.ppjwa.cn

awk '{print $1, $3}' a.txt
来源：http://dfn.nanxinkj.top

[R49] awk 带条件
来源：http://jcc.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jlt.c1oappe.top

[R50] awk 求和
来源：http://ntt.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ucx.andypj.xyz

[R51] 排序去重取前几
来源：http://gfo.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hwq.aizwys.cn

[R52] 统计行数
来源：http://klx.cucudq.cn

wc -l a.txt
来源：http://wqd.birdmap.top

[R53] 查看文件头与实时尾
来源：http://cbj.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rzp.aibaodan.cn

[R54] 比较两个文件
来源：http://uch.xylfe.cn

diff a.txt b.txt
来源：http://yqu.guowangkeji.top

[R55] 压缩与解压
来源：http://lyw.daria6918.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nru.nwbrower.top

[R56] 远程拷贝
来源：http://ueu.shuidangran.top

scp file user@host:/path/
来源：http://zgr.tian-w.cn

[R57] 远程执行命令
来源：http://wsg.shanyushiyangtech.top

ssh user@host 'uptime'
来源：http://aqh.fanxiaobao.xyz

[R58] 下载文件
来源：http://hpo.iojbl.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iow.xuetiantiany.cn

[R59] 发 POST JSON
来源：http://mzs.yangfankeji.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nyi.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://koj.wangdashe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://igc.9152youxi.cn

[R61] 磁盘占用
来源：http://bxb.hcnkem.com

df -h;  du -sh *
来源：http://ubt.ppjwa.cn

[R62] 找最占空间的文件
来源：http://hse.tianlin.xyz

du -ah . | sort -rh | head -10
来源：http://vvk.ydzc1.top

[R63] 内存与进程
来源：http://gif.jinghuilouyu.cn

free -h;  ps aux | grep nginx
来源：http://nwh.tianlin.xyz

[R64] 结束进程
来源：http://mmr.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://fcx.fengsongda.top

[R65] 查看端口占用
来源：http://rxe.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pzb.fengsongda.top

[R66] 定时任务
来源：http://loo.zhoulong.xyz

crontab -e;  crontab -l
来源：http://wpe.tarul.cn

[R67] 生成随机十六进制串
来源：http://jfz.gotoacloud.top

openssl rand -hex 16
来源：http://ldm.andypj.xyz

[R68] 计算文件校验值
来源：http://mqz.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://abo.hammf.cn

[R69] 生成随机密码
来源：http://vye.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://gwn.redwolf501.top

[R70] 时间戳与互转
来源：http://zfq.hammf.cn

date +%s;  date -d @1700000000
来源：http://gvl.jianghu66.top

[R71] 日期格式化
来源：http://ghe.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rbj.sxryk.cn

[R72] 等待端口就绪
来源：http://uul.ppjwa.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hff.ctjpmb.com

[R73] 分割大日志
来源：http://fgg.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://qki.pengpengdd.cyou

[R74] 批量重命名
来源：http://qis.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mmq.sjlbkw.cn

[R75] 导出环境变量
来源：http://euv.daria6918.cn

export PATH="$HOME/bin:$PATH"
来源：http://bnc.ydjk.org.cn

[R76] 使用临时文件
来源：http://zki.ybcxt.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zwi.shuidangran.top

[R77] 读取用户输入
来源：http://cdo.feifeiyinyue.top

read -rp "请输入: " ans
来源：http://rga.wangdashe.top

[R78] 交互式菜单
来源：http://lpa.fehbvm.com

select opt in a b c; do echo "$opt"; break; done
来源：http://seh.tarul.cn

[R79] 解析命令行选项
来源：http://dlc.hnxiangtu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vio.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://dqi.xingfuxueyuan.xyz

time ./run.sh
来源：http://rfa.nwbrower.top

================================================================================
来源：http://zeh.wangdashe.top

S. C / C++ 专题
来源：http://arx.jqgfzy.top

================================================================================
来源：http://zdu.zhengqikj.top

[S01] C：Hello World
来源：http://ozc.jinghuilouyu.cn

#include <stdio.h>
来源：http://fok.ywan-chungtsiang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ubt.zhiwuduotai.top

[S02] C：变量与格式化输出
来源：http://tiq.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://fzj.xziqi.cn

[S03] C：读入整数
来源：http://fpy.epnwcf.com

int x; scanf("%d", &x);
来源：http://mxi.hcnkem.com

[S04] C：字符串复制
来源：http://bcv.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://qgg.gzhubu.top

[S05] C：字符串长度
来源：http://zgo.hnqzz.top

strlen(s)
来源：http://wyt.yueranfly.top

[S06] C：字符串比较
来源：http://uvx.dashuyun.cn

strcmp(a, b) == 0
来源：http://ucx.ctjpmb.com

[S07] C：数组遍历求和
来源：http://eij.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kez.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://xnv.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vyf.yongpay.top

[S09] C：结构体定义与初始化
来源：http://ixc.gotoacloud.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qvr.xziqi.cn

[S10] C：指针与解引用
来源：http://ccr.chenzaomai.com

int *p = &a;  *p = 5;
来源：http://urx.xylfe.cn

[S11] C：逐行读文件
来源：http://hib.ctjpmb.com

FILE *f = fopen("a.txt", "r");
来源：http://lto.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sne.yfazqb.com

fclose(f);
来源：http://yyb.hammf.cn

[S12] C：写文件
来源：http://syu.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hlu.hfpthk.cn

[S13] C：宏定义
来源：http://spc.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dvo.sjlbkw.cn

[S14] C：枚举
来源：http://ztm.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://qnb.gaohongyu789.top

[S15] C：类型转换
来源：http://gwz.hesvh.cn

(double) a / b
来源：http://buk.iojbl.cn

[S16] C：位操作置位
来源：http://vao.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://rjy.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://oyr.shanyushiyangtech.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nir.gaohongyu789.top

[S18] C：命令行参数
来源：http://maa.0kj1m.cn

int main(int argc, char **argv)
来源：http://ins.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://psn.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://uiu.zdbjq.cn

[S20] C：二分查找
来源：http://vmy.zhaomingkeji.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qbv.yongpay.top

[S21] C：字符类别判断
来源：http://kyz.zhiwuduotai.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pyh.52xcode.cn

[S22] C：字符串转数字
来源：http://uur.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ytk.yonumen.top

[S23] C：随机数
来源：http://vwg.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lyk.chenjidiqi.icu

[S24] C：获取本地时间
来源：http://aay.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mqj.daria6918.cn

[S25] C：内存拷贝
来源：http://kgm.wangshuangyany.cn

memcpy(dst, src, n);
来源：http://vgt.cucudq.cn

[S26] C：内存清零
来源：http://gda.0kj1m.cn

memset(a, 0, sizeof a);
来源：http://etm.fanxiaobao.xyz

[S27] C：定义常量
来源：http://wif.daria6918.cn

const double PI = 3.14159;
来源：http://emb.jyoumei.cn

[S28] C：静态变量
来源：http://hxd.pycfn.com

static int counter = 0;
来源：http://vfx.zycfv.cn

[S29] C：变参函数
来源：http://dwd.wangdashe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rok.yuanzhike.top

[S30] C：头文件保护
来源：http://ikm.sysykeji.top

#ifndef X_H
来源：http://nde.yj202588.top

#define X_H
来源：http://tcu.guowangkeji.top

#endif
来源：http://zha.jqgfzy.top

[S31] C++：Hello World
来源：http://upx.yanxiufei.cn

#include <iostream>
来源：http://jqx.dianchejie.cn

int main() { std::cout << "Hello\n"; }
来源：http://ptj.zhongyouzk.top

[S32] C++：字符串
来源：http://rjb.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://vxw.c1oappe.top

[S33] C++：vector 增删
来源：http://vsg.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fca.nwbrower.top

[S34] C++：遍历 vector
来源：http://tqr.hfpthk.cn

for (auto &x : v) { std::cout << x; }
来源：http://tdz.hcnkem.com

[S35] C++：map
来源：http://hnk.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ezl.ppjwa.cn

[S36] C++：unordered_map
来源：http://taz.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wfr.haohaochexian.top

[S37] C++：set
来源：http://owj.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cjm.shanyushiyangtech.top

[S38] C++：排序
来源：http://kcd.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://dvk.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://wcy.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pyz.zdqjudy.top

[S40] C++：查找元素
来源：http://bll.jinghuilouyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ujk.ppjwa.cn

[S41] C++：类与构造函数
来源：http://irx.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gsy.iojbl.cn

[S42] C++：继承与虚函数
来源：http://tpq.ywan-chungtsiang.top

class B : public Base { public: void f() override {} };
来源：http://wwc.shzxlz.cn

[S43] C++：智能指针
来源：http://yls.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://qpo.gaohongyu789.top

[S44] C++：引用传参
来源：http://tds.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://ttl.jinqigfzy.top

[S45] C++：lambda
来源：http://zqo.pycfn.com

auto add = [](int a, int b) { return a + b; };
来源：http://jfw.hywenlv.cn

[S46] C++：函数模板
来源：http://ono.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kks.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://jyg.zhixingplan.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kva.daxiang520.top

[S48] C++：逐行读文件
来源：http://tch.yongpay.top

std::ifstream in("a.txt");  std::string line;
来源：http://ndh.fktsv.cn

while (std::getline(in, line)) { }
来源：http://uev.nanxuanxn.top

[S49] C++：写文件
来源：http://yvq.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wez.zhijiandao.cn

[S50] C++：格式化数字
来源：http://tzy.smart0.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ctn.andypj.xyz

[S51] C++：显式类型转换
来源：http://zmb.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://hac.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://zyv.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://isx.hesvh.cn

[S53] C++：移动语义
来源：http://iiy.havefunace.top

std::vector<int> w = std::move(v);
来源：http://ijl.yj20258.top

[S54] C++：异常处理
来源：http://ofl.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uzp.jinqigufen.top

[S55] C++：结构化绑定
来源：http://tba.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://exj.hcnkem.com

[S56] C++：optional
来源：http://tmx.hysaishi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ndo.daria6918.cn

[S57] C++：编译期常量
来源：http://ofl.yj202588.top

constexpr int N = 10;
来源：http://zzy.zdqjudy.top

[S58] C++：命名空间
来源：http://zqi.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://joe.xylfe.cn

[S59] C++：静态断言
来源：http://eqw.zhoulong.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bpo.ehwqpu.com

[S60] C++：遍历并删除元素
来源：http://ezf.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ctr.epnwcf.com

================================================================================
来源：http://ivr.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hsp.vehdjk.com

================================================================================
来源：http://hwj.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://wjk.0kj1m.cn

println("Hello")
来源：http://hxl.yfazqb.com

[T02] Kotlin：变量
来源：http://esl.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ulw.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://iui.gotoacloud.top

"值: $b"
来源：http://nbb.vehdjk.com

[T04] Kotlin：空安全
来源：http://sfd.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://hag.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://trd.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jez.yfazqb.com

[T06] Kotlin：集合映射
来源：http://eqj.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ajo.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://anh.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://huk.yonumen.top

[T08] Kotlin：数据类
来源：http://dfq.yj20258.top

data class User(val name: String, val age: Int)
来源：http://gff.dashuyun.cn

[T09] Kotlin：扩展函数
来源：http://pwx.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://wst.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://xfv.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://bht.aibaodan.cn

[T11] Kotlin：协程
来源：http://jfs.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wef.0kj1m.cn

[T12] Kotlin：解构声明
来源：http://udj.cashguo.top

val (a, b) = Pair(1, 2)
来源：http://lig.316326.xyz

[T13] Kotlin：只读 Map
来源：http://bsw.yonumen.top

val m = mapOf("a" to 1)
来源：http://ztl.xingfuxueyuan.xyz

[T14] Kotlin：循环
来源：http://vcj.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://hvu.zhaomingkeji.xyz

[T15] Kotlin：接口
来源：http://isv.ehwqpu.com

interface Shape { fun area(): Double }
来源：http://mac.aizwys.cn

[T16] Swift：Hello World
来源：http://vmr.nanxuanxn.top

print("Hello")
来源：http://izb.ybcxt.top

[T17] Swift：变量与常量
来源：http://woo.haohaochexian.top

var a = 1;  let b = 2
来源：http://pnp.yuxming.cn

[T18] Swift：字符串插值
来源：http://kpn.xuanzx.com

"值: \(b)"
来源：http://jye.gogol.net.cn

[T19] Swift：可选绑定
来源：http://wuh.jiagoushi.top

if let n = opt { print(n) }
来源：http://ocn.gogol.net.cn

[T20] Swift：数组操作
来源：http://hqc.gotoacloud.top

var a = [1, 2, 3];  a.append(4)
来源：http://kqy.snrcjt.cn

[T21] Swift：遍历
来源：http://jxy.cashguo.top

for x in a { print(x) }
来源：http://efa.vqdsnc.cn

[T22] Swift：字典
来源：http://lcf.fengsongda.top

var d = ["a": 1];  d["b"] = 2
来源：http://ext.zhixingplan.top

[T23] Swift：函数
来源：http://nrh.hnqzz.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fmn.birdmap.top

[T24] Swift：闭包
来源：http://gzn.tianlin.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://yxo.dianchejie.cn


<!-- 参考信息 -->