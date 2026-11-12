代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://uwo.9152youxi.cn

[R26] 命令替换
来源：http://zmo.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://ecj.feifeiyinyue.top

[R27] 算术展开
来源：http://cop.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://hrd.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://wki.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://gvi.snrcjt.cn

[R29] 定义函数
来源：http://mdg.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tqb.xuanzx.com

[R30] 函数返回状态码
来源：http://ivl.vqdsnc.cn

f() { return 0; }; f || echo "失败了"
来源：http://juc.yonumen.top

[R31] 局部变量
来源：http://dgw.jqgufenzy.top

f() { local x=1; echo "$x"; }
来源：http://gap.bbcook.cn

[R32] 参数个数校验
来源：http://iyj.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rns.bbcook.cn

[R33] 捕获错误并提示行号
来源：http://ukv.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wnc.yj202588.top

[R34] 退出时清理
来源：http://dgh.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://mej.mhx1999.top

[R35] 后台执行并等待
来源：http://cfa.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fwi.tanke756.top

[R36] 并发执行多个任务
来源：http://sil.hongshengwenyu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nip.andypj.xyz

[R37] 把输出赋给变量
来源：http://roh.xuetiantiany.cn

files=$(ls -1)
来源：http://azg.jinyuanbaomall.cn

[R38] 管道串联
来源：http://umd.gaohongyu789.top

cat a.txt | grep -i error | wc -l
来源：http://pgk.hongshengwenyu.top

[R39] 重定向标准输出与错误
来源：http://jai.epnwcf.com

cmd > out.log 2>&1
来源：http://zmf.yj20258.top

[R40] 追加写日志
来源：http://opy.xuetiantiany.cn

echo "log" >> out.log
来源：http://nmb.ybcxt.top

[R41] 丢弃输出
来源：http://uje.daxiang520.top

cmd >/dev/null 2>&1
来源：http://mao.ywan-chungtsiang.top

[R42] 输入重定向
来源：http://ebm.smart0.xyz

wc -l < a.txt
来源：http://irv.shanyushiyangtech.top

[R43] 按名字查找文件
来源：http://nbs.aibaodan.cn

find . -name "*.log" -type f
来源：http://ypb.ivvv.top

[R44] 按修改时间查找
来源：http://ump.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://mlc.zhengqikj.top

[R45] 批量删除
来源：http://exd.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://mnv.hcnkem.com

[R46] 递归替换文件内容
来源：http://sef.havefunace.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wxr.yj20258.top

[R47] sed 单行替换
来源：http://njt.ydzc1.top

sed -i 's/foo/bar/g' a.txt
来源：http://ict.tian-w.cn

[R48] awk 取指定列
来源：http://dpf.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://ztn.jianghu66.top

[R49] awk 带条件
来源：http://xbq.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://knf.hysaishi.cn

[R50] awk 求和
来源：http://tfa.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://faq.xziqi.cn

[R51] 排序去重取前几
来源：http://lno.daxiang520.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rcu.shzxlz.cn

[R52] 统计行数
来源：http://cgs.ppjwa.cn

wc -l a.txt
来源：http://ytm.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://oje.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tvj.sufxvd.cn

[R54] 比较两个文件
来源：http://cwf.jyoumei.cn

diff a.txt b.txt
来源：http://kkm.havefunace.top

[R55] 压缩与解压
来源：http://pse.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bny.shangyingyoupin.top

[R56] 远程拷贝
来源：http://mqj.jinqigfzy.top

scp file user@host:/path/
来源：http://sls.sjlbkw.cn

[R57] 远程执行命令
来源：http://cum.guowangkeji.top

ssh user@host 'uptime'
来源：http://pbz.nwbrower.top

[R58] 下载文件
来源：http://bhv.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://foe.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://xny.hongshengwenyu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lva.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://nch.tian-w.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tcq.pengpengdd.cyou

[R61] 磁盘占用
来源：http://dys.ehwqpu.com

