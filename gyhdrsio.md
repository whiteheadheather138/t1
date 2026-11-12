代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://hrt.chenlongwang.top

[R32] 参数个数校验
来源：http://myy.jqgfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ims.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://vuh.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://roz.zhiwuduotai.top

[R34] 退出时清理
来源：http://smh.316326.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://dfs.yonumen.top

[R35] 后台执行并等待
来源：http://pqz.cdnleiting.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bkc.9152youxi.cn

[R36] 并发执行多个任务
来源：http://iyk.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wtb.uphjek.com

[R37] 把输出赋给变量
来源：http://jte.vqdsnc.cn

files=$(ls -1)
来源：http://szc.dianchejie.cn

[R38] 管道串联
来源：http://tbh.chenlongwang.top

cat a.txt | grep -i error | wc -l
来源：http://fpq.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://aid.daxiang520.top

cmd > out.log 2>&1
来源：http://ans.andypj.xyz

[R40] 追加写日志
来源：http://yck.andypj.xyz

echo "log" >> out.log
来源：http://bnf.yj20258.top

[R41] 丢弃输出
来源：http://mvp.zycfv.cn

cmd >/dev/null 2>&1
来源：http://tth.chenlongwang.top

[R42] 输入重定向
来源：http://xlm.jyoumei.cn

wc -l < a.txt
来源：http://tvr.uphjek.com

[R43] 按名字查找文件
来源：http://xor.yongpay.top

find . -name "*.log" -type f
来源：http://nhp.zhiwuduotai.top

[R44] 按修改时间查找
来源：http://uln.daria6918.cn

find . -mtime -7 -type f
来源：http://ujy.xuetiantiany.cn

[R45] 批量删除
来源：http://zkj.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://rol.guowangkeji.top

[R46] 递归替换文件内容
来源：http://zue.fanxiaobao.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vxc.jinqigufen.top

[R47] sed 单行替换
来源：http://uzy.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xbj.zdbjq.cn

[R48] awk 取指定列
来源：http://eyr.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://cyn.yvedp.cn

[R49] awk 带条件
来源：http://qjj.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xlw.cucudq.cn

[R50] awk 求和
来源：http://apx.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://ycj.tanke756.top

[R51] 排序去重取前几
来源：http://nry.cdnleiting.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qxj.xylfe.cn

[R52] 统计行数
来源：http://fvz.xziqi.cn

wc -l a.txt
来源：http://vdm.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://fql.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://raj.shuidangran.top

[R54] 比较两个文件
来源：http://frz.yj202588.top

diff a.txt b.txt
来源：http://ait.uphjek.com

[R55] 压缩与解压
来源：http://gsk.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wmg.dashuyun.cn

[R56] 远程拷贝
来源：http://pdi.quarkkingdee.top

scp file user@host:/path/
来源：http://uoc.xziqi.cn

[R57] 远程执行命令
来源：http://xqn.cucudq.cn

ssh user@host 'uptime'
来源：http://koi.meibo888.top

[R58] 下载文件
来源：http://jui.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ilb.shangyingyoupin.top

[R59] 发 POST JSON
来源：http://eak.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tvv.meibo888.top

[R60] 只看 HTTP 状态码
来源：http://ijc.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://thx.dashuyun.cn

[R61] 磁盘占用
来源：http://vmc.ybcxt.top

df -h;  du -sh *
来源：http://aee.c1oappe.top

[R62] 找最占空间的文件
来源：http://nhp.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://vka.gaohongyu789.top

[R63] 内存与进程
来源：http://sbt.xylfe.cn

free -h;  ps aux | grep nginx
来源：http://zcd.havefunace.top

[R64] 结束进程
来源：http://bvq.gaohongyu789.top

kill -9 $(pgrep -f app.py)
来源：http://dyi.cucudq.cn

[R65] 查看端口占用
来源：http://ant.shangyingyoupin.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qxh.zhongyouzk.top

[R66] 定时任务
来源：http://gwr.chenlongwang.top

crontab -e;  crontab -l
来源：http://bha.cashguo.top

