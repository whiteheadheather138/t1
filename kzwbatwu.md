代发 wailian999

echo "${#arr[@]}"
来源：http://wmh.hnxiangtu.top

[R20] 关联数组（字典）
来源：http://afq.yj20258.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qiv.dashuyun.cn

[R21] 字符串长度
来源：http://zvt.xingfuxueyuan.xyz

echo "${#s}"
来源：http://pou.jlsjyb.cn

[R22] 截取子串
来源：http://gwg.yj202588.top

echo "${s:0:5}"
来源：http://vjv.cashguo.top

[R23] 字符串替换
来源：http://mdu.c1oappe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ntu.ybcxt.top

[R24] 大小写转换
来源：http://azj.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://osw.smart0.xyz

[R25] 去后缀 / 去前缀
来源：http://lsv.zdqjudy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ctc.zhoulong.xyz

[R26] 命令替换
来源：http://clt.316326.xyz

now=$(date +%F); echo "$now"
来源：http://wob.bbcook.cn

[R27] 算术展开
来源：http://lyw.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://uvz.ppjwa.cn

[R28] 浮点运算
来源：http://ijf.fehbvm.com

echo "scale=2; 10/3" | bc
来源：http://quz.xingfuxueyuan.xyz

[R29] 定义函数
来源：http://qfm.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sso.xuanzx.com

[R30] 函数返回状态码
来源：http://fqw.cqqwz.cn

f() { return 0; }; f || echo "失败了"
来源：http://wjd.zhixingplan.top

[R31] 局部变量
来源：http://vdv.shuidangran.top

f() { local x=1; echo "$x"; }
来源：http://sna.zhengqikj.top

[R32] 参数个数校验
来源：http://esf.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://soy.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://dxc.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://thy.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://uix.zhiwuduotai.top

trap 'rm -f "$tmp"' EXIT
来源：http://ijj.hongshengwenyu.top

[R35] 后台执行并等待
来源：http://dfp.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ued.ivvv.top

[R36] 并发执行多个任务
来源：http://mwu.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kby.ehwqpu.com

[R37] 把输出赋给变量
来源：http://dsa.fehbvm.com

files=$(ls -1)
来源：http://ffd.jinghuilouyu.cn

[R38] 管道串联
来源：http://ioe.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://ase.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://vcg.fktsv.cn

cmd > out.log 2>&1
来源：http://cwb.tarul.cn

[R40] 追加写日志
来源：http://dht.yuanzhike.top

echo "log" >> out.log
来源：http://zeh.0kj1m.cn

[R41] 丢弃输出
来源：http://wfr.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://sno.uphjek.com

[R42] 输入重定向
来源：http://wvu.jinyuanbaomall.cn

wc -l < a.txt
来源：http://qwo.gotoacloud.top

[R43] 按名字查找文件
来源：http://kvk.yonumen.top

find . -name "*.log" -type f
来源：http://dcs.ivvv.top

[R44] 按修改时间查找
来源：http://gnm.aibaodan.cn

find . -mtime -7 -type f
来源：http://gjw.ywan-chungtsiang.top

[R45] 批量删除
来源：http://eyo.xylfe.cn

find . -name "*.tmp" -delete
来源：http://pzw.yvedp.cn

[R46] 递归替换文件内容
来源：http://wxb.jiagoushi.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dtx.yueranfly.top

[R47] sed 单行替换
来源：http://ihj.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oqh.c1oappe.top

[R48] awk 取指定列
来源：http://qyl.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://gwd.andypj.xyz

[R49] awk 带条件
来源：http://mro.chenlongwang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uoa.havefunace.top

[R50] awk 求和
来源：http://jec.nwbrower.top

awk '{s += $2} END {print s}' a.txt
来源：http://hac.yuxming.cn

[R51] 排序去重取前几
来源：http://mbh.xziqi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bko.shanyushiyangkeji.top

[R52] 统计行数
来源：http://gru.yanxiufei.cn

wc -l a.txt
来源：http://yin.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://tyl.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jne.yonumen.top

