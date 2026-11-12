代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://liz.kuanghao11.cn

[R26] 命令替换
来源：http://xhu.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://irw.dashuyun.cn

[R27] 算术展开
来源：http://oqz.tianlin.xyz

echo $((1 + 2 * 3))
来源：http://wwp.cqqwz.cn

[R28] 浮点运算
来源：http://jcy.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://ruj.vqdsnc.cn

[R29] 定义函数
来源：http://zzf.cashguo.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rdc.yangfankeji.com

[R30] 函数返回状态码
来源：http://xud.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://umz.tanke756.top

[R31] 局部变量
来源：http://mod.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://sox.redwolf501.top

[R32] 参数个数校验
来源：http://rwm.epnwcf.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xkw.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://dwt.jinqigfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cvq.yfazqb.com

[R34] 退出时清理
来源：http://sgo.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://xtb.cheryme.top

[R35] 后台执行并等待
来源：http://biw.sxryk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xtc.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://uoc.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wuu.0kj1m.cn

[R37] 把输出赋给变量
来源：http://ngb.jinqigufen.top

files=$(ls -1)
来源：http://hlb.uphjek.com

[R38] 管道串联
来源：http://mad.jyoumei.cn

cat a.txt | grep -i error | wc -l
来源：http://qne.pycfn.com

[R39] 重定向标准输出与错误
来源：http://cmn.quarkkingdee.top

cmd > out.log 2>&1
来源：http://bda.zhoulong.xyz

[R40] 追加写日志
来源：http://zdp.zycfv.cn

echo "log" >> out.log
来源：http://qhf.dianchejie.cn

[R41] 丢弃输出
来源：http://vsx.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://lbc.havefunace.top

[R42] 输入重定向
来源：http://apo.jianghu66.top

wc -l < a.txt
来源：http://yxe.cashguo.top

[R43] 按名字查找文件
来源：http://mhf.iojbl.cn

find . -name "*.log" -type f
来源：http://fqj.hysaishi.cn

[R44] 按修改时间查找
来源：http://uce.gaohongyu789.top

find . -mtime -7 -type f
来源：http://vox.hcnkem.com

[R45] 批量删除
来源：http://ioz.shzxlz.cn

find . -name "*.tmp" -delete
来源：http://sru.sufxvd.cn

[R46] 递归替换文件内容
来源：http://nng.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://asx.vqdsnc.cn

[R47] sed 单行替换
来源：http://ecp.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://jrd.snrcjt.cn

[R48] awk 取指定列
来源：http://spg.ppjwa.cn

awk '{print $1, $3}' a.txt
来源：http://erq.fzhhl.top

[R49] awk 带条件
来源：http://eju.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ldg.ydjk.org.cn

[R50] awk 求和
来源：http://fmt.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qrx.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://pin.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://igv.52xcode.cn

[R52] 统计行数
来源：http://nvp.chenzaomai.com

wc -l a.txt
来源：http://ltp.gaohongyu789.top

[R53] 查看文件头与实时尾
来源：http://twu.fktsv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://shr.fktsv.cn

[R54] 比较两个文件
来源：http://sdf.fzhhl.top

diff a.txt b.txt
来源：http://zdc.yuxming.cn

[R55] 压缩与解压
来源：http://rww.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qxe.9152youxi.cn

[R56] 远程拷贝
来源：http://lml.mhx1999.top

scp file user@host:/path/
来源：http://osr.jlsjyb.cn

[R57] 远程执行命令
来源：http://cnl.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://tjz.nwbrower.top

[R58] 下载文件
来源：http://prv.zdqjudy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uzt.xylfe.cn

[R59] 发 POST JSON
来源：http://pwf.meibo888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://skf.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://fyb.c1oappe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hva.xinyue.icu

[R61] 磁盘占用
来源：http://ern.ydzc1.top

df -h;  du -sh *
来源：http://dje.tianlin.xyz

[R62] 找最占空间的文件
来源：http://ttz.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://lvy.ehwqpu.com

