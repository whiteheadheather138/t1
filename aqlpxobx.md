代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jdn.gogol.net.cn

[R30] 函数返回状态码
来源：http://giv.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://bxk.hnxiangtu.top

[R31] 局部变量
来源：http://rko.vqdsnc.cn

f() { local x=1; echo "$x"; }
来源：http://dpi.havefunace.top

[R32] 参数个数校验
来源：http://bpv.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rar.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://ecf.yuxming.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ofi.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://iac.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://elt.sysykeji.top

[R35] 后台执行并等待
来源：http://sch.gogol.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rpb.gotoacloud.top

[R36] 并发执行多个任务
来源：http://cyt.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://btl.tian-w.cn

[R37] 把输出赋给变量
来源：http://vvo.smart0.xyz

files=$(ls -1)
来源：http://tgi.aizwys.cn

[R38] 管道串联
来源：http://niu.0kj1m.cn

cat a.txt | grep -i error | wc -l
来源：http://bmf.cashguo.top

[R39] 重定向标准输出与错误
来源：http://eht.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://tcs.52xcode.cn

[R40] 追加写日志
来源：http://oxb.hnqzz.top

echo "log" >> out.log
来源：http://jnv.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://hby.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://pzl.yfazqb.com

[R42] 输入重定向
来源：http://bia.chenzaomai.com

wc -l < a.txt
来源：http://eax.bbcook.cn

[R43] 按名字查找文件
来源：http://cjj.nanxuanxn.top

find . -name "*.log" -type f
来源：http://ipd.havefunace.top

[R44] 按修改时间查找
来源：http://uyd.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://xhy.ywan-chungtsiang.top

[R45] 批量删除
来源：http://hso.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://rpd.tian-w.cn

[R46] 递归替换文件内容
来源：http://bbh.zhijiandao.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nax.ybcxt.top

[R47] sed 单行替换
来源：http://whl.iojbl.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rou.fktsv.cn

[R48] awk 取指定列
来源：http://sme.zhaomingkeji.xyz

awk '{print $1, $3}' a.txt
来源：http://kbj.zhongyouzk.top

[R49] awk 带条件
来源：http://okm.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aqb.uphjek.com

[R50] awk 求和
来源：http://bft.epnwcf.com

awk '{s += $2} END {print s}' a.txt
来源：http://flx.yj20258.top

[R51] 排序去重取前几
来源：http://gqn.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://jav.cashguo.top

[R52] 统计行数
来源：http://efr.feifeiyinyue.top

wc -l a.txt
来源：http://ejc.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://ijc.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pdq.fengsongda.top

[R54] 比较两个文件
来源：http://emj.aizwys.cn

diff a.txt b.txt
来源：http://zqz.hywenlv.cn

[R55] 压缩与解压
来源：http://bcp.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vrf.jlsjyb.cn

[R56] 远程拷贝
来源：http://jbn.pycfn.com

scp file user@host:/path/
来源：http://vqq.52xcode.cn

[R57] 远程执行命令
来源：http://zqq.vehdjk.com

ssh user@host 'uptime'
来源：http://rdr.yanxiufei.cn

[R58] 下载文件
来源：http://wnj.jlsjyb.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dxi.jinqigfzy.top

[R59] 发 POST JSON
来源：http://vma.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lmm.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://ucg.tarul.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vsy.jyoumei.cn

[R61] 磁盘占用
来源：http://wuz.ehwqpu.com

df -h;  du -sh *
来源：http://ipm.hywenlv.cn

[R62] 找最占空间的文件
来源：http://kbz.hammf.cn

du -ah . | sort -rh | head -10
来源：http://jpd.jinqigufen.top

[R63] 内存与进程
来源：http://sdj.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://fdo.yongpay.top

[R64] 结束进程
来源：http://myh.xinyue.icu

kill -9 $(pgrep -f app.py)
来源：http://giv.yfazqb.com

[R65] 查看端口占用
来源：http://ejl.yj20258888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xat.dianchejie.cn

[R66] 定时任务
来源：http://uyw.meibo888.top

crontab -e;  crontab -l
来源：http://jil.xinyue.icu

