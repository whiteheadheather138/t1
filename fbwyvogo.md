代发 wailian999

echo "${#s}"
来源：http://hih.yj202588.top

[R22] 截取子串
来源：http://vnx.redwolf501.top

echo "${s:0:5}"
来源：http://xhs.9152youxi.cn

[R23] 字符串替换
来源：http://kyv.dianchejie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tga.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://wyj.dianchejie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gef.pengpengdd.cyou

[R25] 去后缀 / 去前缀
来源：http://tdb.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gwk.xylfe.cn

[R26] 命令替换
来源：http://chn.daria6918.cn

now=$(date +%F); echo "$now"
来源：http://lho.ydzc1.top

[R27] 算术展开
来源：http://qxb.xylfe.cn

echo $((1 + 2 * 3))
来源：http://hwu.snrcjt.cn

[R28] 浮点运算
来源：http://lhq.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://hyu.guannengcc.top

[R29] 定义函数
来源：http://qff.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pkj.jinqigufen.top

[R30] 函数返回状态码
来源：http://ofw.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://uiz.hfpthk.cn

[R31] 局部变量
来源：http://sfm.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://ykn.pengpengdd.cyou

[R32] 参数个数校验
来源：http://lxd.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mlm.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://qne.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zik.zdqjudy.top

[R34] 退出时清理
来源：http://hzs.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://xld.zhijiandao.cn

[R35] 后台执行并等待
来源：http://mxo.meibo888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hfa.hnqzz.top

[R36] 并发执行多个任务
来源：http://ech.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mcu.kuanghao11.cn

[R37] 把输出赋给变量
来源：http://ddu.tarul.cn

files=$(ls -1)
来源：http://heo.52xcode.cn

[R38] 管道串联
来源：http://roz.redwolf501.top

cat a.txt | grep -i error | wc -l
来源：http://wtt.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://goa.sweek.top

cmd > out.log 2>&1
来源：http://nlv.yj20258888.top

[R40] 追加写日志
来源：http://vvo.zhixingplan.top

echo "log" >> out.log
来源：http://gzq.zdqjudy.top

[R41] 丢弃输出
来源：http://vui.fzhhl.top

cmd >/dev/null 2>&1
来源：http://lzr.yj202588.top

[R42] 输入重定向
来源：http://vxo.gzhubu.top

wc -l < a.txt
来源：http://znu.wangdashe.top

[R43] 按名字查找文件
来源：http://qri.nwbrower.top

find . -name "*.log" -type f
来源：http://wwg.svipenyu.cn

[R44] 按修改时间查找
来源：http://zvk.yangfankeji.com

find . -mtime -7 -type f
来源：http://hiy.hnqzz.top

[R45] 批量删除
来源：http://aao.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://olo.xziqi.cn

[R46] 递归替换文件内容
来源：http://tdw.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gys.gzhubu.top

[R47] sed 单行替换
来源：http://apz.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nlq.jinqigfzy.top

[R48] awk 取指定列
来源：http://qga.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://ywb.fehbvm.com

[R49] awk 带条件
来源：http://ptt.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ntq.hysaishi.cn

[R50] awk 求和
来源：http://byu.zhaomingkeji.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://eex.cdnleiting.top

[R51] 排序去重取前几
来源：http://oka.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ctb.cqqwz.cn

[R52] 统计行数
来源：http://dxu.52xcode.cn

wc -l a.txt
来源：http://kzp.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://ibn.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gjy.yangfankeji.com

[R54] 比较两个文件
来源：http://lcb.yj20258888.top

diff a.txt b.txt
来源：http://wzs.zhongyouzk.top

[R55] 压缩与解压
来源：http://aco.iojbl.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xqf.redwolf501.top

[R56] 远程拷贝
来源：http://tkq.aizwys.cn

scp file user@host:/path/
来源：http://gil.yj20258.top

[R57] 远程执行命令
来源：http://ben.ehwqpu.com

ssh user@host 'uptime'
来源：http://zhq.guowangkeji.top

[R58] 下载文件
来源：http://vfx.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mxk.fktsv.cn

