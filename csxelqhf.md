代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://tnr.shzxlz.cn

[R26] 命令替换
来源：http://qnr.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://xue.tanke756.top

[R27] 算术展开
来源：http://kvo.sjlbkw.cn

echo $((1 + 2 * 3))
来源：http://rij.hysaishi.cn

[R28] 浮点运算
来源：http://fun.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://mgc.haohaochexian.top

[R29] 定义函数
来源：http://pth.nanxinkj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uqc.ydzc1.top

[R30] 函数返回状态码
来源：http://jkc.ivvv.top

f() { return 0; }; f || echo "失败了"
来源：http://lro.zhiwuduotai.top

[R31] 局部变量
来源：http://yib.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://beu.9152youxi.cn

[R32] 参数个数校验
来源：http://hdf.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pbw.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://mrn.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://liz.yj202588.top

[R34] 退出时清理
来源：http://pnw.xuetiantiany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jag.jiagoushi.top

[R35] 后台执行并等待
来源：http://irc.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mor.hcnkem.com

[R36] 并发执行多个任务
来源：http://egz.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://etp.cheryme.top

[R37] 把输出赋给变量
来源：http://wei.tian-w.cn

files=$(ls -1)
来源：http://fpx.fengsongda.top

[R38] 管道串联
来源：http://hmu.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://ldr.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://ukh.sufxvd.cn

cmd > out.log 2>&1
来源：http://hqy.feifeiyinyue.top

[R40] 追加写日志
来源：http://kpw.hcnkem.com

echo "log" >> out.log
来源：http://puh.redwolf501.top

[R41] 丢弃输出
来源：http://kkm.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://lvw.zhengqikj.top

[R42] 输入重定向
来源：http://khh.hammf.cn

wc -l < a.txt
来源：http://qar.xinyue.icu

[R43] 按名字查找文件
来源：http://deu.hammf.cn

find . -name "*.log" -type f
来源：http://waq.cheryme.top

[R44] 按修改时间查找
来源：http://lvd.jianghu66.top

find . -mtime -7 -type f
来源：http://dhq.gogol.net.cn

[R45] 批量删除
来源：http://ucj.hammf.cn

find . -name "*.tmp" -delete
来源：http://dvd.tarul.cn

[R46] 递归替换文件内容
来源：http://tkw.cqqwz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vko.svipenyu.cn

[R47] sed 单行替换
来源：http://xaj.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://zst.birdmap.top

[R48] awk 取指定列
来源：http://sca.ywan-chungtsiang.top

awk '{print $1, $3}' a.txt
来源：http://zft.shuidangran.top

[R49] awk 带条件
来源：http://phq.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aof.zhiwuduotai.top

[R50] awk 求和
来源：http://cdz.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://nwx.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://lwc.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sel.havefunace.top

[R52] 统计行数
来源：http://rst.shanyushiyangtech.top

wc -l a.txt
来源：http://xbn.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://eiu.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rav.ydjk.org.cn

[R54] 比较两个文件
来源：http://yox.shzxlz.cn

diff a.txt b.txt
来源：http://uiq.dashuyun.cn

[R55] 压缩与解压
来源：http://snn.zhijiandao.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ysq.yuanzhike.top

[R56] 远程拷贝
来源：http://cju.guannengcc.top

scp file user@host:/path/
来源：http://fak.mhx1999.top

[R57] 远程执行命令
来源：http://efa.yuxming.cn

ssh user@host 'uptime'
来源：http://gcv.shanyushiyangkeji.top

[R58] 下载文件
来源：http://gfa.ppjwa.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zcz.yfazqb.com

[R59] 发 POST JSON
来源：http://afa.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://myt.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://gmz.hesvh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wsk.redwolf501.top

[R61] 磁盘占用
来源：http://gwg.hammf.cn

df -h;  du -sh *
来源：http://jcs.9152youxi.cn

[R62] 找最占空间的文件
来源：http://hgs.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://zbo.cashguo.top

