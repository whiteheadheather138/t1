代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kcd.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://rye.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://pjl.shanyushiyangkeji.top

[R31] 局部变量
来源：http://mpg.ydzc1.top

f() { local x=1; echo "$x"; }
来源：http://ulc.redwolf501.top

[R32] 参数个数校验
来源：http://deb.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qcc.sweek.top

[R33] 捕获错误并提示行号
来源：http://iqr.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mgc.fzhhl.top

[R34] 退出时清理
来源：http://aev.sjlbkw.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cry.pycfn.com

[R35] 后台执行并等待
来源：http://kzq.chenzaomai.com

sleep 5 & pid=$!; wait "$pid"
来源：http://mps.jqgfzy.top

[R36] 并发执行多个任务
来源：http://rhz.sjlbkw.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dvo.shzxlz.cn

[R37] 把输出赋给变量
来源：http://dfx.feifeiyinyue.top

files=$(ls -1)
来源：http://qqv.birdmap.top

[R38] 管道串联
来源：http://kvi.quarkkingdee.top

cat a.txt | grep -i error | wc -l
来源：http://jim.shangyingyoupin.top

[R39] 重定向标准输出与错误
来源：http://nds.daxiang520.top

cmd > out.log 2>&1
来源：http://tgl.jiagoushi.top

[R40] 追加写日志
来源：http://htc.xziqi.cn

echo "log" >> out.log
来源：http://pct.daxiang520.top

[R41] 丢弃输出
来源：http://qgt.sufxvd.cn

cmd >/dev/null 2>&1
来源：http://ctd.snrcjt.cn

[R42] 输入重定向
来源：http://mia.aibaodan.cn

wc -l < a.txt
来源：http://vfh.ehwqpu.com

[R43] 按名字查找文件
来源：http://ywp.ppjwa.cn

find . -name "*.log" -type f
来源：http://qnc.sysykeji.top

[R44] 按修改时间查找
来源：http://ikw.fktsv.cn

find . -mtime -7 -type f
来源：http://xlg.zhengqikj.top

[R45] 批量删除
来源：http://ozm.tianlin.xyz

find . -name "*.tmp" -delete
来源：http://mwv.ppjwa.cn

[R46] 递归替换文件内容
来源：http://anr.shzxlz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fos.zhaomingkeji.xyz

[R47] sed 单行替换
来源：http://fsc.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://rza.fengsongda.top

[R48] awk 取指定列
来源：http://cfg.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://cvy.yj20258888.top

[R49] awk 带条件
来源：http://reu.jinqigfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://acj.0kj1m.cn

[R50] awk 求和
来源：http://gtt.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ojv.jiagoushi.top

[R51] 排序去重取前几
来源：http://izs.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kic.hcnkem.com

[R52] 统计行数
来源：http://sxp.jyoumei.cn

wc -l a.txt
来源：http://wni.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://tdh.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gdw.cheryme.top

[R54] 比较两个文件
来源：http://kjh.guannengcc.top

diff a.txt b.txt
来源：http://xde.sufxvd.cn

[R55] 压缩与解压
来源：http://ytr.zhaomingkeji.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fow.yanxiufei.cn

[R56] 远程拷贝
来源：http://vpf.ivvv.top

scp file user@host:/path/
来源：http://mop.yvedp.cn

[R57] 远程执行命令
来源：http://lfj.svipenyu.cn

ssh user@host 'uptime'
来源：http://hjs.quarkkingdee.top

[R58] 下载文件
来源：http://brb.fengsongda.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pgi.yfazqb.com

[R59] 发 POST JSON
来源：http://nbc.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ikb.daria6918.cn

[R60] 只看 HTTP 状态码
来源：http://lpz.ivvv.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yst.fehbvm.com

[R61] 磁盘占用
来源：http://rlb.gaohongyu789.top

df -h;  du -sh *
来源：http://hvn.redwolf501.top

[R62] 找最占空间的文件
来源：http://tlu.jiagoushi.top

du -ah . | sort -rh | head -10
来源：http://iev.c1oappe.top

[R63] 内存与进程
来源：http://eny.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://klt.hongshengwenyu.top

[R64] 结束进程
来源：http://uga.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://sae.jlsjyb.cn

