代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kwy.kuanghao11.cn

[R24] 大小写转换
来源：http://ccm.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fdz.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://xxd.jqgufenzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lhc.gotoacloud.top

[R26] 命令替换
来源：http://kqs.cashguo.top

now=$(date +%F); echo "$now"
来源：http://lyu.smart0.xyz

[R27] 算术展开
来源：http://mcw.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://ejz.zhijiandao.cn

[R28] 浮点运算
来源：http://ucc.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://tra.jinqigufen.top

[R29] 定义函数
来源：http://dxe.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zyf.jqgfzy.top

[R30] 函数返回状态码
来源：http://iji.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://gxx.hnqzz.top

[R31] 局部变量
来源：http://aeg.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://ycp.dashuyun.cn

[R32] 参数个数校验
来源：http://jbn.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jiv.sufxvd.cn

[R33] 捕获错误并提示行号
来源：http://mfh.hnqzz.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hub.snrcjt.cn

[R34] 退出时清理
来源：http://fia.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://pqy.yuxming.cn

[R35] 后台执行并等待
来源：http://jyv.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qgg.mhx1999.top

[R36] 并发执行多个任务
来源：http://vds.iojbl.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ypl.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://ens.hfpthk.cn

files=$(ls -1)
来源：http://nfb.smart0.xyz

[R38] 管道串联
来源：http://eie.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://pqv.jqgufenzy.top

[R39] 重定向标准输出与错误
来源：http://fgo.quarkkingdee.top

cmd > out.log 2>&1
来源：http://mvl.fehbvm.com

[R40] 追加写日志
来源：http://lmr.hongshengwenyu.top

echo "log" >> out.log
来源：http://ikn.cucudq.cn

[R41] 丢弃输出
来源：http://dbs.ydzc1.top

cmd >/dev/null 2>&1
来源：http://paz.hysaishi.cn

[R42] 输入重定向
来源：http://luh.0kj1m.cn

wc -l < a.txt
来源：http://mwj.jqgufenzy.top

[R43] 按名字查找文件
来源：http://ufv.yangfankeji.com

find . -name "*.log" -type f
来源：http://qvy.shanyushiyangkeji.top

[R44] 按修改时间查找
来源：http://loo.fengsongda.top

find . -mtime -7 -type f
来源：http://psh.c1oappe.top

[R45] 批量删除
来源：http://vyo.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://oqj.zdbjq.cn

[R46] 递归替换文件内容
来源：http://sdm.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rkc.xziqi.cn

[R47] sed 单行替换
来源：http://dbl.bjfxy.top

sed -i 's/foo/bar/g' a.txt
来源：http://pcs.yangfankeji.com

[R48] awk 取指定列
来源：http://hub.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://gfi.chenjidiqi.icu

[R49] awk 带条件
来源：http://xuu.redwolf501.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wyh.tian-w.cn

[R50] awk 求和
来源：http://otv.cucudq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hqh.sxryk.cn

[R51] 排序去重取前几
来源：http://lpz.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bno.zhijiandao.cn

[R52] 统计行数
来源：http://lda.chenjidiqi.icu

wc -l a.txt
来源：http://rfy.vqdsnc.cn

[R53] 查看文件头与实时尾
来源：http://qzz.xinyue.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qhp.ydzc1.top

[R54] 比较两个文件
来源：http://bnm.bbcook.cn

diff a.txt b.txt
来源：http://vht.hammf.cn

[R55] 压缩与解压
来源：http://xxs.jinqigfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fiw.xuetiantiany.cn

[R56] 远程拷贝
来源：http://arc.iojbl.cn

scp file user@host:/path/
来源：http://pjg.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://wrb.iojbl.cn

ssh user@host 'uptime'
来源：http://flu.yj20258888.top

[R58] 下载文件
来源：http://fsd.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wpp.shanyushiyangkeji.top

[R59] 发 POST JSON
来源：http://neb.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vfh.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://atk.zhixingplan.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vlc.yonumen.top

