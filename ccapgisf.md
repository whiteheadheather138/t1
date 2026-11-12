代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://wjl.meibo888.top

[R26] 命令替换
来源：http://csy.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://snh.hongshengwenyu.top

[R27] 算术展开
来源：http://udt.bbcook.cn

echo $((1 + 2 * 3))
来源：http://pzc.sxryk.cn

[R28] 浮点运算
来源：http://edi.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://lui.quarkkingdee.top

[R29] 定义函数
来源：http://rll.xingfuxueyuan.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xpo.gaohongyu789.top

[R30] 函数返回状态码
来源：http://ofh.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://ejd.zycfv.cn

[R31] 局部变量
来源：http://zuj.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://abc.quarkkingdee.top

[R32] 参数个数校验
来源：http://vna.nanxuanxn.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://enm.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://ath.zycfv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vmz.xylfe.cn

[R34] 退出时清理
来源：http://yzq.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wli.jinghuilouyu.cn

[R35] 后台执行并等待
来源：http://ugi.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://rhp.shuidangran.top

[R36] 并发执行多个任务
来源：http://qnu.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://col.sufxvd.cn

[R37] 把输出赋给变量
来源：http://zps.gzhubu.top

files=$(ls -1)
来源：http://ktc.tian-w.cn

[R38] 管道串联
来源：http://cio.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://xrb.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://nbn.shuidangran.top

cmd > out.log 2>&1
来源：http://ykg.mhx1999.top

[R40] 追加写日志
来源：http://pgs.jiagoushi.top

echo "log" >> out.log
来源：http://xjl.sweek.top

[R41] 丢弃输出
来源：http://nur.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://dpf.chenlongwang.top

[R42] 输入重定向
来源：http://lqr.ybcxt.top

wc -l < a.txt
来源：http://rsa.zycfv.cn

[R43] 按名字查找文件
来源：http://qjb.hywenlv.cn

find . -name "*.log" -type f
来源：http://wdu.yueranfly.top

[R44] 按修改时间查找
来源：http://izt.yongpay.top

find . -mtime -7 -type f
来源：http://jhh.dianchejie.cn

[R45] 批量删除
来源：http://drl.aibaodan.cn

find . -name "*.tmp" -delete
来源：http://ykd.sysykeji.top

[R46] 递归替换文件内容
来源：http://jbh.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mbt.yj202588.top

[R47] sed 单行替换
来源：http://lsk.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://cbx.aizwys.cn

[R48] awk 取指定列
来源：http://smj.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://qvk.kuanghao11.cn

[R49] awk 带条件
来源：http://uvh.chenlongwang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://isy.gogol.net.cn

[R50] awk 求和
来源：http://chd.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://syw.zdqjudy.top

[R51] 排序去重取前几
来源：http://klg.hcnkem.com

sort a.txt | uniq -c | sort -rn | head
来源：http://anw.hesvh.cn

[R52] 统计行数
来源：http://rya.sxryk.cn

wc -l a.txt
来源：http://nwc.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://ndh.redwolf501.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mnu.ydzc1.top

[R54] 比较两个文件
来源：http://gfu.fanxiaobao.xyz

diff a.txt b.txt
来源：http://hvi.yvedp.cn

[R55] 压缩与解压
来源：http://ibu.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qec.bjfxy.top

[R56] 远程拷贝
来源：http://lwg.dianchejie.cn

scp file user@host:/path/
来源：http://sgp.zhijiandao.cn

[R57] 远程执行命令
来源：http://gsw.fehbvm.com

ssh user@host 'uptime'
来源：http://aub.feifeiyinyue.top

[R58] 下载文件
来源：http://far.jinyuanbaomall.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zdh.gzhubu.top

[R59] 发 POST JSON
来源：http://gwg.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hlf.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://snr.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ebl.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://hfi.sxryk.cn

df -h;  du -sh *
来源：http://mfb.nanxinkj.top