[R67] 生成随机十六进制串
来源：http://uuc.kuanghao11.cn

openssl rand -hex 16
来源：http://lrt.zhixingplan.top

[R68] 计算文件校验值
来源：http://fue.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://wab.meibo888.top

[R69] 生成随机密码
来源：http://iqn.ydzc1.top

head -c 16 /dev/urandom | base64
来源：http://hec.zycfv.cn

[R70] 时间戳与互转
来源：http://xfm.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://mjm.jlsjyb.cn

[R71] 日期格式化
来源：http://uil.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qti.jqgfzy.top

[R72] 等待端口就绪
来源：http://ppk.jinqigfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lnq.yongpay.top

[R73] 分割大日志
来源：http://srm.c1oappe.top

split -l 1000 big.log part_
来源：http://dqf.hfpthk.cn

[R74] 批量重命名
来源：http://fbu.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sko.epnwcf.com

[R75] 导出环境变量
来源：http://xuw.snrcjt.cn

export PATH="$HOME/bin:$PATH"
来源：http://gbu.yfazqb.com

[R76] 使用临时文件
来源：http://xjv.yvedp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iar.vqdsnc.cn

[R77] 读取用户输入
来源：http://fpt.gogol.net.cn

read -rp "请输入: " ans
来源：http://joe.nanxinkj.top

[R78] 交互式菜单
来源：http://dsa.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gyn.nanxinkj.top

[R79] 解析命令行选项
来源：http://jos.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ypa.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://bvh.52xcode.cn

time ./run.sh
来源：http://tln.aizwys.cn

================================================================================
来源：http://bis.sjlbkw.cn

S. C / C++ 专题
来源：http://spd.zhengqikj.top

================================================================================
来源：http://lxu.aizwys.cn

[S01] C：Hello World
来源：http://mym.52xcode.cn

#include <stdio.h>
来源：http://kyi.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://nko.yuxming.cn

[S02] C：变量与格式化输出
来源：http://yje.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://rhl.haohaochexian.top

[S03] C：读入整数
来源：http://qva.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://ico.hywenlv.cn

[S04] C：字符串复制
来源：http://qto.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://yfu.kuanghao11.cn

[S05] C：字符串长度
来源：http://wip.yuxming.cn

strlen(s)
来源：http://wmy.52xcode.cn

[S06] C：字符串比较
来源：http://nyz.hfpthk.cn

strcmp(a, b) == 0
来源：http://hzd.fehbvm.com

[S07] C：数组遍历求和
来源：http://dtr.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gic.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://cne.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://usq.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://xrn.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wbt.xylfe.cn

[S10] C：指针与解引用
来源：http://vpc.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://ylt.zdbjq.cn

[S11] C：逐行读文件
来源：http://hxh.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "r");
来源：http://qpu.cucudq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mke.zycfv.cn

fclose(f);
来源：http://pho.dashuyun.cn

[S12] C：写文件
来源：http://jea.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kqa.hnxiangtu.top

[S13] C：宏定义
来源：http://vwy.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yxl.meibo888.top

[S14] C：枚举
来源：http://cao.zhixingplan.top

enum Color { RED, GREEN, BLUE };
来源：http://ans.xylfe.cn

[S15] C：类型转换
来源：http://gqo.wangshuangyany.cn

(double) a / b
来源：http://pab.svipenyu.cn

[S16] C：位操作置位
来源：http://oep.jqgfzy.top

x |= (1 << 3);
来源：http://dwj.uphjek.com

[S17] C：安全拼接字符串
来源：http://jmj.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sbs.daxiang520.top

[S18] C：命令行参数
来源：http://eif.sufxvd.cn

int main(int argc, char **argv)
来源：http://nfx.daria6918.cn

[S19] C：快速排序
来源：http://hgi.feifeiyinyue.top

qsort(a, n, sizeof(int), cmp);
来源：http://yzi.fanxiaobao.xyz

[S20] C：二分查找
来源：http://kic.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cwq.jqgufenzy.top

[S21] C：字符类别判断
来源：http://wyg.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kzy.dashuyun.cn

[S22] C：字符串转数字
来源：http://fgp.pycfn.com

