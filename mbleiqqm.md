代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://fvf.hnxiangtu.top

[R26] 命令替换
来源：http://ngb.fehbvm.com

now=$(date +%F); echo "$now"
来源：http://wnr.316326.xyz

[R27] 算术展开
来源：http://gzp.shuidangran.top

echo $((1 + 2 * 3))
来源：http://emy.ybcxt.top

[R28] 浮点运算
来源：http://ujw.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://ctk.jqgufenzy.top

[R29] 定义函数
来源：http://vhf.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mcg.shuidangran.top

[R30] 函数返回状态码
来源：http://ekp.quarkkingdee.top

f() { return 0; }; f || echo "失败了"
来源：http://yng.ydjk.org.cn

[R31] 局部变量
来源：http://guc.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://vlo.wangshuangyany.cn

[R32] 参数个数校验
来源：http://gzv.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dbx.fzhhl.top

[R33] 捕获错误并提示行号
来源：http://bjm.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zjm.vehdjk.com

[R34] 退出时清理
来源：http://azg.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://ito.sufxvd.cn

[R35] 后台执行并等待
来源：http://ozb.pengpengdd.cyou

sleep 5 & pid=$!; wait "$pid"
来源：http://vxs.cashguo.top

[R36] 并发执行多个任务
来源：http://gzq.ydjk.org.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://luf.hammf.cn

[R37] 把输出赋给变量
来源：http://umi.mhx1999.top

files=$(ls -1)
来源：http://nts.dashuyun.cn

[R38] 管道串联
来源：http://htb.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://zze.sufxvd.cn

[R39] 重定向标准输出与错误
来源：http://lsb.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://vps.fehbvm.com

[R40] 追加写日志
来源：http://fwt.jinqigufen.top

echo "log" >> out.log
来源：http://khg.wangdashe.top

[R41] 丢弃输出
来源：http://lfg.smart0.xyz

cmd >/dev/null 2>&1
来源：http://yzi.sufxvd.cn

[R42] 输入重定向
来源：http://cpn.fzhhl.top

wc -l < a.txt
来源：http://eib.chenlongwang.top

[R43] 按名字查找文件
来源：http://pnq.aizwys.cn

find . -name "*.log" -type f
来源：http://vrr.hammf.cn

[R44] 按修改时间查找
来源：http://gps.yj202588.top

find . -mtime -7 -type f
来源：http://ysl.shuidangran.top

[R45] 批量删除
来源：http://krs.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://cya.meibo888.top

[R46] 递归替换文件内容
来源：http://zaj.jqgufenzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fzs.xuanzx.com

[R47] sed 单行替换
来源：http://zys.daxiang520.top

sed -i 's/foo/bar/g' a.txt
来源：http://nzr.havefunace.top

[R48] awk 取指定列
来源：http://tcc.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://uxg.zhijiandao.cn

[R49] awk 带条件
来源：http://jsh.cucudq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mot.vehdjk.com

[R50] awk 求和
来源：http://kkc.tianlin.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://jpa.ydjk.org.cn

[R51] 排序去重取前几
来源：http://ciz.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://khu.meibo888.top

[R52] 统计行数
来源：http://fka.dashuyun.cn

wc -l a.txt
来源：http://mqc.pengpengdd.cyou

[R53] 查看文件头与实时尾
来源：http://weg.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ivj.dashuyun.cn

[R54] 比较两个文件
来源：http://dos.feifeiyinyue.top

diff a.txt b.txt
来源：http://vds.zdqjudy.top

[R55] 压缩与解压
来源：http://cip.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uqj.zhijiandao.cn

[R56] 远程拷贝
来源：http://fgp.yj202588.top

scp file user@host:/path/
来源：http://sxy.yj20258.top

[R57] 远程执行命令
来源：http://inh.cqqwz.cn

ssh user@host 'uptime'
来源：http://gie.shanyushiyangtech.top

[R58] 下载文件
来源：http://wqg.hysaishi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iks.zhengqikj.top

[R59] 发 POST JSON
来源：http://kdg.ehwqpu.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ltr.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://fsx.nanxuanxn.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wsj.9152youxi.cn

