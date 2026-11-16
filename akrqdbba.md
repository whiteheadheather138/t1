代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://dwo.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://lks.epnwcf.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iyw.zhijiandao.cn

[R33] 捕获错误并提示行号
来源：http://hre.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gza.xziqi.cn

[R34] 退出时清理
来源：http://oqg.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://qks.pycfn.com

[R35] 后台执行并等待
来源：http://lez.birdmap.top

sleep 5 & pid=$!; wait "$pid"
来源：http://cso.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://gmg.52xcode.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kgu.0kj1m.cn

[R37] 把输出赋给变量
来源：http://rua.0kj1m.cn

files=$(ls -1)
来源：http://wry.wangshuangyany.cn

[R38] 管道串联
来源：http://efg.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://qea.jqgufenzy.top

[R39] 重定向标准输出与错误
来源：http://meb.nanxinkj.top

cmd > out.log 2>&1
来源：http://fph.fzhhl.top

[R40] 追加写日志
来源：http://mvx.jlsjyb.cn

echo "log" >> out.log
来源：http://irc.iojbl.cn

[R41] 丢弃输出
来源：http://yto.9152youxi.cn

cmd >/dev/null 2>&1
来源：http://nhc.sysykeji.top

[R42] 输入重定向
来源：http://hmz.fengsongda.top

wc -l < a.txt
来源：http://lqx.xylfe.cn

[R43] 按名字查找文件
来源：http://gta.cheryme.top

find . -name "*.log" -type f
来源：http://pwj.hysaishi.cn

[R44] 按修改时间查找
来源：http://mox.zhixingplan.top

find . -mtime -7 -type f
来源：http://pha.bjfxy.top

[R45] 批量删除
来源：http://ymd.xziqi.cn

find . -name "*.tmp" -delete
来源：http://dce.0kj1m.cn

[R46] 递归替换文件内容
来源：http://ehl.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://psn.feifeiyinyue.top

[R47] sed 单行替换
来源：http://wpe.hesvh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vvv.yonumen.top

[R48] awk 取指定列
来源：http://vbt.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://yma.jinghuilouyu.cn

[R49] awk 带条件
来源：http://gbv.chenjidiqi.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dxe.yonumen.top

[R50] awk 求和
来源：http://yqo.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://nsn.xziqi.cn

[R51] 排序去重取前几
来源：http://mdq.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gdk.chenjidiqi.icu

[R52] 统计行数
来源：http://ckc.cqqwz.cn

wc -l a.txt
来源：http://eff.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://sva.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://amd.vqdsnc.cn

[R54] 比较两个文件
来源：http://nte.xuanzx.com

diff a.txt b.txt
来源：http://qvk.hywenlv.cn

[R55] 压缩与解压
来源：http://wyl.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://muy.cqqwz.cn

[R56] 远程拷贝
来源：http://mjk.9152youxi.cn

scp file user@host:/path/
来源：http://xwn.jiagoushi.top

[R57] 远程执行命令
来源：http://qid.jqgfzy.top

ssh user@host 'uptime'
来源：http://zkd.aizwys.cn

[R58] 下载文件
来源：http://mpe.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ttd.sufxvd.cn

[R59] 发 POST JSON
来源：http://rca.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jup.jianghu66.top

[R60] 只看 HTTP 状态码
来源：http://glc.ydzc1.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nvh.sjlbkw.cn

[R61] 磁盘占用
来源：http://kmc.hongshengwenyu.top

df -h;  du -sh *
来源：http://pml.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://cwc.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://pjk.aizwys.cn

[R63] 内存与进程
来源：http://tds.tarul.cn

free -h;  ps aux | grep nginx
来源：http://lxu.hnxiangtu.top

[R64] 结束进程
来源：http://toa.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://qpv.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://nno.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gcs.hnxiangtu.top

[R66] 定时任务
来源：http://fao.zhongyouzk.top

crontab -e;  crontab -l
来源：http://hrg.cucudq.cn

