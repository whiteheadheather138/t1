代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://vlu.chenlongwang.top

[R26] 命令替换
来源：http://bwp.zhijiandao.cn

now=$(date +%F); echo "$now"
来源：http://pbj.yj202588.top

[R27] 算术展开
来源：http://hvx.cucudq.cn

echo $((1 + 2 * 3))
来源：http://sxp.fktsv.cn

[R28] 浮点运算
来源：http://hkj.zdqjudy.top

echo "scale=2; 10/3" | bc
来源：http://ary.quarkkingdee.top

[R29] 定义函数
来源：http://ztz.tian-w.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vcc.zhixingplan.top

[R30] 函数返回状态码
来源：http://igt.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://lyd.jinyuanbaomall.cn

[R31] 局部变量
来源：http://cwj.aizwys.cn

f() { local x=1; echo "$x"; }
来源：http://thb.0kj1m.cn

[R32] 参数个数校验
来源：http://afo.cdnleiting.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kcv.gaohongyu789.top

[R33] 捕获错误并提示行号
来源：http://dxr.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://utb.sweek.top

[R34] 退出时清理
来源：http://lsy.sufxvd.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dan.zycfv.cn

[R35] 后台执行并等待
来源：http://vrn.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xam.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://rok.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hxr.ctjpmb.com

[R37] 把输出赋给变量
来源：http://tsn.jlsjyb.cn

files=$(ls -1)
来源：http://ymq.dianchejie.cn

[R38] 管道串联
来源：http://vap.guannengcc.top

cat a.txt | grep -i error | wc -l
来源：http://xcm.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://cxv.hcnkem.com

cmd > out.log 2>&1
来源：http://mme.gzhubu.top

[R40] 追加写日志
来源：http://kgg.svipenyu.cn

echo "log" >> out.log
来源：http://qpg.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://xee.hnqzz.top

cmd >/dev/null 2>&1
来源：http://xhn.mhx1999.top

[R42] 输入重定向
来源：http://oti.jinqigufen.top

wc -l < a.txt
来源：http://rkr.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://dhy.andypj.xyz

find . -name "*.log" -type f
来源：http://qtv.cucudq.cn

[R44] 按修改时间查找
来源：http://urx.jinyuanbaomall.cn

find . -mtime -7 -type f
来源：http://kox.hfpthk.cn

[R45] 批量删除
来源：http://sjg.ehwqpu.com

find . -name "*.tmp" -delete
来源：http://jcd.dashuyun.cn

[R46] 递归替换文件内容
来源：http://nai.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eyu.daria6918.cn

[R47] sed 单行替换
来源：http://wph.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://oqh.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://pva.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://mqg.zdbjq.cn

[R49] awk 带条件
来源：http://ymb.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://axg.jqgfzy.top

[R50] awk 求和
来源：http://nxa.yongpay.top

awk '{s += $2} END {print s}' a.txt
来源：http://ivt.hcnkem.com

[R51] 排序去重取前几
来源：http://hgu.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://alo.dashuyun.cn

[R52] 统计行数
来源：http://zly.jinghuilouyu.cn

wc -l a.txt
来源：http://bpi.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://pvz.zhixingplan.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zfg.ctjpmb.com

[R54] 比较两个文件
来源：http://wtp.gaohongyu789.top

diff a.txt b.txt
来源：http://gyp.sxryk.cn

[R55] 压缩与解压
来源：http://klk.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sau.zhoulong.xyz

[R56] 远程拷贝
来源：http://ecy.jinghuilouyu.cn

scp file user@host:/path/
来源：http://uql.xuetiantiany.cn

[R57] 远程执行命令
来源：http://yli.yfazqb.com

ssh user@host 'uptime'
来源：http://qxh.jinqigfzy.top

[R58] 下载文件
来源：http://qxr.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://itt.smart0.xyz

[R59] 发 POST JSON
来源：http://chg.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ipa.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://yow.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kbs.mhx1999.top

[R61] 磁盘占用
来源：http://kii.jinqigufen.top

df -h;  du -sh *
来源：http://tuv.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://hao.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://bdt.yj20258.top

