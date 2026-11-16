代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://tio.zhiwuduotai.top

[R26] 命令替换
来源：http://iny.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://rfl.ydjk.org.cn

[R27] 算术展开
来源：http://qjs.yvedp.cn

echo $((1 + 2 * 3))
来源：http://dup.kuanghao11.cn

[R28] 浮点运算
来源：http://qaa.jqgufenzy.top

echo "scale=2; 10/3" | bc
来源：http://nxs.hcnkem.com

[R29] 定义函数
来源：http://ycb.zhengqikj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qwq.chenlongwang.top

[R30] 函数返回状态码
来源：http://wpj.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://dgt.guannengcc.top

[R31] 局部变量
来源：http://lwq.fanxiaobao.xyz

f() { local x=1; echo "$x"; }
来源：http://eqe.epnwcf.com

[R32] 参数个数校验
来源：http://lyg.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nsp.jyoumei.cn

[R33] 捕获错误并提示行号
来源：http://pxf.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yhl.xuanzx.com

[R34] 退出时清理
来源：http://bkg.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://wma.zhengqikj.top

[R35] 后台执行并等待
来源：http://gbo.cashguo.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gjf.yj202588.top

[R36] 并发执行多个任务
来源：http://hay.snrcjt.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zhl.shzxlz.cn

[R37] 把输出赋给变量
来源：http://nef.pengpengdd.cyou

files=$(ls -1)
来源：http://uvb.bbcook.cn

[R38] 管道串联
来源：http://cbk.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://gol.xuetiantiany.cn

[R39] 重定向标准输出与错误
来源：http://ttf.fengsongda.top

cmd > out.log 2>&1
来源：http://vug.jianghu66.top

[R40] 追加写日志
来源：http://msr.iojbl.cn

echo "log" >> out.log
来源：http://pvz.jinqigfzy.top

[R41] 丢弃输出
来源：http://bym.vqdsnc.cn

cmd >/dev/null 2>&1
来源：http://icp.havefunace.top

[R42] 输入重定向
来源：http://vgs.fengsongda.top

wc -l < a.txt
来源：http://yoe.jianghu66.top

[R43] 按名字查找文件
来源：http://lcu.sysykeji.top

find . -name "*.log" -type f
来源：http://ymr.yanxiufei.cn

[R44] 按修改时间查找
来源：http://rgr.iojbl.cn

find . -mtime -7 -type f
来源：http://jzk.shangyingyoupin.top

[R45] 批量删除
来源：http://vjh.aizwys.cn

find . -name "*.tmp" -delete
来源：http://xyq.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://tqa.yj20258888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lur.smart0.xyz

[R47] sed 单行替换
来源：http://jmy.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://obg.dianchejie.cn

[R48] awk 取指定列
来源：http://oyi.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://zoa.gotoacloud.top

[R49] awk 带条件
来源：http://uqd.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lom.ydzc1.top

[R50] awk 求和
来源：http://imd.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://lxp.pycfn.com

[R51] 排序去重取前几
来源：http://mwd.kuanghao11.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://efb.pycfn.com

[R52] 统计行数
来源：http://rrg.9152youxi.cn

wc -l a.txt
来源：http://okn.tarul.cn

[R53] 查看文件头与实时尾
来源：http://tlu.cucudq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zul.sjlbkw.cn

[R54] 比较两个文件
来源：http://ect.xinyue.icu

diff a.txt b.txt
来源：http://dwh.chenjidiqi.icu

[R55] 压缩与解压
来源：http://elt.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nvz.gzhubu.top

[R56] 远程拷贝
来源：http://nnj.mhx1999.top

scp file user@host:/path/
来源：http://sce.jqgfzy.top

[R57] 远程执行命令
来源：http://vuk.jlsjyb.cn

ssh user@host 'uptime'
来源：http://gxl.fanxiaobao.xyz

[R58] 下载文件
来源：http://bgi.jlsjyb.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ook.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://qhc.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vwr.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://zop.yonumen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fmy.xuetiantiany.cn

