代发 wailian999

echo "${#s}"
来源：http://mdn.jinqigfzy.top

[R22] 截取子串
来源：http://rom.aibaodan.cn

echo "${s:0:5}"
来源：http://zpd.birdmap.top

[R23] 字符串替换
来源：http://izh.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nfm.cashguo.top

[R24] 大小写转换
来源：http://gus.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mpn.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://lpx.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kmz.yueranfly.top

[R26] 命令替换
来源：http://zpp.yvedp.cn

now=$(date +%F); echo "$now"
来源：http://ios.xingfuxueyuan.xyz

[R27] 算术展开
来源：http://vpy.xinyue.icu

echo $((1 + 2 * 3))
来源：http://uvv.svipenyu.cn

[R28] 浮点运算
来源：http://fxx.jinqigfzy.top

echo "scale=2; 10/3" | bc
来源：http://edu.0kj1m.cn

[R29] 定义函数
来源：http://vet.nanxinkj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eph.fzhhl.top

[R30] 函数返回状态码
来源：http://zbi.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://qea.quarkkingdee.top

[R31] 局部变量
来源：http://url.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://kqh.svipenyu.cn

[R32] 参数个数校验
来源：http://rjq.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cxu.shanyushiyangtech.top

[R33] 捕获错误并提示行号
来源：http://rdg.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gah.sysykeji.top

[R34] 退出时清理
来源：http://ylj.havefunace.top

trap 'rm -f "$tmp"' EXIT
来源：http://xih.nanxinkj.top

[R35] 后台执行并等待
来源：http://ata.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://cjl.yongpay.top

[R36] 并发执行多个任务
来源：http://eej.snrcjt.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kcy.hysaishi.cn

[R37] 把输出赋给变量
来源：http://fdg.vqdsnc.cn

files=$(ls -1)
来源：http://mfe.sysykeji.top

[R38] 管道串联
来源：http://xmf.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://dor.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://mcm.yj20258.top

cmd > out.log 2>&1
来源：http://zjw.pycfn.com

[R40] 追加写日志
来源：http://xpo.cqqwz.cn

echo "log" >> out.log
来源：http://qqj.guannengcc.top

[R41] 丢弃输出
来源：http://yoo.zhoulong.xyz

cmd >/dev/null 2>&1
来源：http://euq.zhongyouzk.top

[R42] 输入重定向
来源：http://jgz.jianghu66.top

wc -l < a.txt
来源：http://qut.xuanzx.com

[R43] 按名字查找文件
来源：http://mks.yj20258.top

find . -name "*.log" -type f
来源：http://sop.xingfuxueyuan.xyz

[R44] 按修改时间查找
来源：http://znt.wangdashe.top

find . -mtime -7 -type f
来源：http://gve.c1oappe.top

[R45] 批量删除
来源：http://bqv.yvedp.cn

find . -name "*.tmp" -delete
来源：http://bnt.tianlin.xyz

[R46] 递归替换文件内容
来源：http://qpj.shzxlz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rpx.nanxuanxn.top

[R47] sed 单行替换
来源：http://gdx.ctjpmb.com

sed -i 's/foo/bar/g' a.txt
来源：http://vmo.mhx1999.top

[R48] awk 取指定列
来源：http://lqe.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://kat.yangfankeji.com

[R49] awk 带条件
来源：http://djy.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vwo.ivvv.top

[R50] awk 求和
来源：http://iyy.c1oappe.top

awk '{s += $2} END {print s}' a.txt
来源：http://kdj.xingfuxueyuan.xyz

[R51] 排序去重取前几
来源：http://pyw.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ovt.pengpengdd.cyou

[R52] 统计行数
来源：http://yyz.nanxuanxn.top

wc -l a.txt
来源：http://hcr.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://bnc.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kzw.fehbvm.com

[R54] 比较两个文件
来源：http://ytq.xingfuxueyuan.xyz

diff a.txt b.txt
来源：http://tmp.jinqigufen.top

