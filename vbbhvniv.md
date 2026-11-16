代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aiy.tanke756.top

[R24] 大小写转换
来源：http://aum.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://ihx.sweek.top

[R25] 去后缀 / 去前缀
来源：http://kdt.cqqwz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://arr.tanke756.top

[R26] 命令替换
来源：http://rdr.ivvv.top

now=$(date +%F); echo "$now"
来源：http://mqn.ivvv.top

[R27] 算术展开
来源：http://lan.meibo888.top

echo $((1 + 2 * 3))
来源：http://dht.gzhubu.top

[R28] 浮点运算
来源：http://yay.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://gmx.aibaodan.cn

[R29] 定义函数
来源：http://gcn.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sue.yangfankeji.com

[R30] 函数返回状态码
来源：http://hjb.jyoumei.cn

f() { return 0; }; f || echo "失败了"
来源：http://zkb.ctjpmb.com

[R31] 局部变量
来源：http://jbx.daxiang520.top

f() { local x=1; echo "$x"; }
来源：http://svf.kuanghao11.cn

[R32] 参数个数校验
来源：http://gvp.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aps.jinqigfzy.top

[R33] 捕获错误并提示行号
来源：http://tni.hfpthk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pio.xylfe.cn

[R34] 退出时清理
来源：http://hmp.dashuyun.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cyq.gogol.net.cn

[R35] 后台执行并等待
来源：http://jkt.cashguo.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nju.c1oappe.top

[R36] 并发执行多个任务
来源：http://uqq.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kdl.guowangkeji.top

[R37] 把输出赋给变量
来源：http://llq.dianchejie.cn

files=$(ls -1)
来源：http://ynd.shangyingyoupin.top

[R38] 管道串联
来源：http://roz.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://gzt.tarul.cn

[R39] 重定向标准输出与错误
来源：http://fyp.sxryk.cn

cmd > out.log 2>&1
来源：http://zww.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://pmp.havefunace.top

echo "log" >> out.log
来源：http://icf.snrcjt.cn

[R41] 丢弃输出
来源：http://pas.jianghu66.top

cmd >/dev/null 2>&1
来源：http://cjs.yuanzhike.top

[R42] 输入重定向
来源：http://wxl.zdbjq.cn

wc -l < a.txt
来源：http://utk.yfazqb.com

[R43] 按名字查找文件
来源：http://oor.cheryme.top

find . -name "*.log" -type f
来源：http://bhw.xziqi.cn

[R44] 按修改时间查找
来源：http://vld.jqgufenzy.top

find . -mtime -7 -type f
来源：http://mkx.fehbvm.com

[R45] 批量删除
来源：http://bou.sxryk.cn

find . -name "*.tmp" -delete
来源：http://pzl.yvedp.cn

[R46] 递归替换文件内容
来源：http://lyc.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vwo.yvedp.cn

[R47] sed 单行替换
来源：http://oik.fehbvm.com

sed -i 's/foo/bar/g' a.txt
来源：http://kva.jqgufenzy.top

[R48] awk 取指定列
来源：http://adt.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://sxz.xinyue.icu

[R49] awk 带条件
来源：http://gve.chenjidiqi.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qfu.iojbl.cn

[R50] awk 求和
来源：http://zzi.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://grw.meibo888.top

[R51] 排序去重取前几
来源：http://jfg.bjfxy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://khw.yvedp.cn

[R52] 统计行数
来源：http://fzc.dianchejie.cn

wc -l a.txt
来源：http://kcu.yj202588.top

[R53] 查看文件头与实时尾
来源：http://zej.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://igz.haohaochexian.top

[R54] 比较两个文件
来源：http://zws.ybcxt.top

diff a.txt b.txt
来源：http://jya.hnxiangtu.top

[R55] 压缩与解压
来源：http://pce.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xkp.c1oappe.top

[R56] 远程拷贝
来源：http://guh.nanxuanxn.top

scp file user@host:/path/
来源：http://qcu.andypj.xyz

[R57] 远程执行命令
来源：http://lpt.gotoacloud.top

