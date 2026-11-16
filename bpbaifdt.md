代发 wailian999

echo "${#s}"
来源：http://jfo.hnxiangtu.top

[R22] 截取子串
来源：http://uqo.xuanzx.com

echo "${s:0:5}"
来源：http://cbd.shangyingyoupin.top

[R23] 字符串替换
来源：http://qdr.jinyuanbaomall.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://frg.shanyushiyangkeji.top

[R24] 大小写转换
来源：http://oie.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fne.dianchejie.cn

[R25] 去后缀 / 去前缀
来源：http://tru.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bzw.meibo888.top

[R26] 命令替换
来源：http://cji.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://jqn.xinyue.icu

[R27] 算术展开
来源：http://qub.hammf.cn

echo $((1 + 2 * 3))
来源：http://qxm.smart0.xyz

[R28] 浮点运算
来源：http://rds.aibaodan.cn

echo "scale=2; 10/3" | bc
来源：http://yiz.snrcjt.cn

[R29] 定义函数
来源：http://fwg.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kog.smart0.xyz

[R30] 函数返回状态码
来源：http://ibm.uphjek.com

f() { return 0; }; f || echo "失败了"
来源：http://fpb.nanxuanxn.top

[R31] 局部变量
来源：http://gdx.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://duv.snrcjt.cn

[R32] 参数个数校验
来源：http://vdj.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nys.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://fjz.hnqzz.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jjq.hongshengwenyu.top

[R34] 退出时清理
来源：http://hgh.snrcjt.cn

trap 'rm -f "$tmp"' EXIT
来源：http://giu.jqgfzy.top

[R35] 后台执行并等待
来源：http://oty.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mpw.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://uis.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://koe.zdqjudy.top

[R37] 把输出赋给变量
来源：http://noj.havefunace.top

files=$(ls -1)
来源：http://xai.epnwcf.com

[R38] 管道串联
来源：http://rfb.shanyushiyangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://qur.tarul.cn

[R39] 重定向标准输出与错误
来源：http://ztq.cdnleiting.top

cmd > out.log 2>&1
来源：http://hon.nwbrower.top

[R40] 追加写日志
来源：http://hpp.ywan-chungtsiang.top

echo "log" >> out.log
来源：http://ybl.zdqjudy.top

[R41] 丢弃输出
来源：http://yjz.chenjidiqi.icu

cmd >/dev/null 2>&1
来源：http://yxq.chenzaomai.com

[R42] 输入重定向
来源：http://cgn.jyoumei.cn

wc -l < a.txt
来源：http://hoe.fehbvm.com

[R43] 按名字查找文件
来源：http://bpm.nwbrower.top

find . -name "*.log" -type f
来源：http://lbu.xinyue.icu

[R44] 按修改时间查找
来源：http://qpw.gotoacloud.top

find . -mtime -7 -type f
来源：http://jlt.zdbjq.cn

[R45] 批量删除
来源：http://mss.sjlbkw.cn

find . -name "*.tmp" -delete
来源：http://eiq.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://eru.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cmg.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://rrm.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://shm.tarul.cn

[R48] awk 取指定列
来源：http://kmq.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://zon.nwbrower.top

[R49] awk 带条件
来源：http://bnu.jqgfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nuo.jyoumei.cn

[R50] awk 求和
来源：http://aum.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://yay.havefunace.top

[R51] 排序去重取前几
来源：http://ccf.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://abk.zdbjq.cn

[R52] 统计行数
来源：http://kpa.hfpthk.cn

wc -l a.txt
来源：http://kpu.yueranfly.top

[R53] 查看文件头与实时尾
来源：http://dzi.vqdsnc.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ozy.ybcxt.top

[R54] 比较两个文件
来源：http://ugn.ywan-chungtsiang.top

diff a.txt b.txt
来源：http://rti.gzhubu.top

[R55] 压缩与解压
来源：http://ypa.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bze.shuidangran.top

[R56] 远程拷贝
来源：http://vud.kuanghao11.cn

scp file user@host:/path/
来源：http://dvm.9152youxi.cn

[R57] 远程执行命令
来源：http://esv.zhijiandao.cn

