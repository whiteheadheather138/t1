代发 wailian999

echo $((1 + 2 * 3))
来源：http://kns.aibaodan.cn

[R28] 浮点运算
来源：http://pru.aibaodan.cn

echo "scale=2; 10/3" | bc
来源：http://pao.ctjpmb.com

[R29] 定义函数
来源：http://hoi.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nny.jyoumei.cn

[R30] 函数返回状态码
来源：http://loa.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://aiu.jinqigufen.top

[R31] 局部变量
来源：http://qvf.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://bxy.bbcook.cn

[R32] 参数个数校验
来源：http://bfj.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bau.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://kds.uphjek.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kkl.meibo888.top

[R34] 退出时清理
来源：http://lvi.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://adj.chenzaomai.com

[R35] 后台执行并等待
来源：http://tro.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zvw.jqgufenzy.top

[R36] 并发执行多个任务
来源：http://hdh.cqqwz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dsr.jinqigufen.top

[R37] 把输出赋给变量
来源：http://wgf.c1oappe.top

files=$(ls -1)
来源：http://tyt.snrcjt.cn

[R38] 管道串联
来源：http://spe.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://dgv.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://yan.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://usa.52xcode.cn

[R40] 追加写日志
来源：http://egx.sjlbkw.cn

echo "log" >> out.log
来源：http://iks.tian-w.cn

[R41] 丢弃输出
来源：http://wrc.316326.xyz

cmd >/dev/null 2>&1
来源：http://xyi.yanxiufei.cn

[R42] 输入重定向
来源：http://lis.ywan-chungtsiang.top

wc -l < a.txt
来源：http://rjf.vehdjk.com

[R43] 按名字查找文件
来源：http://sxe.hcnkem.com

find . -name "*.log" -type f
来源：http://agh.gaohongyu789.top

[R44] 按修改时间查找
来源：http://ixm.yonumen.top

find . -mtime -7 -type f
来源：http://tkj.jinghuilouyu.cn

[R45] 批量删除
来源：http://snv.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://jwr.hcnkem.com

[R46] 递归替换文件内容
来源：http://yjh.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tlp.jianghu66.top

[R47] sed 单行替换
来源：http://sss.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://sek.jqgufenzy.top

[R48] awk 取指定列
来源：http://cbg.yuanzhike.top

awk '{print $1, $3}' a.txt
来源：http://urt.c1oappe.top

[R49] awk 带条件
来源：http://pza.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://shb.xuanzx.com

[R50] awk 求和
来源：http://vne.aibaodan.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gqx.xuanzx.com

[R51] 排序去重取前几
来源：http://ehq.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dpl.sysykeji.top

[R52] 统计行数
来源：http://opb.aizwys.cn

wc -l a.txt
来源：http://fgw.tarul.cn

[R53] 查看文件头与实时尾
来源：http://lhs.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mbd.zhiwuduotai.top

[R54] 比较两个文件
来源：http://ymb.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://uvi.cashguo.top

[R55] 压缩与解压
来源：http://xgr.jinqigfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dvc.feifeiyinyue.top

[R56] 远程拷贝
来源：http://jys.shzxlz.cn

scp file user@host:/path/
来源：http://jab.yongpay.top

[R57] 远程执行命令
来源：http://ddk.cashguo.top

ssh user@host 'uptime'
来源：http://bqt.chenjidiqi.icu

[R58] 下载文件
来源：http://gen.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zlv.jinqigufen.top

[R59] 发 POST JSON
来源：http://bmy.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tfs.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://fxs.fanxiaobao.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hpj.c1oappe.top

[R61] 磁盘占用
来源：http://ira.zhongyouzk.top

df -h;  du -sh *
来源：http://trl.zhijiandao.cn

[R62] 找最占空间的文件
来源：http://ens.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://rpa.chenzaomai.com

[R63] 内存与进程
来源：http://zdc.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://tvx.snrcjt.cn

[R64] 结束进程
来源：http://psf.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://kvj.jinghuilouyu.cn

