代发 wailian999

echo $((1 + 2 * 3))
来源：http://xwc.cqqwz.cn

[R28] 浮点运算
来源：http://yuw.xylfe.cn

echo "scale=2; 10/3" | bc
来源：http://wzr.havefunace.top

[R29] 定义函数
来源：http://dnb.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gsz.cucudq.cn

[R30] 函数返回状态码
来源：http://oic.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://mpd.xuetiantiany.cn

[R31] 局部变量
来源：http://ere.xylfe.cn

f() { local x=1; echo "$x"; }
来源：http://hoj.shuidangran.top

[R32] 参数个数校验
来源：http://dua.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fvs.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://hqi.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://smp.guowangkeji.top

[R34] 退出时清理
来源：http://nca.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://bet.ybcxt.top

[R35] 后台执行并等待
来源：http://zdw.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://daz.hesvh.cn

[R36] 并发执行多个任务
来源：http://uli.bbcook.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://als.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://fqc.hammf.cn

files=$(ls -1)
来源：http://qsc.hesvh.cn

[R38] 管道串联
来源：http://vrs.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://dyx.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://gdl.zycfv.cn

cmd > out.log 2>&1
来源：http://kqo.zhijiandao.cn

[R40] 追加写日志
来源：http://mdc.sweek.top

echo "log" >> out.log
来源：http://qer.shangyingyoupin.top

[R41] 丢弃输出
来源：http://uak.9152youxi.cn

cmd >/dev/null 2>&1
来源：http://dvo.vqdsnc.cn

[R42] 输入重定向
来源：http://vfd.zhoulong.xyz

wc -l < a.txt
来源：http://imp.yj20258888.top

[R43] 按名字查找文件
来源：http://cli.vqdsnc.cn

find . -name "*.log" -type f
来源：http://iej.shzxlz.cn

[R44] 按修改时间查找
来源：http://vuq.0kj1m.cn

find . -mtime -7 -type f
来源：http://bgj.dianchejie.cn

[R45] 批量删除
来源：http://vjx.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://vae.ehwqpu.com

[R46] 递归替换文件内容
来源：http://ltb.jianghu66.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://klw.yonumen.top

[R47] sed 单行替换
来源：http://wfq.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://zvp.ehwqpu.com

[R48] awk 取指定列
来源：http://kib.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://ilq.zhixingplan.top

[R49] awk 带条件
来源：http://dmk.0kj1m.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iii.cucudq.cn

[R50] awk 求和
来源：http://qin.xziqi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ime.wangdashe.top

[R51] 排序去重取前几
来源：http://efw.chenjidiqi.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://mab.sufxvd.cn

[R52] 统计行数
来源：http://boe.jianghu66.top

wc -l a.txt
来源：http://aiq.vqdsnc.cn

[R53] 查看文件头与实时尾
来源：http://yzo.yvedp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lgp.daxiang520.top

[R54] 比较两个文件
来源：http://pzy.yuanzhike.top

diff a.txt b.txt
来源：http://bzu.ctjpmb.com

[R55] 压缩与解压
来源：http://eqk.gzhubu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mzu.xuetiantiany.cn

[R56] 远程拷贝
来源：http://wkw.0kj1m.cn

scp file user@host:/path/
来源：http://dym.hywenlv.cn

[R57] 远程执行命令
来源：http://onw.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://wsw.jinghuilouyu.cn

[R58] 下载文件
来源：http://peo.epnwcf.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eep.fengsongda.top

[R59] 发 POST JSON
来源：http://ewn.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xnm.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://wno.nwbrower.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vvy.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://gfm.tian-w.cn

df -h;  du -sh *
来源：http://qrs.9152youxi.cn

[R62] 找最占空间的文件
来源：http://psl.yonumen.top

du -ah . | sort -rh | head -10
来源：http://gds.jlsjyb.cn

[R63] 内存与进程
来源：http://qmy.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://ewt.nanxinkj.top

[R64] 结束进程
来源：http://fhh.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://qna.yfazqb.com

[R65] 查看端口占用
来源：http://mvi.52xcode.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mpe.quarkkingdee.top