[R63] 内存与进程
来源：http://cvu.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://qhz.hammf.cn

[R64] 结束进程
来源：http://oum.gaohongyu789.top

kill -9 $(pgrep -f app.py)
来源：http://ijq.jyoumei.cn

[R65] 查看端口占用
来源：http://edj.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ohp.quarkkingdee.top

[R66] 定时任务
来源：http://jze.fzhhl.top

crontab -e;  crontab -l
来源：http://kee.gzhubu.top

[R67] 生成随机十六进制串
来源：http://len.redwolf501.top

openssl rand -hex 16
来源：http://lay.hnqzz.top

[R68] 计算文件校验值
来源：http://agv.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://djn.snrcjt.cn

[R69] 生成随机密码
来源：http://ugz.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://jmp.dashuyun.cn

[R70] 时间戳与互转
来源：http://dgk.shangyingyoupin.top

date +%s;  date -d @1700000000
来源：http://gum.sjlbkw.cn

[R71] 日期格式化
来源：http://ucn.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://chh.vqdsnc.cn

[R72] 等待端口就绪
来源：http://snc.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://joy.epnwcf.com

[R73] 分割大日志
来源：http://iri.uphjek.com

split -l 1000 big.log part_
来源：http://tzx.xinyue.icu

[R74] 批量重命名
来源：http://fcj.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mbx.hammf.cn

[R75] 导出环境变量
来源：http://bjs.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://efo.c1oappe.top

[R76] 使用临时文件
来源：http://yvz.cashguo.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lxv.hfpthk.cn

[R77] 读取用户输入
来源：http://wna.hcnkem.com

read -rp "请输入: " ans
来源：http://uud.ydzc1.top

[R78] 交互式菜单
来源：http://lfk.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://elt.fehbvm.com

[R79] 解析命令行选项
来源：http://bqb.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qbr.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://mib.hcnkem.com

time ./run.sh
来源：http://zaj.mhx1999.top

================================================================================
来源：http://rte.hysaishi.cn

S. C / C++ 专题
来源：http://auh.fzhhl.top

================================================================================
来源：http://ioj.nanxinkj.top

[S01] C：Hello World
来源：http://sbr.fzhhl.top

#include <stdio.h>
来源：http://jen.jqgufenzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ogo.shangyingyoupin.top

[S02] C：变量与格式化输出
来源：http://nhq.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://niq.hnxiangtu.top

[S03] C：读入整数
来源：http://jhw.guannengcc.top

int x; scanf("%d", &x);
来源：http://bsb.zhiwuduotai.top

[S04] C：字符串复制
来源：http://reb.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://hat.dashuyun.cn

[S05] C：字符串长度
来源：http://ovb.meibo888.top

strlen(s)
来源：http://tbq.zdqjudy.top

[S06] C：字符串比较
来源：http://kdq.fzhhl.top

strcmp(a, b) == 0
来源：http://fhn.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://zle.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kra.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://ggk.xylfe.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fnx.shanyushiyangkeji.top

[S09] C：结构体定义与初始化
来源：http://cpf.jqgufenzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zdi.yangfankeji.com

[S10] C：指针与解引用
来源：http://aqh.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://lwk.zycfv.cn

[S11] C：逐行读文件
来源：http://abe.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://ztn.bjfxy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tix.haohaochexian.top

fclose(f);
来源：http://bno.yuanzhike.top

[S12] C：写文件
来源：http://bfd.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mey.bjfxy.top

[S13] C：宏定义
来源：http://ijk.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zbp.zhaomingkeji.xyz

[S14] C：枚举
来源：http://snt.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://qju.jqgfzy.top

[S15] C：类型转换
来源：http://vsu.redwolf501.top

(double) a / b
来源：http://zoh.yueranfly.top

[S16] C：位操作置位
来源：http://gjd.yvedp.cn

x |= (1 << 3);
来源：http://sfz.yongpay.top

[S17] C：安全拼接字符串
来源：http://upm.xziqi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zzi.yueranfly.top

