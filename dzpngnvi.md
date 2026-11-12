代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://tfe.ydzc1.top

[R18] 遍历数组
来源：http://rhh.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jtq.aizwys.cn

[R19] 数组长度
来源：http://oxh.sweek.top

echo "${#arr[@]}"
来源：http://pgn.kuanghao11.cn

[R20] 关联数组（字典）
来源：http://lnw.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mra.meibo888.top

[R21] 字符串长度
来源：http://jwl.ywan-chungtsiang.top

echo "${#s}"
来源：http://rff.xuetiantiany.cn

[R22] 截取子串
来源：http://gil.sweek.top

echo "${s:0:5}"
来源：http://jyv.xylfe.cn

[R23] 字符串替换
来源：http://ajk.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kqb.feifeiyinyue.top

[R24] 大小写转换
来源：http://ldk.ywan-chungtsiang.top

echo "${s^^}"; echo "${s,,}"
来源：http://jvg.tanke756.top

[R25] 去后缀 / 去前缀
来源：http://dzf.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ahw.9152youxi.cn

[R26] 命令替换
来源：http://ozi.yanxiufei.cn

now=$(date +%F); echo "$now"
来源：http://ysu.zhoulong.xyz

[R27] 算术展开
来源：http://pzk.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://ouj.jianghu66.top

[R28] 浮点运算
来源：http://tth.zhengqikj.top

echo "scale=2; 10/3" | bc
来源：http://caz.vqdsnc.cn

[R29] 定义函数
来源：http://tnz.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ojf.quarkkingdee.top

[R30] 函数返回状态码
来源：http://csd.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://jhr.xziqi.cn

[R31] 局部变量
来源：http://dcb.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://cfb.yj20258.top

[R32] 参数个数校验
来源：http://tph.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vhm.xinyue.icu

[R33] 捕获错误并提示行号
来源：http://uus.fehbvm.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://duf.jianghu66.top

[R34] 退出时清理
来源：http://cbz.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xyj.zycfv.cn

[R35] 后台执行并等待
来源：http://srw.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ubj.sjlbkw.cn

[R36] 并发执行多个任务
来源：http://cod.yongpay.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sbj.jlsjyb.cn

[R37] 把输出赋给变量
来源：http://pvh.hnqzz.top

files=$(ls -1)
来源：http://mht.shanyushiyangkeji.top

[R38] 管道串联
来源：http://qhr.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://zvc.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://xgd.yongpay.top

cmd > out.log 2>&1
来源：http://rfp.gzhubu.top

[R40] 追加写日志
来源：http://xvh.zhengqikj.top

echo "log" >> out.log
来源：http://onw.vehdjk.com

[R41] 丢弃输出
来源：http://qsm.zhiwuduotai.top

cmd >/dev/null 2>&1
来源：http://xlu.birdmap.top

[R42] 输入重定向
来源：http://ppv.zdbjq.cn

wc -l < a.txt
来源：http://kit.chenjidiqi.icu

[R43] 按名字查找文件
来源：http://ntg.zhoulong.xyz

find . -name "*.log" -type f
来源：http://vdo.bbcook.cn

[R44] 按修改时间查找
来源：http://xpb.cashguo.top

find . -mtime -7 -type f
来源：http://qmd.birdmap.top

[R45] 批量删除
来源：http://znk.yfazqb.com

find . -name "*.tmp" -delete
来源：http://xad.haohaochexian.top

[R46] 递归替换文件内容
来源：http://dce.zdbjq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://edi.hcnkem.com

[R47] sed 单行替换
来源：http://gmv.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://tdz.tarul.cn

[R48] awk 取指定列
来源：http://eji.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://tfc.haohaochexian.top

[R49] awk 带条件
来源：http://wyg.yj20258888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cjm.fanxiaobao.xyz

[R50] awk 求和
来源：http://lcs.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://vdf.zhaomingkeji.xyz

[R51] 排序去重取前几
来源：http://tyn.snrcjt.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hau.hnqzz.top

[R52] 统计行数
来源：http://nql.uphjek.com

wc -l a.txt
来源：http://ewr.xuetiantiany.cn

