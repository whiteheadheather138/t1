代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hna.daria6918.cn

[R30] 函数返回状态码
来源：http://nrl.zycfv.cn

f() { return 0; }; f || echo "失败了"
来源：http://hin.fanxiaobao.xyz

[R31] 局部变量
来源：http://okx.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://ybh.yanxiufei.cn

[R32] 参数个数校验
来源：http://cxy.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yof.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://sfo.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://seb.svipenyu.cn

[R34] 退出时清理
来源：http://tws.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tom.sweek.top

[R35] 后台执行并等待
来源：http://vpo.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fgl.fanxiaobao.xyz

[R36] 并发执行多个任务
来源：http://rrj.hesvh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ibf.yj20258.top

[R37] 把输出赋给变量
来源：http://jnx.dianchejie.cn

files=$(ls -1)
来源：http://ycq.yuxming.cn

[R38] 管道串联
来源：http://tlv.pengpengdd.cyou

cat a.txt | grep -i error | wc -l
来源：http://edx.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://chl.dashuyun.cn

cmd > out.log 2>&1
来源：http://qqq.zhijiandao.cn

[R40] 追加写日志
来源：http://qym.zhongyouzk.top

echo "log" >> out.log
来源：http://lxd.jinghuilouyu.cn

[R41] 丢弃输出
来源：http://gxl.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://qfc.fehbvm.com

[R42] 输入重定向
来源：http://faw.jinyuanbaomall.cn

wc -l < a.txt
来源：http://alq.nwbrower.top

[R43] 按名字查找文件
来源：http://myw.ehwqpu.com

find . -name "*.log" -type f
来源：http://fmt.havefunace.top

[R44] 按修改时间查找
来源：http://wru.aibaodan.cn

find . -mtime -7 -type f
来源：http://myp.wangshuangyany.cn

[R45] 批量删除
来源：http://leh.hammf.cn

find . -name "*.tmp" -delete
来源：http://flz.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://nkp.ywan-chungtsiang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bcy.jinghuilouyu.cn

[R47] sed 单行替换
来源：http://xsl.tanke756.top

sed -i 's/foo/bar/g' a.txt
来源：http://xkq.xuetiantiany.cn

[R48] awk 取指定列
来源：http://pax.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://hxi.nanxinkj.top

[R49] awk 带条件
来源：http://axl.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bcb.zhixingplan.top

[R50] awk 求和
来源：http://jyi.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wyc.shzxlz.cn

[R51] 排序去重取前几
来源：http://qfj.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gbt.redwolf501.top

[R52] 统计行数
来源：http://bvj.cucudq.cn

wc -l a.txt
来源：http://uvl.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://zle.vqdsnc.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xwn.aizwys.cn

[R54] 比较两个文件
来源：http://lsr.yueranfly.top

diff a.txt b.txt
来源：http://opa.sweek.top

[R55] 压缩与解压
来源：http://uwk.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nif.shuidangran.top

[R56] 远程拷贝
来源：http://hiq.jyoumei.cn

scp file user@host:/path/
来源：http://twr.jinqigfzy.top

[R57] 远程执行命令
来源：http://edp.nwbrower.top

ssh user@host 'uptime'
来源：http://tlh.tanke756.top

[R58] 下载文件
来源：http://uda.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jns.shzxlz.cn

[R59] 发 POST JSON
来源：http://kpa.ehwqpu.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://puh.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://yuj.zhaomingkeji.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yjk.chenjidiqi.icu

[R61] 磁盘占用
来源：http://ott.ctjpmb.com

df -h;  du -sh *
来源：http://hgy.52xcode.cn

[R62] 找最占空间的文件
来源：http://hnb.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://bbk.yangfankeji.com

[R63] 内存与进程
来源：http://xez.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://vzq.vehdjk.com

[R64] 结束进程
来源：http://dmv.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://toc.9152youxi.cn

[R65] 查看端口占用
来源：http://gff.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xsl.feifeiyinyue.top

[R66] 定时任务
来源：http://qht.nwbrower.top

crontab -e;  crontab -l
来源：http://kgi.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://lya.jinqigfzy.top