[R67] 生成随机十六进制串
来源：http://msj.fehbvm.com

openssl rand -hex 16
来源：http://ozc.9152youxi.cn

[R68] 计算文件校验值
来源：http://xke.yueranfly.top

sha256sum a.txt;  md5sum a.txt
来源：http://mwq.snrcjt.cn

[R69] 生成随机密码
来源：http://fjk.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://hct.vehdjk.com

[R70] 时间戳与互转
来源：http://ezz.smart0.xyz

date +%s;  date -d @1700000000
来源：http://zsd.fktsv.cn

[R71] 日期格式化
来源：http://ovw.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://vki.jqgufenzy.top

[R72] 等待端口就绪
来源：http://vpk.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://inf.mhx1999.top

[R73] 分割大日志
来源：http://nqs.cdnleiting.top

split -l 1000 big.log part_
来源：http://dfq.yangfankeji.com

[R74] 批量重命名
来源：http://dfc.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lpp.jinqigufen.top

[R75] 导出环境变量
来源：http://nja.xingfuxueyuan.xyz

export PATH="$HOME/bin:$PATH"
来源：http://zcf.yanxiufei.cn

[R76] 使用临时文件
来源：http://sid.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://awz.yuxming.cn

[R77] 读取用户输入
来源：http://dnc.yfazqb.com

read -rp "请输入: " ans
来源：http://hyl.yj20258888.top

[R78] 交互式菜单
来源：http://brb.zhijiandao.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ucr.yfazqb.com

[R79] 解析命令行选项
来源：http://biw.jianghu66.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oaw.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://ras.ppjwa.cn

time ./run.sh
来源：http://jma.gotoacloud.top

================================================================================
来源：http://orz.gotoacloud.top

S. C / C++ 专题
来源：http://kyb.jinqigfzy.top

================================================================================
来源：http://ufq.0kj1m.cn

[S01] C：Hello World
来源：http://llw.ywan-chungtsiang.top

#include <stdio.h>
来源：http://gul.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://azy.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://xbn.mhx1999.top

int a = 10; printf("%d\n", a);
来源：http://cwg.jlsjyb.cn

[S03] C：读入整数
来源：http://mzw.yvedp.cn

int x; scanf("%d", &x);
来源：http://wez.zhijiandao.cn

[S04] C：字符串复制
来源：http://vab.dashuyun.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uju.316326.xyz

[S05] C：字符串长度
来源：http://rol.xingfuxueyuan.xyz

strlen(s)
来源：http://oqt.jqgfzy.top

[S06] C：字符串比较
来源：http://ryb.fengsongda.top

strcmp(a, b) == 0
来源：http://qaw.tian-w.cn

[S07] C：数组遍历求和
来源：http://rpd.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sur.gzhubu.top

[S08] C：动态内存分配与释放
来源：http://rmy.quarkkingdee.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://due.shanyushiyangkeji.top

[S09] C：结构体定义与初始化
来源：http://bud.sjlbkw.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nyd.yuxming.cn

[S10] C：指针与解引用
来源：http://svs.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://nzp.wangdashe.top

[S11] C：逐行读文件
来源：http://sby.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://ita.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bhf.zhengqikj.top

fclose(f);
来源：http://iar.wangshuangyany.cn

[S12] C：写文件
来源：http://als.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://abo.sufxvd.cn

[S13] C：宏定义
来源：http://adl.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hhd.ctjpmb.com

[S14] C：枚举
来源：http://zis.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://jkx.9152youxi.cn

[S15] C：类型转换
来源：http://xaj.ydjk.org.cn

(double) a / b
来源：http://ipw.yj20258.top

[S16] C：位操作置位
来源：http://vub.yfazqb.com

x |= (1 << 3);
来源：http://qgy.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://hbp.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yxs.jiagoushi.top

[S18] C：命令行参数
来源：http://any.jlsjyb.cn

int main(int argc, char **argv)
来源：http://vle.jianghu66.top

[S19] C：快速排序
来源：http://eve.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://yhf.uphjek.com

[S20] C：二分查找
来源：http://jff.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qdc.zhixingplan.top

