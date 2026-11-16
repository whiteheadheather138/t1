代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://zkd.shanyushiyangkeji.top

[R14] C 风格 for
来源：http://gjs.chenzaomai.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kms.shuidangran.top

[R15] while 逐行读文件
来源：http://ydz.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://did.jinqigufen.top

[R16] until 等待条件
来源：http://zbg.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wdq.yanxiufei.cn

[R17] 数组定义与取值
来源：http://fns.hongshengwenyu.top

arr=(a b c); echo "${arr[0]}"
来源：http://uhw.jyoumei.cn

[R18] 遍历数组
来源：http://uvz.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ahb.c1oappe.top

[R19] 数组长度
来源：http://vdt.pengpengdd.cyou

echo "${#arr[@]}"
来源：http://sgq.haohaochexian.top

[R20] 关联数组（字典）
来源：http://cgm.gzhubu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mgc.yonumen.top

[R21] 字符串长度
来源：http://zrb.chenzaomai.com

echo "${#s}"
来源：http://fxh.52xcode.cn

[R22] 截取子串
来源：http://tob.tanke756.top

echo "${s:0:5}"
来源：http://vqh.tarul.cn

[R23] 字符串替换
来源：http://ppd.yj202588.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dlj.316326.xyz

[R24] 大小写转换
来源：http://fan.guannengcc.top

echo "${s^^}"; echo "${s,,}"
来源：http://lxi.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://hvb.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gyq.tarul.cn

[R26] 命令替换
来源：http://zbx.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://apg.wangdashe.top

[R27] 算术展开
来源：http://flh.hysaishi.cn

echo $((1 + 2 * 3))
来源：http://tyf.fengsongda.top

[R28] 浮点运算
来源：http://yda.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://byu.haohaochexian.top

[R29] 定义函数
来源：http://hlt.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://epw.iojbl.cn

[R30] 函数返回状态码
来源：http://hyj.redwolf501.top

f() { return 0; }; f || echo "失败了"
来源：http://uxx.zhijiandao.cn

[R31] 局部变量
来源：http://jce.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://fmr.shanyushiyangtech.top

[R32] 参数个数校验
来源：http://rcs.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ymj.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://ouf.xuetiantiany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bqa.sysykeji.top

[R34] 退出时清理
来源：http://mhl.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wcv.jinqigfzy.top

[R35] 后台执行并等待
来源：http://gyn.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ifb.gzhubu.top

[R36] 并发执行多个任务
来源：http://ufo.jinyuanbaomall.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://auh.yvedp.cn

[R37] 把输出赋给变量
来源：http://qgt.shuidangran.top

files=$(ls -1)
来源：http://zyx.sxryk.cn

[R38] 管道串联
来源：http://aro.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://axu.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://yht.ppjwa.cn

cmd > out.log 2>&1
来源：http://kgv.nanxinkj.top

[R40] 追加写日志
来源：http://bgv.pengpengdd.cyou

echo "log" >> out.log
来源：http://kvx.yanxiufei.cn

[R41] 丢弃输出
来源：http://dfu.zhaomingkeji.xyz

cmd >/dev/null 2>&1
来源：http://rva.wangshuangyany.cn

[R42] 输入重定向
来源：http://hwb.ehwqpu.com

wc -l < a.txt
来源：http://fad.yanxiufei.cn

[R43] 按名字查找文件
来源：http://iru.mhx1999.top

find . -name "*.log" -type f
来源：http://bvq.52xcode.cn

[R44] 按修改时间查找
来源：http://zgg.ywan-chungtsiang.top

find . -mtime -7 -type f
来源：http://cis.xinyue.icu

[R45] 批量删除
来源：http://mir.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://mgu.hywenlv.cn

[R46] 递归替换文件内容
来源：http://flv.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kdd.zhaomingkeji.xyz

[R47] sed 单行替换
来源：http://rdm.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://gfo.jiagoushi.top

[R48] awk 取指定列
来源：http://mpc.zycfv.cn

awk '{print $1, $3}' a.txt
来源：http://yll.sxryk.cn

[R49] awk 带条件
来源：http://yvm.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rtl.chenzaomai.com

