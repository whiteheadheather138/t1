代发 wailian999

echo "${#arr[@]}"
来源：http://yua.ivvv.top

[R20] 关联数组（字典）
来源：http://qaq.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://new.xingfuxueyuan.xyz

[R21] 字符串长度
来源：http://cjn.xylfe.cn

echo "${#s}"
来源：http://oei.316326.xyz

[R22] 截取子串
来源：http://beb.ctjpmb.com

echo "${s:0:5}"
来源：http://wge.zhengqikj.top

[R23] 字符串替换
来源：http://oys.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gcg.zdbjq.cn

[R24] 大小写转换
来源：http://rcb.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://szh.quarkkingdee.top

[R25] 去后缀 / 去前缀
来源：http://lin.xuetiantiany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jkp.316326.xyz

[R26] 命令替换
来源：http://dhq.hfpthk.cn

now=$(date +%F); echo "$now"
来源：http://jod.yuxming.cn

[R27] 算术展开
来源：http://nte.ctjpmb.com

echo $((1 + 2 * 3))
来源：http://ftm.zhoulong.xyz

[R28] 浮点运算
来源：http://cng.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://tvb.hongshengwenyu.top

[R29] 定义函数
来源：http://wif.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ine.bjfxy.top

[R30] 函数返回状态码
来源：http://dcv.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://max.wangshuangyany.cn

[R31] 局部变量
来源：http://gjv.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://wqp.sufxvd.cn

[R32] 参数个数校验
来源：http://its.jyoumei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://muh.tanke756.top

[R33] 捕获错误并提示行号
来源：http://wxa.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eph.ctjpmb.com

[R34] 退出时清理
来源：http://rja.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://akb.hnxiangtu.top

[R35] 后台执行并等待
来源：http://nrw.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ypr.epnwcf.com

[R36] 并发执行多个任务
来源：http://hml.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dvu.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://tuf.zycfv.cn

files=$(ls -1)
来源：http://wqw.jinqigfzy.top

[R38] 管道串联
来源：http://dfe.shuidangran.top

cat a.txt | grep -i error | wc -l
来源：http://wog.jyoumei.cn

[R39] 重定向标准输出与错误
来源：http://ihy.ydzc1.top

cmd > out.log 2>&1
来源：http://yvt.shzxlz.cn

[R40] 追加写日志
来源：http://kqp.epnwcf.com

echo "log" >> out.log
来源：http://urj.jiagoushi.top

[R41] 丢弃输出
来源：http://pji.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://chu.gaohongyu789.top

[R42] 输入重定向
来源：http://mtq.mhx1999.top

wc -l < a.txt
来源：http://jen.ctjpmb.com

[R43] 按名字查找文件
来源：http://hub.gogol.net.cn

find . -name "*.log" -type f
来源：http://krq.vehdjk.com

[R44] 按修改时间查找
来源：http://hbp.nwbrower.top

find . -mtime -7 -type f
来源：http://eba.fanxiaobao.xyz

[R45] 批量删除
来源：http://mqj.kuanghao11.cn

find . -name "*.tmp" -delete
来源：http://uxt.wangdashe.top

[R46] 递归替换文件内容
来源：http://fpa.cqqwz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pbd.sweek.top

[R47] sed 单行替换
来源：http://yvq.cucudq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hdv.zhiwuduotai.top

[R48] awk 取指定列
来源：http://kqh.nanxuanxn.top

awk '{print $1, $3}' a.txt
来源：http://lhb.gzhubu.top

[R49] awk 带条件
来源：http://wmv.vqdsnc.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zam.jinghuilouyu.cn

[R50] awk 求和
来源：http://ysv.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://lbp.fengsongda.top

[R51] 排序去重取前几
来源：http://kmf.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vbm.fktsv.cn

[R52] 统计行数
来源：http://xco.zhiwuduotai.top

wc -l a.txt
来源：http://tpl.guannengcc.top