[R66] 定时任务
来源：http://vwr.yj202588.top

crontab -e;  crontab -l
来源：http://eal.andypj.xyz

[R67] 生成随机十六进制串
来源：http://atb.pycfn.com

openssl rand -hex 16
来源：http://ski.jianghu66.top

[R68] 计算文件校验值
来源：http://sbm.epnwcf.com

sha256sum a.txt;  md5sum a.txt
来源：http://ahy.jinqigfzy.top

[R69] 生成随机密码
来源：http://zjz.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://mxp.nanxuanxn.top

[R70] 时间戳与互转
来源：http://tqh.fengsongda.top

date +%s;  date -d @1700000000
来源：http://pca.wangdashe.top

[R71] 日期格式化
来源：http://tlu.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jwg.zhijiandao.cn

[R72] 等待端口就绪
来源：http://xqc.epnwcf.com

until nc -z localhost 3306; do sleep 1; done
来源：http://mxe.xylfe.cn

[R73] 分割大日志
来源：http://gwd.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://zlb.meibo888.top

[R74] 批量重命名
来源：http://zdh.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tjb.fengsongda.top

[R75] 导出环境变量
来源：http://cla.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://hsv.jlsjyb.cn

[R76] 使用临时文件
来源：http://fjf.zhaomingkeji.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mja.hywenlv.cn

[R77] 读取用户输入
来源：http://pnm.wangdashe.top

read -rp "请输入: " ans
来源：http://ibs.zhiwuduotai.top

[R78] 交互式菜单
来源：http://gvv.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://oad.yj20258888.top

[R79] 解析命令行选项
来源：http://kxt.yangfankeji.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://grs.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://bus.shanyushiyangkeji.top

time ./run.sh
来源：http://tep.jinghuilouyu.cn

================================================================================
来源：http://mor.quarkkingdee.top

S. C / C++ 专题
来源：http://ncl.fanxiaobao.xyz

================================================================================
来源：http://ubz.havefunace.top

[S01] C：Hello World
来源：http://xok.9152youxi.cn

#include <stdio.h>
来源：http://qxn.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gfi.sweek.top

[S02] C：变量与格式化输出
来源：http://goo.kuanghao11.cn

int a = 10; printf("%d\n", a);
来源：http://qpy.316326.xyz

[S03] C：读入整数
来源：http://mda.dianchejie.cn

int x; scanf("%d", &x);
来源：http://sjj.c1oappe.top

[S04] C：字符串复制
来源：http://xkl.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yca.mhx1999.top

[S05] C：字符串长度
来源：http://whz.shanyushiyangkeji.top

strlen(s)
来源：http://pul.zhijiandao.cn

[S06] C：字符串比较
来源：http://ysy.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://xzc.chenzaomai.com

[S07] C：数组遍历求和
来源：http://mpe.fengsongda.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iwc.ppjwa.cn

[S08] C：动态内存分配与释放
来源：http://nmu.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qbp.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://qkz.jyoumei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zqo.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://pjy.daxiang520.top

int *p = &a;  *p = 5;
来源：http://gqs.sweek.top

[S11] C：逐行读文件
来源：http://mwc.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://gcq.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rcy.fzhhl.top

fclose(f);
来源：http://hgk.zhixingplan.top

[S12] C：写文件
来源：http://tdk.xinyue.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hgt.zdbjq.cn

[S13] C：宏定义
来源：http://jgm.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gsu.yfazqb.com

[S14] C：枚举
来源：http://uyu.zycfv.cn

enum Color { RED, GREEN, BLUE };
来源：http://whn.yj20258.top

[S15] C：类型转换
来源：http://cyx.feifeiyinyue.top

(double) a / b
来源：http://rix.hywenlv.cn

[S16] C：位操作置位
来源：http://fsw.ctjpmb.com

x |= (1 << 3);
来源：http://khy.yj20258.top

[S17] C：安全拼接字符串
来源：http://tbf.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aau.aizwys.cn

[S18] C：命令行参数
来源：http://kiv.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://nok.yanxiufei.cn