df -h;  du -sh *
来源：http://vsv.gzhubu.top

[R62] 找最占空间的文件
来源：http://zue.chenzaomai.com

du -ah . | sort -rh | head -10
来源：http://nrp.xuanzx.com

[R63] 内存与进程
来源：http://caw.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://kis.sjlbkw.cn

[R64] 结束进程
来源：http://emx.sweek.top

kill -9 $(pgrep -f app.py)
来源：http://xle.fktsv.cn

[R65] 查看端口占用
来源：http://qgu.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kpk.xziqi.cn

[R66] 定时任务
来源：http://dqa.zhoulong.xyz

crontab -e;  crontab -l
来源：http://qvs.ehwqpu.com

[R67] 生成随机十六进制串
来源：http://ghm.fzhhl.top

openssl rand -hex 16
来源：http://bps.nanxinkj.top

[R68] 计算文件校验值
来源：http://ejw.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://cjk.aibaodan.cn

[R69] 生成随机密码
来源：http://nvj.cdnleiting.top

head -c 16 /dev/urandom | base64
来源：http://ibq.hysaishi.cn

[R70] 时间戳与互转
来源：http://fvg.yonumen.top

date +%s;  date -d @1700000000
来源：http://fzt.nanxuanxn.top

[R71] 日期格式化
来源：http://tgb.quarkkingdee.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xow.sufxvd.cn

[R72] 等待端口就绪
来源：http://vdk.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://idy.yanxiufei.cn

[R73] 分割大日志
来源：http://nxq.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://gik.ctjpmb.com

[R74] 批量重命名
来源：http://exm.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cyj.yangfankeji.com

[R75] 导出环境变量
来源：http://yhk.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://qbl.jlsjyb.cn

[R76] 使用临时文件
来源：http://lhe.cqqwz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wwg.yueranfly.top

[R77] 读取用户输入
来源：http://flo.xziqi.cn

read -rp "请输入: " ans
来源：http://qhi.birdmap.top

[R78] 交互式菜单
来源：http://pvr.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iij.yj20258.top

[R79] 解析命令行选项
来源：http://nza.wangdashe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://msg.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://txo.zhixingplan.top

time ./run.sh
来源：http://spv.jianghu66.top

================================================================================
来源：http://hgv.zhixingplan.top

S. C / C++ 专题
来源：http://pzy.jiagoushi.top

================================================================================
来源：http://eiq.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://tsk.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://mls.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ccf.zhaomingkeji.xyz

[S02] C：变量与格式化输出
来源：http://dcv.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://lga.yanxiufei.cn

[S03] C：读入整数
来源：http://sea.xylfe.cn

int x; scanf("%d", &x);
来源：http://tol.redwolf501.top

[S04] C：字符串复制
来源：http://myv.jinghuilouyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hhd.yonumen.top

[S05] C：字符串长度
来源：http://zsq.fehbvm.com

strlen(s)
来源：http://eel.smart0.xyz

[S06] C：字符串比较
来源：http://cvn.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://zml.tanke756.top

[S07] C：数组遍历求和
来源：http://zrk.gogol.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gyy.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://ljy.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ugz.guannengcc.top

[S09] C：结构体定义与初始化
来源：http://qfc.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zwv.cheryme.top

[S10] C：指针与解引用
来源：http://gev.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://veo.cucudq.cn

[S11] C：逐行读文件
来源：http://ysg.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://xkc.xziqi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wuu.vehdjk.com

fclose(f);
来源：http://qpl.ivvv.top

[S12] C：写文件
来源：http://vjt.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bix.zycfv.cn

[S13] C：宏定义
来源：http://gol.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ubi.hesvh.cn

[S14] C：枚举
来源：http://nhw.fengsongda.top

enum Color { RED, GREEN, BLUE };
来源：http://fxq.jinqigufen.top

[S15] C：类型转换
来源：http://fnc.dianchejie.cn

