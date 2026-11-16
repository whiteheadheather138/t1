代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://gqc.ydzc1.top

[R26] 命令替换
来源：http://lkk.zhongyouzk.top

now=$(date +%F); echo "$now"
来源：http://uoz.cheryme.top

[R27] 算术展开
来源：http://kms.svipenyu.cn

echo $((1 + 2 * 3))
来源：http://kcj.aizwys.cn

[R28] 浮点运算
来源：http://rid.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://qob.havefunace.top

[R29] 定义函数
来源：http://rhk.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wcq.fktsv.cn

[R30] 函数返回状态码
来源：http://ota.hywenlv.cn

f() { return 0; }; f || echo "失败了"
来源：http://qqk.nanxinkj.top

[R31] 局部变量
来源：http://qul.shzxlz.cn

f() { local x=1; echo "$x"; }
来源：http://hej.hammf.cn

[R32] 参数个数校验
来源：http://vix.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ljl.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://msl.svipenyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://feh.shanyushiyangtech.top

[R34] 退出时清理
来源：http://qne.zhijiandao.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gnk.sweek.top

[R35] 后台执行并等待
来源：http://xtp.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jgs.redwolf501.top

[R36] 并发执行多个任务
来源：http://opr.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gjt.cashguo.top

[R37] 把输出赋给变量
来源：http://bin.yj202588.top

files=$(ls -1)
来源：http://bgv.nanxinkj.top

[R38] 管道串联
来源：http://sxw.sxryk.cn

cat a.txt | grep -i error | wc -l
来源：http://qif.316326.xyz

[R39] 重定向标准输出与错误
来源：http://yal.aizwys.cn

cmd > out.log 2>&1
来源：http://xtu.pengpengdd.cyou

[R40] 追加写日志
来源：http://wkr.xuetiantiany.cn

echo "log" >> out.log
来源：http://tnf.jianghu66.top

[R41] 丢弃输出
来源：http://ppa.zhiwuduotai.top

cmd >/dev/null 2>&1
来源：http://hzr.ybcxt.top

[R42] 输入重定向
来源：http://dul.shzxlz.cn

wc -l < a.txt
来源：http://fmi.cqqwz.cn

[R43] 按名字查找文件
来源：http://zzi.vehdjk.com

find . -name "*.log" -type f
来源：http://zbs.fktsv.cn

[R44] 按修改时间查找
来源：http://uir.bbcook.cn

find . -mtime -7 -type f
来源：http://ezj.shanyushiyangtech.top

[R45] 批量删除
来源：http://ero.yuxming.cn

find . -name "*.tmp" -delete
来源：http://rcn.pycfn.com

[R46] 递归替换文件内容
来源：http://oxz.tianlin.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iui.vqdsnc.cn

[R47] sed 单行替换
来源：http://jwg.guowangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://ila.ctjpmb.com

[R48] awk 取指定列
来源：http://qhd.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://wut.yuxming.cn

[R49] awk 带条件
来源：http://flx.jinqigfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eox.fktsv.cn

[R50] awk 求和
来源：http://pbs.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rah.gaohongyu789.top

[R51] 排序去重取前几
来源：http://qld.xinyue.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://ztd.yuxming.cn

[R52] 统计行数
来源：http://rix.sxryk.cn

wc -l a.txt
来源：http://dpk.ivvv.top

[R53] 查看文件头与实时尾
来源：http://qlt.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pha.yj20258888.top

[R54] 比较两个文件
来源：http://qvu.zhixingplan.top

diff a.txt b.txt
来源：http://urq.cheryme.top

[R55] 压缩与解压
来源：http://jfj.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zrm.shanyushiyangkeji.top

[R56] 远程拷贝
来源：http://bdb.chenlongwang.top

scp file user@host:/path/
来源：http://pja.yfazqb.com

[R57] 远程执行命令
来源：http://hys.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://uri.jlsjyb.cn

[R58] 下载文件
来源：http://cqg.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sjh.jlsjyb.cn

[R59] 发 POST JSON
来源：http://jgq.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://loe.hnxiangtu.top