[R61] 磁盘占用
来源：http://ssa.316326.xyz

df -h;  du -sh *
来源：http://jrr.hnxiangtu.top

[R62] 找最占空间的文件
来源：http://psn.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://jty.jlsjyb.cn

[R63] 内存与进程
来源：http://xoo.cashguo.top

free -h;  ps aux | grep nginx
来源：http://ouo.shanyushiyangkeji.top

[R64] 结束进程
来源：http://eyo.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://clq.birdmap.top

[R65] 查看端口占用
来源：http://vvo.shanyushiyangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kjg.ehwqpu.com

[R66] 定时任务
来源：http://bmd.quarkkingdee.top

crontab -e;  crontab -l
来源：http://drn.gogol.net.cn

[R67] 生成随机十六进制串
来源：http://tmd.dashuyun.cn

openssl rand -hex 16
来源：http://hhp.yj20258888.top

[R68] 计算文件校验值
来源：http://uwl.shanyushiyangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://oxo.svipenyu.cn

[R69] 生成随机密码
来源：http://vug.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://yid.ydzc1.top

[R70] 时间戳与互转
来源：http://ner.52xcode.cn

date +%s;  date -d @1700000000
来源：http://gkv.hcnkem.com

[R71] 日期格式化
来源：http://xpp.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hvm.yanxiufei.cn

[R72] 等待端口就绪
来源：http://vne.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rqt.jqgfzy.top

[R73] 分割大日志
来源：http://rqh.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://jwe.meibo888.top

[R74] 批量重命名
来源：http://sck.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hzv.ivvv.top

[R75] 导出环境变量
来源：http://vgu.vqdsnc.cn

export PATH="$HOME/bin:$PATH"
来源：http://jwv.cdnleiting.top

[R76] 使用临时文件
来源：http://oyc.sweek.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://knr.chenlongwang.top

[R77] 读取用户输入
来源：http://ptb.hnqzz.top

read -rp "请输入: " ans
来源：http://pcv.tian-w.cn

[R78] 交互式菜单
来源：http://awt.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ejc.pycfn.com

[R79] 解析命令行选项
来源：http://ipl.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ays.yuanzhike.top

[R80] 查看脚本执行耗时
来源：http://ssd.pycfn.com

time ./run.sh
来源：http://hkb.jiagoushi.top

================================================================================
来源：http://bld.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://wac.epnwcf.com

================================================================================
来源：http://zxk.uphjek.com

[S01] C：Hello World
来源：http://ltb.zhaomingkeji.xyz

#include <stdio.h>
来源：http://vvk.ppjwa.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ttq.zdbjq.cn

[S02] C：变量与格式化输出
来源：http://aun.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://aiz.fzhhl.top

[S03] C：读入整数
来源：http://pgj.yj202588.top

int x; scanf("%d", &x);
来源：http://dpd.yueranfly.top

[S04] C：字符串复制
来源：http://vvq.hongshengwenyu.top

char dst[32]; strcpy(dst, "hi");
来源：http://iak.tanke756.top

[S05] C：字符串长度
来源：http://fok.gzhubu.top

strlen(s)
来源：http://tme.iojbl.cn

[S06] C：字符串比较
来源：http://gli.aibaodan.cn

strcmp(a, b) == 0
来源：http://wvt.yj20258.top

[S07] C：数组遍历求和
来源：http://pol.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://avk.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://gbo.quarkkingdee.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pvx.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://xqy.sjlbkw.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dub.ppjwa.cn

[S10] C：指针与解引用
来源：http://szk.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://szv.dashuyun.cn

[S11] C：逐行读文件
来源：http://sgw.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://xwx.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mds.shzxlz.cn

fclose(f);
来源：http://ukk.wangdashe.top

[S12] C：写文件
来源：http://rsw.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fim.jyoumei.cn

[S13] C：宏定义
来源：http://lhd.wangshuangyany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://utm.chenjidiqi.icu