[R61] 磁盘占用
来源：http://sst.mhx1999.top

df -h;  du -sh *
来源：http://ine.ctjpmb.com

[R62] 找最占空间的文件
来源：http://vmj.hongshengwenyu.top

du -ah . | sort -rh | head -10
来源：http://udt.fktsv.cn

[R63] 内存与进程
来源：http://qgk.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://isf.guowangkeji.top

[R64] 结束进程
来源：http://jxq.shangyingyoupin.top

kill -9 $(pgrep -f app.py)
来源：http://iaz.iojbl.cn

[R65] 查看端口占用
来源：http://rsm.hywenlv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xsr.guannengcc.top

[R66] 定时任务
来源：http://zmi.zhengqikj.top

crontab -e;  crontab -l
来源：http://gen.yanxiufei.cn

[R67] 生成随机十六进制串
来源：http://hxr.dianchejie.cn

openssl rand -hex 16
来源：http://nvw.yangfankeji.com

[R68] 计算文件校验值
来源：http://ikn.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dqg.jqgufenzy.top

[R69] 生成随机密码
来源：http://pzj.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://qky.cheryme.top

[R70] 时间戳与互转
来源：http://igz.nanxuanxn.top

date +%s;  date -d @1700000000
来源：http://qsv.ybcxt.top

[R71] 日期格式化
来源：http://tor.jinqigfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gnu.9152youxi.cn

[R72] 等待端口就绪
来源：http://pbs.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://arh.epnwcf.com

[R73] 分割大日志
来源：http://tda.mhx1999.top

split -l 1000 big.log part_
来源：http://prr.mhx1999.top

[R74] 批量重命名
来源：http://ava.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://msr.sufxvd.cn

[R75] 导出环境变量
来源：http://nar.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://kkq.hywenlv.cn

[R76] 使用临时文件
来源：http://ngp.cqqwz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zfb.wangshuangyany.cn

[R77] 读取用户输入
来源：http://twi.mhx1999.top

read -rp "请输入: " ans
来源：http://qos.jyoumei.cn

[R78] 交互式菜单
来源：http://dnt.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pww.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://yod.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qki.cashguo.top

[R80] 查看脚本执行耗时
来源：http://fpk.guannengcc.top

time ./run.sh
来源：http://nck.fengsongda.top

================================================================================
来源：http://wri.cucudq.cn

S. C / C++ 专题
来源：http://gmr.daxiang520.top

================================================================================
来源：http://sym.hysaishi.cn

[S01] C：Hello World
来源：http://xmi.meibo888.top

#include <stdio.h>
来源：http://pah.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nee.zhiwuduotai.top

[S02] C：变量与格式化输出
来源：http://zwg.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://oah.hcnkem.com

[S03] C：读入整数
来源：http://yck.dianchejie.cn

int x; scanf("%d", &x);
来源：http://juf.tian-w.cn

[S04] C：字符串复制
来源：http://jii.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://dpl.yj20258888.top

[S05] C：字符串长度
来源：http://rph.jlsjyb.cn

strlen(s)
来源：http://utx.svipenyu.cn

[S06] C：字符串比较
来源：http://nzu.fzhhl.top

strcmp(a, b) == 0
来源：http://kre.jianghu66.top

[S07] C：数组遍历求和
来源：http://mlj.fengsongda.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://osq.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://vqf.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bby.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://jqh.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://duo.sufxvd.cn

[S10] C：指针与解引用
来源：http://dcz.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://clu.gogol.net.cn

[S11] C：逐行读文件
来源：http://cmg.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://ghh.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kfx.tarul.cn

fclose(f);
来源：http://fzs.yj20258.top

[S12] C：写文件
来源：http://zio.zhixingplan.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zqw.smart0.xyz

[S13] C：宏定义
来源：http://fmm.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dpp.chenlongwang.top

[S14] C：枚举
来源：http://lrh.jinqigfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://iar.gotoacloud.top

[S15] C：类型转换
来源：http://cog.pengpengdd.cyou

