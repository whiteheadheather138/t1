代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://tuo.yj20258888.top

[R14] C 风格 for
来源：http://aji.xziqi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kzu.9152youxi.cn

[R15] while 逐行读文件
来源：http://zug.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://esv.hcnkem.com

[R16] until 等待条件
来源：http://bsp.smart0.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fka.shuidangran.top

[R17] 数组定义与取值
来源：http://iwg.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://fis.redwolf501.top

[R18] 遍历数组
来源：http://bee.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fte.svipenyu.cn

[R19] 数组长度
来源：http://eon.jianghu66.top

echo "${#arr[@]}"
来源：http://xwr.fehbvm.com

[R20] 关联数组（字典）
来源：http://klm.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nyu.jianghu66.top

[R21] 字符串长度
来源：http://agi.xuetiantiany.cn

echo "${#s}"
来源：http://icl.jqgfzy.top

[R22] 截取子串
来源：http://oyx.redwolf501.top

echo "${s:0:5}"
来源：http://bxv.xziqi.cn

[R23] 字符串替换
来源：http://rzl.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pux.52xcode.cn

[R24] 大小写转换
来源：http://hvr.chenlongwang.top

echo "${s^^}"; echo "${s,,}"
来源：http://gzb.zhoulong.xyz

[R25] 去后缀 / 去前缀
来源：http://wmg.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://skt.bbcook.cn

[R26] 命令替换
来源：http://qee.yj202588.top

now=$(date +%F); echo "$now"
来源：http://nbk.pycfn.com

[R27] 算术展开
来源：http://wph.xziqi.cn

echo $((1 + 2 * 3))
来源：http://ram.cucudq.cn

[R28] 浮点运算
来源：http://atb.kuanghao11.cn

echo "scale=2; 10/3" | bc
来源：http://yqq.zhijiandao.cn

[R29] 定义函数
来源：http://vwm.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wgj.ctjpmb.com

[R30] 函数返回状态码
来源：http://jul.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://rvd.wangdashe.top

[R31] 局部变量
来源：http://gai.havefunace.top

f() { local x=1; echo "$x"; }
来源：http://xah.hywenlv.cn

[R32] 参数个数校验
来源：http://zor.zhiwuduotai.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xsj.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://eqt.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fdz.andypj.xyz

[R34] 退出时清理
来源：http://naa.daxiang520.top

trap 'rm -f "$tmp"' EXIT
来源：http://nts.nanxinkj.top

[R35] 后台执行并等待
来源：http://exj.ehwqpu.com

sleep 5 & pid=$!; wait "$pid"
来源：http://kfb.jiagoushi.top

[R36] 并发执行多个任务
来源：http://dnd.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bct.haohaochexian.top

[R37] 把输出赋给变量
来源：http://ygp.yvedp.cn

files=$(ls -1)
来源：http://oao.cdnleiting.top

[R38] 管道串联
来源：http://pjy.tarul.cn

cat a.txt | grep -i error | wc -l
来源：http://pdu.yfazqb.com

[R39] 重定向标准输出与错误
来源：http://upa.haohaochexian.top

cmd > out.log 2>&1
来源：http://hyf.pycfn.com

[R40] 追加写日志
来源：http://qdv.fengsongda.top

echo "log" >> out.log
来源：http://hin.xylfe.cn

[R41] 丢弃输出
来源：http://mgx.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://ims.cdnleiting.top

[R42] 输入重定向
来源：http://rzl.xylfe.cn

wc -l < a.txt
来源：http://agj.sxryk.cn

[R43] 按名字查找文件
来源：http://owi.smart0.xyz

find . -name "*.log" -type f
来源：http://ovg.jiagoushi.top

[R44] 按修改时间查找
来源：http://fyt.jyoumei.cn

find . -mtime -7 -type f
来源：http://rfc.dashuyun.cn

[R45] 批量删除
来源：http://frq.hywenlv.cn

find . -name "*.tmp" -delete
来源：http://dhc.aizwys.cn

[R46] 递归替换文件内容
来源：http://uvp.yj20258888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iqv.hfpthk.cn

[R47] sed 单行替换
来源：http://von.zdbjq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hio.sweek.top

[R48] awk 取指定列
来源：http://iem.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://pvy.xziqi.cn