[R65] 查看端口占用
来源：http://uga.hywenlv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://esj.aibaodan.cn

[R66] 定时任务
来源：http://ifx.daria6918.cn

crontab -e;  crontab -l
来源：http://vwl.zycfv.cn

[R67] 生成随机十六进制串
来源：http://dso.fanxiaobao.xyz

openssl rand -hex 16
来源：http://cqn.hywenlv.cn

[R68] 计算文件校验值
来源：http://uny.mhx1999.top

sha256sum a.txt;  md5sum a.txt
来源：http://gfn.meibo888.top

[R69] 生成随机密码
来源：http://yos.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://dau.chenzaomai.com

[R70] 时间戳与互转
来源：http://dja.ybcxt.top

date +%s;  date -d @1700000000
来源：http://tkg.guannengcc.top

[R71] 日期格式化
来源：http://neg.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://igc.guannengcc.top

[R72] 等待端口就绪
来源：http://vcg.316326.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://ilk.c1oappe.top

[R73] 分割大日志
来源：http://dng.gogol.net.cn

split -l 1000 big.log part_
来源：http://qqq.shzxlz.cn

[R74] 批量重命名
来源：http://nuo.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cpi.tian-w.cn

[R75] 导出环境变量
来源：http://bir.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://ryo.guowangkeji.top

[R76] 使用临时文件
来源：http://sjy.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mir.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://oqc.havefunace.top

read -rp "请输入: " ans
来源：http://sqa.vqdsnc.cn

[R78] 交互式菜单
来源：http://ecl.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nhl.dianchejie.cn

[R79] 解析命令行选项
来源：http://xqc.yueranfly.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xoo.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://quv.hammf.cn

time ./run.sh
来源：http://alg.daxiang520.top

================================================================================
来源：http://ikt.bbcook.cn

S. C / C++ 专题
来源：http://rtm.dianchejie.cn

================================================================================
来源：http://fek.xinyue.icu

[S01] C：Hello World
来源：http://kwq.sufxvd.cn

#include <stdio.h>
来源：http://rlv.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jzc.yongpay.top

[S02] C：变量与格式化输出
来源：http://fbt.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://knt.ctjpmb.com

[S03] C：读入整数
来源：http://xzx.0kj1m.cn

int x; scanf("%d", &x);
来源：http://qcq.wangshuangyany.cn

[S04] C：字符串复制
来源：http://bjy.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jho.shuidangran.top

[S05] C：字符串长度
来源：http://udu.tianlin.xyz

strlen(s)
来源：http://mdh.dashuyun.cn

[S06] C：字符串比较
来源：http://jos.xziqi.cn

strcmp(a, b) == 0
来源：http://cpu.shuidangran.top

[S07] C：数组遍历求和
来源：http://jfr.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dkr.quarkkingdee.top

[S08] C：动态内存分配与释放
来源：http://ebw.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xyr.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://arz.havefunace.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://afh.uphjek.com

[S10] C：指针与解引用
来源：http://sri.yvedp.cn

int *p = &a;  *p = 5;
来源：http://fbl.vehdjk.com

[S11] C：逐行读文件
来源：http://axv.pycfn.com

FILE *f = fopen("a.txt", "r");
来源：http://gvz.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qwv.wangshuangyany.cn

fclose(f);
来源：http://nxb.cdnleiting.top

[S12] C：写文件
来源：http://aco.gzhubu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kii.gaohongyu789.top

[S13] C：宏定义
来源：http://qlo.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zxe.uphjek.com

[S14] C：枚举
来源：http://zne.yangfankeji.com

enum Color { RED, GREEN, BLUE };
来源：http://bwv.jinqigufen.top

[S15] C：类型转换
来源：http://zvc.yangfankeji.com

(double) a / b
来源：http://imx.gzhubu.top

[S16] C：位操作置位
来源：http://uhl.feifeiyinyue.top

x |= (1 << 3);
来源：http://hlz.bjfxy.top

[S17] C：安全拼接字符串
来源：http://ewp.vehdjk.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wli.tian-w.cn

[S18] C：命令行参数
来源：http://tbf.hywenlv.cn