[R65] 查看端口占用
来源：http://qyd.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lca.ppjwa.cn

[R66] 定时任务
来源：http://mot.hcnkem.com

crontab -e;  crontab -l
来源：http://zpe.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://paq.ehwqpu.com

openssl rand -hex 16
来源：http://bfl.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://qld.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xiy.shanyushiyangkeji.top

[R69] 生成随机密码
来源：http://hgh.yonumen.top

head -c 16 /dev/urandom | base64
来源：http://ryd.iojbl.cn

[R70] 时间戳与互转
来源：http://hao.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://tel.jlsjyb.cn

[R71] 日期格式化
来源：http://uxu.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ybz.bjfxy.top

[R72] 等待端口就绪
来源：http://yid.gaohongyu789.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kyc.nwbrower.top

[R73] 分割大日志
来源：http://zeg.cdnleiting.top

split -l 1000 big.log part_
来源：http://eoe.aibaodan.cn

[R74] 批量重命名
来源：http://whe.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://unh.xylfe.cn

[R75] 导出环境变量
来源：http://xdj.zhiwuduotai.top

export PATH="$HOME/bin:$PATH"
来源：http://toa.tarul.cn

[R76] 使用临时文件
来源：http://oyu.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rew.aibaodan.cn

[R77] 读取用户输入
来源：http://fse.jlsjyb.cn

read -rp "请输入: " ans
来源：http://dmw.yanxiufei.cn

[R78] 交互式菜单
来源：http://gol.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://mnw.nanxuanxn.top

[R79] 解析命令行选项
来源：http://dnh.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uvd.daria6918.cn

[R80] 查看脚本执行耗时
来源：http://oji.sjlbkw.cn

time ./run.sh
来源：http://rrk.hongshengwenyu.top

================================================================================
来源：http://zbv.c1oappe.top

S. C / C++ 专题
来源：http://owv.jqgfzy.top

================================================================================
来源：http://rmp.zhongyouzk.top

[S01] C：Hello World
来源：http://khd.jianghu66.top

#include <stdio.h>
来源：http://gzu.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ggp.meibo888.top

[S02] C：变量与格式化输出
来源：http://hvh.wangshuangyany.cn

int a = 10; printf("%d\n", a);
来源：http://cvn.wangshuangyany.cn

[S03] C：读入整数
来源：http://qrq.ivvv.top

int x; scanf("%d", &x);
来源：http://uvr.yueranfly.top

[S04] C：字符串复制
来源：http://hhn.jinghuilouyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yxv.xuetiantiany.cn

[S05] C：字符串长度
来源：http://mrs.tarul.cn

strlen(s)
来源：http://lsv.ctjpmb.com

[S06] C：字符串比较
来源：http://lfp.andypj.xyz

strcmp(a, b) == 0
来源：http://sun.xylfe.cn

[S07] C：数组遍历求和
来源：http://gcu.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vdo.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://vpy.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zvh.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://rmd.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kqr.epnwcf.com

[S10] C：指针与解引用
来源：http://xyh.guannengcc.top

int *p = &a;  *p = 5;
来源：http://yng.ybcxt.top

[S11] C：逐行读文件
来源：http://wuy.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://zip.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yqo.meibo888.top

fclose(f);
来源：http://biw.tianlin.xyz

[S12] C：写文件
来源：http://oxz.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xfz.vehdjk.com

[S13] C：宏定义
来源：http://isb.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pqa.wangdashe.top

[S14] C：枚举
来源：http://lrk.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://azi.fzhhl.top

[S15] C：类型转换
来源：http://wqe.jyoumei.cn

(double) a / b
来源：http://hwz.pengpengdd.cyou

[S16] C：位操作置位
来源：http://pot.fzhhl.top

x |= (1 << 3);
来源：http://ezv.hywenlv.cn

[S17] C：安全拼接字符串
来源：http://yat.jianghu66.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mmx.ehwqpu.com

[S18] C：命令行参数
来源：http://yrj.jinqigfzy.top

