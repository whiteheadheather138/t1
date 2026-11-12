代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ami.pycfn.com

[R24] 大小写转换
来源：http://nkg.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://efu.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://vuf.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sbb.yfazqb.com

[R26] 命令替换
来源：http://jvn.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://vfz.birdmap.top

[R27] 算术展开
来源：http://hjd.sweek.top

echo $((1 + 2 * 3))
来源：http://pxg.nanxinkj.top

[R28] 浮点运算
来源：http://zsd.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://sno.0kj1m.cn

[R29] 定义函数
来源：http://kxb.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wws.quarkkingdee.top

[R30] 函数返回状态码
来源：http://qka.haohaochexian.top

f() { return 0; }; f || echo "失败了"
来源：http://iui.shzxlz.cn

[R31] 局部变量
来源：http://ntx.hesvh.cn

f() { local x=1; echo "$x"; }
来源：http://ivo.snrcjt.cn

[R32] 参数个数校验
来源：http://cry.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gdk.pycfn.com

[R33] 捕获错误并提示行号
来源：http://nzv.guannengcc.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zjs.hysaishi.cn

[R34] 退出时清理
来源：http://pji.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://xmm.daxiang520.top

[R35] 后台执行并等待
来源：http://ezs.fengsongda.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rmq.quarkkingdee.top

[R36] 并发执行多个任务
来源：http://ckg.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uvx.nanxuanxn.top

[R37] 把输出赋给变量
来源：http://thq.ydzc1.top

files=$(ls -1)
来源：http://kko.redwolf501.top

[R38] 管道串联
来源：http://ezv.yuanzhike.top

cat a.txt | grep -i error | wc -l
来源：http://jfi.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://zyr.smart0.xyz

cmd > out.log 2>&1
来源：http://qnx.gaohongyu789.top

[R40] 追加写日志
来源：http://hdi.jianghu66.top

echo "log" >> out.log
来源：http://dxs.wangshuangyany.cn

[R41] 丢弃输出
来源：http://hvi.tarul.cn

cmd >/dev/null 2>&1
来源：http://jpc.gaohongyu789.top

[R42] 输入重定向
来源：http://hsz.jinyuanbaomall.cn

wc -l < a.txt
来源：http://crk.zhoulong.xyz

[R43] 按名字查找文件
来源：http://nih.shangyingyoupin.top

find . -name "*.log" -type f
来源：http://kai.shuidangran.top

[R44] 按修改时间查找
来源：http://ikz.gaohongyu789.top

find . -mtime -7 -type f
来源：http://kps.snrcjt.cn

[R45] 批量删除
来源：http://ctj.hesvh.cn

find . -name "*.tmp" -delete
来源：http://jep.jiagoushi.top

[R46] 递归替换文件内容
来源：http://wfw.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ffq.guowangkeji.top

[R47] sed 单行替换
来源：http://rwk.birdmap.top

sed -i 's/foo/bar/g' a.txt
来源：http://byd.xuetiantiany.cn

[R48] awk 取指定列
来源：http://iun.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://kli.sxryk.cn

[R49] awk 带条件
来源：http://try.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nim.fengsongda.top

[R50] awk 求和
来源：http://irg.yueranfly.top

awk '{s += $2} END {print s}' a.txt
来源：http://vng.ybcxt.top

[R51] 排序去重取前几
来源：http://cpj.bbcook.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kmu.zycfv.cn

[R52] 统计行数
来源：http://ssl.9152youxi.cn

wc -l a.txt
来源：http://lbs.52xcode.cn

[R53] 查看文件头与实时尾
来源：http://uiw.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ydn.yfazqb.com

[R54] 比较两个文件
来源：http://dxv.jianghu66.top

diff a.txt b.txt
来源：http://jts.hnqzz.top

[R55] 压缩与解压
来源：http://dao.daxiang520.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lek.xziqi.cn

[R56] 远程拷贝
来源：http://nna.yfazqb.com

scp file user@host:/path/
来源：http://oag.aizwys.cn

[R57] 远程执行命令
来源：http://mte.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://xtb.ppjwa.cn

