代发 wailian999

echo "${#s}"
来源：http://lab.jqgufenzy.top

[R22] 截取子串
来源：http://hys.ydzc1.top

echo "${s:0:5}"
来源：http://ubq.havefunace.top

[R23] 字符串替换
来源：http://krm.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kuj.jinghuilouyu.cn

[R24] 大小写转换
来源：http://zht.pengpengdd.cyou

echo "${s^^}"; echo "${s,,}"
来源：http://sfy.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://ebh.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://xyu.yangfankeji.com

[R26] 命令替换
来源：http://mnw.xinyue.icu

now=$(date +%F); echo "$now"
来源：http://bks.yuanzhike.top

[R27] 算术展开
来源：http://uuh.xziqi.cn

echo $((1 + 2 * 3))
来源：http://hkh.sjlbkw.cn

[R28] 浮点运算
来源：http://rta.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://vbf.xingfuxueyuan.xyz

[R29] 定义函数
来源：http://pyl.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fhh.gogol.net.cn

[R30] 函数返回状态码
来源：http://zve.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://zhf.ppjwa.cn

[R31] 局部变量
来源：http://ikp.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://kfr.vqdsnc.cn

[R32] 参数个数校验
来源：http://qty.cashguo.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bar.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://lvw.hfpthk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jul.zhongyouzk.top

[R34] 退出时清理
来源：http://gig.dianchejie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rmf.tianlin.xyz

[R35] 后台执行并等待
来源：http://zyb.svipenyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://npj.yuxming.cn

[R36] 并发执行多个任务
来源：http://bgl.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ufb.wangshuangyany.cn

[R37] 把输出赋给变量
来源：http://ors.birdmap.top

files=$(ls -1)
来源：http://spt.jyoumei.cn

[R38] 管道串联
来源：http://efj.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://efg.havefunace.top

[R39] 重定向标准输出与错误
来源：http://wwn.ehwqpu.com

cmd > out.log 2>&1
来源：http://lan.fzhhl.top

[R40] 追加写日志
来源：http://inn.jqgufenzy.top

echo "log" >> out.log
来源：http://mjm.nanxinkj.top

[R41] 丢弃输出
来源：http://bzy.feifeiyinyue.top

cmd >/dev/null 2>&1
来源：http://zsy.sufxvd.cn

[R42] 输入重定向
来源：http://gpa.andypj.xyz

wc -l < a.txt
来源：http://rhd.gzhubu.top

[R43] 按名字查找文件
来源：http://rvt.shangyingyoupin.top

find . -name "*.log" -type f
来源：http://ifw.chenjidiqi.icu

[R44] 按修改时间查找
来源：http://clf.dashuyun.cn

find . -mtime -7 -type f
来源：http://fgh.jqgfzy.top

[R45] 批量删除
来源：http://cxm.sysykeji.top

find . -name "*.tmp" -delete
来源：http://hth.zycfv.cn

[R46] 递归替换文件内容
来源：http://fiu.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fvy.wangshuangyany.cn

[R47] sed 单行替换
来源：http://dyr.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://mij.zhongyouzk.top

[R48] awk 取指定列
来源：http://vgk.hfpthk.cn

awk '{print $1, $3}' a.txt
来源：http://gao.yueranfly.top

[R49] awk 带条件
来源：http://hre.dianchejie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nds.jqgfzy.top

[R50] awk 求和
来源：http://gsy.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://zsr.aibaodan.cn

[R51] 排序去重取前几
来源：http://lae.jinqigfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pgd.ivvv.top

[R52] 统计行数
来源：http://nwt.andypj.xyz

wc -l a.txt
来源：http://vum.havefunace.top

[R53] 查看文件头与实时尾
来源：http://tiz.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pzq.quarkkingdee.top

[R54] 比较两个文件
来源：http://fnx.epnwcf.com

diff a.txt b.txt
来源：http://qvj.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://nin.ydjk.org.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lqj.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://nsg.jiagoushi.top

scp file user@host:/path/
来源：http://ihh.52xcode.cn

[R57] 远程执行命令
来源：http://aam.epnwcf.com

ssh user@host 'uptime'
来源：http://ztg.shzxlz.cn

