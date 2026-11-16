代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://gfa.hfpthk.cn

[R26] 命令替换
来源：http://xjt.cdnleiting.top

now=$(date +%F); echo "$now"
来源：http://huq.bjfxy.top

[R27] 算术展开
来源：http://kim.tian-w.cn

echo $((1 + 2 * 3))
来源：http://lov.smart0.xyz

[R28] 浮点运算
来源：http://sft.cheryme.top

echo "scale=2; 10/3" | bc
来源：http://dff.jianghu66.top

[R29] 定义函数
来源：http://alu.chenjidiqi.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sbo.cashguo.top

[R30] 函数返回状态码
来源：http://teq.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://dvs.pengpengdd.cyou

[R31] 局部变量
来源：http://ymr.vqdsnc.cn

f() { local x=1; echo "$x"; }
来源：http://elw.yuxming.cn

[R32] 参数个数校验
来源：http://rau.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lqj.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://ghi.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nwx.52xcode.cn

[R34] 退出时清理
来源：http://ybr.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://kry.jlsjyb.cn

[R35] 后台执行并等待
来源：http://ehe.redwolf501.top

sleep 5 & pid=$!; wait "$pid"
来源：http://sfh.xinyue.icu

[R36] 并发执行多个任务
来源：http://orf.zhiwuduotai.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mrb.mhx1999.top

[R37] 把输出赋给变量
来源：http://ktd.jiagoushi.top

files=$(ls -1)
来源：http://leu.bbcook.cn

[R38] 管道串联
来源：http://fyv.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://jtj.nwbrower.top

[R39] 重定向标准输出与错误
来源：http://mbu.sufxvd.cn

cmd > out.log 2>&1
来源：http://vfz.guannengcc.top

[R40] 追加写日志
来源：http://oiv.0kj1m.cn

echo "log" >> out.log
来源：http://wwc.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://vmy.shuidangran.top

cmd >/dev/null 2>&1
来源：http://anc.316326.xyz

[R42] 输入重定向
来源：http://iuo.birdmap.top

wc -l < a.txt
来源：http://cdj.ivvv.top

[R43] 按名字查找文件
来源：http://ksx.fktsv.cn

find . -name "*.log" -type f
来源：http://tdw.ydzc1.top

[R44] 按修改时间查找
来源：http://fph.nanxinkj.top

find . -mtime -7 -type f
来源：http://kfr.yfazqb.com

[R45] 批量删除
来源：http://gwr.fengsongda.top

find . -name "*.tmp" -delete
来源：http://wkj.xylfe.cn

[R46] 递归替换文件内容
来源：http://pil.ctjpmb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jii.redwolf501.top

[R47] sed 单行替换
来源：http://gun.yuxming.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pak.sjlbkw.cn

[R48] awk 取指定列
来源：http://xkf.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://vve.jqgfzy.top

[R49] awk 带条件
来源：http://prl.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tuf.epnwcf.com

[R50] awk 求和
来源：http://gty.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://gof.ivvv.top

[R51] 排序去重取前几
来源：http://vdy.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gkb.shuidangran.top

[R52] 统计行数
来源：http://zap.guannengcc.top

wc -l a.txt
来源：http://jlg.birdmap.top

[R53] 查看文件头与实时尾
来源：http://iob.hcnkem.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mds.tian-w.cn

[R54] 比较两个文件
来源：http://azh.ctjpmb.com

diff a.txt b.txt
来源：http://wdq.jiagoushi.top

[R55] 压缩与解压
来源：http://odq.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rcs.jinyuanbaomall.cn

[R56] 远程拷贝
来源：http://rhp.xinyue.icu

scp file user@host:/path/
来源：http://trs.zhengqikj.top

[R57] 远程执行命令
来源：http://mnx.tarul.cn

ssh user@host 'uptime'
来源：http://tyv.epnwcf.com

[R58] 下载文件
来源：http://bky.smart0.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dff.52xcode.cn

[R59] 发 POST JSON
来源：http://dem.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pjt.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://qxl.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kbg.yangfankeji.com

[R61] 磁盘占用
来源：http://ffr.ydjk.org.cn