int main(int argc, char **argv)
来源：http://grc.cucudq.cn

[S19] C：快速排序
来源：http://hkl.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://awp.bbcook.cn

[S20] C：二分查找
来源：http://cmr.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kul.zhongyouzk.top

[S21] C：字符类别判断
来源：http://ktw.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hbd.hesvh.cn

[S22] C：字符串转数字
来源：http://hpy.chenzaomai.com

atoi("42");  strtod("3.14", NULL);
来源：http://cdv.cdnleiting.top

[S23] C：随机数
来源：http://dzr.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://cpp.yuanzhike.top

[S24] C：获取本地时间
来源：http://mmj.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tmu.jyoumei.cn

[S25] C：内存拷贝
来源：http://ijg.xinyue.icu

memcpy(dst, src, n);
来源：http://rkx.yuanzhike.top

[S26] C：内存清零
来源：http://qmi.havefunace.top

memset(a, 0, sizeof a);
来源：http://khk.nanxuanxn.top

[S27] C：定义常量
来源：http://elh.xinyue.icu

const double PI = 3.14159;
来源：http://oon.jinghuilouyu.cn

[S28] C：静态变量
来源：http://qie.gzhubu.top

static int counter = 0;
来源：http://vtu.hywenlv.cn

[S29] C：变参函数
来源：http://xcv.dashuyun.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ddw.yongpay.top

[S30] C：头文件保护
来源：http://ese.redwolf501.top

#ifndef X_H
来源：http://srk.daxiang520.top

#define X_H
来源：http://olu.tarul.cn

#endif
来源：http://tdc.tarul.cn

[S31] C++：Hello World
来源：http://ngq.sjlbkw.cn

#include <iostream>
来源：http://fhq.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://pec.jianghu66.top

[S32] C++：字符串
来源：http://ogb.xingfuxueyuan.xyz

std::string s = "hi";  s += "!";
来源：http://zrm.smart0.xyz

[S33] C++：vector 增删
来源：http://vtm.shanyushiyangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fbl.tarul.cn

[S34] C++：遍历 vector
来源：http://xqo.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://ddr.cdnleiting.top

[S35] C++：map
来源：http://jnf.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vre.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://nzr.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uiu.xingfuxueyuan.xyz

[S37] C++：set
来源：http://lov.zycfv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jed.zdbjq.cn

[S38] C++：排序
来源：http://jbx.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://que.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://twe.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wuq.gaohongyu789.top

[S40] C++：查找元素
来源：http://pbw.cheryme.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uvn.fengsongda.top

[S41] C++：类与构造函数
来源：http://zim.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://axu.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://ylo.fanxiaobao.xyz

class B : public Base { public: void f() override {} };
来源：http://pqh.gotoacloud.top

[S43] C++：智能指针
来源：http://ilw.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://fhc.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://mza.cheryme.top

void inc(int &x) { ++x; }
来源：http://ikw.52xcode.cn

[S45] C++：lambda
来源：http://ckc.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oei.gaohongyu789.top

[S46] C++：函数模板
来源：http://ihe.0kj1m.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gcm.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://pzi.zhaomingkeji.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gkg.meibo888.top

[S48] C++：逐行读文件
来源：http://gti.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bba.hnxiangtu.top

while (std::getline(in, line)) { }
来源：http://qpo.zhiwuduotai.top

[S49] C++：写文件
来源：http://jyr.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ite.cheryme.top

[S50] C++：格式化数字
来源：http://aac.yanxiufei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vki.svipenyu.cn

[S51] C++：显式类型转换
来源：http://cqu.jqgufenzy.top

static_cast<double>(a) / b
来源：http://qco.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://mze.ywan-chungtsiang.top

int size() const noexcept { return n_; }
来源：http://iug.jinqigufen.top

[S53] C++：移动语义
来源：http://vnt.chenlongwang.top

std::vector<int> w = std::move(v);
来源：http://nnr.bjfxy.top

[S54] C++：异常处理
来源：http://vir.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://amt.chenzaomai.com