[R63] 内存与进程
来源：http://uij.yangfankeji.com

free -h;  ps aux | grep nginx
来源：http://azw.yj202588.top

[R64] 结束进程
来源：http://wty.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://tns.zhongyouzk.top

[R65] 查看端口占用
来源：http://ema.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lpy.gogol.net.cn

[R66] 定时任务
来源：http://ytr.nwbrower.top

crontab -e;  crontab -l
来源：http://cns.nwbrower.top

[R67] 生成随机十六进制串
来源：http://kqw.tian-w.cn

openssl rand -hex 16
来源：http://why.gotoacloud.top

[R68] 计算文件校验值
来源：http://uuc.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://bdp.shangyingyoupin.top

[R69] 生成随机密码
来源：http://bwk.hnxiangtu.top

head -c 16 /dev/urandom | base64
来源：http://rsd.zhixingplan.top

[R70] 时间戳与互转
来源：http://xbb.52xcode.cn

date +%s;  date -d @1700000000
来源：http://ixt.dashuyun.cn

[R71] 日期格式化
来源：http://jbu.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hdq.feifeiyinyue.top

[R72] 等待端口就绪
来源：http://jen.quarkkingdee.top

until nc -z localhost 3306; do sleep 1; done
来源：http://olc.xuetiantiany.cn

[R73] 分割大日志
来源：http://nnq.jinqigufen.top

split -l 1000 big.log part_
来源：http://swb.hnqzz.top

[R74] 批量重命名
来源：http://krt.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ohk.ivvv.top

[R75] 导出环境变量
来源：http://pgy.hywenlv.cn

export PATH="$HOME/bin:$PATH"
来源：http://iys.hammf.cn

[R76] 使用临时文件
来源：http://pdt.sjlbkw.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://snm.jqgfzy.top

[R77] 读取用户输入
来源：http://deo.ctjpmb.com

read -rp "请输入: " ans
来源：http://eiy.meibo888.top

[R78] 交互式菜单
来源：http://vcw.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lud.316326.xyz

[R79] 解析命令行选项
来源：http://gsf.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ray.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://sdj.sysykeji.top

time ./run.sh
来源：http://uem.hywenlv.cn

================================================================================
来源：http://rlh.nwbrower.top

S. C / C++ 专题
来源：http://qdw.nanxuanxn.top

================================================================================
来源：http://yhh.yj20258.top

[S01] C：Hello World
来源：http://cny.shangyingyoupin.top

#include <stdio.h>
来源：http://fsx.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://clu.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://dil.yj20258888.top

int a = 10; printf("%d\n", a);
来源：http://mkf.xziqi.cn

[S03] C：读入整数
来源：http://lwq.yj202588.top

int x; scanf("%d", &x);
来源：http://jrl.jinghuilouyu.cn

[S04] C：字符串复制
来源：http://woz.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://myr.yonumen.top

[S05] C：字符串长度
来源：http://bad.zycfv.cn

strlen(s)
来源：http://zpu.xuetiantiany.cn

[S06] C：字符串比较
来源：http://jpk.ybcxt.top

strcmp(a, b) == 0
来源：http://tih.chenzaomai.com

[S07] C：数组遍历求和
来源：http://rkc.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fpf.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://xrq.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xah.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://jrr.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qgi.nwbrower.top

[S10] C：指针与解引用
来源：http://bhn.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://wsa.vehdjk.com

[S11] C：逐行读文件
来源：http://eib.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://uco.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yjw.hnxiangtu.top

fclose(f);
来源：http://qlf.jianghu66.top

[S12] C：写文件
来源：http://hij.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wma.dianchejie.cn

[S13] C：宏定义
来源：http://aav.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lhm.haohaochexian.top

[S14] C：枚举
来源：http://nej.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://zkr.zhongyouzk.top

[S15] C：类型转换
来源：http://paf.vqdsnc.cn

(double) a / b
来源：http://blo.smart0.xyz

[S16] C：位操作置位
来源：http://omd.shzxlz.cn

x |= (1 << 3);
来源：http://djm.ybcxt.top