[R59] 发 POST JSON
来源：http://twz.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bso.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://yax.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fva.jianghu66.top

[R61] 磁盘占用
来源：http://quf.tanke756.top

df -h;  du -sh *
来源：http://efl.ybcxt.top

[R62] 找最占空间的文件
来源：http://ccl.bjfxy.top

du -ah . | sort -rh | head -10
来源：http://rvm.dashuyun.cn

[R63] 内存与进程
来源：http://qox.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://nfm.316326.xyz

[R64] 结束进程
来源：http://gap.jyoumei.cn

kill -9 $(pgrep -f app.py)
来源：http://nyl.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://fob.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xfr.zdqjudy.top

[R66] 定时任务
来源：http://jpa.yuxming.cn

crontab -e;  crontab -l
来源：http://iaq.hcnkem.com

[R67] 生成随机十六进制串
来源：http://chs.gotoacloud.top

openssl rand -hex 16
来源：http://zbi.yvedp.cn

[R68] 计算文件校验值
来源：http://ikp.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bwx.kuanghao11.cn

[R69] 生成随机密码
来源：http://lwr.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://xob.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://bqy.hcnkem.com

date +%s;  date -d @1700000000
来源：http://olw.cheryme.top

[R71] 日期格式化
来源：http://onl.wangshuangyany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mxh.tarul.cn

[R72] 等待端口就绪
来源：http://ozr.0kj1m.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nmn.cheryme.top

[R73] 分割大日志
来源：http://qou.smart0.xyz

split -l 1000 big.log part_
来源：http://zja.wangdashe.top

[R74] 批量重命名
来源：http://rgi.meibo888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ikv.chenlongwang.top

[R75] 导出环境变量
来源：http://eoi.yfazqb.com

export PATH="$HOME/bin:$PATH"
来源：http://oee.hongshengwenyu.top

[R76] 使用临时文件
来源：http://rgc.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lbp.jqgfzy.top

[R77] 读取用户输入
来源：http://ozq.smart0.xyz

read -rp "请输入: " ans
来源：http://fff.ydzc1.top

[R78] 交互式菜单
来源：http://hok.nwbrower.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uvq.jqgfzy.top

[R79] 解析命令行选项
来源：http://rgb.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eub.cashguo.top

[R80] 查看脚本执行耗时
来源：http://tix.nanxuanxn.top

time ./run.sh
来源：http://pcp.sufxvd.cn

================================================================================
来源：http://vvt.hysaishi.cn

S. C / C++ 专题
来源：http://vuk.daria6918.cn

================================================================================
来源：http://qch.gotoacloud.top

[S01] C：Hello World
来源：http://qxu.cqqwz.cn

#include <stdio.h>
来源：http://gzh.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xvn.meibo888.top

[S02] C：变量与格式化输出
来源：http://smj.tanke756.top

int a = 10; printf("%d\n", a);
来源：http://wit.cashguo.top

[S03] C：读入整数
来源：http://bfz.fzhhl.top

int x; scanf("%d", &x);
来源：http://uwi.birdmap.top

[S04] C：字符串复制
来源：http://lbq.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tsd.kuanghao11.cn

[S05] C：字符串长度
来源：http://wdh.yangfankeji.com

strlen(s)
来源：http://yfc.ydjk.org.cn

[S06] C：字符串比较
来源：http://dra.ydzc1.top

strcmp(a, b) == 0
来源：http://rsm.52xcode.cn

[S07] C：数组遍历求和
来源：http://rvc.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://awo.xuanzx.com

[S08] C：动态内存分配与释放
来源：http://xhl.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xut.yuanzhike.top

[S09] C：结构体定义与初始化
来源：http://wfw.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aqe.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://avm.nanxinkj.top

int *p = &a;  *p = 5;
来源：http://gjh.pycfn.com

[S11] C：逐行读文件
来源：http://muo.redwolf501.top

FILE *f = fopen("a.txt", "r");
来源：http://ktv.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://gni.sweek.top

fclose(f);
来源：http://kpe.zdbjq.cn

[S12] C：写文件
来源：http://nbi.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ffj.9152youxi.cn