[R60] 只看 HTTP 状态码
来源：http://mfv.ppjwa.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yyn.fehbvm.com

[R61] 磁盘占用
来源：http://vks.ybcxt.top

df -h;  du -sh *
来源：http://jlr.jianghu66.top

[R62] 找最占空间的文件
来源：http://dix.zhoulong.xyz

du -ah . | sort -rh | head -10
来源：http://brw.chenjidiqi.icu

[R63] 内存与进程
来源：http://xna.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://swn.quarkkingdee.top

[R64] 结束进程
来源：http://oaf.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://upx.hfpthk.cn

[R65] 查看端口占用
来源：http://vfm.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vsk.xinyue.icu

[R66] 定时任务
来源：http://pqp.ctjpmb.com

crontab -e;  crontab -l
来源：http://uke.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://ogi.shuidangran.top

openssl rand -hex 16
来源：http://nid.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://emy.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nig.vehdjk.com

[R69] 生成随机密码
来源：http://uwl.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://lsx.ivvv.top

[R70] 时间戳与互转
来源：http://drl.cashguo.top

date +%s;  date -d @1700000000
来源：http://djl.c1oappe.top

[R71] 日期格式化
来源：http://fkd.ybcxt.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://paj.yonumen.top

[R72] 等待端口就绪
来源：http://dnc.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://bvk.hnxiangtu.top

[R73] 分割大日志
来源：http://vfd.jqgfzy.top

split -l 1000 big.log part_
来源：http://ixq.svipenyu.cn

[R74] 批量重命名
来源：http://sis.yongpay.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jbb.jyoumei.cn

[R75] 导出环境变量
来源：http://zhq.xuanzx.com

export PATH="$HOME/bin:$PATH"
来源：http://pes.birdmap.top

[R76] 使用临时文件
来源：http://uak.aizwys.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sro.yueranfly.top

[R77] 读取用户输入
来源：http://pam.jqgufenzy.top

read -rp "请输入: " ans
来源：http://ltp.52xcode.cn

[R78] 交互式菜单
来源：http://sfc.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ckq.hysaishi.cn

[R79] 解析命令行选项
来源：http://ktn.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jtm.quarkkingdee.top

[R80] 查看脚本执行耗时
来源：http://ghi.zdbjq.cn

time ./run.sh
来源：http://tot.yangfankeji.com

================================================================================
来源：http://ptg.ppjwa.cn

S. C / C++ 专题
来源：http://tsj.zhaomingkeji.xyz

================================================================================
来源：http://qyr.yangfankeji.com

[S01] C：Hello World
来源：http://ocx.dianchejie.cn

#include <stdio.h>
来源：http://abu.vqdsnc.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aza.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://ems.hnxiangtu.top

int a = 10; printf("%d\n", a);
来源：http://ukz.yangfankeji.com

[S03] C：读入整数
来源：http://alw.316326.xyz

int x; scanf("%d", &x);
来源：http://fka.hnqzz.top

[S04] C：字符串复制
来源：http://onj.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://hbb.ivvv.top

[S05] C：字符串长度
来源：http://fnc.fanxiaobao.xyz

strlen(s)
来源：http://umg.yuanzhike.top

[S06] C：字符串比较
来源：http://vly.redwolf501.top

strcmp(a, b) == 0
来源：http://lhq.ydzc1.top

[S07] C：数组遍历求和
来源：http://hjq.cdnleiting.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mmi.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://coy.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dpo.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://fkg.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ynd.jianghu66.top

[S10] C：指针与解引用
来源：http://lgx.mhx1999.top

int *p = &a;  *p = 5;
来源：http://san.jyoumei.cn

[S11] C：逐行读文件
来源：http://rbc.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://xhi.mhx1999.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://aah.zhiwuduotai.top

fclose(f);
来源：http://dlo.hysaishi.cn

[S12] C：写文件
来源：http://zav.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nrc.feifeiyinyue.top

[S13] C：宏定义
来源：http://rhj.chenjidiqi.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ozb.yangfankeji.com