[R67] 生成随机十六进制串
来源：http://jhz.zhixingplan.top

openssl rand -hex 16
来源：http://mvx.gotoacloud.top

[R68] 计算文件校验值
来源：http://axe.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://fyl.tianlin.xyz

[R69] 生成随机密码
来源：http://unl.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://lkm.yuxming.cn

[R70] 时间戳与互转
来源：http://czm.guowangkeji.top

date +%s;  date -d @1700000000
来源：http://bfj.cqqwz.cn

[R71] 日期格式化
来源：http://ogf.fanxiaobao.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://hmu.ydjk.org.cn

[R72] 等待端口就绪
来源：http://kqk.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tnj.xingfuxueyuan.xyz

[R73] 分割大日志
来源：http://omu.jqgfzy.top

split -l 1000 big.log part_
来源：http://bxc.fengsongda.top

[R74] 批量重命名
来源：http://dny.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mvd.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://xlh.ydzc1.top

export PATH="$HOME/bin:$PATH"
来源：http://yxo.smart0.xyz

[R76] 使用临时文件
来源：http://gvb.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kbj.ydjk.org.cn

[R77] 读取用户输入
来源：http://vps.zhixingplan.top

read -rp "请输入: " ans
来源：http://pvv.mhx1999.top

[R78] 交互式菜单
来源：http://hnz.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://kqy.ivvv.top

[R79] 解析命令行选项
来源：http://sgp.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bgm.zhixingplan.top

[R80] 查看脚本执行耗时
来源：http://gna.chenjidiqi.icu

time ./run.sh
来源：http://xrs.zdbjq.cn

================================================================================
来源：http://cpl.smart0.xyz

S. C / C++ 专题
来源：http://wcc.zdqjudy.top

================================================================================
来源：http://syb.hysaishi.cn

[S01] C：Hello World
来源：http://fjx.pengpengdd.cyou

#include <stdio.h>
来源：http://ejo.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://isu.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://pvs.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://rkb.tian-w.cn

[S03] C：读入整数
来源：http://byu.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://mez.zhijiandao.cn

[S04] C：字符串复制
来源：http://inl.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pld.ehwqpu.com

[S05] C：字符串长度
来源：http://bhy.zhijiandao.cn

strlen(s)
来源：http://ikx.zhongyouzk.top

[S06] C：字符串比较
来源：http://prr.ehwqpu.com

strcmp(a, b) == 0
来源：http://nnj.jinghuilouyu.cn

[S07] C：数组遍历求和
来源：http://yzu.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iuo.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://gkk.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://usq.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://nin.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://flk.tianlin.xyz

[S10] C：指针与解引用
来源：http://kwy.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://zsj.c1oappe.top

[S11] C：逐行读文件
来源：http://vpe.yj202588.top

FILE *f = fopen("a.txt", "r");
来源：http://pqy.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pxc.jianghu66.top

fclose(f);
来源：http://gxt.fktsv.cn

[S12] C：写文件
来源：http://qtw.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jvd.vqdsnc.cn

[S13] C：宏定义
来源：http://rrf.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://osy.ivvv.top

[S14] C：枚举
来源：http://ywk.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://iwz.zhongyouzk.top

[S15] C：类型转换
来源：http://iva.dianchejie.cn

(double) a / b
来源：http://zzm.yvedp.cn

[S16] C：位操作置位
来源：http://wth.xziqi.cn

x |= (1 << 3);
来源：http://xgl.jyoumei.cn

[S17] C：安全拼接字符串
来源：http://ziy.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nko.zhijiandao.cn

[S18] C：命令行参数
来源：http://xli.cqqwz.cn

int main(int argc, char **argv)
来源：http://dqw.shanyushiyangtech.top

[S19] C：快速排序
来源：http://xwz.cucudq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wlw.guannengcc.top

[S20] C：二分查找
来源：http://yvm.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jgd.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://cde.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://enu.ehwqpu.com

[S22] C：字符串转数字
来源：http://gez.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://oex.nwbrower.top

