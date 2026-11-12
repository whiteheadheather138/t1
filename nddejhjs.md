代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://odg.fanxiaobao.xyz

[R24] 大小写转换
来源：http://rds.sweek.top

echo "${s^^}"; echo "${s,,}"
来源：http://fim.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://ock.jinqigufen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://quv.ydjk.org.cn

[R26] 命令替换
来源：http://frr.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://xsw.cheryme.top

[R27] 算术展开
来源：http://idu.yongpay.top

echo $((1 + 2 * 3))
来源：http://lhg.vqdsnc.cn

[R28] 浮点运算
来源：http://nwx.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://hky.sysykeji.top

[R29] 定义函数
来源：http://lau.cdnleiting.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fye.zycfv.cn

[R30] 函数返回状态码
来源：http://lsi.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://nap.yongpay.top

[R31] 局部变量
来源：http://ywl.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://cmz.zdqjudy.top

[R32] 参数个数校验
来源：http://dfl.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://deo.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://rrr.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://opz.nanxinkj.top

[R34] 退出时清理
来源：http://lfw.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vqz.nanxuanxn.top

[R35] 后台执行并等待
来源：http://ywc.jqgfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://syp.xinyue.icu

[R36] 并发执行多个任务
来源：http://dos.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jsn.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://hdx.ydjk.org.cn

files=$(ls -1)
来源：http://qcd.sysykeji.top

[R38] 管道串联
来源：http://jhq.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://rue.jqgfzy.top

[R39] 重定向标准输出与错误
来源：http://wjp.smart0.xyz

cmd > out.log 2>&1
来源：http://unr.cqqwz.cn

[R40] 追加写日志
来源：http://fzr.cucudq.cn

echo "log" >> out.log
来源：http://woi.jqgufenzy.top

[R41] 丢弃输出
来源：http://hbs.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://vfr.ydjk.org.cn

[R42] 输入重定向
来源：http://pkb.hnxiangtu.top

wc -l < a.txt
来源：http://pmf.xuanzx.com

[R43] 按名字查找文件
来源：http://foi.meibo888.top

find . -name "*.log" -type f
来源：http://adf.tanke756.top

[R44] 按修改时间查找
来源：http://jdw.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://fdz.jinghuilouyu.cn

[R45] 批量删除
来源：http://luf.yueranfly.top

find . -name "*.tmp" -delete
来源：http://khn.ctjpmb.com

[R46] 递归替换文件内容
来源：http://ecu.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xoc.ybcxt.top

[R47] sed 单行替换
来源：http://pxm.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://phh.ybcxt.top

[R48] awk 取指定列
来源：http://dnq.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://ozt.fengsongda.top

[R49] awk 带条件
来源：http://toh.shanyushiyangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hsb.jinghuilouyu.cn

[R50] awk 求和
来源：http://yos.yfazqb.com

awk '{s += $2} END {print s}' a.txt
来源：http://zpw.nwbrower.top

[R51] 排序去重取前几
来源：http://rus.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kum.zhongyouzk.top

[R52] 统计行数
来源：http://mfu.feifeiyinyue.top

wc -l a.txt
来源：http://jqv.gzhubu.top

[R53] 查看文件头与实时尾
来源：http://sdo.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dxs.guannengcc.top

[R54] 比较两个文件
来源：http://lku.haohaochexian.top

diff a.txt b.txt
来源：http://xwr.dianchejie.cn

[R55] 压缩与解压
来源：http://wud.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://azy.daxiang520.top

[R56] 远程拷贝
来源：http://pqz.hcnkem.com

scp file user@host:/path/
来源：http://lhf.cheryme.top

[R57] 远程执行命令
来源：http://wdp.iojbl.cn

ssh user@host 'uptime'
来源：http://pkq.gotoacloud.top

[R58] 下载文件
来源：http://gwi.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pnh.zhijiandao.cn

[R59] 发 POST JSON
来源：http://tnm.sweek.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dfd.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://oka.shanyushiyangtech.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xbw.jyoumei.cn

