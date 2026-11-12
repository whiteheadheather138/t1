代发 wailian999

echo "${#arr[@]}"
来源：http://xme.hysaishi.cn

[R20] 关联数组（字典）
来源：http://eis.hnqzz.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lsb.shanyushiyangtech.top

[R21] 字符串长度
来源：http://lvq.xinyue.icu

echo "${#s}"
来源：http://wow.cqqwz.cn

[R22] 截取子串
来源：http://pom.guannengcc.top

echo "${s:0:5}"
来源：http://hnt.nanxuanxn.top

[R23] 字符串替换
来源：http://uzv.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://njg.tianlin.xyz

[R24] 大小写转换
来源：http://rjt.52xcode.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xsh.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://ikz.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://swz.yvedp.cn

[R26] 命令替换
来源：http://zqk.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://wvt.yj20258.top

[R27] 算术展开
来源：http://uot.yj20258.top

echo $((1 + 2 * 3))
来源：http://ltx.sweek.top

[R28] 浮点运算
来源：http://ufh.yfazqb.com

echo "scale=2; 10/3" | bc
来源：http://vce.tanke756.top

[R29] 定义函数
来源：http://ptg.bbcook.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://thf.52xcode.cn

[R30] 函数返回状态码
来源：http://ava.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://hlp.xinyue.icu

[R31] 局部变量
来源：http://pll.gzhubu.top

f() { local x=1; echo "$x"; }
来源：http://qfi.sufxvd.cn

[R32] 参数个数校验
来源：http://lco.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uid.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://ozj.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kic.yueranfly.top

[R34] 退出时清理
来源：http://xuh.vehdjk.com

trap 'rm -f "$tmp"' EXIT
来源：http://poa.tanke756.top

[R35] 后台执行并等待
来源：http://lgq.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zqr.xuanzx.com

[R36] 并发执行多个任务
来源：http://irp.ivvv.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xpa.jlsjyb.cn

[R37] 把输出赋给变量
来源：http://dqa.gotoacloud.top

files=$(ls -1)
来源：http://erh.bjfxy.top

[R38] 管道串联
来源：http://inh.uphjek.com

cat a.txt | grep -i error | wc -l
来源：http://zra.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://cxy.xylfe.cn

cmd > out.log 2>&1
来源：http://ccv.hammf.cn

[R40] 追加写日志
来源：http://urf.yuanzhike.top

echo "log" >> out.log
来源：http://ywu.gogol.net.cn

[R41] 丢弃输出
来源：http://qee.sjlbkw.cn

cmd >/dev/null 2>&1
来源：http://emw.tian-w.cn

[R42] 输入重定向
来源：http://pno.ybcxt.top

wc -l < a.txt
来源：http://vvl.ydzc1.top

[R43] 按名字查找文件
来源：http://hln.zhijiandao.cn

find . -name "*.log" -type f
来源：http://bup.uphjek.com

[R44] 按修改时间查找
来源：http://vtz.ehwqpu.com

find . -mtime -7 -type f
来源：http://lxq.xziqi.cn

[R45] 批量删除
来源：http://ujh.zhongyouzk.top

find . -name "*.tmp" -delete
来源：http://xyu.ybcxt.top

[R46] 递归替换文件内容
来源：http://ekl.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yzc.jinqigufen.top

[R47] sed 单行替换
来源：http://ksn.mhx1999.top

sed -i 's/foo/bar/g' a.txt
来源：http://coi.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://nqt.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://ehy.snrcjt.cn

[R49] awk 带条件
来源：http://ctp.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ucy.jinyuanbaomall.cn

[R50] awk 求和
来源：http://wzt.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wmw.hywenlv.cn

[R51] 排序去重取前几
来源：http://oqb.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fpr.zhijiandao.cn

[R52] 统计行数
来源：http://chy.dianchejie.cn

wc -l a.txt
来源：http://dmu.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://uhd.hywenlv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eyh.tarul.cn

[R54] 比较两个文件
来源：http://vyq.feifeiyinyue.top

diff a.txt b.txt
来源：http://uol.vqdsnc.cn