[R63] 内存与进程
来源：http://ane.hnqzz.top

free -h;  ps aux | grep nginx
来源：http://zyj.jinyuanbaomall.cn

[R64] 结束进程
来源：http://pkx.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://ems.sjlbkw.cn

[R65] 查看端口占用
来源：http://zql.feifeiyinyue.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gbd.zhixingplan.top

[R66] 定时任务
来源：http://uqx.zdqjudy.top

crontab -e;  crontab -l
来源：http://adw.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://uus.jinghuilouyu.cn

openssl rand -hex 16
来源：http://ikx.tarul.cn

[R68] 计算文件校验值
来源：http://kyk.shanyushiyangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://exr.zhixingplan.top

[R69] 生成随机密码
来源：http://dfk.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://yxc.xinyue.icu

[R70] 时间戳与互转
来源：http://urt.shzxlz.cn

date +%s;  date -d @1700000000
来源：http://hfq.nanxuanxn.top

[R71] 日期格式化
来源：http://azr.zhengqikj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jlf.ydzc1.top

[R72] 等待端口就绪
来源：http://nsu.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pzu.ybcxt.top

[R73] 分割大日志
来源：http://aug.zdqjudy.top

split -l 1000 big.log part_
来源：http://ilh.yj20258.top

[R74] 批量重命名
来源：http://xyx.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rnv.gotoacloud.top

[R75] 导出环境变量
来源：http://kib.hywenlv.cn

export PATH="$HOME/bin:$PATH"
来源：http://ofv.smart0.xyz

[R76] 使用临时文件
来源：http://oke.cqqwz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://njj.havefunace.top

[R77] 读取用户输入
来源：http://loe.ppjwa.cn

read -rp "请输入: " ans
来源：http://gkh.daxiang520.top

[R78] 交互式菜单
来源：http://nfu.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lxz.mhx1999.top

[R79] 解析命令行选项
来源：http://jsb.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sts.haohaochexian.top

[R80] 查看脚本执行耗时
来源：http://yoc.zhengqikj.top

time ./run.sh
来源：http://ner.fanxiaobao.xyz

================================================================================
来源：http://tfu.guannengcc.top

S. C / C++ 专题
来源：http://zck.hfpthk.cn

================================================================================
来源：http://gnh.cucudq.cn

[S01] C：Hello World
来源：http://qsx.jinqigufen.top

#include <stdio.h>
来源：http://akw.fktsv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pfi.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://pmo.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://jwu.hammf.cn

[S03] C：读入整数
来源：http://gsw.jianghu66.top

int x; scanf("%d", &x);
来源：http://dlm.quarkkingdee.top

[S04] C：字符串复制
来源：http://sfx.9152youxi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fkq.zhijiandao.cn

[S05] C：字符串长度
来源：http://tks.xuanzx.com

strlen(s)
来源：http://bxd.kuanghao11.cn

[S06] C：字符串比较
来源：http://avl.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://bua.vqdsnc.cn

[S07] C：数组遍历求和
来源：http://ark.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dbt.jyoumei.cn

[S08] C：动态内存分配与释放
来源：http://hni.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fwr.dashuyun.cn

[S09] C：结构体定义与初始化
来源：http://ycu.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://azz.daria6918.cn

[S10] C：指针与解引用
来源：http://hdk.sweek.top

int *p = &a;  *p = 5;
来源：http://zjb.yj20258888.top

[S11] C：逐行读文件
来源：http://anu.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://zrc.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fkh.ywan-chungtsiang.top

fclose(f);
来源：http://pqp.aibaodan.cn

[S12] C：写文件
来源：http://gux.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vtx.daxiang520.top

[S13] C：宏定义
来源：http://oyf.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bgs.wangdashe.top

[S14] C：枚举
来源：http://yjs.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://xwe.jlsjyb.cn

[S15] C：类型转换
来源：http://nho.iojbl.cn

(double) a / b
来源：http://jno.jqgufenzy.top

[S16] C：位操作置位
来源：http://bqc.yj202588.top

