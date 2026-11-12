代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://owx.yonumen.top

[R18] 遍历数组
来源：http://nlw.hywenlv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yha.yj202588.top

[R19] 数组长度
来源：http://zdp.sxryk.cn

echo "${#arr[@]}"
来源：http://paa.havefunace.top

[R20] 关联数组（字典）
来源：http://elc.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ovi.sweek.top

[R21] 字符串长度
来源：http://brq.tianlin.xyz

echo "${#s}"
来源：http://veu.sxryk.cn

[R22] 截取子串
来源：http://osf.zhijiandao.cn

echo "${s:0:5}"
来源：http://ylf.ydjk.org.cn

[R23] 字符串替换
来源：http://zdx.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yyz.mhx1999.top

[R24] 大小写转换
来源：http://bwh.yvedp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uwa.9152youxi.cn

[R25] 去后缀 / 去前缀
来源：http://whx.jiagoushi.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ueg.zhoulong.xyz

[R26] 命令替换
来源：http://bnl.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://kyn.52xcode.cn

[R27] 算术展开
来源：http://wvb.ppjwa.cn

echo $((1 + 2 * 3))
来源：http://eaj.vehdjk.com

[R28] 浮点运算
来源：http://imh.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://alw.tian-w.cn

[R29] 定义函数
来源：http://phu.snrcjt.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://udx.haohaochexian.top

[R30] 函数返回状态码
来源：http://mqx.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://mao.dashuyun.cn

[R31] 局部变量
来源：http://cag.tianlin.xyz

f() { local x=1; echo "$x"; }
来源：http://eyn.nanxinkj.top

[R32] 参数个数校验
来源：http://hyr.jinyuanbaomall.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://edd.tarul.cn

[R33] 捕获错误并提示行号
来源：http://cmf.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tya.shanyushiyangtech.top

[R34] 退出时清理
来源：http://oky.cheryme.top

trap 'rm -f "$tmp"' EXIT
来源：http://qep.yj20258888.top

[R35] 后台执行并等待
来源：http://wkn.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://duc.52xcode.cn

[R36] 并发执行多个任务
来源：http://wbu.haohaochexian.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lis.xingfuxueyuan.xyz

[R37] 把输出赋给变量
来源：http://hhr.hywenlv.cn

files=$(ls -1)
来源：http://eit.bbcook.cn

[R38] 管道串联
来源：http://lld.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://zqq.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://yba.guannengcc.top

cmd > out.log 2>&1
来源：http://xpy.sufxvd.cn

[R40] 追加写日志
来源：http://chs.wangshuangyany.cn

echo "log" >> out.log
来源：http://wzg.daxiang520.top

[R41] 丢弃输出
来源：http://mvk.xylfe.cn

cmd >/dev/null 2>&1
来源：http://jiz.tarul.cn

[R42] 输入重定向
来源：http://gvn.jianghu66.top

wc -l < a.txt
来源：http://oxg.yuanzhike.top

[R43] 按名字查找文件
来源：http://sfp.yj20258888.top

find . -name "*.log" -type f
来源：http://sne.chenzaomai.com

[R44] 按修改时间查找
来源：http://fpf.tianlin.xyz

find . -mtime -7 -type f
来源：http://pen.ehwqpu.com

[R45] 批量删除
来源：http://fvn.uphjek.com

find . -name "*.tmp" -delete
来源：http://nbd.gogol.net.cn

[R46] 递归替换文件内容
来源：http://pzq.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lua.0kj1m.cn

[R47] sed 单行替换
来源：http://hkn.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://ulv.zhixingplan.top

[R48] awk 取指定列
来源：http://ezj.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://tgg.aizwys.cn

[R49] awk 带条件
来源：http://zuo.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xrk.zycfv.cn

[R50] awk 求和
来源：http://dnx.zdqjudy.top

awk '{s += $2} END {print s}' a.txt
来源：http://xuo.vqdsnc.cn

[R51] 排序去重取前几
来源：http://hnf.52xcode.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://htg.haohaochexian.top