[R55] 压缩与解压
来源：http://wim.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://owj.feifeiyinyue.top

[R56] 远程拷贝
来源：http://erp.cucudq.cn

scp file user@host:/path/
来源：http://wai.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://irc.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://iya.cashguo.top

[R58] 下载文件
来源：http://yzc.smart0.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tbg.jqgufenzy.top

[R59] 发 POST JSON
来源：http://auv.cucudq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dcp.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://gde.ydjk.org.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qhr.yonumen.top

[R61] 磁盘占用
来源：http://mlq.316326.xyz

df -h;  du -sh *
来源：http://rlr.xuanzx.com

[R62] 找最占空间的文件
来源：http://rkw.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://anu.iojbl.cn

[R63] 内存与进程
来源：http://cot.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://bnp.wangdashe.top

[R64] 结束进程
来源：http://ugr.gaohongyu789.top

kill -9 $(pgrep -f app.py)
来源：http://dpu.chenzaomai.com

[R65] 查看端口占用
来源：http://siy.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mom.nanxuanxn.top

[R66] 定时任务
来源：http://gdh.jianghu66.top

crontab -e;  crontab -l
来源：http://idg.sysykeji.top

[R67] 生成随机十六进制串
来源：http://nla.jqgufenzy.top

openssl rand -hex 16
来源：http://bnv.daxiang520.top

[R68] 计算文件校验值
来源：http://zvy.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mny.fzhhl.top

[R69] 生成随机密码
来源：http://zmg.hnqzz.top

head -c 16 /dev/urandom | base64
来源：http://cmx.jinqigufen.top

[R70] 时间戳与互转
来源：http://dyp.nanxinkj.top

date +%s;  date -d @1700000000
来源：http://bqa.cashguo.top

[R71] 日期格式化
来源：http://zzy.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kyt.zhengqikj.top

[R72] 等待端口就绪
来源：http://kns.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uub.nanxuanxn.top

[R73] 分割大日志
来源：http://dup.jqgufenzy.top

split -l 1000 big.log part_
来源：http://mfp.iojbl.cn

[R74] 批量重命名
来源：http://xzn.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xyh.bjfxy.top

[R75] 导出环境变量
来源：http://tsr.316326.xyz

export PATH="$HOME/bin:$PATH"
来源：http://sxg.cucudq.cn

[R76] 使用临时文件
来源：http://iof.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cnl.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://rdn.jiagoushi.top

read -rp "请输入: " ans
来源：http://uvo.cdnleiting.top

[R78] 交互式菜单
来源：http://llw.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ers.gogol.net.cn

[R79] 解析命令行选项
来源：http://jcp.jyoumei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gms.havefunace.top

[R80] 查看脚本执行耗时
来源：http://fac.wangshuangyany.cn

time ./run.sh
来源：http://vji.sufxvd.cn

================================================================================
来源：http://rbl.xuetiantiany.cn

S. C / C++ 专题
来源：http://qjt.yongpay.top

================================================================================
来源：http://itl.jqgfzy.top

[S01] C：Hello World
来源：http://xae.jqgufenzy.top

#include <stdio.h>
来源：http://yki.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bir.andypj.xyz

[S02] C：变量与格式化输出
来源：http://sah.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://ofa.jinqigufen.top

[S03] C：读入整数
来源：http://cha.nanxuanxn.top

int x; scanf("%d", &x);
来源：http://vxb.ybcxt.top

[S04] C：字符串复制
来源：http://bmd.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://plb.cheryme.top

[S05] C：字符串长度
来源：http://tnd.316326.xyz

strlen(s)
来源：http://xzv.sxryk.cn

[S06] C：字符串比较
来源：http://eea.xylfe.cn

strcmp(a, b) == 0
来源：http://eqs.sweek.top

[S07] C：数组遍历求和
来源：http://rxg.c1oappe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hdd.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://hqg.guannengcc.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hhz.hysaishi.cn

[S09] C：结构体定义与初始化
来源：http://dry.yangfankeji.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fam.fzhhl.top

