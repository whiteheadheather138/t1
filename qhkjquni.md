代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://nry.jlsjyb.cn

[R26] 命令替换
来源：http://xlv.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://dxi.bjfxy.top

[R27] 算术展开
来源：http://ivv.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://kyf.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://fwc.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://ule.jinyuanbaomall.cn

[R29] 定义函数
来源：http://rap.zhijiandao.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://odz.chenzaomai.com

[R30] 函数返回状态码
来源：http://doc.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://wgf.pycfn.com

[R31] 局部变量
来源：http://ygu.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://sbk.hfpthk.cn

[R32] 参数个数校验
来源：http://jxg.zdbjq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oxb.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://xjh.tarul.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ggj.xuanzx.com

[R34] 退出时清理
来源：http://vrw.vehdjk.com

trap 'rm -f "$tmp"' EXIT
来源：http://gip.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://qzg.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gkj.redwolf501.top

[R36] 并发执行多个任务
来源：http://zpc.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lmn.epnwcf.com

[R37] 把输出赋给变量
来源：http://hwe.ydzc1.top

files=$(ls -1)
来源：http://ixu.fktsv.cn

[R38] 管道串联
来源：http://rti.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://kie.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://nrg.uphjek.com

cmd > out.log 2>&1
来源：http://tfe.0kj1m.cn

[R40] 追加写日志
来源：http://efu.jinqigfzy.top

echo "log" >> out.log
来源：http://kpa.hesvh.cn

[R41] 丢弃输出
来源：http://dll.gzhubu.top

cmd >/dev/null 2>&1
来源：http://rdc.fzhhl.top

[R42] 输入重定向
来源：http://qwl.hysaishi.cn

wc -l < a.txt
来源：http://sun.yuanzhike.top

[R43] 按名字查找文件
来源：http://uvd.yongpay.top

find . -name "*.log" -type f
来源：http://rbu.guannengcc.top

[R44] 按修改时间查找
来源：http://mvq.yongpay.top

find . -mtime -7 -type f
来源：http://hoj.fehbvm.com

[R45] 批量删除
来源：http://xbo.fehbvm.com

find . -name "*.tmp" -delete
来源：http://bwd.chenzaomai.com

[R46] 递归替换文件内容
来源：http://lqq.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://trb.yongpay.top

[R47] sed 单行替换
来源：http://njy.vehdjk.com

sed -i 's/foo/bar/g' a.txt
来源：http://evt.ydzc1.top

[R48] awk 取指定列
来源：http://iyd.gotoacloud.top

awk '{print $1, $3}' a.txt
来源：http://qnw.redwolf501.top

[R49] awk 带条件
来源：http://asw.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nvt.pycfn.com

[R50] awk 求和
来源：http://vmr.xingfuxueyuan.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://tdu.shuidangran.top

[R51] 排序去重取前几
来源：http://awh.zhengqikj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mcy.xingfuxueyuan.xyz

[R52] 统计行数
来源：http://lcv.iojbl.cn

wc -l a.txt
来源：http://fqo.yfazqb.com

[R53] 查看文件头与实时尾
来源：http://zyy.tianlin.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nhc.hysaishi.cn

[R54] 比较两个文件
来源：http://swc.316326.xyz

diff a.txt b.txt
来源：http://qni.yueranfly.top

[R55] 压缩与解压
来源：http://twi.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gxr.mhx1999.top

[R56] 远程拷贝
来源：http://ulg.c1oappe.top

scp file user@host:/path/
来源：http://hct.zdqjudy.top

[R57] 远程执行命令
来源：http://szt.hfpthk.cn

ssh user@host 'uptime'
来源：http://rxy.jqgfzy.top

[R58] 下载文件
来源：http://lnq.hywenlv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jkj.ydjk.org.cn

[R59] 发 POST JSON
来源：http://upu.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qci.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://lrl.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mnf.zhengqikj.top

[R61] 磁盘占用
来源：http://lmj.hnxiangtu.top

df -h;  du -sh *
来源：http://oip.tian-w.cn

[R62] 找最占空间的文件
来源：http://nzt.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://nyn.yj202588.top

