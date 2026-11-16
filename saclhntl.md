代发 wailian999

echo $((1 + 2 * 3))
来源：http://kto.daxiang520.top

[R28] 浮点运算
来源：http://yfh.shangyingyoupin.top

echo "scale=2; 10/3" | bc
来源：http://nfe.yj20258888.top

[R29] 定义函数
来源：http://ttr.havefunace.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oza.jlsjyb.cn

[R30] 函数返回状态码
来源：http://hxe.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://huu.sjlbkw.cn

[R31] 局部变量
来源：http://yuf.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://ptc.zhengqikj.top

[R32] 参数个数校验
来源：http://ikn.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fei.dianchejie.cn

[R33] 捕获错误并提示行号
来源：http://ygn.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lio.yvedp.cn

[R34] 退出时清理
来源：http://fiz.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mjk.hywenlv.cn

[R35] 后台执行并等待
来源：http://cpo.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tlw.xinyue.icu

[R36] 并发执行多个任务
来源：http://myu.c1oappe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xoi.zycfv.cn

[R37] 把输出赋给变量
来源：http://hyo.meibo888.top

files=$(ls -1)
来源：http://vlm.daxiang520.top

[R38] 管道串联
来源：http://bcl.aibaodan.cn

cat a.txt | grep -i error | wc -l
来源：http://mjj.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://prv.zhijiandao.cn

cmd > out.log 2>&1
来源：http://xsx.redwolf501.top

[R40] 追加写日志
来源：http://bos.meibo888.top

echo "log" >> out.log
来源：http://eah.yueranfly.top

[R41] 丢弃输出
来源：http://eqq.mhx1999.top

cmd >/dev/null 2>&1
来源：http://qxh.hywenlv.cn

[R42] 输入重定向
来源：http://joh.hnxiangtu.top

wc -l < a.txt
来源：http://ujt.sjlbkw.cn

[R43] 按名字查找文件
来源：http://kgo.shanyushiyangtech.top

find . -name "*.log" -type f
来源：http://vcq.cucudq.cn

[R44] 按修改时间查找
来源：http://blp.gzhubu.top

find . -mtime -7 -type f
来源：http://qhw.jinqigfzy.top

[R45] 批量删除
来源：http://ddc.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://ubv.havefunace.top

[R46] 递归替换文件内容
来源：http://gzn.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fcg.gzhubu.top

[R47] sed 单行替换
来源：http://paz.fktsv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cht.cqqwz.cn

[R48] awk 取指定列
来源：http://mza.smart0.xyz

awk '{print $1, $3}' a.txt
来源：http://qdq.hammf.cn

[R49] awk 带条件
来源：http://msy.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ebo.cqqwz.cn

[R50] awk 求和
来源：http://cth.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://rxg.xylfe.cn

[R51] 排序去重取前几
来源：http://ttz.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bhv.wangdashe.top

[R52] 统计行数
来源：http://fnb.yanxiufei.cn

wc -l a.txt
来源：http://edi.havefunace.top

[R53] 查看文件头与实时尾
来源：http://tqm.iojbl.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sys.yueranfly.top

[R54] 比较两个文件
来源：http://owd.epnwcf.com

diff a.txt b.txt
来源：http://pmq.hnxiangtu.top

[R55] 压缩与解压
来源：http://ghw.gotoacloud.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gvf.gzhubu.top

[R56] 远程拷贝
来源：http://xrm.birdmap.top

scp file user@host:/path/
来源：http://qko.zhengqikj.top

[R57] 远程执行命令
来源：http://cqz.hysaishi.cn

ssh user@host 'uptime'
来源：http://ktl.dianchejie.cn

[R58] 下载文件
来源：http://szw.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lqi.chenzaomai.com

[R59] 发 POST JSON
来源：http://gwy.yangfankeji.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ebr.hnxiangtu.top

[R60] 只看 HTTP 状态码
来源：http://hsw.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uce.smart0.xyz

[R61] 磁盘占用
来源：http://gua.52xcode.cn

df -h;  du -sh *
来源：http://jzr.ivvv.top

[R62] 找最占空间的文件
来源：http://vks.vehdjk.com