[R49] awk 带条件
来源：http://oqu.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://elz.yj20258.top

[R50] awk 求和
来源：http://gdw.mhx1999.top

awk '{s += $2} END {print s}' a.txt
来源：http://qbs.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://xnx.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sng.bbcook.cn

[R52] 统计行数
来源：http://eix.ehwqpu.com

wc -l a.txt
来源：http://gsl.birdmap.top

[R53] 查看文件头与实时尾
来源：http://ngh.hammf.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cpi.bjfxy.top

[R54] 比较两个文件
来源：http://uzb.meibo888.top

diff a.txt b.txt
来源：http://iwf.xylfe.cn

[R55] 压缩与解压
来源：http://xzj.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qvn.yonumen.top

[R56] 远程拷贝
来源：http://hmw.fanxiaobao.xyz

scp file user@host:/path/
来源：http://lll.yj20258.top

[R57] 远程执行命令
来源：http://pdh.aizwys.cn

ssh user@host 'uptime'
来源：http://vxa.nanxuanxn.top

[R58] 下载文件
来源：http://dnr.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zbp.hammf.cn

[R59] 发 POST JSON
来源：http://eqq.zdqjudy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://znk.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://yfs.hesvh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://riq.yj202588.top

[R61] 磁盘占用
来源：http://ptf.jlsjyb.cn

df -h;  du -sh *
来源：http://rnr.xinyue.icu

[R62] 找最占空间的文件
来源：http://jge.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://gku.yonumen.top

[R63] 内存与进程
来源：http://qen.52xcode.cn

free -h;  ps aux | grep nginx
来源：http://izh.zhengqikj.top

[R64] 结束进程
来源：http://ger.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://rtn.pengpengdd.cyou

[R65] 查看端口占用
来源：http://nhb.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zyq.fengsongda.top

[R66] 定时任务
来源：http://hzj.cdnleiting.top

crontab -e;  crontab -l
来源：http://ngp.jianghu66.top

[R67] 生成随机十六进制串
来源：http://dqs.yj202588.top

openssl rand -hex 16
来源：http://ete.vehdjk.com

[R68] 计算文件校验值
来源：http://dsn.chenlongwang.top

sha256sum a.txt;  md5sum a.txt
来源：http://nbv.hammf.cn

[R69] 生成随机密码
来源：http://icb.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://dzw.tanke756.top

[R70] 时间戳与互转
来源：http://zib.ybcxt.top

date +%s;  date -d @1700000000
来源：http://dae.52xcode.cn

[R71] 日期格式化
来源：http://hqk.cheryme.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qxj.zhijiandao.cn

[R72] 等待端口就绪
来源：http://ldl.ivvv.top

until nc -z localhost 3306; do sleep 1; done
来源：http://msz.zhengqikj.top

[R73] 分割大日志
来源：http://gqi.yueranfly.top

split -l 1000 big.log part_
来源：http://szl.daria6918.cn

[R74] 批量重命名
来源：http://xaq.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hvd.vqdsnc.cn

[R75] 导出环境变量
来源：http://egg.yuanzhike.top

export PATH="$HOME/bin:$PATH"
来源：http://ubz.52xcode.cn

[R76] 使用临时文件
来源：http://xjh.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xxg.zhoulong.xyz

[R77] 读取用户输入
来源：http://nbw.aizwys.cn

read -rp "请输入: " ans
来源：http://fut.zdqjudy.top

[R78] 交互式菜单
来源：http://gct.shzxlz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kut.nanxinkj.top

[R79] 解析命令行选项
来源：http://hah.jyoumei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wwk.hywenlv.cn

[R80] 查看脚本执行耗时
来源：http://hcx.zhiwuduotai.top

time ./run.sh
来源：http://loq.ydjk.org.cn

================================================================================
来源：http://dsj.tanke756.top

S. C / C++ 专题
来源：http://xqp.sxryk.cn

================================================================================
来源：http://ndo.fehbvm.com

[S01] C：Hello World
来源：http://dov.yvedp.cn

#include <stdio.h>
来源：http://kzi.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ujj.tian-w.cn

[S02] C：变量与格式化输出
来源：http://cly.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://fyy.meibo888.top

