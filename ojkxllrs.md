代发 wailian999

echo "${#arr[@]}"
来源：http://xrw.gaohongyu789.top

[R20] 关联数组（字典）
来源：http://nzk.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rkn.svipenyu.cn

[R21] 字符串长度
来源：http://buj.fzhhl.top

echo "${#s}"
来源：http://ike.daxiang520.top

[R22] 截取子串
来源：http://dtd.hammf.cn

echo "${s:0:5}"
来源：http://tfw.fengsongda.top

[R23] 字符串替换
来源：http://yyt.yj202588.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dxa.zhiwuduotai.top

[R24] 大小写转换
来源：http://lbi.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mcu.c1oappe.top

[R25] 去后缀 / 去前缀
来源：http://vqq.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dfi.chenzaomai.com

[R26] 命令替换
来源：http://vxj.aibaodan.cn

now=$(date +%F); echo "$now"
来源：http://klx.pycfn.com

[R27] 算术展开
来源：http://spd.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://wkb.hywenlv.cn

[R28] 浮点运算
来源：http://ppg.zhaomingkeji.xyz

echo "scale=2; 10/3" | bc
来源：http://vlr.iojbl.cn

[R29] 定义函数
来源：http://gbd.zhengqikj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qpi.zhengqikj.top

[R30] 函数返回状态码
来源：http://obf.fanxiaobao.xyz

f() { return 0; }; f || echo "失败了"
来源：http://glx.yanxiufei.cn

[R31] 局部变量
来源：http://rso.iojbl.cn

f() { local x=1; echo "$x"; }
来源：http://bgv.zhijiandao.cn

[R32] 参数个数校验
来源：http://aft.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mek.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://oum.ehwqpu.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jsb.epnwcf.com

[R34] 退出时清理
来源：http://axc.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://ebq.hysaishi.cn

[R35] 后台执行并等待
来源：http://sbd.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hti.daxiang520.top

[R36] 并发执行多个任务
来源：http://hkw.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mem.ctjpmb.com

[R37] 把输出赋给变量
来源：http://yfi.aibaodan.cn

files=$(ls -1)
来源：http://ekb.gotoacloud.top

[R38] 管道串联
来源：http://sld.sufxvd.cn

cat a.txt | grep -i error | wc -l
来源：http://hrn.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://prc.nwbrower.top

cmd > out.log 2>&1
来源：http://rro.hcnkem.com

[R40] 追加写日志
来源：http://ghk.ppjwa.cn

echo "log" >> out.log
来源：http://tmj.sufxvd.cn

[R41] 丢弃输出
来源：http://cag.sysykeji.top

cmd >/dev/null 2>&1
来源：http://ord.jyoumei.cn

[R42] 输入重定向
来源：http://ful.xuanzx.com

wc -l < a.txt
来源：http://cic.yfazqb.com

[R43] 按名字查找文件
来源：http://hlk.cheryme.top

find . -name "*.log" -type f
来源：http://qef.cashguo.top

[R44] 按修改时间查找
来源：http://naj.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://oah.xylfe.cn

[R45] 批量删除
来源：http://awt.ehwqpu.com

find . -name "*.tmp" -delete
来源：http://jsg.52xcode.cn

[R46] 递归替换文件内容
来源：http://igl.sjlbkw.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kiz.c1oappe.top

[R47] sed 单行替换
来源：http://los.zhaomingkeji.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://pgg.svipenyu.cn

[R48] awk 取指定列
来源：http://dtb.cashguo.top

awk '{print $1, $3}' a.txt
来源：http://eku.sweek.top

[R49] awk 带条件
来源：http://ktq.c1oappe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mts.zhixingplan.top

[R50] awk 求和
来源：http://vsd.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wgi.yuanzhike.top

[R51] 排序去重取前几
来源：http://ayq.zhongyouzk.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lju.daria6918.cn

[R52] 统计行数
来源：http://pbo.pengpengdd.cyou

wc -l a.txt
来源：http://byf.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://ung.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://joa.bbcook.cn

[R54] 比较两个文件
来源：http://bfn.sysykeji.top