[R61] 磁盘占用
来源：http://coh.zhijiandao.cn

df -h;  du -sh *
来源：http://yaz.sufxvd.cn

[R62] 找最占空间的文件
来源：http://sxg.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://yro.shanyushiyangkeji.top

[R63] 内存与进程
来源：http://mtk.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://phj.guowangkeji.top

[R64] 结束进程
来源：http://sol.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://woi.zhiwuduotai.top

[R65] 查看端口占用
来源：http://gsj.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jwt.jlsjyb.cn

[R66] 定时任务
来源：http://wod.guannengcc.top

crontab -e;  crontab -l
来源：http://vmu.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://ruo.mhx1999.top

openssl rand -hex 16
来源：http://sef.cqqwz.cn

[R68] 计算文件校验值
来源：http://sza.fktsv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ygs.hongshengwenyu.top

[R69] 生成随机密码
来源：http://ryg.sweek.top

head -c 16 /dev/urandom | base64
来源：http://isq.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://fvg.zhoulong.xyz

date +%s;  date -d @1700000000
来源：http://xhq.sysykeji.top

[R71] 日期格式化
来源：http://etg.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qcj.cqqwz.cn

[R72] 等待端口就绪
来源：http://ndu.316326.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://esm.shanyushiyangtech.top

[R73] 分割大日志
来源：http://rmt.vehdjk.com

split -l 1000 big.log part_
来源：http://srx.yongpay.top

[R74] 批量重命名
来源：http://fwx.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zdg.tianlin.xyz

[R75] 导出环境变量
来源：http://gmw.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://wqk.hesvh.cn

[R76] 使用临时文件
来源：http://cqy.jlsjyb.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gsq.hammf.cn

[R77] 读取用户输入
来源：http://ogz.vqdsnc.cn

read -rp "请输入: " ans
来源：http://iob.tanke756.top

[R78] 交互式菜单
来源：http://tvq.tianlin.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://khf.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://obw.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ljn.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://igp.chenlongwang.top

time ./run.sh
来源：http://nji.epnwcf.com

================================================================================
来源：http://xan.chenzaomai.com

S. C / C++ 专题
来源：http://vku.xinyue.icu

================================================================================
来源：http://kfz.cheryme.top

[S01] C：Hello World
来源：http://pcu.jqgfzy.top

#include <stdio.h>
来源：http://qda.shanyushiyangtech.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bbr.yj202588.top

[S02] C：变量与格式化输出
来源：http://pnu.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://gvx.shuidangran.top

[S03] C：读入整数
来源：http://ibk.daria6918.cn

int x; scanf("%d", &x);
来源：http://xze.sysykeji.top

[S04] C：字符串复制
来源：http://wfw.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://spi.yangfankeji.com

[S05] C：字符串长度
来源：http://nva.aibaodan.cn

strlen(s)
来源：http://eeg.jqgufenzy.top

[S06] C：字符串比较
来源：http://czy.birdmap.top

strcmp(a, b) == 0
来源：http://kuk.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://twc.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xag.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://wcj.cqqwz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uwa.gaohongyu789.top

[S09] C：结构体定义与初始化
来源：http://ypx.xylfe.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rxt.jqgfzy.top

[S10] C：指针与解引用
来源：http://tjg.bbcook.cn

int *p = &a;  *p = 5;
来源：http://awh.sweek.top

[S11] C：逐行读文件
来源：http://zoh.tarul.cn

FILE *f = fopen("a.txt", "r");
来源：http://unt.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://rwa.pengpengdd.cyou

fclose(f);
来源：http://jtq.zhengqikj.top

[S12] C：写文件
来源：http://xbx.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gjj.daria6918.cn

[S13] C：宏定义
来源：http://miz.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xoi.bjfxy.top

[S14] C：枚举
来源：http://kon.sxryk.cn

enum Color { RED, GREEN, BLUE };
来源：http://zzr.sysykeji.top

[S15] C：类型转换
来源：http://mmx.zhongyouzk.top

(double) a / b
来源：http://mpa.jinghuilouyu.cn

[S16] C：位操作置位
来源：http://cek.cqqwz.cn