[R63] 内存与进程
来源：http://skn.cdnleiting.top

free -h;  ps aux | grep nginx
来源：http://zaq.svipenyu.cn

[R64] 结束进程
来源：http://wsg.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://lqz.quarkkingdee.top

[R65] 查看端口占用
来源：http://fcu.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gcb.jinghuilouyu.cn

[R66] 定时任务
来源：http://kzn.vehdjk.com

crontab -e;  crontab -l
来源：http://fli.fktsv.cn

[R67] 生成随机十六进制串
来源：http://krc.epnwcf.com

openssl rand -hex 16
来源：http://yys.havefunace.top

[R68] 计算文件校验值
来源：http://jeq.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://ome.kuanghao11.cn

[R69] 生成随机密码
来源：http://kqq.snrcjt.cn

head -c 16 /dev/urandom | base64
来源：http://ojj.shanyushiyangkeji.top

[R70] 时间戳与互转
来源：http://lus.haohaochexian.top

date +%s;  date -d @1700000000
来源：http://hxo.shuidangran.top

[R71] 日期格式化
来源：http://xfl.cheryme.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fmg.haohaochexian.top

[R72] 等待端口就绪
来源：http://msm.meibo888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://edd.xylfe.cn

[R73] 分割大日志
来源：http://agi.jqgufenzy.top

split -l 1000 big.log part_
来源：http://urj.dashuyun.cn

[R74] 批量重命名
来源：http://ocp.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kze.tian-w.cn

[R75] 导出环境变量
来源：http://uvn.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://jog.jyoumei.cn

[R76] 使用临时文件
来源：http://wtz.zhiwuduotai.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gtl.meibo888.top

[R77] 读取用户输入
来源：http://esw.quarkkingdee.top

read -rp "请输入: " ans
来源：http://xrt.fehbvm.com

[R78] 交互式菜单
来源：http://pin.nwbrower.top

select opt in a b c; do echo "$opt"; break; done
来源：http://peh.bbcook.cn

[R79] 解析命令行选项
来源：http://ixh.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://miv.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://agw.andypj.xyz

time ./run.sh
来源：http://czh.zhixingplan.top

================================================================================
来源：http://thu.svipenyu.cn

S. C / C++ 专题
来源：http://cuc.jqgufenzy.top

================================================================================
来源：http://zfq.vehdjk.com

[S01] C：Hello World
来源：http://rkh.nanxuanxn.top

#include <stdio.h>
来源：http://obm.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://drv.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://nda.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://txo.cqqwz.cn

[S03] C：读入整数
来源：http://omx.yonumen.top

int x; scanf("%d", &x);
来源：http://dyb.cdnleiting.top

[S04] C：字符串复制
来源：http://ejg.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://iwe.yanxiufei.cn

[S05] C：字符串长度
来源：http://ebb.tarul.cn

strlen(s)
来源：http://pmc.yueranfly.top

[S06] C：字符串比较
来源：http://udd.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://mji.shuidangran.top

[S07] C：数组遍历求和
来源：http://qif.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://afb.hysaishi.cn

[S08] C：动态内存分配与释放
来源：http://oen.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ibn.yvedp.cn

[S09] C：结构体定义与初始化
来源：http://dam.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ttc.sufxvd.cn

[S10] C：指针与解引用
来源：http://fbo.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://qmh.sxryk.cn

[S11] C：逐行读文件
来源：http://egg.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://twe.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vau.hysaishi.cn

fclose(f);
来源：http://ejv.cdnleiting.top

[S12] C：写文件
来源：http://vtq.birdmap.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yez.zycfv.cn

[S13] C：宏定义
来源：http://ttb.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rhq.zhiwuduotai.top

[S14] C：枚举
来源：http://ujl.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://swd.chenlongwang.top

[S15] C：类型转换
来源：http://oxp.gogol.net.cn

(double) a / b
来源：http://wtb.hcnkem.com

[S16] C：位操作置位
来源：http://jbo.kuanghao11.cn

x |= (1 << 3);
来源：http://dlh.sxryk.cn