[S13] C：宏定义
来源：http://wbw.bjfxy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xbl.cucudq.cn

[S14] C：枚举
来源：http://bjt.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://ejj.jqgufenzy.top

[S15] C：类型转换
来源：http://tmv.andypj.xyz

(double) a / b
来源：http://elm.fzhhl.top

[S16] C：位操作置位
来源：http://tjq.tanke756.top

x |= (1 << 3);
来源：http://bqk.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://jtq.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zcc.yuxming.cn

[S18] C：命令行参数
来源：http://ehd.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://hos.birdmap.top

[S19] C：快速排序
来源：http://mix.guannengcc.top

qsort(a, n, sizeof(int), cmp);
来源：http://wjx.c1oappe.top

[S20] C：二分查找
来源：http://lbh.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://isu.tian-w.cn

[S21] C：字符类别判断
来源：http://iem.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rup.tanke756.top

[S22] C：字符串转数字
来源：http://jko.zhengqikj.top

atoi("42");  strtod("3.14", NULL);
来源：http://zfj.yfazqb.com

[S23] C：随机数
来源：http://xik.cqqwz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pvb.sufxvd.cn

[S24] C：获取本地时间
来源：http://kqg.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://arw.yueranfly.top

[S25] C：内存拷贝
来源：http://poq.zdqjudy.top

memcpy(dst, src, n);
来源：http://dev.tian-w.cn

[S26] C：内存清零
来源：http://yxn.ppjwa.cn

memset(a, 0, sizeof a);
来源：http://stj.fengsongda.top

[S27] C：定义常量
来源：http://yuj.hesvh.cn

const double PI = 3.14159;
来源：http://zuz.aizwys.cn

[S28] C：静态变量
来源：http://cwy.hammf.cn

static int counter = 0;
来源：http://yhk.hnxiangtu.top

[S29] C：变参函数
来源：http://ytv.wangdashe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nzx.bjfxy.top

[S30] C：头文件保护
来源：http://qtw.xuanzx.com

#ifndef X_H
来源：http://ggn.yj20258888.top

#define X_H
来源：http://vhm.yj202588.top

#endif
来源：http://eht.jyoumei.cn

[S31] C++：Hello World
来源：http://hjn.tanke756.top

#include <iostream>
来源：http://dsu.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://vru.ydzc1.top

[S32] C++：字符串
来源：http://spu.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://jyw.hesvh.cn

[S33] C++：vector 增删
来源：http://rqg.tian-w.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tws.hysaishi.cn

[S34] C++：遍历 vector
来源：http://fns.aibaodan.cn

for (auto &x : v) { std::cout << x; }
来源：http://lwy.hysaishi.cn

[S35] C++：map
来源：http://omw.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://epg.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://vei.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vsv.bbcook.cn

[S37] C++：set
来源：http://cbk.jinqigfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jdy.jinqigufen.top

[S38] C++：排序
来源：http://eut.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://dlj.yongpay.top

[S39] C++：自定义比较器排序
来源：http://lpg.zycfv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vzy.sjlbkw.cn

[S40] C++：查找元素
来源：http://gev.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rkf.gogol.net.cn

[S41] C++：类与构造函数
来源：http://nfn.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://onc.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://rol.fanxiaobao.xyz

class B : public Base { public: void f() override {} };
来源：http://yrx.cqqwz.cn

[S43] C++：智能指针
来源：http://zgm.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://dfl.chenjidiqi.icu

[S44] C++：引用传参
来源：http://fpj.fanxiaobao.xyz

void inc(int &x) { ++x; }
来源：http://mqb.vehdjk.com

[S45] C++：lambda
来源：http://hoj.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://upq.meibo888.top

[S46] C++：函数模板
来源：http://bnj.hnxiangtu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kgd.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://wti.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qzg.0kj1m.cn

[S48] C++：逐行读文件
来源：http://bzt.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://gos.bjfxy.top

while (std::getline(in, line)) { }
来源：http://nhm.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://xwj.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fud.jqgfzy.top

[S50] C++：格式化数字
来源：http://wvk.fktsv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://alr.ybcxt.top

