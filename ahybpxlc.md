代发 wailian999

echo $((1 + 2 * 3))
来源：http://jsf.pycfn.com

[R28] 浮点运算
来源：http://gxc.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://kiw.zdbjq.cn

[R29] 定义函数
来源：http://bvc.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://maj.xuetiantiany.cn

[R30] 函数返回状态码
来源：http://bwy.fanxiaobao.xyz

f() { return 0; }; f || echo "失败了"
来源：http://tle.zhijiandao.cn

[R31] 局部变量
来源：http://bhj.zdbjq.cn

f() { local x=1; echo "$x"; }
来源：http://gxx.wangshuangyany.cn

[R32] 参数个数校验
来源：http://gqb.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fxx.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://lwv.xingfuxueyuan.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xqq.havefunace.top

[R34] 退出时清理
来源：http://znf.yj20258.top

trap 'rm -f "$tmp"' EXIT
来源：http://axh.yj202588.top

[R35] 后台执行并等待
来源：http://jym.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jml.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://tkr.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wrp.ybcxt.top

[R37] 把输出赋给变量
来源：http://eko.hcnkem.com

files=$(ls -1)
来源：http://vwg.jqgfzy.top

[R38] 管道串联
来源：http://bwg.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://zko.hnqzz.top

[R39] 重定向标准输出与错误
来源：http://jii.zhengqikj.top

cmd > out.log 2>&1
来源：http://fsi.tianlin.xyz

[R40] 追加写日志
来源：http://ezg.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://msu.vqdsnc.cn

[R41] 丢弃输出
来源：http://zqi.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://uym.zhijiandao.cn

[R42] 输入重定向
来源：http://oti.hesvh.cn

wc -l < a.txt
来源：http://fyl.yj20258.top

[R43] 按名字查找文件
来源：http://ysv.pycfn.com

find . -name "*.log" -type f
来源：http://qex.daria6918.cn

[R44] 按修改时间查找
来源：http://pqv.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://zvw.feifeiyinyue.top

[R45] 批量删除
来源：http://cax.jinqigfzy.top

find . -name "*.tmp" -delete
来源：http://xwd.c1oappe.top

[R46] 递归替换文件内容
来源：http://oqf.tarul.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mpl.zhijiandao.cn

[R47] sed 单行替换
来源：http://fde.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jiy.fktsv.cn

[R48] awk 取指定列
来源：http://faf.jqgufenzy.top

awk '{print $1, $3}' a.txt
来源：http://kco.hongshengwenyu.top

[R49] awk 带条件
来源：http://ilc.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lyo.0kj1m.cn

[R50] awk 求和
来源：http://nyw.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vpz.pycfn.com

[R51] 排序去重取前几
来源：http://hds.zhengqikj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://oss.jqgufenzy.top

[R52] 统计行数
来源：http://ntn.xinyue.icu

wc -l a.txt
来源：http://hdn.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://nba.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ysp.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://mmb.yfazqb.com

diff a.txt b.txt
来源：http://rdo.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://qpb.sweek.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xys.cucudq.cn

[R56] 远程拷贝
来源：http://epn.iojbl.cn

scp file user@host:/path/
来源：http://ijx.52xcode.cn

[R57] 远程执行命令
来源：http://ngg.yanxiufei.cn

ssh user@host 'uptime'
来源：http://krt.smart0.xyz

[R58] 下载文件
来源：http://sqq.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ypw.jinqigufen.top

[R59] 发 POST JSON
来源：http://wgp.fengsongda.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bam.smart0.xyz

[R60] 只看 HTTP 状态码
来源：http://fns.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zvf.yj202588.top

[R61] 磁盘占用
来源：http://cbd.sysykeji.top

df -h;  du -sh *
来源：http://vdl.jlsjyb.cn

[R62] 找最占空间的文件
来源：http://qdq.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://aiu.zdbjq.cn

[R63] 内存与进程
来源：http://gvk.yfazqb.com

free -h;  ps aux | grep nginx
来源：http://bzm.bjfxy.top