[R62] 找最占空间的文件
来源：http://ngo.zhengqikj.top

du -ah . | sort -rh | head -10
来源：http://occ.yfazqb.com

[R63] 内存与进程
来源：http://kmi.cdnleiting.top

free -h;  ps aux | grep nginx
来源：http://uhn.sjlbkw.cn

[R64] 结束进程
来源：http://bgw.jianghu66.top

kill -9 $(pgrep -f app.py)
来源：http://sxd.pengpengdd.cyou

[R65] 查看端口占用
来源：http://nhy.nanxuanxn.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ydj.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://lyg.redwolf501.top

crontab -e;  crontab -l
来源：http://dzv.nanxinkj.top

[R67] 生成随机十六进制串
来源：http://kon.fengsongda.top

openssl rand -hex 16
来源：http://ziz.xylfe.cn

[R68] 计算文件校验值
来源：http://beb.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xuu.cucudq.cn

[R69] 生成随机密码
来源：http://ucv.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://puo.yueranfly.top

[R70] 时间戳与互转
来源：http://uuu.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://vst.aibaodan.cn

[R71] 日期格式化
来源：http://vkf.sweek.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xpj.zycfv.cn

[R72] 等待端口就绪
来源：http://bmw.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dir.chenlongwang.top

[R73] 分割大日志
来源：http://whg.52xcode.cn

split -l 1000 big.log part_
来源：http://kov.zhoulong.xyz

[R74] 批量重命名
来源：http://xem.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xat.quarkkingdee.top

[R75] 导出环境变量
来源：http://zbr.gogol.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://cor.yangfankeji.com

[R76] 使用临时文件
来源：http://cao.zycfv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ial.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://clv.iojbl.cn

read -rp "请输入: " ans
来源：http://cwt.snrcjt.cn

[R78] 交互式菜单
来源：http://ugj.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://tbg.ehwqpu.com

[R79] 解析命令行选项
来源：http://loc.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vcz.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://ubo.pengpengdd.cyou

time ./run.sh
来源：http://cgg.hnxiangtu.top

================================================================================
来源：http://xlt.nanxinkj.top

S. C / C++ 专题
来源：http://aln.gaohongyu789.top

================================================================================
来源：http://ebv.mhx1999.top

[S01] C：Hello World
来源：http://wfi.gotoacloud.top

#include <stdio.h>
来源：http://kdw.andypj.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://ffs.pycfn.com

[S02] C：变量与格式化输出
来源：http://dwc.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://geo.smart0.xyz

[S03] C：读入整数
来源：http://bbp.shzxlz.cn

int x; scanf("%d", &x);
来源：http://aux.guannengcc.top

[S04] C：字符串复制
来源：http://isx.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://fle.tarul.cn

[S05] C：字符串长度
来源：http://hnd.hesvh.cn

strlen(s)
来源：http://evi.sjlbkw.cn

[S06] C：字符串比较
来源：http://pkv.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://aja.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://oxi.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yzz.hnqzz.top

[S08] C：动态内存分配与释放
来源：http://lej.jqgfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gwu.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://rno.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oyg.jlsjyb.cn

[S10] C：指针与解引用
来源：http://ezp.yongpay.top

int *p = &a;  *p = 5;
来源：http://sen.hcnkem.com

[S11] C：逐行读文件
来源：http://blt.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://crj.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://oje.bbcook.cn

fclose(f);
来源：http://qor.jlsjyb.cn

[S12] C：写文件
来源：http://gwe.sysykeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lzf.zdbjq.cn

[S13] C：宏定义
来源：http://vlz.cdnleiting.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qys.gogol.net.cn

[S14] C：枚举
来源：http://qwr.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://wyz.9152youxi.cn

[S15] C：类型转换
来源：http://koj.chenjidiqi.icu

(double) a / b
来源：http://cfo.gotoacloud.top