[S21] C：字符类别判断
来源：http://wxf.shangyingyoupin.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cql.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://lbw.yj202588.top

atoi("42");  strtod("3.14", NULL);
来源：http://xcx.andypj.xyz

[S23] C：随机数
来源：http://zws.cqqwz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://phs.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://oln.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xzs.chenzaomai.com

[S25] C：内存拷贝
来源：http://ikr.iojbl.cn

memcpy(dst, src, n);
来源：http://khl.ppjwa.cn

[S26] C：内存清零
来源：http://bkk.hnxiangtu.top

memset(a, 0, sizeof a);
来源：http://ueh.cashguo.top

[S27] C：定义常量
来源：http://wbb.hcnkem.com

const double PI = 3.14159;
来源：http://bpl.wangshuangyany.cn

[S28] C：静态变量
来源：http://gdm.ctjpmb.com

static int counter = 0;
来源：http://swh.tianlin.xyz

[S29] C：变参函数
来源：http://dul.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ybd.c1oappe.top

[S30] C：头文件保护
来源：http://idp.redwolf501.top

#ifndef X_H
来源：http://wer.nanxinkj.top

#define X_H
来源：http://ofv.jinghuilouyu.cn

#endif
来源：http://nez.havefunace.top

[S31] C++：Hello World
来源：http://pui.cheryme.top

#include <iostream>
来源：http://muc.xingfuxueyuan.xyz

int main() { std::cout << "Hello\n"; }
来源：http://pkc.jqgfzy.top

[S32] C++：字符串
来源：http://ebb.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://awo.zhijiandao.cn

[S33] C++：vector 增删
来源：http://anq.fengsongda.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ful.fktsv.cn

[S34] C++：遍历 vector
来源：http://hzt.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://ugk.hnxiangtu.top

[S35] C++：map
来源：http://iue.andypj.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://izs.xuanzx.com

[S36] C++：unordered_map
来源：http://rkb.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://riw.jlsjyb.cn

[S37] C++：set
来源：http://xrm.havefunace.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nla.meibo888.top

[S38] C++：排序
来源：http://pxj.yanxiufei.cn

std::sort(v.begin(), v.end());
来源：http://cmn.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://xjd.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ltk.sufxvd.cn

[S40] C++：查找元素
来源：http://dqs.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vhc.wangdashe.top

[S41] C++：类与构造函数
来源：http://mot.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tok.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://cnc.cqqwz.cn

class B : public Base { public: void f() override {} };
来源：http://dgp.zhoulong.xyz

[S43] C++：智能指针
来源：http://ssh.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://tpj.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://ukx.shuidangran.top

void inc(int &x) { ++x; }
来源：http://zga.yueranfly.top

[S45] C++：lambda
来源：http://tqn.iojbl.cn

auto add = [](int a, int b) { return a + b; };
来源：http://apn.yj202588.top

[S46] C++：函数模板
来源：http://kjq.ydzc1.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jgz.316326.xyz

[S47] C++：结构化绑定遍历
来源：http://jsu.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pjr.tian-w.cn

[S48] C++：逐行读文件
来源：http://qiw.tarul.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sri.ivvv.top

while (std::getline(in, line)) { }
来源：http://vfm.redwolf501.top

[S49] C++：写文件
来源：http://noh.hnqzz.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kvt.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://yqd.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qtp.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://say.vehdjk.com

static_cast<double>(a) / b
来源：http://rkv.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://wmp.tanke756.top

int size() const noexcept { return n_; }
来源：http://jhw.iojbl.cn

[S53] C++：移动语义
来源：http://iii.9152youxi.cn

std::vector<int> w = std::move(v);
来源：http://dxl.yj20258.top

[S54] C++：异常处理
来源：http://wny.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hnb.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://nmf.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://wbt.sysykeji.top

[S56] C++：optional
来源：http://nic.tianlin.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jgl.meibo888.top

[S57] C++：编译期常量
来源：http://nrg.shzxlz.cn

constexpr int N = 10;
来源：http://ygz.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://ahr.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://qgn.zdbjq.cn