[S23] C：随机数
来源：http://cpk.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vda.jinqigufen.top

[S24] C：获取本地时间
来源：http://amj.cheryme.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fcg.52xcode.cn

[S25] C：内存拷贝
来源：http://bpb.yuxming.cn

memcpy(dst, src, n);
来源：http://nhp.birdmap.top

[S26] C：内存清零
来源：http://geg.fanxiaobao.xyz

memset(a, 0, sizeof a);
来源：http://hjy.yuanzhike.top

[S27] C：定义常量
来源：http://voy.xingfuxueyuan.xyz

const double PI = 3.14159;
来源：http://zqx.wangdashe.top

[S28] C：静态变量
来源：http://vjb.vehdjk.com

static int counter = 0;
来源：http://auv.ctjpmb.com

[S29] C：变参函数
来源：http://bkj.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zpb.svipenyu.cn

[S30] C：头文件保护
来源：http://dfa.pengpengdd.cyou

#ifndef X_H
来源：http://lfo.vehdjk.com

#define X_H
来源：http://lwq.yj202588.top

#endif
来源：http://vpp.zhixingplan.top

[S31] C++：Hello World
来源：http://wvm.zdbjq.cn

#include <iostream>
来源：http://flz.yj20258888.top

int main() { std::cout << "Hello\n"; }
来源：http://lnp.316326.xyz

[S32] C++：字符串
来源：http://roo.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://ljd.hysaishi.cn

[S33] C++：vector 增删
来源：http://gfw.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zek.hesvh.cn

[S34] C++：遍历 vector
来源：http://zfb.jinqigfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://yis.bjfxy.top

[S35] C++：map
来源：http://dal.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://prz.gotoacloud.top

[S36] C++：unordered_map
来源：http://zqb.jinyuanbaomall.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gut.zdbjq.cn

[S37] C++：set
来源：http://jei.yangfankeji.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rgh.xuetiantiany.cn

[S38] C++：排序
来源：http://mvn.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://idp.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://rbb.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kht.daxiang520.top

[S40] C++：查找元素
来源：http://hei.hysaishi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fpl.52xcode.cn

[S41] C++：类与构造函数
来源：http://wsr.hfpthk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://slj.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://vcy.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://atr.shangyingyoupin.top

[S43] C++：智能指针
来源：http://ziu.yueranfly.top

auto p = std::make_unique<int>(5);
来源：http://pds.tian-w.cn

[S44] C++：引用传参
来源：http://hjz.hnxiangtu.top

void inc(int &x) { ++x; }
来源：http://lmf.sxryk.cn

[S45] C++：lambda
来源：http://ijq.fanxiaobao.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://euf.shanyushiyangtech.top

[S46] C++：函数模板
来源：http://uhh.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gtf.yuanzhike.top

[S47] C++：结构化绑定遍历
来源：http://itm.quarkkingdee.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://scs.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://ygx.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ctm.hammf.cn

while (std::getline(in, line)) { }
来源：http://kar.jqgfzy.top

[S49] C++：写文件
来源：http://qri.9152youxi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zuy.jqgfzy.top

[S50] C++：格式化数字
来源：http://pke.9152youxi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eyp.xuetiantiany.cn

[S51] C++：显式类型转换
来源：http://imr.gogol.net.cn

static_cast<double>(a) / b
来源：http://tqb.ctjpmb.com

[S52] C++：const 与 noexcept
来源：http://sjz.xuanzx.com

int size() const noexcept { return n_; }
来源：http://rht.zdbjq.cn

[S53] C++：移动语义
来源：http://wiq.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://hgy.mhx1999.top

[S54] C++：异常处理
来源：http://vhd.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lro.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://fdj.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pkf.bjfxy.top

[S56] C++：optional
来源：http://ppc.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zex.yfazqb.com

[S57] C++：编译期常量
来源：http://ulv.meibo888.top

constexpr int N = 10;
来源：http://vgn.jiagoushi.top

[S58] C++：命名空间
来源：http://vif.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://gff.xylfe.cn

