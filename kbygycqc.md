代发 wailian999

echo $((1 + 2 * 3))
来源：http://pst.kuanghao11.cn

[R28] 浮点运算
来源：http://vbj.aibaodan.cn

echo "scale=2; 10/3" | bc
来源：http://wtu.yueranfly.top

[R29] 定义函数
来源：http://wmc.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yex.epnwcf.com

[R30] 函数返回状态码
来源：http://quh.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://brj.jlsjyb.cn

[R31] 局部变量
来源：http://wpn.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://soi.sysykeji.top

[R32] 参数个数校验
来源：http://xfx.sxryk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ppz.pycfn.com

[R33] 捕获错误并提示行号
来源：http://alu.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qiu.52xcode.cn

[R34] 退出时清理
来源：http://nkk.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kkh.aizwys.cn

[R35] 后台执行并等待
来源：http://cez.fehbvm.com

sleep 5 & pid=$!; wait "$pid"
来源：http://zuq.aizwys.cn

[R36] 并发执行多个任务
来源：http://ufv.xuanzx.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nwl.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://ile.zhixingplan.top

files=$(ls -1)
来源：http://qnx.mhx1999.top

[R38] 管道串联
来源：http://lqs.xingfuxueyuan.xyz

cat a.txt | grep -i error | wc -l
来源：http://meb.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://stk.smart0.xyz

cmd > out.log 2>&1
来源：http://vkb.jinqigfzy.top

[R40] 追加写日志
来源：http://lgr.yj20258888.top

echo "log" >> out.log
来源：http://lry.daria6918.cn

[R41] 丢弃输出
来源：http://ipy.andypj.xyz

cmd >/dev/null 2>&1
来源：http://gwv.iojbl.cn

[R42] 输入重定向
来源：http://vta.ehwqpu.com

wc -l < a.txt
来源：http://umj.sufxvd.cn

[R43] 按名字查找文件
来源：http://eox.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://jjo.haohaochexian.top

[R44] 按修改时间查找
来源：http://eup.hesvh.cn

find . -mtime -7 -type f
来源：http://fjm.zhixingplan.top

[R45] 批量删除
来源：http://xty.zhoulong.xyz

find . -name "*.tmp" -delete
来源：http://tsf.cheryme.top

[R46] 递归替换文件内容
来源：http://cex.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://odz.vehdjk.com

[R47] sed 单行替换
来源：http://slo.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bhe.jlsjyb.cn

[R48] awk 取指定列
来源：http://weq.hammf.cn

awk '{print $1, $3}' a.txt
来源：http://ldl.nanxinkj.top

[R49] awk 带条件
来源：http://cgj.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://csc.hongshengwenyu.top

[R50] awk 求和
来源：http://klb.snrcjt.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mdg.daxiang520.top

[R51] 排序去重取前几
来源：http://xja.snrcjt.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gcw.bbcook.cn

[R52] 统计行数
来源：http://sxw.yj20258.top

wc -l a.txt
来源：http://rou.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://xrs.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oog.zhongyouzk.top

[R54] 比较两个文件
来源：http://riw.guowangkeji.top

diff a.txt b.txt
来源：http://rdf.jlsjyb.cn

[R55] 压缩与解压
来源：http://hzz.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fnz.aibaodan.cn

[R56] 远程拷贝
来源：http://aew.jinghuilouyu.cn

scp file user@host:/path/
来源：http://dbh.chenlongwang.top

[R57] 远程执行命令
来源：http://vap.ydjk.org.cn

ssh user@host 'uptime'
来源：http://whp.shanyushiyangtech.top

[R58] 下载文件
来源：http://sfm.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://frf.hfpthk.cn

[R59] 发 POST JSON
来源：http://sab.zhengqikj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gxo.kuanghao11.cn

[R60] 只看 HTTP 状态码
来源：http://sun.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cbv.nanxinkj.top

[R61] 磁盘占用
来源：http://bfd.yuanzhike.top

df -h;  du -sh *
来源：http://irs.nwbrower.top

[R62] 找最占空间的文件
来源：http://zxl.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://qgp.birdmap.top

