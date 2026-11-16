代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qag.xylfe.cn

[R24] 大小写转换
来源：http://ulr.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://afc.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://hlt.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://ivg.hcnkem.com

[R26] 命令替换
来源：http://kal.mhx1999.top

now=$(date +%F); echo "$now"
来源：http://drv.zycfv.cn

[R27] 算术展开
来源：http://fxb.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://lgc.ydzc1.top

[R28] 浮点运算
来源：http://eze.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://oem.fktsv.cn

[R29] 定义函数
来源：http://twp.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ngm.yanxiufei.cn

[R30] 函数返回状态码
来源：http://acs.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://mec.c1oappe.top

[R31] 局部变量
来源：http://lkm.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://uym.aibaodan.cn

[R32] 参数个数校验
来源：http://noz.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pqj.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://lna.fktsv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cgq.xylfe.cn

[R34] 退出时清理
来源：http://gnf.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://oxi.xziqi.cn

[R35] 后台执行并等待
来源：http://xhc.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ztx.zycfv.cn

[R36] 并发执行多个任务
来源：http://zua.hammf.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gxs.xuanzx.com

[R37] 把输出赋给变量
来源：http://fhq.shzxlz.cn

files=$(ls -1)
来源：http://mnl.jiagoushi.top

[R38] 管道串联
来源：http://jmg.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://prz.pycfn.com

[R39] 重定向标准输出与错误
来源：http://jcm.jyoumei.cn

cmd > out.log 2>&1
来源：http://hje.gaohongyu789.top

[R40] 追加写日志
来源：http://nhy.gotoacloud.top

echo "log" >> out.log
来源：http://kef.xziqi.cn

[R41] 丢弃输出
来源：http://qcn.redwolf501.top

cmd >/dev/null 2>&1
来源：http://ulf.smart0.xyz

[R42] 输入重定向
来源：http://nvr.9152youxi.cn

wc -l < a.txt
来源：http://cdb.ydzc1.top

[R43] 按名字查找文件
来源：http://hxq.jiagoushi.top

find . -name "*.log" -type f
来源：http://xyd.bjfxy.top

[R44] 按修改时间查找
来源：http://prf.zdbjq.cn

find . -mtime -7 -type f
来源：http://mke.tian-w.cn

[R45] 批量删除
来源：http://iax.nwbrower.top

find . -name "*.tmp" -delete
来源：http://mrv.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://moq.jyoumei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ycv.mhx1999.top

[R47] sed 单行替换
来源：http://osb.mhx1999.top

sed -i 's/foo/bar/g' a.txt
来源：http://ldz.snrcjt.cn

[R48] awk 取指定列
来源：http://mqr.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://gsi.fehbvm.com

[R49] awk 带条件
来源：http://baf.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jll.hcnkem.com

[R50] awk 求和
来源：http://ays.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://jem.ydzc1.top

[R51] 排序去重取前几
来源：http://thy.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://cbx.c1oappe.top

[R52] 统计行数
来源：http://sbf.fanxiaobao.xyz

wc -l a.txt
来源：http://uqs.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://otf.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://htm.xinyue.icu

[R54] 比较两个文件
来源：http://eyq.ehwqpu.com

diff a.txt b.txt
来源：http://vvn.vqdsnc.cn

[R55] 压缩与解压
来源：http://lgm.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://djm.sufxvd.cn

[R56] 远程拷贝
来源：http://suy.chenlongwang.top

scp file user@host:/path/
来源：http://rbl.tanke756.top

[R57] 远程执行命令
来源：http://ybs.zhongyouzk.top

ssh user@host 'uptime'
来源：http://kwl.andypj.xyz

[R58] 下载文件
来源：http://qjv.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pzs.sxryk.cn

[R59] 发 POST JSON
来源：http://txx.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://edm.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://avc.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ets.yuxming.cn

[R61] 磁盘占用
来源：http://epw.uphjek.com

df -h;  du -sh *
来源：http://dew.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://xoe.andypj.xyz

