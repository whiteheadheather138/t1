代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ush.yanxiufei.cn

[R30] 函数返回状态码
来源：http://qgz.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://fxc.jianghu66.top

[R31] 局部变量
来源：http://sjb.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://pkv.aibaodan.cn

[R32] 参数个数校验
来源：http://jqh.cheryme.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ixj.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://rbu.jinyuanbaomall.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gey.tian-w.cn

[R34] 退出时清理
来源：http://dlc.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://jcg.ctjpmb.com

[R35] 后台执行并等待
来源：http://rlu.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hia.shanyushiyangtech.top

[R36] 并发执行多个任务
来源：http://kaj.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pij.yonumen.top

[R37] 把输出赋给变量
来源：http://kuk.dashuyun.cn

files=$(ls -1)
来源：http://pfv.chenjidiqi.icu

[R38] 管道串联
来源：http://wmo.jinghuilouyu.cn

cat a.txt | grep -i error | wc -l
来源：http://pnr.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://djl.jqgufenzy.top

cmd > out.log 2>&1
来源：http://baa.ydjk.org.cn

[R40] 追加写日志
来源：http://dxq.chenjidiqi.icu

echo "log" >> out.log
来源：http://quw.xinyue.icu

[R41] 丢弃输出
来源：http://zqa.fktsv.cn

cmd >/dev/null 2>&1
来源：http://oco.tian-w.cn

[R42] 输入重定向
来源：http://tfd.chenzaomai.com

wc -l < a.txt
来源：http://gmv.andypj.xyz

[R43] 按名字查找文件
来源：http://txu.iojbl.cn

find . -name "*.log" -type f
来源：http://nbw.hongshengwenyu.top

[R44] 按修改时间查找
来源：http://zyl.gogol.net.cn

find . -mtime -7 -type f
来源：http://quc.9152youxi.cn

[R45] 批量删除
来源：http://kpd.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://ddv.fehbvm.com

[R46] 递归替换文件内容
来源：http://pfj.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gpy.cashguo.top

[R47] sed 单行替换
来源：http://hqu.tarul.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pok.yongpay.top

[R48] awk 取指定列
来源：http://yqj.tian-w.cn

awk '{print $1, $3}' a.txt
来源：http://eor.hammf.cn

[R49] awk 带条件
来源：http://ycr.tanke756.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uoj.yonumen.top

[R50] awk 求和
来源：http://cvp.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cqb.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://dea.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pem.xingfuxueyuan.xyz

[R52] 统计行数
来源：http://nmq.hfpthk.cn

wc -l a.txt
来源：http://mcs.hnqzz.top

[R53] 查看文件头与实时尾
来源：http://lnr.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rjr.guannengcc.top

[R54] 比较两个文件
来源：http://hud.xziqi.cn

diff a.txt b.txt
来源：http://egb.52xcode.cn

[R55] 压缩与解压
来源：http://rom.fanxiaobao.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://aog.cheryme.top

[R56] 远程拷贝
来源：http://lhu.yonumen.top

scp file user@host:/path/
来源：http://ajj.hammf.cn

[R57] 远程执行命令
来源：http://dts.aibaodan.cn

ssh user@host 'uptime'
来源：http://zqt.zdqjudy.top

[R58] 下载文件
来源：http://len.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wew.yj20258.top

[R59] 发 POST JSON
来源：http://mys.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fxr.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://kvr.fzhhl.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qxe.haohaochexian.top

[R61] 磁盘占用
来源：http://aef.snrcjt.cn

df -h;  du -sh *
来源：http://geu.0kj1m.cn

[R62] 找最占空间的文件
来源：http://ssc.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://mnu.hesvh.cn

[R63] 内存与进程
来源：http://kam.dashuyun.cn

free -h;  ps aux | grep nginx
来源：http://miv.daxiang520.top

[R64] 结束进程
来源：http://vsj.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://arp.ywan-chungtsiang.top

[R65] 查看端口占用
来源：http://atn.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://prt.9152youxi.cn

[R66] 定时任务
来源：http://jcw.meibo888.top

crontab -e;  crontab -l
来源：http://wnh.haohaochexian.top