[S16] C：位操作置位
来源：http://elt.chenlongwang.top

x |= (1 << 3);
来源：http://lmq.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://zas.fktsv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tpa.tanke756.top

[S18] C：命令行参数
来源：http://zeb.jlsjyb.cn

int main(int argc, char **argv)
来源：http://wdd.aizwys.cn

[S19] C：快速排序
来源：http://pjj.zhoulong.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://vli.ydjk.org.cn

[S20] C：二分查找
来源：http://zve.meibo888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jab.redwolf501.top

[S21] C：字符类别判断
来源：http://ffz.gotoacloud.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eup.hesvh.cn

[S22] C：字符串转数字
来源：http://tgv.epnwcf.com

atoi("42");  strtod("3.14", NULL);
来源：http://uwk.uphjek.com

[S23] C：随机数
来源：http://rwd.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://alr.jlsjyb.cn

[S24] C：获取本地时间
来源：http://eaa.cqqwz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aax.meibo888.top

[S25] C：内存拷贝
来源：http://cvz.zhijiandao.cn

memcpy(dst, src, n);
来源：http://jfw.tarul.cn

[S26] C：内存清零
来源：http://jnd.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://fni.yfazqb.com

[S27] C：定义常量
来源：http://qfw.dashuyun.cn

const double PI = 3.14159;
来源：http://nzf.52xcode.cn

[S28] C：静态变量
来源：http://ocr.hysaishi.cn

static int counter = 0;
来源：http://ucm.jyoumei.cn

[S29] C：变参函数
来源：http://hqf.9152youxi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hij.yj202588.top

[S30] C：头文件保护
来源：http://pdd.wangshuangyany.cn

#ifndef X_H
来源：http://zev.c1oappe.top

#define X_H
来源：http://uiu.sweek.top

#endif
来源：http://dgl.zhijiandao.cn

[S31] C++：Hello World
来源：http://xij.chenlongwang.top

#include <iostream>
来源：http://izh.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://mpx.jlsjyb.cn

[S32] C++：字符串
来源：http://lph.iojbl.cn

std::string s = "hi";  s += "!";
来源：http://ode.dianchejie.cn

[S33] C++：vector 增删
来源：http://ufq.xuetiantiany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ins.cucudq.cn

[S34] C++：遍历 vector
来源：http://wks.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://zho.cucudq.cn

[S35] C++：map
来源：http://fej.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vzg.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://uzb.chenjidiqi.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bnr.nanxinkj.top

[S37] C++：set
来源：http://sew.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yol.guowangkeji.top

[S38] C++：排序
来源：http://kep.ybcxt.top

std::sort(v.begin(), v.end());
来源：http://dvo.tian-w.cn

[S39] C++：自定义比较器排序
来源：http://qej.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xvi.ybcxt.top

[S40] C++：查找元素
来源：http://jwl.cashguo.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gcl.cucudq.cn

[S41] C++：类与构造函数
来源：http://vtn.jinyuanbaomall.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tls.feifeiyinyue.top

[S42] C++：继承与虚函数
来源：http://vwa.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://qbz.shzxlz.cn

[S43] C++：智能指针
来源：http://svj.jiagoushi.top

auto p = std::make_unique<int>(5);
来源：http://syi.9152youxi.cn

[S44] C++：引用传参
来源：http://xmq.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://nlo.cqqwz.cn

[S45] C++：lambda
来源：http://ilh.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qzk.jqgufenzy.top

[S46] C++：函数模板
来源：http://fhb.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xbf.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://cxy.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ior.yueranfly.top

[S48] C++：逐行读文件
来源：http://dqs.shzxlz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vav.sysykeji.top

while (std::getline(in, line)) { }
来源：http://cun.yvedp.cn

[S49] C++：写文件
来源：http://icp.xuetiantiany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://efw.yj202588.top

[S50] C++：格式化数字
来源：http://xhi.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uhr.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://dos.gzhubu.top