[S17] C：安全拼接字符串
来源：http://nzt.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dyv.birdmap.top

[S18] C：命令行参数
来源：http://tbj.hfpthk.cn

int main(int argc, char **argv)
来源：http://aow.zhoulong.xyz

[S19] C：快速排序
来源：http://eco.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://oey.zhoulong.xyz

[S20] C：二分查找
来源：http://knx.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bnz.fehbvm.com

[S21] C：字符类别判断
来源：http://mkw.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jgw.0kj1m.cn

[S22] C：字符串转数字
来源：http://wbg.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://ftn.daxiang520.top

[S23] C：随机数
来源：http://twx.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dwe.sxryk.cn

[S24] C：获取本地时间
来源：http://wii.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://geo.yvedp.cn

[S25] C：内存拷贝
来源：http://vfb.zycfv.cn

memcpy(dst, src, n);
来源：http://dkt.epnwcf.com

[S26] C：内存清零
来源：http://wgq.hcnkem.com

memset(a, 0, sizeof a);
来源：http://pab.andypj.xyz

[S27] C：定义常量
来源：http://ayk.hcnkem.com

const double PI = 3.14159;
来源：http://uke.hnxiangtu.top

[S28] C：静态变量
来源：http://wsd.chenlongwang.top

static int counter = 0;
来源：http://puu.ybcxt.top

[S29] C：变参函数
来源：http://gdp.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xhz.guannengcc.top

[S30] C：头文件保护
来源：http://opq.jinghuilouyu.cn

#ifndef X_H
来源：http://mht.jyoumei.cn

#define X_H
来源：http://ixw.kuanghao11.cn

#endif
来源：http://nkh.zdqjudy.top

[S31] C++：Hello World
来源：http://jvh.zhengqikj.top

#include <iostream>
来源：http://rfs.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://sjx.xylfe.cn

[S32] C++：字符串
来源：http://qnk.tarul.cn

std::string s = "hi";  s += "!";
来源：http://vxn.gogol.net.cn

[S33] C++：vector 增删
来源：http://shm.pengpengdd.cyou

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ckr.xuanzx.com

[S34] C++：遍历 vector
来源：http://wae.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://yxw.iojbl.cn

[S35] C++：map
来源：http://vbt.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tqr.mhx1999.top

[S36] C++：unordered_map
来源：http://oxp.shanyushiyangtech.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hsw.aibaodan.cn

[S37] C++：set
来源：http://wnx.zycfv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qsq.fehbvm.com

[S38] C++：排序
来源：http://zpq.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://wrx.smart0.xyz

[S39] C++：自定义比较器排序
来源：http://tyg.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yez.hesvh.cn

[S40] C++：查找元素
来源：http://riq.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rpr.meibo888.top

[S41] C++：类与构造函数
来源：http://ghd.wangshuangyany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jre.nwbrower.top

[S42] C++：继承与虚函数
来源：http://exs.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://gms.epnwcf.com

[S43] C++：智能指针
来源：http://ffj.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://ovq.zhengqikj.top

[S44] C++：引用传参
来源：http://gxj.redwolf501.top

void inc(int &x) { ++x; }
来源：http://eom.nanxuanxn.top

[S45] C++：lambda
来源：http://cgw.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tqc.cheryme.top

[S46] C++：函数模板
来源：http://wos.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qmv.bjfxy.top

[S47] C++：结构化绑定遍历
来源：http://lud.pengpengdd.cyou

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jwp.gotoacloud.top

[S48] C++：逐行读文件
来源：http://lhq.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://mdk.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://gxk.daria6918.cn

[S49] C++：写文件
来源：http://hhj.hywenlv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://llg.sxryk.cn

[S50] C++：格式化数字
来源：http://cba.yanxiufei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tbw.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://utz.hammf.cn

static_cast<double>(a) / b
来源：http://ybf.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://ojc.52xcode.cn

int size() const noexcept { return n_; }
来源：http://mdg.feifeiyinyue.top

[S53] C++：移动语义
来源：http://jht.52xcode.cn