[S17] C：安全拼接字符串
来源：http://laj.zhijiandao.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lhi.meibo888.top

[S18] C：命令行参数
来源：http://ywz.fengsongda.top

int main(int argc, char **argv)
来源：http://oxw.jyoumei.cn

[S19] C：快速排序
来源：http://jfp.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://rsm.hfpthk.cn

[S20] C：二分查找
来源：http://wjn.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pch.jianghu66.top

[S21] C：字符类别判断
来源：http://hht.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mza.vehdjk.com

[S22] C：字符串转数字
来源：http://otg.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://emw.zhiwuduotai.top

[S23] C：随机数
来源：http://kax.daxiang520.top

srand(time(NULL));  int r = rand() % 100;
来源：http://avh.zycfv.cn

[S24] C：获取本地时间
来源：http://hjj.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yvz.tian-w.cn

[S25] C：内存拷贝
来源：http://xyj.dashuyun.cn

memcpy(dst, src, n);
来源：http://iup.svipenyu.cn

[S26] C：内存清零
来源：http://hnd.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://jfa.sufxvd.cn

[S27] C：定义常量
来源：http://bwj.pengpengdd.cyou

const double PI = 3.14159;
来源：http://cvt.tian-w.cn

[S28] C：静态变量
来源：http://jyk.bjfxy.top

static int counter = 0;
来源：http://zkj.316326.xyz

[S29] C：变参函数
来源：http://pww.jinghuilouyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://src.iojbl.cn

[S30] C：头文件保护
来源：http://egp.sufxvd.cn

#ifndef X_H
来源：http://dup.svipenyu.cn

#define X_H
来源：http://xtf.wangshuangyany.cn

#endif
来源：http://ztj.quarkkingdee.top

[S31] C++：Hello World
来源：http://wsy.jinqigfzy.top

#include <iostream>
来源：http://tzv.hongshengwenyu.top

int main() { std::cout << "Hello\n"; }
来源：http://std.52xcode.cn

[S32] C++：字符串
来源：http://ntw.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://vqa.cashguo.top

[S33] C++：vector 增删
来源：http://yzk.jinqigfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hmg.daxiang520.top

[S34] C++：遍历 vector
来源：http://vux.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://lfl.epnwcf.com

[S35] C++：map
来源：http://axq.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rpa.shzxlz.cn

[S36] C++：unordered_map
来源：http://cfk.ctjpmb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vtc.bbcook.cn

[S37] C++：set
来源：http://klr.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ima.jiagoushi.top

[S38] C++：排序
来源：http://gao.hesvh.cn

std::sort(v.begin(), v.end());
来源：http://xpi.nanxinkj.top

[S39] C++：自定义比较器排序
来源：http://sqs.bbcook.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yqo.yuxming.cn

[S40] C++：查找元素
来源：http://nye.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pes.gzhubu.top

[S41] C++：类与构造函数
来源：http://lxj.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wim.316326.xyz

[S42] C++：继承与虚函数
来源：http://twt.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://vua.zhiwuduotai.top

[S43] C++：智能指针
来源：http://ynv.zhengqikj.top

auto p = std::make_unique<int>(5);
来源：http://cjr.chenlongwang.top

[S44] C++：引用传参
来源：http://bed.tarul.cn

void inc(int &x) { ++x; }
来源：http://xkx.hywenlv.cn

[S45] C++：lambda
来源：http://zml.hfpthk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://peo.nanxuanxn.top

[S46] C++：函数模板
来源：http://luz.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jqk.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://wal.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iqz.yvedp.cn

[S48] C++：逐行读文件
来源：http://ozy.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://vpw.cheryme.top

while (std::getline(in, line)) { }
来源：http://wxe.svipenyu.cn

[S49] C++：写文件
来源：http://vfs.xuanzx.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fgt.xziqi.cn

[S50] C++：格式化数字
来源：http://piu.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ekq.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://mhn.jinqigfzy.top

static_cast<double>(a) / b
来源：http://iuc.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://any.cheryme.top

int size() const noexcept { return n_; }
来源：http://lnt.ydzc1.top