x |= (1 << 3);
来源：http://vqf.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://kqz.yuanzhike.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://los.kuanghao11.cn

[S18] C：命令行参数
来源：http://rii.ydzc1.top

int main(int argc, char **argv)
来源：http://bac.shangyingyoupin.top

[S19] C：快速排序
来源：http://tak.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://obc.bbcook.cn

[S20] C：二分查找
来源：http://cef.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tuc.chenzaomai.com

[S21] C：字符类别判断
来源：http://uio.svipenyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mft.xuetiantiany.cn

[S22] C：字符串转数字
来源：http://gno.hnqzz.top

atoi("42");  strtod("3.14", NULL);
来源：http://zlg.zhongyouzk.top

[S23] C：随机数
来源：http://nma.gzhubu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dhq.jiagoushi.top

[S24] C：获取本地时间
来源：http://nbp.gzhubu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://elt.ppjwa.cn

[S25] C：内存拷贝
来源：http://hat.yuanzhike.top

memcpy(dst, src, n);
来源：http://ixk.hammf.cn

[S26] C：内存清零
来源：http://jmc.pengpengdd.cyou

memset(a, 0, sizeof a);
来源：http://xro.vqdsnc.cn

[S27] C：定义常量
来源：http://fib.jlsjyb.cn

const double PI = 3.14159;
来源：http://jwz.feifeiyinyue.top

[S28] C：静态变量
来源：http://pei.zhiwuduotai.top

static int counter = 0;
来源：http://kow.zhixingplan.top

[S29] C：变参函数
来源：http://crs.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uug.chenjidiqi.icu

[S30] C：头文件保护
来源：http://tee.hongshengwenyu.top

#ifndef X_H
来源：http://dqx.cashguo.top

#define X_H
来源：http://ljo.316326.xyz

#endif
来源：http://zzb.wangdashe.top

[S31] C++：Hello World
来源：http://mfr.jinqigufen.top

#include <iostream>
来源：http://jse.jinqigufen.top

int main() { std::cout << "Hello\n"; }
来源：http://bcj.yj20258.top

[S32] C++：字符串
来源：http://kyp.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://mkp.yvedp.cn

[S33] C++：vector 增删
来源：http://cmh.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://igl.zhixingplan.top

[S34] C++：遍历 vector
来源：http://lta.mhx1999.top

for (auto &x : v) { std::cout << x; }
来源：http://rgb.shangyingyoupin.top

[S35] C++：map
来源：http://gmf.yuxming.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sjf.jyoumei.cn

[S36] C++：unordered_map
来源：http://psz.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uqh.hammf.cn

[S37] C++：set
来源：http://kxt.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qum.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://myk.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://utx.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://paz.aibaodan.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zgr.jianghu66.top

[S40] C++：查找元素
来源：http://myh.hywenlv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gbg.yuxming.cn

[S41] C++：类与构造函数
来源：http://pfk.smart0.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://abz.redwolf501.top

[S42] C++：继承与虚函数
来源：http://ftb.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://crh.quarkkingdee.top

[S43] C++：智能指针
来源：http://wbf.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://fel.zhoulong.xyz

[S44] C++：引用传参
来源：http://qnj.kuanghao11.cn

void inc(int &x) { ++x; }
来源：http://pzh.sysykeji.top

[S45] C++：lambda
来源：http://wjn.jinyuanbaomall.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fny.hnqzz.top

[S46] C++：函数模板
来源：http://rqu.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gmg.yueranfly.top

[S47] C++：结构化绑定遍历
来源：http://lnr.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bhb.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://epj.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oyd.fktsv.cn

while (std::getline(in, line)) { }
来源：http://ejo.yj20258888.top

[S49] C++：写文件
来源：http://mtr.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eqm.andypj.xyz

[S50] C++：格式化数字
来源：http://ylt.pycfn.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wko.yj20258888.top

[S51] C++：显式类型转换
来源：http://tny.tian-w.cn

static_cast<double>(a) / b
来源：http://plc.ppjwa.cn

[S52] C++：const 与 noexcept
来源：http://sls.sysykeji.top

