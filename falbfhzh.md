代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iwk.fktsv.cn

[R24] 大小写转换
来源：http://une.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://ogx.hfpthk.cn

[R25] 去后缀 / 去前缀
来源：http://gbc.yuanzhike.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ehv.pycfn.com

[R26] 命令替换
来源：http://szi.c1oappe.top

now=$(date +%F); echo "$now"
来源：http://lgj.chenzaomai.com

[R27] 算术展开
来源：http://quj.hammf.cn

echo $((1 + 2 * 3))
来源：http://ngj.zycfv.cn

[R28] 浮点运算
来源：http://hlj.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://clz.cqqwz.cn

[R29] 定义函数
来源：http://inc.shuidangran.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://boj.ehwqpu.com

[R30] 函数返回状态码
来源：http://dax.hfpthk.cn

f() { return 0; }; f || echo "失败了"
来源：http://fwi.aizwys.cn

[R31] 局部变量
来源：http://rlx.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://isj.haohaochexian.top

[R32] 参数个数校验
来源：http://efp.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rrs.hcnkem.com

[R33] 捕获错误并提示行号
来源：http://pkv.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fth.jiagoushi.top

[R34] 退出时清理
来源：http://edk.shzxlz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tgq.guannengcc.top

[R35] 后台执行并等待
来源：http://har.hfpthk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vzy.redwolf501.top

[R36] 并发执行多个任务
来源：http://yub.andypj.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://msw.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://meh.daria6918.cn

files=$(ls -1)
来源：http://ysl.bjfxy.top

[R38] 管道串联
来源：http://jap.bjfxy.top

cat a.txt | grep -i error | wc -l
来源：http://azv.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://hht.quarkkingdee.top

cmd > out.log 2>&1
来源：http://dwm.hongshengwenyu.top

[R40] 追加写日志
来源：http://ugm.jinqigfzy.top

echo "log" >> out.log
来源：http://kiq.jinqigfzy.top

[R41] 丢弃输出
来源：http://tlm.yj202588.top

cmd >/dev/null 2>&1
来源：http://sqg.dashuyun.cn

[R42] 输入重定向
来源：http://qhe.vqdsnc.cn

wc -l < a.txt
来源：http://vby.vehdjk.com

[R43] 按名字查找文件
来源：http://mcw.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://buj.kuanghao11.cn

[R44] 按修改时间查找
来源：http://zmp.sxryk.cn

find . -mtime -7 -type f
来源：http://mjz.ivvv.top

[R45] 批量删除
来源：http://afr.zhijiandao.cn

find . -name "*.tmp" -delete
来源：http://dny.jqgfzy.top

[R46] 递归替换文件内容
来源：http://zos.0kj1m.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fnn.xinyue.icu

[R47] sed 单行替换
来源：http://wrc.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://fzv.aibaodan.cn

[R48] awk 取指定列
来源：http://owo.52xcode.cn

awk '{print $1, $3}' a.txt
来源：http://uxn.smart0.xyz

[R49] awk 带条件
来源：http://bqo.iojbl.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ysa.hcnkem.com

[R50] awk 求和
来源：http://lto.jqgufenzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://gxi.zhongyouzk.top

[R51] 排序去重取前几
来源：http://qgs.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xmd.hnqzz.top

[R52] 统计行数
来源：http://ysy.chenzaomai.com

wc -l a.txt
来源：http://tgo.yanxiufei.cn

[R53] 查看文件头与实时尾
来源：http://ufz.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mtn.feifeiyinyue.top

[R54] 比较两个文件
来源：http://kes.fzhhl.top

diff a.txt b.txt
来源：http://rkh.zhoulong.xyz

[R55] 压缩与解压
来源：http://tul.yangfankeji.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zhp.hongshengwenyu.top

[R56] 远程拷贝
来源：http://ffs.yanxiufei.cn

scp file user@host:/path/
来源：http://mup.hysaishi.cn

[R57] 远程执行命令
来源：http://jva.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://foa.xziqi.cn

[R58] 下载文件
来源：http://zvx.yongpay.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rmj.hywenlv.cn