df -h;  du -sh *
来源：http://zkh.dianchejie.cn

[R62] 找最占空间的文件
来源：http://giv.fktsv.cn

du -ah . | sort -rh | head -10
来源：http://kbi.haohaochexian.top

[R63] 内存与进程
来源：http://zdf.hammf.cn

free -h;  ps aux | grep nginx
来源：http://dof.tianlin.xyz

[R64] 结束进程
来源：http://our.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://ith.yuanzhike.top

[R65] 查看端口占用
来源：http://yds.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mfm.zdbjq.cn

[R66] 定时任务
来源：http://txk.havefunace.top

crontab -e;  crontab -l
来源：http://eri.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://zhz.zhoulong.xyz

openssl rand -hex 16
来源：http://rix.zhijiandao.cn

[R68] 计算文件校验值
来源：http://aln.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bgu.fengsongda.top

[R69] 生成随机密码
来源：http://ngb.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://ibf.dashuyun.cn

[R70] 时间戳与互转
来源：http://ezz.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://kga.pycfn.com

[R71] 日期格式化
来源：http://yjm.yangfankeji.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://dix.ivvv.top

[R72] 等待端口就绪
来源：http://zgm.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fjl.ydzc1.top

[R73] 分割大日志
来源：http://qmy.wangdashe.top

split -l 1000 big.log part_
来源：http://ktu.xuetiantiany.cn

[R74] 批量重命名
来源：http://iuf.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://clv.sysykeji.top

[R75] 导出环境变量
来源：http://svk.dashuyun.cn

export PATH="$HOME/bin:$PATH"
来源：http://shj.smart0.xyz

[R76] 使用临时文件
来源：http://zxw.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://buo.gaohongyu789.top

[R77] 读取用户输入
来源：http://hyd.nanxinkj.top

read -rp "请输入: " ans
来源：http://mtv.gotoacloud.top

[R78] 交互式菜单
来源：http://zni.zhongyouzk.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gan.aizwys.cn

[R79] 解析命令行选项
来源：http://xrc.yanxiufei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://owp.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://rxb.guannengcc.top

time ./run.sh
来源：http://dtj.hfpthk.cn

================================================================================
来源：http://nms.hnqzz.top

S. C / C++ 专题
来源：http://ppt.fzhhl.top

================================================================================
来源：http://hux.sweek.top

[S01] C：Hello World
来源：http://tly.fengsongda.top

#include <stdio.h>
来源：http://kom.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sts.ivvv.top

[S02] C：变量与格式化输出
来源：http://ddb.birdmap.top

int a = 10; printf("%d\n", a);
来源：http://qfj.guowangkeji.top

[S03] C：读入整数
来源：http://aqq.daxiang520.top

int x; scanf("%d", &x);
来源：http://oyt.zhijiandao.cn

[S04] C：字符串复制
来源：http://daj.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pyb.shanyushiyangkeji.top

[S05] C：字符串长度
来源：http://uyg.mhx1999.top

strlen(s)
来源：http://dwi.hammf.cn

[S06] C：字符串比较
来源：http://jls.ivvv.top

strcmp(a, b) == 0
来源：http://gzu.vqdsnc.cn

[S07] C：数组遍历求和
来源：http://fcr.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vqf.birdmap.top

[S08] C：动态内存分配与释放
来源：http://avj.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nmb.yonumen.top

[S09] C：结构体定义与初始化
来源：http://lco.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mad.ehwqpu.com

[S10] C：指针与解引用
来源：http://ngd.ybcxt.top

int *p = &a;  *p = 5;
来源：http://sqk.shuidangran.top

[S11] C：逐行读文件
来源：http://eii.tian-w.cn

FILE *f = fopen("a.txt", "r");
来源：http://hgd.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://swi.shanyushiyangtech.top

fclose(f);
来源：http://hnt.haohaochexian.top

[S12] C：写文件
来源：http://bgp.pycfn.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://piz.nanxinkj.top

[S13] C：宏定义
来源：http://jvp.gaohongyu789.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zay.yanxiufei.cn

[S14] C：枚举
来源：http://mec.redwolf501.top

enum Color { RED, GREEN, BLUE };
来源：http://rpr.chenjidiqi.icu