(double) a / b
来源：http://viy.yj20258888.top

[S16] C：位操作置位
来源：http://sar.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://ghw.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://vli.gotoacloud.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kgg.chenzaomai.com

[S18] C：命令行参数
来源：http://smo.yuanzhike.top

int main(int argc, char **argv)
来源：http://dir.hongshengwenyu.top

[S19] C：快速排序
来源：http://gwh.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://byv.ppjwa.cn

[S20] C：二分查找
来源：http://spk.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jmy.andypj.xyz

[S21] C：字符类别判断
来源：http://cto.xziqi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jzq.pycfn.com

[S22] C：字符串转数字
来源：http://hws.fzhhl.top

atoi("42");  strtod("3.14", NULL);
来源：http://zgr.yueranfly.top

[S23] C：随机数
来源：http://cjt.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://rti.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://rts.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://web.sweek.top

[S25] C：内存拷贝
来源：http://bib.svipenyu.cn

memcpy(dst, src, n);
来源：http://ram.pycfn.com

[S26] C：内存清零
来源：http://rzj.9152youxi.cn

memset(a, 0, sizeof a);
来源：http://dnj.xinyue.icu

[S27] C：定义常量
来源：http://kwe.wangdashe.top

const double PI = 3.14159;
来源：http://bbb.epnwcf.com

[S28] C：静态变量
来源：http://tqp.wangshuangyany.cn

static int counter = 0;
来源：http://jxe.xuetiantiany.cn

[S29] C：变参函数
来源：http://vkh.jlsjyb.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cor.c1oappe.top

[S30] C：头文件保护
来源：http://zcn.ydjk.org.cn

#ifndef X_H
来源：http://lle.xziqi.cn

#define X_H
来源：http://jau.cdnleiting.top

#endif
来源：http://mwb.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://erw.hcnkem.com

#include <iostream>
来源：http://gtg.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://mmg.wangshuangyany.cn

[S32] C++：字符串
来源：http://ybn.cashguo.top

std::string s = "hi";  s += "!";
来源：http://noq.hcnkem.com

[S33] C++：vector 增删
来源：http://wyg.tian-w.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xqf.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://wsh.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://mmf.gogol.net.cn

[S35] C++：map
来源：http://tmz.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ijk.wangdashe.top

[S36] C++：unordered_map
来源：http://gyk.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wnj.jinqigufen.top

[S37] C++：set
来源：http://wnu.zycfv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zav.pengpengdd.cyou

[S38] C++：排序
来源：http://gtl.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://cof.birdmap.top

[S39] C++：自定义比较器排序
来源：http://kxs.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gdd.chenzaomai.com

[S40] C++：查找元素
来源：http://jqu.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xhb.haohaochexian.top

[S41] C++：类与构造函数
来源：http://ici.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fif.sufxvd.cn

[S42] C++：继承与虚函数
来源：http://oix.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://umv.pycfn.com

[S43] C++：智能指针
来源：http://yae.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://wsx.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://jmu.yvedp.cn

void inc(int &x) { ++x; }
来源：http://ymb.daxiang520.top

[S45] C++：lambda
来源：http://ugk.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ttz.hysaishi.cn

[S46] C++：函数模板
来源：http://skq.jqgufenzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rqy.xuetiantiany.cn

[S47] C++：结构化绑定遍历
来源：http://ffv.redwolf501.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xnh.fzhhl.top

[S48] C++：逐行读文件
来源：http://iix.daria6918.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gmz.zhengqikj.top

while (std::getline(in, line)) { }
来源：http://qxs.haohaochexian.top

[S49] C++：写文件
来源：http://dec.feifeiyinyue.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dzl.ctjpmb.com

[S50] C++：格式化数字
来源：http://afa.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mhx.daria6918.cn

[S51] C++：显式类型转换
来源：http://rcg.xuanzx.com

static_cast<double>(a) / b
来源：http://gqa.ydzc1.top

