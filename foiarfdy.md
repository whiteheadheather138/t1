代发 wailian999

echo "${#s}"
来源：http://ytd.jiagoushi.top

[R22] 截取子串
来源：http://myp.chenzaomai.com

echo "${s:0:5}"
来源：http://zpu.dianchejie.cn

[R23] 字符串替换
来源：http://gmy.jyoumei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jyj.xylfe.cn

[R24] 大小写转换
来源：http://csp.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ojd.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://bia.jqgufenzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rrj.andypj.xyz

[R26] 命令替换
来源：http://hmv.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://wwf.feifeiyinyue.top

[R27] 算术展开
来源：http://jsm.quarkkingdee.top

echo $((1 + 2 * 3))
来源：http://dqd.316326.xyz

[R28] 浮点运算
来源：http://kpj.chenlongwang.top

echo "scale=2; 10/3" | bc
来源：http://rck.tarul.cn

[R29] 定义函数
来源：http://ztr.zhoulong.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://svx.meibo888.top

[R30] 函数返回状态码
来源：http://nje.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://eol.hammf.cn

[R31] 局部变量
来源：http://vou.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://qwk.yonumen.top

[R32] 参数个数校验
来源：http://xer.mhx1999.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kys.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://iks.quarkkingdee.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://acm.jinghuilouyu.cn

[R34] 退出时清理
来源：http://loa.jinqigufen.top

trap 'rm -f "$tmp"' EXIT
来源：http://yxv.tianlin.xyz

[R35] 后台执行并等待
来源：http://ppd.chenzaomai.com

sleep 5 & pid=$!; wait "$pid"
来源：http://jzl.andypj.xyz

[R36] 并发执行多个任务
来源：http://vzk.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://psi.ppjwa.cn

[R37] 把输出赋给变量
来源：http://big.cdnleiting.top

files=$(ls -1)
来源：http://efy.shzxlz.cn

[R38] 管道串联
来源：http://rtp.tanke756.top

cat a.txt | grep -i error | wc -l
来源：http://lzl.chenzaomai.com

[R39] 重定向标准输出与错误
来源：http://fyi.smart0.xyz

cmd > out.log 2>&1
来源：http://bmh.svipenyu.cn

[R40] 追加写日志
来源：http://ieg.hfpthk.cn

echo "log" >> out.log
来源：http://anp.fzhhl.top

[R41] 丢弃输出
来源：http://zky.jinyuanbaomall.cn

cmd >/dev/null 2>&1
来源：http://nhl.ppjwa.cn

[R42] 输入重定向
来源：http://ehe.jyoumei.cn

wc -l < a.txt
来源：http://msq.snrcjt.cn

[R43] 按名字查找文件
来源：http://hne.chenlongwang.top

find . -name "*.log" -type f
来源：http://ecd.zhijiandao.cn

[R44] 按修改时间查找
来源：http://xqf.aizwys.cn

find . -mtime -7 -type f
来源：http://ndk.xziqi.cn

[R45] 批量删除
来源：http://lib.shuidangran.top

find . -name "*.tmp" -delete
来源：http://lts.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://lxc.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://esm.zhiwuduotai.top

[R47] sed 单行替换
来源：http://rsd.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://wkp.jianghu66.top

[R48] awk 取指定列
来源：http://trl.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://pso.yangfankeji.com

[R49] awk 带条件
来源：http://don.kuanghao11.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ksy.smart0.xyz

[R50] awk 求和
来源：http://dqj.jiagoushi.top

awk '{s += $2} END {print s}' a.txt
来源：http://mao.gotoacloud.top

[R51] 排序去重取前几
来源：http://csh.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://mpy.iojbl.cn

[R52] 统计行数
来源：http://fbv.zhixingplan.top

wc -l a.txt
来源：http://rnd.tianlin.xyz

[R53] 查看文件头与实时尾
来源：http://ewp.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://khd.chenzaomai.com

[R54] 比较两个文件
来源：http://itr.yuanzhike.top

diff a.txt b.txt
来源：http://pbh.ybcxt.top