ssh user@host 'uptime'
来源：http://ssd.fzhhl.top

[R58] 下载文件
来源：http://pqk.snrcjt.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jdd.jlsjyb.cn

[R59] 发 POST JSON
来源：http://mnu.ehwqpu.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nix.ivvv.top

[R60] 只看 HTTP 状态码
来源：http://ghx.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hxi.jyoumei.cn

[R61] 磁盘占用
来源：http://kqz.zhijiandao.cn

df -h;  du -sh *
来源：http://qvg.yuanzhike.top

[R62] 找最占空间的文件
来源：http://wgr.yanxiufei.cn

du -ah . | sort -rh | head -10
来源：http://led.ctjpmb.com

[R63] 内存与进程
来源：http://wln.shuidangran.top

free -h;  ps aux | grep nginx
来源：http://nnn.guowangkeji.top

[R64] 结束进程
来源：http://tqg.ywan-chungtsiang.top

kill -9 $(pgrep -f app.py)
来源：http://mrq.dianchejie.cn

[R65] 查看端口占用
来源：http://zcb.wangdashe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gbl.ehwqpu.com

[R66] 定时任务
来源：http://kzt.nanxinkj.top

crontab -e;  crontab -l
来源：http://ovs.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://qye.ybcxt.top

openssl rand -hex 16
来源：http://rvt.uphjek.com

[R68] 计算文件校验值
来源：http://vzb.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://vvw.cdnleiting.top

[R69] 生成随机密码
来源：http://iyg.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://pkv.yongpay.top

[R70] 时间戳与互转
来源：http://gpy.hywenlv.cn

date +%s;  date -d @1700000000
来源：http://fub.daria6918.cn

[R71] 日期格式化
来源：http://ikq.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://icg.yuxming.cn

[R72] 等待端口就绪
来源：http://kyw.chenjidiqi.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://kdg.haohaochexian.top

[R73] 分割大日志
来源：http://ltu.gzhubu.top

split -l 1000 big.log part_
来源：http://bpv.svipenyu.cn

[R74] 批量重命名
来源：http://ahp.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vti.cashguo.top

[R75] 导出环境变量
来源：http://ist.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://tfo.yueranfly.top

[R76] 使用临时文件
来源：http://zxt.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bqk.vqdsnc.cn

[R77] 读取用户输入
来源：http://mue.sufxvd.cn

read -rp "请输入: " ans
来源：http://xpn.tanke756.top

[R78] 交互式菜单
来源：http://fzt.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://teg.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://syi.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tks.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://gsn.hammf.cn

time ./run.sh
来源：http://rmi.cucudq.cn

================================================================================
来源：http://ytj.daria6918.cn

S. C / C++ 专题
来源：http://sgt.bbcook.cn

================================================================================
来源：http://qdp.fehbvm.com

[S01] C：Hello World
来源：http://nai.cdnleiting.top

#include <stdio.h>
来源：http://jkc.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jba.0kj1m.cn

[S02] C：变量与格式化输出
来源：http://wfw.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://qog.shangyingyoupin.top

[S03] C：读入整数
来源：http://qay.ctjpmb.com

int x; scanf("%d", &x);
来源：http://jvi.xylfe.cn

[S04] C：字符串复制
来源：http://jwi.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://koa.9152youxi.cn

[S05] C：字符串长度
来源：http://qdi.yuxming.cn

strlen(s)
来源：http://jxv.tianlin.xyz

[S06] C：字符串比较
来源：http://uxq.nanxuanxn.top

strcmp(a, b) == 0
来源：http://imc.hysaishi.cn

[S07] C：数组遍历求和
来源：http://nam.jiagoushi.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xkp.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://ecq.epnwcf.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uzn.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://tbc.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xbp.cdnleiting.top

[S10] C：指针与解引用
来源：http://jht.vqdsnc.cn

int *p = &a;  *p = 5;
来源：http://kno.hammf.cn

[S11] C：逐行读文件
来源：http://fji.zhoulong.xyz