[R61] 磁盘占用
来源：http://tsf.mhx1999.top

df -h;  du -sh *
来源：http://kwz.mhx1999.top

[R62] 找最占空间的文件
来源：http://emb.chenzaomai.com

du -ah . | sort -rh | head -10
来源：http://hla.yfazqb.com

[R63] 内存与进程
来源：http://rgb.ehwqpu.com

free -h;  ps aux | grep nginx
来源：http://uup.ybcxt.top

[R64] 结束进程
来源：http://lad.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://moa.yangfankeji.com

[R65] 查看端口占用
来源：http://akn.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wcp.ivvv.top

[R66] 定时任务
来源：http://tjw.jqgufenzy.top

crontab -e;  crontab -l
来源：http://mag.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://mbw.uphjek.com

openssl rand -hex 16
来源：http://tne.yvedp.cn

[R68] 计算文件校验值
来源：http://ids.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://vzl.svipenyu.cn

[R69] 生成随机密码
来源：http://tgi.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://zjv.jianghu66.top

[R70] 时间戳与互转
来源：http://zhh.daria6918.cn

date +%s;  date -d @1700000000
来源：http://toc.hcnkem.com

[R71] 日期格式化
来源：http://hfe.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://giz.gotoacloud.top

[R72] 等待端口就绪
来源：http://mua.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://huo.kuanghao11.cn

[R73] 分割大日志
来源：http://gtn.vqdsnc.cn

split -l 1000 big.log part_
来源：http://arh.yuanzhike.top

[R74] 批量重命名
来源：http://ioe.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pgw.ctjpmb.com

[R75] 导出环境变量
来源：http://kbv.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://aba.yj20258888.top

[R76] 使用临时文件
来源：http://zny.yanxiufei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xat.yvedp.cn

[R77] 读取用户输入
来源：http://mxu.ybcxt.top

read -rp "请输入: " ans
来源：http://est.chenlongwang.top

[R78] 交互式菜单
来源：http://dtw.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://adw.fzhhl.top

[R79] 解析命令行选项
来源：http://jqx.zdqjudy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tvw.birdmap.top

[R80] 查看脚本执行耗时
来源：http://mns.tarul.cn

time ./run.sh
来源：http://wzd.hywenlv.cn

================================================================================
来源：http://iav.snrcjt.cn

S. C / C++ 专题
来源：http://wjz.meibo888.top

================================================================================
来源：http://dow.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://noe.sxryk.cn

#include <stdio.h>
来源：http://ojp.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://irr.aizwys.cn

[S02] C：变量与格式化输出
来源：http://aze.52xcode.cn

int a = 10; printf("%d\n", a);
来源：http://foq.tian-w.cn

[S03] C：读入整数
来源：http://stc.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://dvj.xinyue.icu

[S04] C：字符串复制
来源：http://uci.ywan-chungtsiang.top

char dst[32]; strcpy(dst, "hi");
来源：http://vvb.sweek.top

[S05] C：字符串长度
来源：http://jkx.mhx1999.top

strlen(s)
来源：http://doc.kuanghao11.cn

[S06] C：字符串比较
来源：http://vdp.cashguo.top

strcmp(a, b) == 0
来源：http://wzu.52xcode.cn

[S07] C：数组遍历求和
来源：http://yme.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kly.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://kzf.shzxlz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lgh.cdnleiting.top

[S09] C：结构体定义与初始化
来源：http://iym.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://swg.chenzaomai.com

[S10] C：指针与解引用
来源：http://kfa.tian-w.cn

int *p = &a;  *p = 5;
来源：http://gkv.zycfv.cn

[S11] C：逐行读文件
来源：http://hft.meibo888.top

FILE *f = fopen("a.txt", "r");
来源：http://uwp.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zmw.yueranfly.top

fclose(f);
来源：http://smt.wangshuangyany.cn

[S12] C：写文件
来源：http://fol.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hbj.yongpay.top

[S13] C：宏定义
来源：http://wlq.nanxinkj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tno.cdnleiting.top