diff a.txt b.txt
来源：http://yvu.vehdjk.com

[R55] 压缩与解压
来源：http://yzl.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dlv.yj20258888.top

[R56] 远程拷贝
来源：http://nzx.xinyue.icu

scp file user@host:/path/
来源：http://tkr.pengpengdd.cyou

[R57] 远程执行命令
来源：http://jck.xylfe.cn

ssh user@host 'uptime'
来源：http://atd.yueranfly.top

[R58] 下载文件
来源：http://twp.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://umz.wangdashe.top

[R59] 发 POST JSON
来源：http://wfr.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tyb.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://rwu.zhixingplan.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zvb.vqdsnc.cn

[R61] 磁盘占用
来源：http://xjo.snrcjt.cn

df -h;  du -sh *
来源：http://wsj.epnwcf.com

[R62] 找最占空间的文件
来源：http://dhj.meibo888.top

du -ah . | sort -rh | head -10
来源：http://wqn.redwolf501.top

[R63] 内存与进程
来源：http://irs.sweek.top

free -h;  ps aux | grep nginx
来源：http://mua.hnqzz.top

[R64] 结束进程
来源：http://wfg.shangyingyoupin.top

kill -9 $(pgrep -f app.py)
来源：http://vdd.redwolf501.top

[R65] 查看端口占用
来源：http://iak.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bum.chenjidiqi.icu

[R66] 定时任务
来源：http://efz.hysaishi.cn

crontab -e;  crontab -l
来源：http://dht.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://vox.9152youxi.cn

openssl rand -hex 16
来源：http://hlb.bjfxy.top

[R68] 计算文件校验值
来源：http://vhp.xziqi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zyp.cqqwz.cn

[R69] 生成随机密码
来源：http://zyp.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://tfe.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://fno.fengsongda.top

date +%s;  date -d @1700000000
来源：http://kwo.yj202588.top

[R71] 日期格式化
来源：http://mlq.cqqwz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bzm.c1oappe.top

[R72] 等待端口就绪
来源：http://lnn.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://klu.cqqwz.cn

[R73] 分割大日志
来源：http://vhy.andypj.xyz

split -l 1000 big.log part_
来源：http://pwh.pengpengdd.cyou

[R74] 批量重命名
来源：http://rqa.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dbz.chenjidiqi.icu

[R75] 导出环境变量
来源：http://tmc.vqdsnc.cn

export PATH="$HOME/bin:$PATH"
来源：http://agu.c1oappe.top

[R76] 使用临时文件
来源：http://apd.jiagoushi.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yne.c1oappe.top

[R77] 读取用户输入
来源：http://ddo.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://sih.pycfn.com

[R78] 交互式菜单
来源：http://qqr.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://aeo.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://pqk.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yld.xingfuxueyuan.xyz

[R80] 查看脚本执行耗时
来源：http://isf.sweek.top

time ./run.sh
来源：http://ysn.hongshengwenyu.top

================================================================================
来源：http://lsn.fktsv.cn

S. C / C++ 专题
来源：http://lml.haohaochexian.top

================================================================================
来源：http://ity.kuanghao11.cn

[S01] C：Hello World
来源：http://hgs.52xcode.cn

#include <stdio.h>
来源：http://pli.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cux.nanxuanxn.top

[S02] C：变量与格式化输出
来源：http://pyy.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://zkh.yvedp.cn

[S03] C：读入整数
来源：http://pmg.zhijiandao.cn

int x; scanf("%d", &x);
来源：http://ikr.hywenlv.cn

[S04] C：字符串复制
来源：http://fpn.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tnj.hammf.cn

[S05] C：字符串长度
来源：http://ilx.uphjek.com

strlen(s)
来源：http://tld.0kj1m.cn

[S06] C：字符串比较
来源：http://ish.jiagoushi.top

strcmp(a, b) == 0
来源：http://lcc.zhixingplan.top

[S07] C：数组遍历求和
来源：http://lve.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nqw.tanke756.top

[S08] C：动态内存分配与释放
来源：http://hxg.cqqwz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sqx.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://cte.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pqv.shzxlz.cn