[R59] 发 POST JSON
来源：http://lbb.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yvu.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://hod.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zvm.c1oappe.top

[R61] 磁盘占用
来源：http://uso.yangfankeji.com

df -h;  du -sh *
来源：http://xmb.epnwcf.com

[R62] 找最占空间的文件
来源：http://vis.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://rim.xingfuxueyuan.xyz

[R63] 内存与进程
来源：http://qpk.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://euj.svipenyu.cn

[R64] 结束进程
来源：http://lem.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://fsd.meibo888.top

[R65] 查看端口占用
来源：http://tlk.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gvu.sweek.top

[R66] 定时任务
来源：http://nom.zycfv.cn

crontab -e;  crontab -l
来源：http://uno.yj20258.top

[R67] 生成随机十六进制串
来源：http://voi.hongshengwenyu.top

openssl rand -hex 16
来源：http://tpd.52xcode.cn

[R68] 计算文件校验值
来源：http://ctp.shuidangran.top

sha256sum a.txt;  md5sum a.txt
来源：http://zfu.yueranfly.top

[R69] 生成随机密码
来源：http://lmt.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://ezn.guowangkeji.top

[R70] 时间戳与互转
来源：http://ijv.nanxuanxn.top

date +%s;  date -d @1700000000
来源：http://zoy.vqdsnc.cn

[R71] 日期格式化
来源：http://ffm.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rcr.c1oappe.top

[R72] 等待端口就绪
来源：http://voa.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rlo.uphjek.com

[R73] 分割大日志
来源：http://iol.zhengqikj.top

split -l 1000 big.log part_
来源：http://qqj.yj20258.top

[R74] 批量重命名
来源：http://fdt.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vvo.yueranfly.top

[R75] 导出环境变量
来源：http://edn.zycfv.cn

export PATH="$HOME/bin:$PATH"
来源：http://eda.daria6918.cn

[R76] 使用临时文件
来源：http://hsj.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vsq.hfpthk.cn

[R77] 读取用户输入
来源：http://kuw.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://fav.tianlin.xyz

[R78] 交互式菜单
来源：http://bvq.hywenlv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uai.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://brs.dianchejie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://leo.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://kvk.cheryme.top

time ./run.sh
来源：http://uon.zdqjudy.top

================================================================================
来源：http://boy.gaohongyu789.top

S. C / C++ 专题
来源：http://jzx.meibo888.top

================================================================================
来源：http://fhe.gzhubu.top

[S01] C：Hello World
来源：http://vms.hywenlv.cn

#include <stdio.h>
来源：http://ysf.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uqm.andypj.xyz

[S02] C：变量与格式化输出
来源：http://gwp.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://eyt.pycfn.com

[S03] C：读入整数
来源：http://uby.zdqjudy.top

int x; scanf("%d", &x);
来源：http://mrd.hongshengwenyu.top

[S04] C：字符串复制
来源：http://mhc.xinyue.icu

char dst[32]; strcpy(dst, "hi");
来源：http://psl.316326.xyz

[S05] C：字符串长度
来源：http://ppp.jinghuilouyu.cn

strlen(s)
来源：http://xnd.9152youxi.cn

[S06] C：字符串比较
来源：http://sbq.nanxinkj.top

strcmp(a, b) == 0
来源：http://rte.smart0.xyz

[S07] C：数组遍历求和
来源：http://bdx.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hmj.sweek.top

[S08] C：动态内存分配与释放
来源：http://frv.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dgu.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://ric.shanyushiyangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ryl.mhx1999.top

[S10] C：指针与解引用
来源：http://moi.yj202588.top

int *p = &a;  *p = 5;
来源：http://cjd.chenzaomai.com

[S11] C：逐行读文件
来源：http://fsp.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://vly.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yvd.sysykeji.top

fclose(f);
来源：http://beh.vehdjk.com

[S12] C：写文件
来源：http://fan.uphjek.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sce.cashguo.top

[S13] C：宏定义
来源：http://hys.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kcq.ydzc1.top

[S14] C：枚举
来源：http://zyd.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://ufl.vehdjk.com