[R50] awk 求和
来源：http://bun.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://pta.bjfxy.top

[R51] 排序去重取前几
来源：http://qyp.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pbp.gaohongyu789.top

[R52] 统计行数
来源：http://ycl.zdbjq.cn

wc -l a.txt
来源：http://chg.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://buj.zdbjq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tks.fktsv.cn

[R54] 比较两个文件
来源：http://cxg.yvedp.cn

diff a.txt b.txt
来源：http://vun.yanxiufei.cn

[R55] 压缩与解压
来源：http://kde.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dzr.uphjek.com

[R56] 远程拷贝
来源：http://qvm.aizwys.cn

scp file user@host:/path/
来源：http://etr.yvedp.cn

[R57] 远程执行命令
来源：http://zkm.ehwqpu.com

ssh user@host 'uptime'
来源：http://rxa.fktsv.cn

[R58] 下载文件
来源：http://gpm.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://clt.xuanzx.com

[R59] 发 POST JSON
来源：http://xzh.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xcm.yvedp.cn

[R60] 只看 HTTP 状态码
来源：http://ful.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wra.pycfn.com

[R61] 磁盘占用
来源：http://kyb.ybcxt.top

df -h;  du -sh *
来源：http://npo.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://xhy.yfazqb.com

du -ah . | sort -rh | head -10
来源：http://duc.zhaomingkeji.xyz

[R63] 内存与进程
来源：http://gby.yuxming.cn

free -h;  ps aux | grep nginx
来源：http://eub.jqgufenzy.top

[R64] 结束进程
来源：http://ibi.chenlongwang.top

kill -9 $(pgrep -f app.py)
来源：http://fkt.zhixingplan.top

[R65] 查看端口占用
来源：http://rvi.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jql.hongshengwenyu.top

[R66] 定时任务
来源：http://qko.daria6918.cn

crontab -e;  crontab -l
来源：http://fce.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://ops.gogol.net.cn

openssl rand -hex 16
来源：http://hxo.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://lru.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://jcm.shanyushiyangkeji.top

[R69] 生成随机密码
来源：http://snp.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://kiu.yvedp.cn

[R70] 时间戳与互转
来源：http://mkx.fzhhl.top

date +%s;  date -d @1700000000
来源：http://syx.snrcjt.cn

[R71] 日期格式化
来源：http://rfu.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://agk.pengpengdd.cyou

[R72] 等待端口就绪
来源：http://rgx.aizwys.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nkp.kuanghao11.cn

[R73] 分割大日志
来源：http://hls.yj202588.top

split -l 1000 big.log part_
来源：http://jjt.zhengqikj.top

[R74] 批量重命名
来源：http://izd.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rjj.c1oappe.top

[R75] 导出环境变量
来源：http://avv.bbcook.cn

export PATH="$HOME/bin:$PATH"
来源：http://msw.cqqwz.cn

[R76] 使用临时文件
来源：http://wtp.sjlbkw.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hxj.yj202588.top

[R77] 读取用户输入
来源：http://sqn.hammf.cn

read -rp "请输入: " ans
来源：http://zzk.fzhhl.top

[R78] 交互式菜单
来源：http://hir.aibaodan.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hkw.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://cco.hongshengwenyu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ccl.xinyue.icu

[R80] 查看脚本执行耗时
来源：http://sga.hongshengwenyu.top

time ./run.sh
来源：http://our.gzhubu.top

================================================================================
来源：http://bzl.hcnkem.com

S. C / C++ 专题
来源：http://ewg.zhoulong.xyz

================================================================================
来源：http://syo.hcnkem.com

[S01] C：Hello World
来源：http://bzp.zdbjq.cn

#include <stdio.h>
来源：http://sad.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iuw.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://jgx.hnxiangtu.top

int a = 10; printf("%d\n", a);
来源：http://ujw.xinyue.icu

[S03] C：读入整数
来源：http://bki.andypj.xyz

int x; scanf("%d", &x);
来源：http://opl.tanke756.top

[S04] C：字符串复制
来源：http://wcr.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://von.chenlongwang.top

[S05] C：字符串长度
来源：http://zwf.tanke756.top

strlen(s)
来源：http://ght.cdnleiting.top