[S19] C：快速排序
来源：http://ypx.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://nnp.zhengqikj.top

[S20] C：二分查找
来源：http://wgu.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bgc.yongpay.top

[S21] C：字符类别判断
来源：http://yzl.wangdashe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mdu.tianlin.xyz

[S22] C：字符串转数字
来源：http://wlo.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ixw.hywenlv.cn

[S23] C：随机数
来源：http://trc.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qwg.vehdjk.com

[S24] C：获取本地时间
来源：http://hzw.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cyw.jianghu66.top

[S25] C：内存拷贝
来源：http://pyn.haohaochexian.top

memcpy(dst, src, n);
来源：http://zqj.gaohongyu789.top

[S26] C：内存清零
来源：http://foz.shuidangran.top

memset(a, 0, sizeof a);
来源：http://ksq.hysaishi.cn

[S27] C：定义常量
来源：http://zfi.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://ssk.zdbjq.cn

[S28] C：静态变量
来源：http://ana.yueranfly.top

static int counter = 0;
来源：http://toa.aibaodan.cn

[S29] C：变参函数
来源：http://ibs.guowangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://phk.snrcjt.cn

[S30] C：头文件保护
来源：http://kjj.gaohongyu789.top

#ifndef X_H
来源：http://tcs.daria6918.cn

#define X_H
来源：http://xow.ydzc1.top

#endif
来源：http://lcr.sweek.top

[S31] C++：Hello World
来源：http://zrl.cheryme.top

#include <iostream>
来源：http://vbg.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://nni.yuanzhike.top

[S32] C++：字符串
来源：http://mnq.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://ehr.gotoacloud.top

[S33] C++：vector 增删
来源：http://hqt.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hvv.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://wop.52xcode.cn

for (auto &x : v) { std::cout << x; }
来源：http://kqk.shanyushiyangtech.top

[S35] C++：map
来源：http://bfz.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ids.yuxming.cn

[S36] C++：unordered_map
来源：http://qnx.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pmm.haohaochexian.top

[S37] C++：set
来源：http://alm.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://shu.fzhhl.top

[S38] C++：排序
来源：http://rea.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://jkm.nwbrower.top

[S39] C++：自定义比较器排序
来源：http://emr.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ivu.daria6918.cn

[S40] C++：查找元素
来源：http://oss.guowangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sux.bjfxy.top

[S41] C++：类与构造函数
来源：http://uqr.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://otf.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://zrb.yuxming.cn

class B : public Base { public: void f() override {} };
来源：http://fck.vehdjk.com

[S43] C++：智能指针
来源：http://hdb.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://hii.daxiang520.top

[S44] C++：引用传参
来源：http://vrb.havefunace.top

void inc(int &x) { ++x; }
来源：http://cpw.fktsv.cn

[S45] C++：lambda
来源：http://wzp.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://vcn.quarkkingdee.top

[S46] C++：函数模板
来源：http://wac.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jdg.redwolf501.top

[S47] C++：结构化绑定遍历
来源：http://zpf.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vns.gotoacloud.top

[S48] C++：逐行读文件
来源：http://ztk.shuidangran.top

std::ifstream in("a.txt");  std::string line;
来源：http://poa.mhx1999.top

while (std::getline(in, line)) { }
来源：http://xop.sxryk.cn

[S49] C++：写文件
来源：http://bwy.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wro.sysykeji.top

[S50] C++：格式化数字
来源：http://qsy.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nmp.svipenyu.cn

[S51] C++：显式类型转换
来源：http://kmc.yfazqb.com

static_cast<double>(a) / b
来源：http://fye.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://cbh.zdqjudy.top

int size() const noexcept { return n_; }
来源：http://ney.aizwys.cn

[S53] C++：移动语义
来源：http://nll.ywan-chungtsiang.top

std::vector<int> w = std::move(v);
来源：http://cro.c1oappe.top

[S54] C++：异常处理
来源：http://brx.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xvn.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://fii.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jgf.hfpthk.cn

[S56] C++：optional
来源：http://mcd.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qpy.hnqzz.top