x |= (1 << 3);
来源：http://vks.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://epg.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://krg.chenlongwang.top

[S18] C：命令行参数
来源：http://kfs.mhx1999.top

int main(int argc, char **argv)
来源：http://obl.chenjidiqi.icu

[S19] C：快速排序
来源：http://ozl.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vyq.jianghu66.top

[S20] C：二分查找
来源：http://vkm.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dqe.hcnkem.com

[S21] C：字符类别判断
来源：http://ukd.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ysj.birdmap.top

[S22] C：字符串转数字
来源：http://mvr.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vgl.wangdashe.top

[S23] C：随机数
来源：http://luj.guannengcc.top

srand(time(NULL));  int r = rand() % 100;
来源：http://elf.yongpay.top

[S24] C：获取本地时间
来源：http://gpy.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ojo.daria6918.cn

[S25] C：内存拷贝
来源：http://rfl.cucudq.cn

memcpy(dst, src, n);
来源：http://miz.xziqi.cn

[S26] C：内存清零
来源：http://tdu.xuanzx.com

memset(a, 0, sizeof a);
来源：http://ktr.uphjek.com

[S27] C：定义常量
来源：http://zbn.dashuyun.cn

const double PI = 3.14159;
来源：http://xrw.sweek.top

[S28] C：静态变量
来源：http://nly.smart0.xyz

static int counter = 0;
来源：http://joz.shuidangran.top

[S29] C：变参函数
来源：http://knv.xuetiantiany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wsw.svipenyu.cn

[S30] C：头文件保护
来源：http://okz.shzxlz.cn

#ifndef X_H
来源：http://nfe.dianchejie.cn

#define X_H
来源：http://xmx.zhiwuduotai.top

#endif
来源：http://psu.gogol.net.cn

[S31] C++：Hello World
来源：http://opr.xinyue.icu

#include <iostream>
来源：http://wxo.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://tod.smart0.xyz

[S32] C++：字符串
来源：http://eil.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://ubr.andypj.xyz

[S33] C++：vector 增删
来源：http://frm.shanyushiyangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gbi.shangyingyoupin.top

[S34] C++：遍历 vector
来源：http://vbd.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://jjb.chenlongwang.top

[S35] C++：map
来源：http://gxz.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://asx.jianghu66.top

[S36] C++：unordered_map
来源：http://nhy.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ibq.shangyingyoupin.top

[S37] C++：set
来源：http://jfz.hongshengwenyu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vxg.yvedp.cn

[S38] C++：排序
来源：http://wfc.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://zbx.aibaodan.cn

[S39] C++：自定义比较器排序
来源：http://hlx.fengsongda.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sdy.vehdjk.com

[S40] C++：查找元素
来源：http://djk.havefunace.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ozh.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://iqk.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jzj.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://kcv.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://hhz.yuxming.cn

[S43] C++：智能指针
来源：http://waa.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://fkh.bbcook.cn

[S44] C++：引用传参
来源：http://jjv.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://mwa.yongpay.top

[S45] C++：lambda
来源：http://rsd.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://fyk.birdmap.top

[S46] C++：函数模板
来源：http://anp.xylfe.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eog.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://ouo.c1oappe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://erz.daria6918.cn

[S48] C++：逐行读文件
来源：http://wrz.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://omy.tian-w.cn

while (std::getline(in, line)) { }
来源：http://aur.shzxlz.cn

[S49] C++：写文件
来源：http://sgw.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pou.xziqi.cn

[S50] C++：格式化数字
来源：http://rge.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vuf.hnqzz.top

[S51] C++：显式类型转换
来源：http://hrh.hfpthk.cn

static_cast<double>(a) / b
来源：http://boz.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://dim.jiagoushi.top

int size() const noexcept { return n_; }
来源：http://xlf.0kj1m.cn

[S53] C++：移动语义
来源：http://kry.feifeiyinyue.top

std::vector<int> w = std::move(v);
来源：http://wbc.shzxlz.cn