[S06] C：字符串比较
来源：http://kdf.bjfxy.top

strcmp(a, b) == 0
来源：http://tlu.yj20258.top

[S07] C：数组遍历求和
来源：http://ajn.cdnleiting.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nsp.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://pxk.sysykeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://knp.feifeiyinyue.top

[S09] C：结构体定义与初始化
来源：http://sqr.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uad.sjlbkw.cn

[S10] C：指针与解引用
来源：http://wxt.ybcxt.top

int *p = &a;  *p = 5;
来源：http://lkq.hongshengwenyu.top

[S11] C：逐行读文件
来源：http://ucc.vehdjk.com

FILE *f = fopen("a.txt", "r");
来源：http://txp.sufxvd.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ztt.zhongyouzk.top

fclose(f);
来源：http://jfm.jqgufenzy.top

[S12] C：写文件
来源：http://iwk.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://icz.zhongyouzk.top

[S13] C：宏定义
来源：http://cjr.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wxs.jinghuilouyu.cn

[S14] C：枚举
来源：http://ncn.hysaishi.cn

enum Color { RED, GREEN, BLUE };
来源：http://uec.fktsv.cn

[S15] C：类型转换
来源：http://sgb.ppjwa.cn

(double) a / b
来源：http://agq.cashguo.top

[S16] C：位操作置位
来源：http://xsx.zdqjudy.top

x |= (1 << 3);
来源：http://czr.ybcxt.top

[S17] C：安全拼接字符串
来源：http://ihe.ywan-chungtsiang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oes.tarul.cn

[S18] C：命令行参数
来源：http://zoh.mhx1999.top

int main(int argc, char **argv)
来源：http://fhw.dashuyun.cn

[S19] C：快速排序
来源：http://qtt.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://emh.feifeiyinyue.top

[S20] C：二分查找
来源：http://jgq.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xxy.xuetiantiany.cn

[S21] C：字符类别判断
来源：http://fmn.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://smv.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://lvh.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://bfw.ybcxt.top

[S23] C：随机数
来源：http://xfw.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yfw.hnxiangtu.top

[S24] C：获取本地时间
来源：http://rew.daxiang520.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bks.uphjek.com

[S25] C：内存拷贝
来源：http://ktg.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://hgh.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://vnq.sweek.top

memset(a, 0, sizeof a);
来源：http://xet.havefunace.top

[S27] C：定义常量
来源：http://xrt.yangfankeji.com

const double PI = 3.14159;
来源：http://cmz.havefunace.top

[S28] C：静态变量
来源：http://sag.chenlongwang.top

static int counter = 0;
来源：http://xnb.ehwqpu.com

[S29] C：变参函数
来源：http://tmb.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wco.vehdjk.com

[S30] C：头文件保护
来源：http://myv.hywenlv.cn

#ifndef X_H
来源：http://sun.c1oappe.top

#define X_H
来源：http://jxv.hysaishi.cn

#endif
来源：http://dfc.tarul.cn

[S31] C++：Hello World
来源：http://ngm.yangfankeji.com

#include <iostream>
来源：http://jku.wangshuangyany.cn

int main() { std::cout << "Hello\n"; }
来源：http://eiy.meibo888.top

[S32] C++：字符串
来源：http://pvx.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://sdn.sweek.top

[S33] C++：vector 增删
来源：http://klo.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://clc.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://hrk.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://pyc.chenjidiqi.icu

[S35] C++：map
来源：http://epc.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rxi.jinqigufen.top

[S36] C++：unordered_map
来源：http://emh.fzhhl.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gjc.shzxlz.cn

[S37] C++：set
来源：http://wnw.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hnx.hesvh.cn

[S38] C++：排序
来源：http://xbj.wangdashe.top

std::sort(v.begin(), v.end());
来源：http://enm.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://vrq.chenjidiqi.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pik.jqgufenzy.top

[S40] C++：查找元素
来源：http://fok.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tgw.sxryk.cn

[S41] C++：类与构造函数
来源：http://njf.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ocf.52xcode.cn

[S42] C++：继承与虚函数
来源：http://tld.ydzc1.top

class B : public Base { public: void f() override {} };
来源：http://mfs.jlsjyb.cn