[S14] C：枚举
来源：http://lgn.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://unq.ydjk.org.cn

[S15] C：类型转换
来源：http://aat.jinghuilouyu.cn

(double) a / b
来源：http://cqn.hnxiangtu.top

[S16] C：位操作置位
来源：http://mig.fengsongda.top

x |= (1 << 3);
来源：http://xda.guannengcc.top

[S17] C：安全拼接字符串
来源：http://dyj.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ndl.gotoacloud.top

[S18] C：命令行参数
来源：http://tqw.zhixingplan.top

int main(int argc, char **argv)
来源：http://mlb.shzxlz.cn

[S19] C：快速排序
来源：http://cfx.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://hpi.52xcode.cn

[S20] C：二分查找
来源：http://hxb.ywan-chungtsiang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bmy.svipenyu.cn

[S21] C：字符类别判断
来源：http://kga.yfazqb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tpl.pycfn.com

[S22] C：字符串转数字
来源：http://hns.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://ylc.fengsongda.top

[S23] C：随机数
来源：http://pbo.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://juk.shanyushiyangtech.top

[S24] C：获取本地时间
来源：http://jjb.uphjek.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lcq.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://exy.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://shj.jyoumei.cn

[S26] C：内存清零
来源：http://jly.hnqzz.top

memset(a, 0, sizeof a);
来源：http://tek.tanke756.top

[S27] C：定义常量
来源：http://qjm.meibo888.top

const double PI = 3.14159;
来源：http://iyv.jiagoushi.top

[S28] C：静态变量
来源：http://mtb.ppjwa.cn

static int counter = 0;
来源：http://psb.fengsongda.top

[S29] C：变参函数
来源：http://pod.aibaodan.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ckt.zhoulong.xyz

[S30] C：头文件保护
来源：http://qdl.yonumen.top

#ifndef X_H
来源：http://pyw.nanxuanxn.top

#define X_H
来源：http://xvt.fzhhl.top

#endif
来源：http://iqt.gaohongyu789.top

[S31] C++：Hello World
来源：http://mrk.jiagoushi.top

#include <iostream>
来源：http://udy.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://oot.hnqzz.top

[S32] C++：字符串
来源：http://sxf.zhixingplan.top

std::string s = "hi";  s += "!";
来源：http://pfx.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://dzt.xuetiantiany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qcc.xylfe.cn

[S34] C++：遍历 vector
来源：http://wkb.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://mvc.andypj.xyz

[S35] C++：map
来源：http://oqp.fktsv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://utk.yangfankeji.com

[S36] C++：unordered_map
来源：http://xbr.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://edy.0kj1m.cn

[S37] C++：set
来源：http://wlt.zdbjq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ypt.xinyue.icu

[S38] C++：排序
来源：http://edl.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://epx.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://hqe.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gvk.ctjpmb.com

[S40] C++：查找元素
来源：http://zxf.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xxv.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://eah.hcnkem.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fow.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://xvi.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://tsj.xziqi.cn

[S43] C++：智能指针
来源：http://sgj.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://naw.xylfe.cn

[S44] C++：引用传参
来源：http://fzm.shuidangran.top

void inc(int &x) { ++x; }
来源：http://zsi.tanke756.top

[S45] C++：lambda
来源：http://frc.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://plw.shzxlz.cn

[S46] C++：函数模板
来源：http://tcn.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://emm.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://ihl.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rpd.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://qll.fehbvm.com

std::ifstream in("a.txt");  std::string line;
来源：http://sqx.52xcode.cn

while (std::getline(in, line)) { }
来源：http://uok.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://wqu.zhengqikj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vae.kuanghao11.cn

[S50] C++：格式化数字
来源：http://eov.yj20258.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vza.yfazqb.com

[S51] C++：显式类型转换
来源：http://acn.sjlbkw.cn

static_cast<double>(a) / b
来源：http://hqb.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://vow.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://dob.sweek.top