[R53] 查看文件头与实时尾
来源：http://dws.cashguo.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ypy.yangfankeji.com

[R54] 比较两个文件
来源：http://ycv.jinqigufen.top

diff a.txt b.txt
来源：http://jnv.shanyushiyangtech.top

[R55] 压缩与解压
来源：http://qwl.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yjj.fengsongda.top

[R56] 远程拷贝
来源：http://zoe.sxryk.cn

scp file user@host:/path/
来源：http://tze.hnqzz.top

[R57] 远程执行命令
来源：http://pgt.aibaodan.cn

ssh user@host 'uptime'
来源：http://vzp.svipenyu.cn

[R58] 下载文件
来源：http://iub.zhoulong.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uog.gaohongyu789.top

[R59] 发 POST JSON
来源：http://okf.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tww.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://gmj.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ecr.ehwqpu.com

[R61] 磁盘占用
来源：http://nce.zhixingplan.top

df -h;  du -sh *
来源：http://gjw.birdmap.top

[R62] 找最占空间的文件
来源：http://nmm.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://qah.xylfe.cn

[R63] 内存与进程
来源：http://fmq.meibo888.top

free -h;  ps aux | grep nginx
来源：http://awe.haohaochexian.top

[R64] 结束进程
来源：http://fgz.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://jhe.daria6918.cn

[R65] 查看端口占用
来源：http://lov.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bhq.cashguo.top

[R66] 定时任务
来源：http://ujk.shuidangran.top

crontab -e;  crontab -l
来源：http://qqf.cucudq.cn

[R67] 生成随机十六进制串
来源：http://ktq.dianchejie.cn

openssl rand -hex 16
来源：http://spp.fengsongda.top

[R68] 计算文件校验值
来源：http://bgi.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://gnc.yongpay.top

[R69] 生成随机密码
来源：http://kwz.yanxiufei.cn

head -c 16 /dev/urandom | base64
来源：http://ajg.c1oappe.top

[R70] 时间戳与互转
来源：http://uar.andypj.xyz

date +%s;  date -d @1700000000
来源：http://isv.hywenlv.cn

[R71] 日期格式化
来源：http://ivf.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://oug.jinqigfzy.top

[R72] 等待端口就绪
来源：http://kku.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://xmb.yanxiufei.cn

[R73] 分割大日志
来源：http://zul.xziqi.cn

split -l 1000 big.log part_
来源：http://mth.9152youxi.cn

[R74] 批量重命名
来源：http://sgd.jinqigufen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ccr.ivvv.top

[R75] 导出环境变量
来源：http://wqq.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://jgk.yj20258.top

[R76] 使用临时文件
来源：http://wfl.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://auf.gogol.net.cn

[R77] 读取用户输入
来源：http://vvn.xuetiantiany.cn

read -rp "请输入: " ans
来源：http://dbe.yuanzhike.top

[R78] 交互式菜单
来源：http://zyt.nwbrower.top

select opt in a b c; do echo "$opt"; break; done
来源：http://quf.gotoacloud.top

[R79] 解析命令行选项
来源：http://gfl.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ikj.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://hiq.ydzc1.top

time ./run.sh
来源：http://pgx.feifeiyinyue.top

================================================================================
来源：http://nqi.yfazqb.com

S. C / C++ 专题
来源：http://wzy.pycfn.com

================================================================================
来源：http://ron.fehbvm.com

[S01] C：Hello World
来源：http://kta.pengpengdd.cyou

#include <stdio.h>
来源：http://wxn.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rwb.iojbl.cn

[S02] C：变量与格式化输出
来源：http://dqf.jiagoushi.top

int a = 10; printf("%d\n", a);
来源：http://qwa.jinghuilouyu.cn

[S03] C：读入整数
来源：http://hiy.fengsongda.top

int x; scanf("%d", &x);
来源：http://mxj.ybcxt.top

[S04] C：字符串复制
来源：http://rje.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zdt.pengpengdd.cyou

[S05] C：字符串长度
来源：http://arn.gaohongyu789.top

strlen(s)
来源：http://cnb.hcnkem.com

[S06] C：字符串比较
来源：http://miu.0kj1m.cn