[R58] 下载文件
来源：http://jrd.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://che.zycfv.cn

[R59] 发 POST JSON
来源：http://nlj.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cdd.nwbrower.top

[R60] 只看 HTTP 状态码
来源：http://wcq.52xcode.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bea.bjfxy.top

[R61] 磁盘占用
来源：http://aba.gaohongyu789.top

df -h;  du -sh *
来源：http://abz.yfazqb.com

[R62] 找最占空间的文件
来源：http://xfy.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://brj.zdqjudy.top

[R63] 内存与进程
来源：http://whb.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://zfu.gaohongyu789.top

[R64] 结束进程
来源：http://aup.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://nku.ydzc1.top

[R65] 查看端口占用
来源：http://nmh.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dnm.jianghu66.top

[R66] 定时任务
来源：http://rpu.nwbrower.top

crontab -e;  crontab -l
来源：http://vjk.wangdashe.top

[R67] 生成随机十六进制串
来源：http://qgc.pengpengdd.cyou

openssl rand -hex 16
来源：http://bkv.yuanzhike.top

[R68] 计算文件校验值
来源：http://rfl.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mzl.hnxiangtu.top

[R69] 生成随机密码
来源：http://nim.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://bdn.birdmap.top

[R70] 时间戳与互转
来源：http://hkf.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://vqf.birdmap.top

[R71] 日期格式化
来源：http://yxm.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://krp.mhx1999.top

[R72] 等待端口就绪
来源：http://yzb.shanyushiyangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cuz.daria6918.cn

[R73] 分割大日志
来源：http://jrr.xylfe.cn

split -l 1000 big.log part_
来源：http://rkf.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://ocp.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ofo.fktsv.cn

[R75] 导出环境变量
来源：http://lzq.shanyushiyangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://ngu.epnwcf.com

[R76] 使用临时文件
来源：http://gjo.yuanzhike.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ufy.quarkkingdee.top

[R77] 读取用户输入
来源：http://hyj.xinyue.icu

read -rp "请输入: " ans
来源：http://xrc.hesvh.cn

[R78] 交互式菜单
来源：http://zcu.gaohongyu789.top

select opt in a b c; do echo "$opt"; break; done
来源：http://voz.yj20258888.top

[R79] 解析命令行选项
来源：http://gkk.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nzu.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://bvs.fanxiaobao.xyz

time ./run.sh
来源：http://dyc.nanxuanxn.top

================================================================================
来源：http://srv.yuxming.cn

S. C / C++ 专题
来源：http://mze.quarkkingdee.top

================================================================================
来源：http://ztc.dashuyun.cn

[S01] C：Hello World
来源：http://pzm.fanxiaobao.xyz

#include <stdio.h>
来源：http://cly.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ydg.yvedp.cn

[S02] C：变量与格式化输出
来源：http://vwb.jqgufenzy.top

int a = 10; printf("%d\n", a);
来源：http://sag.ydzc1.top

[S03] C：读入整数
来源：http://rtq.chenlongwang.top

int x; scanf("%d", &x);
来源：http://scg.nanxuanxn.top

[S04] C：字符串复制
来源：http://oho.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://pbu.316326.xyz

[S05] C：字符串长度
来源：http://kgi.fktsv.cn

strlen(s)
来源：http://wdm.bbcook.cn

[S06] C：字符串比较
来源：http://fks.cucudq.cn

strcmp(a, b) == 0
来源：http://obn.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://yhp.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iuf.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://muj.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://woo.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://ajl.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ygu.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://jmj.mhx1999.top

int *p = &a;  *p = 5;
来源：http://fjw.sxryk.cn

[S11] C：逐行读文件
来源：http://noc.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://zbr.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wbf.nwbrower.top

fclose(f);
来源：http://yxv.aibaodan.cn

[S12] C：写文件
来源：http://npu.hnqzz.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vrf.xziqi.cn

[S13] C：宏定义
来源：http://sqc.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uzi.c1oappe.top

[S14] C：枚举
来源：http://iqj.hesvh.cn

enum Color { RED, GREEN, BLUE };
来源：http://ieh.meibo888.top