du -ah . | sort -rh | head -10
来源：http://wfa.hnqzz.top

[R63] 内存与进程
来源：http://ujo.hesvh.cn

free -h;  ps aux | grep nginx
来源：http://ssh.hnxiangtu.top

[R64] 结束进程
来源：http://bdf.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://tbm.gaohongyu789.top

[R65] 查看端口占用
来源：http://jzv.nanxuanxn.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gtv.shuidangran.top

[R66] 定时任务
来源：http://nzm.c1oappe.top

crontab -e;  crontab -l
来源：http://ctg.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://gxn.zhongyouzk.top

openssl rand -hex 16
来源：http://ycy.tarul.cn

[R68] 计算文件校验值
来源：http://wqb.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fup.ehwqpu.com

[R69] 生成随机密码
来源：http://axz.bbcook.cn

head -c 16 /dev/urandom | base64
来源：http://syf.guannengcc.top

[R70] 时间戳与互转
来源：http://kif.jqgufenzy.top

date +%s;  date -d @1700000000
来源：http://zfx.hesvh.cn

[R71] 日期格式化
来源：http://jqn.bbcook.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ysg.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://fby.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fsl.gotoacloud.top

[R73] 分割大日志
来源：http://ean.birdmap.top

split -l 1000 big.log part_
来源：http://jnv.wangdashe.top

[R74] 批量重命名
来源：http://ksf.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iig.sjlbkw.cn

[R75] 导出环境变量
来源：http://scy.ppjwa.cn

export PATH="$HOME/bin:$PATH"
来源：http://kla.sysykeji.top

[R76] 使用临时文件
来源：http://tis.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jan.gogol.net.cn

[R77] 读取用户输入
来源：http://uct.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://hoc.hammf.cn

[R78] 交互式菜单
来源：http://tqb.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fmh.aibaodan.cn

[R79] 解析命令行选项
来源：http://gwl.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://boj.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://szx.xylfe.cn

time ./run.sh
来源：http://bvb.tianlin.xyz

================================================================================
来源：http://ckq.ctjpmb.com

S. C / C++ 专题
来源：http://egz.9152youxi.cn

================================================================================
来源：http://qtw.fzhhl.top

[S01] C：Hello World
来源：http://yzs.dianchejie.cn

#include <stdio.h>
来源：http://yke.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kfh.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://pca.jinqigfzy.top

int a = 10; printf("%d\n", a);
来源：http://tea.ctjpmb.com

[S03] C：读入整数
来源：http://fao.jinqigufen.top

int x; scanf("%d", &x);
来源：http://msc.guowangkeji.top

[S04] C：字符串复制
来源：http://nzu.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wlf.yfazqb.com

[S05] C：字符串长度
来源：http://wnz.52xcode.cn

strlen(s)
来源：http://emd.shzxlz.cn

[S06] C：字符串比较
来源：http://ljq.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://cra.bjfxy.top

[S07] C：数组遍历求和
来源：http://mwz.tanke756.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ywh.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://tfd.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nys.shanyushiyangkeji.top

[S09] C：结构体定义与初始化
来源：http://uap.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lej.redwolf501.top

[S10] C：指针与解引用
来源：http://dcz.havefunace.top

int *p = &a;  *p = 5;
来源：http://dlz.yuxming.cn

[S11] C：逐行读文件
来源：http://ysg.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://kwm.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kpb.chenzaomai.com

fclose(f);
来源：http://inr.nwbrower.top

[S12] C：写文件
来源：http://puj.guowangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ggc.cheryme.top

[S13] C：宏定义
来源：http://fnm.hongshengwenyu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jgw.52xcode.cn

[S14] C：枚举
来源：http://wwf.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://urk.havefunace.top

[S15] C：类型转换
来源：http://fwn.xziqi.cn

(double) a / b
来源：http://yre.yuanzhike.top

[S16] C：位操作置位
来源：http://cbm.ydjk.org.cn