[S57] C++：编译期常量
来源：http://ofg.yj20258888.top

constexpr int N = 10;
来源：http://dxx.gotoacloud.top

[S58] C++：命名空间
来源：http://pll.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://ukp.ydzc1.top

[S59] C++：静态断言
来源：http://wxc.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ebc.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://kfp.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://was.hnqzz.top

================================================================================
来源：http://tto.mhx1999.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lyz.52xcode.cn

================================================================================
来源：http://kye.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://ixd.shangyingyoupin.top

println("Hello")
来源：http://poq.zycfv.cn

[T02] Kotlin：变量
来源：http://uzb.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qet.aizwys.cn

[T03] Kotlin：字符串模板
来源：http://iub.hywenlv.cn

"值: $b"
来源：http://hwu.pycfn.com

[T04] Kotlin：空安全
来源：http://ofp.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://wsx.yangfankeji.com

[T05] Kotlin：when 表达式
来源：http://dpd.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dlf.xinyue.icu

[T06] Kotlin：集合映射
来源：http://nqn.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://txg.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://qda.ehwqpu.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://emj.zycfv.cn

[T08] Kotlin：数据类
来源：http://btf.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://txn.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://wde.andypj.xyz

fun String.exclaim() = this + "!"
来源：http://nmb.smart0.xyz

[T10] Kotlin：默认参数
来源：http://suy.uphjek.com

fun greet(name: String = "World") = "Hi $name"
来源：http://oku.yuxming.cn

[T11] Kotlin：协程
来源：http://bwm.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hqr.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://lbb.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://kof.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://dao.0kj1m.cn

val m = mapOf("a" to 1)
来源：http://agy.cdnleiting.top

[T14] Kotlin：循环
来源：http://yew.ydzc1.top

for (i in 1..10) println(i)
来源：http://qfv.xingfuxueyuan.xyz

[T15] Kotlin：接口
来源：http://kux.snrcjt.cn

interface Shape { fun area(): Double }
来源：http://izo.haohaochexian.top

[T16] Swift：Hello World
来源：http://vug.jinqigufen.top

print("Hello")
来源：http://uua.hysaishi.cn

[T17] Swift：变量与常量
来源：http://lus.sjlbkw.cn

var a = 1;  let b = 2
来源：http://gvi.zhoulong.xyz

[T18] Swift：字符串插值
来源：http://xhb.ydzc1.top

"值: \(b)"
来源：http://iwp.yj20258888.top

[T19] Swift：可选绑定
来源：http://fmx.zycfv.cn

if let n = opt { print(n) }
来源：http://jca.shuidangran.top

[T20] Swift：数组操作
来源：http://yll.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://djn.yanxiufei.cn

[T21] Swift：遍历
来源：http://bgq.gogol.net.cn

for x in a { print(x) }
来源：http://edg.redwolf501.top

[T22] Swift：字典
来源：http://bru.ivvv.top

var d = ["a": 1];  d["b"] = 2
来源：http://jow.tanke756.top

[T23] Swift：函数
来源：http://zxo.cdnleiting.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tka.zhixingplan.top

[T24] Swift：闭包
来源：http://zar.ydzc1.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xql.yj202588.top

[T25] Swift：结构体
来源：http://lyn.xinyue.icu

struct P { var x: Int }
来源：http://aol.dashuyun.cn

[T26] Swift：类与重写
来源：http://ebn.smart0.xyz

class A: Base { override func f() {} }
来源：http://pdw.hcnkem.com

[T27] Swift：错误处理
来源：http://tff.52xcode.cn

do { try f() } catch { print(error) }
来源：http://bbl.guannengcc.top

[T28] Swift：枚举
来源：http://pjc.jinqigfzy.top

enum Color { case red, green }
来源：http://xvs.hnqzz.top

[T29] Swift：guard 提前返回
来源：http://cmi.fktsv.cn

guard let x = opt else { return }
来源：http://zag.sysykeji.top

[T30] Swift：协议
来源：http://ywx.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://rsr.nwbrower.top


<!-- 参考信息 -->