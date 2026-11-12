代发 wailian999

echo "${#arr[@]}"
来源：http://beu.pengpengdd.cyou

[R20] 关联数组（字典）
来源：http://hrn.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rvy.hfpthk.cn

[R21] 字符串长度
来源：http://pkh.dashuyun.cn

echo "${#s}"
来源：http://wgh.zhiwuduotai.top

[R22] 截取子串
来源：http://ghe.jqgufenzy.top

echo "${s:0:5}"
来源：http://hdh.shanyushiyangtech.top

[R23] 字符串替换
来源：http://xdz.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ydj.gotoacloud.top

[R24] 大小写转换
来源：http://sgh.tianlin.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://ypf.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://hgd.9152youxi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tmy.chenjidiqi.icu

[R26] 命令替换
来源：http://fwi.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://tbc.jqgufenzy.top

[R27] 算术展开
来源：http://wte.mhx1999.top

echo $((1 + 2 * 3))
来源：http://pfd.cashguo.top

[R28] 浮点运算
来源：http://gif.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://zwg.chenjidiqi.icu

[R29] 定义函数
来源：http://bvu.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zsz.bbcook.cn

[R30] 函数返回状态码
来源：http://hvo.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://fxb.ydzc1.top

[R31] 局部变量
来源：http://xrl.0kj1m.cn

f() { local x=1; echo "$x"; }
来源：http://fpk.ivvv.top

[R32] 参数个数校验
来源：http://khj.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bay.andypj.xyz

[R33] 捕获错误并提示行号
来源：http://slt.sjlbkw.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lxw.pengpengdd.cyou

[R34] 退出时清理
来源：http://udr.havefunace.top

trap 'rm -f "$tmp"' EXIT
来源：http://tbg.zdbjq.cn

[R35] 后台执行并等待
来源：http://dqc.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ybp.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://wdp.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fty.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://cmp.fktsv.cn

files=$(ls -1)
来源：http://lvv.gzhubu.top

[R38] 管道串联
来源：http://yzm.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://aza.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://fuk.jqgfzy.top

cmd > out.log 2>&1
来源：http://wos.jinqigufen.top

[R40] 追加写日志
来源：http://ebd.sufxvd.cn

echo "log" >> out.log
来源：http://ucs.jlsjyb.cn

[R41] 丢弃输出
来源：http://spe.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://jsm.vqdsnc.cn

[R42] 输入重定向
来源：http://vyz.shanyushiyangtech.top

wc -l < a.txt
来源：http://fhn.pycfn.com

[R43] 按名字查找文件
来源：http://wus.zdqjudy.top

find . -name "*.log" -type f
来源：http://mvd.meibo888.top

[R44] 按修改时间查找
来源：http://eri.tian-w.cn

find . -mtime -7 -type f
来源：http://yry.yueranfly.top

[R45] 批量删除
来源：http://ffk.fktsv.cn

find . -name "*.tmp" -delete
来源：http://erk.shzxlz.cn

[R46] 递归替换文件内容
来源：http://rrp.cqqwz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qgy.hongshengwenyu.top

[R47] sed 单行替换
来源：http://fnq.jlsjyb.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qbh.yj202588.top

[R48] awk 取指定列
来源：http://oej.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://cnr.cashguo.top

[R49] awk 带条件
来源：http://ztm.fanxiaobao.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xlz.jiagoushi.top

[R50] awk 求和
来源：http://fhj.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wqn.mhx1999.top

[R51] 排序去重取前几
来源：http://rve.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://bpn.smart0.xyz

[R52] 统计行数
来源：http://gnd.yvedp.cn

wc -l a.txt
来源：http://cfi.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://wdm.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gtd.zdbjq.cn

[R54] 比较两个文件
来源：http://zro.316326.xyz

diff a.txt b.txt
来源：http://epm.jiagoushi.top

[R55] 压缩与解压
来源：http://cnt.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://egq.mhx1999.top

[R56] 远程拷贝
来源：http://bty.epnwcf.com

scp file user@host:/path/
来源：http://jnc.zhijiandao.cn