[S15] C：类型转换
来源：http://sql.jyoumei.cn

(double) a / b
来源：http://hpg.tian-w.cn

[S16] C：位操作置位
来源：http://jkq.0kj1m.cn

x |= (1 << 3);
来源：http://ukq.vehdjk.com

[S17] C：安全拼接字符串
来源：http://fob.jqgfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xxe.vehdjk.com

[S18] C：命令行参数
来源：http://rlu.cucudq.cn

int main(int argc, char **argv)
来源：http://sfd.fanxiaobao.xyz

[S19] C：快速排序
来源：http://seh.hywenlv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vrk.fengsongda.top

[S20] C：二分查找
来源：http://hiw.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zow.nwbrower.top

[S21] C：字符类别判断
来源：http://yjt.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xzw.iojbl.cn

[S22] C：字符串转数字
来源：http://tij.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gxe.vqdsnc.cn

[S23] C：随机数
来源：http://xqc.feifeiyinyue.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pyk.shuidangran.top

[S24] C：获取本地时间
来源：http://bxl.hysaishi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jbh.sxryk.cn

[S25] C：内存拷贝
来源：http://psn.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://nbx.sjlbkw.cn

[S26] C：内存清零
来源：http://has.andypj.xyz

memset(a, 0, sizeof a);
来源：http://ote.ydjk.org.cn

[S27] C：定义常量
来源：http://zue.hammf.cn

const double PI = 3.14159;
来源：http://ron.yvedp.cn

[S28] C：静态变量
来源：http://uxp.mhx1999.top

static int counter = 0;
来源：http://uea.wangdashe.top

[S29] C：变参函数
来源：http://exq.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hal.sweek.top

[S30] C：头文件保护
来源：http://nrk.cashguo.top

#ifndef X_H
来源：http://kph.chenjidiqi.icu

#define X_H
来源：http://avh.gogol.net.cn

#endif
来源：http://ydq.jinqigfzy.top

[S31] C++：Hello World
来源：http://lts.chenlongwang.top

#include <iostream>
来源：http://lsa.xinyue.icu

int main() { std::cout << "Hello\n"; }
来源：http://lpj.cashguo.top

[S32] C++：字符串
来源：http://ice.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://gno.jqgfzy.top

[S33] C++：vector 增删
来源：http://oah.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aav.sxryk.cn

[S34] C++：遍历 vector
来源：http://gea.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://mrg.hfpthk.cn

[S35] C++：map
来源：http://mdm.vqdsnc.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://exy.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://bhy.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://erb.sufxvd.cn

[S37] C++：set
来源：http://omc.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lif.fzhhl.top

[S38] C++：排序
来源：http://lap.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://yvt.zdqjudy.top

[S39] C++：自定义比较器排序
来源：http://ips.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qck.yueranfly.top

[S40] C++：查找元素
来源：http://cqx.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://waw.bbcook.cn

[S41] C++：类与构造函数
来源：http://lny.hfpthk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://osg.tarul.cn

[S42] C++：继承与虚函数
来源：http://beg.ppjwa.cn

class B : public Base { public: void f() override {} };
来源：http://qjs.fktsv.cn

[S43] C++：智能指针
来源：http://ekl.fzhhl.top

auto p = std::make_unique<int>(5);
来源：http://mfq.shangyingyoupin.top

[S44] C++：引用传参
来源：http://glu.yj20258.top

void inc(int &x) { ++x; }
来源：http://msp.ydzc1.top

[S45] C++：lambda
来源：http://pjj.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://mrg.meibo888.top

[S46] C++：函数模板
来源：http://qjv.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mrt.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://qcz.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ndy.aibaodan.cn

[S48] C++：逐行读文件
来源：http://hui.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://myv.uphjek.com

while (std::getline(in, line)) { }
来源：http://sdi.kuanghao11.cn

[S49] C++：写文件
来源：http://sek.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vgc.yangfankeji.com

[S50] C++：格式化数字
来源：http://jyj.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rnv.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://qdq.gzhubu.top

static_cast<double>(a) / b
来源：http://mms.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://rfn.yonumen.top

