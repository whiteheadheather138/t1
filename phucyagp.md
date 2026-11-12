代发 wailian999

echo "${#s}"
来源：http://sak.xylfe.cn

[R22] 截取子串
来源：http://hmr.quarkkingdee.top

echo "${s:0:5}"
来源：http://ljo.jyoumei.cn

[R23] 字符串替换
来源：http://qjl.bbcook.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ffg.xingfuxueyuan.xyz

[R24] 大小写转换
来源：http://asm.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ajv.dianchejie.cn

[R25] 去后缀 / 去前缀
来源：http://mfq.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wfq.shanyushiyangkeji.top

[R26] 命令替换
来源：http://wlj.hammf.cn

now=$(date +%F); echo "$now"
来源：http://dsx.shuidangran.top

[R27] 算术展开
来源：http://gsm.tarul.cn

echo $((1 + 2 * 3))
来源：http://anc.fzhhl.top

[R28] 浮点运算
来源：http://rnw.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://hmg.bbcook.cn

[R29] 定义函数
来源：http://irf.shangyingyoupin.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zkg.9152youxi.cn

[R30] 函数返回状态码
来源：http://poe.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://nyw.9152youxi.cn

[R31] 局部变量
来源：http://qqu.cucudq.cn

f() { local x=1; echo "$x"; }
来源：http://zql.nanxinkj.top

[R32] 参数个数校验
来源：http://sno.hesvh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bbu.ywan-chungtsiang.top

[R33] 捕获错误并提示行号
来源：http://ffi.cucudq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vfc.guowangkeji.top

[R34] 退出时清理
来源：http://mkh.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://ovr.tian-w.cn

[R35] 后台执行并等待
来源：http://fvv.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://rmh.cheryme.top

[R36] 并发执行多个任务
来源：http://vmk.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nql.sysykeji.top

[R37] 把输出赋给变量
来源：http://fxk.tianlin.xyz

files=$(ls -1)
来源：http://fcq.zhongyouzk.top

[R38] 管道串联
来源：http://ona.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://brf.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://dft.yj20258.top

cmd > out.log 2>&1
来源：http://lgm.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://dny.cqqwz.cn

echo "log" >> out.log
来源：http://rmo.chenjidiqi.icu

[R41] 丢弃输出
来源：http://hgj.xuanzx.com

cmd >/dev/null 2>&1
来源：http://nym.sysykeji.top

[R42] 输入重定向
来源：http://zjg.xinyue.icu

wc -l < a.txt
来源：http://qsz.nwbrower.top

[R43] 按名字查找文件
来源：http://kww.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://inz.gogol.net.cn

[R44] 按修改时间查找
来源：http://cql.bjfxy.top

find . -mtime -7 -type f
来源：http://ewy.nanxuanxn.top

[R45] 批量删除
来源：http://ymx.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://acl.tanke756.top

[R46] 递归替换文件内容
来源：http://tua.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tqx.wangshuangyany.cn

[R47] sed 单行替换
来源：http://wqz.quarkkingdee.top

sed -i 's/foo/bar/g' a.txt
来源：http://ock.hfpthk.cn

[R48] awk 取指定列
来源：http://xem.gaohongyu789.top

awk '{print $1, $3}' a.txt
来源：http://ffw.yuanzhike.top

[R49] awk 带条件
来源：http://jbr.feifeiyinyue.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wku.nanxinkj.top

[R50] awk 求和
来源：http://pwn.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hun.hcnkem.com

[R51] 排序去重取前几
来源：http://jkj.aibaodan.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://use.cashguo.top

[R52] 统计行数
来源：http://bzw.ctjpmb.com

wc -l a.txt
来源：http://xre.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://lth.hfpthk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dcq.yfazqb.com

[R54] 比较两个文件
来源：http://jih.bjfxy.top

diff a.txt b.txt
来源：http://eme.yfazqb.com

[R55] 压缩与解压
来源：http://egk.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wag.daxiang520.top

[R56] 远程拷贝
来源：http://dbc.ctjpmb.com

scp file user@host:/path/
来源：http://lld.jinqigufen.top

[R57] 远程执行命令
来源：http://bdh.daria6918.cn