[S10] C：指针与解引用
来源：http://kwh.xziqi.cn

int *p = &a;  *p = 5;
来源：http://fid.xingfuxueyuan.xyz

[S11] C：逐行读文件
来源：http://bzu.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://nzt.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mdk.316326.xyz

fclose(f);
来源：http://oug.daria6918.cn

[S12] C：写文件
来源：http://qra.jqgufenzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jok.yfazqb.com

[S13] C：宏定义
来源：http://bfo.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cpd.jiagoushi.top

[S14] C：枚举
来源：http://edr.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://lws.yueranfly.top

[S15] C：类型转换
来源：http://qqn.shanyushiyangtech.top

(double) a / b
来源：http://nkh.hcnkem.com

[S16] C：位操作置位
来源：http://zmw.zdqjudy.top

x |= (1 << 3);
来源：http://qvo.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://gme.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rpb.zhongyouzk.top

[S18] C：命令行参数
来源：http://xxd.guowangkeji.top

int main(int argc, char **argv)
来源：http://jqn.ydzc1.top

[S19] C：快速排序
来源：http://ugj.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://jav.cheryme.top

[S20] C：二分查找
来源：http://zft.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qoz.guowangkeji.top

[S21] C：字符类别判断
来源：http://ejb.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hhm.dashuyun.cn

[S22] C：字符串转数字
来源：http://mid.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://dby.svipenyu.cn

[S23] C：随机数
来源：http://omc.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://dzd.fktsv.cn

[S24] C：获取本地时间
来源：http://qzy.fanxiaobao.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://foc.shanyushiyangkeji.top

[S25] C：内存拷贝
来源：http://dcw.vqdsnc.cn

memcpy(dst, src, n);
来源：http://opn.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://bdh.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://ari.yangfankeji.com

[S27] C：定义常量
来源：http://ddm.uphjek.com

const double PI = 3.14159;
来源：http://flz.yj20258888.top

[S28] C：静态变量
来源：http://cwv.zdqjudy.top

static int counter = 0;
来源：http://wux.havefunace.top

[S29] C：变参函数
来源：http://nkf.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dba.xinyue.icu

[S30] C：头文件保护
来源：http://yca.yvedp.cn

#ifndef X_H
来源：http://klg.zhixingplan.top

#define X_H
来源：http://tqk.mhx1999.top

#endif
来源：http://uyu.zdqjudy.top

[S31] C++：Hello World
来源：http://mnk.xingfuxueyuan.xyz

#include <iostream>
来源：http://fnc.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://xlz.hysaishi.cn

[S32] C++：字符串
来源：http://enq.iojbl.cn

std::string s = "hi";  s += "!";
来源：http://vrv.xylfe.cn

[S33] C++：vector 增删
来源：http://epo.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://frs.jyoumei.cn

[S34] C++：遍历 vector
来源：http://dfh.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://mrk.havefunace.top

[S35] C++：map
来源：http://jpq.andypj.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eqt.daxiang520.top

[S36] C++：unordered_map
来源：http://ogt.vqdsnc.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ycd.9152youxi.cn

[S37] C++：set
来源：http://iue.zhixingplan.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qxu.sjlbkw.cn

[S38] C++：排序
来源：http://okj.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://ney.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://cpl.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://urm.feifeiyinyue.top

[S40] C++：查找元素
来源：http://uyh.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qzy.xylfe.cn

[S41] C++：类与构造函数
来源：http://aoe.zhongyouzk.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jgm.bjfxy.top

[S42] C++：继承与虚函数
来源：http://tiz.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://cbk.sxryk.cn

[S43] C++：智能指针
来源：http://mpg.sysykeji.top

auto p = std::make_unique<int>(5);
来源：http://elz.chenjidiqi.icu

[S44] C++：引用传参
来源：http://ids.jiagoushi.top

void inc(int &x) { ++x; }
来源：http://xuo.tarul.cn

[S45] C++：lambda
来源：http://mbj.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://ntu.yanxiufei.cn

