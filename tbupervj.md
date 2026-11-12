代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tco.yj202588.top

[R30] 函数返回状态码
来源：http://pdq.tarul.cn

f() { return 0; }; f || echo "失败了"
来源：http://xzb.jinghuilouyu.cn

[R31] 局部变量
来源：http://wzp.guowangkeji.top

f() { local x=1; echo "$x"; }
来源：http://dxz.yuxming.cn

[R32] 参数个数校验
来源：http://vfh.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wvl.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://tjd.jinqigfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ksr.andypj.xyz

[R34] 退出时清理
来源：http://imr.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://kft.hfpthk.cn

[R35] 后台执行并等待
来源：http://hui.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://euo.wangdashe.top

[R36] 并发执行多个任务
来源：http://bav.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sbw.hammf.cn

[R37] 把输出赋给变量
来源：http://qhr.feifeiyinyue.top

files=$(ls -1)
来源：http://kni.zhaomingkeji.xyz

[R38] 管道串联
来源：http://uxp.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://ozr.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://awy.yueranfly.top

cmd > out.log 2>&1
来源：http://sjs.fehbvm.com

[R40] 追加写日志
来源：http://zsw.vqdsnc.cn

echo "log" >> out.log
来源：http://mdi.dianchejie.cn

[R41] 丢弃输出
来源：http://zxo.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://ueu.kuanghao11.cn

[R42] 输入重定向
来源：http://aiy.tian-w.cn

wc -l < a.txt
来源：http://vmz.nanxuanxn.top

[R43] 按名字查找文件
来源：http://ppe.jqgfzy.top

find . -name "*.log" -type f
来源：http://lek.xingfuxueyuan.xyz

[R44] 按修改时间查找
来源：http://qmg.zhiwuduotai.top

find . -mtime -7 -type f
来源：http://npv.zhengqikj.top

[R45] 批量删除
来源：http://zwi.zycfv.cn

find . -name "*.tmp" -delete
来源：http://nbm.sysykeji.top

[R46] 递归替换文件内容
来源：http://ajy.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vdn.dashuyun.cn

[R47] sed 单行替换
来源：http://mcv.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://fpi.fzhhl.top

[R48] awk 取指定列
来源：http://cwz.meibo888.top

awk '{print $1, $3}' a.txt
来源：http://xdk.yj202588.top

[R49] awk 带条件
来源：http://dqg.redwolf501.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uqt.aizwys.cn

[R50] awk 求和
来源：http://iws.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ylk.hongshengwenyu.top

[R51] 排序去重取前几
来源：http://xps.nanxuanxn.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ovu.gogol.net.cn

[R52] 统计行数
来源：http://fev.sxryk.cn

wc -l a.txt
来源：http://jlc.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://klp.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pug.xuetiantiany.cn

[R54] 比较两个文件
来源：http://xii.daria6918.cn

diff a.txt b.txt
来源：http://amj.vqdsnc.cn

[R55] 压缩与解压
来源：http://nbr.zhixingplan.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://opg.fehbvm.com

[R56] 远程拷贝
来源：http://ufq.wangdashe.top

scp file user@host:/path/
来源：http://ctm.52xcode.cn

[R57] 远程执行命令
来源：http://tpo.fktsv.cn

ssh user@host 'uptime'
来源：http://mpa.xziqi.cn

[R58] 下载文件
来源：http://cge.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xhx.yangfankeji.com

[R59] 发 POST JSON
来源：http://cys.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sny.ehwqpu.com

[R60] 只看 HTTP 状态码
来源：http://xkn.hesvh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cmk.ppjwa.cn

[R61] 磁盘占用
来源：http://hfm.fanxiaobao.xyz

df -h;  du -sh *
来源：http://lux.hnqzz.top

[R62] 找最占空间的文件
来源：http://apb.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://ksp.yanxiufei.cn

[R63] 内存与进程
来源：http://rtp.xinyue.icu

free -h;  ps aux | grep nginx
来源：http://nzj.sjlbkw.cn

[R64] 结束进程
来源：http://jgc.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://qxa.zhijiandao.cn

[R65] 查看端口占用
来源：http://bgt.jinqigufen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cdb.chenjidiqi.icu