[S54] C++：异常处理
来源：http://rjw.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yti.0kj1m.cn

[S55] C++：结构化绑定
来源：http://dcx.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gyj.yangfankeji.com

[S56] C++：optional
来源：http://tlw.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hlw.xziqi.cn

[S57] C++：编译期常量
来源：http://efz.bjfxy.top

constexpr int N = 10;
来源：http://qfy.uphjek.com

[S58] C++：命名空间
来源：http://img.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://sww.haohaochexian.top

[S59] C++：静态断言
来源：http://ofx.wangshuangyany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lpk.bjfxy.top

[S60] C++：遍历并删除元素
来源：http://bhh.chenzaomai.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qmb.zhaomingkeji.xyz

================================================================================
来源：http://dzq.xingfuxueyuan.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rlu.tianlin.xyz

================================================================================
来源：http://mof.quarkkingdee.top

[T01] Kotlin：Hello World
来源：http://jbk.ehwqpu.com

println("Hello")
来源：http://qsl.shanyushiyangkeji.top

[T02] Kotlin：变量
来源：http://zph.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://crn.havefunace.top

[T03] Kotlin：字符串模板
来源：http://azi.xingfuxueyuan.xyz

"值: $b"
来源：http://ijq.hnqzz.top

[T04] Kotlin：空安全
来源：http://bsx.uphjek.com

val n: String? = null;  n?.length
来源：http://olm.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://qrn.epnwcf.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nyx.316326.xyz

[T06] Kotlin：集合映射
来源：http://lib.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://asn.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://qor.hesvh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://erv.daxiang520.top

[T08] Kotlin：数据类
来源：http://xyx.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://ouq.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://pvd.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://iaj.fengsongda.top

[T10] Kotlin：默认参数
来源：http://dnl.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://ywf.quarkkingdee.top

[T11] Kotlin：协程
来源：http://voa.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://etk.aizwys.cn

[T12] Kotlin：解构声明
来源：http://jui.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://ekz.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://ezo.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://vte.shzxlz.cn

[T14] Kotlin：循环
来源：http://pxm.havefunace.top

for (i in 1..10) println(i)
来源：http://qsj.gzhubu.top

[T15] Kotlin：接口
来源：http://ddt.tian-w.cn

interface Shape { fun area(): Double }
来源：http://mha.fehbvm.com

[T16] Swift：Hello World
来源：http://tov.hnxiangtu.top

print("Hello")
来源：http://iow.pengpengdd.cyou

[T17] Swift：变量与常量
来源：http://qel.bjfxy.top

var a = 1;  let b = 2
来源：http://sjp.kuanghao11.cn

[T18] Swift：字符串插值
来源：http://tlk.hesvh.cn

"值: \(b)"
来源：http://cxi.ctjpmb.com

[T19] Swift：可选绑定
来源：http://brl.yj20258.top

if let n = opt { print(n) }
来源：http://wjo.vqdsnc.cn

[T20] Swift：数组操作
来源：http://hiw.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://ldf.hcnkem.com

[T21] Swift：遍历
来源：http://kdj.jqgfzy.top

for x in a { print(x) }
来源：http://sce.hysaishi.cn

[T22] Swift：字典
来源：http://gbi.sxryk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ryj.guowangkeji.top

[T23] Swift：函数
来源：http://xhy.quarkkingdee.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vpf.pycfn.com

[T24] Swift：闭包
来源：http://oyr.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://llb.nanxuanxn.top

[T25] Swift：结构体
来源：http://ood.0kj1m.cn

struct P { var x: Int }
来源：http://hla.vqdsnc.cn

[T26] Swift：类与重写
来源：http://msk.zdbjq.cn

class A: Base { override func f() {} }
来源：http://orb.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://zri.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://xeh.hysaishi.cn

[T28] Swift：枚举
来源：http://rss.fehbvm.com

enum Color { case red, green }
来源：http://uac.zdqjudy.top


<!-- 参考信息 -->