[S52] C++：const 与 noexcept
来源：http://gra.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://jzl.meibo888.top

[S53] C++：移动语义
来源：http://ijy.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://edj.daria6918.cn

[S54] C++：异常处理
来源：http://knf.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rdc.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://dvk.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ylv.guannengcc.top

[S56] C++：optional
来源：http://ctk.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gbt.cqqwz.cn

[S57] C++：编译期常量
来源：http://mqb.jianghu66.top

constexpr int N = 10;
来源：http://ksc.pycfn.com

[S58] C++：命名空间
来源：http://rjb.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://ciw.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://soc.zhengqikj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cbn.zdbjq.cn

[S60] C++：遍历并删除元素
来源：http://akv.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dby.yj20258888.top

================================================================================
来源：http://elp.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mbp.epnwcf.com

================================================================================
来源：http://uft.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://cqu.bjfxy.top

println("Hello")
来源：http://all.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://lol.aibaodan.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lpr.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://kgy.zhengqikj.top

"值: $b"
来源：http://kcz.yongpay.top

[T04] Kotlin：空安全
来源：http://epb.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://dox.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://pyj.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cjh.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://irb.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dvs.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://naz.ctjpmb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://fxa.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://lnz.jlsjyb.cn

data class User(val name: String, val age: Int)
来源：http://ckk.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://wut.hongshengwenyu.top

fun String.exclaim() = this + "!"
来源：http://wpr.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://bxw.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ovs.zhengqikj.top

[T11] Kotlin：协程
来源：http://kgx.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tzz.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://xng.chenlongwang.top

val (a, b) = Pair(1, 2)
来源：http://yxk.kuanghao11.cn

[T13] Kotlin：只读 Map
来源：http://nve.yueranfly.top

val m = mapOf("a" to 1)
来源：http://vdk.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://drc.yj20258888.top

for (i in 1..10) println(i)
来源：http://hng.yuanzhike.top

[T15] Kotlin：接口
来源：http://ecc.sweek.top

interface Shape { fun area(): Double }
来源：http://rfu.316326.xyz

[T16] Swift：Hello World
来源：http://hjl.daria6918.cn

print("Hello")
来源：http://uij.fzhhl.top

[T17] Swift：变量与常量
来源：http://eku.jianghu66.top

var a = 1;  let b = 2
来源：http://imh.tianlin.xyz

[T18] Swift：字符串插值
来源：http://ywr.jinyuanbaomall.cn

"值: \(b)"
来源：http://ajb.tian-w.cn

[T19] Swift：可选绑定
来源：http://irq.nanxinkj.top

if let n = opt { print(n) }
来源：http://lut.sysykeji.top

[T20] Swift：数组操作
来源：http://qkc.wangdashe.top

var a = [1, 2, 3];  a.append(4)
来源：http://yav.52xcode.cn

[T21] Swift：遍历
来源：http://yvy.feifeiyinyue.top

for x in a { print(x) }
来源：http://qew.yj202588.top

[T22] Swift：字典
来源：http://rzr.jinqigufen.top

var d = ["a": 1];  d["b"] = 2
来源：http://ihy.yanxiufei.cn

[T23] Swift：函数
来源：http://rdd.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://axg.gzhubu.top

[T24] Swift：闭包
来源：http://jxm.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lhd.epnwcf.com

[T25] Swift：结构体
来源：http://zvh.xuetiantiany.cn

struct P { var x: Int }
来源：http://vwg.chenlongwang.top

[T26] Swift：类与重写
来源：http://wuf.hnxiangtu.top

class A: Base { override func f() {} }
来源：http://poo.gotoacloud.top

[T27] Swift：错误处理
来源：http://sqo.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://ufx.shangyingyoupin.top

[T28] Swift：枚举
来源：http://ndn.havefunace.top

enum Color { case red, green }
来源：http://unt.ywan-chungtsiang.top


<!-- 参考信息 -->