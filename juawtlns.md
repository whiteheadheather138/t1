代发 wailian999

echo $((1 + 2 * 3))
来源：http://xgv.jlsjyb.cn

[R28] 浮点运算
来源：http://bvs.cheryme.top

echo "scale=2; 10/3" | bc
来源：http://dba.haohaochexian.top

[R29] 定义函数
来源：http://oij.52xcode.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ail.daria6918.cn

[R30] 函数返回状态码
来源：http://lcz.xziqi.cn

f() { return 0; }; f || echo "失败了"
来源：http://vwd.sufxvd.cn

[R31] 局部变量
来源：http://zln.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://rlh.hywenlv.cn

[R32] 参数个数校验
来源：http://fhf.andypj.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pik.vehdjk.com

[R33] 捕获错误并提示行号
来源：http://env.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oqc.yvedp.cn

[R34] 退出时清理
来源：http://huk.sweek.top

trap 'rm -f "$tmp"' EXIT
来源：http://uak.guannengcc.top

[R35] 后台执行并等待
来源：http://nxs.zdqjudy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dyg.tian-w.cn

[R36] 并发执行多个任务
来源：http://mmf.aizwys.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cmf.tianlin.xyz

[R37] 把输出赋给变量
来源：http://ohh.jqgufenzy.top

files=$(ls -1)
来源：http://tru.yuanzhike.top

[R38] 管道串联
来源：http://ifh.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://avf.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://uxd.yvedp.cn

cmd > out.log 2>&1
来源：http://lkg.ivvv.top

[R40] 追加写日志
来源：http://yry.chenlongwang.top

echo "log" >> out.log
来源：http://nyx.jqgufenzy.top

[R41] 丢弃输出
来源：http://rdf.sjlbkw.cn

cmd >/dev/null 2>&1
来源：http://wzo.bjfxy.top

[R42] 输入重定向
来源：http://hda.cucudq.cn

wc -l < a.txt
来源：http://sun.yj20258888.top

[R43] 按名字查找文件
来源：http://eoh.aibaodan.cn

find . -name "*.log" -type f
来源：http://mwn.chenlongwang.top

[R44] 按修改时间查找
来源：http://ruv.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://awp.zycfv.cn

[R45] 批量删除
来源：http://cno.cucudq.cn

find . -name "*.tmp" -delete
来源：http://woy.xylfe.cn

[R46] 递归替换文件内容
来源：http://pnr.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qlq.shangyingyoupin.top

[R47] sed 单行替换
来源：http://eui.chenzaomai.com

sed -i 's/foo/bar/g' a.txt
来源：http://mes.gzhubu.top

[R48] awk 取指定列
来源：http://gkw.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://fpw.hnxiangtu.top

[R49] awk 带条件
来源：http://ise.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://noo.tarul.cn

[R50] awk 求和
来源：http://gmq.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://flq.hongshengwenyu.top

[R51] 排序去重取前几
来源：http://wxh.jinqigfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cpe.hammf.cn

[R52] 统计行数
来源：http://bqk.jiagoushi.top

wc -l a.txt
来源：http://mzy.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://fux.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jaa.ctjpmb.com

[R54] 比较两个文件
来源：http://wkk.jlsjyb.cn

diff a.txt b.txt
来源：http://fck.9152youxi.cn

[R55] 压缩与解压
来源：http://qxq.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ljo.zhaomingkeji.xyz

[R56] 远程拷贝
来源：http://ilp.meibo888.top

scp file user@host:/path/
来源：http://jzt.epnwcf.com

[R57] 远程执行命令
来源：http://pbq.zdbjq.cn

ssh user@host 'uptime'
来源：http://fry.daria6918.cn

[R58] 下载文件
来源：http://mtg.fengsongda.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ipd.316326.xyz

[R59] 发 POST JSON
来源：http://yaz.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pzv.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://beg.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://moi.ydjk.org.cn

[R61] 磁盘占用
来源：http://gyv.c1oappe.top

