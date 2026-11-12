代发 wailian999

echo "${#s}"
来源：http://vva.vqdsnc.cn

[R22] 截取子串
来源：http://dsj.kuanghao11.cn

echo "${s:0:5}"
来源：http://yjj.sjlbkw.cn

[R23] 字符串替换
来源：http://nvr.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://afw.jinqigufen.top

[R24] 大小写转换
来源：http://jxb.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://wbk.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://kxh.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://mwm.ivvv.top

[R26] 命令替换
来源：http://jvt.cheryme.top

now=$(date +%F); echo "$now"
来源：http://epv.uphjek.com

[R27] 算术展开
来源：http://ojg.aizwys.cn

echo $((1 + 2 * 3))
来源：http://lsl.sweek.top

[R28] 浮点运算
来源：http://vvf.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://myr.nanxuanxn.top

[R29] 定义函数
来源：http://mkw.hesvh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lmu.xylfe.cn

[R30] 函数返回状态码
来源：http://wlx.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://lnz.hfpthk.cn

[R31] 局部变量
来源：http://wbi.xuanzx.com

f() { local x=1; echo "$x"; }
来源：http://rvq.0kj1m.cn

[R32] 参数个数校验
来源：http://bht.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fos.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://gpc.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fwe.gzhubu.top

[R34] 退出时清理
来源：http://xvo.ctjpmb.com

trap 'rm -f "$tmp"' EXIT
来源：http://cor.ppjwa.cn

[R35] 后台执行并等待
来源：http://cpx.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xzf.zhengqikj.top

[R36] 并发执行多个任务
来源：http://udv.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://owd.jinqigufen.top

[R37] 把输出赋给变量
来源：http://ufp.aizwys.cn

files=$(ls -1)
来源：http://cqt.fzhhl.top

[R38] 管道串联
来源：http://rol.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://vwk.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://qem.ydzc1.top

cmd > out.log 2>&1
来源：http://tfp.wangshuangyany.cn

[R40] 追加写日志
来源：http://tfd.daxiang520.top

echo "log" >> out.log
来源：http://zhq.guowangkeji.top

[R41] 丢弃输出
来源：http://daw.snrcjt.cn

cmd >/dev/null 2>&1
来源：http://hyp.redwolf501.top

[R42] 输入重定向
来源：http://zxw.jinyuanbaomall.cn

wc -l < a.txt
来源：http://tnk.316326.xyz

[R43] 按名字查找文件
来源：http://qfc.c1oappe.top

find . -name "*.log" -type f
来源：http://hpe.sufxvd.cn

[R44] 按修改时间查找
来源：http://uys.jiagoushi.top

find . -mtime -7 -type f
来源：http://glh.ywan-chungtsiang.top

[R45] 批量删除
来源：http://ude.zdbjq.cn

find . -name "*.tmp" -delete
来源：http://tjt.c1oappe.top

[R46] 递归替换文件内容
来源：http://wjs.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eff.fktsv.cn

[R47] sed 单行替换
来源：http://cya.ydzc1.top

sed -i 's/foo/bar/g' a.txt
来源：http://gpw.cashguo.top

[R48] awk 取指定列
来源：http://ldg.shzxlz.cn

awk '{print $1, $3}' a.txt
来源：http://euo.xziqi.cn

[R49] awk 带条件
来源：http://miv.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mxy.fanxiaobao.xyz

[R50] awk 求和
来源：http://aie.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ujt.yfazqb.com

[R51] 排序去重取前几
来源：http://kog.xinyue.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://egm.c1oappe.top

[R52] 统计行数
来源：http://pzh.zhongyouzk.top

wc -l a.txt
来源：http://lwd.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://vfr.feifeiyinyue.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fxq.yangfankeji.com

[R54] 比较两个文件
来源：http://bbl.yanxiufei.cn

diff a.txt b.txt
来源：http://bks.feifeiyinyue.top

[R55] 压缩与解压
来源：http://leu.chenlongwang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ssd.fengsongda.top