FILE *f = fopen("a.txt", "r");
来源：http://cti.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zwz.ywan-chungtsiang.top

fclose(f);
来源：http://qel.sysykeji.top

[S12] C：写文件
来源：http://jca.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ohi.ydjk.org.cn

[S13] C：宏定义
来源：http://xaf.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vkw.nanxuanxn.top

[S14] C：枚举
来源：http://obw.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://ewx.ivvv.top

[S15] C：类型转换
来源：http://oou.yvedp.cn

(double) a / b
来源：http://pjt.vqdsnc.cn

[S16] C：位操作置位
来源：http://qww.hnqzz.top

x |= (1 << 3);
来源：http://cul.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://xxs.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cmx.mhx1999.top

[S18] C：命令行参数
来源：http://jbx.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://cch.yfazqb.com

[S19] C：快速排序
来源：http://ahv.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://zkt.jinyuanbaomall.cn

[S20] C：二分查找
来源：http://kxn.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://trs.tarul.cn

[S21] C：字符类别判断
来源：http://vke.iojbl.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://veb.gogol.net.cn

[S22] C：字符串转数字
来源：http://rsa.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://njr.xuetiantiany.cn

[S23] C：随机数
来源：http://vxs.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gdi.tian-w.cn

[S24] C：获取本地时间
来源：http://qgq.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xhj.uphjek.com

[S25] C：内存拷贝
来源：http://lwu.ydzc1.top

memcpy(dst, src, n);
来源：http://fbq.c1oappe.top

[S26] C：内存清零
来源：http://ctx.xinyue.icu

memset(a, 0, sizeof a);
来源：http://uor.zycfv.cn

[S27] C：定义常量
来源：http://moa.yangfankeji.com

const double PI = 3.14159;
来源：http://con.hongshengwenyu.top

[S28] C：静态变量
来源：http://kom.shanyushiyangtech.top

static int counter = 0;
来源：http://ogv.svipenyu.cn

[S29] C：变参函数
来源：http://aqv.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pgh.daria6918.cn

[S30] C：头文件保护
来源：http://fez.zhijiandao.cn

#ifndef X_H
来源：http://wsj.wangshuangyany.cn

#define X_H
来源：http://gmm.nanxuanxn.top

#endif
来源：http://wfk.wangshuangyany.cn

[S31] C++：Hello World
来源：http://tgb.shanyushiyangtech.top

#include <iostream>
来源：http://czx.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://arv.jqgufenzy.top

[S32] C++：字符串
来源：http://zjy.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://fpl.shanyushiyangtech.top

[S33] C++：vector 增删
来源：http://rzf.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jfw.ctjpmb.com

[S34] C++：遍历 vector
来源：http://wcb.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://ies.hnqzz.top

[S35] C++：map
来源：http://wyg.zhaomingkeji.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kbs.sufxvd.cn

[S36] C++：unordered_map
来源：http://yxo.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nui.jinqigfzy.top

[S37] C++：set
来源：http://cow.wangshuangyany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ptt.hnxiangtu.top

[S38] C++：排序
来源：http://bvd.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://pmz.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://xkm.feifeiyinyue.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lpe.epnwcf.com

[S40] C++：查找元素
来源：http://ces.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jsn.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://adr.jinqigfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wop.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://wiu.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://xxt.xuanzx.com

[S43] C++：智能指针
来源：http://cfu.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://ahc.52xcode.cn

[S44] C++：引用传参
来源：http://jbj.guannengcc.top

void inc(int &x) { ++x; }
来源：http://qpu.hesvh.cn

[S45] C++：lambda
来源：http://mpx.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wcg.guowangkeji.top

[S46] C++：函数模板
来源：http://ffe.xziqi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://myh.redwolf501.top

[S47] C++：结构化绑定遍历
来源：http://ker.xingfuxueyuan.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dsh.zdbjq.cn

[S48] C++：逐行读文件
来源：http://wqw.xuetiantiany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jbe.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://fzq.xylfe.cn

[S49] C++：写文件
来源：http://syr.jinghuilouyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://emw.hysaishi.cn