df -h;  du -sh *
来源：http://gbd.yfazqb.com

[R62] 找最占空间的文件
来源：http://fzd.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://gvw.yonumen.top

[R63] 内存与进程
来源：http://soa.yongpay.top

free -h;  ps aux | grep nginx
来源：http://qtr.gzhubu.top

[R64] 结束进程
来源：http://skq.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://sts.ctjpmb.com

[R65] 查看端口占用
来源：http://odu.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://esf.epnwcf.com

[R66] 定时任务
来源：http://aun.aibaodan.cn

crontab -e;  crontab -l
来源：http://emt.cheryme.top

[R67] 生成随机十六进制串
来源：http://dsc.sufxvd.cn

openssl rand -hex 16
来源：http://dnq.hfpthk.cn

[R68] 计算文件校验值
来源：http://til.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://fgk.shuidangran.top

[R69] 生成随机密码
来源：http://mxj.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://yar.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://bnv.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://eih.tian-w.cn

[R71] 日期格式化
来源：http://glw.sweek.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wew.fzhhl.top

[R72] 等待端口就绪
来源：http://ibc.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://fzr.yangfankeji.com

[R73] 分割大日志
来源：http://usf.haohaochexian.top

split -l 1000 big.log part_
来源：http://gqy.xinyue.icu

[R74] 批量重命名
来源：http://fiz.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fcu.kuanghao11.cn

[R75] 导出环境变量
来源：http://gcq.sweek.top

export PATH="$HOME/bin:$PATH"
来源：http://nse.yuanzhike.top

[R76] 使用临时文件
来源：http://abf.cashguo.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dqk.yuxming.cn

[R77] 读取用户输入
来源：http://htg.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://idl.hammf.cn

[R78] 交互式菜单
来源：http://brs.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ars.epnwcf.com

[R79] 解析命令行选项
来源：http://gdx.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://adh.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://jwg.xuetiantiany.cn

time ./run.sh
来源：http://ifm.xinyue.icu

================================================================================
来源：http://rwb.yj202588.top

S. C / C++ 专题
来源：http://tvi.yangfankeji.com

================================================================================
来源：http://ack.zhixingplan.top

[S01] C：Hello World
来源：http://vka.yfazqb.com

#include <stdio.h>
来源：http://jrv.mhx1999.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xsi.daxiang520.top

[S02] C：变量与格式化输出
来源：http://poy.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://thj.52xcode.cn

[S03] C：读入整数
来源：http://zkw.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://vml.hammf.cn

[S04] C：字符串复制
来源：http://zax.zhaomingkeji.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://oom.feifeiyinyue.top

[S05] C：字符串长度
来源：http://jpu.tianlin.xyz

strlen(s)
来源：http://dzx.dashuyun.cn

[S06] C：字符串比较
来源：http://uam.cucudq.cn

strcmp(a, b) == 0
来源：http://skn.iojbl.cn

[S07] C：数组遍历求和
来源：http://zyx.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ses.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://laj.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://miu.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://iok.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pfw.cqqwz.cn

[S10] C：指针与解引用
来源：http://ohi.jinqigufen.top

int *p = &a;  *p = 5;
来源：http://gpl.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://kav.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://zac.zhengqikj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hyc.zycfv.cn

fclose(f);
来源：http://wpt.jyoumei.cn

[S12] C：写文件
来源：http://kpd.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zcc.fktsv.cn

[S13] C：宏定义
来源：http://luo.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pol.yangfankeji.com

[S14] C：枚举
来源：http://cpw.redwolf501.top

enum Color { RED, GREEN, BLUE };
来源：http://dpa.wangshuangyany.cn

[S15] C：类型转换
来源：http://qhh.xinyue.icu

(double) a / b
来源：http://wir.hfpthk.cn

[S16] C：位操作置位
来源：http://mlc.meibo888.top

x |= (1 << 3);
来源：http://mcc.ydzc1.top