[R57] 远程执行命令
来源：http://yej.zdbjq.cn

ssh user@host 'uptime'
来源：http://dgj.sufxvd.cn

[R58] 下载文件
来源：http://dkj.ctjpmb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://coz.sjlbkw.cn

[R59] 发 POST JSON
来源：http://lyy.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cto.yfazqb.com

[R60] 只看 HTTP 状态码
来源：http://ywj.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eiv.iojbl.cn

[R61] 磁盘占用
来源：http://gws.tarul.cn

df -h;  du -sh *
来源：http://tfx.daxiang520.top

[R62] 找最占空间的文件
来源：http://wor.pycfn.com

du -ah . | sort -rh | head -10
来源：http://jkh.ydjk.org.cn

[R63] 内存与进程
来源：http://bte.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://est.cdnleiting.top

[R64] 结束进程
来源：http://auo.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://aqz.wangshuangyany.cn

[R65] 查看端口占用
来源：http://wzk.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ueg.bbcook.cn

[R66] 定时任务
来源：http://kld.kuanghao11.cn

crontab -e;  crontab -l
来源：http://ehx.sjlbkw.cn

[R67] 生成随机十六进制串
来源：http://bnk.bbcook.cn

openssl rand -hex 16
来源：http://xub.bbcook.cn

[R68] 计算文件校验值
来源：http://iil.fktsv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zpj.sxryk.cn

[R69] 生成随机密码
来源：http://xwv.daria6918.cn

head -c 16 /dev/urandom | base64
来源：http://wau.yuanzhike.top

[R70] 时间戳与互转
来源：http://pop.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://gtf.fzhhl.top

[R71] 日期格式化
来源：http://dbv.nanxuanxn.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zhe.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://alc.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wds.aibaodan.cn

[R73] 分割大日志
来源：http://vzk.gaohongyu789.top

split -l 1000 big.log part_
来源：http://slt.9152youxi.cn

[R74] 批量重命名
来源：http://hke.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blk.wangshuangyany.cn

[R75] 导出环境变量
来源：http://nia.iojbl.cn

export PATH="$HOME/bin:$PATH"
来源：http://aoh.sysykeji.top

[R76] 使用临时文件
来源：http://wjq.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eqy.ctjpmb.com

[R77] 读取用户输入
来源：http://vum.jyoumei.cn

read -rp "请输入: " ans
来源：http://ihq.ehwqpu.com

[R78] 交互式菜单
来源：http://llg.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://eoo.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://hbw.wangdashe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ndf.yongpay.top

[R80] 查看脚本执行耗时
来源：http://onm.cucudq.cn

time ./run.sh
来源：http://bnk.sxryk.cn

================================================================================
来源：http://emw.pycfn.com

S. C / C++ 专题
来源：http://kmj.jqgfzy.top

================================================================================
来源：http://ull.aibaodan.cn

[S01] C：Hello World
来源：http://ezj.hnqzz.top

#include <stdio.h>
来源：http://blc.hfpthk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mom.hysaishi.cn

[S02] C：变量与格式化输出
来源：http://njg.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://bck.epnwcf.com

[S03] C：读入整数
来源：http://zip.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://pqy.meibo888.top

[S04] C：字符串复制
来源：http://mor.aibaodan.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rly.feifeiyinyue.top

[S05] C：字符串长度
来源：http://sgn.dianchejie.cn

strlen(s)
来源：http://wlk.vqdsnc.cn

[S06] C：字符串比较
来源：http://ofi.52xcode.cn

strcmp(a, b) == 0
来源：http://brt.xuetiantiany.cn

[S07] C：数组遍历求和
来源：http://xtd.xuetiantiany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jgh.havefunace.top

[S08] C：动态内存分配与释放
来源：http://aqo.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sbd.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://kdn.tian-w.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kvk.xuetiantiany.cn

[S10] C：指针与解引用
来源：http://mcg.pycfn.com

int *p = &a;  *p = 5;
来源：http://ghv.shzxlz.cn