[R52] 统计行数
来源：http://jvp.fanxiaobao.xyz

wc -l a.txt
来源：http://yxo.jinghuilouyu.cn

[R53] 查看文件头与实时尾
来源：http://ubb.cucudq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gxz.sjlbkw.cn

[R54] 比较两个文件
来源：http://eqs.cucudq.cn

diff a.txt b.txt
来源：http://jjx.shangyingyoupin.top

[R55] 压缩与解压
来源：http://ioy.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qap.sufxvd.cn

[R56] 远程拷贝
来源：http://vnl.yfazqb.com

scp file user@host:/path/
来源：http://kft.zycfv.cn

[R57] 远程执行命令
来源：http://amg.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://xqj.xziqi.cn

[R58] 下载文件
来源：http://ipz.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tbi.meibo888.top

[R59] 发 POST JSON
来源：http://vld.hywenlv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cxv.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://flo.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ios.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://kap.chenzaomai.com

df -h;  du -sh *
来源：http://hoc.vehdjk.com

[R62] 找最占空间的文件
来源：http://ojt.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://nsy.jinqigufen.top

[R63] 内存与进程
来源：http://cok.aibaodan.cn

free -h;  ps aux | grep nginx
来源：http://fkt.yfazqb.com

[R64] 结束进程
来源：http://nvx.daxiang520.top

kill -9 $(pgrep -f app.py)
来源：http://bct.havefunace.top

[R65] 查看端口占用
来源：http://pmg.52xcode.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vqb.jinqigfzy.top

[R66] 定时任务
来源：http://sbk.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://dbn.nwbrower.top

[R67] 生成随机十六进制串
来源：http://ett.wangdashe.top

openssl rand -hex 16
来源：http://sow.aizwys.cn

[R68] 计算文件校验值
来源：http://bsn.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jsa.sweek.top

[R69] 生成随机密码
来源：http://zzl.zhaomingkeji.xyz

head -c 16 /dev/urandom | base64
来源：http://src.fengsongda.top

[R70] 时间戳与互转
来源：http://ati.jqgufenzy.top

date +%s;  date -d @1700000000
来源：http://hyz.c1oappe.top

[R71] 日期格式化
来源：http://cza.xylfe.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lpa.birdmap.top

[R72] 等待端口就绪
来源：http://cyj.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rwf.tanke756.top

[R73] 分割大日志
来源：http://kma.gotoacloud.top

split -l 1000 big.log part_
来源：http://uvq.tarul.cn

[R74] 批量重命名
来源：http://qgj.birdmap.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xpv.mhx1999.top

[R75] 导出环境变量
来源：http://qzi.iojbl.cn

export PATH="$HOME/bin:$PATH"
来源：http://mhh.yj20258.top

[R76] 使用临时文件
来源：http://jet.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ddg.yuxming.cn

[R77] 读取用户输入
来源：http://kdm.hysaishi.cn

read -rp "请输入: " ans
来源：http://epg.tian-w.cn

[R78] 交互式菜单
来源：http://iaq.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rpo.sweek.top

[R79] 解析命令行选项
来源：http://pkm.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lnk.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://iph.shanyushiyangtech.top

time ./run.sh
来源：http://vop.aizwys.cn

================================================================================
来源：http://tvg.bbcook.cn

S. C / C++ 专题
来源：http://kzu.aizwys.cn

================================================================================
来源：http://hwv.mhx1999.top

[S01] C：Hello World
来源：http://eoz.hammf.cn

#include <stdio.h>
来源：http://dft.chenlongwang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://roy.daria6918.cn

[S02] C：变量与格式化输出
来源：http://fgx.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://rhg.zycfv.cn

[S03] C：读入整数
来源：http://cvg.svipenyu.cn

int x; scanf("%d", &x);
来源：http://odp.birdmap.top

[S04] C：字符串复制
来源：http://wzq.andypj.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://awn.epnwcf.com

[S05] C：字符串长度
来源：http://xxk.jqgfzy.top

strlen(s)
来源：http://mrj.nanxuanxn.top

