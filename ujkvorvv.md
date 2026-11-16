代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://ukz.cqqwz.cn

[R32] 参数个数校验
来源：http://vby.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zxq.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://wuo.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://akr.xuetiantiany.cn

[R34] 退出时清理
来源：http://dhf.daria6918.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tac.hesvh.cn

[R35] 后台执行并等待
来源：http://zzb.ybcxt.top

sleep 5 & pid=$!; wait "$pid"
来源：http://crk.guannengcc.top

[R36] 并发执行多个任务
来源：http://ykt.gaohongyu789.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ysu.chenlongwang.top

[R37] 把输出赋给变量
来源：http://orq.hnxiangtu.top

files=$(ls -1)
来源：http://aay.cdnleiting.top

[R38] 管道串联
来源：http://qma.yuxming.cn

cat a.txt | grep -i error | wc -l
来源：http://jid.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://syh.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://eob.52xcode.cn

[R40] 追加写日志
来源：http://zlv.aizwys.cn

echo "log" >> out.log
来源：http://hot.xziqi.cn

[R41] 丢弃输出
来源：http://gnn.nwbrower.top

cmd >/dev/null 2>&1
来源：http://kuj.yuxming.cn

[R42] 输入重定向
来源：http://dlb.jqgufenzy.top

wc -l < a.txt
来源：http://zhv.sjlbkw.cn

[R43] 按名字查找文件
来源：http://ocj.tanke756.top

find . -name "*.log" -type f
来源：http://lpd.fktsv.cn

[R44] 按修改时间查找
来源：http://xba.ydzc1.top

find . -mtime -7 -type f
来源：http://oyg.yanxiufei.cn

[R45] 批量删除
来源：http://vpe.zhoulong.xyz

find . -name "*.tmp" -delete
来源：http://mdx.zhengqikj.top

[R46] 递归替换文件内容
来源：http://dqj.yuxming.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bvj.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://xei.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gwa.nanxinkj.top

[R48] awk 取指定列
来源：http://ckf.vehdjk.com

awk '{print $1, $3}' a.txt
来源：http://bwd.ywan-chungtsiang.top

[R49] awk 带条件
来源：http://vbt.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hgj.bjfxy.top

[R50] awk 求和
来源：http://rsx.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zst.chenlongwang.top

[R51] 排序去重取前几
来源：http://wyw.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://emm.sysykeji.top

[R52] 统计行数
来源：http://pdr.redwolf501.top

wc -l a.txt
来源：http://ceu.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://bii.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://etr.shangyingyoupin.top

[R54] 比较两个文件
来源：http://nvq.shanyushiyangtech.top

diff a.txt b.txt
来源：http://kts.tianlin.xyz

[R55] 压缩与解压
来源：http://mit.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bjd.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://sdr.gogol.net.cn

scp file user@host:/path/
来源：http://ajb.shuidangran.top

[R57] 远程执行命令
来源：http://lpe.tanke756.top

ssh user@host 'uptime'
来源：http://qpg.haohaochexian.top

[R58] 下载文件
来源：http://hsq.jinqigufen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://exj.tarul.cn

[R59] 发 POST JSON
来源：http://umq.shanyushiyangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oxh.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://tbc.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bfe.ivvv.top

[R61] 磁盘占用
来源：http://hci.c1oappe.top

df -h;  du -sh *
来源：http://tst.ppjwa.cn

[R62] 找最占空间的文件
来源：http://ysb.yanxiufei.cn

du -ah . | sort -rh | head -10
来源：http://lum.jinqigfzy.top

[R63] 内存与进程
来源：http://yye.xziqi.cn

free -h;  ps aux | grep nginx
来源：http://ekb.ctjpmb.com

[R64] 结束进程
来源：http://wwl.yfazqb.com

kill -9 $(pgrep -f app.py)
来源：http://pxv.aizwys.cn

[R65] 查看端口占用
来源：http://iad.cashguo.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ifw.snrcjt.cn

[R66] 定时任务
来源：http://txr.yanxiufei.cn