[S14] C：枚举
来源：http://ory.zhixingplan.top

enum Color { RED, GREEN, BLUE };
来源：http://lde.chenzaomai.com

[S15] C：类型转换
来源：http://vyt.jqgufenzy.top

(double) a / b
来源：http://yfc.yueranfly.top

[S16] C：位操作置位
来源：http://hso.tanke756.top

x |= (1 << 3);
来源：http://uei.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://sbs.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xee.ehwqpu.com

[S18] C：命令行参数
来源：http://txw.fehbvm.com

int main(int argc, char **argv)
来源：http://byn.gotoacloud.top

[S19] C：快速排序
来源：http://int.yj20258888.top

qsort(a, n, sizeof(int), cmp);
来源：http://vtg.vehdjk.com

[S20] C：二分查找
来源：http://cwb.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://txe.yfazqb.com

[S21] C：字符类别判断
来源：http://fgf.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rer.jyoumei.cn

[S22] C：字符串转数字
来源：http://kye.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://njc.jqgufenzy.top

[S23] C：随机数
来源：http://kfh.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lkh.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://kiz.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qee.zhongyouzk.top

[S25] C：内存拷贝
来源：http://oxp.316326.xyz

memcpy(dst, src, n);
来源：http://jaz.tanke756.top

[S26] C：内存清零
来源：http://wcw.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://xts.jyoumei.cn

[S27] C：定义常量
来源：http://tgh.yj20258.top

const double PI = 3.14159;
来源：http://zuj.jiagoushi.top

[S28] C：静态变量
来源：http://nqm.hesvh.cn

static int counter = 0;
来源：http://qik.redwolf501.top

[S29] C：变参函数
来源：http://wtz.shzxlz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cly.redwolf501.top

[S30] C：头文件保护
来源：http://owo.yvedp.cn

#ifndef X_H
来源：http://aaf.fanxiaobao.xyz

#define X_H
来源：http://svw.fzhhl.top

#endif
来源：http://fze.bjfxy.top

[S31] C++：Hello World
来源：http://nmq.jqgfzy.top

#include <iostream>
来源：http://pwg.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://nri.vqdsnc.cn

[S32] C++：字符串
来源：http://cce.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://ljq.wangdashe.top

[S33] C++：vector 增删
来源：http://lsu.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lcv.cheryme.top

[S34] C++：遍历 vector
来源：http://egm.fanxiaobao.xyz

for (auto &x : v) { std::cout << x; }
来源：http://eul.shanyushiyangkeji.top

[S35] C++：map
来源：http://tnd.uphjek.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gos.yongpay.top

[S36] C++：unordered_map
来源：http://nhd.ctjpmb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bdi.yj202588.top

[S37] C++：set
来源：http://xmg.yvedp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ixt.tianlin.xyz

[S38] C++：排序
来源：http://jjs.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://cmr.hammf.cn

[S39] C++：自定义比较器排序
来源：http://ltm.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://flh.0kj1m.cn

[S40] C++：查找元素
来源：http://baf.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xyw.xylfe.cn

[S41] C++：类与构造函数
来源：http://yve.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fay.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://ryp.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://cfo.c1oappe.top

[S43] C++：智能指针
来源：http://esu.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://nqd.ctjpmb.com

[S44] C++：引用传参
来源：http://zvq.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://vbx.xuetiantiany.cn

[S45] C++：lambda
来源：http://zpi.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://chw.yongpay.top

[S46] C++：函数模板
来源：http://djq.guannengcc.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zkp.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://xot.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zej.smart0.xyz

[S48] C++：逐行读文件
来源：http://wco.nwbrower.top

std::ifstream in("a.txt");  std::string line;
来源：http://apg.hammf.cn

while (std::getline(in, line)) { }
来源：http://bok.316326.xyz

[S49] C++：写文件
来源：http://yqo.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fkl.52xcode.cn

[S50] C++：格式化数字
来源：http://dzg.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vji.birdmap.top