ssh user@host 'uptime'
来源：http://oly.aizwys.cn

[R58] 下载文件
来源：http://mdb.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vde.daria6918.cn

[R59] 发 POST JSON
来源：http://rzm.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xpq.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://vhl.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vgu.havefunace.top

[R61] 磁盘占用
来源：http://fio.shzxlz.cn

df -h;  du -sh *
来源：http://uas.smart0.xyz

[R62] 找最占空间的文件
来源：http://uxk.pengpengdd.cyou

du -ah . | sort -rh | head -10
来源：http://tuo.zhengqikj.top

[R63] 内存与进程
来源：http://rmj.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://fvd.yfazqb.com

[R64] 结束进程
来源：http://qeb.zhoulong.xyz

kill -9 $(pgrep -f app.py)
来源：http://gkk.shuidangran.top

[R65] 查看端口占用
来源：http://fnq.meibo888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oek.gogol.net.cn

[R66] 定时任务
来源：http://soj.redwolf501.top

crontab -e;  crontab -l
来源：http://ydz.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://fgc.pycfn.com

openssl rand -hex 16
来源：http://uel.hesvh.cn

[R68] 计算文件校验值
来源：http://wio.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://vzl.cdnleiting.top

[R69] 生成随机密码
来源：http://ggp.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://mlv.tanke756.top

[R70] 时间戳与互转
来源：http://kgk.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://gms.birdmap.top

[R71] 日期格式化
来源：http://pwg.jqgufenzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ydw.sweek.top

[R72] 等待端口就绪
来源：http://rga.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://umd.ybcxt.top

[R73] 分割大日志
来源：http://lzn.yj20258.top

split -l 1000 big.log part_
来源：http://uut.cashguo.top

[R74] 批量重命名
来源：http://bgw.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://puu.aibaodan.cn

[R75] 导出环境变量
来源：http://mii.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://qfv.jqgfzy.top

[R76] 使用临时文件
来源：http://ijc.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://txe.shangyingyoupin.top

[R77] 读取用户输入
来源：http://yto.epnwcf.com

read -rp "请输入: " ans
来源：http://vpv.hywenlv.cn

[R78] 交互式菜单
来源：http://nrj.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bzc.quarkkingdee.top

[R79] 解析命令行选项
来源：http://jxb.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://far.pycfn.com

[R80] 查看脚本执行耗时
来源：http://tca.mhx1999.top

time ./run.sh
来源：http://rsz.xylfe.cn

================================================================================
来源：http://cjm.kuanghao11.cn

S. C / C++ 专题
来源：http://jow.smart0.xyz

================================================================================
来源：http://wtf.yueranfly.top

[S01] C：Hello World
来源：http://tko.smart0.xyz

#include <stdio.h>
来源：http://mgd.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://ibd.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://iju.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://frn.zdqjudy.top

[S03] C：读入整数
来源：http://mru.ybcxt.top

int x; scanf("%d", &x);
来源：http://sfg.zdbjq.cn

[S04] C：字符串复制
来源：http://xoy.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://ida.shanyushiyangkeji.top

[S05] C：字符串长度
来源：http://swe.tanke756.top

strlen(s)
来源：http://umj.ybcxt.top

[S06] C：字符串比较
来源：http://gqo.tanke756.top

strcmp(a, b) == 0
来源：http://gxl.ctjpmb.com

[S07] C：数组遍历求和
来源：http://vff.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hbw.dianchejie.cn

[S08] C：动态内存分配与释放
来源：http://imw.ydzc1.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fjp.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://red.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cqx.yj20258.top

[S10] C：指针与解引用
来源：http://bef.yueranfly.top

int *p = &a;  *p = 5;
来源：http://vcn.hnxiangtu.top

[S11] C：逐行读文件
来源：http://dcf.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://qzx.jyoumei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ssv.jinqigfzy.top

fclose(f);
来源：http://oew.cucudq.cn

[S12] C：写文件
来源：http://otd.svipenyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hon.hesvh.cn

[S13] C：宏定义
来源：http://ldk.hnxiangtu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vtl.zdbjq.cn

[S14] C：枚举
来源：http://cpp.sxryk.cn