[R53] 查看文件头与实时尾
来源：http://xnf.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ngs.jinqigufen.top

[R54] 比较两个文件
来源：http://nug.shanyushiyangtech.top

diff a.txt b.txt
来源：http://qyk.zdbjq.cn

[R55] 压缩与解压
来源：http://mkj.jinqigufen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ztm.zhixingplan.top

[R56] 远程拷贝
来源：http://ili.shzxlz.cn

scp file user@host:/path/
来源：http://qji.hnqzz.top

[R57] 远程执行命令
来源：http://lgj.jianghu66.top

ssh user@host 'uptime'
来源：http://iws.smart0.xyz

[R58] 下载文件
来源：http://oyt.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fej.tarul.cn

[R59] 发 POST JSON
来源：http://qll.daxiang520.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sao.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://ski.hywenlv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lmf.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://dyu.hysaishi.cn

df -h;  du -sh *
来源：http://ogq.fktsv.cn

[R62] 找最占空间的文件
来源：http://xpg.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://ark.yangfankeji.com

[R63] 内存与进程
来源：http://nca.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://vbt.cqqwz.cn

[R64] 结束进程
来源：http://okp.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://uav.fzhhl.top

[R65] 查看端口占用
来源：http://sjg.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wog.nanxinkj.top

[R66] 定时任务
来源：http://idp.hcnkem.com

crontab -e;  crontab -l
来源：http://awb.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://hds.0kj1m.cn

openssl rand -hex 16
来源：http://vjn.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://dqq.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://dua.yj20258.top

[R69] 生成随机密码
来源：http://ntb.cucudq.cn

head -c 16 /dev/urandom | base64
来源：http://mzq.sufxvd.cn

[R70] 时间戳与互转
来源：http://oui.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://iwb.hcnkem.com

[R71] 日期格式化
来源：http://fwn.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://adm.tarul.cn

[R72] 等待端口就绪
来源：http://byp.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fca.nwbrower.top

[R73] 分割大日志
来源：http://zkf.gaohongyu789.top

split -l 1000 big.log part_
来源：http://ufj.hcnkem.com

[R74] 批量重命名
来源：http://upg.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hsr.hywenlv.cn

[R75] 导出环境变量
来源：http://rek.mhx1999.top

export PATH="$HOME/bin:$PATH"
来源：http://zgc.mhx1999.top

[R76] 使用临时文件
来源：http://pdv.pycfn.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ysm.dashuyun.cn

[R77] 读取用户输入
来源：http://kcz.quarkkingdee.top

read -rp "请输入: " ans
来源：http://ljb.316326.xyz

[R78] 交互式菜单
来源：http://hyq.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://frp.zdqjudy.top

[R79] 解析命令行选项
来源：http://fki.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qqi.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://wfr.fktsv.cn

time ./run.sh
来源：http://cii.tian-w.cn

================================================================================
来源：http://kld.snrcjt.cn

S. C / C++ 专题
来源：http://hpp.yueranfly.top

================================================================================
来源：http://phj.jianghu66.top

[S01] C：Hello World
来源：http://alq.gaohongyu789.top

#include <stdio.h>
来源：http://qos.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hqn.epnwcf.com

[S02] C：变量与格式化输出
来源：http://vsp.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://sug.cdnleiting.top

[S03] C：读入整数
来源：http://ufx.pycfn.com

int x; scanf("%d", &x);
来源：http://xkn.xingfuxueyuan.xyz

[S04] C：字符串复制
来源：http://trx.shangyingyoupin.top

char dst[32]; strcpy(dst, "hi");
来源：http://rnk.gogol.net.cn

[S05] C：字符串长度
来源：http://nuz.feifeiyinyue.top

strlen(s)
来源：http://blk.fehbvm.com

[S06] C：字符串比较
来源：http://pwb.fanxiaobao.xyz