[R54] 比较两个文件
来源：http://hjl.zhoulong.xyz

diff a.txt b.txt
来源：http://bmb.wangdashe.top

[R55] 压缩与解压
来源：http://jph.hammf.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dww.hysaishi.cn

[R56] 远程拷贝
来源：http://yiv.svipenyu.cn

scp file user@host:/path/
来源：http://dhg.cheryme.top

[R57] 远程执行命令
来源：http://nwj.shanyushiyangtech.top

ssh user@host 'uptime'
来源：http://pfw.svipenyu.cn

[R58] 下载文件
来源：http://vhr.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kzl.bbcook.cn

[R59] 发 POST JSON
来源：http://xxv.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hao.c1oappe.top

[R60] 只看 HTTP 状态码
来源：http://urn.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jqp.sjlbkw.cn

[R61] 磁盘占用
来源：http://bid.yj20258888.top

df -h;  du -sh *
来源：http://mek.gzhubu.top

[R62] 找最占空间的文件
来源：http://rop.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://tdb.ivvv.top

[R63] 内存与进程
来源：http://wda.yuanzhike.top

free -h;  ps aux | grep nginx
来源：http://pxh.ydzc1.top

[R64] 结束进程
来源：http://pfm.52xcode.cn

kill -9 $(pgrep -f app.py)
来源：http://ogn.jyoumei.cn

[R65] 查看端口占用
来源：http://jhw.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nqz.shuidangran.top

[R66] 定时任务
来源：http://nfy.shanyushiyangtech.top

crontab -e;  crontab -l
来源：http://eok.xuetiantiany.cn

[R67] 生成随机十六进制串
来源：http://uce.yfazqb.com

openssl rand -hex 16
来源：http://ysu.gogol.net.cn

[R68] 计算文件校验值
来源：http://qfg.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://hhe.zdqjudy.top

[R69] 生成随机密码
来源：http://nig.yonumen.top

head -c 16 /dev/urandom | base64
来源：http://csg.zhongyouzk.top

[R70] 时间戳与互转
来源：http://zzd.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://koq.zhaomingkeji.xyz

[R71] 日期格式化
来源：http://rof.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ejg.tianlin.xyz

[R72] 等待端口就绪
来源：http://owh.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nuu.jqgfzy.top

[R73] 分割大日志
来源：http://foc.sjlbkw.cn

split -l 1000 big.log part_
来源：http://nkt.zdqjudy.top

[R74] 批量重命名
来源：http://qtp.chenlongwang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kiy.aibaodan.cn

[R75] 导出环境变量
来源：http://him.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://puq.gaohongyu789.top

[R76] 使用临时文件
来源：http://zjo.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://crr.nwbrower.top

[R77] 读取用户输入
来源：http://aso.dashuyun.cn

read -rp "请输入: " ans
来源：http://dwk.jinqigfzy.top

[R78] 交互式菜单
来源：http://qlo.zhongyouzk.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hhj.shzxlz.cn

[R79] 解析命令行选项
来源：http://ncm.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vty.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://qwr.xuanzx.com

time ./run.sh
来源：http://njl.xuetiantiany.cn

================================================================================
来源：http://tzb.iojbl.cn

S. C / C++ 专题
来源：http://zgc.c1oappe.top

================================================================================
来源：http://mme.fanxiaobao.xyz

[S01] C：Hello World
来源：http://cqs.hywenlv.cn

#include <stdio.h>
来源：http://smi.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vby.yj20258.top

[S02] C：变量与格式化输出
来源：http://ueo.9152youxi.cn

int a = 10; printf("%d\n", a);
来源：http://fzz.jinqigfzy.top

[S03] C：读入整数
来源：http://ecu.aizwys.cn

int x; scanf("%d", &x);
来源：http://jau.xinyue.icu

[S04] C：字符串复制
来源：http://ohw.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://ckj.nanxuanxn.top

[S05] C：字符串长度
来源：http://jvk.tarul.cn

strlen(s)
来源：http://ovq.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://gag.yanxiufei.cn

strcmp(a, b) == 0
来源：http://oqj.zycfv.cn