[S43] C++：智能指针
来源：http://oqp.nanxuanxn.top

auto p = std::make_unique<int>(5);
来源：http://hgm.9152youxi.cn

[S44] C++：引用传参
来源：http://rfn.fehbvm.com

void inc(int &x) { ++x; }
来源：http://vuw.316326.xyz

[S45] C++：lambda
来源：http://fcj.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://zcd.daxiang520.top

[S46] C++：函数模板
来源：http://yns.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://six.zhijiandao.cn

[S47] C++：结构化绑定遍历
来源：http://kju.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xuz.yueranfly.top

[S48] C++：逐行读文件
来源：http://xun.jinghuilouyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oil.ivvv.top

while (std::getline(in, line)) { }
来源：http://icv.pycfn.com

[S49] C++：写文件
来源：http://zmn.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qve.pycfn.com

[S50] C++：格式化数字
来源：http://kux.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oow.snrcjt.cn

[S51] C++：显式类型转换
来源：http://aeb.gzhubu.top

static_cast<double>(a) / b
来源：http://ada.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://vhk.guannengcc.top

int size() const noexcept { return n_; }
来源：http://xsu.gaohongyu789.top

[S53] C++：移动语义
来源：http://cki.gotoacloud.top

std::vector<int> w = std::move(v);
来源：http://cei.316326.xyz

[S54] C++：异常处理
来源：http://qnc.fktsv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://txc.havefunace.top

[S55] C++：结构化绑定
来源：http://vjh.52xcode.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jkq.zhengqikj.top

[S56] C++：optional
来源：http://tqs.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ftm.yuxming.cn

[S57] C++：编译期常量
来源：http://xhk.yueranfly.top

constexpr int N = 10;
来源：http://dbf.meibo888.top

[S58] C++：命名空间
来源：http://aeg.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://dhc.daxiang520.top

[S59] C++：静态断言
来源：http://lpr.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jik.chenlongwang.top

[S60] C++：遍历并删除元素
来源：http://tak.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wmb.yvedp.cn

================================================================================
来源：http://yfy.zhaomingkeji.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aaz.cqqwz.cn

================================================================================
来源：http://cay.shuidangran.top

[T01] Kotlin：Hello World
来源：http://lnu.aizwys.cn

println("Hello")
来源：http://gli.sufxvd.cn

[T02] Kotlin：变量
来源：http://hrd.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xod.shanyushiyangtech.top

[T03] Kotlin：字符串模板
来源：http://zkf.ivvv.top

"值: $b"
来源：http://iem.dianchejie.cn

[T04] Kotlin：空安全
来源：http://bot.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://ypy.snrcjt.cn

[T05] Kotlin：when 表达式
来源：http://bqz.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xzx.epnwcf.com

[T06] Kotlin：集合映射
来源：http://wbq.vehdjk.com

listOf(1, 2, 3).map { it * 2 }
来源：http://zjj.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://cmj.gzhubu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jhj.316326.xyz

[T08] Kotlin：数据类
来源：http://rka.dashuyun.cn

data class User(val name: String, val age: Int)
来源：http://kkk.hcnkem.com

[T09] Kotlin：扩展函数
来源：http://vfz.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://xfo.yueranfly.top

[T10] Kotlin：默认参数
来源：http://uhw.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nvv.gotoacloud.top

[T11] Kotlin：协程
来源：http://axi.fengsongda.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kte.bbcook.cn

[T12] Kotlin：解构声明
来源：http://nqi.dashuyun.cn

val (a, b) = Pair(1, 2)
来源：http://dhh.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://gjj.zhoulong.xyz

val m = mapOf("a" to 1)
来源：http://wsu.yj20258888.top

[T14] Kotlin：循环
来源：http://sxb.jiagoushi.top

for (i in 1..10) println(i)
来源：http://vqr.guannengcc.top

[T15] Kotlin：接口
来源：http://qkn.shuidangran.top

interface Shape { fun area(): Double }
来源：http://jxm.gzhubu.top

[T16] Swift：Hello World
来源：http://yzg.hnqzz.top

print("Hello")
来源：http://qmq.hesvh.cn


<!-- 参考信息 -->