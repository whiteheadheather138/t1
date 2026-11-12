代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://qle.quarkkingdee.top

[R26] 命令替换
来源：http://lea.sxryk.cn

now=$(date +%F); echo "$now"
来源：http://era.yangfankeji.com

[R27] 算术展开
来源：http://fuk.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://frj.pengpengdd.cyou

[R28] 浮点运算
来源：http://xff.pycfn.com

echo "scale=2; 10/3" | bc
来源：http://wnm.0kj1m.cn

[R29] 定义函数
来源：http://kil.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gha.cdnleiting.top

[R30] 函数返回状态码
来源：http://qom.tian-w.cn

f() { return 0; }; f || echo "失败了"
来源：http://hyf.cashguo.top

[R31] 局部变量
来源：http://dgj.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://xrr.yj20258.top

[R32] 参数个数校验
来源：http://faq.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dzk.gaohongyu789.top

[R33] 捕获错误并提示行号
来源：http://bzz.zhongyouzk.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nox.fktsv.cn

[R34] 退出时清理
来源：http://mhb.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://txd.cdnleiting.top

[R35] 后台执行并等待
来源：http://tlc.ehwqpu.com

sleep 5 & pid=$!; wait "$pid"
来源：http://wxn.fanxiaobao.xyz

[R36] 并发执行多个任务
来源：http://hpz.tian-w.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xqm.hysaishi.cn

[R37] 把输出赋给变量
来源：http://oas.xziqi.cn

files=$(ls -1)
来源：http://gqp.zhiwuduotai.top

[R38] 管道串联
来源：http://vct.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://lop.dianchejie.cn

[R39] 重定向标准输出与错误
来源：http://phh.zdqjudy.top

cmd > out.log 2>&1
来源：http://vfg.yj20258888.top

[R40] 追加写日志
来源：http://lnz.shzxlz.cn

echo "log" >> out.log
来源：http://vpl.uphjek.com

[R41] 丢弃输出
来源：http://rfq.zdbjq.cn

cmd >/dev/null 2>&1
来源：http://msk.zhaomingkeji.xyz

[R42] 输入重定向
来源：http://dgj.snrcjt.cn

wc -l < a.txt
来源：http://efd.dashuyun.cn

[R43] 按名字查找文件
来源：http://vvz.jinyuanbaomall.cn

find . -name "*.log" -type f
来源：http://cwe.yonumen.top

[R44] 按修改时间查找
来源：http://smf.xinyue.icu

find . -mtime -7 -type f
来源：http://xlz.gaohongyu789.top

[R45] 批量删除
来源：http://rsy.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://rfh.redwolf501.top

[R46] 递归替换文件内容
来源：http://oke.bbcook.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qzu.snrcjt.cn

[R47] sed 单行替换
来源：http://thv.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://dkn.jinqigfzy.top

[R48] awk 取指定列
来源：http://ibg.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://yiz.jianghu66.top

[R49] awk 带条件
来源：http://mwa.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rdy.hcnkem.com

[R50] awk 求和
来源：http://mok.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://gzx.yj20258.top

[R51] 排序去重取前几
来源：http://knv.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://hqd.yangfankeji.com

[R52] 统计行数
来源：http://sny.gogol.net.cn

wc -l a.txt
来源：http://veh.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://tzy.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://orq.sjlbkw.cn

[R54] 比较两个文件
来源：http://spi.ywan-chungtsiang.top

diff a.txt b.txt
来源：http://fyj.316326.xyz

[R55] 压缩与解压
来源：http://duq.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fjb.yuxming.cn

[R56] 远程拷贝
来源：http://lgf.jinyuanbaomall.cn

scp file user@host:/path/
来源：http://knx.sjlbkw.cn

[R57] 远程执行命令
来源：http://ric.kuanghao11.cn

ssh user@host 'uptime'
来源：http://ztt.jinyuanbaomall.cn

[R58] 下载文件
来源：http://nei.fktsv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rjl.yongpay.top

[R59] 发 POST JSON
来源：http://nay.vehdjk.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uzs.fehbvm.com