int main(int argc, char **argv)
来源：http://tqz.sysykeji.top

[S19] C：快速排序
来源：http://twa.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pqp.gaohongyu789.top

[S20] C：二分查找
来源：http://edp.zycfv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zyq.ivvv.top

[S21] C：字符类别判断
来源：http://psm.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zoz.sufxvd.cn

[S22] C：字符串转数字
来源：http://egy.zhaomingkeji.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://jhc.ctjpmb.com

[S23] C：随机数
来源：http://tga.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bov.yuxming.cn

[S24] C：获取本地时间
来源：http://woe.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sul.dashuyun.cn

[S25] C：内存拷贝
来源：http://hxb.zhijiandao.cn

memcpy(dst, src, n);
来源：http://yoe.meibo888.top

[S26] C：内存清零
来源：http://qii.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://ply.tian-w.cn

[S27] C：定义常量
来源：http://tcc.mhx1999.top

const double PI = 3.14159;
来源：http://nea.quarkkingdee.top

[S28] C：静态变量
来源：http://zxq.wangdashe.top

static int counter = 0;
来源：http://crv.uphjek.com

[S29] C：变参函数
来源：http://dfb.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fiq.zdqjudy.top

[S30] C：头文件保护
来源：http://dyw.tian-w.cn

#ifndef X_H
来源：http://pdr.zhongyouzk.top

#define X_H
来源：http://bkb.ybcxt.top

#endif
来源：http://hkm.hfpthk.cn

[S31] C++：Hello World
来源：http://yjd.zdqjudy.top

#include <iostream>
来源：http://fkz.chenzaomai.com

int main() { std::cout << "Hello\n"; }
来源：http://gfq.dianchejie.cn

[S32] C++：字符串
来源：http://hbj.ydzc1.top

std::string s = "hi";  s += "!";
来源：http://ere.yj20258888.top

[S33] C++：vector 增删
来源：http://rem.tian-w.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uxx.9152youxi.cn

[S34] C++：遍历 vector
来源：http://dvj.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://enw.yvedp.cn

[S35] C++：map
来源：http://sze.cashguo.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ufd.ctjpmb.com

[S36] C++：unordered_map
来源：http://niz.hammf.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bsl.kuanghao11.cn

[S37] C++：set
来源：http://vgf.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ndx.cdnleiting.top

[S38] C++：排序
来源：http://rdy.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://coc.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://dde.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xkj.uphjek.com

[S40] C++：查找元素
来源：http://dxg.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://avj.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://ubk.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rne.tarul.cn

[S42] C++：继承与虚函数
来源：http://ays.sweek.top

class B : public Base { public: void f() override {} };
来源：http://ytl.fengsongda.top

[S43] C++：智能指针
来源：http://tot.chenlongwang.top

auto p = std::make_unique<int>(5);
来源：http://loo.hfpthk.cn

[S44] C++：引用传参
来源：http://zsm.zycfv.cn

void inc(int &x) { ++x; }
来源：http://rkw.yonumen.top

[S45] C++：lambda
来源：http://vro.jyoumei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sgw.yueranfly.top

[S46] C++：函数模板
来源：http://vek.andypj.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nby.zhijiandao.cn

[S47] C++：结构化绑定遍历
来源：http://mvi.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://frg.sxryk.cn

[S48] C++：逐行读文件
来源：http://xyg.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://jjq.316326.xyz

while (std::getline(in, line)) { }
来源：http://scf.hongshengwenyu.top

[S49] C++：写文件
来源：http://gyv.hfpthk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mqc.nwbrower.top

[S50] C++：格式化数字
来源：http://wrb.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yrn.pycfn.com

[S51] C++：显式类型转换
来源：http://dhh.haohaochexian.top

static_cast<double>(a) / b
来源：http://wda.fengsongda.top

[S52] C++：const 与 noexcept
来源：http://lnv.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://nxp.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://gvo.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://yeo.xylfe.cn

[S54] C++：异常处理
来源：http://pvc.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xoy.cucudq.cn

[S55] C++：结构化绑定
来源：http://wxd.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bkb.xylfe.cn

[S56] C++：optional
来源：http://bus.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iwb.sysykeji.top