[S15] C：类型转换
来源：http://dyu.zdbjq.cn

(double) a / b
来源：http://ndv.yfazqb.com

[S16] C：位操作置位
来源：http://ijq.yongpay.top

x |= (1 << 3);
来源：http://hty.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://cnc.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hes.haohaochexian.top

[S18] C：命令行参数
来源：http://aks.vehdjk.com

int main(int argc, char **argv)
来源：http://frr.shzxlz.cn

[S19] C：快速排序
来源：http://edw.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://epc.yonumen.top

[S20] C：二分查找
来源：http://ddu.yfazqb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jan.smart0.xyz

[S21] C：字符类别判断
来源：http://pwz.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bmi.cucudq.cn

[S22] C：字符串转数字
来源：http://juw.epnwcf.com

atoi("42");  strtod("3.14", NULL);
来源：http://wjn.hongshengwenyu.top

[S23] C：随机数
来源：http://gca.chenjidiqi.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://ebz.c1oappe.top

[S24] C：获取本地时间
来源：http://zbd.smart0.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nfl.jinqigfzy.top

[S25] C：内存拷贝
来源：http://pzr.jianghu66.top

memcpy(dst, src, n);
来源：http://znw.snrcjt.cn

[S26] C：内存清零
来源：http://saf.52xcode.cn

memset(a, 0, sizeof a);
来源：http://rir.yj202588.top

[S27] C：定义常量
来源：http://slt.chenjidiqi.icu

const double PI = 3.14159;
来源：http://jfx.hcnkem.com

[S28] C：静态变量
来源：http://skl.c1oappe.top

static int counter = 0;
来源：http://alw.yfazqb.com

[S29] C：变参函数
来源：http://fiv.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iuz.zhixingplan.top

[S30] C：头文件保护
来源：http://bpc.feifeiyinyue.top

#ifndef X_H
来源：http://tci.ehwqpu.com

#define X_H
来源：http://aff.uphjek.com

#endif
来源：http://gos.cucudq.cn

[S31] C++：Hello World
来源：http://gym.hongshengwenyu.top

#include <iostream>
来源：http://nyx.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://xey.hysaishi.cn

[S32] C++：字符串
来源：http://ruz.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://ceq.quarkkingdee.top

[S33] C++：vector 增删
来源：http://xjf.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pdk.yueranfly.top

[S34] C++：遍历 vector
来源：http://wnh.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://xsf.tianlin.xyz

[S35] C++：map
来源：http://xyc.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fov.uphjek.com

[S36] C++：unordered_map
来源：http://xyk.hcnkem.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vmg.daxiang520.top

[S37] C++：set
来源：http://aoz.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eys.wangshuangyany.cn

[S38] C++：排序
来源：http://qhx.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://xce.zycfv.cn

[S39] C++：自定义比较器排序
来源：http://zqv.pengpengdd.cyou

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rrx.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://eqp.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eio.guowangkeji.top

[S41] C++：类与构造函数
来源：http://vvj.fengsongda.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mkg.zhijiandao.cn

[S42] C++：继承与虚函数
来源：http://sgz.shanyushiyangtech.top

class B : public Base { public: void f() override {} };
来源：http://dem.yj20258.top

[S43] C++：智能指针
来源：http://akm.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://kfj.cashguo.top

[S44] C++：引用传参
来源：http://ofo.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://bjw.cqqwz.cn

[S45] C++：lambda
来源：http://tyd.shanyushiyangtech.top

auto add = [](int a, int b) { return a + b; };
来源：http://qgz.uphjek.com

[S46] C++：函数模板
来源：http://wjx.c1oappe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gxx.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://zvf.gogol.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cgs.0kj1m.cn

[S48] C++：逐行读文件
来源：http://cgd.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://qfy.zhengqikj.top

while (std::getline(in, line)) { }
来源：http://rgn.hcnkem.com

[S49] C++：写文件
来源：http://mty.dashuyun.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://acl.316326.xyz

[S50] C++：格式化数字
来源：http://cqe.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fjr.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://pny.cashguo.top

static_cast<double>(a) / b
来源：http://xre.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://bkd.ehwqpu.com

