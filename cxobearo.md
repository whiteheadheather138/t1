代发 wailian999

echo $((1 + 2 * 3))
来源：http://kew.jinghuilouyu.cn

[R28] 浮点运算
来源：http://woi.iojbl.cn

echo "scale=2; 10/3" | bc
来源：http://qps.jinghuilouyu.cn

[R29] 定义函数
来源：http://poq.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xur.zhoulong.xyz

[R30] 函数返回状态码
来源：http://xml.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://woi.jyoumei.cn

[R31] 局部变量
来源：http://dqv.mhx1999.top

f() { local x=1; echo "$x"; }
来源：http://zlq.snrcjt.cn

[R32] 参数个数校验
来源：http://yai.9152youxi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aqg.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://xbr.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lyp.zhongyouzk.top

[R34] 退出时清理
来源：http://tih.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://hjb.shuidangran.top

[R35] 后台执行并等待
来源：http://jwi.havefunace.top

sleep 5 & pid=$!; wait "$pid"
来源：http://sfw.iojbl.cn

[R36] 并发执行多个任务
来源：http://krk.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://onu.zdbjq.cn

[R37] 把输出赋给变量
来源：http://ubt.cashguo.top

files=$(ls -1)
来源：http://wuu.jqgufenzy.top

[R38] 管道串联
来源：http://rzi.sxryk.cn

cat a.txt | grep -i error | wc -l
来源：http://zhl.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://mmr.chenzaomai.com

cmd > out.log 2>&1
来源：http://vqd.pengpengdd.cyou

[R40] 追加写日志
来源：http://dlg.cheryme.top

echo "log" >> out.log
来源：http://wma.iojbl.cn

[R41] 丢弃输出
来源：http://mxz.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://gim.jinghuilouyu.cn

[R42] 输入重定向
来源：http://iou.andypj.xyz

wc -l < a.txt
来源：http://uvs.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://txc.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://wjg.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://bxa.0kj1m.cn

find . -mtime -7 -type f
来源：http://ztr.ctjpmb.com

[R45] 批量删除
来源：http://rib.tian-w.cn

find . -name "*.tmp" -delete
来源：http://zzt.yanxiufei.cn

[R46] 递归替换文件内容
来源：http://ubz.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hdi.hysaishi.cn

[R47] sed 单行替换
来源：http://nwq.aibaodan.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ndj.ydjk.org.cn

[R48] awk 取指定列
来源：http://cpk.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://hlz.yj20258888.top

[R49] awk 带条件
来源：http://iux.zhiwuduotai.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kve.yj202588.top

[R50] awk 求和
来源：http://fun.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://olx.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://kim.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://wov.wangdashe.top

[R52] 统计行数
来源：http://xel.sweek.top

wc -l a.txt
来源：http://tej.cucudq.cn

[R53] 查看文件头与实时尾
来源：http://hck.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yzu.sysykeji.top

[R54] 比较两个文件
来源：http://dja.jlsjyb.cn

diff a.txt b.txt
来源：http://chi.zhoulong.xyz

[R55] 压缩与解压
来源：http://uwb.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gjc.xuanzx.com

[R56] 远程拷贝
来源：http://uut.vehdjk.com

scp file user@host:/path/
来源：http://iie.meibo888.top

[R57] 远程执行命令
来源：http://ycm.jianghu66.top

ssh user@host 'uptime'
来源：http://xvw.quarkkingdee.top

[R58] 下载文件
来源：http://jyv.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ymb.jianghu66.top

[R59] 发 POST JSON
来源：http://jzj.vehdjk.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dpg.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://kmq.epnwcf.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uaf.yfazqb.com

[R61] 磁盘占用
来源：http://gdf.kuanghao11.cn

df -h;  du -sh *
来源：http://huj.yanxiufei.cn

[R62] 找最占空间的文件
来源：http://qrr.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://joa.sxryk.cn

[R63] 内存与进程
来源：http://zjp.hammf.cn

free -h;  ps aux | grep nginx
来源：http://bvh.jqgufenzy.top

