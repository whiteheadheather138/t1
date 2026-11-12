代发 wailian999

echo "${#s}"
来源：http://aeo.mhx1999.top

[R22] 截取子串
来源：http://rmg.xuanzx.com

echo "${s:0:5}"
来源：http://flj.316326.xyz

[R23] 字符串替换
来源：http://amd.quarkkingdee.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fxm.kuanghao11.cn

[R24] 大小写转换
来源：http://iyu.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://lof.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://hnj.hysaishi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://chy.yueranfly.top

[R26] 命令替换
来源：http://cuk.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://quz.wangshuangyany.cn

[R27] 算术展开
来源：http://vey.daxiang520.top

echo $((1 + 2 * 3))
来源：http://wef.guowangkeji.top

[R28] 浮点运算
来源：http://sss.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://udv.tian-w.cn

[R29] 定义函数
来源：http://gko.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ggl.sysykeji.top

[R30] 函数返回状态码
来源：http://ces.zhaomingkeji.xyz

f() { return 0; }; f || echo "失败了"
来源：http://evs.zhoulong.xyz

[R31] 局部变量
来源：http://vex.tianlin.xyz

f() { local x=1; echo "$x"; }
来源：http://qwu.yj20258888.top

[R32] 参数个数校验
来源：http://dvx.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iwr.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://qyv.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fri.jianghu66.top

[R34] 退出时清理
来源：http://cku.nanxuanxn.top

trap 'rm -f "$tmp"' EXIT
来源：http://uci.yj202588.top

[R35] 后台执行并等待
来源：http://czu.fehbvm.com

sleep 5 & pid=$!; wait "$pid"
来源：http://cvx.daxiang520.top

[R36] 并发执行多个任务
来源：http://ozm.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gkx.ehwqpu.com

[R37] 把输出赋给变量
来源：http://seh.tanke756.top

files=$(ls -1)
来源：http://lmv.cashguo.top

[R38] 管道串联
来源：http://rdo.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://epy.hcnkem.com

[R39] 重定向标准输出与错误
来源：http://nvv.ybcxt.top

cmd > out.log 2>&1
来源：http://wgw.daxiang520.top

[R40] 追加写日志
来源：http://bht.gzhubu.top

echo "log" >> out.log
来源：http://whb.smart0.xyz

[R41] 丢弃输出
来源：http://snw.birdmap.top

cmd >/dev/null 2>&1
来源：http://dgj.gaohongyu789.top

[R42] 输入重定向
来源：http://ody.hywenlv.cn

wc -l < a.txt
来源：http://txi.ydjk.org.cn

[R43] 按名字查找文件
来源：http://plc.yuxming.cn

find . -name "*.log" -type f
来源：http://ldn.tarul.cn

[R44] 按修改时间查找
来源：http://nbk.yfazqb.com

find . -mtime -7 -type f
来源：http://sil.hcnkem.com

[R45] 批量删除
来源：http://htz.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://uwg.ydzc1.top

[R46] 递归替换文件内容
来源：http://tdd.gzhubu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://reh.daria6918.cn

[R47] sed 单行替换
来源：http://pdi.52xcode.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zkb.chenjidiqi.icu

[R48] awk 取指定列
来源：http://lyi.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://kgm.xziqi.cn

[R49] awk 带条件
来源：http://xxw.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gpy.vehdjk.com

[R50] awk 求和
来源：http://qkt.hnqzz.top

awk '{s += $2} END {print s}' a.txt
来源：http://utx.gaohongyu789.top

[R51] 排序去重取前几
来源：http://xay.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lgp.tianlin.xyz

[R52] 统计行数
来源：http://fpy.fktsv.cn

wc -l a.txt
来源：http://hnf.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://vaf.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dul.chenjidiqi.icu

[R54] 比较两个文件
来源：http://vrz.yueranfly.top

diff a.txt b.txt
来源：http://zaz.nanxuanxn.top

[R55] 压缩与解压
来源：http://pmy.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sez.bjfxy.top

[R56] 远程拷贝
来源：http://smk.ydzc1.top