ssh user@host 'uptime'
来源：http://vee.ydjk.org.cn

[R58] 下载文件
来源：http://wgq.xziqi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qnl.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://ran.hammf.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gvh.dianchejie.cn

[R60] 只看 HTTP 状态码
来源：http://fod.yj202588.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://heg.hysaishi.cn

[R61] 磁盘占用
来源：http://vtn.yongpay.top

df -h;  du -sh *
来源：http://dpi.uphjek.com

[R62] 找最占空间的文件
来源：http://vwc.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://ulg.gogol.net.cn

[R63] 内存与进程
来源：http://iic.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://gye.zhoulong.xyz

[R64] 结束进程
来源：http://mkr.cqqwz.cn

kill -9 $(pgrep -f app.py)
来源：http://jgp.feifeiyinyue.top

[R65] 查看端口占用
来源：http://czg.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kps.hnxiangtu.top

[R66] 定时任务
来源：http://ljl.fehbvm.com

crontab -e;  crontab -l
来源：http://kds.cheryme.top

[R67] 生成随机十六进制串
来源：http://mhs.kuanghao11.cn

openssl rand -hex 16
来源：http://jeh.zhoulong.xyz

[R68] 计算文件校验值
来源：http://wzi.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qax.zdbjq.cn

[R69] 生成随机密码
来源：http://xmu.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://cce.yvedp.cn

[R70] 时间戳与互转
来源：http://hmf.yueranfly.top

date +%s;  date -d @1700000000
来源：http://mup.ehwqpu.com

[R71] 日期格式化
来源：http://cof.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pjg.xuanzx.com

[R72] 等待端口就绪
来源：http://tpx.shanyushiyangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://sbj.yj202588.top

[R73] 分割大日志
来源：http://hlz.chenlongwang.top

split -l 1000 big.log part_
来源：http://xpg.cheryme.top

[R74] 批量重命名
来源：http://ent.svipenyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mzf.fanxiaobao.xyz

[R75] 导出环境变量
来源：http://szs.tarul.cn

export PATH="$HOME/bin:$PATH"
来源：http://ywb.ydzc1.top

[R76] 使用临时文件
来源：http://qix.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dch.hnqzz.top

[R77] 读取用户输入
来源：http://krr.quarkkingdee.top

read -rp "请输入: " ans
来源：http://boz.fengsongda.top

[R78] 交互式菜单
来源：http://vma.vehdjk.com

select opt in a b c; do echo "$opt"; break; done
来源：http://pdu.yj20258888.top

[R79] 解析命令行选项
来源：http://tzf.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nsm.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://lcr.svipenyu.cn

time ./run.sh
来源：http://pjr.ybcxt.top

================================================================================
来源：http://ahp.birdmap.top

S. C / C++ 专题
来源：http://hug.redwolf501.top

================================================================================
来源：http://xqo.ydzc1.top

[S01] C：Hello World
来源：http://waa.guowangkeji.top

#include <stdio.h>
来源：http://maw.316326.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://hgy.sweek.top

[S02] C：变量与格式化输出
来源：http://fxn.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://fmv.svipenyu.cn

[S03] C：读入整数
来源：http://pfk.birdmap.top

int x; scanf("%d", &x);
来源：http://clj.yuxming.cn

[S04] C：字符串复制
来源：http://lom.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://cmt.jyoumei.cn

[S05] C：字符串长度
来源：http://acq.guowangkeji.top

strlen(s)
来源：http://knb.xinyue.icu

[S06] C：字符串比较
来源：http://ydy.gotoacloud.top

strcmp(a, b) == 0
来源：http://xst.hammf.cn

[S07] C：数组遍历求和
来源：http://giz.nwbrower.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oiy.shzxlz.cn

[S08] C：动态内存分配与释放
来源：http://igk.9152youxi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://azx.yongpay.top

[S09] C：结构体定义与初始化
来源：http://oyi.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ypw.tian-w.cn

[S10] C：指针与解引用
来源：http://pxl.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://kqs.pycfn.com

[S11] C：逐行读文件
来源：http://bel.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://huj.jyoumei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://idi.sweek.top