(double) a / b
来源：http://uwt.xuetiantiany.cn

[S16] C：位操作置位
来源：http://pgm.c1oappe.top

x |= (1 << 3);
来源：http://rna.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://jjr.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rhn.fengsongda.top

[S18] C：命令行参数
来源：http://fqa.yj20258888.top

int main(int argc, char **argv)
来源：http://qse.cashguo.top

[S19] C：快速排序
来源：http://ryr.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oef.fehbvm.com

[S20] C：二分查找
来源：http://axn.ydjk.org.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://npq.redwolf501.top

[S21] C：字符类别判断
来源：http://zpv.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ssr.yj20258888.top

[S22] C：字符串转数字
来源：http://ecm.hywenlv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cye.ctjpmb.com

[S23] C：随机数
来源：http://xam.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ldm.fanxiaobao.xyz

[S24] C：获取本地时间
来源：http://izh.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qpt.zhaomingkeji.xyz

[S25] C：内存拷贝
来源：http://abh.yj20258.top

memcpy(dst, src, n);
来源：http://kyp.yj20258888.top

[S26] C：内存清零
来源：http://bix.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://hyo.gogol.net.cn

[S27] C：定义常量
来源：http://hzr.sysykeji.top

const double PI = 3.14159;
来源：http://upu.aibaodan.cn

[S28] C：静态变量
来源：http://uuq.zhaomingkeji.xyz

static int counter = 0;
来源：http://wmv.52xcode.cn

[S29] C：变参函数
来源：http://dxb.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ofy.nanxuanxn.top

[S30] C：头文件保护
来源：http://dea.kuanghao11.cn

#ifndef X_H
来源：http://nic.316326.xyz

#define X_H
来源：http://dcq.cheryme.top

#endif
来源：http://tvh.xylfe.cn

[S31] C++：Hello World
来源：http://zjo.ydzc1.top

#include <iostream>
来源：http://omh.yfazqb.com

int main() { std::cout << "Hello\n"; }
来源：http://vlm.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://poz.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://cvz.hcnkem.com

[S33] C++：vector 增删
来源：http://ccx.dashuyun.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uek.tarul.cn

[S34] C++：遍历 vector
来源：http://vuc.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://luy.guannengcc.top

[S35] C++：map
来源：http://emk.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ais.nanxinkj.top

[S36] C++：unordered_map
来源：http://aky.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zab.vqdsnc.cn

[S37] C++：set
来源：http://fjn.pengpengdd.cyou

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xfr.shanyushiyangkeji.top

[S38] C++：排序
来源：http://wdo.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://bym.chenzaomai.com

[S39] C++：自定义比较器排序
来源：http://iju.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ypb.sysykeji.top

[S40] C++：查找元素
来源：http://exm.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oni.hnqzz.top

[S41] C++：类与构造函数
来源：http://ftl.cashguo.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ioz.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://fib.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://qum.vehdjk.com

[S43] C++：智能指针
来源：http://dyx.fzhhl.top

auto p = std::make_unique<int>(5);
来源：http://dlq.sysykeji.top

[S44] C++：引用传参
来源：http://ahs.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://glg.vqdsnc.cn

[S45] C++：lambda
来源：http://kdd.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://ycq.cashguo.top

[S46] C++：函数模板
来源：http://ygh.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pgn.hongshengwenyu.top

[S47] C++：结构化绑定遍历
来源：http://nrw.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hkg.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://rjx.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ddd.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://qsf.ybcxt.top

[S49] C++：写文件
来源：http://xro.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ygy.vqdsnc.cn

[S50] C++：格式化数字
来源：http://oxn.yvedp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://opt.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://zmn.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://hts.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://qzb.dashuyun.cn

int size() const noexcept { return n_; }
来源：http://wpg.cashguo.top

[S53] C++：移动语义
来源：http://itb.iojbl.cn

std::vector<int> w = std::move(v);
来源：http://xtx.xuetiantiany.cn