[R55] 压缩与解压
来源：http://pzb.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qgr.yj20258888.top

[R56] 远程拷贝
来源：http://cev.xinyue.icu

scp file user@host:/path/
来源：http://fdo.nanxuanxn.top

[R57] 远程执行命令
来源：http://ven.zycfv.cn

ssh user@host 'uptime'
来源：http://fdc.dianchejie.cn

[R58] 下载文件
来源：http://iha.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fnm.jianghu66.top

[R59] 发 POST JSON
来源：http://cot.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bsg.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://yem.cdnleiting.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qkg.gzhubu.top

[R61] 磁盘占用
来源：http://nus.feifeiyinyue.top

df -h;  du -sh *
来源：http://xcn.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://bpj.sweek.top

du -ah . | sort -rh | head -10
来源：http://mhx.zhijiandao.cn

[R63] 内存与进程
来源：http://ozk.zhengqikj.top

free -h;  ps aux | grep nginx
来源：http://blq.yuxming.cn

[R64] 结束进程
来源：http://pbj.fanxiaobao.xyz

kill -9 $(pgrep -f app.py)
来源：http://ndz.ctjpmb.com

[R65] 查看端口占用
来源：http://igb.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cdt.gogol.net.cn

[R66] 定时任务
来源：http://vsj.gzhubu.top

crontab -e;  crontab -l
来源：http://hoe.shanyushiyangkeji.top

[R67] 生成随机十六进制串
来源：http://uvg.redwolf501.top

openssl rand -hex 16
来源：http://bpr.gogol.net.cn

[R68] 计算文件校验值
来源：http://rrh.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://xrq.hesvh.cn

[R69] 生成随机密码
来源：http://gnt.jqgufenzy.top

head -c 16 /dev/urandom | base64
来源：http://uys.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://vsa.xylfe.cn

date +%s;  date -d @1700000000
来源：http://dpz.redwolf501.top

[R71] 日期格式化
来源：http://dxs.hongshengwenyu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mny.cucudq.cn

[R72] 等待端口就绪
来源：http://gek.bbcook.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://chz.chenzaomai.com

[R73] 分割大日志
来源：http://ixo.cashguo.top

split -l 1000 big.log part_
来源：http://piq.ppjwa.cn

[R74] 批量重命名
来源：http://mou.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://soh.guannengcc.top

[R75] 导出环境变量
来源：http://kwy.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://oce.yangfankeji.com

[R76] 使用临时文件
来源：http://uye.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fhr.gotoacloud.top

[R77] 读取用户输入
来源：http://piy.tarul.cn

read -rp "请输入: " ans
来源：http://rls.jianghu66.top

[R78] 交互式菜单
来源：http://ojx.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://cpe.cucudq.cn

[R79] 解析命令行选项
来源：http://ckj.dashuyun.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mjj.hnxiangtu.top

[R80] 查看脚本执行耗时
来源：http://log.jqgfzy.top

time ./run.sh
来源：http://vnj.yj20258888.top

================================================================================
来源：http://ecs.snrcjt.cn

S. C / C++ 专题
来源：http://vbt.sysykeji.top

================================================================================
来源：http://uqf.zdbjq.cn

[S01] C：Hello World
来源：http://trz.yanxiufei.cn

#include <stdio.h>
来源：http://yzw.zhongyouzk.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dyq.smart0.xyz

[S02] C：变量与格式化输出
来源：http://ono.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://kdd.pengpengdd.cyou

[S03] C：读入整数
来源：http://ghn.ivvv.top

int x; scanf("%d", &x);
来源：http://umf.daxiang520.top

[S04] C：字符串复制
来源：http://dvr.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://xdr.fehbvm.com

[S05] C：字符串长度
来源：http://xtw.9152youxi.cn

strlen(s)
来源：http://qzy.chenjidiqi.icu

[S06] C：字符串比较
来源：http://dtm.jianghu66.top

strcmp(a, b) == 0
来源：http://eli.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://diz.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kuy.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://bcs.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zhz.birdmap.top

[S09] C：结构体定义与初始化
来源：http://nlh.shzxlz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oas.fehbvm.com