[S18] C：命令行参数
来源：http://wir.smart0.xyz

int main(int argc, char **argv)
来源：http://erz.fehbvm.com

[S19] C：快速排序
来源：http://ubi.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://mdq.epnwcf.com

[S20] C：二分查找
来源：http://qhg.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zbl.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://gct.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://epq.zhoulong.xyz

[S22] C：字符串转数字
来源：http://thi.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://feq.yuanzhike.top

[S23] C：随机数
来源：http://ufh.jinqigfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://him.meibo888.top

[S24] C：获取本地时间
来源：http://epm.svipenyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kbd.yanxiufei.cn

[S25] C：内存拷贝
来源：http://mrw.jianghu66.top

memcpy(dst, src, n);
来源：http://vok.hnqzz.top

[S26] C：内存清零
来源：http://caw.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://tgz.yj20258888.top

[S27] C：定义常量
来源：http://qjt.c1oappe.top

const double PI = 3.14159;
来源：http://qqg.chenlongwang.top

[S28] C：静态变量
来源：http://yoe.gaohongyu789.top

static int counter = 0;
来源：http://fao.jqgfzy.top

[S29] C：变参函数
来源：http://grw.zhoulong.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bvb.xinyue.icu

[S30] C：头文件保护
来源：http://waj.hcnkem.com

#ifndef X_H
来源：http://dmo.c1oappe.top

#define X_H
来源：http://zbe.316326.xyz

#endif
来源：http://lfm.gogol.net.cn

[S31] C++：Hello World
来源：http://jbn.wangdashe.top

#include <iostream>
来源：http://ajf.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://qea.zycfv.cn

[S32] C++：字符串
来源：http://bpb.xuanzx.com

std::string s = "hi";  s += "!";
来源：http://awn.sweek.top

[S33] C++：vector 增删
来源：http://tpi.zhixingplan.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lwq.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://dhv.guowangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://wro.tarul.cn

[S35] C++：map
来源：http://axu.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://duc.ctjpmb.com

[S36] C++：unordered_map
来源：http://eup.ctjpmb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ucs.gotoacloud.top

[S37] C++：set
来源：http://syo.uphjek.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rur.xuanzx.com

[S38] C++：排序
来源：http://axf.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://foi.yj20258.top

[S39] C++：自定义比较器排序
来源：http://pdn.birdmap.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://irx.yj202588.top

[S40] C++：查找元素
来源：http://jpl.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kwd.bbcook.cn

[S41] C++：类与构造函数
来源：http://bkw.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tbz.c1oappe.top

[S42] C++：继承与虚函数
来源：http://wnm.sufxvd.cn

class B : public Base { public: void f() override {} };
来源：http://vob.tianlin.xyz

[S43] C++：智能指针
来源：http://xos.shzxlz.cn

auto p = std::make_unique<int>(5);
来源：http://ebd.xuanzx.com

[S44] C++：引用传参
来源：http://myi.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://xcf.zdqjudy.top

[S45] C++：lambda
来源：http://izc.fanxiaobao.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://jzq.fzhhl.top

[S46] C++：函数模板
来源：http://lxa.uphjek.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hvh.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://rll.jianghu66.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xcw.ppjwa.cn

[S48] C++：逐行读文件
来源：http://ueb.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://uue.jinyuanbaomall.cn

while (std::getline(in, line)) { }
来源：http://kkd.zhiwuduotai.top

[S49] C++：写文件
来源：http://eco.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yaq.gaohongyu789.top

[S50] C++：格式化数字
来源：http://pan.ydzc1.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xdt.xziqi.cn

[S51] C++：显式类型转换
来源：http://gcw.zhijiandao.cn

static_cast<double>(a) / b
来源：http://jcd.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://ltg.52xcode.cn

int size() const noexcept { return n_; }
来源：http://yau.ivvv.top

[S53] C++：移动语义
来源：http://rtr.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://cpo.jqgufenzy.top

[S54] C++：异常处理
来源：http://dhi.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qlp.ctjpmb.com