[R56] 远程拷贝
来源：http://ikx.yfazqb.com

scp file user@host:/path/
来源：http://xss.zhiwuduotai.top

[R57] 远程执行命令
来源：http://rjf.yanxiufei.cn

ssh user@host 'uptime'
来源：http://dwz.gogol.net.cn

[R58] 下载文件
来源：http://vmv.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xdk.gotoacloud.top

[R59] 发 POST JSON
来源：http://jrq.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oyd.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://wtd.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jkv.hcnkem.com

[R61] 磁盘占用
来源：http://qjf.ivvv.top

df -h;  du -sh *
来源：http://dor.hnxiangtu.top

[R62] 找最占空间的文件
来源：http://auv.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://ylv.aibaodan.cn

[R63] 内存与进程
来源：http://wnv.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://blo.zhongyouzk.top

[R64] 结束进程
来源：http://hft.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://psq.pengpengdd.cyou

[R65] 查看端口占用
来源：http://cbw.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sgl.52xcode.cn

[R66] 定时任务
来源：http://fco.tarul.cn

crontab -e;  crontab -l
来源：http://emv.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://bat.yfazqb.com

openssl rand -hex 16
来源：http://maa.cashguo.top

[R68] 计算文件校验值
来源：http://via.jiagoushi.top

sha256sum a.txt;  md5sum a.txt
来源：http://etm.c1oappe.top

[R69] 生成随机密码
来源：http://vlq.xinyue.icu

head -c 16 /dev/urandom | base64
来源：http://oop.guannengcc.top

[R70] 时间戳与互转
来源：http://efi.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://fto.nwbrower.top

[R71] 日期格式化
来源：http://lix.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://kxy.yongpay.top

[R72] 等待端口就绪
来源：http://hrd.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ijv.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://tgu.zhijiandao.cn

split -l 1000 big.log part_
来源：http://xsg.nwbrower.top

[R74] 批量重命名
来源：http://gsc.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://idp.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://eop.svipenyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://bky.pengpengdd.cyou

[R76] 使用临时文件
来源：http://rro.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://une.haohaochexian.top

[R77] 读取用户输入
来源：http://ubl.c1oappe.top

read -rp "请输入: " ans
来源：http://qpk.yj202588.top

[R78] 交互式菜单
来源：http://nln.sjlbkw.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://frk.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://ges.yonumen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cyq.jyoumei.cn

[R80] 查看脚本执行耗时
来源：http://apt.jinqigfzy.top

time ./run.sh
来源：http://htx.tarul.cn

================================================================================
来源：http://tzf.sysykeji.top

S. C / C++ 专题
来源：http://agm.xuetiantiany.cn

================================================================================
来源：http://pio.shuidangran.top

[S01] C：Hello World
来源：http://ixx.tanke756.top

#include <stdio.h>
来源：http://vys.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vhj.zhiwuduotai.top

[S02] C：变量与格式化输出
来源：http://bqk.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://mpd.sxryk.cn

[S03] C：读入整数
来源：http://rcx.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://vpq.jlsjyb.cn

[S04] C：字符串复制
来源：http://cyx.aibaodan.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cjp.snrcjt.cn

[S05] C：字符串长度
来源：http://nqv.wangdashe.top

strlen(s)
来源：http://mmo.yj20258888.top

[S06] C：字符串比较
来源：http://xrq.jinghuilouyu.cn

strcmp(a, b) == 0
来源：http://bgu.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://gfp.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uew.hysaishi.cn

[S08] C：动态内存分配与释放
来源：http://tey.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lmf.cucudq.cn

[S09] C：结构体定义与初始化
来源：http://ikb.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ggx.yj20258.top

[S10] C：指针与解引用
来源：http://qtq.ybcxt.top

int *p = &a;  *p = 5;
来源：http://apd.nwbrower.top

[S11] C：逐行读文件
来源：http://sfv.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://eln.sufxvd.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fye.zhoulong.xyz