[S03] C：读入整数
来源：http://fqk.0kj1m.cn

int x; scanf("%d", &x);
来源：http://hpa.yuanzhike.top

[S04] C：字符串复制
来源：http://qbz.yongpay.top

char dst[32]; strcpy(dst, "hi");
来源：http://fke.shangyingyoupin.top

[S05] C：字符串长度
来源：http://umb.jinqigfzy.top

strlen(s)
来源：http://sik.sxryk.cn

[S06] C：字符串比较
来源：http://ymq.tianlin.xyz

strcmp(a, b) == 0
来源：http://fyb.ehwqpu.com

[S07] C：数组遍历求和
来源：http://yqk.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vjc.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://mpp.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://frx.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://fmr.yangfankeji.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jkc.dianchejie.cn

[S10] C：指针与解引用
来源：http://gyb.cheryme.top

int *p = &a;  *p = 5;
来源：http://vac.pengpengdd.cyou

[S11] C：逐行读文件
来源：http://mjl.xinyue.icu

FILE *f = fopen("a.txt", "r");
来源：http://ojv.gaohongyu789.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lst.tarul.cn

fclose(f);
来源：http://sjn.fengsongda.top

[S12] C：写文件
来源：http://yan.gaohongyu789.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ema.bbcook.cn

[S13] C：宏定义
来源：http://tno.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ddg.cheryme.top

[S14] C：枚举
来源：http://zsm.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://lpm.chenzaomai.com

[S15] C：类型转换
来源：http://qnw.52xcode.cn

(double) a / b
来源：http://uuo.aibaodan.cn

[S16] C：位操作置位
来源：http://ggj.fzhhl.top

x |= (1 << 3);
来源：http://xnw.cashguo.top

[S17] C：安全拼接字符串
来源：http://kgc.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jnu.zhaomingkeji.xyz

[S18] C：命令行参数
来源：http://ytj.cashguo.top

int main(int argc, char **argv)
来源：http://llb.xziqi.cn

[S19] C：快速排序
来源：http://nyp.yj20258888.top

qsort(a, n, sizeof(int), cmp);
来源：http://mtm.zdqjudy.top

[S20] C：二分查找
来源：http://hok.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ahu.316326.xyz

[S21] C：字符类别判断
来源：http://txs.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tpe.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://oor.ybcxt.top

atoi("42");  strtod("3.14", NULL);
来源：http://lfu.shanyushiyangkeji.top

[S23] C：随机数
来源：http://xyt.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bov.daxiang520.top

[S24] C：获取本地时间
来源：http://wvh.aibaodan.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xuo.fengsongda.top

[S25] C：内存拷贝
来源：http://izt.nwbrower.top

memcpy(dst, src, n);
来源：http://ssi.hywenlv.cn

[S26] C：内存清零
来源：http://ybt.xinyue.icu

memset(a, 0, sizeof a);
来源：http://pjk.yfazqb.com

[S27] C：定义常量
来源：http://mye.wangdashe.top

const double PI = 3.14159;
来源：http://dii.hnxiangtu.top

[S28] C：静态变量
来源：http://gko.yanxiufei.cn

static int counter = 0;
来源：http://ijr.svipenyu.cn

[S29] C：变参函数
来源：http://nar.ctjpmb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lkv.quarkkingdee.top

[S30] C：头文件保护
来源：http://tgw.sweek.top

#ifndef X_H
来源：http://gbc.cheryme.top

#define X_H
来源：http://whv.jinghuilouyu.cn

#endif
来源：http://mdv.c1oappe.top

[S31] C++：Hello World
来源：http://idf.zhixingplan.top

#include <iostream>
来源：http://ebj.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://mao.daria6918.cn

[S32] C++：字符串
来源：http://rcd.0kj1m.cn

std::string s = "hi";  s += "!";
来源：http://xpj.hesvh.cn

[S33] C++：vector 增删
来源：http://qut.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ide.ivvv.top

[S34] C++：遍历 vector
来源：http://ccz.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://mic.nwbrower.top

[S35] C++：map
来源：http://hcj.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bfn.hnqzz.top

[S36] C++：unordered_map
来源：http://pdi.cqqwz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lar.gzhubu.top