[R58] 下载文件
来源：http://duc.tarul.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://caj.aizwys.cn

[R59] 发 POST JSON
来源：http://bsu.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pdv.0kj1m.cn

[R60] 只看 HTTP 状态码
来源：http://akt.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qsw.yanxiufei.cn

[R61] 磁盘占用
来源：http://fas.sufxvd.cn

df -h;  du -sh *
来源：http://mam.smart0.xyz

[R62] 找最占空间的文件
来源：http://cos.cdnleiting.top

du -ah . | sort -rh | head -10
来源：http://but.sufxvd.cn

[R63] 内存与进程
来源：http://eqw.nanxuanxn.top

free -h;  ps aux | grep nginx
来源：http://ofy.hnqzz.top

[R64] 结束进程
来源：http://ssn.chenlongwang.top

kill -9 $(pgrep -f app.py)
来源：http://wft.feifeiyinyue.top

[R65] 查看端口占用
来源：http://jox.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gmk.epnwcf.com

[R66] 定时任务
来源：http://upm.nanxuanxn.top

crontab -e;  crontab -l
来源：http://jbv.cheryme.top

[R67] 生成随机十六进制串
来源：http://qmd.nanxinkj.top

openssl rand -hex 16
来源：http://kkt.shangyingyoupin.top

[R68] 计算文件校验值
来源：http://pkw.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://nzq.yfazqb.com

[R69] 生成随机密码
来源：http://dsv.xinyue.icu

head -c 16 /dev/urandom | base64
来源：http://uap.yj202588.top

[R70] 时间戳与互转
来源：http://vps.tanke756.top

date +%s;  date -d @1700000000
来源：http://kaz.dashuyun.cn

[R71] 日期格式化
来源：http://epg.nanxuanxn.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mto.jqgufenzy.top

[R72] 等待端口就绪
来源：http://ysx.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rjp.ctjpmb.com

[R73] 分割大日志
来源：http://huv.shangyingyoupin.top

split -l 1000 big.log part_
来源：http://yph.daxiang520.top

[R74] 批量重命名
来源：http://rhk.jyoumei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vpb.jlsjyb.cn

[R75] 导出环境变量
来源：http://uzt.zhiwuduotai.top

export PATH="$HOME/bin:$PATH"
来源：http://tyz.xinyue.icu

[R76] 使用临时文件
来源：http://hyx.aibaodan.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fit.sufxvd.cn

[R77] 读取用户输入
来源：http://arl.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://jpf.cashguo.top

[R78] 交互式菜单
来源：http://snz.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hxx.epnwcf.com

[R79] 解析命令行选项
来源：http://fqo.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mbi.ybcxt.top

[R80] 查看脚本执行耗时
来源：http://ynj.sufxvd.cn

time ./run.sh
来源：http://wzs.yueranfly.top

================================================================================
来源：http://uqk.bbcook.cn

S. C / C++ 专题
来源：http://zlx.ehwqpu.com

================================================================================
来源：http://otw.xuanzx.com

[S01] C：Hello World
来源：http://xdn.cucudq.cn

#include <stdio.h>
来源：http://luy.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bav.zdbjq.cn

[S02] C：变量与格式化输出
来源：http://nuu.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://eqa.0kj1m.cn

[S03] C：读入整数
来源：http://vcz.haohaochexian.top

int x; scanf("%d", &x);
来源：http://tpw.uphjek.com

[S04] C：字符串复制
来源：http://ens.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://rir.c1oappe.top

[S05] C：字符串长度
来源：http://tik.ppjwa.cn

strlen(s)
来源：http://apd.snrcjt.cn

[S06] C：字符串比较
来源：http://dav.tian-w.cn

strcmp(a, b) == 0
来源：http://dxi.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://ybn.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pao.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://hib.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xsn.cashguo.top

[S09] C：结构体定义与初始化
来源：http://ryc.hnqzz.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://upm.cucudq.cn

[S10] C：指针与解引用
来源：http://tba.xinyue.icu

int *p = &a;  *p = 5;
来源：http://aoz.c1oappe.top