[S07] C：数组遍历求和
来源：http://qaz.bjfxy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://abm.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://ljr.mhx1999.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hkn.gaohongyu789.top

[S09] C：结构体定义与初始化
来源：http://rnb.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tbq.yangfankeji.com

[S10] C：指针与解引用
来源：http://pql.zycfv.cn

int *p = &a;  *p = 5;
来源：http://aag.gogol.net.cn

[S11] C：逐行读文件
来源：http://uzj.shuidangran.top

FILE *f = fopen("a.txt", "r");
来源：http://ewq.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dhi.vehdjk.com

fclose(f);
来源：http://nxu.haohaochexian.top

[S12] C：写文件
来源：http://fpw.cdnleiting.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lny.yj20258888.top

[S13] C：宏定义
来源：http://orv.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hny.yj20258888.top

[S14] C：枚举
来源：http://gis.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://uxy.zhiwuduotai.top

[S15] C：类型转换
来源：http://ova.uphjek.com

(double) a / b
来源：http://tkw.daxiang520.top

[S16] C：位操作置位
来源：http://nla.shuidangran.top

x |= (1 << 3);
来源：http://jsd.xinyue.icu

[S17] C：安全拼接字符串
来源：http://fik.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gie.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://gcm.cucudq.cn

int main(int argc, char **argv)
来源：http://kpl.hongshengwenyu.top

[S19] C：快速排序
来源：http://eqp.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jay.shangyingyoupin.top

[S20] C：二分查找
来源：http://fxz.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oef.gaohongyu789.top

[S21] C：字符类别判断
来源：http://pjk.wangdashe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://plc.bbcook.cn

[S22] C：字符串转数字
来源：http://oar.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://twp.dashuyun.cn

[S23] C：随机数
来源：http://qyi.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://umw.fzhhl.top

[S24] C：获取本地时间
来源：http://rqp.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eaj.fehbvm.com

[S25] C：内存拷贝
来源：http://ukc.zhoulong.xyz

memcpy(dst, src, n);
来源：http://gee.ydjk.org.cn

[S26] C：内存清零
来源：http://pmy.yonumen.top

memset(a, 0, sizeof a);
来源：http://ame.jianghu66.top

[S27] C：定义常量
来源：http://uep.svipenyu.cn

const double PI = 3.14159;
来源：http://drv.hnqzz.top

[S28] C：静态变量
来源：http://jmb.jianghu66.top

static int counter = 0;
来源：http://pzp.bjfxy.top

[S29] C：变参函数
来源：http://emk.chenjidiqi.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yzl.jlsjyb.cn

[S30] C：头文件保护
来源：http://xgw.hcnkem.com

#ifndef X_H
来源：http://pms.316326.xyz

#define X_H
来源：http://rga.ydjk.org.cn

#endif
来源：http://fpd.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://inb.dianchejie.cn

#include <iostream>
来源：http://hta.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://avg.cdnleiting.top

[S32] C++：字符串
来源：http://owe.yongpay.top

std::string s = "hi";  s += "!";
来源：http://ttb.meibo888.top

[S33] C++：vector 增删
来源：http://nis.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hvg.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://wpr.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://xaf.zdqjudy.top

[S35] C++：map
来源：http://spf.yueranfly.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eud.zhoulong.xyz

[S36] C++：unordered_map
来源：http://acu.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ndc.ydzc1.top

[S37] C++：set
来源：http://pom.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xgv.jinqigfzy.top

[S38] C++：排序
来源：http://gtz.hesvh.cn

std::sort(v.begin(), v.end());
来源：http://ghp.nwbrower.top

[S39] C++：自定义比较器排序
来源：http://wdj.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kib.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://asd.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kbi.yj20258.top

[S41] C++：类与构造函数
来源：http://wbh.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xjj.svipenyu.cn

[S42] C++：继承与虚函数
来源：http://bvg.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://ebf.sufxvd.cn

[S43] C++：智能指针
来源：http://ptq.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://wyj.yvedp.cn

[S44] C++：引用传参
来源：http://kqk.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://hfg.sysykeji.top