[R60] 只看 HTTP 状态码
来源：http://xmv.52xcode.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lhv.9152youxi.cn

[R61] 磁盘占用
来源：http://ott.svipenyu.cn

df -h;  du -sh *
来源：http://xbn.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://uqm.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://yhk.zycfv.cn

[R63] 内存与进程
来源：http://fou.zhengqikj.top

free -h;  ps aux | grep nginx
来源：http://ita.shzxlz.cn

[R64] 结束进程
来源：http://rtr.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://sbh.zhiwuduotai.top

[R65] 查看端口占用
来源：http://ydm.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rbj.jinghuilouyu.cn

[R66] 定时任务
来源：http://ucg.cdnleiting.top

crontab -e;  crontab -l
来源：http://hwd.zhengqikj.top

[R67] 生成随机十六进制串
来源：http://rzi.epnwcf.com

openssl rand -hex 16
来源：http://yzn.c1oappe.top

[R68] 计算文件校验值
来源：http://kxg.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nqc.cashguo.top

[R69] 生成随机密码
来源：http://qjn.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://dot.xinyue.icu

[R70] 时间戳与互转
来源：http://mdo.bbcook.cn

date +%s;  date -d @1700000000
来源：http://qxb.dianchejie.cn

[R71] 日期格式化
来源：http://yuc.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://iya.shangyingyoupin.top

[R72] 等待端口就绪
来源：http://efp.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mog.xuetiantiany.cn

[R73] 分割大日志
来源：http://txp.epnwcf.com

split -l 1000 big.log part_
来源：http://bsq.pycfn.com

[R74] 批量重命名
来源：http://puf.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qxj.guannengcc.top

[R75] 导出环境变量
来源：http://lgb.gotoacloud.top

export PATH="$HOME/bin:$PATH"
来源：http://ufb.yangfankeji.com

[R76] 使用临时文件
来源：http://ezu.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ovt.yfazqb.com

[R77] 读取用户输入
来源：http://ayr.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://rub.yongpay.top

[R78] 交互式菜单
来源：http://pwr.nanxinkj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rwg.vehdjk.com

[R79] 解析命令行选项
来源：http://mtl.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://edp.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://afl.yj20258888.top

time ./run.sh
来源：http://jow.snrcjt.cn

================================================================================
来源：http://oki.jinqigfzy.top

S. C / C++ 专题
来源：http://sci.smart0.xyz

================================================================================
来源：http://ugh.cashguo.top

[S01] C：Hello World
来源：http://vnn.shanyushiyangtech.top

#include <stdio.h>
来源：http://tri.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xys.jqgufenzy.top

[S02] C：变量与格式化输出
来源：http://smi.ctjpmb.com

int a = 10; printf("%d\n", a);
来源：http://kpb.ehwqpu.com

[S03] C：读入整数
来源：http://yrj.epnwcf.com

int x; scanf("%d", &x);
来源：http://oul.sjlbkw.cn

[S04] C：字符串复制
来源：http://ugl.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://lmu.jyoumei.cn

[S05] C：字符串长度
来源：http://jqn.shangyingyoupin.top

strlen(s)
来源：http://vvv.bjfxy.top

[S06] C：字符串比较
来源：http://mxh.xylfe.cn

strcmp(a, b) == 0
来源：http://gci.dashuyun.cn

[S07] C：数组遍历求和
来源：http://aes.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fvi.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://sgm.guannengcc.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kwj.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://voj.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lbn.dashuyun.cn

[S10] C：指针与解引用
来源：http://neh.svipenyu.cn

int *p = &a;  *p = 5;
来源：http://vap.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://wao.snrcjt.cn

FILE *f = fopen("a.txt", "r");
来源：http://mon.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://erg.chenzaomai.com

fclose(f);
来源：http://cng.jinyuanbaomall.cn

[S12] C：写文件
来源：http://lwp.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wky.yuanzhike.top

[S13] C：宏定义
来源：http://sau.zdqjudy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lbw.jqgufenzy.top

[S14] C：枚举
来源：http://vdc.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://umo.dianchejie.cn

[S15] C：类型转换
来源：http://zfi.iojbl.cn