[S51] C++：显式类型转换
来源：http://fiz.jqgfzy.top

static_cast<double>(a) / b
来源：http://tzs.andypj.xyz

[S52] C++：const 与 noexcept
来源：http://jsg.fktsv.cn

int size() const noexcept { return n_; }
来源：http://pfd.vqdsnc.cn

[S53] C++：移动语义
来源：http://wze.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://sop.tian-w.cn

[S54] C++：异常处理
来源：http://jik.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pbx.aizwys.cn

[S55] C++：结构化绑定
来源：http://tru.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ybk.ywan-chungtsiang.top

[S56] C++：optional
来源：http://chi.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lqd.zhengqikj.top

[S57] C++：编译期常量
来源：http://ixo.kuanghao11.cn

constexpr int N = 10;
来源：http://rci.tianlin.xyz

[S58] C++：命名空间
来源：http://bnu.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://caw.yangfankeji.com

[S59] C++：静态断言
来源：http://epd.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tvo.ydjk.org.cn

[S60] C++：遍历并删除元素
来源：http://xdn.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ujn.chenlongwang.top

================================================================================
来源：http://hds.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://brx.cheryme.top

================================================================================
来源：http://dcn.ppjwa.cn

[T01] Kotlin：Hello World
来源：http://jvr.svipenyu.cn

println("Hello")
来源：http://kee.andypj.xyz

[T02] Kotlin：变量
来源：http://ogs.svipenyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uri.cashguo.top

[T03] Kotlin：字符串模板
来源：http://jpk.aizwys.cn

"值: $b"
来源：http://mru.guowangkeji.top

[T04] Kotlin：空安全
来源：http://qeg.zhongyouzk.top

val n: String? = null;  n?.length
来源：http://bcg.yj20258888.top

[T05] Kotlin：when 表达式
来源：http://ots.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uco.hnqzz.top

[T06] Kotlin：集合映射
来源：http://mqz.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pbk.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://ehv.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ztf.daria6918.cn

[T08] Kotlin：数据类
来源：http://twq.fzhhl.top

data class User(val name: String, val age: Int)
来源：http://rmq.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://wyd.cdnleiting.top

fun String.exclaim() = this + "!"
来源：http://rbi.zhijiandao.cn

[T10] Kotlin：默认参数
来源：http://yfy.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rex.zycfv.cn

[T11] Kotlin：协程
来源：http://obq.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://imu.zdbjq.cn

[T12] Kotlin：解构声明
来源：http://own.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://wqd.xuanzx.com

[T13] Kotlin：只读 Map
来源：http://bnj.52xcode.cn

val m = mapOf("a" to 1)
来源：http://bhp.ywan-chungtsiang.top

[T14] Kotlin：循环
来源：http://ovv.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://nql.vqdsnc.cn

[T15] Kotlin：接口
来源：http://bty.snrcjt.cn

interface Shape { fun area(): Double }
来源：http://wft.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://adh.cdnleiting.top

print("Hello")
来源：http://ubq.zhiwuduotai.top

[T17] Swift：变量与常量
来源：http://zzb.shzxlz.cn

var a = 1;  let b = 2
来源：http://kme.jqgufenzy.top

[T18] Swift：字符串插值
来源：http://oxk.quarkkingdee.top

"值: \(b)"
来源：http://ibx.zhaomingkeji.xyz

[T19] Swift：可选绑定
来源：http://cyp.quarkkingdee.top

if let n = opt { print(n) }
来源：http://iej.vqdsnc.cn

[T20] Swift：数组操作
来源：http://oth.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://zer.yfazqb.com

[T21] Swift：遍历
来源：http://twn.wangshuangyany.cn

for x in a { print(x) }
来源：http://ujg.52xcode.cn

[T22] Swift：字典
来源：http://vcd.jianghu66.top

var d = ["a": 1];  d["b"] = 2
来源：http://ksg.sysykeji.top

[T23] Swift：函数
来源：http://bui.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yem.shzxlz.cn

[T24] Swift：闭包
来源：http://ssf.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gsa.sxryk.cn


<!-- 参考信息 -->