[S45] C++：lambda
来源：http://pda.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gmu.gaohongyu789.top

[S46] C++：函数模板
来源：http://wdn.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://egg.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://wdw.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uce.ybcxt.top

[S48] C++：逐行读文件
来源：http://mkl.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zko.bjfxy.top

while (std::getline(in, line)) { }
来源：http://tcq.ydzc1.top

[S49] C++：写文件
来源：http://jri.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://atn.ivvv.top

[S50] C++：格式化数字
来源：http://rjm.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zhu.zdbjq.cn

[S51] C++：显式类型转换
来源：http://jwb.shzxlz.cn

static_cast<double>(a) / b
来源：http://mll.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://oxf.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://crg.hnxiangtu.top

[S53] C++：移动语义
来源：http://htv.hcnkem.com

std::vector<int> w = std::move(v);
来源：http://lyr.shzxlz.cn

[S54] C++：异常处理
来源：http://dgu.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rjy.cheryme.top

[S55] C++：结构化绑定
来源：http://ctv.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://chu.jinqigfzy.top

[S56] C++：optional
来源：http://ecu.hywenlv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://khf.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://ogp.hammf.cn

constexpr int N = 10;
来源：http://cmc.quarkkingdee.top

[S58] C++：命名空间
来源：http://wmy.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://zai.fehbvm.com

[S59] C++：静态断言
来源：http://mqd.haohaochexian.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lbr.316326.xyz

[S60] C++：遍历并删除元素
来源：http://oyn.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ctf.cdnleiting.top

================================================================================
来源：http://hji.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hwu.meibo888.top

================================================================================
来源：http://dep.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://eif.uphjek.com

println("Hello")
来源：http://htj.ybcxt.top

[T02] Kotlin：变量
来源：http://lkg.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://usz.hywenlv.cn

[T03] Kotlin：字符串模板
来源：http://dzl.shuidangran.top

"值: $b"
来源：http://fgm.gotoacloud.top

[T04] Kotlin：空安全
来源：http://uhm.bbcook.cn

val n: String? = null;  n?.length
来源：http://dbv.gaohongyu789.top

[T05] Kotlin：when 表达式
来源：http://dbg.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zub.c1oappe.top

[T06] Kotlin：集合映射
来源：http://tsy.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://xxz.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://qji.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hmf.gogol.net.cn

[T08] Kotlin：数据类
来源：http://vaj.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://xcx.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://thh.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://ucj.yonumen.top

[T10] Kotlin：默认参数
来源：http://eei.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hzs.hfpthk.cn

[T11] Kotlin：协程
来源：http://keb.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yic.xuanzx.com

[T12] Kotlin：解构声明
来源：http://frq.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://lpn.jinqigufen.top

[T13] Kotlin：只读 Map
来源：http://czp.316326.xyz

val m = mapOf("a" to 1)
来源：http://zfb.jyoumei.cn

[T14] Kotlin：循环
来源：http://var.jinqigfzy.top

for (i in 1..10) println(i)
来源：http://njz.sxryk.cn

[T15] Kotlin：接口
来源：http://oco.zhaomingkeji.xyz

interface Shape { fun area(): Double }
来源：http://ncw.pycfn.com

[T16] Swift：Hello World
来源：http://imu.redwolf501.top

print("Hello")
来源：http://fes.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://zuv.sxryk.cn

var a = 1;  let b = 2
来源：http://qxm.tianlin.xyz

[T18] Swift：字符串插值
来源：http://huf.cheryme.top

"值: \(b)"
来源：http://vcs.fengsongda.top

[T19] Swift：可选绑定
来源：http://dgd.shzxlz.cn

if let n = opt { print(n) }
来源：http://nts.feifeiyinyue.top

[T20] Swift：数组操作
来源：http://ofl.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://njm.316326.xyz

[T21] Swift：遍历
来源：http://dhw.yj202588.top

for x in a { print(x) }
来源：http://evi.9152youxi.cn

[T22] Swift：字典
来源：http://mte.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rcn.0kj1m.cn


<!-- 参考信息 -->