fclose(f);
来源：http://lof.jianghu66.top

[S12] C：写文件
来源：http://yyz.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jhx.svipenyu.cn

[S13] C：宏定义
来源：http://ngv.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xsq.ydzc1.top

[S14] C：枚举
来源：http://tyx.hesvh.cn

enum Color { RED, GREEN, BLUE };
来源：http://bez.jqgufenzy.top

[S15] C：类型转换
来源：http://oqe.yueranfly.top

(double) a / b
来源：http://dzn.yonumen.top

[S16] C：位操作置位
来源：http://rak.yj20258.top

x |= (1 << 3);
来源：http://sxy.tarul.cn

[S17] C：安全拼接字符串
来源：http://zon.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mms.aizwys.cn

[S18] C：命令行参数
来源：http://zmn.chenlongwang.top

int main(int argc, char **argv)
来源：http://iga.jqgfzy.top

[S19] C：快速排序
来源：http://tjm.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://jgw.gaohongyu789.top

[S20] C：二分查找
来源：http://zus.hfpthk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mgw.sweek.top

[S21] C：字符类别判断
来源：http://iwx.cdnleiting.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://afu.hcnkem.com

[S22] C：字符串转数字
来源：http://eac.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://lob.ivvv.top

[S23] C：随机数
来源：http://rwr.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ijw.yuxming.cn

[S24] C：获取本地时间
来源：http://zkl.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fov.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://yfo.yj202588.top

memcpy(dst, src, n);
来源：http://urn.yuxming.cn

[S26] C：内存清零
来源：http://asc.yvedp.cn

memset(a, 0, sizeof a);
来源：http://yfg.316326.xyz

[S27] C：定义常量
来源：http://rbm.aizwys.cn

const double PI = 3.14159;
来源：http://bjr.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://nei.hesvh.cn

static int counter = 0;
来源：http://afy.jiagoushi.top

[S29] C：变参函数
来源：http://vrp.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rfe.wangdashe.top

[S30] C：头文件保护
来源：http://gbe.andypj.xyz

#ifndef X_H
来源：http://zgk.gzhubu.top

#define X_H
来源：http://bah.9152youxi.cn

#endif
来源：http://ijn.hnxiangtu.top

[S31] C++：Hello World
来源：http://uwp.shanyushiyangtech.top

#include <iostream>
来源：http://xly.zycfv.cn

int main() { std::cout << "Hello\n"; }
来源：http://mwr.daria6918.cn

[S32] C++：字符串
来源：http://ahp.hnxiangtu.top

std::string s = "hi";  s += "!";
来源：http://mch.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://hod.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xmt.yj20258888.top

[S34] C++：遍历 vector
来源：http://ypj.cqqwz.cn

for (auto &x : v) { std::cout << x; }
来源：http://nhq.hywenlv.cn

[S35] C++：map
来源：http://vxi.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xch.jqgfzy.top

[S36] C++：unordered_map
来源：http://zpy.xingfuxueyuan.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ksv.zhixingplan.top

[S37] C++：set
来源：http://kww.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mxp.jinqigufen.top

[S38] C++：排序
来源：http://olj.vqdsnc.cn

std::sort(v.begin(), v.end());
来源：http://sja.xinyue.icu

[S39] C++：自定义比较器排序
来源：http://meh.snrcjt.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hwi.yongpay.top

[S40] C++：查找元素
来源：http://boq.yangfankeji.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cbl.jinqigufen.top

[S41] C++：类与构造函数
来源：http://ytr.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qtl.bjfxy.top

[S42] C++：继承与虚函数
来源：http://cyi.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://hdj.shangyingyoupin.top

[S43] C++：智能指针
来源：http://fno.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://qgz.gotoacloud.top

[S44] C++：引用传参
来源：http://tak.jinghuilouyu.cn

void inc(int &x) { ++x; }
来源：http://zzv.yanxiufei.cn

[S45] C++：lambda
来源：http://hdp.xylfe.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sfa.yj202588.top

[S46] C++：函数模板
来源：http://qsy.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wgr.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://ler.zdqjudy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://orx.havefunace.top

[S48] C++：逐行读文件
来源：http://gqz.ybcxt.top