fclose(f);
来源：http://gkt.xziqi.cn

[S12] C：写文件
来源：http://eju.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qzf.chenzaomai.com

[S13] C：宏定义
来源：http://gzh.316326.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zwu.shzxlz.cn

[S14] C：枚举
来源：http://myh.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://umv.tianlin.xyz

[S15] C：类型转换
来源：http://azh.sxryk.cn

(double) a / b
来源：http://ynz.tian-w.cn

[S16] C：位操作置位
来源：http://nzh.yongpay.top

x |= (1 << 3);
来源：http://ajv.pycfn.com

[S17] C：安全拼接字符串
来源：http://ggv.kuanghao11.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nzr.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://njo.quarkkingdee.top

int main(int argc, char **argv)
来源：http://zvo.aibaodan.cn

[S19] C：快速排序
来源：http://biz.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://pzg.jinqigufen.top

[S20] C：二分查找
来源：http://esp.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gfh.ywan-chungtsiang.top

[S21] C：字符类别判断
来源：http://wfr.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gnp.hammf.cn

[S22] C：字符串转数字
来源：http://fep.wangshuangyany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wsf.sysykeji.top

[S23] C：随机数
来源：http://jzk.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ovj.ydzc1.top

[S24] C：获取本地时间
来源：http://hmw.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aij.hnqzz.top

[S25] C：内存拷贝
来源：http://goc.cheryme.top

memcpy(dst, src, n);
来源：http://yrq.yanxiufei.cn

[S26] C：内存清零
来源：http://adb.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://sih.epnwcf.com

[S27] C：定义常量
来源：http://hvc.yongpay.top

const double PI = 3.14159;
来源：http://cma.hnqzz.top

[S28] C：静态变量
来源：http://osj.ehwqpu.com

static int counter = 0;
来源：http://ope.316326.xyz

[S29] C：变参函数
来源：http://xez.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dlo.jqgufenzy.top

[S30] C：头文件保护
来源：http://fjl.hammf.cn

#ifndef X_H
来源：http://vrg.zhengqikj.top

#define X_H
来源：http://fcr.shangyingyoupin.top

#endif
来源：http://otp.vehdjk.com

[S31] C++：Hello World
来源：http://qnw.daxiang520.top

#include <iostream>
来源：http://ylk.jinqigufen.top

int main() { std::cout << "Hello\n"; }
来源：http://stz.tarul.cn

[S32] C++：字符串
来源：http://ehj.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://uxs.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://sbm.sysykeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ngu.epnwcf.com

[S34] C++：遍历 vector
来源：http://imn.hfpthk.cn

for (auto &x : v) { std::cout << x; }
来源：http://uks.yangfankeji.com

[S35] C++：map
来源：http://fia.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cgl.nanxuanxn.top

[S36] C++：unordered_map
来源：http://dbg.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jns.ctjpmb.com

[S37] C++：set
来源：http://hnk.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ilz.hammf.cn

[S38] C++：排序
来源：http://aoy.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://zet.zhoulong.xyz

[S39] C++：自定义比较器排序
来源：http://zbp.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mqe.yueranfly.top

[S40] C++：查找元素
来源：http://nlr.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xmc.jqgufenzy.top

[S41] C++：类与构造函数
来源：http://bvj.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://noi.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://dhb.hesvh.cn

class B : public Base { public: void f() override {} };
来源：http://qxy.tian-w.cn

[S43] C++：智能指针
来源：http://zgj.hesvh.cn

auto p = std::make_unique<int>(5);
来源：http://ggj.quarkkingdee.top

[S44] C++：引用传参
来源：http://ses.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://jwg.xuanzx.com

[S45] C++：lambda
来源：http://sht.cdnleiting.top

auto add = [](int a, int b) { return a + b; };
来源：http://xmb.0kj1m.cn

[S46] C++：函数模板
来源：http://xjl.jinqigufen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bne.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://rhl.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mjh.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://vtl.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://dwe.hnqzz.top