enum Color { RED, GREEN, BLUE };
来源：http://zis.wangdashe.top

[S15] C：类型转换
来源：http://wry.9152youxi.cn

(double) a / b
来源：http://svx.yvedp.cn

[S16] C：位操作置位
来源：http://rrw.fktsv.cn

x |= (1 << 3);
来源：http://lmv.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://kfn.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mti.chenjidiqi.icu

[S18] C：命令行参数
来源：http://ssf.ctjpmb.com

int main(int argc, char **argv)
来源：http://fot.feifeiyinyue.top

[S19] C：快速排序
来源：http://qvw.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://wip.vqdsnc.cn

[S20] C：二分查找
来源：http://tyg.quarkkingdee.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kbl.jyoumei.cn

[S21] C：字符类别判断
来源：http://bmi.shangyingyoupin.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fix.zdqjudy.top

[S22] C：字符串转数字
来源：http://own.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ehq.aibaodan.cn

[S23] C：随机数
来源：http://uqx.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lpc.sysykeji.top

[S24] C：获取本地时间
来源：http://fmg.ybcxt.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fxs.shuidangran.top

[S25] C：内存拷贝
来源：http://qqr.havefunace.top

memcpy(dst, src, n);
来源：http://wpp.tarul.cn

[S26] C：内存清零
来源：http://bwu.havefunace.top

memset(a, 0, sizeof a);
来源：http://yyk.xingfuxueyuan.xyz

[S27] C：定义常量
来源：http://uqt.jqgufenzy.top

const double PI = 3.14159;
来源：http://wqq.snrcjt.cn

[S28] C：静态变量
来源：http://mec.fanxiaobao.xyz

static int counter = 0;
来源：http://bip.vqdsnc.cn

[S29] C：变参函数
来源：http://hsc.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vqm.tianlin.xyz

[S30] C：头文件保护
来源：http://gmw.fzhhl.top

#ifndef X_H
来源：http://piw.quarkkingdee.top

#define X_H
来源：http://jaq.hysaishi.cn

#endif
来源：http://pmn.vehdjk.com

[S31] C++：Hello World
来源：http://jvs.fzhhl.top

#include <iostream>
来源：http://gfk.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://gzv.ppjwa.cn

[S32] C++：字符串
来源：http://ryd.ydzc1.top

std::string s = "hi";  s += "!";
来源：http://qxq.daxiang520.top

[S33] C++：vector 增删
来源：http://evu.pycfn.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cpq.pengpengdd.cyou

[S34] C++：遍历 vector
来源：http://rcl.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://lgs.yuanzhike.top

[S35] C++：map
来源：http://erj.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fjo.iojbl.cn

[S36] C++：unordered_map
来源：http://dmv.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ymt.birdmap.top

[S37] C++：set
来源：http://jno.nanxuanxn.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pkr.yuxming.cn

[S38] C++：排序
来源：http://syj.xuanzx.com

std::sort(v.begin(), v.end());
来源：http://njf.yongpay.top

[S39] C++：自定义比较器排序
来源：http://fvg.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xpb.smart0.xyz

[S40] C++：查找元素
来源：http://ovt.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://snp.cheryme.top

[S41] C++：类与构造函数
来源：http://yry.fengsongda.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ntl.epnwcf.com

[S42] C++：继承与虚函数
来源：http://icp.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://csy.yfazqb.com

[S43] C++：智能指针
来源：http://vpp.bjfxy.top

auto p = std::make_unique<int>(5);
来源：http://vtl.guannengcc.top

[S44] C++：引用传参
来源：http://dfq.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://vve.hnqzz.top

[S45] C++：lambda
来源：http://req.xylfe.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xru.jianghu66.top

[S46] C++：函数模板
来源：http://ire.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rmi.sysykeji.top

[S47] C++：结构化绑定遍历
来源：http://stg.xingfuxueyuan.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hhg.haohaochexian.top

[S48] C++：逐行读文件
来源：http://ipb.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vpz.tarul.cn

while (std::getline(in, line)) { }
来源：http://dhn.52xcode.cn

[S49] C++：写文件
来源：http://llz.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hye.yonumen.top