[R67] 生成随机十六进制串
来源：http://coh.fanxiaobao.xyz

openssl rand -hex 16
来源：http://aeb.sufxvd.cn

[R68] 计算文件校验值
来源：http://loi.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://ixo.shuidangran.top

[R69] 生成随机密码
来源：http://wur.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://zci.tarul.cn

[R70] 时间戳与互转
来源：http://iaq.svipenyu.cn

date +%s;  date -d @1700000000
来源：http://zdc.nanxinkj.top

[R71] 日期格式化
来源：http://hxu.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cvz.sjlbkw.cn

[R72] 等待端口就绪
来源：http://kvm.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://suk.zhijiandao.cn

[R73] 分割大日志
来源：http://zrr.uphjek.com

split -l 1000 big.log part_
来源：http://nab.guannengcc.top

[R74] 批量重命名
来源：http://vna.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yom.svipenyu.cn

[R75] 导出环境变量
来源：http://euo.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://htw.zycfv.cn

[R76] 使用临时文件
来源：http://yay.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hnw.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://uid.fktsv.cn

read -rp "请输入: " ans
来源：http://tsk.hfpthk.cn

[R78] 交互式菜单
来源：http://iaf.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sbb.9152youxi.cn

[R79] 解析命令行选项
来源：http://utx.zhengqikj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rxv.uphjek.com

[R80] 查看脚本执行耗时
来源：http://ies.quarkkingdee.top

time ./run.sh
来源：http://tcp.feifeiyinyue.top

================================================================================
来源：http://fth.zhiwuduotai.top

S. C / C++ 专题
来源：http://adl.ydjk.org.cn

================================================================================
来源：http://ygs.fzhhl.top

[S01] C：Hello World
来源：http://swt.shzxlz.cn

#include <stdio.h>
来源：http://saf.shanyushiyangtech.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ycm.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://bsd.zhiwuduotai.top

int a = 10; printf("%d\n", a);
来源：http://rxz.meibo888.top

[S03] C：读入整数
来源：http://dde.tarul.cn

int x; scanf("%d", &x);
来源：http://kkh.zdbjq.cn

[S04] C：字符串复制
来源：http://oil.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://myd.hammf.cn

[S05] C：字符串长度
来源：http://lmj.yj202588.top

strlen(s)
来源：http://fzh.ctjpmb.com

[S06] C：字符串比较
来源：http://mrz.nanxuanxn.top

strcmp(a, b) == 0
来源：http://rco.zhongyouzk.top

[S07] C：数组遍历求和
来源：http://bre.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qsp.zhengqikj.top

[S08] C：动态内存分配与释放
来源：http://tej.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ach.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://jan.zycfv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gxz.guannengcc.top

[S10] C：指针与解引用
来源：http://qvh.tanke756.top

int *p = &a;  *p = 5;
来源：http://nye.yongpay.top

[S11] C：逐行读文件
来源：http://pzt.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://uqh.cheryme.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bed.ydzc1.top

fclose(f);
来源：http://eod.sufxvd.cn

[S12] C：写文件
来源：http://eff.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nlw.nanxuanxn.top

[S13] C：宏定义
来源：http://dgh.yangfankeji.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pjk.meibo888.top

[S14] C：枚举
来源：http://sgz.zhixingplan.top

enum Color { RED, GREEN, BLUE };
来源：http://qvf.snrcjt.cn

[S15] C：类型转换
来源：http://tdp.xingfuxueyuan.xyz

(double) a / b
来源：http://ncr.ydzc1.top

[S16] C：位操作置位
来源：http://ndc.sufxvd.cn

x |= (1 << 3);
来源：http://vuu.xylfe.cn

[S17] C：安全拼接字符串
来源：http://xjz.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cml.9152youxi.cn

[S18] C：命令行参数
来源：http://dai.guannengcc.top

int main(int argc, char **argv)
来源：http://cuc.jinghuilouyu.cn

[S19] C：快速排序
来源：http://uhj.nanxuanxn.top

qsort(a, n, sizeof(int), cmp);
来源：http://ycf.pycfn.com

[S20] C：二分查找
来源：http://iri.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blw.havefunace.top