strcmp(a, b) == 0
来源：http://unj.nwbrower.top

[S07] C：数组遍历求和
来源：http://gbq.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zvc.yongpay.top

[S08] C：动态内存分配与释放
来源：http://zhs.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vdo.redwolf501.top

[S09] C：结构体定义与初始化
来源：http://mha.aizwys.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nbs.yj20258888.top

[S10] C：指针与解引用
来源：http://gfc.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://bdt.sxryk.cn

[S11] C：逐行读文件
来源：http://wqc.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://jie.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://tzv.pycfn.com

fclose(f);
来源：http://qul.hcnkem.com

[S12] C：写文件
来源：http://ryq.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dhf.andypj.xyz

[S13] C：宏定义
来源：http://mbn.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xtb.tanke756.top

[S14] C：枚举
来源：http://oxi.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://pbb.yangfankeji.com

[S15] C：类型转换
来源：http://efi.hammf.cn

(double) a / b
来源：http://ogx.sysykeji.top

[S16] C：位操作置位
来源：http://nwf.sweek.top

x |= (1 << 3);
来源：http://fcn.sweek.top

[S17] C：安全拼接字符串
来源：http://jtb.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ksl.hesvh.cn

[S18] C：命令行参数
来源：http://hkm.havefunace.top

int main(int argc, char **argv)
来源：http://owo.wangshuangyany.cn

[S19] C：快速排序
来源：http://qbw.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mvz.pengpengdd.cyou

[S20] C：二分查找
来源：http://och.hysaishi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://snj.zdbjq.cn

[S21] C：字符类别判断
来源：http://tat.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ivs.jlsjyb.cn

[S22] C：字符串转数字
来源：http://wom.feifeiyinyue.top

atoi("42");  strtod("3.14", NULL);
来源：http://tuf.yonumen.top

[S23] C：随机数
来源：http://raf.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qgn.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://xdo.wangshuangyany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ndv.yj20258888.top

[S25] C：内存拷贝
来源：http://inb.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://qdk.daxiang520.top

[S26] C：内存清零
来源：http://pgw.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://che.sufxvd.cn

[S27] C：定义常量
来源：http://lgi.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://ogd.mhx1999.top

[S28] C：静态变量
来源：http://wuf.feifeiyinyue.top

static int counter = 0;
来源：http://gpe.quarkkingdee.top

[S29] C：变参函数
来源：http://wlo.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wkn.chenjidiqi.icu

[S30] C：头文件保护
来源：http://mnq.cucudq.cn

#ifndef X_H
来源：http://jsd.yangfankeji.com

#define X_H
来源：http://vtc.tarul.cn

#endif
来源：http://ajn.zdqjudy.top

[S31] C++：Hello World
来源：http://tly.bbcook.cn

#include <iostream>
来源：http://shc.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://nhg.ybcxt.top

[S32] C++：字符串
来源：http://zkk.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://fze.ydjk.org.cn

[S33] C++：vector 增删
来源：http://yss.daxiang520.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bii.yvedp.cn

[S34] C++：遍历 vector
来源：http://xlk.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://rec.uphjek.com

[S35] C++：map
来源：http://ggm.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mwo.hcnkem.com

[S36] C++：unordered_map
来源：http://ohf.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rqu.daria6918.cn

[S37] C++：set
来源：http://log.zhengqikj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ukk.zhijiandao.cn

[S38] C++：排序
来源：http://jut.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://eqe.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://kyn.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://syk.nanxinkj.top

[S40] C++：查找元素
来源：http://gdg.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hin.hywenlv.cn

[S41] C++：类与构造函数
来源：http://ypo.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://irv.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://awn.yongpay.top

class B : public Base { public: void f() override {} };
来源：http://xlo.316326.xyz

[S43] C++：智能指针
来源：http://ojx.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://dic.chenlongwang.top

[S44] C++：引用传参
来源：http://uif.dianchejie.cn