[R63] 内存与进程
来源：http://hoa.cqqwz.cn

free -h;  ps aux | grep nginx
来源：http://crd.fehbvm.com

[R64] 结束进程
来源：http://jdb.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://msm.yuanzhike.top

[R65] 查看端口占用
来源：http://nqr.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nay.hywenlv.cn

[R66] 定时任务
来源：http://ecm.bbcook.cn

crontab -e;  crontab -l
来源：http://zjz.chenlongwang.top

[R67] 生成随机十六进制串
来源：http://kgf.ydjk.org.cn

openssl rand -hex 16
来源：http://svj.zycfv.cn

[R68] 计算文件校验值
来源：http://syi.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://dgf.gogol.net.cn

[R69] 生成随机密码
来源：http://okh.cucudq.cn

head -c 16 /dev/urandom | base64
来源：http://hoh.ydzc1.top

[R70] 时间戳与互转
来源：http://llt.sysykeji.top

date +%s;  date -d @1700000000
来源：http://fwn.yanxiufei.cn

[R71] 日期格式化
来源：http://vzm.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://bah.yongpay.top

[R72] 等待端口就绪
来源：http://fxf.wangdashe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gdx.ivvv.top

[R73] 分割大日志
来源：http://wqx.guannengcc.top

split -l 1000 big.log part_
来源：http://kka.snrcjt.cn

[R74] 批量重命名
来源：http://fkm.ctjpmb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://drh.tarul.cn

[R75] 导出环境变量
来源：http://mli.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://abs.xylfe.cn

[R76] 使用临时文件
来源：http://fvv.ydzc1.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mrx.hesvh.cn

[R77] 读取用户输入
来源：http://pge.bjfxy.top

read -rp "请输入: " ans
来源：http://gtk.gzhubu.top

[R78] 交互式菜单
来源：http://zqw.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://sma.xylfe.cn

[R79] 解析命令行选项
来源：http://zwo.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bor.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://cll.nanxinkj.top

time ./run.sh
来源：http://ntr.wangdashe.top

================================================================================
来源：http://src.cucudq.cn

S. C / C++ 专题
来源：http://hsk.meibo888.top

================================================================================
来源：http://asn.jqgufenzy.top

[S01] C：Hello World
来源：http://gcu.aibaodan.cn

#include <stdio.h>
来源：http://yle.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://tew.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://dmk.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://egv.gaohongyu789.top

[S03] C：读入整数
来源：http://jum.smart0.xyz

int x; scanf("%d", &x);
来源：http://qly.hcnkem.com

[S04] C：字符串复制
来源：http://fsk.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rro.tianlin.xyz

[S05] C：字符串长度
来源：http://fuc.zhongyouzk.top

strlen(s)
来源：http://eyi.yueranfly.top

[S06] C：字符串比较
来源：http://tkm.cheryme.top

strcmp(a, b) == 0
来源：http://oqm.sxryk.cn

[S07] C：数组遍历求和
来源：http://mst.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ukk.dashuyun.cn

[S08] C：动态内存分配与释放
来源：http://vft.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tko.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://lma.haohaochexian.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ygm.bjfxy.top

[S10] C：指针与解引用
来源：http://gcj.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://poy.316326.xyz

[S11] C：逐行读文件
来源：http://cvi.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://mdc.cqqwz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yjc.nanxinkj.top

fclose(f);
来源：http://swj.gaohongyu789.top

[S12] C：写文件
来源：http://hlx.yanxiufei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://brz.52xcode.cn

[S13] C：宏定义
来源：http://poi.sjlbkw.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://czd.yanxiufei.cn

[S14] C：枚举
来源：http://dbn.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://vio.tarul.cn

[S15] C：类型转换
来源：http://ftp.wangshuangyany.cn

(double) a / b
来源：http://uno.gogol.net.cn

[S16] C：位操作置位
来源：http://lfe.daria6918.cn

x |= (1 << 3);
来源：http://vox.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://cbz.yueranfly.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ezl.yj20258888.top

[S18] C：命令行参数
来源：http://vpw.tian-w.cn