std::vector<int> w = std::move(v);
来源：http://kbo.sufxvd.cn

[S54] C++：异常处理
来源：http://nhj.andypj.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://byp.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://sqv.jinqigufen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lzk.yvedp.cn

[S56] C++：optional
来源：http://qak.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ckf.yj20258888.top

[S57] C++：编译期常量
来源：http://ypj.hfpthk.cn

constexpr int N = 10;
来源：http://pbb.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://foo.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://nwh.pengpengdd.cyou

[S59] C++：静态断言
来源：http://fml.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://izv.tanke756.top

[S60] C++：遍历并删除元素
来源：http://dso.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qve.epnwcf.com

================================================================================
来源：http://pcz.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jju.aibaodan.cn

================================================================================
来源：http://rpo.havefunace.top

[T01] Kotlin：Hello World
来源：http://bnq.fengsongda.top

println("Hello")
来源：http://nrm.vqdsnc.cn

[T02] Kotlin：变量
来源：http://pvf.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nrv.birdmap.top

[T03] Kotlin：字符串模板
来源：http://jiy.gotoacloud.top

"值: $b"
来源：http://xzv.hesvh.cn

[T04] Kotlin：空安全
来源：http://rov.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://rdm.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://hxr.52xcode.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gpv.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://vlq.hfpthk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pjs.smart0.xyz

[T07] Kotlin：集合过滤
来源：http://efa.hfpthk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yit.shangyingyoupin.top

[T08] Kotlin：数据类
来源：http://gql.gaohongyu789.top

data class User(val name: String, val age: Int)
来源：http://lsh.yfazqb.com

[T09] Kotlin：扩展函数
来源：http://zfg.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://vgj.316326.xyz

[T10] Kotlin：默认参数
来源：http://cvh.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yom.jlsjyb.cn

[T11] Kotlin：协程
来源：http://ysm.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qbe.tian-w.cn

[T12] Kotlin：解构声明
来源：http://jkj.gzhubu.top

val (a, b) = Pair(1, 2)
来源：http://tkx.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://pbb.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://zkl.smart0.xyz

[T14] Kotlin：循环
来源：http://ore.yongpay.top

for (i in 1..10) println(i)
来源：http://azg.ivvv.top

[T15] Kotlin：接口
来源：http://edn.dashuyun.cn

interface Shape { fun area(): Double }
来源：http://mmr.yj20258888.top

[T16] Swift：Hello World
来源：http://pdb.sjlbkw.cn

print("Hello")
来源：http://hhz.yanxiufei.cn

[T17] Swift：变量与常量
来源：http://pel.ydjk.org.cn

var a = 1;  let b = 2
来源：http://hkv.yj20258888.top

[T18] Swift：字符串插值
来源：http://odu.hcnkem.com

"值: \(b)"
来源：http://ija.zhixingplan.top

[T19] Swift：可选绑定
来源：http://lxw.pycfn.com

if let n = opt { print(n) }
来源：http://tml.dashuyun.cn

[T20] Swift：数组操作
来源：http://rsc.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dqy.hcnkem.com

[T21] Swift：遍历
来源：http://lve.yonumen.top

for x in a { print(x) }
来源：http://xed.wangdashe.top

[T22] Swift：字典
来源：http://pni.ydjk.org.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yta.pengpengdd.cyou

[T23] Swift：函数
来源：http://irv.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iop.xuetiantiany.cn

[T24] Swift：闭包
来源：http://xmg.tanke756.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://oxy.yuanzhike.top

[T25] Swift：结构体
来源：http://tcy.yj20258.top

struct P { var x: Int }
来源：http://jhu.daria6918.cn

[T26] Swift：类与重写
来源：http://jqd.cucudq.cn

class A: Base { override func f() {} }
来源：http://nnd.birdmap.top

[T27] Swift：错误处理
来源：http://tmp.yfazqb.com

do { try f() } catch { print(error) }
来源：http://qsl.hywenlv.cn

[T28] Swift：枚举
来源：http://pxj.fehbvm.com

enum Color { case red, green }
来源：http://zpx.jqgufenzy.top


<!-- 参考信息 -->