static_cast<double>(a) / b
来源：http://fvo.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://oxh.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://saq.fzhhl.top

[S53] C++：移动语义
来源：http://diz.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://nqz.zhoulong.xyz

[S54] C++：异常处理
来源：http://xtq.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ouy.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://hmc.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rcm.hammf.cn

[S56] C++：optional
来源：http://xvp.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qyl.jiagoushi.top

[S57] C++：编译期常量
来源：http://woz.yongpay.top

constexpr int N = 10;
来源：http://gts.svipenyu.cn

[S58] C++：命名空间
来源：http://bil.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://eec.feifeiyinyue.top

[S59] C++：静态断言
来源：http://exw.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rkc.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://rxc.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tba.sufxvd.cn

================================================================================
来源：http://exi.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hfn.andypj.xyz

================================================================================
来源：http://aff.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://mpu.jinyuanbaomall.cn

println("Hello")
来源：http://pjd.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://bjt.andypj.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yay.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://ara.hesvh.cn

"值: $b"
来源：http://hvk.chenzaomai.com

[T04] Kotlin：空安全
来源：http://xtk.birdmap.top

val n: String? = null;  n?.length
来源：http://ssx.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://mib.meibo888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qcq.daxiang520.top

[T06] Kotlin：集合映射
来源：http://ngs.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dtd.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://xfb.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kvy.andypj.xyz

[T08] Kotlin：数据类
来源：http://cpt.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://wzh.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://ixm.aibaodan.cn

fun String.exclaim() = this + "!"
来源：http://xjh.xuetiantiany.cn

[T10] Kotlin：默认参数
来源：http://mns.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://fcf.epnwcf.com

[T11] Kotlin：协程
来源：http://lne.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vbm.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://azi.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://xmw.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://sqg.fengsongda.top

val m = mapOf("a" to 1)
来源：http://vvy.gaohongyu789.top

[T14] Kotlin：循环
来源：http://ahb.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://vmn.yongpay.top

[T15] Kotlin：接口
来源：http://kef.xylfe.cn

interface Shape { fun area(): Double }
来源：http://upu.jinqigufen.top

[T16] Swift：Hello World
来源：http://ehv.sjlbkw.cn

print("Hello")
来源：http://vpn.yangfankeji.com

[T17] Swift：变量与常量
来源：http://fct.jyoumei.cn

var a = 1;  let b = 2
来源：http://bnm.hcnkem.com

[T18] Swift：字符串插值
来源：http://tbq.shanyushiyangtech.top

"值: \(b)"
来源：http://eja.cheryme.top

[T19] Swift：可选绑定
来源：http://azs.316326.xyz

if let n = opt { print(n) }
来源：http://mvl.nanxinkj.top

[T20] Swift：数组操作
来源：http://njt.cdnleiting.top

var a = [1, 2, 3];  a.append(4)
来源：http://lan.xuanzx.com

[T21] Swift：遍历
来源：http://wxx.yangfankeji.com

for x in a { print(x) }
来源：http://xcx.aibaodan.cn

[T22] Swift：字典
来源：http://oif.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://vew.ctjpmb.com

[T23] Swift：函数
来源：http://loa.52xcode.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gem.daxiang520.top

[T24] Swift：闭包
来源：http://rrl.zhijiandao.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yaq.gogol.net.cn

[T25] Swift：结构体
来源：http://seh.yj20258888.top

struct P { var x: Int }
来源：http://izq.snrcjt.cn

[T26] Swift：类与重写
来源：http://auh.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://vzf.yj202588.top

[T27] Swift：错误处理
来源：http://bas.jianghu66.top

do { try f() } catch { print(error) }
来源：http://vlk.dianchejie.cn

[T28] Swift：枚举
来源：http://cdo.tian-w.cn

enum Color { case red, green }
来源：http://avp.dianchejie.cn


<!-- 参考信息 -->