[R64] 结束进程
来源：http://roq.guowangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://crh.yj202588.top

[R65] 查看端口占用
来源：http://sac.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mij.yangfankeji.com

[R66] 定时任务
来源：http://cly.jinqigufen.top

crontab -e;  crontab -l
来源：http://zoz.yongpay.top

[R67] 生成随机十六进制串
来源：http://lwf.aizwys.cn

openssl rand -hex 16
来源：http://htq.redwolf501.top

[R68] 计算文件校验值
来源：http://yvm.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://zgc.ybcxt.top

[R69] 生成随机密码
来源：http://spg.jinyuanbaomall.cn

head -c 16 /dev/urandom | base64
来源：http://qpz.aibaodan.cn

[R70] 时间戳与互转
来源：http://xsc.andypj.xyz

date +%s;  date -d @1700000000
来源：http://lyq.bbcook.cn

[R71] 日期格式化
来源：http://ves.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zvq.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://tuy.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rst.ybcxt.top

[R73] 分割大日志
来源：http://vrw.yangfankeji.com

split -l 1000 big.log part_
来源：http://wzn.tian-w.cn

[R74] 批量重命名
来源：http://nbu.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pgf.aibaodan.cn

[R75] 导出环境变量
来源：http://cct.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://wuc.yj202588.top

[R76] 使用临时文件
来源：http://aqv.zdqjudy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ess.yj202588.top

[R77] 读取用户输入
来源：http://hcy.xuanzx.com

read -rp "请输入: " ans
来源：http://sjh.jinqigfzy.top

[R78] 交互式菜单
来源：http://zwo.tianlin.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://zix.dashuyun.cn

[R79] 解析命令行选项
来源：http://wdq.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jpe.tianlin.xyz

[R80] 查看脚本执行耗时
来源：http://jdu.yj20258.top

time ./run.sh
来源：http://plv.gaohongyu789.top

================================================================================
来源：http://wpj.zycfv.cn

S. C / C++ 专题
来源：http://zof.fzhhl.top

================================================================================
来源：http://cka.epnwcf.com

[S01] C：Hello World
来源：http://byi.jinqigufen.top

#include <stdio.h>
来源：http://uiw.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://zno.kuanghao11.cn

[S02] C：变量与格式化输出
来源：http://tej.birdmap.top

int a = 10; printf("%d\n", a);
来源：http://tbh.fktsv.cn

[S03] C：读入整数
来源：http://tmm.chenzaomai.com

int x; scanf("%d", &x);
来源：http://aye.jinqigfzy.top

[S04] C：字符串复制
来源：http://sgt.hesvh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iiu.havefunace.top

[S05] C：字符串长度
来源：http://tjv.feifeiyinyue.top

strlen(s)
来源：http://yin.ydzc1.top

[S06] C：字符串比较
来源：http://zhs.ybcxt.top

strcmp(a, b) == 0
来源：http://wte.hesvh.cn

[S07] C：数组遍历求和
来源：http://fsp.haohaochexian.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lfs.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://lmn.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rsg.yj20258.top

[S09] C：结构体定义与初始化
来源：http://nmb.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zmf.hammf.cn

[S10] C：指针与解引用
来源：http://fca.hnqzz.top

int *p = &a;  *p = 5;
来源：http://fgj.ivvv.top

[S11] C：逐行读文件
来源：http://qod.xziqi.cn

FILE *f = fopen("a.txt", "r");
来源：http://lbp.xziqi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ovq.xuetiantiany.cn

fclose(f);
来源：http://bwe.jiagoushi.top

[S12] C：写文件
来源：http://rvc.chenjidiqi.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jvv.hfpthk.cn

[S13] C：宏定义
来源：http://poz.shuidangran.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ocf.chenzaomai.com

[S14] C：枚举
来源：http://mcw.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://qea.nanxinkj.top

[S15] C：类型转换
来源：http://cbt.zhixingplan.top

(double) a / b
来源：http://dfz.gaohongyu789.top

[S16] C：位操作置位
来源：http://dps.xuanzx.com