[R66] 定时任务
来源：http://iti.cheryme.top

crontab -e;  crontab -l
来源：http://zii.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://vks.zycfv.cn

openssl rand -hex 16
来源：http://snw.zhaomingkeji.xyz

[R68] 计算文件校验值
来源：http://rtl.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hjj.jqgfzy.top

[R69] 生成随机密码
来源：http://pap.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://xsh.ydzc1.top

[R70] 时间戳与互转
来源：http://ocl.yuxming.cn

date +%s;  date -d @1700000000
来源：http://ybg.jinqigfzy.top

[R71] 日期格式化
来源：http://acd.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uwc.gogol.net.cn

[R72] 等待端口就绪
来源：http://isq.birdmap.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vjz.hnqzz.top

[R73] 分割大日志
来源：http://ylc.mhx1999.top

split -l 1000 big.log part_
来源：http://rsa.gzhubu.top

[R74] 批量重命名
来源：http://gsv.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vuu.zhiwuduotai.top

[R75] 导出环境变量
来源：http://ila.fengsongda.top

export PATH="$HOME/bin:$PATH"
来源：http://min.ywan-chungtsiang.top

[R76] 使用临时文件
来源：http://pnc.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kol.yj202588.top

[R77] 读取用户输入
来源：http://pns.yuanzhike.top

read -rp "请输入: " ans
来源：http://zsw.bjfxy.top

[R78] 交互式菜单
来源：http://xvs.jinyuanbaomall.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://baw.daria6918.cn

[R79] 解析命令行选项
来源：http://oei.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ukj.yfazqb.com

[R80] 查看脚本执行耗时
来源：http://ckz.cucudq.cn

time ./run.sh
来源：http://dwq.tanke756.top

================================================================================
来源：http://rkg.jqgufenzy.top

S. C / C++ 专题
来源：http://ryx.nwbrower.top

================================================================================
来源：http://api.gaohongyu789.top

[S01] C：Hello World
来源：http://awd.hywenlv.cn

#include <stdio.h>
来源：http://mwm.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://poi.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://qqx.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://sol.haohaochexian.top

[S03] C：读入整数
来源：http://zqp.hcnkem.com

int x; scanf("%d", &x);
来源：http://fkz.yj202588.top

[S04] C：字符串复制
来源：http://mub.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://mds.guannengcc.top

[S05] C：字符串长度
来源：http://kbz.316326.xyz

strlen(s)
来源：http://duu.cqqwz.cn

[S06] C：字符串比较
来源：http://cwf.sysykeji.top

strcmp(a, b) == 0
来源：http://fza.guowangkeji.top

[S07] C：数组遍历求和
来源：http://znn.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lpy.ppjwa.cn

[S08] C：动态内存分配与释放
来源：http://sjv.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://epm.gogol.net.cn

[S09] C：结构体定义与初始化
来源：http://imf.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gns.nanxuanxn.top

[S10] C：指针与解引用
来源：http://mus.zycfv.cn

int *p = &a;  *p = 5;
来源：http://fqk.yangfankeji.com

[S11] C：逐行读文件
来源：http://imy.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://cxk.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://hra.cheryme.top

fclose(f);
来源：http://hsj.hesvh.cn

[S12] C：写文件
来源：http://nxn.jiagoushi.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yln.snrcjt.cn

[S13] C：宏定义
来源：http://fhj.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eld.ivvv.top

[S14] C：枚举
来源：http://vuo.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://low.daxiang520.top

[S15] C：类型转换
来源：http://fhl.jiagoushi.top

(double) a / b
来源：http://mji.zhoulong.xyz

[S16] C：位操作置位
来源：http://ftl.jlsjyb.cn

x |= (1 << 3);
来源：http://zow.xylfe.cn

[S17] C：安全拼接字符串
来源：http://qgm.dashuyun.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sxg.ybcxt.top

[S18] C：命令行参数
来源：http://ore.daria6918.cn

int main(int argc, char **argv)
来源：http://ikr.jlsjyb.cn

[S19] C：快速排序
来源：http://qfu.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lxp.dashuyun.cn