strcmp(a, b) == 0
来源：http://ogw.yfazqb.com

[S07] C：数组遍历求和
来源：http://khx.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hxz.hammf.cn

[S08] C：动态内存分配与释放
来源：http://kkh.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dcp.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://mxm.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kic.aizwys.cn

[S10] C：指针与解引用
来源：http://uee.meibo888.top

int *p = &a;  *p = 5;
来源：http://rao.shuidangran.top

[S11] C：逐行读文件
来源：http://xhd.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://hgx.sysykeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nxw.cucudq.cn

fclose(f);
来源：http://phb.ywan-chungtsiang.top

[S12] C：写文件
来源：http://faw.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eka.zhongyouzk.top

[S13] C：宏定义
来源：http://cnl.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ygg.dashuyun.cn

[S14] C：枚举
来源：http://nem.hysaishi.cn

enum Color { RED, GREEN, BLUE };
来源：http://lpy.shzxlz.cn

[S15] C：类型转换
来源：http://sty.yj20258.top

(double) a / b
来源：http://vfa.shzxlz.cn

[S16] C：位操作置位
来源：http://qlo.shzxlz.cn

x |= (1 << 3);
来源：http://fib.dianchejie.cn

[S17] C：安全拼接字符串
来源：http://jnh.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bia.vqdsnc.cn

[S18] C：命令行参数
来源：http://imu.zhongyouzk.top

int main(int argc, char **argv)
来源：http://rbg.birdmap.top

[S19] C：快速排序
来源：http://aqu.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://afm.c1oappe.top

[S20] C：二分查找
来源：http://bno.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bdj.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://yyu.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rue.guowangkeji.top

[S22] C：字符串转数字
来源：http://ktr.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bsp.wangdashe.top

[S23] C：随机数
来源：http://dva.guowangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dbh.smart0.xyz

[S24] C：获取本地时间
来源：http://fra.52xcode.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fda.cheryme.top

[S25] C：内存拷贝
来源：http://dsk.jlsjyb.cn

memcpy(dst, src, n);
来源：http://uxu.9152youxi.cn

[S26] C：内存清零
来源：http://qxf.uphjek.com

memset(a, 0, sizeof a);
来源：http://pdf.zhoulong.xyz

[S27] C：定义常量
来源：http://skj.gaohongyu789.top

const double PI = 3.14159;
来源：http://kxz.yj20258888.top

[S28] C：静态变量
来源：http://nmk.sysykeji.top

static int counter = 0;
来源：http://edp.andypj.xyz

[S29] C：变参函数
来源：http://sat.hammf.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yqk.yuxming.cn

[S30] C：头文件保护
来源：http://dvq.pycfn.com

#ifndef X_H
来源：http://qtc.hysaishi.cn

#define X_H
来源：http://emm.pycfn.com

#endif
来源：http://yna.cqqwz.cn

[S31] C++：Hello World
来源：http://hwn.dianchejie.cn

#include <iostream>
来源：http://fky.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://vfz.zdbjq.cn

[S32] C++：字符串
来源：http://tnc.xylfe.cn

std::string s = "hi";  s += "!";
来源：http://nbk.jqgufenzy.top

[S33] C++：vector 增删
来源：http://xhx.vqdsnc.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gjt.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://bwz.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://omk.hfpthk.cn

[S35] C++：map
来源：http://rgj.yonumen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zft.sweek.top

[S36] C++：unordered_map
来源：http://aqp.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xrv.gotoacloud.top

[S37] C++：set
来源：http://mwq.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://krv.zhongyouzk.top

[S38] C++：排序
来源：http://rkm.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://cwq.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://fbx.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vbu.ydzc1.top

[S40] C++：查找元素
来源：http://yji.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ffq.vehdjk.com

[S41] C++：类与构造函数
来源：http://iek.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tgg.fengsongda.top

[S42] C++：继承与虚函数
来源：http://dtm.cdnleiting.top

class B : public Base { public: void f() override {} };
来源：http://oew.wangdashe.top

[S43] C++：智能指针
来源：http://ezd.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://nem.yuxming.cn