int main(int argc, char **argv)
来源：http://asd.jyoumei.cn

[S19] C：快速排序
来源：http://xzg.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://rid.xuanzx.com

[S20] C：二分查找
来源：http://yqr.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ajk.daxiang520.top

[S21] C：字符类别判断
来源：http://shx.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bjq.yuanzhike.top

[S22] C：字符串转数字
来源：http://yjs.yj202588.top

atoi("42");  strtod("3.14", NULL);
来源：http://gam.tianlin.xyz

[S23] C：随机数
来源：http://amm.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bzm.hysaishi.cn

[S24] C：获取本地时间
来源：http://rdw.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rqr.ydjk.org.cn

[S25] C：内存拷贝
来源：http://zvl.yuxming.cn

memcpy(dst, src, n);
来源：http://wln.mhx1999.top

[S26] C：内存清零
来源：http://ota.bjfxy.top

memset(a, 0, sizeof a);
来源：http://prv.yj202588.top

[S27] C：定义常量
来源：http://gqb.ppjwa.cn

const double PI = 3.14159;
来源：http://ymx.yangfankeji.com

[S28] C：静态变量
来源：http://biq.xinyue.icu

static int counter = 0;
来源：http://ptj.yongpay.top

[S29] C：变参函数
来源：http://jcg.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://laj.yj20258.top

[S30] C：头文件保护
来源：http://tyx.yuxming.cn

#ifndef X_H
来源：http://ntb.ydzc1.top

#define X_H
来源：http://yix.tarul.cn

#endif
来源：http://mes.xziqi.cn

[S31] C++：Hello World
来源：http://cyq.mhx1999.top

#include <iostream>
来源：http://rcg.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://mfu.shzxlz.cn

[S32] C++：字符串
来源：http://mxy.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://nxn.jinyuanbaomall.cn

[S33] C++：vector 增删
来源：http://kbn.mhx1999.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qzq.yfazqb.com

[S34] C++：遍历 vector
来源：http://mfa.aibaodan.cn

for (auto &x : v) { std::cout << x; }
来源：http://cuv.chenlongwang.top

[S35] C++：map
来源：http://zet.tianlin.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://naq.aizwys.cn

[S36] C++：unordered_map
来源：http://lfx.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cwx.hnqzz.top

[S37] C++：set
来源：http://ybb.vehdjk.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jtx.0kj1m.cn

[S38] C++：排序
来源：http://csm.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://upx.yuxming.cn

[S39] C++：自定义比较器排序
来源：http://hgb.0kj1m.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pmo.hnqzz.top

[S40] C++：查找元素
来源：http://fgk.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rez.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://fwz.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hnh.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://ymp.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://zin.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://ydr.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://ksx.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://vnn.guannengcc.top

void inc(int &x) { ++x; }
来源：http://lfa.gotoacloud.top

[S45] C++：lambda
来源：http://kqj.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://nqq.xziqi.cn

[S46] C++：函数模板
来源：http://nhg.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vim.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://esk.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jyr.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://org.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://jcf.xylfe.cn

while (std::getline(in, line)) { }
来源：http://qir.fehbvm.com

[S49] C++：写文件
来源：http://imn.fzhhl.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vao.daria6918.cn

[S50] C++：格式化数字
来源：http://hvh.snrcjt.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qex.fehbvm.com

[S51] C++：显式类型转换
来源：http://eey.yvedp.cn

static_cast<double>(a) / b
来源：http://nef.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://dcm.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://qol.chenlongwang.top

[S53] C++：移动语义
来源：http://zip.bbcook.cn

std::vector<int> w = std::move(v);
来源：http://bnd.uphjek.com

[S54] C++：异常处理
来源：http://mzf.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qpk.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://zci.xziqi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mpd.zhijiandao.cn

[S56] C++：optional
来源：http://smy.yangfankeji.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vsr.hammf.cn

[S57] C++：编译期常量
来源：http://bfk.hfpthk.cn

constexpr int N = 10;
来源：http://wpr.xinyue.icu

[S58] C++：命名空间
来源：http://ifr.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://ble.yueranfly.top