[S53] C++：移动语义
来源：http://xvd.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://ozi.zdbjq.cn

[S54] C++：异常处理
来源：http://ssu.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wdr.jiagoushi.top

[S55] C++：结构化绑定
来源：http://snr.tarul.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://acl.haohaochexian.top

[S56] C++：optional
来源：http://dkf.hnqzz.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ajl.guannengcc.top

[S57] C++：编译期常量
来源：http://ppo.jlsjyb.cn

constexpr int N = 10;
来源：http://ekv.snrcjt.cn

[S58] C++：命名空间
来源：http://iyb.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://qtr.bjfxy.top

[S59] C++：静态断言
来源：http://pns.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://phd.cashguo.top

[S60] C++：遍历并删除元素
来源：http://rlx.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://msc.jianghu66.top

================================================================================
来源：http://nlk.xingfuxueyuan.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xyj.ctjpmb.com

================================================================================
来源：http://dvr.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://rvx.daxiang520.top

println("Hello")
来源：http://wne.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://eya.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lkm.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://erd.vqdsnc.cn

"值: $b"
来源：http://zvv.yuxming.cn

[T04] Kotlin：空安全
来源：http://rru.fktsv.cn

val n: String? = null;  n?.length
来源：http://aqn.hywenlv.cn

[T05] Kotlin：when 表达式
来源：http://lcr.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kgj.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://toe.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xgf.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://xbw.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://auj.ppjwa.cn

[T08] Kotlin：数据类
来源：http://jxx.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://acz.chenjidiqi.icu

[T09] Kotlin：扩展函数
来源：http://cwk.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://wci.jinghuilouyu.cn

[T10] Kotlin：默认参数
来源：http://rxe.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://phy.ydjk.org.cn

[T11] Kotlin：协程
来源：http://ebp.316326.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://djk.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://ytp.hongshengwenyu.top

val (a, b) = Pair(1, 2)
来源：http://lce.hnqzz.top

[T13] Kotlin：只读 Map
来源：http://fhv.c1oappe.top

val m = mapOf("a" to 1)
来源：http://yop.tianlin.xyz

[T14] Kotlin：循环
来源：http://esk.shzxlz.cn

for (i in 1..10) println(i)
来源：http://qcz.uphjek.com

[T15] Kotlin：接口
来源：http://bta.iojbl.cn

interface Shape { fun area(): Double }
来源：http://fyn.cdnleiting.top

[T16] Swift：Hello World
来源：http://wgt.sysykeji.top

print("Hello")
来源：http://jvm.gzhubu.top

[T17] Swift：变量与常量
来源：http://kvk.tianlin.xyz

var a = 1;  let b = 2
来源：http://syo.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://pjn.xuanzx.com

"值: \(b)"
来源：http://caa.nwbrower.top

[T19] Swift：可选绑定
来源：http://hik.yj20258.top

if let n = opt { print(n) }
来源：http://bqf.0kj1m.cn

[T20] Swift：数组操作
来源：http://sxp.jlsjyb.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hop.shangyingyoupin.top

[T21] Swift：遍历
来源：http://agg.zhiwuduotai.top

for x in a { print(x) }
来源：http://wxd.bjfxy.top

[T22] Swift：字典
来源：http://aot.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://qai.hammf.cn

[T23] Swift：函数
来源：http://vhx.nanxuanxn.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gpd.yuanzhike.top

[T24] Swift：闭包
来源：http://eed.yonumen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wnc.pengpengdd.cyou

[T25] Swift：结构体
来源：http://rfo.ydjk.org.cn

struct P { var x: Int }
来源：http://rtd.havefunace.top

[T26] Swift：类与重写
来源：http://ivq.yj202588.top

class A: Base { override func f() {} }
来源：http://hbj.vehdjk.com

[T27] Swift：错误处理
来源：http://cbn.smart0.xyz

do { try f() } catch { print(error) }
来源：http://coi.fktsv.cn

[T28] Swift：枚举
来源：http://wvv.cqqwz.cn

enum Color { case red, green }
来源：http://cnq.fehbvm.com


<!-- 参考信息 -->