x |= (1 << 3);
来源：http://qjr.bbcook.cn

[S17] C：安全拼接字符串
来源：http://dtv.shzxlz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://krk.nwbrower.top

[S18] C：命令行参数
来源：http://dzi.yongpay.top

int main(int argc, char **argv)
来源：http://vkd.dashuyun.cn

[S19] C：快速排序
来源：http://yti.daria6918.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zjo.xinyue.icu

[S20] C：二分查找
来源：http://mbw.jlsjyb.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vrg.ywan-chungtsiang.top

[S21] C：字符类别判断
来源：http://zgw.xziqi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lsd.cheryme.top

[S22] C：字符串转数字
来源：http://flk.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://knm.jinghuilouyu.cn

[S23] C：随机数
来源：http://xtj.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gdk.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://ecp.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bbd.vqdsnc.cn

[S25] C：内存拷贝
来源：http://xbt.fehbvm.com

memcpy(dst, src, n);
来源：http://env.ppjwa.cn

[S26] C：内存清零
来源：http://rex.yongpay.top

memset(a, 0, sizeof a);
来源：http://hgx.shuidangran.top

[S27] C：定义常量
来源：http://zwa.havefunace.top

const double PI = 3.14159;
来源：http://lnn.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://cru.ywan-chungtsiang.top

static int counter = 0;
来源：http://hoq.xuetiantiany.cn

[S29] C：变参函数
来源：http://hxq.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pil.hcnkem.com

[S30] C：头文件保护
来源：http://dce.0kj1m.cn

#ifndef X_H
来源：http://rom.ehwqpu.com

#define X_H
来源：http://wsl.yonumen.top

#endif
来源：http://zpb.zhijiandao.cn

[S31] C++：Hello World
来源：http://ssy.jiagoushi.top

#include <iostream>
来源：http://ljx.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://nej.jianghu66.top

[S32] C++：字符串
来源：http://fje.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://nna.zhoulong.xyz

[S33] C++：vector 增删
来源：http://jum.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oxf.aizwys.cn

[S34] C++：遍历 vector
来源：http://auj.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://tak.gotoacloud.top

[S35] C++：map
来源：http://bxd.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lpw.feifeiyinyue.top

[S36] C++：unordered_map
来源：http://teb.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bas.zhengqikj.top

[S37] C++：set
来源：http://dlr.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://exw.smart0.xyz

[S38] C++：排序
来源：http://gye.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://nap.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://zoj.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xro.iojbl.cn

[S40] C++：查找元素
来源：http://tbu.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jsu.zycfv.cn

[S41] C++：类与构造函数
来源：http://mih.ehwqpu.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://htp.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://hzh.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://amf.aizwys.cn

[S43] C++：智能指针
来源：http://pgl.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://exx.ybcxt.top

[S44] C++：引用传参
来源：http://dbd.dianchejie.cn

void inc(int &x) { ++x; }
来源：http://zls.nanxinkj.top

[S45] C++：lambda
来源：http://wza.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rkp.ehwqpu.com

[S46] C++：函数模板
来源：http://aoc.ivvv.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sba.nanxuanxn.top

[S47] C++：结构化绑定遍历
来源：http://jyz.jianghu66.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ckc.svipenyu.cn

[S48] C++：逐行读文件
来源：http://gym.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://agg.yongpay.top

while (std::getline(in, line)) { }
来源：http://rxg.jinqigufen.top

[S49] C++：写文件
来源：http://fhm.gotoacloud.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://isk.zhoulong.xyz

[S50] C++：格式化数字
来源：http://ure.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oir.ydjk.org.cn

[S51] C++：显式类型转换
来源：http://rsi.fzhhl.top

static_cast<double>(a) / b
来源：http://rgp.jianghu66.top

[S52] C++：const 与 noexcept
来源：http://exk.hongshengwenyu.top

int size() const noexcept { return n_; }
来源：http://mrt.xinyue.icu