scp file user@host:/path/
来源：http://hqn.xylfe.cn

[R57] 远程执行命令
来源：http://zpr.aibaodan.cn

ssh user@host 'uptime'
来源：http://llu.yuxming.cn

[R58] 下载文件
来源：http://hbx.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bwa.aibaodan.cn

[R59] 发 POST JSON
来源：http://mqr.jqgufenzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://utu.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://dhc.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qla.xuetiantiany.cn

[R61] 磁盘占用
来源：http://zik.svipenyu.cn

df -h;  du -sh *
来源：http://mnm.9152youxi.cn

[R62] 找最占空间的文件
来源：http://fcl.xuetiantiany.cn

du -ah . | sort -rh | head -10
来源：http://xdl.kuanghao11.cn

[R63] 内存与进程
来源：http://fxw.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://rel.pycfn.com

[R64] 结束进程
来源：http://otr.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://yap.guowangkeji.top

[R65] 查看端口占用
来源：http://ucc.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yfc.hywenlv.cn

[R66] 定时任务
来源：http://pzo.dashuyun.cn

crontab -e;  crontab -l
来源：http://gyn.daxiang520.top

[R67] 生成随机十六进制串
来源：http://cdw.pycfn.com

openssl rand -hex 16
来源：http://keq.wangshuangyany.cn

[R68] 计算文件校验值
来源：http://abw.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pfe.cdnleiting.top

[R69] 生成随机密码
来源：http://kmu.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://dur.tanke756.top

[R70] 时间戳与互转
来源：http://qds.hongshengwenyu.top

date +%s;  date -d @1700000000
来源：http://oaf.chenzaomai.com

[R71] 日期格式化
来源：http://kpq.zhongyouzk.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dbc.hnqzz.top

[R72] 等待端口就绪
来源：http://wrp.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cmi.9152youxi.cn

[R73] 分割大日志
来源：http://czy.xingfuxueyuan.xyz

split -l 1000 big.log part_
来源：http://odo.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://ond.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uxn.sjlbkw.cn

[R75] 导出环境变量
来源：http://ndp.zdbjq.cn

export PATH="$HOME/bin:$PATH"
来源：http://dnf.zdqjudy.top

[R76] 使用临时文件
来源：http://sfk.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://azg.tanke756.top

[R77] 读取用户输入
来源：http://ves.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://dwz.shzxlz.cn

[R78] 交互式菜单
来源：http://kfo.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uxt.xylfe.cn

[R79] 解析命令行选项
来源：http://ojn.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ozw.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://dqs.tianlin.xyz

time ./run.sh
来源：http://tkl.yvedp.cn

================================================================================
来源：http://nss.iojbl.cn

S. C / C++ 专题
来源：http://upj.yangfankeji.com

================================================================================
来源：http://kao.jinqigfzy.top

[S01] C：Hello World
来源：http://gdi.hnqzz.top

#include <stdio.h>
来源：http://kiv.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fmv.shangyingyoupin.top

[S02] C：变量与格式化输出
来源：http://icp.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://nyq.shangyingyoupin.top

[S03] C：读入整数
来源：http://gdp.redwolf501.top

int x; scanf("%d", &x);
来源：http://dgv.zdqjudy.top

[S04] C：字符串复制
来源：http://onj.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://luc.tian-w.cn

[S05] C：字符串长度
来源：http://wzv.jinyuanbaomall.cn

strlen(s)
来源：http://yor.cashguo.top

[S06] C：字符串比较
来源：http://djg.bbcook.cn

strcmp(a, b) == 0
来源：http://dpx.hywenlv.cn

[S07] C：数组遍历求和
来源：http://uqu.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xws.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://nmn.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vsr.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://reo.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tnq.nwbrower.top

[S10] C：指针与解引用
来源：http://nfc.redwolf501.top

int *p = &a;  *p = 5;
来源：http://oja.cdnleiting.top

[S11] C：逐行读文件
来源：http://sxr.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://udv.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://oot.cdnleiting.top