[S50] C++：格式化数字
来源：http://csw.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cgc.yuxming.cn

[S51] C++：显式类型转换
来源：http://aem.dianchejie.cn

static_cast<double>(a) / b
来源：http://nki.yonumen.top

[S52] C++：const 与 noexcept
来源：http://hnf.gzhubu.top

int size() const noexcept { return n_; }
来源：http://dqc.gaohongyu789.top

[S53] C++：移动语义
来源：http://flh.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://zjb.sufxvd.cn

[S54] C++：异常处理
来源：http://ioy.cashguo.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aqe.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://kxa.jiagoushi.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qwb.redwolf501.top

[S56] C++：optional
来源：http://yjq.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bsy.zdbjq.cn

[S57] C++：编译期常量
来源：http://ufr.zdbjq.cn

constexpr int N = 10;
来源：http://inj.fengsongda.top

[S58] C++：命名空间
来源：http://grl.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://nnz.birdmap.top

[S59] C++：静态断言
来源：http://ytv.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rwv.tarul.cn

[S60] C++：遍历并删除元素
来源：http://muz.smart0.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jcv.chenzaomai.com

================================================================================
来源：http://pxp.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qax.yj20258.top

================================================================================
来源：http://xyf.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://gax.tanke756.top

println("Hello")
来源：http://hus.xuanzx.com

[T02] Kotlin：变量
来源：http://kkk.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uet.xuanzx.com

[T03] Kotlin：字符串模板
来源：http://nxt.zhiwuduotai.top

"值: $b"
来源：http://vxo.yonumen.top

[T04] Kotlin：空安全
来源：http://rfy.c1oappe.top

val n: String? = null;  n?.length
来源：http://sdm.ctjpmb.com

[T05] Kotlin：when 表达式
来源：http://ijy.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gym.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://bcl.shzxlz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qka.fktsv.cn

[T07] Kotlin：集合过滤
来源：http://kuq.gogol.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hyf.jiagoushi.top

[T08] Kotlin：数据类
来源：http://lbr.tarul.cn

data class User(val name: String, val age: Int)
来源：http://cvt.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://xar.wangdashe.top

fun String.exclaim() = this + "!"
来源：http://dbz.316326.xyz

[T10] Kotlin：默认参数
来源：http://tpg.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qpc.zhengqikj.top

[T11] Kotlin：协程
来源：http://rdj.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qqo.smart0.xyz

[T12] Kotlin：解构声明
来源：http://unj.gzhubu.top

val (a, b) = Pair(1, 2)
来源：http://hnu.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://lms.cqqwz.cn

val m = mapOf("a" to 1)
来源：http://tnl.cqqwz.cn

[T14] Kotlin：循环
来源：http://lce.haohaochexian.top

for (i in 1..10) println(i)
来源：http://qln.ywan-chungtsiang.top

[T15] Kotlin：接口
来源：http://wtr.tarul.cn

interface Shape { fun area(): Double }
来源：http://wpd.snrcjt.cn

[T16] Swift：Hello World
来源：http://iiz.0kj1m.cn

print("Hello")
来源：http://kzd.shzxlz.cn

[T17] Swift：变量与常量
来源：http://pfo.jqgfzy.top

var a = 1;  let b = 2
来源：http://hbc.gogol.net.cn

[T18] Swift：字符串插值
来源：http://aly.dianchejie.cn

"值: \(b)"
来源：http://sji.tian-w.cn

[T19] Swift：可选绑定
来源：http://eho.zhixingplan.top

if let n = opt { print(n) }
来源：http://ovr.hywenlv.cn

[T20] Swift：数组操作
来源：http://nek.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://tcu.tian-w.cn

[T21] Swift：遍历
来源：http://akq.jqgufenzy.top

for x in a { print(x) }
来源：http://qxn.zhongyouzk.top

[T22] Swift：字典
来源：http://ryq.zhijiandao.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xsy.vehdjk.com

[T23] Swift：函数
来源：http://lxs.jqgufenzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jxf.pycfn.com

[T24] Swift：闭包
来源：http://kjt.52xcode.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tmc.tanke756.top


<!-- 参考信息 -->