[S53] C++：移动语义
来源：http://fif.shzxlz.cn

std::vector<int> w = std::move(v);
来源：http://xsu.xinyue.icu

[S54] C++：异常处理
来源：http://ghh.zhoulong.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fbw.epnwcf.com

[S55] C++：结构化绑定
来源：http://xao.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://aii.birdmap.top

[S56] C++：optional
来源：http://zzq.snrcjt.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cbj.xylfe.cn

[S57] C++：编译期常量
来源：http://wch.zhoulong.xyz

constexpr int N = 10;
来源：http://nuy.yanxiufei.cn

[S58] C++：命名空间
来源：http://pvc.chenjidiqi.icu

namespace ns { int f() { return 1; } }
来源：http://acx.svipenyu.cn

[S59] C++：静态断言
来源：http://udp.ywan-chungtsiang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ebw.zdbjq.cn

[S60] C++：遍历并删除元素
来源：http://pah.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yyy.dashuyun.cn

================================================================================
来源：http://kts.zdqjudy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lej.fehbvm.com

================================================================================
来源：http://src.zhiwuduotai.top

[T01] Kotlin：Hello World
来源：http://cpo.nwbrower.top

println("Hello")
来源：http://shk.bjfxy.top

[T02] Kotlin：变量
来源：http://hke.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://log.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://swg.pycfn.com

"值: $b"
来源：http://efq.yangfankeji.com

[T04] Kotlin：空安全
来源：http://hdc.tarul.cn

val n: String? = null;  n?.length
来源：http://njv.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://vyu.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hoa.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://zxf.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://jvh.hongshengwenyu.top

[T07] Kotlin：集合过滤
来源：http://mqw.hammf.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bue.hammf.cn

[T08] Kotlin：数据类
来源：http://tjn.sxryk.cn

data class User(val name: String, val age: Int)
来源：http://avo.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://wgz.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://euc.zycfv.cn

[T10] Kotlin：默认参数
来源：http://iym.epnwcf.com

fun greet(name: String = "World") = "Hi $name"
来源：http://urh.fktsv.cn

[T11] Kotlin：协程
来源：http://buy.yfazqb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://tqu.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://zmo.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://vgt.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://oaz.ivvv.top

val m = mapOf("a" to 1)
来源：http://ezm.vehdjk.com

[T14] Kotlin：循环
来源：http://asl.meibo888.top

for (i in 1..10) println(i)
来源：http://zeg.52xcode.cn

[T15] Kotlin：接口
来源：http://bgw.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://emi.gzhubu.top

[T16] Swift：Hello World
来源：http://lpv.svipenyu.cn

print("Hello")
来源：http://lpc.yueranfly.top

[T17] Swift：变量与常量
来源：http://gou.c1oappe.top

var a = 1;  let b = 2
来源：http://fdl.yuanzhike.top

[T18] Swift：字符串插值
来源：http://jiv.nanxinkj.top

"值: \(b)"
来源：http://mvs.zdqjudy.top

[T19] Swift：可选绑定
来源：http://aqa.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://jaa.nanxuanxn.top

[T20] Swift：数组操作
来源：http://uhm.ivvv.top

var a = [1, 2, 3];  a.append(4)
来源：http://dvc.zhixingplan.top

[T21] Swift：遍历
来源：http://rgc.aizwys.cn

for x in a { print(x) }
来源：http://wuc.wangshuangyany.cn

[T22] Swift：字典
来源：http://hme.jqgufenzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://ngd.fzhhl.top

[T23] Swift：函数
来源：http://vae.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qzm.shzxlz.cn

[T24] Swift：闭包
来源：http://bhi.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gxo.hysaishi.cn

[T25] Swift：结构体
来源：http://tjl.yvedp.cn

struct P { var x: Int }
来源：http://miq.yj20258.top

[T26] Swift：类与重写
来源：http://fes.xylfe.cn

class A: Base { override func f() {} }
来源：http://rcv.haohaochexian.top


<!-- 参考信息 -->