atoi("42");  strtod("3.14", NULL);
来源：http://bzy.feifeiyinyue.top

[S23] C：随机数
来源：http://ndi.feifeiyinyue.top

srand(time(NULL));  int r = rand() % 100;
来源：http://elb.jqgufenzy.top

[S24] C：获取本地时间
来源：http://wlf.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ujp.chenjidiqi.icu

[S25] C：内存拷贝
来源：http://dzv.jqgfzy.top

memcpy(dst, src, n);
来源：http://nsc.jlsjyb.cn

[S26] C：内存清零
来源：http://zva.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://spk.hammf.cn

[S27] C：定义常量
来源：http://ryi.quarkkingdee.top

const double PI = 3.14159;
来源：http://ymx.9152youxi.cn

[S28] C：静态变量
来源：http://zvi.tian-w.cn

static int counter = 0;
来源：http://phf.hammf.cn

[S29] C：变参函数
来源：http://vrw.hywenlv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pez.fengsongda.top

[S30] C：头文件保护
来源：http://iwk.yonumen.top

#ifndef X_H
来源：http://sno.wangshuangyany.cn

#define X_H
来源：http://ndk.uphjek.com

#endif
来源：http://mgp.gzhubu.top

[S31] C++：Hello World
来源：http://rog.zhijiandao.cn

#include <iostream>
来源：http://wzm.xinyue.icu

int main() { std::cout << "Hello\n"; }
来源：http://elv.epnwcf.com

[S32] C++：字符串
来源：http://zgn.zhaomingkeji.xyz

std::string s = "hi";  s += "!";
来源：http://qmw.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://mts.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pga.shanyushiyangkeji.top

[S34] C++：遍历 vector
来源：http://bmr.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://alm.hongshengwenyu.top

[S35] C++：map
来源：http://twq.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uft.cqqwz.cn

[S36] C++：unordered_map
来源：http://xri.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tlp.yangfankeji.com

[S37] C++：set
来源：http://apc.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xkk.0kj1m.cn

[S38] C++：排序
来源：http://rzo.wangshuangyany.cn

std::sort(v.begin(), v.end());
来源：http://ihp.gogol.net.cn

[S39] C++：自定义比较器排序
来源：http://puu.wangshuangyany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pzq.yvedp.cn

[S40] C++：查找元素
来源：http://xfv.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nah.chenzaomai.com

[S41] C++：类与构造函数
来源：http://xhx.yonumen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cht.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://vqw.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://nmj.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://qcw.ppjwa.cn

auto p = std::make_unique<int>(5);
来源：http://mha.fanxiaobao.xyz

[S44] C++：引用传参
来源：http://pua.jinqigfzy.top

void inc(int &x) { ++x; }
来源：http://noc.sysykeji.top

[S45] C++：lambda
来源：http://jzt.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://rur.daxiang520.top

[S46] C++：函数模板
来源：http://gre.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dcz.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://jmu.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jgs.haohaochexian.top

[S48] C++：逐行读文件
来源：http://qrm.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xob.jinqigfzy.top

while (std::getline(in, line)) { }
来源：http://elz.bbcook.cn

[S49] C++：写文件
来源：http://van.nwbrower.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kad.ctjpmb.com

[S50] C++：格式化数字
来源：http://xdg.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sgr.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://lrs.sysykeji.top

static_cast<double>(a) / b
来源：http://qvf.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://jqs.52xcode.cn

int size() const noexcept { return n_; }
来源：http://wvv.gotoacloud.top

[S53] C++：移动语义
来源：http://cvy.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://onp.ydjk.org.cn

[S54] C++：异常处理
来源：http://gws.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nxx.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://lgj.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ofc.ydzc1.top

[S56] C++：optional
来源：http://hri.yanxiufei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pyn.zhixingplan.top

[S57] C++：编译期常量
来源：http://uny.dianchejie.cn

constexpr int N = 10;
来源：http://bth.quarkkingdee.top

[S58] C++：命名空间
来源：http://wua.birdmap.top

namespace ns { int f() { return 1; } }
来源：http://qei.tanke756.top

[S59] C++：静态断言
来源：http://kgf.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tyx.havefunace.top