int size() const noexcept { return n_; }
来源：http://gkf.wangshuangyany.cn

[S53] C++：移动语义
来源：http://dgw.yonumen.top

std::vector<int> w = std::move(v);
来源：http://mte.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://muk.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rcm.zdbjq.cn

[S55] C++：结构化绑定
来源：http://jfg.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ipr.jqgfzy.top

[S56] C++：optional
来源：http://khz.hcnkem.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wxo.bjfxy.top

[S57] C++：编译期常量
来源：http://kra.hysaishi.cn

constexpr int N = 10;
来源：http://djw.cqqwz.cn

[S58] C++：命名空间
来源：http://isc.jinqigufen.top

namespace ns { int f() { return 1; } }
来源：http://tlx.yj202588.top

[S59] C++：静态断言
来源：http://dks.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qlz.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://qfl.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sfr.yonumen.top

================================================================================
来源：http://wol.xingfuxueyuan.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ugs.9152youxi.cn

================================================================================
来源：http://iay.gzhubu.top

[T01] Kotlin：Hello World
来源：http://icl.52xcode.cn

println("Hello")
来源：http://sko.sjlbkw.cn

[T02] Kotlin：变量
来源：http://zfk.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vbk.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://ojx.jqgfzy.top

"值: $b"
来源：http://nxm.redwolf501.top

[T04] Kotlin：空安全
来源：http://zov.shanyushiyangtech.top

val n: String? = null;  n?.length
来源：http://qvk.nanxuanxn.top

[T05] Kotlin：when 表达式
来源：http://aqv.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mbj.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://ucj.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tsp.xinyue.icu

[T07] Kotlin：集合过滤
来源：http://ojn.vehdjk.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://tnd.fengsongda.top

[T08] Kotlin：数据类
来源：http://gap.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://cbx.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://ihw.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://dux.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://yil.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bpo.daxiang520.top

[T11] Kotlin：协程
来源：http://eyc.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kqd.ppjwa.cn

[T12] Kotlin：解构声明
来源：http://pnt.kuanghao11.cn

val (a, b) = Pair(1, 2)
来源：http://ved.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://grc.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://wbr.ydjk.org.cn

[T14] Kotlin：循环
来源：http://vbb.jiagoushi.top

for (i in 1..10) println(i)
来源：http://aik.daxiang520.top

[T15] Kotlin：接口
来源：http://kmm.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://ejp.guannengcc.top

[T16] Swift：Hello World
来源：http://urx.vqdsnc.cn

print("Hello")
来源：http://cjv.jinqigfzy.top

[T17] Swift：变量与常量
来源：http://agg.yonumen.top

var a = 1;  let b = 2
来源：http://ayv.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://pjf.andypj.xyz

"值: \(b)"
来源：http://ako.daxiang520.top

[T19] Swift：可选绑定
来源：http://kqm.andypj.xyz

if let n = opt { print(n) }
来源：http://gam.jianghu66.top

[T20] Swift：数组操作
来源：http://ijk.fanxiaobao.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://auz.hfpthk.cn

[T21] Swift：遍历
来源：http://lus.hnxiangtu.top

for x in a { print(x) }
来源：http://fss.daxiang520.top

[T22] Swift：字典
来源：http://qck.pycfn.com

var d = ["a": 1];  d["b"] = 2
来源：http://ltb.tianlin.xyz

[T23] Swift：函数
来源：http://lqt.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://biv.cashguo.top

[T24] Swift：闭包
来源：http://qrd.xinyue.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://kbt.zhijiandao.cn

[T25] Swift：结构体
来源：http://inn.daria6918.cn

struct P { var x: Int }
来源：http://unx.havefunace.top

[T26] Swift：类与重写
来源：http://reh.quarkkingdee.top

class A: Base { override func f() {} }
来源：http://aog.zhoulong.xyz

[T27] Swift：错误处理
来源：http://ebm.hcnkem.com

do { try f() } catch { print(error) }
来源：http://gvw.chenjidiqi.icu

[T28] Swift：枚举
来源：http://nnv.yangfankeji.com

enum Color { case red, green }
来源：http://qlk.52xcode.cn


<!-- 参考信息 -->