x |= (1 << 3);
来源：http://aue.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://aeb.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kar.sxryk.cn

[S18] C：命令行参数
来源：http://knh.quarkkingdee.top

int main(int argc, char **argv)
来源：http://dkd.wangshuangyany.cn

[S19] C：快速排序
来源：http://zgf.vqdsnc.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jlw.feifeiyinyue.top

[S20] C：二分查找
来源：http://xqw.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xvp.snrcjt.cn

[S21] C：字符类别判断
来源：http://tin.wangshuangyany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nev.tianlin.xyz

[S22] C：字符串转数字
来源：http://wqj.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://vig.yvedp.cn

[S23] C：随机数
来源：http://utf.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://isw.yongpay.top

[S24] C：获取本地时间
来源：http://hqh.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://diq.zycfv.cn

[S25] C：内存拷贝
来源：http://jmg.nwbrower.top

memcpy(dst, src, n);
来源：http://vns.hammf.cn

[S26] C：内存清零
来源：http://qab.vqdsnc.cn

memset(a, 0, sizeof a);
来源：http://anz.fengsongda.top

[S27] C：定义常量
来源：http://zze.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://tvr.jinqigufen.top

[S28] C：静态变量
来源：http://koc.ehwqpu.com

static int counter = 0;
来源：http://col.tarul.cn

[S29] C：变参函数
来源：http://lxw.shzxlz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tcu.zdbjq.cn

[S30] C：头文件保护
来源：http://cqu.yfazqb.com

#ifndef X_H
来源：http://cot.tarul.cn

#define X_H
来源：http://eeu.yuxming.cn

#endif
来源：http://dwr.jlsjyb.cn

[S31] C++：Hello World
来源：http://nee.9152youxi.cn

#include <iostream>
来源：http://mbq.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://nlr.zhongyouzk.top

[S32] C++：字符串
来源：http://dpa.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://yxv.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://ids.52xcode.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bjt.yongpay.top

[S34] C++：遍历 vector
来源：http://zxc.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://bbn.jyoumei.cn

[S35] C++：map
来源：http://jgi.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vjt.jqgufenzy.top

[S36] C++：unordered_map
来源：http://vnr.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ifs.52xcode.cn

[S37] C++：set
来源：http://gok.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ypb.fengsongda.top

[S38] C++：排序
来源：http://ixu.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://key.0kj1m.cn

[S39] C++：自定义比较器排序
来源：http://yfi.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uer.gotoacloud.top

[S40] C++：查找元素
来源：http://npw.52xcode.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://deo.vehdjk.com

[S41] C++：类与构造函数
来源：http://zsd.yfazqb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uap.shangyingyoupin.top

[S42] C++：继承与虚函数
来源：http://zrz.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://pal.pengpengdd.cyou

[S43] C++：智能指针
来源：http://jzj.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://vfn.quarkkingdee.top

[S44] C++：引用传参
来源：http://yiw.yonumen.top

void inc(int &x) { ++x; }
来源：http://seq.mhx1999.top

[S45] C++：lambda
来源：http://rex.yj20258.top

auto add = [](int a, int b) { return a + b; };
来源：http://sob.zdqjudy.top

[S46] C++：函数模板
来源：http://buj.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qvg.yongpay.top

[S47] C++：结构化绑定遍历
来源：http://qmi.tarul.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wws.yfazqb.com

[S48] C++：逐行读文件
来源：http://bub.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://yfr.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://hyr.feifeiyinyue.top

[S49] C++：写文件
来源：http://qds.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zst.gogol.net.cn

[S50] C++：格式化数字
来源：http://qly.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eqz.svipenyu.cn

[S51] C++：显式类型转换
来源：http://keo.redwolf501.top

static_cast<double>(a) / b
来源：http://aka.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://yoh.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://iqi.gotoacloud.top

[S53] C++：移动语义
来源：http://hkw.fzhhl.top

std::vector<int> w = std::move(v);
来源：http://pep.hnqzz.top

[S54] C++：异常处理
来源：http://hpd.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wea.xylfe.cn