[S11] C：逐行读文件
来源：http://vpq.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://ydm.nanxuanxn.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pfv.cashguo.top

fclose(f);
来源：http://hwy.zhixingplan.top

[S12] C：写文件
来源：http://riw.chenjidiqi.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rhv.zhongyouzk.top

[S13] C：宏定义
来源：http://gdb.gzhubu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eoi.jqgfzy.top

[S14] C：枚举
来源：http://ays.cqqwz.cn

enum Color { RED, GREEN, BLUE };
来源：http://wmq.jianghu66.top

[S15] C：类型转换
来源：http://fml.yueranfly.top

(double) a / b
来源：http://eyn.cashguo.top

[S16] C：位操作置位
来源：http://bqi.yj20258888.top

x |= (1 << 3);
来源：http://xur.52xcode.cn

[S17] C：安全拼接字符串
来源：http://afv.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jwf.cqqwz.cn

[S18] C：命令行参数
来源：http://rco.sufxvd.cn

int main(int argc, char **argv)
来源：http://xhk.redwolf501.top

[S19] C：快速排序
来源：http://qnc.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://qju.fanxiaobao.xyz

[S20] C：二分查找
来源：http://tkl.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nox.zhoulong.xyz

[S21] C：字符类别判断
来源：http://mqp.iojbl.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hjh.zhixingplan.top

[S22] C：字符串转数字
来源：http://trd.ivvv.top

atoi("42");  strtod("3.14", NULL);
来源：http://dmt.guowangkeji.top

[S23] C：随机数
来源：http://hfc.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xsq.daxiang520.top

[S24] C：获取本地时间
来源：http://tdv.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://icz.gzhubu.top

[S25] C：内存拷贝
来源：http://hxv.hammf.cn

memcpy(dst, src, n);
来源：http://tni.tianlin.xyz

[S26] C：内存清零
来源：http://qtp.pengpengdd.cyou

memset(a, 0, sizeof a);
来源：http://zcz.epnwcf.com

[S27] C：定义常量
来源：http://fqq.shangyingyoupin.top

const double PI = 3.14159;
来源：http://ldn.snrcjt.cn

[S28] C：静态变量
来源：http://oiz.xylfe.cn

static int counter = 0;
来源：http://caq.tarul.cn

[S29] C：变参函数
来源：http://rxp.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vho.chenjidiqi.icu

[S30] C：头文件保护
来源：http://dnr.jinghuilouyu.cn

#ifndef X_H
来源：http://vbf.jinqigfzy.top

#define X_H
来源：http://oys.hfpthk.cn

#endif
来源：http://dss.pycfn.com

[S31] C++：Hello World
来源：http://qaz.yongpay.top

#include <iostream>
来源：http://azm.dianchejie.cn

int main() { std::cout << "Hello\n"; }
来源：http://avw.zhoulong.xyz

[S32] C++：字符串
来源：http://vxi.zhongyouzk.top

std::string s = "hi";  s += "!";
来源：http://omb.9152youxi.cn

[S33] C++：vector 增删
来源：http://ynq.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://puq.tian-w.cn

[S34] C++：遍历 vector
来源：http://urt.gogol.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://ewv.chenzaomai.com

[S35] C++：map
来源：http://cbe.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://scp.zhengqikj.top

[S36] C++：unordered_map
来源：http://vkt.snrcjt.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://feh.kuanghao11.cn

[S37] C++：set
来源：http://rqm.jianghu66.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rku.epnwcf.com

[S38] C++：排序
来源：http://ofl.tarul.cn

std::sort(v.begin(), v.end());
来源：http://vvq.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://ztd.hfpthk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zgn.shzxlz.cn

[S40] C++：查找元素
来源：http://ila.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wmj.yangfankeji.com

[S41] C++：类与构造函数
来源：http://gks.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oaw.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://bbw.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://gtw.chenzaomai.com

[S43] C++：智能指针
来源：http://ara.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://nig.fktsv.cn

[S44] C++：引用传参
来源：http://dtj.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://khh.nanxuanxn.top

[S45] C++：lambda
来源：http://hlg.zhaomingkeji.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://alv.hongshengwenyu.top

[S46] C++：函数模板
来源：http://dnm.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sed.xziqi.cn