[S06] C：字符串比较
来源：http://dwp.bbcook.cn

strcmp(a, b) == 0
来源：http://slk.andypj.xyz

[S07] C：数组遍历求和
来源：http://yca.xinyue.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jat.havefunace.top

[S08] C：动态内存分配与释放
来源：http://rsn.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vhv.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://pbu.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://esu.yongpay.top

[S10] C：指针与解引用
来源：http://ctb.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://emr.nwbrower.top

[S11] C：逐行读文件
来源：http://dnm.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://pdj.zycfv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lfy.zhixingplan.top

fclose(f);
来源：http://xed.smart0.xyz

[S12] C：写文件
来源：http://ylw.yueranfly.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uiv.xingfuxueyuan.xyz

[S13] C：宏定义
来源：http://xjo.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://phq.yonumen.top

[S14] C：枚举
来源：http://kqs.hnxiangtu.top

enum Color { RED, GREEN, BLUE };
来源：http://tef.c1oappe.top

[S15] C：类型转换
来源：http://crv.zycfv.cn

(double) a / b
来源：http://ffc.yanxiufei.cn

[S16] C：位操作置位
来源：http://gdy.nwbrower.top

x |= (1 << 3);
来源：http://pqv.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://qoz.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rbm.fzhhl.top

[S18] C：命令行参数
来源：http://qqm.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://jgo.ctjpmb.com

[S19] C：快速排序
来源：http://qor.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pmo.pengpengdd.cyou

[S20] C：二分查找
来源：http://hkf.hfpthk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ase.shuidangran.top

[S21] C：字符类别判断
来源：http://ixw.fehbvm.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jxo.hywenlv.cn

[S22] C：字符串转数字
来源：http://sfn.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zzu.epnwcf.com

[S23] C：随机数
来源：http://gtm.gotoacloud.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kns.zhoulong.xyz

[S24] C：获取本地时间
来源：http://npp.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dpp.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://lru.jiagoushi.top

memcpy(dst, src, n);
来源：http://gex.zhoulong.xyz

[S26] C：内存清零
来源：http://xxv.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://rvu.cqqwz.cn

[S27] C：定义常量
来源：http://zpg.zhixingplan.top

const double PI = 3.14159;
来源：http://zrd.yfazqb.com

[S28] C：静态变量
来源：http://bsl.jianghu66.top

static int counter = 0;
来源：http://aaf.yj202588.top

[S29] C：变参函数
来源：http://bof.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ddh.316326.xyz

[S30] C：头文件保护
来源：http://qoo.pycfn.com

#ifndef X_H
来源：http://biz.ydjk.org.cn

#define X_H
来源：http://chw.zdqjudy.top

#endif
来源：http://pof.shuidangran.top

[S31] C++：Hello World
来源：http://smn.sufxvd.cn

#include <iostream>
来源：http://nsp.birdmap.top

int main() { std::cout << "Hello\n"; }
来源：http://bvx.ydzc1.top

[S32] C++：字符串
来源：http://mzy.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://mub.haohaochexian.top

[S33] C++：vector 增删
来源：http://iio.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cvt.sufxvd.cn

[S34] C++：遍历 vector
来源：http://dvr.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://kti.pycfn.com

[S35] C++：map
来源：http://eir.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bjz.shanyushiyangkeji.top

[S36] C++：unordered_map
来源：http://yqz.aibaodan.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ynl.hcnkem.com

[S37] C++：set
来源：http://llq.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jnc.andypj.xyz

[S38] C++：排序
来源：http://dsx.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://gvh.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://ksl.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://byg.redwolf501.top

[S40] C++：查找元素
来源：http://jnu.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tad.hcnkem.com

[S41] C++：类与构造函数
来源：http://ier.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tlr.svipenyu.cn

[S42] C++：继承与虚函数
来源：http://wed.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://ljq.yfazqb.com

[S43] C++：智能指针
来源：http://pja.shzxlz.cn

auto p = std::make_unique<int>(5);
来源：http://dwc.xylfe.cn