[S20] C：二分查找
来源：http://riu.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mfz.ppjwa.cn

[S21] C：字符类别判断
来源：http://wxx.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gmc.jiagoushi.top

[S22] C：字符串转数字
来源：http://lsd.snrcjt.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eii.jinqigfzy.top

[S23] C：随机数
来源：http://qmu.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wef.shanyushiyangkeji.top

[S24] C：获取本地时间
来源：http://xbq.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vax.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://ytn.havefunace.top

memcpy(dst, src, n);
来源：http://gag.xuetiantiany.cn

[S26] C：内存清零
来源：http://zvx.shuidangran.top

memset(a, 0, sizeof a);
来源：http://qed.jianghu66.top

[S27] C：定义常量
来源：http://eti.jianghu66.top

const double PI = 3.14159;
来源：http://too.zhixingplan.top

[S28] C：静态变量
来源：http://ngv.shangyingyoupin.top

static int counter = 0;
来源：http://tix.shanyushiyangtech.top

[S29] C：变参函数
来源：http://jiy.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dgy.hesvh.cn

[S30] C：头文件保护
来源：http://yef.jqgfzy.top

#ifndef X_H
来源：http://zpx.xinyue.icu

#define X_H
来源：http://rnx.xylfe.cn

#endif
来源：http://zpw.zhiwuduotai.top

[S31] C++：Hello World
来源：http://tnf.ppjwa.cn

#include <iostream>
来源：http://dyj.sxryk.cn

int main() { std::cout << "Hello\n"; }
来源：http://nuc.redwolf501.top

[S32] C++：字符串
来源：http://fbj.hcnkem.com

std::string s = "hi";  s += "!";
来源：http://dex.xingfuxueyuan.xyz

[S33] C++：vector 增删
来源：http://yvr.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iup.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://vzr.jinqigfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://skz.hysaishi.cn

[S35] C++：map
来源：http://vib.guowangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://plf.ppjwa.cn

[S36] C++：unordered_map
来源：http://vdg.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jit.chenlongwang.top

[S37] C++：set
来源：http://wls.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vdx.smart0.xyz

[S38] C++：排序
来源：http://iuc.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://wrv.hfpthk.cn

[S39] C++：自定义比较器排序
来源：http://lqh.zycfv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wmd.jlsjyb.cn

[S40] C++：查找元素
来源：http://tde.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xoi.tanke756.top

[S41] C++：类与构造函数
来源：http://ffd.zhongyouzk.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ldl.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://puy.fanxiaobao.xyz

class B : public Base { public: void f() override {} };
来源：http://wlr.birdmap.top

[S43] C++：智能指针
来源：http://lip.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://ehz.zycfv.cn

[S44] C++：引用传参
来源：http://ygg.svipenyu.cn

void inc(int &x) { ++x; }
来源：http://dqd.hnqzz.top

[S45] C++：lambda
来源：http://dyc.ybcxt.top

auto add = [](int a, int b) { return a + b; };
来源：http://iqk.0kj1m.cn

[S46] C++：函数模板
来源：http://ysn.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://guu.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://cel.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vhs.c1oappe.top

[S48] C++：逐行读文件
来源：http://mjj.redwolf501.top

std::ifstream in("a.txt");  std::string line;
来源：http://wmv.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://eaq.redwolf501.top

[S49] C++：写文件
来源：http://dpp.xziqi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ost.chenlongwang.top

[S50] C++：格式化数字
来源：http://gqp.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hae.9152youxi.cn

[S51] C++：显式类型转换
来源：http://gbk.hcnkem.com

static_cast<double>(a) / b
来源：http://ucd.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://lgo.birdmap.top

int size() const noexcept { return n_; }
来源：http://zfl.dianchejie.cn

[S53] C++：移动语义
来源：http://qka.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://dtg.nanxuanxn.top

[S54] C++：异常处理
来源：http://xzp.fzhhl.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://byl.yueranfly.top

[S55] C++：结构化绑定
来源：http://avk.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bkw.pengpengdd.cyou

[S56] C++：optional
来源：http://qyo.chenlongwang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gzt.hywenlv.cn

[S57] C++：编译期常量
来源：http://mak.hnqzz.top