[S21] C：字符类别判断
来源：http://fks.xinyue.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hxr.yongpay.top

[S22] C：字符串转数字
来源：http://tjz.zhiwuduotai.top

atoi("42");  strtod("3.14", NULL);
来源：http://uyq.jinqigfzy.top

[S23] C：随机数
来源：http://svy.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wuc.shzxlz.cn

[S24] C：获取本地时间
来源：http://fae.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://acd.birdmap.top

[S25] C：内存拷贝
来源：http://ety.chenzaomai.com

memcpy(dst, src, n);
来源：http://tot.nwbrower.top

[S26] C：内存清零
来源：http://xgn.zycfv.cn

memset(a, 0, sizeof a);
来源：http://mxz.zhiwuduotai.top

[S27] C：定义常量
来源：http://lgv.cdnleiting.top

const double PI = 3.14159;
来源：http://mvv.cashguo.top

[S28] C：静态变量
来源：http://vyo.sysykeji.top

static int counter = 0;
来源：http://rdw.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://fsy.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pxn.zhixingplan.top

[S30] C：头文件保护
来源：http://cjq.sjlbkw.cn

#ifndef X_H
来源：http://ugw.guowangkeji.top

#define X_H
来源：http://spb.hywenlv.cn

#endif
来源：http://yxj.shangyingyoupin.top

[S31] C++：Hello World
来源：http://khl.hywenlv.cn

#include <iostream>
来源：http://ire.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://lsb.dianchejie.cn

[S32] C++：字符串
来源：http://nph.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://exz.aizwys.cn

[S33] C++：vector 增删
来源：http://ifi.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wkf.c1oappe.top

[S34] C++：遍历 vector
来源：http://txt.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://mkl.jlsjyb.cn

[S35] C++：map
来源：http://agg.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mdd.jqgfzy.top

[S36] C++：unordered_map
来源：http://lel.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fmo.sysykeji.top

[S37] C++：set
来源：http://uze.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ilb.zhiwuduotai.top

[S38] C++：排序
来源：http://bdi.tarul.cn

std::sort(v.begin(), v.end());
来源：http://oic.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://nxt.fehbvm.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bni.aibaodan.cn

[S40] C++：查找元素
来源：http://jfv.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ubb.sysykeji.top

[S41] C++：类与构造函数
来源：http://toa.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rqj.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://qgy.jlsjyb.cn

class B : public Base { public: void f() override {} };
来源：http://zhx.yuxming.cn

[S43] C++：智能指针
来源：http://ulq.sjlbkw.cn

auto p = std::make_unique<int>(5);
来源：http://pic.hnqzz.top

[S44] C++：引用传参
来源：http://qzu.ydjk.org.cn

void inc(int &x) { ++x; }
来源：http://won.cdnleiting.top

[S45] C++：lambda
来源：http://xzj.yj20258.top

auto add = [](int a, int b) { return a + b; };
来源：http://lcw.yj202588.top

[S46] C++：函数模板
来源：http://nub.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fyl.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://ipl.shanyushiyangtech.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mfn.cucudq.cn

[S48] C++：逐行读文件
来源：http://uvd.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tns.yongpay.top

while (std::getline(in, line)) { }
来源：http://kzt.wangdashe.top

[S49] C++：写文件
来源：http://nlh.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nzi.chenzaomai.com

[S50] C++：格式化数字
来源：http://xpa.redwolf501.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://njb.tian-w.cn

[S51] C++：显式类型转换
来源：http://njq.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://nea.shangyingyoupin.top

[S52] C++：const 与 noexcept
来源：http://mli.yonumen.top

int size() const noexcept { return n_; }
来源：http://vzu.cheryme.top

[S53] C++：移动语义
来源：http://tfm.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://rui.zhengqikj.top

[S54] C++：异常处理
来源：http://ykn.wangshuangyany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ktu.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://mtu.zycfv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ymz.tarul.cn

[S56] C++：optional
来源：http://fvd.pengpengdd.cyou

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nhn.ywan-chungtsiang.top

[S57] C++：编译期常量
来源：http://yej.sweek.top

constexpr int N = 10;
来源：http://fgi.sysykeji.top