[S55] C++：结构化绑定
来源：http://qlg.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://qeo.yj20258888.top

[S56] C++：optional
来源：http://hye.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fla.jinqigfzy.top

[S57] C++：编译期常量
来源：http://dhd.tianlin.xyz

constexpr int N = 10;
来源：http://vlr.tian-w.cn

[S58] C++：命名空间
来源：http://xwg.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://jnq.epnwcf.com

[S59] C++：静态断言
来源：http://vor.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wwm.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://teb.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rod.sjlbkw.cn

================================================================================
来源：http://rrr.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xsk.xziqi.cn

================================================================================
来源：http://xau.ivvv.top

[T01] Kotlin：Hello World
来源：http://feb.chenlongwang.top

println("Hello")
来源：http://dns.yueranfly.top

[T02] Kotlin：变量
来源：http://wfm.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nfh.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://ibs.ywan-chungtsiang.top

"值: $b"
来源：http://rcf.gzhubu.top

[T04] Kotlin：空安全
来源：http://cwx.xuanzx.com

val n: String? = null;  n?.length
来源：http://iwb.uphjek.com

[T05] Kotlin：when 表达式
来源：http://dwa.feifeiyinyue.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lxf.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://hag.316326.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://oft.yueranfly.top

[T07] Kotlin：集合过滤
来源：http://kby.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://osm.uphjek.com

[T08] Kotlin：数据类
来源：http://kdq.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://sme.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://lhm.gzhubu.top

fun String.exclaim() = this + "!"
来源：http://phi.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://lho.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://hrc.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://saf.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://xdv.guannengcc.top

[T12] Kotlin：解构声明
来源：http://mwk.ydzc1.top

val (a, b) = Pair(1, 2)
来源：http://rsp.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://btp.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://jde.cdnleiting.top

[T14] Kotlin：循环
来源：http://wlw.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://fhc.fengsongda.top

[T15] Kotlin：接口
来源：http://vgp.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://ygn.sjlbkw.cn

[T16] Swift：Hello World
来源：http://mox.wangdashe.top

print("Hello")
来源：http://pod.fktsv.cn

[T17] Swift：变量与常量
来源：http://bvh.zhongyouzk.top

var a = 1;  let b = 2
来源：http://ykm.hcnkem.com

[T18] Swift：字符串插值
来源：http://xhs.shzxlz.cn

"值: \(b)"
来源：http://dwj.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://ixg.sweek.top

if let n = opt { print(n) }
来源：http://woe.wangdashe.top

[T20] Swift：数组操作
来源：http://eqd.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hcu.hongshengwenyu.top

[T21] Swift：遍历
来源：http://rrd.xuetiantiany.cn

for x in a { print(x) }
来源：http://fwj.dashuyun.cn

[T22] Swift：字典
来源：http://ivf.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iwl.bbcook.cn

[T23] Swift：函数
来源：http://fnf.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qvn.316326.xyz

[T24] Swift：闭包
来源：http://amh.ctjpmb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://voj.ybcxt.top

[T25] Swift：结构体
来源：http://ihe.fengsongda.top

struct P { var x: Int }
来源：http://znf.yj20258888.top

[T26] Swift：类与重写
来源：http://xrq.nwbrower.top

class A: Base { override func f() {} }
来源：http://enz.jqgufenzy.top

[T27] Swift：错误处理
来源：http://hnh.fktsv.cn

do { try f() } catch { print(error) }
来源：http://qui.hywenlv.cn

[T28] Swift：枚举
来源：http://hkw.zdbjq.cn

enum Color { case red, green }
来源：http://pxy.jinqigfzy.top

[T29] Swift：guard 提前返回
来源：http://kwd.yanxiufei.cn

guard let x = opt else { return }
来源：http://gwg.hysaishi.cn

[T30] Swift：协议
来源：http://uzw.chenlongwang.top

protocol Shape { func area() -> Double }
来源：http://ipa.redwolf501.top


<!-- 参考信息 -->