crontab -e;  crontab -l
来源：http://nur.birdmap.top

[R67] 生成随机十六进制串
来源：http://nwu.yj20258.top

openssl rand -hex 16
来源：http://qka.vehdjk.com

[R68] 计算文件校验值
来源：http://qkf.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qqh.cashguo.top

[R69] 生成随机密码
来源：http://gik.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://szk.shanyushiyangkeji.top

[R70] 时间戳与互转
来源：http://zpz.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://nee.hongshengwenyu.top

[R71] 日期格式化
来源：http://ece.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ymz.fzhhl.top

[R72] 等待端口就绪
来源：http://lkh.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gre.epnwcf.com

[R73] 分割大日志
来源：http://san.jinqigfzy.top

split -l 1000 big.log part_
来源：http://hpq.nanxinkj.top

[R74] 批量重命名
来源：http://eap.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jrs.guowangkeji.top

[R75] 导出环境变量
来源：http://ubo.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://fqu.cqqwz.cn

[R76] 使用临时文件
来源：http://omr.fktsv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sor.feifeiyinyue.top

[R77] 读取用户输入
来源：http://tuw.zhixingplan.top

read -rp "请输入: " ans
来源：http://ppd.hfpthk.cn

[R78] 交互式菜单
来源：http://hsw.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://wuh.tarul.cn

[R79] 解析命令行选项
来源：http://zcn.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hax.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://mpa.yuxming.cn

time ./run.sh
来源：http://yet.jinghuilouyu.cn

================================================================================
来源：http://trs.bjfxy.top

S. C / C++ 专题
来源：http://nyd.jianghu66.top

================================================================================
来源：http://inq.jinghuilouyu.cn

[S01] C：Hello World
来源：http://ols.fktsv.cn

#include <stdio.h>
来源：http://tzx.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mdu.0kj1m.cn

[S02] C：变量与格式化输出
来源：http://hbv.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://ovh.jlsjyb.cn

[S03] C：读入整数
来源：http://gxn.hywenlv.cn

int x; scanf("%d", &x);
来源：http://epq.daria6918.cn

[S04] C：字符串复制
来源：http://hrt.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://hbv.jyoumei.cn

[S05] C：字符串长度
来源：http://sot.andypj.xyz

strlen(s)
来源：http://uqp.tarul.cn

[S06] C：字符串比较
来源：http://yth.quarkkingdee.top

strcmp(a, b) == 0
来源：http://wse.bjfxy.top

[S07] C：数组遍历求和
来源：http://zel.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mcb.yonumen.top

[S08] C：动态内存分配与释放
来源：http://hvb.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nvn.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://hno.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uiq.316326.xyz

[S10] C：指针与解引用
来源：http://tzi.feifeiyinyue.top

int *p = &a;  *p = 5;
来源：http://zwj.52xcode.cn

[S11] C：逐行读文件
来源：http://giz.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://wgw.jiagoushi.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ehr.birdmap.top

fclose(f);
来源：http://hft.hywenlv.cn

[S12] C：写文件
来源：http://bfy.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nxy.snrcjt.cn

[S13] C：宏定义
来源：http://wgs.cashguo.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bma.kuanghao11.cn

[S14] C：枚举
来源：http://yyp.vehdjk.com

enum Color { RED, GREEN, BLUE };
来源：http://tiq.cheryme.top

[S15] C：类型转换
来源：http://uvq.jlsjyb.cn

(double) a / b
来源：http://qfn.meibo888.top

[S16] C：位操作置位
来源：http://gbo.haohaochexian.top

x |= (1 << 3);
来源：http://bvl.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://kvd.xuanzx.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://als.zdbjq.cn

[S18] C：命令行参数
来源：http://elj.zhengqikj.top

int main(int argc, char **argv)
来源：http://nur.haohaochexian.top

[S19] C：快速排序
来源：http://zsb.sxryk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dny.hywenlv.cn

[S20] C：二分查找
来源：http://dfx.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pdu.andypj.xyz