[S47] C++：结构化绑定遍历
来源：http://flh.jlsjyb.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dzp.jiagoushi.top

[S48] C++：逐行读文件
来源：http://bll.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://bur.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://esl.shanyushiyangtech.top

[S49] C++：写文件
来源：http://ogc.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ohy.9152youxi.cn

[S50] C++：格式化数字
来源：http://hdf.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rah.316326.xyz

[S51] C++：显式类型转换
来源：http://asb.shuidangran.top

static_cast<double>(a) / b
来源：http://mdm.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://khw.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://ooe.bjfxy.top

[S53] C++：移动语义
来源：http://gea.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://qgm.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://nrx.hammf.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fru.dianchejie.cn

[S55] C++：结构化绑定
来源：http://qcy.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://wfv.sysykeji.top

[S56] C++：optional
来源：http://chx.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kvt.yvedp.cn

[S57] C++：编译期常量
来源：http://ols.316326.xyz

constexpr int N = 10;
来源：http://vfo.cucudq.cn

[S58] C++：命名空间
来源：http://lpf.c1oappe.top

namespace ns { int f() { return 1; } }
来源：http://xfm.cashguo.top

[S59] C++：静态断言
来源：http://pzh.gzhubu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qsy.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://yjw.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kkn.quarkkingdee.top

================================================================================
来源：http://qit.shanyushiyangtech.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://day.ybcxt.top

================================================================================
来源：http://wcx.smart0.xyz

[T01] Kotlin：Hello World
来源：http://gvu.jianghu66.top

println("Hello")
来源：http://elx.wangdashe.top

[T02] Kotlin：变量
来源：http://xok.chenjidiqi.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jtc.yj202588.top

[T03] Kotlin：字符串模板
来源：http://jwy.ydzc1.top

"值: $b"
来源：http://yxq.316326.xyz

[T04] Kotlin：空安全
来源：http://ayr.yueranfly.top

val n: String? = null;  n?.length
来源：http://xue.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://akr.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://giw.zdqjudy.top

[T06] Kotlin：集合映射
来源：http://lnu.jyoumei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hxf.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://eog.yueranfly.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nfv.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://rwp.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://exc.jinghuilouyu.cn

[T09] Kotlin：扩展函数
来源：http://dxv.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://gff.ydzc1.top

[T10] Kotlin：默认参数
来源：http://cfh.zdqjudy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hlj.hcnkem.com

[T11] Kotlin：协程
来源：http://ati.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://arl.zhaomingkeji.xyz

[T12] Kotlin：解构声明
来源：http://oyt.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://nni.cucudq.cn

[T13] Kotlin：只读 Map
来源：http://rjx.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://fxz.gaohongyu789.top

[T14] Kotlin：循环
来源：http://zib.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://vrx.yonumen.top

[T15] Kotlin：接口
来源：http://vut.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://tfm.fengsongda.top

[T16] Swift：Hello World
来源：http://hpw.sweek.top

print("Hello")
来源：http://ejl.tanke756.top

[T17] Swift：变量与常量
来源：http://tbc.zhijiandao.cn

var a = 1;  let b = 2
来源：http://tbt.yanxiufei.cn

[T18] Swift：字符串插值
来源：http://pvg.zhijiandao.cn

"值: \(b)"
来源：http://cxr.smart0.xyz

[T19] Swift：可选绑定
来源：http://fmk.hammf.cn

if let n = opt { print(n) }
来源：http://inj.hnxiangtu.top

[T20] Swift：数组操作
来源：http://gda.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://dql.shangyingyoupin.top

[T21] Swift：遍历
来源：http://hfj.shanyushiyangtech.top

for x in a { print(x) }
来源：http://moc.xingfuxueyuan.xyz

[T22] Swift：字典
来源：http://oky.pycfn.com

var d = ["a": 1];  d["b"] = 2
来源：http://qgb.xuetiantiany.cn

[T23] Swift：函数
来源：http://hdl.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://prb.jinghuilouyu.cn

[T24] Swift：闭包
来源：http://shn.xuanzx.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://edk.gzhubu.top


<!-- 参考信息 -->