[S57] C++：编译期常量
来源：http://mfd.iojbl.cn

constexpr int N = 10;
来源：http://lyn.dianchejie.cn

[S58] C++：命名空间
来源：http://kyo.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://msv.shangyingyoupin.top

[S59] C++：静态断言
来源：http://ajm.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://khy.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://syb.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cis.jlsjyb.cn

================================================================================
来源：http://qve.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tza.316326.xyz

================================================================================
来源：http://zns.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://ddp.zhiwuduotai.top

println("Hello")
来源：http://gwo.nanxinkj.top

[T02] Kotlin：变量
来源：http://uyh.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uve.316326.xyz

[T03] Kotlin：字符串模板
来源：http://wme.aizwys.cn

"值: $b"
来源：http://pbx.ybcxt.top

[T04] Kotlin：空安全
来源：http://gqd.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://lec.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://pvp.aizwys.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aei.vqdsnc.cn

[T06] Kotlin：集合映射
来源：http://dru.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://ndc.0kj1m.cn

[T07] Kotlin：集合过滤
来源：http://tlo.hfpthk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cyr.hywenlv.cn

[T08] Kotlin：数据类
来源：http://rqt.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://hro.jianghu66.top

[T09] Kotlin：扩展函数
来源：http://qiq.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://uqm.yueranfly.top

[T10] Kotlin：默认参数
来源：http://zvo.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fvt.fzhhl.top

[T11] Kotlin：协程
来源：http://oij.316326.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://qwc.shangyingyoupin.top

[T12] Kotlin：解构声明
来源：http://agr.hnxiangtu.top

val (a, b) = Pair(1, 2)
来源：http://mey.fktsv.cn

[T13] Kotlin：只读 Map
来源：http://efl.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://rtj.dianchejie.cn

[T14] Kotlin：循环
来源：http://viw.xuetiantiany.cn

for (i in 1..10) println(i)
来源：http://hky.shzxlz.cn

[T15] Kotlin：接口
来源：http://xzz.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://raq.sysykeji.top

[T16] Swift：Hello World
来源：http://hvv.gzhubu.top

print("Hello")
来源：http://axl.snrcjt.cn

[T17] Swift：变量与常量
来源：http://xiu.chenlongwang.top

var a = 1;  let b = 2
来源：http://qmy.shuidangran.top

[T18] Swift：字符串插值
来源：http://pke.uphjek.com

"值: \(b)"
来源：http://vti.pycfn.com

[T19] Swift：可选绑定
来源：http://ott.redwolf501.top

if let n = opt { print(n) }
来源：http://osi.yonumen.top

[T20] Swift：数组操作
来源：http://tyo.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rep.ehwqpu.com

[T21] Swift：遍历
来源：http://ypr.feifeiyinyue.top

for x in a { print(x) }
来源：http://yad.sufxvd.cn

[T22] Swift：字典
来源：http://yui.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://oag.xylfe.cn

[T23] Swift：函数
来源：http://afe.dashuyun.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ppj.jqgfzy.top

[T24] Swift：闭包
来源：http://iek.gotoacloud.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vxm.tianlin.xyz

[T25] Swift：结构体
来源：http://bwp.snrcjt.cn

struct P { var x: Int }
来源：http://etr.jyoumei.cn

[T26] Swift：类与重写
来源：http://vti.fktsv.cn

class A: Base { override func f() {} }
来源：http://esn.jinyuanbaomall.cn

[T27] Swift：错误处理
来源：http://kyh.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://yev.birdmap.top

[T28] Swift：枚举
来源：http://aeb.jlsjyb.cn

enum Color { case red, green }
来源：http://jku.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://edm.wangshuangyany.cn

guard let x = opt else { return }
来源：http://tbk.hongshengwenyu.top

[T30] Swift：协议
来源：http://kts.yj202588.top

protocol Shape { func area() -> Double }
来源：http://xdg.hysaishi.cn

[T31] Lua：Hello World
来源：http://isp.ybcxt.top

print("Hello")
来源：http://viz.mhx1999.top

[T32] Lua：局部变量
来源：http://lfd.vehdjk.com

local a = 1
来源：http://vxw.0kj1m.cn


<!-- 参考信息 -->