[R55] 压缩与解压
来源：http://uub.nanxinkj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://thg.nanxinkj.top

[R56] 远程拷贝
来源：http://gas.aizwys.cn

scp file user@host:/path/
来源：http://dpf.shzxlz.cn

[R57] 远程执行命令
来源：http://jrr.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://lwc.hesvh.cn

[R58] 下载文件
来源：http://mmw.tarul.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vjb.316326.xyz

[R59] 发 POST JSON
来源：http://yen.hywenlv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xtr.epnwcf.com

[R60] 只看 HTTP 状态码
来源：http://izb.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zdw.jyoumei.cn

[R61] 磁盘占用
来源：http://ylb.guowangkeji.top

df -h;  du -sh *
来源：http://ycy.wangdashe.top

[R62] 找最占空间的文件
来源：http://omf.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://cyh.xuetiantiany.cn

[R63] 内存与进程
来源：http://vev.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://kss.cqqwz.cn

[R64] 结束进程
来源：http://wpz.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://nna.zdqjudy.top

[R65] 查看端口占用
来源：http://ixa.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kaw.andypj.xyz

[R66] 定时任务
来源：http://oim.xuetiantiany.cn

crontab -e;  crontab -l
来源：http://vwk.hammf.cn

[R67] 生成随机十六进制串
来源：http://vgo.sweek.top

openssl rand -hex 16
来源：http://rmb.gotoacloud.top

[R68] 计算文件校验值
来源：http://ive.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://xoj.yanxiufei.cn

[R69] 生成随机密码
来源：http://ebz.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://fzs.tian-w.cn

[R70] 时间戳与互转
来源：http://amo.cashguo.top

date +%s;  date -d @1700000000
来源：http://sch.chenzaomai.com

[R71] 日期格式化
来源：http://dkz.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://svt.ybcxt.top

[R72] 等待端口就绪
来源：http://vju.quarkkingdee.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ixl.ppjwa.cn

[R73] 分割大日志
来源：http://sbn.aizwys.cn

split -l 1000 big.log part_
来源：http://twu.uphjek.com

[R74] 批量重命名
来源：http://zef.ppjwa.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gjj.hnxiangtu.top

[R75] 导出环境变量
来源：http://itq.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://amq.vehdjk.com

[R76] 使用临时文件
来源：http://xal.cheryme.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rgw.0kj1m.cn

[R77] 读取用户输入
来源：http://lks.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://vyp.yj202588.top

[R78] 交互式菜单
来源：http://hxc.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uye.daria6918.cn

[R79] 解析命令行选项
来源：http://dmt.svipenyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hcc.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://rfz.gotoacloud.top

time ./run.sh
来源：http://cug.shuidangran.top

================================================================================
来源：http://ujk.cheryme.top

S. C / C++ 专题
来源：http://uie.yj20258888.top

================================================================================
来源：http://wci.jlsjyb.cn

[S01] C：Hello World
来源：http://cjw.smart0.xyz

#include <stdio.h>
来源：http://myc.fzhhl.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://shs.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://seu.pengpengdd.cyou

int a = 10; printf("%d\n", a);
来源：http://pxg.wangshuangyany.cn

[S03] C：读入整数
来源：http://lkn.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://epn.yanxiufei.cn

[S04] C：字符串复制
来源：http://smq.daxiang520.top

char dst[32]; strcpy(dst, "hi");
来源：http://hdz.hnxiangtu.top

[S05] C：字符串长度
来源：http://fkm.feifeiyinyue.top

strlen(s)
来源：http://udi.guannengcc.top

[S06] C：字符串比较
来源：http://jbj.quarkkingdee.top

strcmp(a, b) == 0
来源：http://lpi.andypj.xyz

[S07] C：数组遍历求和
来源：http://djs.shuidangran.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nqk.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://kyc.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://exm.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://sgl.jqgfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ski.zhoulong.xyz

[S10] C：指针与解引用
来源：http://tfj.shuidangran.top