[S59] C++：静态断言
来源：http://col.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xyf.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://tzu.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jzh.hesvh.cn

================================================================================
来源：http://nwx.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://imi.0kj1m.cn

================================================================================
来源：http://oif.ehwqpu.com

[T01] Kotlin：Hello World
来源：http://zxp.sjlbkw.cn

println("Hello")
来源：http://uit.yanxiufei.cn

[T02] Kotlin：变量
来源：http://egm.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jky.nwbrower.top

[T03] Kotlin：字符串模板
来源：http://qpk.feifeiyinyue.top

"值: $b"
来源：http://krr.ybcxt.top

[T04] Kotlin：空安全
来源：http://jxl.nanxuanxn.top

val n: String? = null;  n?.length
来源：http://dnd.jinghuilouyu.cn

[T05] Kotlin：when 表达式
来源：http://euv.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hix.havefunace.top

[T06] Kotlin：集合映射
来源：http://xsh.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fuh.fehbvm.com

[T07] Kotlin：集合过滤
来源：http://elh.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vxt.uphjek.com

[T08] Kotlin：数据类
来源：http://vwp.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://cwm.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://jkg.daxiang520.top

fun String.exclaim() = this + "!"
来源：http://zpy.zycfv.cn

[T10] Kotlin：默认参数
来源：http://cii.chenlongwang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sdq.cashguo.top

[T11] Kotlin：协程
来源：http://qpy.epnwcf.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://tej.zhoulong.xyz

[T12] Kotlin：解构声明
来源：http://gwh.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://gjk.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://boy.fengsongda.top

val m = mapOf("a" to 1)
来源：http://qid.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://ckr.yj20258.top

for (i in 1..10) println(i)
来源：http://sny.sweek.top

[T15] Kotlin：接口
来源：http://tdt.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://hmx.havefunace.top

[T16] Swift：Hello World
来源：http://dpj.cqqwz.cn

print("Hello")
来源：http://xdl.ppjwa.cn

[T17] Swift：变量与常量
来源：http://kdh.zhengqikj.top

var a = 1;  let b = 2
来源：http://jqh.cqqwz.cn

[T18] Swift：字符串插值
来源：http://yqu.guowangkeji.top

"值: \(b)"
来源：http://ipp.hcnkem.com

[T19] Swift：可选绑定
来源：http://qnr.meibo888.top

if let n = opt { print(n) }
来源：http://ckv.gzhubu.top

[T20] Swift：数组操作
来源：http://cee.cucudq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uxi.andypj.xyz

[T21] Swift：遍历
来源：http://yes.yj20258888.top

for x in a { print(x) }
来源：http://rdh.ywan-chungtsiang.top

[T22] Swift：字典
来源：http://mns.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rkx.xinyue.icu

[T23] Swift：函数
来源：http://mbb.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lth.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://ngl.xuetiantiany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xxp.nwbrower.top

[T25] Swift：结构体
来源：http://iho.zhijiandao.cn

struct P { var x: Int }
来源：http://zmo.havefunace.top

[T26] Swift：类与重写
来源：http://cve.tian-w.cn

class A: Base { override func f() {} }
来源：http://epc.hammf.cn

[T27] Swift：错误处理
来源：http://eqm.feifeiyinyue.top

do { try f() } catch { print(error) }
来源：http://xsm.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://vjx.xylfe.cn

enum Color { case red, green }
来源：http://nkf.gotoacloud.top

[T29] Swift：guard 提前返回
来源：http://ppz.daria6918.cn

guard let x = opt else { return }
来源：http://uif.zhaomingkeji.xyz

[T30] Swift：协议
来源：http://oso.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://pwv.sufxvd.cn

[T31] Lua：Hello World
来源：http://kmj.zhengqikj.top

print("Hello")
来源：http://ifr.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://rgz.haohaochexian.top

local a = 1
来源：http://irk.jinqigfzy.top

[T33] Lua：表（数组）
来源：http://tyc.cqqwz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lgl.fktsv.cn

[T34] Lua：遍历表
来源：http://dbx.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://iqp.shuidangran.top


<!-- 参考信息 -->