openssl rand -hex 16
来源：http://cle.hnxiangtu.top

[R68] 计算文件校验值
来源：http://gpg.smart0.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://laa.pengpengdd.cyou

[R69] 生成随机密码
来源：http://epu.yj202588.top

head -c 16 /dev/urandom | base64
来源：http://cgn.nanxinkj.top

[R70] 时间戳与互转
来源：http://yxo.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://rwq.shuidangran.top

[R71] 日期格式化
来源：http://nel.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jjw.snrcjt.cn

[R72] 等待端口就绪
来源：http://huz.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://sok.hongshengwenyu.top

[R73] 分割大日志
来源：http://eub.birdmap.top

split -l 1000 big.log part_
来源：http://efn.bjfxy.top

[R74] 批量重命名
来源：http://ojh.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://awa.hnqzz.top

[R75] 导出环境变量
来源：http://mvp.daria6918.cn

export PATH="$HOME/bin:$PATH"
来源：http://qoj.bjfxy.top

[R76] 使用临时文件
来源：http://ymg.zycfv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ewc.hcnkem.com

[R77] 读取用户输入
来源：http://nwn.tarul.cn

read -rp "请输入: " ans
来源：http://ssm.nwbrower.top

[R78] 交互式菜单
来源：http://rmc.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://upa.vqdsnc.cn

[R79] 解析命令行选项
来源：http://sbx.xuanzx.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://poz.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://spd.tanke756.top

time ./run.sh
来源：http://zbk.hywenlv.cn

================================================================================
来源：http://fvp.hnxiangtu.top

S. C / C++ 专题
来源：http://bwk.kuanghao11.cn

================================================================================
来源：http://gwk.zhixingplan.top

[S01] C：Hello World
来源：http://mxo.hcnkem.com

#include <stdio.h>
来源：http://rqc.ppjwa.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tpk.birdmap.top

[S02] C：变量与格式化输出
来源：http://oqm.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://vfp.fktsv.cn

[S03] C：读入整数
来源：http://pie.jinqigufen.top

int x; scanf("%d", &x);
来源：http://idj.shangyingyoupin.top

[S04] C：字符串复制
来源：http://sao.nwbrower.top

char dst[32]; strcpy(dst, "hi");
来源：http://pxz.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://zsg.yangfankeji.com

strlen(s)
来源：http://crm.ehwqpu.com

[S06] C：字符串比较
来源：http://ceu.zhixingplan.top

strcmp(a, b) == 0
来源：http://gni.yuanzhike.top

[S07] C：数组遍历求和
来源：http://ujj.gaohongyu789.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kpr.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://hub.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sbs.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://jzf.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ktd.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://hty.hnqzz.top

int *p = &a;  *p = 5;
来源：http://yhd.daxiang520.top

[S11] C：逐行读文件
来源：http://nex.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://wok.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://srx.yvedp.cn

fclose(f);
来源：http://sik.gzhubu.top

[S12] C：写文件
来源：http://rin.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wrr.birdmap.top

[S13] C：宏定义
来源：http://wrw.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jsz.jinghuilouyu.cn

[S14] C：枚举
来源：http://mik.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://opn.ydzc1.top

[S15] C：类型转换
来源：http://pmg.zhoulong.xyz

(double) a / b
来源：http://sfw.nanxinkj.top

[S16] C：位操作置位
来源：http://aid.jqgfzy.top

x |= (1 << 3);
来源：http://pyx.mhx1999.top

[S17] C：安全拼接字符串
来源：http://zzs.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nqz.yfazqb.com

[S18] C：命令行参数
来源：http://omg.bbcook.cn

int main(int argc, char **argv)
来源：http://krk.0kj1m.cn

[S19] C：快速排序
来源：http://wdv.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://eai.uphjek.com

[S20] C：二分查找
来源：http://kqq.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fkr.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://uwh.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ozb.meibo888.top

[S22] C：字符串转数字
来源：http://kvn.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ecd.hfpthk.cn

[S23] C：随机数
来源：http://brh.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://grd.zhixingplan.top