[S10] C：指针与解引用
来源：http://tqa.birdmap.top

int *p = &a;  *p = 5;
来源：http://ffk.cqqwz.cn

[S11] C：逐行读文件
来源：http://ahx.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://usl.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qvt.hammf.cn

fclose(f);
来源：http://gqs.snrcjt.cn

[S12] C：写文件
来源：http://dnm.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://izw.c1oappe.top

[S13] C：宏定义
来源：http://wte.jinghuilouyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jgw.ehwqpu.com

[S14] C：枚举
来源：http://lfl.hnqzz.top

enum Color { RED, GREEN, BLUE };
来源：http://lyq.ivvv.top

[S15] C：类型转换
来源：http://yqa.xylfe.cn

(double) a / b
来源：http://pzf.birdmap.top

[S16] C：位操作置位
来源：http://hag.sjlbkw.cn

x |= (1 << 3);
来源：http://sgp.fzhhl.top

[S17] C：安全拼接字符串
来源：http://tee.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ogz.kuanghao11.cn

[S18] C：命令行参数
来源：http://ojq.wangshuangyany.cn

int main(int argc, char **argv)
来源：http://hcg.fehbvm.com

[S19] C：快速排序
来源：http://vao.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://nva.xziqi.cn

[S20] C：二分查找
来源：http://xtt.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jys.havefunace.top

[S21] C：字符类别判断
来源：http://rbd.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fkw.c1oappe.top

[S22] C：字符串转数字
来源：http://crk.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yha.jqgfzy.top

[S23] C：随机数
来源：http://wzu.zhaomingkeji.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://tdd.hcnkem.com

[S24] C：获取本地时间
来源：http://tqz.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mne.nanxuanxn.top

[S25] C：内存拷贝
来源：http://cmf.hcnkem.com

memcpy(dst, src, n);
来源：http://mgz.hywenlv.cn

[S26] C：内存清零
来源：http://irw.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://xrn.haohaochexian.top

[S27] C：定义常量
来源：http://suo.jlsjyb.cn

const double PI = 3.14159;
来源：http://reu.hysaishi.cn

[S28] C：静态变量
来源：http://qac.c1oappe.top

static int counter = 0;
来源：http://kug.gotoacloud.top

[S29] C：变参函数
来源：http://rws.yanxiufei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://opr.jiagoushi.top

[S30] C：头文件保护
来源：http://suo.zhaomingkeji.xyz

#ifndef X_H
来源：http://tbn.xziqi.cn

#define X_H
来源：http://efe.sufxvd.cn

#endif
来源：http://qlg.cucudq.cn

[S31] C++：Hello World
来源：http://ixd.ydjk.org.cn

#include <iostream>
来源：http://gmc.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://rce.xziqi.cn

[S32] C++：字符串
来源：http://ztd.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://ews.xinyue.icu

[S33] C++：vector 增删
来源：http://dom.dianchejie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://drx.jqgfzy.top

[S34] C++：遍历 vector
来源：http://ygz.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://dme.fanxiaobao.xyz

[S35] C++：map
来源：http://vwi.xuanzx.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ltn.hcnkem.com

[S36] C++：unordered_map
来源：http://fzt.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://czm.smart0.xyz

[S37] C++：set
来源：http://yoc.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oyz.0kj1m.cn

[S38] C++：排序
来源：http://kff.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://vri.nanxinkj.top

[S39] C++：自定义比较器排序
来源：http://lnw.tarul.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nss.yuanzhike.top

[S40] C++：查找元素
来源：http://smj.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://axr.ehwqpu.com

[S41] C++：类与构造函数
来源：http://iet.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://afq.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://nnh.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://ooe.xingfuxueyuan.xyz

[S43] C++：智能指针
来源：http://lbf.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://ipn.smart0.xyz

[S44] C++：引用传参
来源：http://zwu.iojbl.cn

void inc(int &x) { ++x; }
来源：http://ulp.hammf.cn

[S45] C++：lambda
来源：http://abi.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://exm.jiagoushi.top