constexpr int N = 10;
来源：http://ean.jianghu66.top

[S58] C++：命名空间
来源：http://vav.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://hde.bjfxy.top

[S59] C++：静态断言
来源：http://mbb.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xmw.zhaomingkeji.xyz

[S60] C++：遍历并删除元素
来源：http://tkv.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ebe.daxiang520.top

================================================================================
来源：http://yen.ydzc1.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fsr.vehdjk.com

================================================================================
来源：http://qki.hammf.cn

[T01] Kotlin：Hello World
来源：http://nec.9152youxi.cn

println("Hello")
来源：http://ylk.cashguo.top

[T02] Kotlin：变量
来源：http://jmz.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://srx.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://qze.yueranfly.top

"值: $b"
来源：http://eoy.hywenlv.cn

[T04] Kotlin：空安全
来源：http://zpn.ywan-chungtsiang.top

val n: String? = null;  n?.length
来源：http://uba.zhongyouzk.top

[T05] Kotlin：when 表达式
来源：http://uzi.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zoy.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://mly.zycfv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://krq.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://kxz.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://knb.cucudq.cn

[T08] Kotlin：数据类
来源：http://jos.hammf.cn

data class User(val name: String, val age: Int)
来源：http://tfa.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://qrj.cheryme.top

fun String.exclaim() = this + "!"
来源：http://ujc.xinyue.icu

[T10] Kotlin：默认参数
来源：http://exj.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xgf.cdnleiting.top

[T11] Kotlin：协程
来源：http://xdf.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wrx.havefunace.top

[T12] Kotlin：解构声明
来源：http://reb.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://qbg.zhaomingkeji.xyz

[T13] Kotlin：只读 Map
来源：http://qtt.fktsv.cn

val m = mapOf("a" to 1)
来源：http://hie.nanxinkj.top

[T14] Kotlin：循环
来源：http://vdm.jianghu66.top

for (i in 1..10) println(i)
来源：http://kzv.nanxuanxn.top

[T15] Kotlin：接口
来源：http://jpb.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://jhz.iojbl.cn

[T16] Swift：Hello World
来源：http://wfo.zhoulong.xyz

print("Hello")
来源：http://ifm.ydzc1.top

[T17] Swift：变量与常量
来源：http://dth.gotoacloud.top

var a = 1;  let b = 2
来源：http://zto.jiagoushi.top

[T18] Swift：字符串插值
来源：http://iso.snrcjt.cn

"值: \(b)"
来源：http://aac.smart0.xyz

[T19] Swift：可选绑定
来源：http://gyi.meibo888.top

if let n = opt { print(n) }
来源：http://gek.guowangkeji.top

[T20] Swift：数组操作
来源：http://wzz.tianlin.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://wtg.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://foc.jyoumei.cn

for x in a { print(x) }
来源：http://bde.kuanghao11.cn

[T22] Swift：字典
来源：http://rad.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oyl.gaohongyu789.top

[T23] Swift：函数
来源：http://qmq.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dnf.yvedp.cn

[T24] Swift：闭包
来源：http://cct.gotoacloud.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kyp.sxryk.cn

[T25] Swift：结构体
来源：http://zgw.birdmap.top

struct P { var x: Int }
来源：http://txn.ehwqpu.com

[T26] Swift：类与重写
来源：http://nyx.svipenyu.cn

class A: Base { override func f() {} }
来源：http://gbj.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://odf.xingfuxueyuan.xyz

do { try f() } catch { print(error) }
来源：http://abu.xziqi.cn

[T28] Swift：枚举
来源：http://dxi.zhongyouzk.top

enum Color { case red, green }
来源：http://ylh.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://sgg.shzxlz.cn

guard let x = opt else { return }
来源：http://axy.aizwys.cn

[T30] Swift：协议
来源：http://utg.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://lnh.yongpay.top

[T31] Lua：Hello World
来源：http://vnr.vehdjk.com

print("Hello")
来源：http://hgg.redwolf501.top

[T32] Lua：局部变量
来源：http://joh.tanke756.top

local a = 1
来源：http://qco.uphjek.com


<!-- 参考信息 -->