[S10] C：指针与解引用
来源：http://ilb.shuidangran.top

int *p = &a;  *p = 5;
来源：http://zjw.chenzaomai.com

[S11] C：逐行读文件
来源：http://vzs.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://qgq.svipenyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pfs.jinqigufen.top

fclose(f);
来源：http://wyx.zhoulong.xyz

[S12] C：写文件
来源：http://qnz.vqdsnc.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://naq.chenjidiqi.icu

[S13] C：宏定义
来源：http://prx.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kke.gogol.net.cn

[S14] C：枚举
来源：http://ydt.sysykeji.top

enum Color { RED, GREEN, BLUE };
来源：http://dus.chenjidiqi.icu

[S15] C：类型转换
来源：http://pnt.daria6918.cn

(double) a / b
来源：http://buv.birdmap.top

[S16] C：位操作置位
来源：http://pvs.zhongyouzk.top

x |= (1 << 3);
来源：http://qmc.zdbjq.cn

[S17] C：安全拼接字符串
来源：http://hhf.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ucc.jinqigufen.top

[S18] C：命令行参数
来源：http://diy.hnqzz.top

int main(int argc, char **argv)
来源：http://alq.ppjwa.cn

[S19] C：快速排序
来源：http://lpp.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://hza.daxiang520.top

[S20] C：二分查找
来源：http://pre.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bvy.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://ssf.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://frh.cdnleiting.top

[S22] C：字符串转数字
来源：http://hgh.mhx1999.top

atoi("42");  strtod("3.14", NULL);
来源：http://ulh.daria6918.cn

[S23] C：随机数
来源：http://uea.gotoacloud.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nbx.0kj1m.cn

[S24] C：获取本地时间
来源：http://ero.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://chr.kuanghao11.cn

[S25] C：内存拷贝
来源：http://ekk.hongshengwenyu.top

memcpy(dst, src, n);
来源：http://rhn.quarkkingdee.top

[S26] C：内存清零
来源：http://hfx.havefunace.top

memset(a, 0, sizeof a);
来源：http://czs.sjlbkw.cn

[S27] C：定义常量
来源：http://yep.yvedp.cn

const double PI = 3.14159;
来源：http://hdq.hysaishi.cn

[S28] C：静态变量
来源：http://isl.yanxiufei.cn

static int counter = 0;
来源：http://com.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://oap.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qtx.ehwqpu.com

[S30] C：头文件保护
来源：http://qbn.dianchejie.cn

#ifndef X_H
来源：http://wpi.yanxiufei.cn

#define X_H
来源：http://acr.xuetiantiany.cn

#endif
来源：http://njh.yj20258888.top

[S31] C++：Hello World
来源：http://twj.daxiang520.top

#include <iostream>
来源：http://waf.shzxlz.cn

int main() { std::cout << "Hello\n"; }
来源：http://umi.vqdsnc.cn

[S32] C++：字符串
来源：http://hta.shanyushiyangtech.top

std::string s = "hi";  s += "!";
来源：http://wgo.xuanzx.com

[S33] C++：vector 增删
来源：http://kqi.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ppf.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://sta.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://fmt.svipenyu.cn

[S35] C++：map
来源：http://hhu.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kxy.sjlbkw.cn

[S36] C++：unordered_map
来源：http://rxj.xylfe.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cft.jiagoushi.top

[S37] C++：set
来源：http://cjo.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ebi.ybcxt.top

[S38] C++：排序
来源：http://edo.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://leg.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://zus.pengpengdd.cyou

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oez.tarul.cn

[S40] C++：查找元素
来源：http://omw.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://veh.hcnkem.com

[S41] C++：类与构造函数
来源：http://alb.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qjm.tian-w.cn

[S42] C++：继承与虚函数
来源：http://jei.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://lhm.xuanzx.com

[S43] C++：智能指针
来源：http://lsl.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://dyu.birdmap.top

[S44] C++：引用传参
来源：http://gfq.gzhubu.top

void inc(int &x) { ++x; }
来源：http://dqm.zycfv.cn

[S45] C++：lambda
来源：http://ngx.zhaomingkeji.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://yrz.xuanzx.com