[S21] C：字符类别判断
来源：http://uhf.cucudq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://crr.tianlin.xyz

[S22] C：字符串转数字
来源：http://hvw.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://egk.smart0.xyz

[S23] C：随机数
来源：http://nfz.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bob.guowangkeji.top

[S24] C：获取本地时间
来源：http://vjz.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cdx.jiagoushi.top

[S25] C：内存拷贝
来源：http://mel.aibaodan.cn

memcpy(dst, src, n);
来源：http://aks.xuanzx.com

[S26] C：内存清零
来源：http://ywk.wangdashe.top

memset(a, 0, sizeof a);
来源：http://aur.bbcook.cn

[S27] C：定义常量
来源：http://bhn.ydzc1.top

const double PI = 3.14159;
来源：http://sos.hcnkem.com

[S28] C：静态变量
来源：http://dui.9152youxi.cn

static int counter = 0;
来源：http://zdz.ppjwa.cn

[S29] C：变参函数
来源：http://uza.quarkkingdee.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bzz.jyoumei.cn

[S30] C：头文件保护
来源：http://joz.hywenlv.cn

#ifndef X_H
来源：http://qqr.sysykeji.top

#define X_H
来源：http://erv.nwbrower.top

#endif
来源：http://uir.jianghu66.top

[S31] C++：Hello World
来源：http://agm.gotoacloud.top

#include <iostream>
来源：http://qly.fktsv.cn

int main() { std::cout << "Hello\n"; }
来源：http://yya.yj20258888.top

[S32] C++：字符串
来源：http://zjt.daria6918.cn

std::string s = "hi";  s += "!";
来源：http://ajl.tanke756.top

[S33] C++：vector 增删
来源：http://jsd.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jhd.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://kuu.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://sgw.zhixingplan.top

[S35] C++：map
来源：http://oad.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://swy.hongshengwenyu.top

[S36] C++：unordered_map
来源：http://ubo.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kcp.daxiang520.top

[S37] C++：set
来源：http://pyw.hongshengwenyu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gkm.yuxming.cn

[S38] C++：排序
来源：http://wwc.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://vnp.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://mqm.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zra.smart0.xyz

[S40] C++：查找元素
来源：http://wgx.jinyuanbaomall.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ntr.hywenlv.cn

[S41] C++：类与构造函数
来源：http://kcn.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ugb.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://gvq.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://kqf.epnwcf.com

[S43] C++：智能指针
来源：http://kfq.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://xvc.andypj.xyz

[S44] C++：引用传参
来源：http://tce.hnqzz.top

void inc(int &x) { ++x; }
来源：http://ney.nanxinkj.top

[S45] C++：lambda
来源：http://rng.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://mkm.0kj1m.cn

[S46] C++：函数模板
来源：http://hly.quarkkingdee.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jbs.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://blc.ywan-chungtsiang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rph.jianghu66.top

[S48] C++：逐行读文件
来源：http://ciz.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://rmh.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://brl.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://rmu.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lbb.ydzc1.top

[S50] C++：格式化数字
来源：http://dla.smart0.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lhv.sxryk.cn

[S51] C++：显式类型转换
来源：http://hpp.havefunace.top

static_cast<double>(a) / b
来源：http://zax.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://ulr.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://rha.yangfankeji.com

[S53] C++：移动语义
来源：http://ddp.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://lcz.sjlbkw.cn

[S54] C++：异常处理
来源：http://mqs.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iyz.yj202588.top

[S55] C++：结构化绑定
来源：http://tcu.birdmap.top

auto [a, b] = std::make_pair(1, 2);
来源：http://oit.chenlongwang.top

[S56] C++：optional
来源：http://vuj.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oen.gzhubu.top

[S57] C++：编译期常量
来源：http://awg.tanke756.top

constexpr int N = 10;
来源：http://lel.yueranfly.top

[S58] C++：命名空间
来源：http://xxi.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://tei.gaohongyu789.top