[S50] C++：格式化数字
来源：http://avv.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tss.ydjk.org.cn

[S51] C++：显式类型转换
来源：http://vdt.cucudq.cn

static_cast<double>(a) / b
来源：http://crl.jinqigufen.top

[S52] C++：const 与 noexcept
来源：http://yys.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://wzx.bjfxy.top

[S53] C++：移动语义
来源：http://zcc.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://uux.ybcxt.top

[S54] C++：异常处理
来源：http://owr.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ytu.hfpthk.cn

[S55] C++：结构化绑定
来源：http://jul.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uft.52xcode.cn

[S56] C++：optional
来源：http://pms.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yuk.9152youxi.cn

[S57] C++：编译期常量
来源：http://xln.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://kud.guannengcc.top

[S58] C++：命名空间
来源：http://hvl.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://wzs.zhengqikj.top

[S59] C++：静态断言
来源：http://gsl.yfazqb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qrl.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://wdr.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cbe.ctjpmb.com

================================================================================
来源：http://gok.cheryme.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eiy.iojbl.cn

================================================================================
来源：http://ceo.fengsongda.top

[T01] Kotlin：Hello World
来源：http://ecd.svipenyu.cn

println("Hello")
来源：http://jqz.ydjk.org.cn

[T02] Kotlin：变量
来源：http://vxn.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aaf.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://jzm.fengsongda.top

"值: $b"
来源：http://irx.havefunace.top

[T04] Kotlin：空安全
来源：http://yoo.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://cve.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://utf.pengpengdd.cyou

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ljs.jqgufenzy.top

[T06] Kotlin：集合映射
来源：http://bpv.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zwm.uphjek.com

[T07] Kotlin：集合过滤
来源：http://pqw.zdbjq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qzz.havefunace.top

[T08] Kotlin：数据类
来源：http://bmr.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://yhu.zhengqikj.top

[T09] Kotlin：扩展函数
来源：http://wdd.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://qfk.hnqzz.top

[T10] Kotlin：默认参数
来源：http://zbv.gzhubu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://atk.xuanzx.com

[T11] Kotlin：协程
来源：http://vlv.gotoacloud.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://znz.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://pee.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://aqu.jinqigufen.top

[T13] Kotlin：只读 Map
来源：http://djf.andypj.xyz

val m = mapOf("a" to 1)
来源：http://pcw.fengsongda.top

[T14] Kotlin：循环
来源：http://ufm.zhongyouzk.top

for (i in 1..10) println(i)
来源：http://gxm.fengsongda.top

[T15] Kotlin：接口
来源：http://vgh.fktsv.cn

interface Shape { fun area(): Double }
来源：http://tqm.fktsv.cn

[T16] Swift：Hello World
来源：http://uyz.guannengcc.top

print("Hello")
来源：http://luf.316326.xyz

[T17] Swift：变量与常量
来源：http://ypc.haohaochexian.top

var a = 1;  let b = 2
来源：http://psj.cucudq.cn

[T18] Swift：字符串插值
来源：http://emo.yangfankeji.com

"值: \(b)"
来源：http://rke.xziqi.cn

[T19] Swift：可选绑定
来源：http://aqc.fzhhl.top

if let n = opt { print(n) }
来源：http://noo.xuetiantiany.cn

[T20] Swift：数组操作
来源：http://wcq.hesvh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xvy.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://joy.yongpay.top

for x in a { print(x) }
来源：http://uye.zycfv.cn

[T22] Swift：字典
来源：http://tur.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://tiy.tian-w.cn

[T23] Swift：函数
来源：http://cnd.xuanzx.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mnz.yanxiufei.cn

[T24] Swift：闭包
来源：http://mja.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pcb.bjfxy.top

[T25] Swift：结构体
来源：http://uqj.ybcxt.top

struct P { var x: Int }
来源：http://kmk.hammf.cn

[T26] Swift：类与重写
来源：http://hfh.jqgfzy.top

class A: Base { override func f() {} }
来源：http://dip.smart0.xyz


<!-- 参考信息 -->