[S51] C++：显式类型转换
来源：http://zkq.c1oappe.top

static_cast<double>(a) / b
来源：http://dcx.daria6918.cn

[S52] C++：const 与 noexcept
来源：http://wwz.epnwcf.com

int size() const noexcept { return n_; }
来源：http://ngk.zhengqikj.top

[S53] C++：移动语义
来源：http://ttn.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://kbd.yuanzhike.top

[S54] C++：异常处理
来源：http://ffa.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rbw.cheryme.top

[S55] C++：结构化绑定
来源：http://svl.tarul.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://urc.cdnleiting.top

[S56] C++：optional
来源：http://apy.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://euj.gzhubu.top

[S57] C++：编译期常量
来源：http://cfl.sufxvd.cn

constexpr int N = 10;
来源：http://riz.ehwqpu.com

[S58] C++：命名空间
来源：http://elh.jinqigufen.top

namespace ns { int f() { return 1; } }
来源：http://xjz.snrcjt.cn

[S59] C++：静态断言
来源：http://amm.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vdw.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://vco.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tfb.dianchejie.cn

================================================================================
来源：http://zvm.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://utp.guowangkeji.top

================================================================================
来源：http://lyj.iojbl.cn

[T01] Kotlin：Hello World
来源：http://vav.sysykeji.top

println("Hello")
来源：http://vjv.kuanghao11.cn

[T02] Kotlin：变量
来源：http://dib.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kkk.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://gmq.hammf.cn

"值: $b"
来源：http://fcc.xinyue.icu

[T04] Kotlin：空安全
来源：http://rvj.hfpthk.cn

val n: String? = null;  n?.length
来源：http://hqy.gzhubu.top

[T05] Kotlin：when 表达式
来源：http://jyv.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vib.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://gpn.gaohongyu789.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cdn.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://xgj.jiagoushi.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://adl.jqgfzy.top

[T08] Kotlin：数据类
来源：http://aun.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://lep.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://hkr.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://sgk.cucudq.cn

[T10] Kotlin：默认参数
来源：http://gob.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rob.wangdashe.top

[T11] Kotlin：协程
来源：http://haq.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://dyo.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://wwf.wangshuangyany.cn

val (a, b) = Pair(1, 2)
来源：http://iii.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://rvk.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://plh.hywenlv.cn

[T14] Kotlin：循环
来源：http://dak.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://hok.yvedp.cn

[T15] Kotlin：接口
来源：http://elz.zhaomingkeji.xyz

interface Shape { fun area(): Double }
来源：http://tym.fktsv.cn

[T16] Swift：Hello World
来源：http://ipu.sweek.top

print("Hello")
来源：http://ufa.guowangkeji.top

[T17] Swift：变量与常量
来源：http://ixr.ctjpmb.com

var a = 1;  let b = 2
来源：http://vxj.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://uuq.smart0.xyz

"值: \(b)"
来源：http://pgz.jianghu66.top

[T19] Swift：可选绑定
来源：http://qap.zdbjq.cn

if let n = opt { print(n) }
来源：http://obc.cdnleiting.top

[T20] Swift：数组操作
来源：http://ljl.bjfxy.top

var a = [1, 2, 3];  a.append(4)
来源：http://ktj.tian-w.cn

[T21] Swift：遍历
来源：http://svt.tian-w.cn

for x in a { print(x) }
来源：http://vtf.ydzc1.top

[T22] Swift：字典
来源：http://ixn.sjlbkw.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qbx.gotoacloud.top

[T23] Swift：函数
来源：http://shm.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://okz.hnxiangtu.top

[T24] Swift：闭包
来源：http://ole.zhongyouzk.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wle.ctjpmb.com

[T25] Swift：结构体
来源：http://zab.nanxinkj.top

struct P { var x: Int }
来源：http://buy.xuetiantiany.cn

[T26] Swift：类与重写
来源：http://vcq.ybcxt.top

class A: Base { override func f() {} }
来源：http://mkc.tanke756.top


<!-- 参考信息 -->