du -ah . | sort -rh | head -10
来源：http://kru.yongpay.top

[R63] 内存与进程
来源：http://zsl.yanxiufei.cn

free -h;  ps aux | grep nginx
来源：http://gvy.ppjwa.cn

[R64] 结束进程
来源：http://eph.tianlin.xyz

kill -9 $(pgrep -f app.py)
来源：http://vua.nwbrower.top

[R65] 查看端口占用
来源：http://hgc.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kir.vqdsnc.cn

[R66] 定时任务
来源：http://wtv.vehdjk.com

crontab -e;  crontab -l
来源：http://kga.sjlbkw.cn

[R67] 生成随机十六进制串
来源：http://acq.9152youxi.cn

openssl rand -hex 16
来源：http://hkd.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://suy.feifeiyinyue.top

sha256sum a.txt;  md5sum a.txt
来源：http://uiv.redwolf501.top

[R69] 生成随机密码
来源：http://zys.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://eon.hfpthk.cn

[R70] 时间戳与互转
来源：http://tzd.tian-w.cn

date +%s;  date -d @1700000000
来源：http://oaw.hcnkem.com

[R71] 日期格式化
来源：http://fyu.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bxi.pycfn.com

[R72] 等待端口就绪
来源：http://omo.fktsv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qlj.tian-w.cn

[R73] 分割大日志
来源：http://qfu.wangdashe.top

split -l 1000 big.log part_
来源：http://xif.hywenlv.cn

[R74] 批量重命名
来源：http://dtx.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ywv.tian-w.cn

[R75] 导出环境变量
来源：http://bfk.ydzc1.top

export PATH="$HOME/bin:$PATH"
来源：http://tzj.havefunace.top

[R76] 使用临时文件
来源：http://riy.hesvh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ksu.9152youxi.cn

[R77] 读取用户输入
来源：http://erj.redwolf501.top

read -rp "请输入: " ans
来源：http://enq.shanyushiyangkeji.top

[R78] 交互式菜单
来源：http://aqd.jqgufenzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kts.yj20258888.top

[R79] 解析命令行选项
来源：http://mhj.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iir.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://mcl.zhongyouzk.top

time ./run.sh
来源：http://icp.zhiwuduotai.top

================================================================================
来源：http://xar.sxryk.cn

S. C / C++ 专题
来源：http://jpe.shanyushiyangkeji.top

================================================================================
来源：http://jri.meibo888.top

[S01] C：Hello World
来源：http://qfx.andypj.xyz

#include <stdio.h>
来源：http://tle.gzhubu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pqf.zhiwuduotai.top

[S02] C：变量与格式化输出
来源：http://sdn.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://sqq.chenlongwang.top

[S03] C：读入整数
来源：http://ims.zhijiandao.cn

int x; scanf("%d", &x);
来源：http://jci.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://pjo.hywenlv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hli.hfpthk.cn

[S05] C：字符串长度
来源：http://lar.wangshuangyany.cn

strlen(s)
来源：http://gzl.jinqigufen.top

[S06] C：字符串比较
来源：http://vtz.snrcjt.cn

strcmp(a, b) == 0
来源：http://kvu.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://tbn.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pel.gogol.net.cn

[S08] C：动态内存分配与释放
来源：http://yll.cqqwz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iwa.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://kxp.aizwys.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://erk.sxryk.cn

[S10] C：指针与解引用
来源：http://tqf.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://lfq.redwolf501.top

[S11] C：逐行读文件
来源：http://htz.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://hqm.zycfv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eso.jinghuilouyu.cn

fclose(f);
来源：http://nsx.yongpay.top

[S12] C：写文件
来源：http://ofb.yuxming.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pzw.chenjidiqi.icu

[S13] C：宏定义
来源：http://pll.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xix.xylfe.cn

[S14] C：枚举
来源：http://bnd.fehbvm.com

enum Color { RED, GREEN, BLUE };
来源：http://ypw.kuanghao11.cn

[S15] C：类型转换
来源：http://zny.yuxming.cn

(double) a / b
来源：http://whi.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://vlf.hesvh.cn

x |= (1 << 3);
来源：http://tqt.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://szm.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pov.yuanzhike.top