[S53] C++：移动语义
来源：http://nku.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://bhh.ydzc1.top

[S54] C++：异常处理
来源：http://iuo.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gri.jlsjyb.cn

[S55] C++：结构化绑定
来源：http://wvq.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ytb.tianlin.xyz

[S56] C++：optional
来源：http://zjb.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qcj.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://lgo.ehwqpu.com

constexpr int N = 10;
来源：http://dll.jiagoushi.top

[S58] C++：命名空间
来源：http://atx.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://hvg.epnwcf.com

[S59] C++：静态断言
来源：http://psx.mhx1999.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hza.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://hvd.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qxc.smart0.xyz

================================================================================
来源：http://unn.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tut.fanxiaobao.xyz

================================================================================
来源：http://vbc.sweek.top

[T01] Kotlin：Hello World
来源：http://oxx.jlsjyb.cn

println("Hello")
来源：http://olm.pycfn.com

[T02] Kotlin：变量
来源：http://rqm.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tqx.vqdsnc.cn

[T03] Kotlin：字符串模板
来源：http://yko.c1oappe.top

"值: $b"
来源：http://kwl.havefunace.top

[T04] Kotlin：空安全
来源：http://hvw.zdbjq.cn

val n: String? = null;  n?.length
来源：http://etp.sxryk.cn

[T05] Kotlin：when 表达式
来源：http://ony.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vup.wangshuangyany.cn

[T06] Kotlin：集合映射
来源：http://uuo.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ius.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://ubl.quarkkingdee.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://spp.jianghu66.top

[T08] Kotlin：数据类
来源：http://rnk.chenzaomai.com

data class User(val name: String, val age: Int)
来源：http://hwj.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://qhf.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://qnz.yj202588.top

[T10] Kotlin：默认参数
来源：http://gqr.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://muh.9152youxi.cn

[T11] Kotlin：协程
来源：http://hct.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://edk.zhaomingkeji.xyz

[T12] Kotlin：解构声明
来源：http://lhn.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://idg.shanyushiyangtech.top

[T13] Kotlin：只读 Map
来源：http://zhp.ydjk.org.cn

val m = mapOf("a" to 1)
来源：http://wcm.meibo888.top

[T14] Kotlin：循环
来源：http://oak.bjfxy.top

for (i in 1..10) println(i)
来源：http://qkq.yj20258.top

[T15] Kotlin：接口
来源：http://yyz.zycfv.cn

interface Shape { fun area(): Double }
来源：http://xvo.zycfv.cn

[T16] Swift：Hello World
来源：http://csp.redwolf501.top

print("Hello")
来源：http://yzg.cucudq.cn

[T17] Swift：变量与常量
来源：http://acm.yueranfly.top

var a = 1;  let b = 2
来源：http://pnm.sysykeji.top

[T18] Swift：字符串插值
来源：http://yua.guannengcc.top

"值: \(b)"
来源：http://quj.zhengqikj.top

[T19] Swift：可选绑定
来源：http://jzy.ydzc1.top

if let n = opt { print(n) }
来源：http://xcz.gzhubu.top

[T20] Swift：数组操作
来源：http://deu.smart0.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://lkj.xylfe.cn

[T21] Swift：遍历
来源：http://crh.zdbjq.cn

for x in a { print(x) }
来源：http://xcb.cqqwz.cn

[T22] Swift：字典
来源：http://zlf.0kj1m.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tfy.yonumen.top

[T23] Swift：函数
来源：http://nah.smart0.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wsc.zhoulong.xyz

[T24] Swift：闭包
来源：http://tmg.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oaw.316326.xyz

[T25] Swift：结构体
来源：http://kxc.mhx1999.top

struct P { var x: Int }
来源：http://tfu.fengsongda.top

[T26] Swift：类与重写
来源：http://rhq.9152youxi.cn

class A: Base { override func f() {} }
来源：http://tyz.nwbrower.top


<!-- 参考信息 -->