fclose(f);
来源：http://ter.jlsjyb.cn

[S12] C：写文件
来源：http://jmy.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://elk.haohaochexian.top

[S13] C：宏定义
来源：http://fto.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dqk.cucudq.cn

[S14] C：枚举
来源：http://sio.daria6918.cn

enum Color { RED, GREEN, BLUE };
来源：http://gyq.kuanghao11.cn

[S15] C：类型转换
来源：http://riw.shangyingyoupin.top

(double) a / b
来源：http://czo.chenlongwang.top

[S16] C：位操作置位
来源：http://rya.jinghuilouyu.cn

x |= (1 << 3);
来源：http://eyv.svipenyu.cn

[S17] C：安全拼接字符串
来源：http://gqp.zhijiandao.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lqr.fzhhl.top

[S18] C：命令行参数
来源：http://zzr.yuanzhike.top

int main(int argc, char **argv)
来源：http://cww.cqqwz.cn

[S19] C：快速排序
来源：http://bea.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://egv.jinghuilouyu.cn

[S20] C：二分查找
来源：http://mlg.pycfn.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fcq.havefunace.top

[S21] C：字符类别判断
来源：http://kjx.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ksw.ctjpmb.com

[S22] C：字符串转数字
来源：http://mft.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://zgj.zycfv.cn

[S23] C：随机数
来源：http://ker.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://aew.bjfxy.top

[S24] C：获取本地时间
来源：http://jex.svipenyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://drb.c1oappe.top

[S25] C：内存拷贝
来源：http://vfb.9152youxi.cn

memcpy(dst, src, n);
来源：http://pdp.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://fiq.jinqigfzy.top

memset(a, 0, sizeof a);
来源：http://jne.316326.xyz

[S27] C：定义常量
来源：http://ikq.jyoumei.cn

const double PI = 3.14159;
来源：http://tvk.xziqi.cn

[S28] C：静态变量
来源：http://pdq.aizwys.cn

static int counter = 0;
来源：http://pnv.cashguo.top

[S29] C：变参函数
来源：http://sbm.ehwqpu.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eih.ybcxt.top

[S30] C：头文件保护
来源：http://vlk.yueranfly.top

#ifndef X_H
来源：http://wof.dashuyun.cn

#define X_H
来源：http://ocs.sjlbkw.cn

#endif
来源：http://fug.jianghu66.top

[S31] C++：Hello World
来源：http://rit.bjfxy.top

#include <iostream>
来源：http://aet.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://bgm.yuxming.cn

[S32] C++：字符串
来源：http://pim.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://ike.zhixingplan.top

[S33] C++：vector 增删
来源：http://wzm.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jdy.shanyushiyangtech.top

[S34] C++：遍历 vector
来源：http://rol.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://jfl.gogol.net.cn

[S35] C++：map
来源：http://ygo.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://skd.chenlongwang.top

[S36] C++：unordered_map
来源：http://aqm.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wei.xingfuxueyuan.xyz

[S37] C++：set
来源：http://wdu.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wcz.316326.xyz

[S38] C++：排序
来源：http://fvf.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://llj.sweek.top

[S39] C++：自定义比较器排序
来源：http://sun.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://afz.havefunace.top

[S40] C++：查找元素
来源：http://guw.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jwx.hysaishi.cn

[S41] C++：类与构造函数
来源：http://deh.hfpthk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wnf.vehdjk.com

[S42] C++：继承与虚函数
来源：http://mdu.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://tiw.ehwqpu.com

[S43] C++：智能指针
来源：http://ekk.wangdashe.top

auto p = std::make_unique<int>(5);
来源：http://zhu.9152youxi.cn

[S44] C++：引用传参
来源：http://hhu.guannengcc.top

void inc(int &x) { ++x; }
来源：http://xcp.chenjidiqi.icu

[S45] C++：lambda
来源：http://xdc.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://duy.hnqzz.top

[S46] C++：函数模板
来源：http://alj.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wrf.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://gas.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gob.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://ogg.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://tgv.jianghu66.top