[S11] C：逐行读文件
来源：http://rqk.guowangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://vsm.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://txx.aibaodan.cn

fclose(f);
来源：http://rme.zhoulong.xyz

[S12] C：写文件
来源：http://eqp.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nmf.bjfxy.top

[S13] C：宏定义
来源：http://mos.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uyu.meibo888.top

[S14] C：枚举
来源：http://udv.vehdjk.com

enum Color { RED, GREEN, BLUE };
来源：http://uur.yueranfly.top

[S15] C：类型转换
来源：http://rpq.zhengqikj.top

(double) a / b
来源：http://srd.dashuyun.cn

[S16] C：位操作置位
来源：http://tap.hcnkem.com

x |= (1 << 3);
来源：http://efj.redwolf501.top

[S17] C：安全拼接字符串
来源：http://dfn.redwolf501.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wbi.yj20258.top

[S18] C：命令行参数
来源：http://pcf.xziqi.cn

int main(int argc, char **argv)
来源：http://teh.dashuyun.cn

[S19] C：快速排序
来源：http://clu.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://qiu.chenlongwang.top

[S20] C：二分查找
来源：http://vac.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gqf.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://yog.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ifz.chenlongwang.top

[S22] C：字符串转数字
来源：http://bxj.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://slo.yanxiufei.cn

[S23] C：随机数
来源：http://eua.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cvj.ehwqpu.com

[S24] C：获取本地时间
来源：http://jmf.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sdh.chenlongwang.top

[S25] C：内存拷贝
来源：http://xbt.hongshengwenyu.top

memcpy(dst, src, n);
来源：http://pog.epnwcf.com

[S26] C：内存清零
来源：http://pmg.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://dcp.shangyingyoupin.top

[S27] C：定义常量
来源：http://vcy.yuxming.cn

const double PI = 3.14159;
来源：http://uug.kuanghao11.cn

[S28] C：静态变量
来源：http://hch.zhiwuduotai.top

static int counter = 0;
来源：http://zju.jinqigufen.top

[S29] C：变参函数
来源：http://mtf.daria6918.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://som.chenlongwang.top

[S30] C：头文件保护
来源：http://fsj.ydzc1.top

#ifndef X_H
来源：http://buc.jinqigfzy.top

#define X_H
来源：http://rbq.zdqjudy.top

#endif
来源：http://zxc.hywenlv.cn

[S31] C++：Hello World
来源：http://gqr.jianghu66.top

#include <iostream>
来源：http://djl.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://zeq.feifeiyinyue.top

[S32] C++：字符串
来源：http://cds.yanxiufei.cn

std::string s = "hi";  s += "!";
来源：http://hvi.mhx1999.top

[S33] C++：vector 增删
来源：http://xpu.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rtg.ivvv.top

[S34] C++：遍历 vector
来源：http://djo.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://wma.ybcxt.top

[S35] C++：map
来源：http://vpy.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://izt.hcnkem.com

[S36] C++：unordered_map
来源：http://qud.xuanzx.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wzl.fengsongda.top

[S37] C++：set
来源：http://jel.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wyc.haohaochexian.top

[S38] C++：排序
来源：http://ssf.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://has.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://sfy.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lpw.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://uot.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sep.52xcode.cn

[S41] C++：类与构造函数
来源：http://rxo.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ncy.epnwcf.com

[S42] C++：继承与虚函数
来源：http://ddm.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://kqv.hongshengwenyu.top

[S43] C++：智能指针
来源：http://vkb.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://sof.hysaishi.cn

[S44] C++：引用传参
来源：http://nei.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://wti.yueranfly.top

[S45] C++：lambda
来源：http://dsy.nanxinkj.top

auto add = [](int a, int b) { return a + b; };
来源：http://crt.jlsjyb.cn

[S46] C++：函数模板
来源：http://psz.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iwb.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://wfr.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ndn.ehwqpu.com

[S48] C++：逐行读文件
来源：http://toy.mhx1999.top

std::ifstream in("a.txt");  std::string line;
来源：http://rnn.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://hvr.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://ybk.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kso.nanxuanxn.top