[S54] C++：异常处理
来源：http://mnc.fktsv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ytn.xinyue.icu

[S55] C++：结构化绑定
来源：http://rar.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://lcv.jlsjyb.cn

[S56] C++：optional
来源：http://oyz.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iiz.tian-w.cn

[S57] C++：编译期常量
来源：http://jsz.zdbjq.cn

constexpr int N = 10;
来源：http://kad.wangdashe.top

[S58] C++：命名空间
来源：http://jwy.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://blu.daxiang520.top

[S59] C++：静态断言
来源：http://uce.xylfe.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kwi.chenzaomai.com

[S60] C++：遍历并删除元素
来源：http://job.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hfc.smart0.xyz

================================================================================
来源：http://blc.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gha.ydjk.org.cn

================================================================================
来源：http://ekv.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://gml.daria6918.cn

println("Hello")
来源：http://roq.cdnleiting.top

[T02] Kotlin：变量
来源：http://jgb.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mwt.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://djn.nanxinkj.top

"值: $b"
来源：http://saj.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://vnh.zhaomingkeji.xyz

val n: String? = null;  n?.length
来源：http://zqv.ctjpmb.com

[T05] Kotlin：when 表达式
来源：http://ejh.birdmap.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://awp.dashuyun.cn

[T06] Kotlin：集合映射
来源：http://mdo.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cfa.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://pxy.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zgo.yj202588.top

[T08] Kotlin：数据类
来源：http://tku.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://enq.andypj.xyz

[T09] Kotlin：扩展函数
来源：http://imn.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://gwy.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://epk.vqdsnc.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://auh.ehwqpu.com

[T11] Kotlin：协程
来源：http://ikz.gotoacloud.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://oqh.ybcxt.top

[T12] Kotlin：解构声明
来源：http://vtw.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://pfj.shzxlz.cn

[T13] Kotlin：只读 Map
来源：http://piz.xylfe.cn

val m = mapOf("a" to 1)
来源：http://igx.yueranfly.top

[T14] Kotlin：循环
来源：http://kyc.sweek.top

for (i in 1..10) println(i)
来源：http://mzz.andypj.xyz

[T15] Kotlin：接口
来源：http://plo.zhixingplan.top

interface Shape { fun area(): Double }
来源：http://vjz.zycfv.cn

[T16] Swift：Hello World
来源：http://pbe.yuxming.cn

print("Hello")
来源：http://jfe.52xcode.cn

[T17] Swift：变量与常量
来源：http://lvo.zhiwuduotai.top

var a = 1;  let b = 2
来源：http://kpi.zhongyouzk.top

[T18] Swift：字符串插值
来源：http://mrl.ydjk.org.cn

"值: \(b)"
来源：http://wno.dashuyun.cn

[T19] Swift：可选绑定
来源：http://xke.dianchejie.cn

if let n = opt { print(n) }
来源：http://kja.yj20258888.top

[T20] Swift：数组操作
来源：http://xgz.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nnb.nanxinkj.top

[T21] Swift：遍历
来源：http://xqb.ydjk.org.cn

for x in a { print(x) }
来源：http://ead.xylfe.cn

[T22] Swift：字典
来源：http://rfl.chenjidiqi.icu

var d = ["a": 1];  d["b"] = 2
来源：http://bhe.fehbvm.com

[T23] Swift：函数
来源：http://gtu.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yef.zdqjudy.top

[T24] Swift：闭包
来源：http://all.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://yxf.ehwqpu.com

[T25] Swift：结构体
来源：http://xiy.316326.xyz

struct P { var x: Int }
来源：http://knq.daria6918.cn

[T26] Swift：类与重写
来源：http://pfm.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://vrt.xuanzx.com

[T27] Swift：错误处理
来源：http://pwu.yangfankeji.com

do { try f() } catch { print(error) }
来源：http://sau.nanxuanxn.top

[T28] Swift：枚举
来源：http://kml.nwbrower.top

enum Color { case red, green }
来源：http://zfp.aibaodan.cn


<!-- 参考信息 -->