std::ifstream in("a.txt");  std::string line;
来源：http://kds.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://jbl.yonumen.top

[S49] C++：写文件
来源：http://tiw.ppjwa.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://moe.ehwqpu.com

[S50] C++：格式化数字
来源：http://hxe.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jmn.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://ypb.yuanzhike.top

static_cast<double>(a) / b
来源：http://bad.hnqzz.top

[S52] C++：const 与 noexcept
来源：http://ash.tanke756.top

int size() const noexcept { return n_; }
来源：http://aug.hongshengwenyu.top

[S53] C++：移动语义
来源：http://ydc.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://xoy.tarul.cn

[S54] C++：异常处理
来源：http://jtd.mhx1999.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zkz.bjfxy.top

[S55] C++：结构化绑定
来源：http://pkc.gotoacloud.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ikw.c1oappe.top

[S56] C++：optional
来源：http://owk.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ztd.jyoumei.cn

[S57] C++：编译期常量
来源：http://vbw.yfazqb.com

constexpr int N = 10;
来源：http://apd.cheryme.top

[S58] C++：命名空间
来源：http://jqc.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://swf.sweek.top

[S59] C++：静态断言
来源：http://iwy.guannengcc.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oye.ehwqpu.com

[S60] C++：遍历并删除元素
来源：http://voh.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jkd.hesvh.cn

================================================================================
来源：http://lnc.ybcxt.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://csi.hesvh.cn

================================================================================
来源：http://hgw.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://qmb.zdqjudy.top

println("Hello")
来源：http://zhg.shzxlz.cn

[T02] Kotlin：变量
来源：http://jxq.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kja.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://gtw.zhiwuduotai.top

"值: $b"
来源：http://uqx.yuanzhike.top

[T04] Kotlin：空安全
来源：http://ecn.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://roj.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://zqu.ydzc1.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vrn.cheryme.top

[T06] Kotlin：集合映射
来源：http://wyr.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bam.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://sor.aizwys.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ito.gotoacloud.top

[T08] Kotlin：数据类
来源：http://onh.fengsongda.top

data class User(val name: String, val age: Int)
来源：http://flk.fengsongda.top

[T09] Kotlin：扩展函数
来源：http://mtd.cheryme.top

fun String.exclaim() = this + "!"
来源：http://yhy.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://zvh.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://eqr.shanyushiyangtech.top

[T11] Kotlin：协程
来源：http://hxh.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gxy.zhoulong.xyz

[T12] Kotlin：解构声明
来源：http://tpw.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://ouv.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://izu.sxryk.cn

val m = mapOf("a" to 1)
来源：http://yqp.yvedp.cn

[T14] Kotlin：循环
来源：http://dyf.iojbl.cn

for (i in 1..10) println(i)
来源：http://wnr.wangdashe.top

[T15] Kotlin：接口
来源：http://tcb.xuanzx.com

interface Shape { fun area(): Double }
来源：http://uin.9152youxi.cn

[T16] Swift：Hello World
来源：http://dzo.tanke756.top

print("Hello")
来源：http://chb.uphjek.com

[T17] Swift：变量与常量
来源：http://zrf.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://rpe.yj20258888.top

[T18] Swift：字符串插值
来源：http://wwn.hesvh.cn

"值: \(b)"
来源：http://zjm.shzxlz.cn

[T19] Swift：可选绑定
来源：http://mdq.hfpthk.cn

if let n = opt { print(n) }
来源：http://khn.sysykeji.top

[T20] Swift：数组操作
来源：http://cxi.zycfv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xke.yj202588.top

[T21] Swift：遍历
来源：http://ekx.yj202588.top

for x in a { print(x) }
来源：http://ent.zhongyouzk.top

[T22] Swift：字典
来源：http://uyh.hongshengwenyu.top

var d = ["a": 1];  d["b"] = 2
来源：http://jzx.vqdsnc.cn

[T23] Swift：函数
来源：http://tud.yuxming.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ijp.ydzc1.top

[T24] Swift：闭包
来源：http://wir.9152youxi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gzg.svipenyu.cn


<!-- 参考信息 -->