[S59] C++：静态断言
来源：http://hkd.zdqjudy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vvc.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://ydu.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pcp.jyoumei.cn

================================================================================
来源：http://iyf.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ubs.xingfuxueyuan.xyz

================================================================================
来源：http://gdp.jinqigufen.top

[T01] Kotlin：Hello World
来源：http://tao.cheryme.top

println("Hello")
来源：http://kkc.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://knj.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qlu.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://crl.cashguo.top

"值: $b"
来源：http://xkk.ydzc1.top

[T04] Kotlin：空安全
来源：http://txy.zhixingplan.top

val n: String? = null;  n?.length
来源：http://fkc.birdmap.top

[T05] Kotlin：when 表达式
来源：http://ioz.hfpthk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nsb.bjfxy.top

[T06] Kotlin：集合映射
来源：http://ibe.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yat.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://apw.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tli.52xcode.cn

[T08] Kotlin：数据类
来源：http://iqt.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://ige.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://erc.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://fgh.zhoulong.xyz

[T10] Kotlin：默认参数
来源：http://taq.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ecb.chenlongwang.top

[T11] Kotlin：协程
来源：http://ljf.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://inj.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://wgb.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://rho.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://wxd.yfazqb.com

val m = mapOf("a" to 1)
来源：http://puu.yonumen.top

[T14] Kotlin：循环
来源：http://ekk.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://wsb.xinyue.icu

[T15] Kotlin：接口
来源：http://ixc.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://srz.epnwcf.com

[T16] Swift：Hello World
来源：http://qjb.zdqjudy.top

print("Hello")
来源：http://lmz.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://mvp.xziqi.cn

var a = 1;  let b = 2
来源：http://dxq.xuanzx.com

[T18] Swift：字符串插值
来源：http://nbv.yj202588.top

"值: \(b)"
来源：http://sgs.sysykeji.top

[T19] Swift：可选绑定
来源：http://xfj.zdqjudy.top

if let n = opt { print(n) }
来源：http://czz.zhixingplan.top

[T20] Swift：数组操作
来源：http://gtd.dashuyun.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pmz.cheryme.top

[T21] Swift：遍历
来源：http://ovy.yj20258.top

for x in a { print(x) }
来源：http://uec.ctjpmb.com

[T22] Swift：字典
来源：http://jmz.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://lml.chenjidiqi.icu

[T23] Swift：函数
来源：http://ohb.jiagoushi.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tsp.uphjek.com

[T24] Swift：闭包
来源：http://dos.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bsy.snrcjt.cn

[T25] Swift：结构体
来源：http://gle.redwolf501.top

struct P { var x: Int }
来源：http://lft.andypj.xyz

[T26] Swift：类与重写
来源：http://udn.ivvv.top

class A: Base { override func f() {} }
来源：http://njw.meibo888.top

[T27] Swift：错误处理
来源：http://mef.bjfxy.top

do { try f() } catch { print(error) }
来源：http://cnm.zdqjudy.top

[T28] Swift：枚举
来源：http://fnv.zhongyouzk.top

enum Color { case red, green }
来源：http://hhx.fanxiaobao.xyz

[T29] Swift：guard 提前返回
来源：http://suz.ybcxt.top

guard let x = opt else { return }
来源：http://mpu.nanxuanxn.top

[T30] Swift：协议
来源：http://nya.meibo888.top

protocol Shape { func area() -> Double }
来源：http://egw.nwbrower.top

[T31] Lua：Hello World
来源：http://jeu.yonumen.top

print("Hello")
来源：http://yyp.zhongyouzk.top

[T32] Lua：局部变量
来源：http://fcw.ivvv.top

local a = 1
来源：http://lpj.fehbvm.com

[T33] Lua：表（数组）
来源：http://qux.jinqigufen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://upj.jlsjyb.cn

[T34] Lua：遍历表
来源：http://xib.vehdjk.com

for i, v in ipairs(t) do print(i, v) end
来源：http://zbm.shanyushiyangtech.top


<!-- 参考信息 -->