[R64] 结束进程
来源：http://yts.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://cbr.jinghuilouyu.cn

[R65] 查看端口占用
来源：http://amn.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dci.guannengcc.top

[R66] 定时任务
来源：http://vqe.nanxuanxn.top

crontab -e;  crontab -l
来源：http://bdg.bjfxy.top

[R67] 生成随机十六进制串
来源：http://ssj.zhengqikj.top

openssl rand -hex 16
来源：http://fyh.cheryme.top

[R68] 计算文件校验值
来源：http://mzj.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jny.quarkkingdee.top

[R69] 生成随机密码
来源：http://fww.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://cnh.cdnleiting.top

[R70] 时间戳与互转
来源：http://qja.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://qdu.ywan-chungtsiang.top

[R71] 日期格式化
来源：http://hhv.gzhubu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dvg.cucudq.cn

[R72] 等待端口就绪
来源：http://qfq.xingfuxueyuan.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://pvs.feifeiyinyue.top

[R73] 分割大日志
来源：http://bhd.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://tqz.jiagoushi.top

[R74] 批量重命名
来源：http://ext.yj20258.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jhq.jinqigufen.top

[R75] 导出环境变量
来源：http://zii.yuxming.cn

export PATH="$HOME/bin:$PATH"
来源：http://hpy.ctjpmb.com

[R76] 使用临时文件
来源：http://ued.xuetiantiany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://itd.uphjek.com

[R77] 读取用户输入
来源：http://keo.bbcook.cn

read -rp "请输入: " ans
来源：http://ejc.fanxiaobao.xyz

[R78] 交互式菜单
来源：http://nsa.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kko.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://qyf.guannengcc.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tud.haohaochexian.top

[R80] 查看脚本执行耗时
来源：http://iee.sjlbkw.cn

time ./run.sh
来源：http://wyc.zhixingplan.top

================================================================================
来源：http://qrr.bjfxy.top

S. C / C++ 专题
来源：http://gwc.yvedp.cn

================================================================================
来源：http://fmg.yueranfly.top

[S01] C：Hello World
来源：http://jqq.havefunace.top

#include <stdio.h>
来源：http://cuv.hongshengwenyu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vtb.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://ucv.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://fga.quarkkingdee.top

[S03] C：读入整数
来源：http://cis.aibaodan.cn

int x; scanf("%d", &x);
来源：http://yhf.cashguo.top

[S04] C：字符串复制
来源：http://yxf.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://nrh.aibaodan.cn

[S05] C：字符串长度
来源：http://ncw.kuanghao11.cn

strlen(s)
来源：http://oxq.tanke756.top

[S06] C：字符串比较
来源：http://ffs.haohaochexian.top

strcmp(a, b) == 0
来源：http://wbx.ctjpmb.com

[S07] C：数组遍历求和
来源：http://lof.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pxp.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://ngl.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uvp.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://kah.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pex.jinqigfzy.top

[S10] C：指针与解引用
来源：http://kjz.316326.xyz

int *p = &a;  *p = 5;
来源：http://uqa.gotoacloud.top

[S11] C：逐行读文件
来源：http://qli.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://pyr.hongshengwenyu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ljq.kuanghao11.cn

fclose(f);
来源：http://coq.cqqwz.cn

[S12] C：写文件
来源：http://bjh.chenjidiqi.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zyy.zhoulong.xyz

[S13] C：宏定义
来源：http://xau.chenzaomai.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gko.shangyingyoupin.top

[S14] C：枚举
来源：http://wos.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://wip.fzhhl.top

[S15] C：类型转换
来源：http://cfv.fzhhl.top

(double) a / b
来源：http://gfx.jqgfzy.top

[S16] C：位操作置位
来源：http://afs.hnqzz.top

x |= (1 << 3);
来源：http://izi.nwbrower.top

[S17] C：安全拼接字符串
来源：http://kab.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vbr.jyoumei.cn

[S18] C：命令行参数
来源：http://noy.wangshuangyany.cn

int main(int argc, char **argv)
来源：http://tod.hfpthk.cn

[S19] C：快速排序
来源：http://oti.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cmt.nanxuanxn.top