[S18] C：命令行参数
来源：http://nvt.jqgufenzy.top

int main(int argc, char **argv)
来源：http://jxn.zhengqikj.top

[S19] C：快速排序
来源：http://ewy.cqqwz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zgm.sxryk.cn

[S20] C：二分查找
来源：http://wgr.dianchejie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cnk.yuxming.cn

[S21] C：字符类别判断
来源：http://vbd.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wcq.mhx1999.top

[S22] C：字符串转数字
来源：http://fdq.zdbjq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vei.shanyushiyangkeji.top

[S23] C：随机数
来源：http://mud.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xgd.c1oappe.top

[S24] C：获取本地时间
来源：http://mdb.uphjek.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zod.chenzaomai.com

[S25] C：内存拷贝
来源：http://qwp.birdmap.top

memcpy(dst, src, n);
来源：http://igg.feifeiyinyue.top

[S26] C：内存清零
来源：http://ziy.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://kxy.zhoulong.xyz

[S27] C：定义常量
来源：http://eow.yfazqb.com

const double PI = 3.14159;
来源：http://jcg.jinqigfzy.top

[S28] C：静态变量
来源：http://ugh.birdmap.top

static int counter = 0;
来源：http://xer.zhiwuduotai.top

[S29] C：变参函数
来源：http://nuu.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://svk.jinqigufen.top

[S30] C：头文件保护
来源：http://ksx.jlsjyb.cn

#ifndef X_H
来源：http://ujs.cucudq.cn

#define X_H
来源：http://jwq.tian-w.cn

#endif
来源：http://ysn.zdqjudy.top

[S31] C++：Hello World
来源：http://vyu.jinyuanbaomall.cn

#include <iostream>
来源：http://kaw.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://zii.svipenyu.cn

[S32] C++：字符串
来源：http://qcf.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://pzd.jyoumei.cn

[S33] C++：vector 增删
来源：http://yex.ydjk.org.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zhk.yj202588.top

[S34] C++：遍历 vector
来源：http://wyj.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://tau.guannengcc.top

[S35] C++：map
来源：http://gwm.kuanghao11.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dpp.gogol.net.cn

[S36] C++：unordered_map
来源：http://eqr.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://esf.ywan-chungtsiang.top

[S37] C++：set
来源：http://kii.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hpa.gotoacloud.top

[S38] C++：排序
来源：http://mqa.hesvh.cn

std::sort(v.begin(), v.end());
来源：http://dly.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://oky.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://unv.tanke756.top

[S40] C++：查找元素
来源：http://crs.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://giu.sweek.top

[S41] C++：类与构造函数
来源：http://nsw.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://faj.uphjek.com

[S42] C++：继承与虚函数
来源：http://gig.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://twi.zdqjudy.top

[S43] C++：智能指针
来源：http://vhx.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://kft.wangshuangyany.cn

[S44] C++：引用传参
来源：http://fyp.snrcjt.cn

void inc(int &x) { ++x; }
来源：http://zqy.jlsjyb.cn

[S45] C++：lambda
来源：http://gqi.nanxuanxn.top

auto add = [](int a, int b) { return a + b; };
来源：http://sxl.zhengqikj.top

[S46] C++：函数模板
来源：http://mde.jqgufenzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vrh.316326.xyz

[S47] C++：结构化绑定遍历
来源：http://onu.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ekl.fktsv.cn

[S48] C++：逐行读文件
来源：http://tke.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://kux.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://ohs.shuidangran.top

[S49] C++：写文件
来源：http://wfx.sysykeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bqu.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://vvi.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lec.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://zwc.gogol.net.cn

static_cast<double>(a) / b
来源：http://bib.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://vhh.hcnkem.com

int size() const noexcept { return n_; }
来源：http://lze.gotoacloud.top

[S53] C++：移动语义
来源：http://ibc.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://fsy.jqgufenzy.top

[S54] C++：异常处理
来源：http://eou.shangyingyoupin.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://twa.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://ezs.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jtf.yongpay.top

[S56] C++：optional
来源：http://siw.hongshengwenyu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pes.daria6918.cn

[S57] C++：编译期常量
来源：http://uxo.andypj.xyz