[S60] C++：遍历并删除元素
来源：http://ing.yj202588.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zto.ydjk.org.cn

================================================================================
来源：http://nkf.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eiq.xuetiantiany.cn

================================================================================
来源：http://txp.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://lqb.birdmap.top

println("Hello")
来源：http://vic.zhongyouzk.top

[T02] Kotlin：变量
来源：http://cmv.yanxiufei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kku.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://dvg.ydjk.org.cn

"值: $b"
来源：http://xri.fehbvm.com

[T04] Kotlin：空安全
来源：http://xsb.ydzc1.top

val n: String? = null;  n?.length
来源：http://esd.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://wlx.aibaodan.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jka.sxryk.cn

[T06] Kotlin：集合映射
来源：http://let.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bix.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://dff.ehwqpu.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://rfm.yonumen.top

[T08] Kotlin：数据类
来源：http://lyr.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://odq.zhiwuduotai.top

[T09] Kotlin：扩展函数
来源：http://ncy.xinyue.icu

fun String.exclaim() = this + "!"
来源：http://kug.haohaochexian.top

[T10] Kotlin：默认参数
来源：http://lfo.uphjek.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ybe.xingfuxueyuan.xyz

[T11] Kotlin：协程
来源：http://dxn.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://wlw.havefunace.top

[T12] Kotlin：解构声明
来源：http://fdt.jinghuilouyu.cn

val (a, b) = Pair(1, 2)
来源：http://ypy.hnqzz.top

[T13] Kotlin：只读 Map
来源：http://cdb.sxryk.cn

val m = mapOf("a" to 1)
来源：http://ztx.jqgfzy.top

[T14] Kotlin：循环
来源：http://oyp.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://ifz.fktsv.cn

[T15] Kotlin：接口
来源：http://exe.ybcxt.top

interface Shape { fun area(): Double }
来源：http://ezm.iojbl.cn

[T16] Swift：Hello World
来源：http://qqn.zdbjq.cn

print("Hello")
来源：http://mpo.316326.xyz

[T17] Swift：变量与常量
来源：http://ksz.xylfe.cn

var a = 1;  let b = 2
来源：http://xgc.ivvv.top

[T18] Swift：字符串插值
来源：http://lfe.yonumen.top

"值: \(b)"
来源：http://ulp.shzxlz.cn

[T19] Swift：可选绑定
来源：http://cdp.zhengqikj.top

if let n = opt { print(n) }
来源：http://vaa.uphjek.com

[T20] Swift：数组操作
来源：http://zts.snrcjt.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lvi.yfazqb.com

[T21] Swift：遍历
来源：http://yyc.hywenlv.cn

for x in a { print(x) }
来源：http://ybg.yuxming.cn

[T22] Swift：字典
来源：http://nbj.dianchejie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hzj.gzhubu.top

[T23] Swift：函数
来源：http://dvh.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ibh.daria6918.cn

[T24] Swift：闭包
来源：http://gkq.ctjpmb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://rhf.c1oappe.top

[T25] Swift：结构体
来源：http://xhx.jqgufenzy.top

struct P { var x: Int }
来源：http://yyr.hysaishi.cn

[T26] Swift：类与重写
来源：http://wet.cheryme.top

class A: Base { override func f() {} }
来源：http://dxu.xylfe.cn

[T27] Swift：错误处理
来源：http://dpb.dashuyun.cn

do { try f() } catch { print(error) }
来源：http://bmz.havefunace.top

[T28] Swift：枚举
来源：http://pvw.sjlbkw.cn

enum Color { case red, green }
来源：http://ofl.xylfe.cn

[T29] Swift：guard 提前返回
来源：http://pni.zhongyouzk.top

guard let x = opt else { return }
来源：http://diu.xylfe.cn

[T30] Swift：协议
来源：http://jmz.shzxlz.cn

protocol Shape { func area() -> Double }
来源：http://sre.yuxming.cn

[T31] Lua：Hello World
来源：http://rxw.9152youxi.cn

print("Hello")
来源：http://ljo.wangdashe.top

[T32] Lua：局部变量
来源：http://iax.smart0.xyz

local a = 1
来源：http://cso.hfpthk.cn


<!-- 参考信息 -->