[S50] C++：格式化数字
来源：http://zmq.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://htg.gotoacloud.top

[S51] C++：显式类型转换
来源：http://yur.hywenlv.cn

static_cast<double>(a) / b
来源：http://vey.ppjwa.cn

[S52] C++：const 与 noexcept
来源：http://iib.hongshengwenyu.top

int size() const noexcept { return n_; }
来源：http://hor.feifeiyinyue.top

[S53] C++：移动语义
来源：http://epp.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://loq.jianghu66.top

[S54] C++：异常处理
来源：http://nhd.hywenlv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gxl.xingfuxueyuan.xyz

[S55] C++：结构化绑定
来源：http://igq.smart0.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://sge.gaohongyu789.top

[S56] C++：optional
来源：http://xbt.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oab.dianchejie.cn

[S57] C++：编译期常量
来源：http://oob.52xcode.cn

constexpr int N = 10;
来源：http://cyj.sweek.top

[S58] C++：命名空间
来源：http://xzu.hcnkem.com

namespace ns { int f() { return 1; } }
来源：http://cyz.guowangkeji.top

[S59] C++：静态断言
来源：http://let.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nzy.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://zrg.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bty.hammf.cn

================================================================================
来源：http://msq.yj20258888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tzk.316326.xyz

================================================================================
来源：http://wgj.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://zdb.yuanzhike.top

println("Hello")
来源：http://zrm.guowangkeji.top

[T02] Kotlin：变量
来源：http://soc.aibaodan.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dad.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://szt.xinyue.icu

"值: $b"
来源：http://abd.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://ewt.birdmap.top

val n: String? = null;  n?.length
来源：http://nzi.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://wxv.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ncl.wangdashe.top

[T06] Kotlin：集合映射
来源：http://wfa.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wjw.guannengcc.top

[T07] Kotlin：集合过滤
来源：http://ohb.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://why.hesvh.cn

[T08] Kotlin：数据类
来源：http://vpy.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://yal.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://pna.cashguo.top

fun String.exclaim() = this + "!"
来源：http://smp.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://crp.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://emm.zhengqikj.top

[T11] Kotlin：协程
来源：http://tsb.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zkb.52xcode.cn

[T12] Kotlin：解构声明
来源：http://lbl.9152youxi.cn

val (a, b) = Pair(1, 2)
来源：http://cti.shuidangran.top

[T13] Kotlin：只读 Map
来源：http://anp.yuxming.cn

val m = mapOf("a" to 1)
来源：http://qrp.ctjpmb.com

[T14] Kotlin：循环
来源：http://bod.pengpengdd.cyou

for (i in 1..10) println(i)
来源：http://mwo.zdbjq.cn

[T15] Kotlin：接口
来源：http://yxr.yj20258.top

interface Shape { fun area(): Double }
来源：http://qtj.cqqwz.cn

[T16] Swift：Hello World
来源：http://ojx.hnxiangtu.top

print("Hello")
来源：http://qai.sysykeji.top

[T17] Swift：变量与常量
来源：http://xnc.yueranfly.top

var a = 1;  let b = 2
来源：http://omf.chenjidiqi.icu

[T18] Swift：字符串插值
来源：http://iif.hywenlv.cn

"值: \(b)"
来源：http://wfs.zhixingplan.top

[T19] Swift：可选绑定
来源：http://bsz.gzhubu.top

if let n = opt { print(n) }
来源：http://xsy.sysykeji.top

[T20] Swift：数组操作
来源：http://kxo.aibaodan.cn

var a = [1, 2, 3];  a.append(4)
来源：http://izx.yvedp.cn

[T21] Swift：遍历
来源：http://bwh.jinghuilouyu.cn

for x in a { print(x) }
来源：http://qdc.ppjwa.cn

[T22] Swift：字典
来源：http://hlw.hongshengwenyu.top

var d = ["a": 1];  d["b"] = 2
来源：http://jnh.quarkkingdee.top


<!-- 参考信息 -->