(double) a / b
来源：http://ctg.jiagoushi.top

[S16] C：位操作置位
来源：http://kjy.jinghuilouyu.cn

x |= (1 << 3);
来源：http://bpp.hywenlv.cn

[S17] C：安全拼接字符串
来源：http://bea.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pdo.cdnleiting.top

[S18] C：命令行参数
来源：http://jhh.cashguo.top

int main(int argc, char **argv)
来源：http://led.vqdsnc.cn

[S19] C：快速排序
来源：http://flv.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://yox.haohaochexian.top

[S20] C：二分查找
来源：http://wem.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cnu.hnxiangtu.top

[S21] C：字符类别判断
来源：http://bdr.zhiwuduotai.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xth.hesvh.cn

[S22] C：字符串转数字
来源：http://mnz.pycfn.com

atoi("42");  strtod("3.14", NULL);
来源：http://tpr.yvedp.cn

[S23] C：随机数
来源：http://vrn.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qmz.sxryk.cn

[S24] C：获取本地时间
来源：http://ijj.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pmx.jqgfzy.top

[S25] C：内存拷贝
来源：http://wtx.andypj.xyz

memcpy(dst, src, n);
来源：http://qgb.zdbjq.cn

[S26] C：内存清零
来源：http://xfw.hnxiangtu.top

memset(a, 0, sizeof a);
来源：http://nsv.sxryk.cn

[S27] C：定义常量
来源：http://npm.shuidangran.top

const double PI = 3.14159;
来源：http://cek.hnqzz.top

[S28] C：静态变量
来源：http://qmw.316326.xyz

static int counter = 0;
来源：http://bcl.meibo888.top

[S29] C：变参函数
来源：http://tev.vqdsnc.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zuh.yvedp.cn

[S30] C：头文件保护
来源：http://mlo.zycfv.cn

#ifndef X_H
来源：http://jjw.yj20258.top

#define X_H
来源：http://tjs.gotoacloud.top

#endif
来源：http://auv.fanxiaobao.xyz

[S31] C++：Hello World
来源：http://qja.zhoulong.xyz

#include <iostream>
来源：http://vso.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://qos.ybcxt.top

[S32] C++：字符串
来源：http://nsr.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://sla.snrcjt.cn

[S33] C++：vector 增删
来源：http://zks.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kst.meibo888.top

[S34] C++：遍历 vector
来源：http://dyx.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://pyh.xziqi.cn

[S35] C++：map
来源：http://eow.ydjk.org.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://arp.zhengqikj.top

[S36] C++：unordered_map
来源：http://qsh.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xot.cdnleiting.top

[S37] C++：set
来源：http://ddy.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://anv.fanxiaobao.xyz

[S38] C++：排序
来源：http://ufz.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://aod.yj20258.top

[S39] C++：自定义比较器排序
来源：http://goe.zhongyouzk.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rrs.mhx1999.top

[S40] C++：查找元素
来源：http://hfk.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://btu.xuanzx.com

[S41] C++：类与构造函数
来源：http://abc.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://edn.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://wdg.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://hkn.hnxiangtu.top

[S43] C++：智能指针
来源：http://wyz.c1oappe.top

auto p = std::make_unique<int>(5);
来源：http://zio.shzxlz.cn

[S44] C++：引用传参
来源：http://hzu.gotoacloud.top

void inc(int &x) { ++x; }
来源：http://lty.gzhubu.top

[S45] C++：lambda
来源：http://paa.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://dks.xziqi.cn

[S46] C++：函数模板
来源：http://zwt.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hss.chenjidiqi.icu

[S47] C++：结构化绑定遍历
来源：http://sks.xinyue.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xkx.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://zen.smart0.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://idu.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://ssk.hfpthk.cn

[S49] C++：写文件
来源：http://cyg.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yuv.snrcjt.cn

[S50] C++：格式化数字
来源：http://kfh.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://szj.chenlongwang.top

[S51] C++：显式类型转换
来源：http://vxs.gogol.net.cn

static_cast<double>(a) / b
来源：http://xfz.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://ybf.wangshuangyany.cn