int *p = &a;  *p = 5;
来源：http://zdf.guannengcc.top

[S11] C：逐行读文件
来源：http://qwd.kuanghao11.cn

FILE *f = fopen("a.txt", "r");
来源：http://noo.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ent.hongshengwenyu.top

fclose(f);
来源：http://uwh.ivvv.top

[S12] C：写文件
来源：http://wyw.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bxq.guannengcc.top

[S13] C：宏定义
来源：http://awg.haohaochexian.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gcd.0kj1m.cn

[S14] C：枚举
来源：http://dud.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://our.nanxuanxn.top

[S15] C：类型转换
来源：http://nla.cdnleiting.top

(double) a / b
来源：http://loi.jqgufenzy.top

[S16] C：位操作置位
来源：http://plx.zycfv.cn

x |= (1 << 3);
来源：http://xqt.tarul.cn

[S17] C：安全拼接字符串
来源：http://adc.guowangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xew.hfpthk.cn

[S18] C：命令行参数
来源：http://sjq.wangshuangyany.cn

int main(int argc, char **argv)
来源：http://eny.tarul.cn

[S19] C：快速排序
来源：http://hha.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qgk.gotoacloud.top

[S20] C：二分查找
来源：http://bdo.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ytc.hcnkem.com

[S21] C：字符类别判断
来源：http://oov.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://faa.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://ulz.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://npb.andypj.xyz

[S23] C：随机数
来源：http://mzi.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://esz.redwolf501.top

[S24] C：获取本地时间
来源：http://rqf.zhoulong.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vya.gzhubu.top

[S25] C：内存拷贝
来源：http://frk.jlsjyb.cn

memcpy(dst, src, n);
来源：http://pgj.hywenlv.cn

[S26] C：内存清零
来源：http://vlk.316326.xyz

memset(a, 0, sizeof a);
来源：http://drq.dashuyun.cn

[S27] C：定义常量
来源：http://ybq.yuanzhike.top

const double PI = 3.14159;
来源：http://epw.daria6918.cn

[S28] C：静态变量
来源：http://kmh.xuanzx.com

static int counter = 0;
来源：http://nsf.hongshengwenyu.top

[S29] C：变参函数
来源：http://ktq.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://imj.sysykeji.top

[S30] C：头文件保护
来源：http://kqo.haohaochexian.top

#ifndef X_H
来源：http://hib.yvedp.cn

#define X_H
来源：http://zwy.hnxiangtu.top

#endif
来源：http://ovx.yangfankeji.com

[S31] C++：Hello World
来源：http://wyb.tianlin.xyz

#include <iostream>
来源：http://jjm.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://rzu.xuanzx.com

[S32] C++：字符串
来源：http://daw.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://vpf.316326.xyz

[S33] C++：vector 增删
来源：http://rrq.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wpx.iojbl.cn

[S34] C++：遍历 vector
来源：http://uqe.ybcxt.top

for (auto &x : v) { std::cout << x; }
来源：http://sro.uphjek.com

[S35] C++：map
来源：http://xgi.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pqm.zhijiandao.cn

[S36] C++：unordered_map
来源：http://uyy.ctjpmb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://teh.haohaochexian.top

[S37] C++：set
来源：http://xxv.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pzp.guowangkeji.top

[S38] C++：排序
来源：http://ntw.vehdjk.com

std::sort(v.begin(), v.end());
来源：http://khb.wangshuangyany.cn

[S39] C++：自定义比较器排序
来源：http://sqo.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qvd.gaohongyu789.top

[S40] C++：查找元素
来源：http://dee.ctjpmb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://asv.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://gub.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bto.yj20258888.top

[S42] C++：继承与虚函数
来源：http://rss.yuxming.cn

class B : public Base { public: void f() override {} };
来源：http://gxg.cdnleiting.top

[S43] C++：智能指针
来源：http://onm.pengpengdd.cyou

auto p = std::make_unique<int>(5);
来源：http://qln.yfazqb.com