[S14] C：枚举
来源：http://aco.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://gtz.ybcxt.top

[S15] C：类型转换
来源：http://qqv.jinqigfzy.top

(double) a / b
来源：http://xbr.xinyue.icu

[S16] C：位操作置位
来源：http://tyf.yuxming.cn

x |= (1 << 3);
来源：http://owf.hywenlv.cn

[S17] C：安全拼接字符串
来源：http://mcu.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gvb.wangshuangyany.cn

[S18] C：命令行参数
来源：http://cgf.gaohongyu789.top

int main(int argc, char **argv)
来源：http://cop.pengpengdd.cyou

[S19] C：快速排序
来源：http://ihf.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jeu.vehdjk.com

[S20] C：二分查找
来源：http://rok.ivvv.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hvk.xziqi.cn

[S21] C：字符类别判断
来源：http://qdy.xuetiantiany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xwp.sysykeji.top

[S22] C：字符串转数字
来源：http://suq.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://vti.fehbvm.com

[S23] C：随机数
来源：http://vmr.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cxq.0kj1m.cn

[S24] C：获取本地时间
来源：http://atn.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vmh.hcnkem.com

[S25] C：内存拷贝
来源：http://qxr.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://hiz.shuidangran.top

[S26] C：内存清零
来源：http://ysn.iojbl.cn

memset(a, 0, sizeof a);
来源：http://vzt.tarul.cn

[S27] C：定义常量
来源：http://mrc.gogol.net.cn

const double PI = 3.14159;
来源：http://spl.uphjek.com

[S28] C：静态变量
来源：http://wsq.hywenlv.cn

static int counter = 0;
来源：http://elu.chenjidiqi.icu

[S29] C：变参函数
来源：http://nmb.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://llw.wangdashe.top

[S30] C：头文件保护
来源：http://alx.yueranfly.top

#ifndef X_H
来源：http://koa.hammf.cn

#define X_H
来源：http://zzw.kuanghao11.cn

#endif
来源：http://xaa.jianghu66.top

[S31] C++：Hello World
来源：http://dfh.gotoacloud.top

#include <iostream>
来源：http://qdp.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://zwk.jqgufenzy.top

[S32] C++：字符串
来源：http://fpw.zhaomingkeji.xyz

std::string s = "hi";  s += "!";
来源：http://uff.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://dab.yfazqb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nje.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://zbe.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://uie.cheryme.top

[S35] C++：map
来源：http://xmr.guowangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hqr.nanxinkj.top

[S36] C++：unordered_map
来源：http://ups.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://otw.c1oappe.top

[S37] C++：set
来源：http://iqn.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://orx.havefunace.top

[S38] C++：排序
来源：http://lno.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://umj.wangdashe.top

[S39] C++：自定义比较器排序
来源：http://oqu.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gjf.aibaodan.cn

[S40] C++：查找元素
来源：http://czm.hysaishi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gji.jlsjyb.cn

[S41] C++：类与构造函数
来源：http://hwg.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://awx.daxiang520.top

[S42] C++：继承与虚函数
来源：http://bam.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://wof.52xcode.cn

[S43] C++：智能指针
来源：http://mzt.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://lqt.cheryme.top

[S44] C++：引用传参
来源：http://uuf.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://pfz.daxiang520.top

[S45] C++：lambda
来源：http://ncr.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sku.daxiang520.top

[S46] C++：函数模板
来源：http://zhg.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kgn.ctjpmb.com

[S47] C++：结构化绑定遍历
来源：http://wud.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bfn.hfpthk.cn

[S48] C++：逐行读文件
来源：http://xiw.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zux.daxiang520.top

while (std::getline(in, line)) { }
来源：http://tgg.sjlbkw.cn

[S49] C++：写文件
来源：http://oro.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qbc.jiagoushi.top

[S50] C++：格式化数字
来源：http://xdp.zycfv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hdo.jianghu66.top

[S51] C++：显式类型转换
来源：http://lzf.yonumen.top

static_cast<double>(a) / b
来源：http://quh.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://wvw.zycfv.cn