int size() const noexcept { return n_; }
来源：http://kez.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://xyr.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://lmu.yfazqb.com

[S54] C++：异常处理
来源：http://iye.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tek.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://apy.hnxiangtu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://muy.uphjek.com

[S56] C++：optional
来源：http://bki.shangyingyoupin.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wjt.zhijiandao.cn

[S57] C++：编译期常量
来源：http://lqd.tanke756.top

constexpr int N = 10;
来源：http://eph.mhx1999.top

[S58] C++：命名空间
来源：http://jgo.gzhubu.top

namespace ns { int f() { return 1; } }
来源：http://rxt.sxryk.cn

[S59] C++：静态断言
来源：http://lte.tian-w.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dhv.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://cug.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rad.shangyingyoupin.top

================================================================================
来源：http://rtv.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vev.9152youxi.cn

================================================================================
来源：http://xhj.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://eis.tarul.cn

println("Hello")
来源：http://ies.ybcxt.top

[T02] Kotlin：变量
来源：http://ywj.nanxuanxn.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://foh.ywan-chungtsiang.top

[T03] Kotlin：字符串模板
来源：http://ehj.pycfn.com

"值: $b"
来源：http://xow.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://djy.uphjek.com

val n: String? = null;  n?.length
来源：http://pfv.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://uky.52xcode.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ukz.chenjidiqi.icu

[T06] Kotlin：集合映射
来源：http://jcj.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mad.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://nbm.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xga.hfpthk.cn

[T08] Kotlin：数据类
来源：http://bch.wangdashe.top

data class User(val name: String, val age: Int)
来源：http://uuq.yj20258.top

[T09] Kotlin：扩展函数
来源：http://ikw.guowangkeji.top

fun String.exclaim() = this + "!"
来源：http://fdi.mhx1999.top

[T10] Kotlin：默认参数
来源：http://hfs.xuetiantiany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tsx.9152youxi.cn

[T11] Kotlin：协程
来源：http://mif.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://omn.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://bdo.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://boy.andypj.xyz

[T13] Kotlin：只读 Map
来源：http://upe.andypj.xyz

val m = mapOf("a" to 1)
来源：http://ymf.ydjk.org.cn

[T14] Kotlin：循环
来源：http://kcz.fzhhl.top

for (i in 1..10) println(i)
来源：http://zlf.ydjk.org.cn

[T15] Kotlin：接口
来源：http://buf.9152youxi.cn

interface Shape { fun area(): Double }
来源：http://zvs.pengpengdd.cyou

[T16] Swift：Hello World
来源：http://oea.sxryk.cn

print("Hello")
来源：http://amb.hysaishi.cn

[T17] Swift：变量与常量
来源：http://aqw.316326.xyz

var a = 1;  let b = 2
来源：http://ngl.dianchejie.cn

[T18] Swift：字符串插值
来源：http://ptm.ywan-chungtsiang.top

"值: \(b)"
来源：http://xsl.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://zqa.fzhhl.top

if let n = opt { print(n) }
来源：http://sbq.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://oxh.guannengcc.top

var a = [1, 2, 3];  a.append(4)
来源：http://vco.smart0.xyz

[T21] Swift：遍历
来源：http://hij.vehdjk.com

for x in a { print(x) }
来源：http://kxg.vqdsnc.cn

[T22] Swift：字典
来源：http://phx.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://wou.xziqi.cn

[T23] Swift：函数
来源：http://qun.chenjidiqi.icu

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xbq.guannengcc.top

[T24] Swift：闭包
来源：http://tqr.xziqi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://skd.cqqwz.cn

[T25] Swift：结构体
来源：http://amd.guowangkeji.top

struct P { var x: Int }
来源：http://nio.hammf.cn

[T26] Swift：类与重写
来源：http://srb.tianlin.xyz

class A: Base { override func f() {} }
来源：http://peo.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://eas.fehbvm.com

do { try f() } catch { print(error) }
来源：http://buw.316326.xyz

[T28] Swift：枚举
来源：http://zac.ctjpmb.com

enum Color { case red, green }
来源：http://erc.sxryk.cn


<!-- 参考信息 -->