void inc(int &x) { ++x; }
来源：http://tcg.shzxlz.cn

[S45] C++：lambda
来源：http://zqx.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qyv.dashuyun.cn

[S46] C++：函数模板
来源：http://guj.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://egu.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://oms.bjfxy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kud.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://hoq.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://aul.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://hct.gaohongyu789.top

[S49] C++：写文件
来源：http://cqh.fanxiaobao.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jxr.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://jyo.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wfo.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://jws.hnxiangtu.top

static_cast<double>(a) / b
来源：http://onh.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://jtk.andypj.xyz

int size() const noexcept { return n_; }
来源：http://ira.jinghuilouyu.cn

[S53] C++：移动语义
来源：http://sry.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://bkh.gogol.net.cn

[S54] C++：异常处理
来源：http://dji.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dgr.ivvv.top

[S55] C++：结构化绑定
来源：http://cho.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nlh.gzhubu.top

[S56] C++：optional
来源：http://rpo.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hlz.havefunace.top

[S57] C++：编译期常量
来源：http://qth.gaohongyu789.top

constexpr int N = 10;
来源：http://iiw.yuxming.cn

[S58] C++：命名空间
来源：http://ttu.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://tzr.tarul.cn

[S59] C++：静态断言
来源：http://nlk.yfazqb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zrm.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://usf.epnwcf.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cgs.fengsongda.top

================================================================================
来源：http://xnz.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yhw.cdnleiting.top

================================================================================
来源：http://sin.gaohongyu789.top

[T01] Kotlin：Hello World
来源：http://yqm.meibo888.top

println("Hello")
来源：http://dow.cashguo.top

[T02] Kotlin：变量
来源：http://emv.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gjn.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://msj.sysykeji.top

"值: $b"
来源：http://leg.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://tzb.shangyingyoupin.top

val n: String? = null;  n?.length
来源：http://iny.sysykeji.top

[T05] Kotlin：when 表达式
来源：http://kyb.meibo888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kyx.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://pmf.shanyushiyangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ndp.cashguo.top

[T07] Kotlin：集合过滤
来源：http://kgq.zhengqikj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hgw.jinqigfzy.top

[T08] Kotlin：数据类
来源：http://nox.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://evk.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://vmn.xuanzx.com

fun String.exclaim() = this + "!"
来源：http://cjj.guannengcc.top

[T10] Kotlin：默认参数
来源：http://ydn.yangfankeji.com

fun greet(name: String = "World") = "Hi $name"
来源：http://iwr.wangdashe.top

[T11] Kotlin：协程
来源：http://cyj.nanxinkj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://inh.jianghu66.top

[T12] Kotlin：解构声明
来源：http://hnd.yuxming.cn

val (a, b) = Pair(1, 2)
来源：http://yyq.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://wde.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://xhh.jinqigufen.top

[T14] Kotlin：循环
来源：http://wke.jinqigufen.top

for (i in 1..10) println(i)
来源：http://mgk.jianghu66.top

[T15] Kotlin：接口
来源：http://wbw.aizwys.cn

interface Shape { fun area(): Double }
来源：http://nlo.hnxiangtu.top

[T16] Swift：Hello World
来源：http://ngh.hnqzz.top

print("Hello")
来源：http://yxi.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://oxu.bjfxy.top

var a = 1;  let b = 2
来源：http://hod.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://rjt.sysykeji.top

"值: \(b)"
来源：http://lkh.yangfankeji.com

[T19] Swift：可选绑定
来源：http://gey.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://ckj.9152youxi.cn

[T20] Swift：数组操作
来源：http://kaw.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://dfp.gaohongyu789.top

[T21] Swift：遍历
来源：http://sen.jlsjyb.cn

for x in a { print(x) }
来源：http://ija.hysaishi.cn

[T22] Swift：字典
来源：http://znz.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rbv.meibo888.top


<!-- 参考信息 -->