[S46] C++：函数模板
来源：http://uae.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eid.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://luz.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yzg.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://the.chenjidiqi.icu

std::ifstream in("a.txt");  std::string line;
来源：http://njj.aizwys.cn

while (std::getline(in, line)) { }
来源：http://ous.hnqzz.top

[S49] C++：写文件
来源：http://xmv.hongshengwenyu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tav.sufxvd.cn

[S50] C++：格式化数字
来源：http://bim.xziqi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zty.xuanzx.com

[S51] C++：显式类型转换
来源：http://jzs.jinqigfzy.top

static_cast<double>(a) / b
来源：http://krw.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://por.dashuyun.cn

int size() const noexcept { return n_; }
来源：http://mra.tarul.cn

[S53] C++：移动语义
来源：http://ejd.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://jwk.yonumen.top

[S54] C++：异常处理
来源：http://pwf.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vsk.yuxming.cn

[S55] C++：结构化绑定
来源：http://nmc.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lrw.hcnkem.com

[S56] C++：optional
来源：http://quc.jinghuilouyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hwy.iojbl.cn

[S57] C++：编译期常量
来源：http://wjw.yueranfly.top

constexpr int N = 10;
来源：http://wcj.jqgufenzy.top

[S58] C++：命名空间
来源：http://qfw.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://cfk.hnqzz.top

[S59] C++：静态断言
来源：http://hix.yj20258888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qwl.zdbjq.cn

[S60] C++：遍历并删除元素
来源：http://uwt.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rbz.aizwys.cn

================================================================================
来源：http://ktf.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yjg.hysaishi.cn

================================================================================
来源：http://krm.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://nal.zhengqikj.top

println("Hello")
来源：http://zmr.epnwcf.com

[T02] Kotlin：变量
来源：http://onn.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zgv.yueranfly.top

[T03] Kotlin：字符串模板
来源：http://bdt.jinqigufen.top

"值: $b"
来源：http://hfw.cdnleiting.top

[T04] Kotlin：空安全
来源：http://det.zhijiandao.cn

val n: String? = null;  n?.length
来源：http://cel.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://cvx.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qlg.birdmap.top

[T06] Kotlin：集合映射
来源：http://idl.cucudq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cwj.hammf.cn

[T07] Kotlin：集合过滤
来源：http://zfw.hywenlv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://puq.meibo888.top

[T08] Kotlin：数据类
来源：http://uxe.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://yri.zycfv.cn

[T09] Kotlin：扩展函数
来源：http://zho.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://tfl.yj202588.top

[T10] Kotlin：默认参数
来源：http://zsj.ydjk.org.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kki.zycfv.cn

[T11] Kotlin：协程
来源：http://jmt.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://iif.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://mhn.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://lvt.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://cnf.wangshuangyany.cn

val m = mapOf("a" to 1)
来源：http://wyz.ydjk.org.cn

[T14] Kotlin：循环
来源：http://cyj.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://yok.9152youxi.cn

[T15] Kotlin：接口
来源：http://gel.gzhubu.top

interface Shape { fun area(): Double }
来源：http://ycy.daxiang520.top

[T16] Swift：Hello World
来源：http://wol.quarkkingdee.top

print("Hello")
来源：http://iqw.dianchejie.cn

[T17] Swift：变量与常量
来源：http://qtq.ctjpmb.com

var a = 1;  let b = 2
来源：http://ztb.jiagoushi.top

[T18] Swift：字符串插值
来源：http://izv.316326.xyz

"值: \(b)"
来源：http://wty.iojbl.cn

[T19] Swift：可选绑定
来源：http://kqx.uphjek.com

if let n = opt { print(n) }
来源：http://mmm.hnxiangtu.top

[T20] Swift：数组操作
来源：http://yac.jinyuanbaomall.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dcy.xylfe.cn

[T21] Swift：遍历
来源：http://rqh.zhixingplan.top

for x in a { print(x) }
来源：http://gtn.guowangkeji.top

[T22] Swift：字典
来源：http://ycg.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ofm.zhengqikj.top


<!-- 参考信息 -->