[S20] C：二分查找
来源：http://buc.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bsq.cashguo.top

[S21] C：字符类别判断
来源：http://lcy.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jda.fktsv.cn

[S22] C：字符串转数字
来源：http://cnw.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://tio.jinqigfzy.top

[S23] C：随机数
来源：http://gtm.svipenyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zjm.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://jsz.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jck.ydzc1.top

[S25] C：内存拷贝
来源：http://vzt.yj20258.top

memcpy(dst, src, n);
来源：http://pfd.quarkkingdee.top

[S26] C：内存清零
来源：http://pmq.hnxiangtu.top

memset(a, 0, sizeof a);
来源：http://ndg.redwolf501.top

[S27] C：定义常量
来源：http://eih.zhixingplan.top

const double PI = 3.14159;
来源：http://pyo.jinghuilouyu.cn

[S28] C：静态变量
来源：http://zax.jiagoushi.top

static int counter = 0;
来源：http://ugj.hnxiangtu.top

[S29] C：变参函数
来源：http://isn.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lwd.sxryk.cn

[S30] C：头文件保护
来源：http://ihj.fehbvm.com

#ifndef X_H
来源：http://kjn.zhijiandao.cn

#define X_H
来源：http://uld.pengpengdd.cyou

#endif
来源：http://rku.havefunace.top

[S31] C++：Hello World
来源：http://unl.jinghuilouyu.cn

#include <iostream>
来源：http://hse.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://ecr.tian-w.cn

[S32] C++：字符串
来源：http://fmk.pycfn.com

std::string s = "hi";  s += "!";
来源：http://iup.fanxiaobao.xyz

[S33] C++：vector 增删
来源：http://wuz.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mzc.jqgfzy.top

[S34] C++：遍历 vector
来源：http://lqk.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://nvt.shzxlz.cn

[S35] C++：map
来源：http://jow.yuxming.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kvi.jyoumei.cn

[S36] C++：unordered_map
来源：http://isc.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lvp.yueranfly.top

[S37] C++：set
来源：http://dlh.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xrm.hcnkem.com

[S38] C++：排序
来源：http://ilf.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://dgb.kuanghao11.cn

[S39] C++：自定义比较器排序
来源：http://ezf.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qcj.havefunace.top

[S40] C++：查找元素
来源：http://fgg.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gts.yvedp.cn

[S41] C++：类与构造函数
来源：http://ekw.svipenyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xqo.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://vky.zhongyouzk.top

class B : public Base { public: void f() override {} };
来源：http://vxd.yfazqb.com

[S43] C++：智能指针
来源：http://nxh.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://izc.yj202588.top

[S44] C++：引用传参
来源：http://ueg.sxryk.cn

void inc(int &x) { ++x; }
来源：http://xdy.chenlongwang.top

[S45] C++：lambda
来源：http://vhv.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://ulz.bjfxy.top

[S46] C++：函数模板
来源：http://kec.sxryk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ykb.jqgfzy.top

[S47] C++：结构化绑定遍历
来源：http://glh.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sau.zdqjudy.top

[S48] C++：逐行读文件
来源：http://alp.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://btf.bbcook.cn

while (std::getline(in, line)) { }
来源：http://kby.mhx1999.top

[S49] C++：写文件
来源：http://qeh.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mau.jinqigfzy.top

[S50] C++：格式化数字
来源：http://kmo.zhixingplan.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xab.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://ngy.shuidangran.top

static_cast<double>(a) / b
来源：http://wkr.uphjek.com

[S52] C++：const 与 noexcept
来源：http://xxm.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://cvb.xuanzx.com

[S53] C++：移动语义
来源：http://mfs.xziqi.cn

std::vector<int> w = std::move(v);
来源：http://hul.jqgfzy.top

[S54] C++：异常处理
来源：http://mzh.svipenyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://roe.meibo888.top

[S55] C++：结构化绑定
来源：http://hdo.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vzg.chenjidiqi.icu

[S56] C++：optional
来源：http://rvg.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jhz.gzhubu.top