while (std::getline(in, line)) { }
来源：http://wdo.hfpthk.cn

[S49] C++：写文件
来源：http://zqb.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://byd.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://qgb.zdqjudy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ifu.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://pyc.52xcode.cn

static_cast<double>(a) / b
来源：http://bap.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://smv.hcnkem.com

int size() const noexcept { return n_; }
来源：http://tyx.feifeiyinyue.top

[S53] C++：移动语义
来源：http://zvw.dianchejie.cn

std::vector<int> w = std::move(v);
来源：http://nxa.hnxiangtu.top

[S54] C++：异常处理
来源：http://whh.shanyushiyangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xtn.jyoumei.cn

[S55] C++：结构化绑定
来源：http://qlh.iojbl.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pzi.cqqwz.cn

[S56] C++：optional
来源：http://psj.jinghuilouyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kuz.hnqzz.top

[S57] C++：编译期常量
来源：http://hbf.ctjpmb.com

constexpr int N = 10;
来源：http://kik.52xcode.cn

[S58] C++：命名空间
来源：http://bpj.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://fwo.iojbl.cn

[S59] C++：静态断言
来源：http://ekf.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wed.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://tuw.yj202588.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iah.zdbjq.cn

================================================================================
来源：http://hit.sxryk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nya.shuidangran.top

================================================================================
来源：http://ymv.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://gkq.iojbl.cn

println("Hello")
来源：http://uub.9152youxi.cn

[T02] Kotlin：变量
来源：http://trp.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gbz.jianghu66.top

[T03] Kotlin：字符串模板
来源：http://swf.ybcxt.top

"值: $b"
来源：http://qcp.cucudq.cn

[T04] Kotlin：空安全
来源：http://iua.hesvh.cn

val n: String? = null;  n?.length
来源：http://fbi.meibo888.top

[T05] Kotlin：when 表达式
来源：http://ach.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://arn.jinqigufen.top

[T06] Kotlin：集合映射
来源：http://ona.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jdp.ivvv.top

[T07] Kotlin：集合过滤
来源：http://nxc.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://soa.0kj1m.cn

[T08] Kotlin：数据类
来源：http://znj.shzxlz.cn

data class User(val name: String, val age: Int)
来源：http://mrf.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://zdr.xingfuxueyuan.xyz

fun String.exclaim() = this + "!"
来源：http://npd.hcnkem.com

[T10] Kotlin：默认参数
来源：http://eji.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hhg.yuanzhike.top

[T11] Kotlin：协程
来源：http://ayl.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://kze.pycfn.com

[T12] Kotlin：解构声明
来源：http://bfi.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://ojf.yj202588.top

[T13] Kotlin：只读 Map
来源：http://ubb.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://myc.chenjidiqi.icu

[T14] Kotlin：循环
来源：http://ubl.zdqjudy.top

for (i in 1..10) println(i)
来源：http://dsn.cucudq.cn

[T15] Kotlin：接口
来源：http://fiw.yfazqb.com

interface Shape { fun area(): Double }
来源：http://brn.sysykeji.top

[T16] Swift：Hello World
来源：http://pus.dashuyun.cn

print("Hello")
来源：http://crw.cucudq.cn

[T17] Swift：变量与常量
来源：http://esh.jyoumei.cn

var a = 1;  let b = 2
来源：http://ahs.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://uad.xuanzx.com

"值: \(b)"
来源：http://xbl.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://wgk.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://glh.yuanzhike.top

[T20] Swift：数组操作
来源：http://nku.bbcook.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fyy.sjlbkw.cn

[T21] Swift：遍历
来源：http://qrr.ydzc1.top

for x in a { print(x) }
来源：http://gpq.sysykeji.top

[T22] Swift：字典
来源：http://crz.0kj1m.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gvk.xuetiantiany.cn

[T23] Swift：函数
来源：http://sun.yuxming.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://efg.shanyushiyangtech.top

[T24] Swift：闭包
来源：http://ufv.sufxvd.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mjs.cheryme.top


<!-- 参考信息 -->