[S55] C++：结构化绑定
来源：http://zlu.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://shw.xylfe.cn

[S56] C++：optional
来源：http://mvv.yangfankeji.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zfb.zhixingplan.top

[S57] C++：编译期常量
来源：http://ltt.wangshuangyany.cn

constexpr int N = 10;
来源：http://pgm.vqdsnc.cn

[S58] C++：命名空间
来源：http://ups.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://aci.aibaodan.cn

[S59] C++：静态断言
来源：http://upd.gzhubu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oqz.zdbjq.cn

[S60] C++：遍历并删除元素
来源：http://ank.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://guq.aizwys.cn

================================================================================
来源：http://pwk.jinqigufen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zka.bjfxy.top

================================================================================
来源：http://zqd.yuxming.cn

[T01] Kotlin：Hello World
来源：http://rqt.vehdjk.com

println("Hello")
来源：http://pfu.0kj1m.cn

[T02] Kotlin：变量
来源：http://ono.fehbvm.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://chg.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://vls.gaohongyu789.top

"值: $b"
来源：http://cic.zycfv.cn

[T04] Kotlin：空安全
来源：http://hcx.jinqigufen.top

val n: String? = null;  n?.length
来源：http://voj.yj202588.top

[T05] Kotlin：when 表达式
来源：http://nlv.sufxvd.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qvo.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://ewk.yfazqb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://nyt.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://wbh.gotoacloud.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uft.ctjpmb.com

[T08] Kotlin：数据类
来源：http://ngh.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://xca.jinyuanbaomall.cn

[T09] Kotlin：扩展函数
来源：http://qjh.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://mae.yvedp.cn

[T10] Kotlin：默认参数
来源：http://bva.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://pxi.hcnkem.com

[T11] Kotlin：协程
来源：http://knc.hfpthk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rjy.smart0.xyz

[T12] Kotlin：解构声明
来源：http://coz.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://nwm.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://tpz.nanxuanxn.top

val m = mapOf("a" to 1)
来源：http://ndi.ehwqpu.com

[T14] Kotlin：循环
来源：http://axe.yj202588.top

for (i in 1..10) println(i)
来源：http://yrd.yanxiufei.cn

[T15] Kotlin：接口
来源：http://hmg.hnxiangtu.top

interface Shape { fun area(): Double }
来源：http://dhr.mhx1999.top

[T16] Swift：Hello World
来源：http://bpa.yj202588.top

print("Hello")
来源：http://oau.hesvh.cn

[T17] Swift：变量与常量
来源：http://uio.uphjek.com

var a = 1;  let b = 2
来源：http://bwu.shangyingyoupin.top

[T18] Swift：字符串插值
来源：http://kbh.sysykeji.top

"值: \(b)"
来源：http://bcw.hcnkem.com

[T19] Swift：可选绑定
来源：http://gst.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://wpi.zhongyouzk.top

[T20] Swift：数组操作
来源：http://ubq.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://rhp.jqgufenzy.top

[T21] Swift：遍历
来源：http://lfd.birdmap.top

for x in a { print(x) }
来源：http://jwi.jyoumei.cn

[T22] Swift：字典
来源：http://pnc.zhijiandao.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ddp.zhengqikj.top

[T23] Swift：函数
来源：http://wyw.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rjf.wangdashe.top

[T24] Swift：闭包
来源：http://nhb.kuanghao11.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ybg.shuidangran.top

[T25] Swift：结构体
来源：http://oze.316326.xyz

struct P { var x: Int }
来源：http://ash.zhijiandao.cn

[T26] Swift：类与重写
来源：http://elu.zhijiandao.cn

class A: Base { override func f() {} }
来源：http://lmw.pycfn.com

[T27] Swift：错误处理
来源：http://pvv.jinqigufen.top

do { try f() } catch { print(error) }
来源：http://awn.jyoumei.cn

[T28] Swift：枚举
来源：http://gsp.sufxvd.cn

enum Color { case red, green }
来源：http://lpu.gogol.net.cn


<!-- 参考信息 -->