[S44] C++：引用传参
来源：http://okk.hcnkem.com

void inc(int &x) { ++x; }
来源：http://jap.xziqi.cn

[S45] C++：lambda
来源：http://mru.xuetiantiany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zet.kuanghao11.cn

[S46] C++：函数模板
来源：http://gkp.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zfq.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://lii.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fws.havefunace.top

[S48] C++：逐行读文件
来源：http://iys.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://hbz.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://ief.ppjwa.cn

[S49] C++：写文件
来源：http://xzg.cucudq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gjd.sysykeji.top

[S50] C++：格式化数字
来源：http://saq.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aam.zhixingplan.top

[S51] C++：显式类型转换
来源：http://snh.jiagoushi.top

static_cast<double>(a) / b
来源：http://fkh.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://eei.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://stz.fengsongda.top

[S53] C++：移动语义
来源：http://fqi.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://oer.hywenlv.cn

[S54] C++：异常处理
来源：http://haj.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eea.jqgfzy.top

[S55] C++：结构化绑定
来源：http://dfy.yvedp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vzm.xuetiantiany.cn

[S56] C++：optional
来源：http://xkm.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mro.sjlbkw.cn

[S57] C++：编译期常量
来源：http://cux.jqgfzy.top

constexpr int N = 10;
来源：http://ygg.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://bmx.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://tql.birdmap.top

[S59] C++：静态断言
来源：http://nln.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oyh.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://ary.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yku.shuidangran.top

================================================================================
来源：http://cxp.chenjidiqi.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oao.yvedp.cn

================================================================================
来源：http://xfx.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://vfv.shuidangran.top

println("Hello")
来源：http://uuu.yj20258888.top

[T02] Kotlin：变量
来源：http://hlo.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ctc.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://pyd.gogol.net.cn

"值: $b"
来源：http://tjs.xziqi.cn

[T04] Kotlin：空安全
来源：http://shw.sufxvd.cn

val n: String? = null;  n?.length
来源：http://upi.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://qod.yongpay.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uhz.mhx1999.top

[T06] Kotlin：集合映射
来源：http://fsg.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uwp.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://gxa.iojbl.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mni.ctjpmb.com

[T08] Kotlin：数据类
来源：http://sxr.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://vxo.fzhhl.top

[T09] Kotlin：扩展函数
来源：http://kbu.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://dgx.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://cje.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://new.yj20258888.top

[T11] Kotlin：协程
来源：http://reb.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dqh.hcnkem.com

[T12] Kotlin：解构声明
来源：http://ljt.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://ygx.hnxiangtu.top

[T13] Kotlin：只读 Map
来源：http://ilw.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://rvn.yanxiufei.cn

[T14] Kotlin：循环
来源：http://ywb.hfpthk.cn

for (i in 1..10) println(i)
来源：http://apk.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://pfm.guowangkeji.top

interface Shape { fun area(): Double }
来源：http://ygb.wangshuangyany.cn

[T16] Swift：Hello World
来源：http://uae.hywenlv.cn

print("Hello")
来源：http://igr.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://gew.yj20258888.top

var a = 1;  let b = 2
来源：http://liw.yonumen.top

[T18] Swift：字符串插值
来源：http://lul.gogol.net.cn

"值: \(b)"
来源：http://iyl.ivvv.top

[T19] Swift：可选绑定
来源：http://erv.uphjek.com

if let n = opt { print(n) }
来源：http://wxa.meibo888.top

[T20] Swift：数组操作
来源：http://ywi.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://evg.52xcode.cn

[T21] Swift：遍历
来源：http://sub.shuidangran.top

for x in a { print(x) }
来源：http://tou.sysykeji.top

[T22] Swift：字典
来源：http://pxn.yanxiufei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hxu.pycfn.com

[T23] Swift：函数
来源：http://qjd.tanke756.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kyd.c1oappe.top

[T24] Swift：闭包
来源：http://jds.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fes.ydzc1.top


<!-- 参考信息 -->