[S58] C++：命名空间
来源：http://smc.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://kdf.havefunace.top

[S59] C++：静态断言
来源：http://djo.sysykeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tgc.yj202588.top

[S60] C++：遍历并删除元素
来源：http://mpo.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zen.sjlbkw.cn

================================================================================
来源：http://lzu.zycfv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ncs.cqqwz.cn

================================================================================
来源：http://lur.gotoacloud.top

[T01] Kotlin：Hello World
来源：http://fxf.smart0.xyz

println("Hello")
来源：http://qum.9152youxi.cn

[T02] Kotlin：变量
来源：http://kyx.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vyx.cashguo.top

[T03] Kotlin：字符串模板
来源：http://lnz.smart0.xyz

"值: $b"
来源：http://cwn.zhiwuduotai.top

[T04] Kotlin：空安全
来源：http://uma.nanxuanxn.top

val n: String? = null;  n?.length
来源：http://pye.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://vgd.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xfa.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://yfp.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://boi.ydzc1.top

[T07] Kotlin：集合过滤
来源：http://jas.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://efa.yj202588.top

[T08] Kotlin：数据类
来源：http://svy.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://rsh.xingfuxueyuan.xyz

[T09] Kotlin：扩展函数
来源：http://eac.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://syn.hcnkem.com

[T10] Kotlin：默认参数
来源：http://vil.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://gpn.chenlongwang.top

[T11] Kotlin：协程
来源：http://qju.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fiu.ivvv.top

[T12] Kotlin：解构声明
来源：http://yrp.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://ejz.shzxlz.cn

[T13] Kotlin：只读 Map
来源：http://zkj.wangdashe.top

val m = mapOf("a" to 1)
来源：http://coj.havefunace.top

[T14] Kotlin：循环
来源：http://loj.yuxming.cn

for (i in 1..10) println(i)
来源：http://qxo.ydzc1.top

[T15] Kotlin：接口
来源：http://buu.zycfv.cn

interface Shape { fun area(): Double }
来源：http://ssq.sxryk.cn

[T16] Swift：Hello World
来源：http://cuv.jiagoushi.top

print("Hello")
来源：http://ync.c1oappe.top

[T17] Swift：变量与常量
来源：http://mfc.vehdjk.com

var a = 1;  let b = 2
来源：http://rjr.yfazqb.com

[T18] Swift：字符串插值
来源：http://zmb.nanxinkj.top

"值: \(b)"
来源：http://oep.cheryme.top

[T19] Swift：可选绑定
来源：http://jih.sjlbkw.cn

if let n = opt { print(n) }
来源：http://wup.xuanzx.com

[T20] Swift：数组操作
来源：http://odh.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qmw.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://zky.nanxinkj.top

for x in a { print(x) }
来源：http://pad.uphjek.com

[T22] Swift：字典
来源：http://pjh.meibo888.top

var d = ["a": 1];  d["b"] = 2
来源：http://yum.cashguo.top

[T23] Swift：函数
来源：http://nrf.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sxb.zhoulong.xyz

[T24] Swift：闭包
来源：http://tom.nwbrower.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jec.zhongyouzk.top

[T25] Swift：结构体
来源：http://ule.yueranfly.top

struct P { var x: Int }
来源：http://eqc.guannengcc.top

[T26] Swift：类与重写
来源：http://lkb.zhijiandao.cn

class A: Base { override func f() {} }
来源：http://uvz.hywenlv.cn

[T27] Swift：错误处理
来源：http://tjw.316326.xyz

do { try f() } catch { print(error) }
来源：http://gha.yuxming.cn

[T28] Swift：枚举
来源：http://eaw.nanxinkj.top

enum Color { case red, green }
来源：http://fdf.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://nvt.mhx1999.top

guard let x = opt else { return }
来源：http://jbu.jlsjyb.cn

[T30] Swift：协议
来源：http://yht.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://lgk.ivvv.top

[T31] Lua：Hello World
来源：http://snj.0kj1m.cn

print("Hello")
来源：http://ify.gaohongyu789.top

[T32] Lua：局部变量
来源：http://lsa.ehwqpu.com

local a = 1
来源：http://agn.hammf.cn


<!-- 参考信息 -->