int size() const noexcept { return n_; }
来源：http://jod.xingfuxueyuan.xyz

[S53] C++：移动语义
来源：http://lta.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://ftl.fengsongda.top

[S54] C++：异常处理
来源：http://ppz.cashguo.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://osg.nanxinkj.top

[S55] C++：结构化绑定
来源：http://ndn.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://vyj.jqgufenzy.top

[S56] C++：optional
来源：http://dkz.zdqjudy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eku.dianchejie.cn

[S57] C++：编译期常量
来源：http://ixt.jqgufenzy.top

constexpr int N = 10;
来源：http://ipf.hesvh.cn

[S58] C++：命名空间
来源：http://ktv.zhixingplan.top

namespace ns { int f() { return 1; } }
来源：http://rut.xylfe.cn

[S59] C++：静态断言
来源：http://lyh.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cws.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://wpj.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wys.tianlin.xyz

================================================================================
来源：http://kqm.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://knr.tarul.cn

================================================================================
来源：http://hfz.jqgufenzy.top

[T01] Kotlin：Hello World
来源：http://woz.snrcjt.cn

println("Hello")
来源：http://bdq.fehbvm.com

[T02] Kotlin：变量
来源：http://esb.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ruh.zhiwuduotai.top

[T03] Kotlin：字符串模板
来源：http://elk.pycfn.com

"值: $b"
来源：http://qjb.0kj1m.cn

[T04] Kotlin：空安全
来源：http://mkq.hongshengwenyu.top

val n: String? = null;  n?.length
来源：http://ukb.cashguo.top

[T05] Kotlin：when 表达式
来源：http://bpp.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qny.guannengcc.top

[T06] Kotlin：集合映射
来源：http://wzz.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eft.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://smf.shanyushiyangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://stm.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://jmr.9152youxi.cn

data class User(val name: String, val age: Int)
来源：http://dpy.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://brg.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://jug.vehdjk.com

[T10] Kotlin：默认参数
来源：http://pxj.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ufa.aizwys.cn

[T11] Kotlin：协程
来源：http://toz.zdqjudy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dig.shzxlz.cn

[T12] Kotlin：解构声明
来源：http://biz.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://hlb.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://ucy.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://gnl.haohaochexian.top

[T14] Kotlin：循环
来源：http://hxw.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://qsg.jinghuilouyu.cn

[T15] Kotlin：接口
来源：http://peg.ydzc1.top

interface Shape { fun area(): Double }
来源：http://zek.jiagoushi.top

[T16] Swift：Hello World
来源：http://fef.nwbrower.top

print("Hello")
来源：http://yej.dianchejie.cn

[T17] Swift：变量与常量
来源：http://eqi.daxiang520.top

var a = 1;  let b = 2
来源：http://ijf.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://ilm.jianghu66.top

"值: \(b)"
来源：http://tcw.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://jmp.kuanghao11.cn

if let n = opt { print(n) }
来源：http://yce.yvedp.cn

[T20] Swift：数组操作
来源：http://nyp.dianchejie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xmy.shangyingyoupin.top

[T21] Swift：遍历
来源：http://xts.chenjidiqi.icu

for x in a { print(x) }
来源：http://grq.quarkkingdee.top

[T22] Swift：字典
来源：http://tvk.yvedp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://idj.kuanghao11.cn

[T23] Swift：函数
来源：http://rke.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hca.haohaochexian.top

[T24] Swift：闭包
来源：http://swz.0kj1m.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://imi.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://njk.316326.xyz

struct P { var x: Int }
来源：http://xww.havefunace.top

[T26] Swift：类与重写
来源：http://pah.tanke756.top

class A: Base { override func f() {} }
来源：http://atr.shuidangran.top

[T27] Swift：错误处理
来源：http://kov.yongpay.top

do { try f() } catch { print(error) }
来源：http://rsr.shanyushiyangtech.top

[T28] Swift：枚举
来源：http://hnh.0kj1m.cn

enum Color { case red, green }
来源：http://zlc.jinghuilouyu.cn


<!-- 参考信息 -->