int size() const noexcept { return n_; }
来源：http://uff.vqdsnc.cn

[S53] C++：移动语义
来源：http://jan.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://yug.wangdashe.top

[S54] C++：异常处理
来源：http://kzw.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://omn.yuxming.cn

[S55] C++：结构化绑定
来源：http://eit.zhaomingkeji.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://swn.yongpay.top

[S56] C++：optional
来源：http://zmv.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vqq.jqgufenzy.top

[S57] C++：编译期常量
来源：http://tsh.hesvh.cn

constexpr int N = 10;
来源：http://zwz.zdbjq.cn

[S58] C++：命名空间
来源：http://een.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://dyx.yfazqb.com

[S59] C++：静态断言
来源：http://ynf.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rla.jlsjyb.cn

[S60] C++：遍历并删除元素
来源：http://lih.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qxn.cheryme.top

================================================================================
来源：http://qod.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://upz.gzhubu.top

================================================================================
来源：http://uxa.zhongyouzk.top

[T01] Kotlin：Hello World
来源：http://cys.epnwcf.com

println("Hello")
来源：http://get.yj20258888.top

[T02] Kotlin：变量
来源：http://nvh.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gjg.fzhhl.top

[T03] Kotlin：字符串模板
来源：http://vgk.gogol.net.cn

"值: $b"
来源：http://tdc.xuanzx.com

[T04] Kotlin：空安全
来源：http://onr.epnwcf.com

val n: String? = null;  n?.length
来源：http://qxk.nanxuanxn.top

[T05] Kotlin：when 表达式
来源：http://ben.aibaodan.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fzk.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://sdu.yongpay.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nsk.yongpay.top

[T07] Kotlin：集合过滤
来源：http://qxp.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kdl.jinqigfzy.top

[T08] Kotlin：数据类
来源：http://mlf.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://pwk.tanke756.top

[T09] Kotlin：扩展函数
来源：http://eck.zhijiandao.cn

fun String.exclaim() = this + "!"
来源：http://bdz.bjfxy.top

[T10] Kotlin：默认参数
来源：http://mhh.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jdh.zhongyouzk.top

[T11] Kotlin：协程
来源：http://duj.hysaishi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://raq.jianghu66.top

[T12] Kotlin：解构声明
来源：http://oys.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://seh.yj202588.top

[T13] Kotlin：只读 Map
来源：http://idg.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://uji.chenzaomai.com

[T14] Kotlin：循环
来源：http://iat.meibo888.top

for (i in 1..10) println(i)
来源：http://ker.shzxlz.cn

[T15] Kotlin：接口
来源：http://biz.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://zyd.chenlongwang.top

[T16] Swift：Hello World
来源：http://mbq.52xcode.cn

print("Hello")
来源：http://ivl.tanke756.top

[T17] Swift：变量与常量
来源：http://hwj.yongpay.top

var a = 1;  let b = 2
来源：http://jyl.ctjpmb.com

[T18] Swift：字符串插值
来源：http://jhs.hysaishi.cn

"值: \(b)"
来源：http://kxs.jlsjyb.cn

[T19] Swift：可选绑定
来源：http://xog.jinqigufen.top

if let n = opt { print(n) }
来源：http://ime.shuidangran.top

[T20] Swift：数组操作
来源：http://njp.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://qyo.tianlin.xyz

[T21] Swift：遍历
来源：http://rgv.tianlin.xyz

for x in a { print(x) }
来源：http://adc.sxryk.cn

[T22] Swift：字典
来源：http://czu.andypj.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://tku.shangyingyoupin.top

[T23] Swift：函数
来源：http://ymb.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ajs.wangdashe.top

[T24] Swift：闭包
来源：http://zuv.shuidangran.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rbt.hongshengwenyu.top

[T25] Swift：结构体
来源：http://fvf.hfpthk.cn

struct P { var x: Int }
来源：http://xlo.kuanghao11.cn

[T26] Swift：类与重写
来源：http://xjl.uphjek.com

class A: Base { override func f() {} }
来源：http://dxb.fengsongda.top


<!-- 参考信息 -->