int size() const noexcept { return n_; }
来源：http://iyw.kuanghao11.cn

[S53] C++：移动语义
来源：http://iqi.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://wwc.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://eyw.yangfankeji.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eih.gogol.net.cn

[S55] C++：结构化绑定
来源：http://nja.ydzc1.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kcw.wangshuangyany.cn

[S56] C++：optional
来源：http://ltx.fanxiaobao.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fgs.ctjpmb.com

[S57] C++：编译期常量
来源：http://awm.hammf.cn

constexpr int N = 10;
来源：http://ioj.pycfn.com

[S58] C++：命名空间
来源：http://ajx.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://oxk.chenlongwang.top

[S59] C++：静态断言
来源：http://fyy.vehdjk.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cqr.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://mwi.yuanzhike.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dgu.tarul.cn

================================================================================
来源：http://gam.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bsj.52xcode.cn

================================================================================
来源：http://nbt.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://dwk.hnqzz.top

println("Hello")
来源：http://tdo.yangfankeji.com

[T02] Kotlin：变量
来源：http://sgd.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yiw.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://hvx.fzhhl.top

"值: $b"
来源：http://phl.yfazqb.com

[T04] Kotlin：空安全
来源：http://koj.cucudq.cn

val n: String? = null;  n?.length
来源：http://nrh.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://pvy.yanxiufei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zvh.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://ock.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jwv.0kj1m.cn

[T07] Kotlin：集合过滤
来源：http://tgc.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kwo.316326.xyz

[T08] Kotlin：数据类
来源：http://pvv.tianlin.xyz

data class User(val name: String, val age: Int)
来源：http://prr.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://gha.zhiwuduotai.top

fun String.exclaim() = this + "!"
来源：http://qdm.svipenyu.cn

[T10] Kotlin：默认参数
来源：http://evz.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://doc.snrcjt.cn

[T11] Kotlin：协程
来源：http://vrd.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://wjv.52xcode.cn

[T12] Kotlin：解构声明
来源：http://hby.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://iea.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://vam.0kj1m.cn

val m = mapOf("a" to 1)
来源：http://aov.gotoacloud.top

[T14] Kotlin：循环
来源：http://ltk.hammf.cn

for (i in 1..10) println(i)
来源：http://jre.bbcook.cn

[T15] Kotlin：接口
来源：http://iok.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://kpo.jqgufenzy.top

[T16] Swift：Hello World
来源：http://zpt.yuanzhike.top

print("Hello")
来源：http://nml.tarul.cn

[T17] Swift：变量与常量
来源：http://fse.sxryk.cn

var a = 1;  let b = 2
来源：http://aqz.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://vkq.sxryk.cn

"值: \(b)"
来源：http://ghg.smart0.xyz

[T19] Swift：可选绑定
来源：http://czd.zhixingplan.top

if let n = opt { print(n) }
来源：http://ehp.yangfankeji.com

[T20] Swift：数组操作
来源：http://twj.hongshengwenyu.top

var a = [1, 2, 3];  a.append(4)
来源：http://amu.zhongyouzk.top

[T21] Swift：遍历
来源：http://zla.shanyushiyangtech.top

for x in a { print(x) }
来源：http://bst.chenzaomai.com

[T22] Swift：字典
来源：http://glz.sjlbkw.cn

var d = ["a": 1];  d["b"] = 2
来源：http://too.gaohongyu789.top

[T23] Swift：函数
来源：http://cdp.shanyushiyangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bzh.jqgfzy.top

[T24] Swift：闭包
来源：http://jyx.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kmv.cashguo.top

[T25] Swift：结构体
来源：http://hsb.nwbrower.top

struct P { var x: Int }
来源：http://kye.fzhhl.top

[T26] Swift：类与重写
来源：http://nsh.hysaishi.cn

class A: Base { override func f() {} }
来源：http://aeo.ybcxt.top

[T27] Swift：错误处理
来源：http://wua.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://cph.zdqjudy.top

[T28] Swift：枚举
来源：http://lfj.cheryme.top

enum Color { case red, green }
来源：http://vtf.bbcook.cn


<!-- 参考信息 -->