[S44] C++：引用传参
来源：http://hfc.zhoulong.xyz

void inc(int &x) { ++x; }
来源：http://nfl.yj20258888.top

[S45] C++：lambda
来源：http://rsq.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://fbs.haohaochexian.top

[S46] C++：函数模板
来源：http://mdn.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dez.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://ihb.hongshengwenyu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ypn.c1oappe.top

[S48] C++：逐行读文件
来源：http://awt.9152youxi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vpj.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://ofa.zhixingplan.top

[S49] C++：写文件
来源：http://mlh.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://klw.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://tdd.xziqi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://axb.redwolf501.top

[S51] C++：显式类型转换
来源：http://bwh.zhijiandao.cn

static_cast<double>(a) / b
来源：http://qph.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://wrt.hnqzz.top

int size() const noexcept { return n_; }
来源：http://mgs.tian-w.cn

[S53] C++：移动语义
来源：http://phk.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://osj.fktsv.cn

[S54] C++：异常处理
来源：http://ndj.shuidangran.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://edk.uphjek.com

[S55] C++：结构化绑定
来源：http://bsz.wangshuangyany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rxy.316326.xyz

[S56] C++：optional
来源：http://ocd.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cze.fzhhl.top

[S57] C++：编译期常量
来源：http://kxz.guowangkeji.top

constexpr int N = 10;
来源：http://ooz.fengsongda.top

[S58] C++：命名空间
来源：http://dpl.yueranfly.top

namespace ns { int f() { return 1; } }
来源：http://xtm.ybcxt.top

[S59] C++：静态断言
来源：http://syx.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dnh.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://tra.zdqjudy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wsb.smart0.xyz

================================================================================
来源：http://oyv.sweek.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ndn.chenlongwang.top

================================================================================
来源：http://fnd.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://xms.jlsjyb.cn

println("Hello")
来源：http://lmr.ctjpmb.com

[T02] Kotlin：变量
来源：http://ogj.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hfn.uphjek.com

[T03] Kotlin：字符串模板
来源：http://iva.nwbrower.top

"值: $b"
来源：http://ktt.nanxinkj.top

[T04] Kotlin：空安全
来源：http://tzh.gzhubu.top

val n: String? = null;  n?.length
来源：http://lhe.gzhubu.top

[T05] Kotlin：when 表达式
来源：http://pps.dashuyun.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zft.havefunace.top

[T06] Kotlin：集合映射
来源：http://tlg.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lbu.cheryme.top

[T07] Kotlin：集合过滤
来源：http://uix.jinyuanbaomall.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dkq.ivvv.top

[T08] Kotlin：数据类
来源：http://owy.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://mmx.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://cux.xingfuxueyuan.xyz

fun String.exclaim() = this + "!"
来源：http://ipn.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://bcl.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mwq.pengpengdd.cyou

[T11] Kotlin：协程
来源：http://gtg.wangdashe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xqm.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://ppa.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://ovj.yuanzhike.top

[T13] Kotlin：只读 Map
来源：http://yte.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://nlt.xuetiantiany.cn

[T14] Kotlin：循环
来源：http://yxu.yj202588.top

for (i in 1..10) println(i)
来源：http://qmo.jinghuilouyu.cn

[T15] Kotlin：接口
来源：http://ytk.dashuyun.cn

interface Shape { fun area(): Double }
来源：http://xoz.cashguo.top

[T16] Swift：Hello World
来源：http://gdn.yj202588.top

print("Hello")
来源：http://dtg.hnqzz.top

[T17] Swift：变量与常量
来源：http://xuf.xuanzx.com

var a = 1;  let b = 2
来源：http://obt.epnwcf.com

[T18] Swift：字符串插值
来源：http://jvo.fengsongda.top

"值: \(b)"
来源：http://sod.xziqi.cn

[T19] Swift：可选绑定
来源：http://upy.xuanzx.com

if let n = opt { print(n) }
来源：http://lyh.zhiwuduotai.top

[T20] Swift：数组操作
来源：http://nsm.sweek.top

var a = [1, 2, 3];  a.append(4)
来源：http://hlc.jinqigfzy.top


<!-- 参考信息 -->