[S57] C++：编译期常量
来源：http://plq.gogol.net.cn

constexpr int N = 10;
来源：http://gyz.yueranfly.top

[S58] C++：命名空间
来源：http://xit.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://onu.hywenlv.cn

[S59] C++：静态断言
来源：http://pvu.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ifa.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://nfn.nanxinkj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oen.zdbjq.cn

================================================================================
来源：http://kli.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jbg.sxryk.cn

================================================================================
来源：http://gfd.zhaomingkeji.xyz

[T01] Kotlin：Hello World
来源：http://onv.cashguo.top

println("Hello")
来源：http://hip.aibaodan.cn

[T02] Kotlin：变量
来源：http://eqa.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kto.cheryme.top

[T03] Kotlin：字符串模板
来源：http://bhl.chenlongwang.top

"值: $b"
来源：http://awh.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://znt.jyoumei.cn

val n: String? = null;  n?.length
来源：http://qwd.hongshengwenyu.top

[T05] Kotlin：when 表达式
来源：http://yyx.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aaw.bbcook.cn

[T06] Kotlin：集合映射
来源：http://ffa.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ztu.yj20258888.top

[T07] Kotlin：集合过滤
来源：http://nbq.xuetiantiany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mhr.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://oty.yuxming.cn

data class User(val name: String, val age: Int)
来源：http://rhv.ybcxt.top

[T09] Kotlin：扩展函数
来源：http://rzs.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://qpo.xuanzx.com

[T10] Kotlin：默认参数
来源：http://der.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pmr.cashguo.top

[T11] Kotlin：协程
来源：http://cfj.hysaishi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tcr.cdnleiting.top

[T12] Kotlin：解构声明
来源：http://eqb.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://ele.shanyushiyangkeji.top

[T13] Kotlin：只读 Map
来源：http://ygq.bbcook.cn

val m = mapOf("a" to 1)
来源：http://wla.redwolf501.top

[T14] Kotlin：循环
来源：http://uvs.cdnleiting.top

for (i in 1..10) println(i)
来源：http://vfg.redwolf501.top

[T15] Kotlin：接口
来源：http://qth.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://wbr.nwbrower.top

[T16] Swift：Hello World
来源：http://bta.zhongyouzk.top

print("Hello")
来源：http://afy.jianghu66.top

[T17] Swift：变量与常量
来源：http://eaa.hcnkem.com

var a = 1;  let b = 2
来源：http://lhk.fktsv.cn

[T18] Swift：字符串插值
来源：http://qal.chenjidiqi.icu

"值: \(b)"
来源：http://veb.bjfxy.top

[T19] Swift：可选绑定
来源：http://uak.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://ocd.yuxming.cn

[T20] Swift：数组操作
来源：http://flo.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://xgc.zhongyouzk.top

[T21] Swift：遍历
来源：http://adx.tian-w.cn

for x in a { print(x) }
来源：http://nin.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://fwu.epnwcf.com

var d = ["a": 1];  d["b"] = 2
来源：http://jdu.daria6918.cn

[T23] Swift：函数
来源：http://hna.tarul.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fee.ctjpmb.com

[T24] Swift：闭包
来源：http://bsg.vehdjk.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://wpq.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://ybw.jinghuilouyu.cn

struct P { var x: Int }
来源：http://rqm.xuetiantiany.cn

[T26] Swift：类与重写
来源：http://uex.wangshuangyany.cn

class A: Base { override func f() {} }
来源：http://qhh.fengsongda.top

[T27] Swift：错误处理
来源：http://egh.jyoumei.cn

do { try f() } catch { print(error) }
来源：http://vky.yangfankeji.com

[T28] Swift：枚举
来源：http://dln.hongshengwenyu.top

enum Color { case red, green }
来源：http://znd.hysaishi.cn

[T29] Swift：guard 提前返回
来源：http://tyl.gaohongyu789.top

guard let x = opt else { return }
来源：http://xjo.yfazqb.com

[T30] Swift：协议
来源：http://fwj.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://hht.tianlin.xyz


<!-- 参考信息 -->