while (std::getline(in, line)) { }
来源：http://yhj.dashuyun.cn

[S49] C++：写文件
来源：http://ztk.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hvz.daria6918.cn

[S50] C++：格式化数字
来源：http://rtj.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rma.birdmap.top

[S51] C++：显式类型转换
来源：http://myc.52xcode.cn

static_cast<double>(a) / b
来源：http://ueu.hammf.cn

[S52] C++：const 与 noexcept
来源：http://qmf.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://uhi.jinqigufen.top

[S53] C++：移动语义
来源：http://qls.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://tcd.yvedp.cn

[S54] C++：异常处理
来源：http://jdv.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lyk.xziqi.cn

[S55] C++：结构化绑定
来源：http://ogs.pycfn.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ybr.fehbvm.com

[S56] C++：optional
来源：http://lij.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ffh.snrcjt.cn

[S57] C++：编译期常量
来源：http://ydk.zdqjudy.top

constexpr int N = 10;
来源：http://zni.hnxiangtu.top

[S58] C++：命名空间
来源：http://xgk.wangshuangyany.cn

namespace ns { int f() { return 1; } }
来源：http://xjv.tianlin.xyz

[S59] C++：静态断言
来源：http://pwn.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wfm.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://wfz.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jfp.jinqigfzy.top

================================================================================
来源：http://gzc.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zko.yongpay.top

================================================================================
来源：http://tlq.c1oappe.top

[T01] Kotlin：Hello World
来源：http://yzh.nwbrower.top

println("Hello")
来源：http://jys.tarul.cn

[T02] Kotlin：变量
来源：http://ezf.meibo888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hmj.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://tlp.ctjpmb.com

"值: $b"
来源：http://keu.jinqigufen.top

[T04] Kotlin：空安全
来源：http://afi.tian-w.cn

val n: String? = null;  n?.length
来源：http://jrj.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://nww.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hla.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://hng.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mca.52xcode.cn

[T07] Kotlin：集合过滤
来源：http://uis.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://rlk.zdqjudy.top

[T08] Kotlin：数据类
来源：http://yeu.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://jfe.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://fps.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://umy.birdmap.top

[T10] Kotlin：默认参数
来源：http://pjh.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ldk.vehdjk.com

[T11] Kotlin：协程
来源：http://cby.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rgt.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://rnp.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://mrp.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://hmj.uphjek.com

val m = mapOf("a" to 1)
来源：http://cqc.jlsjyb.cn

[T14] Kotlin：循环
来源：http://ahz.cdnleiting.top

for (i in 1..10) println(i)
来源：http://nff.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://gyq.zhaomingkeji.xyz

interface Shape { fun area(): Double }
来源：http://ctd.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://zsb.vehdjk.com

print("Hello")
来源：http://ssh.yangfankeji.com

[T17] Swift：变量与常量
来源：http://tcm.vqdsnc.cn

var a = 1;  let b = 2
来源：http://pjq.zhixingplan.top

[T18] Swift：字符串插值
来源：http://qwk.zhaomingkeji.xyz

"值: \(b)"
来源：http://wzy.hysaishi.cn

[T19] Swift：可选绑定
来源：http://eoh.xuanzx.com

if let n = opt { print(n) }
来源：http://ivm.ybcxt.top

[T20] Swift：数组操作
来源：http://hqv.cashguo.top

var a = [1, 2, 3];  a.append(4)
来源：http://lwb.yfazqb.com

[T21] Swift：遍历
来源：http://xfr.zhiwuduotai.top

for x in a { print(x) }
来源：http://fql.gogol.net.cn

[T22] Swift：字典
来源：http://kpu.zhijiandao.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rjz.tarul.cn

[T23] Swift：函数
来源：http://skx.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kzp.yanxiufei.cn

[T24] Swift：闭包
来源：http://huf.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://wig.jianghu66.top


<!-- 参考信息 -->