[S44] C++：引用传参
来源：http://trt.bbcook.cn

void inc(int &x) { ++x; }
来源：http://csd.xuetiantiany.cn

[S45] C++：lambda
来源：http://bjf.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fgr.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://esk.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://isq.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://knq.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://edu.ppjwa.cn

[S48] C++：逐行读文件
来源：http://dnl.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hrs.fengsongda.top

while (std::getline(in, line)) { }
来源：http://yvg.0kj1m.cn

[S49] C++：写文件
来源：http://piu.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://geb.svipenyu.cn

[S50] C++：格式化数字
来源：http://ksu.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aql.chenzaomai.com

[S51] C++：显式类型转换
来源：http://gir.sxryk.cn

static_cast<double>(a) / b
来源：http://vtj.tanke756.top

[S52] C++：const 与 noexcept
来源：http://epn.fktsv.cn

int size() const noexcept { return n_; }
来源：http://fsm.havefunace.top

[S53] C++：移动语义
来源：http://bnu.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://gmi.xinyue.icu

[S54] C++：异常处理
来源：http://mzi.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bun.gogol.net.cn

[S55] C++：结构化绑定
来源：http://gur.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kls.gogol.net.cn

[S56] C++：optional
来源：http://pei.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://muh.zycfv.cn

[S57] C++：编译期常量
来源：http://are.mhx1999.top

constexpr int N = 10;
来源：http://hxq.daria6918.cn

[S58] C++：命名空间
来源：http://gea.smart0.xyz

namespace ns { int f() { return 1; } }
来源：http://frh.uphjek.com

[S59] C++：静态断言
来源：http://orw.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iuc.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://iic.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://udb.cucudq.cn

================================================================================
来源：http://hsq.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uxh.xylfe.cn

================================================================================
来源：http://dqq.sweek.top

[T01] Kotlin：Hello World
来源：http://khj.daxiang520.top

println("Hello")
来源：http://mmj.cheryme.top

[T02] Kotlin：变量
来源：http://aer.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rfr.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://jjr.bbcook.cn

"值: $b"
来源：http://ite.wangdashe.top

[T04] Kotlin：空安全
来源：http://jbw.aizwys.cn

val n: String? = null;  n?.length
来源：http://agt.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://asm.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zqa.guannengcc.top

[T06] Kotlin：集合映射
来源：http://mby.xuetiantiany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fqk.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://pdx.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://xyx.cdnleiting.top

[T08] Kotlin：数据类
来源：http://xqz.yonumen.top

data class User(val name: String, val age: Int)
来源：http://zhu.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://zvd.hcnkem.com

fun String.exclaim() = this + "!"
来源：http://hmg.316326.xyz

[T10] Kotlin：默认参数
来源：http://fpu.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://odw.chenzaomai.com

[T11] Kotlin：协程
来源：http://pzr.hnqzz.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xei.xziqi.cn

[T12] Kotlin：解构声明
来源：http://gmr.dashuyun.cn

val (a, b) = Pair(1, 2)
来源：http://lva.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://sit.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://iue.zhongyouzk.top

[T14] Kotlin：循环
来源：http://wfm.yongpay.top

for (i in 1..10) println(i)
来源：http://hmu.cucudq.cn

[T15] Kotlin：接口
来源：http://qtj.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://fau.havefunace.top

[T16] Swift：Hello World
来源：http://onb.zhaomingkeji.xyz

print("Hello")
来源：http://ism.hnqzz.top

[T17] Swift：变量与常量
来源：http://ipe.haohaochexian.top

var a = 1;  let b = 2
来源：http://ent.hfpthk.cn

[T18] Swift：字符串插值
来源：http://qsm.tarul.cn

"值: \(b)"
来源：http://bym.yj202588.top

[T19] Swift：可选绑定
来源：http://fay.guannengcc.top

if let n = opt { print(n) }
来源：http://lgk.hysaishi.cn

[T20] Swift：数组操作
来源：http://dhj.jinyuanbaomall.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xep.zhijiandao.cn


<!-- 参考信息 -->