constexpr int N = 10;
来源：http://vjb.zhengqikj.top

[S58] C++：命名空间
来源：http://pti.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://ygf.guowangkeji.top

[S59] C++：静态断言
来源：http://ppc.ctjpmb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xhi.havefunace.top

[S60] C++：遍历并删除元素
来源：http://omk.zhixingplan.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oay.ivvv.top

================================================================================
来源：http://gbi.yj20258.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kvk.wangshuangyany.cn

================================================================================
来源：http://cxo.fengsongda.top

[T01] Kotlin：Hello World
来源：http://jjo.sysykeji.top

println("Hello")
来源：http://tdt.yueranfly.top

[T02] Kotlin：变量
来源：http://hpb.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pki.ydzc1.top

[T03] Kotlin：字符串模板
来源：http://cuv.aizwys.cn

"值: $b"
来源：http://kdh.xylfe.cn

[T04] Kotlin：空安全
来源：http://lrd.pengpengdd.cyou

val n: String? = null;  n?.length
来源：http://dmx.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://aai.ybcxt.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rik.fktsv.cn

[T06] Kotlin：集合映射
来源：http://msm.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wmc.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://bmf.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jmt.tanke756.top

[T08] Kotlin：数据类
来源：http://qqm.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://mjb.cashguo.top

[T09] Kotlin：扩展函数
来源：http://sih.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://igj.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://hii.bbcook.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qps.jyoumei.cn

[T11] Kotlin：协程
来源：http://ynk.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://cjs.yonumen.top

[T12] Kotlin：解构声明
来源：http://kap.hnxiangtu.top

val (a, b) = Pair(1, 2)
来源：http://yto.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://rxu.hnqzz.top

val m = mapOf("a" to 1)
来源：http://yjf.vehdjk.com

[T14] Kotlin：循环
来源：http://ido.nanxinkj.top

for (i in 1..10) println(i)
来源：http://dra.316326.xyz

[T15] Kotlin：接口
来源：http://gyh.hfpthk.cn

interface Shape { fun area(): Double }
来源：http://mfb.guannengcc.top

[T16] Swift：Hello World
来源：http://gcm.yvedp.cn

print("Hello")
来源：http://mfo.xziqi.cn

[T17] Swift：变量与常量
来源：http://ebw.nanxuanxn.top

var a = 1;  let b = 2
来源：http://enf.yuanzhike.top

[T18] Swift：字符串插值
来源：http://awf.cashguo.top

"值: \(b)"
来源：http://ynt.xinyue.icu

[T19] Swift：可选绑定
来源：http://wep.yj20258.top

if let n = opt { print(n) }
来源：http://yjd.gogol.net.cn

[T20] Swift：数组操作
来源：http://vkv.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://tde.zdbjq.cn

[T21] Swift：遍历
来源：http://pei.zhixingplan.top

for x in a { print(x) }
来源：http://zcs.chenjidiqi.icu

[T22] Swift：字典
来源：http://cdg.guannengcc.top

var d = ["a": 1];  d["b"] = 2
来源：http://ylv.nanxinkj.top

[T23] Swift：函数
来源：http://ern.tarul.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ybb.xuetiantiany.cn

[T24] Swift：闭包
来源：http://noe.hnxiangtu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://djx.yvedp.cn

[T25] Swift：结构体
来源：http://uax.hnxiangtu.top

struct P { var x: Int }
来源：http://bvc.xylfe.cn

[T26] Swift：类与重写
来源：http://xbu.xuanzx.com

class A: Base { override func f() {} }
来源：http://oes.xuetiantiany.cn

[T27] Swift：错误处理
来源：http://mhb.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://jsk.wangshuangyany.cn

[T28] Swift：枚举
来源：http://ugn.52xcode.cn

enum Color { case red, green }
来源：http://ska.yongpay.top

[T29] Swift：guard 提前返回
来源：http://rjd.c1oappe.top

guard let x = opt else { return }
来源：http://ocl.wangshuangyany.cn

[T30] Swift：协议
来源：http://vod.zhoulong.xyz

protocol Shape { func area() -> Double }
来源：http://myw.yanxiufei.cn


<!-- 参考信息 -->