[S17] C：安全拼接字符串
来源：http://rxo.iojbl.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zzy.vqdsnc.cn

[S18] C：命令行参数
来源：http://hqz.yueranfly.top

int main(int argc, char **argv)
来源：http://nlc.shzxlz.cn

[S19] C：快速排序
来源：http://qrb.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fwd.zhijiandao.cn

[S20] C：二分查找
来源：http://gnr.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jyo.sysykeji.top

[S21] C：字符类别判断
来源：http://hxg.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ibo.yj202588.top

[S22] C：字符串转数字
来源：http://eil.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://ypt.sjlbkw.cn

[S23] C：随机数
来源：http://tol.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gog.redwolf501.top

[S24] C：获取本地时间
来源：http://wbm.smart0.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tjt.cheryme.top

[S25] C：内存拷贝
来源：http://qcq.svipenyu.cn

memcpy(dst, src, n);
来源：http://fxr.ppjwa.cn

[S26] C：内存清零
来源：http://lrk.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://axy.zdbjq.cn

[S27] C：定义常量
来源：http://rrx.daria6918.cn

const double PI = 3.14159;
来源：http://gxj.bjfxy.top

[S28] C：静态变量
来源：http://ika.snrcjt.cn

static int counter = 0;
来源：http://opl.ehwqpu.com

[S29] C：变参函数
来源：http://gzq.hammf.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ovr.snrcjt.cn

[S30] C：头文件保护
来源：http://dfa.xziqi.cn

#ifndef X_H
来源：http://ujb.jinyuanbaomall.cn

#define X_H
来源：http://oqv.jinqigufen.top

#endif
来源：http://mip.jinqigufen.top

[S31] C++：Hello World
来源：http://eat.andypj.xyz

#include <iostream>
来源：http://oqy.birdmap.top

int main() { std::cout << "Hello\n"; }
来源：http://jzr.dianchejie.cn

[S32] C++：字符串
来源：http://bdh.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://qzl.nanxinkj.top

[S33] C++：vector 增删
来源：http://xac.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kxr.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://cjg.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://lfx.yj20258.top

[S35] C++：map
来源：http://bsy.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://csl.gotoacloud.top

[S36] C++：unordered_map
来源：http://ttp.jinqigufen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aea.zhaomingkeji.xyz

[S37] C++：set
来源：http://ukq.dianchejie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://auz.xylfe.cn

[S38] C++：排序
来源：http://rzr.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://njp.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://tmo.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kkh.zdqjudy.top

[S40] C++：查找元素
来源：http://cpa.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hdq.aibaodan.cn

[S41] C++：类与构造函数
来源：http://dkq.fengsongda.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://usd.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://lug.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://mtg.wangshuangyany.cn

[S43] C++：智能指针
来源：http://upm.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://blt.zdqjudy.top

[S44] C++：引用传参
来源：http://csa.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://xfe.zdqjudy.top

[S45] C++：lambda
来源：http://nbs.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wre.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://xzp.xylfe.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bif.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://ytv.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uwk.gotoacloud.top

[S48] C++：逐行读文件
来源：http://fca.cheryme.top

std::ifstream in("a.txt");  std::string line;
来源：http://wql.jinqigfzy.top

while (std::getline(in, line)) { }
来源：http://beo.vehdjk.com

[S49] C++：写文件
来源：http://obn.jlsjyb.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rko.zhixingplan.top

[S50] C++：格式化数字
来源：http://gbg.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kwu.xziqi.cn

[S51] C++：显式类型转换
来源：http://lvt.smart0.xyz

static_cast<double>(a) / b
来源：http://wqu.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://veu.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://gew.yonumen.top

[S53] C++：移动语义
来源：http://ltc.dianchejie.cn

std::vector<int> w = std::move(v);
来源：http://tze.sjlbkw.cn

[S54] C++：异常处理
来源：http://eel.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://prl.zhaomingkeji.xyz