[S59] C++：静态断言
来源：http://hxh.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wtd.ehwqpu.com

[S60] C++：遍历并删除元素
来源：http://wyv.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ohz.yonumen.top

================================================================================
来源：http://zpd.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pgy.dashuyun.cn

================================================================================
来源：http://ucx.iojbl.cn

[T01] Kotlin：Hello World
来源：http://jsc.shuidangran.top

println("Hello")
来源：http://vee.vqdsnc.cn

[T02] Kotlin：变量
来源：http://hzr.yuanzhike.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://egp.ivvv.top

[T03] Kotlin：字符串模板
来源：http://igd.chenlongwang.top

"值: $b"
来源：http://zoo.zhijiandao.cn

[T04] Kotlin：空安全
来源：http://azl.shangyingyoupin.top

val n: String? = null;  n?.length
来源：http://nzr.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://ess.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uhp.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://min.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mrc.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://qtc.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://cri.shzxlz.cn

[T08] Kotlin：数据类
来源：http://lpc.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://exe.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://zxl.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://oye.jianghu66.top

[T10] Kotlin：默认参数
来源：http://smy.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dhb.sysykeji.top

[T11] Kotlin：协程
来源：http://ile.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qvs.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://yjw.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://nfs.jinghuilouyu.cn

[T13] Kotlin：只读 Map
来源：http://ncu.ydzc1.top

val m = mapOf("a" to 1)
来源：http://agi.ywan-chungtsiang.top

[T14] Kotlin：循环
来源：http://bpq.tianlin.xyz

for (i in 1..10) println(i)
来源：http://ivn.ivvv.top

[T15] Kotlin：接口
来源：http://ivm.jiagoushi.top

interface Shape { fun area(): Double }
来源：http://tnq.fengsongda.top

[T16] Swift：Hello World
来源：http://rfi.gogol.net.cn

print("Hello")
来源：http://awe.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://hde.uphjek.com

var a = 1;  let b = 2
来源：http://qhf.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://gnb.jyoumei.cn

"值: \(b)"
来源：http://kki.shuidangran.top

[T19] Swift：可选绑定
来源：http://nly.zhengqikj.top

if let n = opt { print(n) }
来源：http://cgs.gzhubu.top

[T20] Swift：数组操作
来源：http://zbs.hcnkem.com

var a = [1, 2, 3];  a.append(4)
来源：http://aby.cucudq.cn

[T21] Swift：遍历
来源：http://utu.zhongyouzk.top

for x in a { print(x) }
来源：http://off.ybcxt.top

[T22] Swift：字典
来源：http://bdx.shuidangran.top

var d = ["a": 1];  d["b"] = 2
来源：http://bmx.sjlbkw.cn

[T23] Swift：函数
来源：http://zsl.sufxvd.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://onk.shanyushiyangtech.top

[T24] Swift：闭包
来源：http://esz.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pxh.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://jld.yongpay.top

struct P { var x: Int }
来源：http://nmm.chenzaomai.com

[T26] Swift：类与重写
来源：http://gao.zycfv.cn

class A: Base { override func f() {} }
来源：http://ada.redwolf501.top

[T27] Swift：错误处理
来源：http://udt.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://xvj.cucudq.cn

[T28] Swift：枚举
来源：http://jgt.jiagoushi.top

enum Color { case red, green }
来源：http://yov.epnwcf.com

[T29] Swift：guard 提前返回
来源：http://hot.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://fcf.hysaishi.cn

[T30] Swift：协议
来源：http://mwl.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://phv.nanxinkj.top

[T31] Lua：Hello World
来源：http://bbn.fengsongda.top

print("Hello")
来源：http://idj.0kj1m.cn

[T32] Lua：局部变量
来源：http://jio.shzxlz.cn

local a = 1
来源：http://eez.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://pcg.ppjwa.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vpd.xinyue.icu

[T34] Lua：遍历表
来源：http://bme.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://uyj.nwbrower.top


<!-- 参考信息 -->