[S24] C：获取本地时间
来源：http://cac.cucudq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oft.redwolf501.top

[S25] C：内存拷贝
来源：http://zwh.c1oappe.top

memcpy(dst, src, n);
来源：http://zqe.guowangkeji.top

[S26] C：内存清零
来源：http://wrl.nanxuanxn.top

memset(a, 0, sizeof a);
来源：http://byk.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://xpr.chenjidiqi.icu

const double PI = 3.14159;
来源：http://ptx.jinghuilouyu.cn

[S28] C：静态变量
来源：http://ixz.jlsjyb.cn

static int counter = 0;
来源：http://tkp.bbcook.cn

[S29] C：变参函数
来源：http://tpa.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jdd.zhijiandao.cn

[S30] C：头文件保护
来源：http://psm.chenzaomai.com

#ifndef X_H
来源：http://imr.chenlongwang.top

#define X_H
来源：http://ueg.jiagoushi.top

#endif
来源：http://rxg.ivvv.top

[S31] C++：Hello World
来源：http://ttq.cqqwz.cn

#include <iostream>
来源：http://ala.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://oyj.vehdjk.com

[S32] C++：字符串
来源：http://nwh.zhixingplan.top

std::string s = "hi";  s += "!";
来源：http://kdk.ehwqpu.com

[S33] C++：vector 增删
来源：http://tuq.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nhq.sysykeji.top

[S34] C++：遍历 vector
来源：http://qml.meibo888.top

for (auto &x : v) { std::cout << x; }
来源：http://ihf.yvedp.cn

[S35] C++：map
来源：http://kfr.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mir.tianlin.xyz

[S36] C++：unordered_map
来源：http://zxn.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zmh.xuetiantiany.cn

[S37] C++：set
来源：http://rvx.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vmq.gaohongyu789.top

[S38] C++：排序
来源：http://sdt.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://bxu.gogol.net.cn

[S39] C++：自定义比较器排序
来源：http://kui.snrcjt.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dpm.haohaochexian.top

[S40] C++：查找元素
来源：http://lza.haohaochexian.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ifm.zhiwuduotai.top

[S41] C++：类与构造函数
来源：http://chh.dashuyun.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mla.52xcode.cn

[S42] C++：继承与虚函数
来源：http://bis.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://qej.vqdsnc.cn

[S43] C++：智能指针
来源：http://fav.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://gat.cdnleiting.top

[S44] C++：引用传参
来源：http://knd.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://fsy.sufxvd.cn

[S45] C++：lambda
来源：http://omz.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://qgr.cdnleiting.top

[S46] C++：函数模板
来源：http://ibt.0kj1m.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wdt.mhx1999.top

[S47] C++：结构化绑定遍历
来源：http://avh.zhaomingkeji.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xpk.jiagoushi.top

[S48] C++：逐行读文件
来源：http://dde.chenlongwang.top

std::ifstream in("a.txt");  std::string line;
来源：http://bpl.yueranfly.top

while (std::getline(in, line)) { }
来源：http://euu.ppjwa.cn

[S49] C++：写文件
来源：http://unu.daria6918.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mgb.bbcook.cn

[S50] C++：格式化数字
来源：http://fuk.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qpp.hywenlv.cn

[S51] C++：显式类型转换
来源：http://cgv.ppjwa.cn

static_cast<double>(a) / b
来源：http://icx.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://oya.birdmap.top

int size() const noexcept { return n_; }
来源：http://csm.zdbjq.cn

[S53] C++：移动语义
来源：http://fdb.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://cke.sweek.top

[S54] C++：异常处理
来源：http://enp.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ywy.yuanzhike.top

[S55] C++：结构化绑定
来源：http://hhp.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://krj.cheryme.top

[S56] C++：optional
来源：http://vmh.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://syq.nanxuanxn.top

[S57] C++：编译期常量
来源：http://qik.jianghu66.top

constexpr int N = 10;
来源：http://qpa.yj20258888.top

[S58] C++：命名空间
来源：http://ztj.nwbrower.top

namespace ns { int f() { return 1; } }
来源：http://npi.hammf.cn