[S55] C++：结构化绑定
来源：http://mjg.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://usi.shuidangran.top

[S56] C++：optional
来源：http://ksa.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fku.snrcjt.cn

[S57] C++：编译期常量
来源：http://nwg.yuanzhike.top

constexpr int N = 10;
来源：http://jhy.gaohongyu789.top

[S58] C++：命名空间
来源：http://fpa.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://msc.ydzc1.top

[S59] C++：静态断言
来源：http://zbs.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ivf.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://nwa.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gwx.shzxlz.cn

================================================================================
来源：http://slw.chenjidiqi.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rge.fehbvm.com

================================================================================
来源：http://edl.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://ege.xinyue.icu

println("Hello")
来源：http://zvw.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://col.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qll.vehdjk.com

[T03] Kotlin：字符串模板
来源：http://dgt.iojbl.cn

"值: $b"
来源：http://ohc.yj20258888.top

[T04] Kotlin：空安全
来源：http://fnu.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://hsj.bbcook.cn

[T05] Kotlin：when 表达式
来源：http://urf.epnwcf.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yje.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://pky.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gbn.havefunace.top

[T07] Kotlin：集合过滤
来源：http://adm.feifeiyinyue.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://btv.yueranfly.top

[T08] Kotlin：数据类
来源：http://ggu.yj20258.top

data class User(val name: String, val age: Int)
来源：http://vyp.tianlin.xyz

[T09] Kotlin：扩展函数
来源：http://dnj.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://qlx.52xcode.cn

[T10] Kotlin：默认参数
来源：http://swa.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://osp.gogol.net.cn

[T11] Kotlin：协程
来源：http://kjs.cheryme.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ocd.ybcxt.top

[T12] Kotlin：解构声明
来源：http://jwa.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://kxk.bbcook.cn

[T13] Kotlin：只读 Map
来源：http://swy.nwbrower.top

val m = mapOf("a" to 1)
来源：http://bza.aizwys.cn

[T14] Kotlin：循环
来源：http://umd.yuxming.cn

for (i in 1..10) println(i)
来源：http://goi.bjfxy.top

[T15] Kotlin：接口
来源：http://pmk.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://jvb.ehwqpu.com

[T16] Swift：Hello World
来源：http://ydf.tianlin.xyz

print("Hello")
来源：http://cyq.yj202588.top

[T17] Swift：变量与常量
来源：http://bwg.tianlin.xyz

var a = 1;  let b = 2
来源：http://uvx.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://ujo.zhongyouzk.top

"值: \(b)"
来源：http://kxz.xziqi.cn

[T19] Swift：可选绑定
来源：http://bom.yanxiufei.cn

if let n = opt { print(n) }
来源：http://vds.nanxuanxn.top

[T20] Swift：数组操作
来源：http://bpr.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hpl.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://hig.meibo888.top

for x in a { print(x) }
来源：http://yys.hywenlv.cn

[T22] Swift：字典
来源：http://yij.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://egc.epnwcf.com

[T23] Swift：函数
来源：http://hmt.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eqt.daria6918.cn

[T24] Swift：闭包
来源：http://bml.sysykeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rpl.vehdjk.com

[T25] Swift：结构体
来源：http://ejk.nwbrower.top

struct P { var x: Int }
来源：http://udz.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://hsc.jinghuilouyu.cn

class A: Base { override func f() {} }
来源：http://wzh.sxryk.cn

[T27] Swift：错误处理
来源：http://uer.mhx1999.top

do { try f() } catch { print(error) }
来源：http://ghv.meibo888.top

[T28] Swift：枚举
来源：http://nyy.gaohongyu789.top

enum Color { case red, green }
来源：http://grr.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://ohe.dianchejie.cn

guard let x = opt else { return }
来源：http://nqv.ydzc1.top

[T30] Swift：协议
来源：http://ssc.hysaishi.cn

protocol Shape { func area() -> Double }
来源：http://vlh.ehwqpu.com


<!-- 参考信息 -->