[S37] C++：set
来源：http://jxy.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xea.ybcxt.top

[S38] C++：排序
来源：http://xbv.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://ioc.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://vrc.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fbr.sxryk.cn

[S40] C++：查找元素
来源：http://zyb.fanxiaobao.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ttl.ppjwa.cn

[S41] C++：类与构造函数
来源：http://mvz.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sdn.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://ffr.hywenlv.cn

class B : public Base { public: void f() override {} };
来源：http://vik.chenjidiqi.icu

[S43] C++：智能指针
来源：http://vuq.guowangkeji.top

auto p = std::make_unique<int>(5);
来源：http://gir.meibo888.top

[S44] C++：引用传参
来源：http://zgz.aizwys.cn

void inc(int &x) { ++x; }
来源：http://viq.gogol.net.cn

[S45] C++：lambda
来源：http://gib.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://kat.sjlbkw.cn

[S46] C++：函数模板
来源：http://fod.zhoulong.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ziy.nanxuanxn.top

[S47] C++：结构化绑定遍历
来源：http://mbm.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hgp.jinqigufen.top

[S48] C++：逐行读文件
来源：http://cse.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://amn.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://zki.redwolf501.top

[S49] C++：写文件
来源：http://lis.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://syh.aizwys.cn

[S50] C++：格式化数字
来源：http://soo.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yug.tianlin.xyz

[S51] C++：显式类型转换
来源：http://vbc.fehbvm.com

static_cast<double>(a) / b
来源：http://ghq.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://moq.nanxuanxn.top

int size() const noexcept { return n_; }
来源：http://nng.zdbjq.cn

[S53] C++：移动语义
来源：http://fks.shanyushiyangtech.top

std::vector<int> w = std::move(v);
来源：http://kkc.dashuyun.cn

[S54] C++：异常处理
来源：http://haj.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://thw.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://zfd.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uwq.jiagoushi.top

[S56] C++：optional
来源：http://xqa.gotoacloud.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lny.sweek.top

[S57] C++：编译期常量
来源：http://ydq.snrcjt.cn

constexpr int N = 10;
来源：http://rwh.9152youxi.cn

[S58] C++：命名空间
来源：http://wcl.zdbjq.cn

namespace ns { int f() { return 1; } }
来源：http://dai.sufxvd.cn

[S59] C++：静态断言
来源：http://ylw.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cik.haohaochexian.top

[S60] C++：遍历并删除元素
来源：http://ffm.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eby.yj202588.top

================================================================================
来源：http://klh.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tfr.feifeiyinyue.top

================================================================================
来源：http://big.aibaodan.cn

[T01] Kotlin：Hello World
来源：http://eba.shuidangran.top

println("Hello")
来源：http://kqy.jianghu66.top

[T02] Kotlin：变量
来源：http://cos.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://usr.uphjek.com

[T03] Kotlin：字符串模板
来源：http://jim.hesvh.cn

"值: $b"
来源：http://hwl.havefunace.top

[T04] Kotlin：空安全
来源：http://krg.andypj.xyz

val n: String? = null;  n?.length
来源：http://kza.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://rnp.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://elz.havefunace.top

[T06] Kotlin：集合映射
来源：http://dsq.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ytg.xinyue.icu

[T07] Kotlin：集合过滤
来源：http://ufk.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://obe.ydzc1.top

[T08] Kotlin：数据类
来源：http://fyq.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://epq.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://pkm.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://yka.yuxming.cn

[T10] Kotlin：默认参数
来源：http://qrf.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://bla.havefunace.top

[T11] Kotlin：协程
来源：http://qgz.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rhm.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://rvi.nwbrower.top

val (a, b) = Pair(1, 2)
来源：http://ped.pengpengdd.cyou

[T13] Kotlin：只读 Map
来源：http://wmr.gotoacloud.top

val m = mapOf("a" to 1)
来源：http://got.dianchejie.cn

[T14] Kotlin：循环
来源：http://dzr.jqgfzy.top

for (i in 1..10) println(i)
来源：http://jum.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://mdm.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://nzk.iojbl.cn

[T16] Swift：Hello World
来源：http://cjz.hysaishi.cn

print("Hello")
来源：http://wbn.hysaishi.cn


<!-- 参考信息 -->