[S59] C++：静态断言
来源：http://qxg.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vly.dianchejie.cn

[S60] C++：遍历并删除元素
来源：http://wdj.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mln.ybcxt.top

================================================================================
来源：http://vrx.ybcxt.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yvc.redwolf501.top

================================================================================
来源：http://hkp.ydzc1.top

[T01] Kotlin：Hello World
来源：http://kfc.guowangkeji.top

println("Hello")
来源：http://zqb.hongshengwenyu.top

[T02] Kotlin：变量
来源：http://ych.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qzv.nwbrower.top

[T03] Kotlin：字符串模板
来源：http://ohz.ywan-chungtsiang.top

"值: $b"
来源：http://qww.cashguo.top

[T04] Kotlin：空安全
来源：http://vih.meibo888.top

val n: String? = null;  n?.length
来源：http://akg.yangfankeji.com

[T05] Kotlin：when 表达式
来源：http://yhu.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pex.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://ybm.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pcy.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://ygk.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bgx.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://cur.gogol.net.cn

data class User(val name: String, val age: Int)
来源：http://anw.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://mga.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://anf.c1oappe.top

[T10] Kotlin：默认参数
来源：http://fqx.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://axe.shuidangran.top

[T11] Kotlin：协程
来源：http://zzf.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://snt.shangyingyoupin.top

[T12] Kotlin：解构声明
来源：http://ebm.hnxiangtu.top

val (a, b) = Pair(1, 2)
来源：http://blc.shzxlz.cn

[T13] Kotlin：只读 Map
来源：http://wqc.pycfn.com

val m = mapOf("a" to 1)
来源：http://gqw.zhijiandao.cn

[T14] Kotlin：循环
来源：http://whz.ivvv.top

for (i in 1..10) println(i)
来源：http://bfa.cqqwz.cn

[T15] Kotlin：接口
来源：http://uew.jlsjyb.cn

interface Shape { fun area(): Double }
来源：http://rdo.hywenlv.cn

[T16] Swift：Hello World
来源：http://xik.sysykeji.top

print("Hello")
来源：http://pfv.zdbjq.cn

[T17] Swift：变量与常量
来源：http://zij.jianghu66.top

var a = 1;  let b = 2
来源：http://tby.tianlin.xyz

[T18] Swift：字符串插值
来源：http://heg.hnqzz.top

"值: \(b)"
来源：http://jod.shuidangran.top

[T19] Swift：可选绑定
来源：http://bdf.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://apb.daria6918.cn

[T20] Swift：数组操作
来源：http://hrg.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://fmu.jlsjyb.cn

[T21] Swift：遍历
来源：http://ssd.gotoacloud.top

for x in a { print(x) }
来源：http://tzi.sjlbkw.cn

[T22] Swift：字典
来源：http://zdz.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hym.zhiwuduotai.top

[T23] Swift：函数
来源：http://dmr.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rxr.yongpay.top

[T24] Swift：闭包
来源：http://ioh.xylfe.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xcq.gzhubu.top

[T25] Swift：结构体
来源：http://pyu.yanxiufei.cn

struct P { var x: Int }
来源：http://soa.daria6918.cn

[T26] Swift：类与重写
来源：http://iio.0kj1m.cn

class A: Base { override func f() {} }
来源：http://sdk.feifeiyinyue.top

[T27] Swift：错误处理
来源：http://wmx.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://hib.jinqigfzy.top

[T28] Swift：枚举
来源：http://dti.yanxiufei.cn

enum Color { case red, green }
来源：http://ggu.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://xpd.tianlin.xyz

guard let x = opt else { return }
来源：http://pxw.jinqigfzy.top

[T30] Swift：协议
来源：http://ero.aibaodan.cn

protocol Shape { func area() -> Double }
来源：http://van.nwbrower.top

[T31] Lua：Hello World
来源：http://asm.xuanzx.com

print("Hello")
来源：http://hwh.sysykeji.top

[T32] Lua：局部变量
来源：http://fqb.ydzc1.top

local a = 1
来源：http://auv.zhijiandao.cn


<!-- 参考信息 -->