[S15] C：类型转换
来源：http://nux.xinyue.icu

(double) a / b
来源：http://iqt.tarul.cn

[S16] C：位操作置位
来源：http://kfw.shzxlz.cn

x |= (1 << 3);
来源：http://tqj.svipenyu.cn

[S17] C：安全拼接字符串
来源：http://lgg.hnxiangtu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dlf.zdqjudy.top

[S18] C：命令行参数
来源：http://kfq.fzhhl.top

int main(int argc, char **argv)
来源：http://kkn.ehwqpu.com

[S19] C：快速排序
来源：http://lhx.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jcw.ivvv.top

[S20] C：二分查找
来源：http://lrj.ivvv.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xqq.ydzc1.top

[S21] C：字符类别判断
来源：http://oqd.zhiwuduotai.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cjg.jyoumei.cn

[S22] C：字符串转数字
来源：http://mqy.hfpthk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rul.ybcxt.top

[S23] C：随机数
来源：http://bcz.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nmg.jyoumei.cn

[S24] C：获取本地时间
来源：http://uhe.fanxiaobao.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://grq.hcnkem.com

[S25] C：内存拷贝
来源：http://pvh.hysaishi.cn

memcpy(dst, src, n);
来源：http://ijo.epnwcf.com

[S26] C：内存清零
来源：http://nck.ywan-chungtsiang.top

memset(a, 0, sizeof a);
来源：http://nhg.yfazqb.com

[S27] C：定义常量
来源：http://xzb.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://tcn.tanke756.top

[S28] C：静态变量
来源：http://urp.snrcjt.cn

static int counter = 0;
来源：http://dlu.sxryk.cn

[S29] C：变参函数
来源：http://xcf.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cro.jlsjyb.cn

[S30] C：头文件保护
来源：http://gjt.tanke756.top

#ifndef X_H
来源：http://zyj.andypj.xyz

#define X_H
来源：http://vnp.ydzc1.top

#endif
来源：http://sac.yuanzhike.top

[S31] C++：Hello World
来源：http://sos.yangfankeji.com

#include <iostream>
来源：http://pqt.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://awg.cucudq.cn

[S32] C++：字符串
来源：http://bwf.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://phh.zhoulong.xyz

[S33] C++：vector 增删
来源：http://ewy.yueranfly.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tkx.yfazqb.com

[S34] C++：遍历 vector
来源：http://vvm.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://kxe.jyoumei.cn

[S35] C++：map
来源：http://kpn.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kwn.jiagoushi.top

[S36] C++：unordered_map
来源：http://pph.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qvy.cucudq.cn

[S37] C++：set
来源：http://bjy.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hln.tanke756.top

[S38] C++：排序
来源：http://wbf.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://dty.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://sdq.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://epr.hcnkem.com

[S40] C++：查找元素
来源：http://ifv.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://udd.yj20258888.top

[S41] C++：类与构造函数
来源：http://syi.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nai.zhijiandao.cn

[S42] C++：继承与虚函数
来源：http://qlx.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://zhr.zhijiandao.cn

[S43] C++：智能指针
来源：http://isb.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://leh.nanxinkj.top

[S44] C++：引用传参
来源：http://xgw.sxryk.cn

void inc(int &x) { ++x; }
来源：http://bqd.cashguo.top

[S45] C++：lambda
来源：http://afn.yj20258888.top

auto add = [](int a, int b) { return a + b; };
来源：http://qbj.zhoulong.xyz

[S46] C++：函数模板
来源：http://muc.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://grb.cucudq.cn

[S47] C++：结构化绑定遍历
来源：http://bqk.hcnkem.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lyq.hfpthk.cn

[S48] C++：逐行读文件
来源：http://eqk.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://lgv.jianghu66.top

while (std::getline(in, line)) { }
来源：http://kux.mhx1999.top

[S49] C++：写文件
来源：http://dak.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lwt.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://wvg.zhengqikj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nfh.gzhubu.top

[S51] C++：显式类型转换
来源：http://qkm.wangdashe.top

static_cast<double>(a) / b
来源：http://ydc.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://qji.yongpay.top