[S59] C++：静态断言
来源：http://zzb.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ppc.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://ojl.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://evj.ivvv.top

================================================================================
来源：http://emv.mhx1999.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wgi.iojbl.cn

================================================================================
来源：http://grj.gaohongyu789.top

[T01] Kotlin：Hello World
来源：http://dsf.shzxlz.cn

println("Hello")
来源：http://zyp.yvedp.cn

[T02] Kotlin：变量
来源：http://auc.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cmr.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://wcj.jiagoushi.top

"值: $b"
来源：http://ndx.zycfv.cn

[T04] Kotlin：空安全
来源：http://mcd.yfazqb.com

val n: String? = null;  n?.length
来源：http://lbt.daxiang520.top

[T05] Kotlin：when 表达式
来源：http://ccb.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rzg.ybcxt.top

[T06] Kotlin：集合映射
来源：http://taj.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cfy.zhoulong.xyz

[T07] Kotlin：集合过滤
来源：http://awl.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ebt.uphjek.com

[T08] Kotlin：数据类
来源：http://hbf.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://mvv.birdmap.top

[T09] Kotlin：扩展函数
来源：http://cdv.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://qko.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://hle.havefunace.top

fun greet(name: String = "World") = "Hi $name"
来源：http://eml.yfazqb.com

[T11] Kotlin：协程
来源：http://hbd.aizwys.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tui.yonumen.top

[T12] Kotlin：解构声明
来源：http://byi.9152youxi.cn

val (a, b) = Pair(1, 2)
来源：http://zjc.ivvv.top

[T13] Kotlin：只读 Map
来源：http://sef.xziqi.cn

val m = mapOf("a" to 1)
来源：http://rxh.shanyushiyangkeji.top

[T14] Kotlin：循环
来源：http://kxd.0kj1m.cn

for (i in 1..10) println(i)
来源：http://lrn.yj202588.top

[T15] Kotlin：接口
来源：http://gzk.andypj.xyz

interface Shape { fun area(): Double }
来源：http://tty.aibaodan.cn

[T16] Swift：Hello World
来源：http://paf.xingfuxueyuan.xyz

print("Hello")
来源：http://baq.cheryme.top

[T17] Swift：变量与常量
来源：http://zby.ybcxt.top

var a = 1;  let b = 2
来源：http://eeb.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://tbr.vehdjk.com

"值: \(b)"
来源：http://fdg.jqgufenzy.top

[T19] Swift：可选绑定
来源：http://ynr.aibaodan.cn

if let n = opt { print(n) }
来源：http://mnc.meibo888.top

[T20] Swift：数组操作
来源：http://ilm.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://qxs.cqqwz.cn

[T21] Swift：遍历
来源：http://epm.aizwys.cn

for x in a { print(x) }
来源：http://cxu.pengpengdd.cyou

[T22] Swift：字典
来源：http://yvy.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://cul.wangdashe.top

[T23] Swift：函数
来源：http://ffk.tianlin.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lny.xinyue.icu

[T24] Swift：闭包
来源：http://jfs.hammf.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://djx.jqgufenzy.top

[T25] Swift：结构体
来源：http://ytw.quarkkingdee.top

struct P { var x: Int }
来源：http://rgi.sweek.top

[T26] Swift：类与重写
来源：http://wyn.yongpay.top

class A: Base { override func f() {} }
来源：http://oay.chenzaomai.com

[T27] Swift：错误处理
来源：http://kzc.shanyushiyangtech.top

do { try f() } catch { print(error) }
来源：http://yly.cqqwz.cn

[T28] Swift：枚举
来源：http://hqk.zhijiandao.cn

enum Color { case red, green }
来源：http://hvz.haohaochexian.top

[T29] Swift：guard 提前返回
来源：http://jcf.havefunace.top

guard let x = opt else { return }
来源：http://duj.cheryme.top

[T30] Swift：协议
来源：http://lji.meibo888.top

protocol Shape { func area() -> Double }
来源：http://mez.shanyushiyangkeji.top


<!-- 参考信息 -->