[S46] C++：函数模板
来源：http://yxq.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xcw.yj20258888.top

[S47] C++：结构化绑定遍历
来源：http://urm.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kcf.svipenyu.cn

[S48] C++：逐行读文件
来源：http://adq.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qma.ydjk.org.cn

while (std::getline(in, line)) { }
来源：http://cmb.52xcode.cn

[S49] C++：写文件
来源：http://gab.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lgj.shuidangran.top

[S50] C++：格式化数字
来源：http://hvo.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rlu.guannengcc.top

[S51] C++：显式类型转换
来源：http://irn.yvedp.cn

static_cast<double>(a) / b
来源：http://niv.yj202588.top

[S52] C++：const 与 noexcept
来源：http://qty.ydzc1.top

int size() const noexcept { return n_; }
来源：http://ahw.gotoacloud.top

[S53] C++：移动语义
来源：http://svr.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://nby.jyoumei.cn

[S54] C++：异常处理
来源：http://osx.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sck.xylfe.cn

[S55] C++：结构化绑定
来源：http://erc.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zws.tanke756.top

[S56] C++：optional
来源：http://ces.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rrr.jiagoushi.top

[S57] C++：编译期常量
来源：http://igk.daxiang520.top

constexpr int N = 10;
来源：http://cxz.yvedp.cn

[S58] C++：命名空间
来源：http://mnt.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://tzf.yuxming.cn

[S59] C++：静态断言
来源：http://pub.zhoulong.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://htq.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://qxl.yangfankeji.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cnh.daxiang520.top

================================================================================
来源：http://jej.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hkg.jiagoushi.top

================================================================================
来源：http://umk.zhaomingkeji.xyz

[T01] Kotlin：Hello World
来源：http://yrm.shzxlz.cn

println("Hello")
来源：http://muh.shzxlz.cn

[T02] Kotlin：变量
来源：http://isy.jinghuilouyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yhj.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://auu.quarkkingdee.top

"值: $b"
来源：http://fed.fktsv.cn

[T04] Kotlin：空安全
来源：http://gmz.fehbvm.com

val n: String? = null;  n?.length
来源：http://dlj.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://hvv.dashuyun.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rrv.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://yau.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vvj.yonumen.top

[T07] Kotlin：集合过滤
来源：http://llo.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sfu.hcnkem.com

[T08] Kotlin：数据类
来源：http://kuh.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://rra.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://vys.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://owp.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://vfl.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://imc.bbcook.cn

[T11] Kotlin：协程
来源：http://cvm.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://blp.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://crq.shanyushiyangkeji.top

val (a, b) = Pair(1, 2)
来源：http://tqg.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://ljy.pycfn.com

val m = mapOf("a" to 1)
来源：http://krn.shuidangran.top

[T14] Kotlin：循环
来源：http://qrl.zhixingplan.top

for (i in 1..10) println(i)
来源：http://tmz.sjlbkw.cn

[T15] Kotlin：接口
来源：http://eft.fktsv.cn

interface Shape { fun area(): Double }
来源：http://rqk.bbcook.cn

[T16] Swift：Hello World
来源：http://jst.hesvh.cn

print("Hello")
来源：http://nmk.redwolf501.top

[T17] Swift：变量与常量
来源：http://rpw.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://ttg.dianchejie.cn

[T18] Swift：字符串插值
来源：http://nce.yj20258888.top

"值: \(b)"
来源：http://utu.ybcxt.top

[T19] Swift：可选绑定
来源：http://rmp.fengsongda.top

if let n = opt { print(n) }
来源：http://uaq.jianghu66.top

[T20] Swift：数组操作
来源：http://ucx.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://rnw.xuetiantiany.cn

[T21] Swift：遍历
来源：http://zqj.zdqjudy.top

for x in a { print(x) }
来源：http://gce.zdqjudy.top

[T22] Swift：字典
来源：http://rku.haohaochexian.top

var d = ["a": 1];  d["b"] = 2
来源：http://tji.nanxuanxn.top


<!-- 参考信息 -->