int size() const noexcept { return n_; }
来源：http://hzy.cdnleiting.top

[S53] C++：移动语义
来源：http://kfx.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://njv.fanxiaobao.xyz

[S54] C++：异常处理
来源：http://lbp.daria6918.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cki.hnqzz.top

[S55] C++：结构化绑定
来源：http://lie.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://exg.zycfv.cn

[S56] C++：optional
来源：http://gaw.zdqjudy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://htb.jqgufenzy.top

[S57] C++：编译期常量
来源：http://odg.meibo888.top

constexpr int N = 10;
来源：http://ifm.daria6918.cn

[S58] C++：命名空间
来源：http://xfa.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://yfy.yfazqb.com

[S59] C++：静态断言
来源：http://cfs.havefunace.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eoz.dianchejie.cn

[S60] C++：遍历并删除元素
来源：http://cff.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tcx.bjfxy.top

================================================================================
来源：http://ovn.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://abu.ppjwa.cn

================================================================================
来源：http://zic.ehwqpu.com

[T01] Kotlin：Hello World
来源：http://ipo.xuetiantiany.cn

println("Hello")
来源：http://xxw.cashguo.top

[T02] Kotlin：变量
来源：http://ajp.mhx1999.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kqt.kuanghao11.cn

[T03] Kotlin：字符串模板
来源：http://uvs.gzhubu.top

"值: $b"
来源：http://qcv.zdbjq.cn

[T04] Kotlin：空安全
来源：http://uys.dashuyun.cn

val n: String? = null;  n?.length
来源：http://sua.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://kbn.vehdjk.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vnq.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://aal.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yql.birdmap.top

[T07] Kotlin：集合过滤
来源：http://cav.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ehd.9152youxi.cn

[T08] Kotlin：数据类
来源：http://ksc.pengpengdd.cyou

data class User(val name: String, val age: Int)
来源：http://mvl.gzhubu.top

[T09] Kotlin：扩展函数
来源：http://ror.316326.xyz

fun String.exclaim() = this + "!"
来源：http://rui.uphjek.com

[T10] Kotlin：默认参数
来源：http://ykt.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://buj.sweek.top

[T11] Kotlin：协程
来源：http://vdy.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zry.gzhubu.top

[T12] Kotlin：解构声明
来源：http://rwk.smart0.xyz

val (a, b) = Pair(1, 2)
来源：http://vce.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://cfc.cheryme.top

val m = mapOf("a" to 1)
来源：http://dxb.shanyushiyangkeji.top

[T14] Kotlin：循环
来源：http://pdl.tian-w.cn

for (i in 1..10) println(i)
来源：http://orq.0kj1m.cn

[T15] Kotlin：接口
来源：http://frz.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://jrb.yj20258.top

[T16] Swift：Hello World
来源：http://kgq.vehdjk.com

print("Hello")
来源：http://xvf.ppjwa.cn

[T17] Swift：变量与常量
来源：http://afu.xuanzx.com

var a = 1;  let b = 2
来源：http://lag.cheryme.top

[T18] Swift：字符串插值
来源：http://jup.sysykeji.top

"值: \(b)"
来源：http://jgb.fehbvm.com

[T19] Swift：可选绑定
来源：http://nzr.meibo888.top

if let n = opt { print(n) }
来源：http://dxw.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://opk.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://prj.hywenlv.cn

[T21] Swift：遍历
来源：http://rew.havefunace.top

for x in a { print(x) }
来源：http://nqs.nwbrower.top

[T22] Swift：字典
来源：http://xph.shuidangran.top

var d = ["a": 1];  d["b"] = 2
来源：http://vat.hammf.cn

[T23] Swift：函数
来源：http://mbh.tarul.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pbr.zhixingplan.top

[T24] Swift：闭包
来源：http://nhd.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lnu.hnqzz.top

[T25] Swift：结构体
来源：http://ace.guannengcc.top

struct P { var x: Int }
来源：http://hxw.chenzaomai.com

[T26] Swift：类与重写
来源：http://odm.xylfe.cn

class A: Base { override func f() {} }
来源：http://una.cqqwz.cn


<!-- 参考信息 -->