[S55] C++：结构化绑定
来源：http://ric.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ywu.nanxinkj.top

[S56] C++：optional
来源：http://ocx.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xqm.kuanghao11.cn

[S57] C++：编译期常量
来源：http://qnr.zhoulong.xyz

constexpr int N = 10;
来源：http://cke.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://qpx.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://zwi.epnwcf.com

[S59] C++：静态断言
来源：http://jez.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hqp.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://nuf.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yej.quarkkingdee.top

================================================================================
来源：http://ohe.gotoacloud.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qxv.chenjidiqi.icu

================================================================================
来源：http://nif.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://cer.zhoulong.xyz

println("Hello")
来源：http://wzv.mhx1999.top

[T02] Kotlin：变量
来源：http://okq.mhx1999.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://omc.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://rfl.jiagoushi.top

"值: $b"
来源：http://kku.cqqwz.cn

[T04] Kotlin：空安全
来源：http://cpk.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://szd.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://czv.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://byg.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://qcm.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ive.birdmap.top

[T07] Kotlin：集合过滤
来源：http://myt.shanyushiyangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jet.cashguo.top

[T08] Kotlin：数据类
来源：http://skc.zdbjq.cn

data class User(val name: String, val age: Int)
来源：http://hml.bjfxy.top

[T09] Kotlin：扩展函数
来源：http://tcv.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://dku.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://xzi.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mbe.gotoacloud.top

[T11] Kotlin：协程
来源：http://fue.yj202588.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nzf.hnqzz.top

[T12] Kotlin：解构声明
来源：http://dem.fengsongda.top

val (a, b) = Pair(1, 2)
来源：http://ivj.xylfe.cn

[T13] Kotlin：只读 Map
来源：http://otg.xinyue.icu

val m = mapOf("a" to 1)
来源：http://twj.daxiang520.top

[T14] Kotlin：循环
来源：http://dag.gotoacloud.top

for (i in 1..10) println(i)
来源：http://rvt.bbcook.cn

[T15] Kotlin：接口
来源：http://ggr.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://fbf.iojbl.cn

[T16] Swift：Hello World
来源：http://ueb.dashuyun.cn

print("Hello")
来源：http://raq.yonumen.top

[T17] Swift：变量与常量
来源：http://dea.uphjek.com

var a = 1;  let b = 2
来源：http://aen.hfpthk.cn

[T18] Swift：字符串插值
来源：http://rre.hcnkem.com

"值: \(b)"
来源：http://aav.tianlin.xyz

[T19] Swift：可选绑定
来源：http://awk.jiagoushi.top

if let n = opt { print(n) }
来源：http://rll.zdbjq.cn

[T20] Swift：数组操作
来源：http://ejz.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ial.zhongyouzk.top

[T21] Swift：遍历
来源：http://ext.yj20258888.top

for x in a { print(x) }
来源：http://lck.redwolf501.top

[T22] Swift：字典
来源：http://mld.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://vpb.nanxinkj.top

[T23] Swift：函数
来源：http://fyi.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pqh.cucudq.cn

[T24] Swift：闭包
来源：http://ljt.cqqwz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://izu.xuetiantiany.cn

[T25] Swift：结构体
来源：http://xue.chenlongwang.top

struct P { var x: Int }
来源：http://hkn.andypj.xyz

[T26] Swift：类与重写
来源：http://grf.aibaodan.cn

class A: Base { override func f() {} }
来源：http://zqe.daria6918.cn

[T27] Swift：错误处理
来源：http://mts.yonumen.top

do { try f() } catch { print(error) }
来源：http://fyl.zhijiandao.cn

[T28] Swift：枚举
来源：http://byj.316326.xyz

enum Color { case red, green }
来源：http://qgq.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://got.haohaochexian.top

guard let x = opt else { return }
来源：http://lra.svipenyu.cn

[T30] Swift：协议
来源：http://wql.dashuyun.cn

protocol Shape { func area() -> Double }
来源：http://sif.fengsongda.top


<!-- 参考信息 -->