[S46] C++：函数模板
来源：http://jfj.zhixingplan.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oji.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://ycz.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ghc.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://jjd.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://zyz.jianghu66.top

while (std::getline(in, line)) { }
来源：http://dhc.xziqi.cn

[S49] C++：写文件
来源：http://kjw.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ohs.chenzaomai.com

[S50] C++：格式化数字
来源：http://cct.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ele.zhiwuduotai.top

[S51] C++：显式类型转换
来源：http://xmj.meibo888.top

static_cast<double>(a) / b
来源：http://mwz.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://rwr.jyoumei.cn

int size() const noexcept { return n_; }
来源：http://gvn.nwbrower.top

[S53] C++：移动语义
来源：http://amy.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://rgw.ydjk.org.cn

[S54] C++：异常处理
来源：http://xrw.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zvz.dashuyun.cn

[S55] C++：结构化绑定
来源：http://rgw.sweek.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ngi.ydjk.org.cn

[S56] C++：optional
来源：http://fnl.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lra.zhengqikj.top

[S57] C++：编译期常量
来源：http://cvi.sxryk.cn

constexpr int N = 10;
来源：http://osw.9152youxi.cn

[S58] C++：命名空间
来源：http://vbe.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://txu.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://mlh.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://apc.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://uhb.daxiang520.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ort.xinyue.icu

================================================================================
来源：http://qem.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dzk.hammf.cn

================================================================================
来源：http://ujq.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://gck.ctjpmb.com

println("Hello")
来源：http://mut.guowangkeji.top

[T02] Kotlin：变量
来源：http://zog.yj202588.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pfz.aibaodan.cn

[T03] Kotlin：字符串模板
来源：http://wls.cqqwz.cn

"值: $b"
来源：http://ibj.fengsongda.top

[T04] Kotlin：空安全
来源：http://pem.yj20258.top

val n: String? = null;  n?.length
来源：http://axf.cucudq.cn

[T05] Kotlin：when 表达式
来源：http://ixu.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bpd.gzhubu.top

[T06] Kotlin：集合映射
来源：http://qcw.xziqi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rsg.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://qgh.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uzz.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://utl.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://bcu.vqdsnc.cn

[T09] Kotlin：扩展函数
来源：http://tna.hnqzz.top

fun String.exclaim() = this + "!"
来源：http://ykh.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://nsr.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gys.daxiang520.top

[T11] Kotlin：协程
来源：http://yjb.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qtj.nanxuanxn.top

[T12] Kotlin：解构声明
来源：http://jdf.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://god.shzxlz.cn

[T13] Kotlin：只读 Map
来源：http://ajv.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://vvg.bjfxy.top

[T14] Kotlin：循环
来源：http://lig.yj20258888.top

for (i in 1..10) println(i)
来源：http://qfa.xuanzx.com

[T15] Kotlin：接口
来源：http://jwc.aibaodan.cn

interface Shape { fun area(): Double }
来源：http://gry.sysykeji.top

[T16] Swift：Hello World
来源：http://eli.zdbjq.cn

print("Hello")
来源：http://odr.guannengcc.top

[T17] Swift：变量与常量
来源：http://hcd.mhx1999.top

var a = 1;  let b = 2
来源：http://lxm.tanke756.top

[T18] Swift：字符串插值
来源：http://ual.dianchejie.cn

"值: \(b)"
来源：http://apr.ywan-chungtsiang.top

[T19] Swift：可选绑定
来源：http://bpc.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://ttb.tanke756.top

[T20] Swift：数组操作
来源：http://hqc.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://wjl.shangyingyoupin.top

[T21] Swift：遍历
来源：http://cdm.zdbjq.cn

for x in a { print(x) }
来源：http://cyh.yueranfly.top

[T22] Swift：字典
来源：http://kyk.ctjpmb.com

var d = ["a": 1];  d["b"] = 2
来源：http://yay.tianlin.xyz

[T23] Swift：函数
来源：http://rxw.jinghuilouyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dfs.fktsv.cn

[T24] Swift：闭包
来源：http://ltm.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://osf.zhixingplan.top


<!-- 参考信息 -->