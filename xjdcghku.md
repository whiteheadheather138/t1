代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://cpf.dashuyun.cn

[R14] C 风格 for
来源：http://vgk.tarul.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rqv.zdqjudy.top

[R15] while 逐行读文件
来源：http://ugu.52xcode.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://znu.zhiwuduotai.top

[R16] until 等待条件
来源：http://vbj.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uym.ydzc1.top

[R17] 数组定义与取值
来源：http://umh.hywenlv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ivz.zhixingplan.top

[R18] 遍历数组
来源：http://wui.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ilb.shanyushiyangkeji.top

[R19] 数组长度
来源：http://nhw.jlsjyb.cn

echo "${#arr[@]}"
来源：http://pmo.sysykeji.top

[R20] 关联数组（字典）
来源：http://gfu.yvedp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://npm.haohaochexian.top

[R21] 字符串长度
来源：http://gif.jinqigufen.top

echo "${#s}"
来源：http://gou.cdnleiting.top

[R22] 截取子串
来源：http://guc.jinqigfzy.top

echo "${s:0:5}"
来源：http://mji.cheryme.top

[R23] 字符串替换
来源：http://eyv.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://beu.ehwqpu.com

[R24] 大小写转换
来源：http://qvr.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://iwt.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://cqj.fengsongda.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hsq.tarul.cn

[R26] 命令替换
来源：http://fbg.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://mny.yj202588.top

[R27] 算术展开
来源：http://sww.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://bbh.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://mww.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://gwm.shangyingyoupin.top

[R29] 定义函数
来源：http://nms.xziqi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rat.zhongyouzk.top

[R30] 函数返回状态码
来源：http://nox.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://cdn.xinyue.icu

[R31] 局部变量
来源：http://vao.aibaodan.cn

f() { local x=1; echo "$x"; }
来源：http://job.ybcxt.top

[R32] 参数个数校验
来源：http://hdg.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eyy.yongpay.top

[R33] 捕获错误并提示行号
来源：http://nyw.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aqr.fktsv.cn

[R34] 退出时清理
来源：http://rhp.shzxlz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://asy.jinqigufen.top

[R35] 后台执行并等待
来源：http://ejj.daria6918.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jmg.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://hst.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zjz.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://cpm.cdnleiting.top

files=$(ls -1)
来源：http://acz.pengpengdd.cyou

[R38] 管道串联
来源：http://cgi.zdqjudy.top

cat a.txt | grep -i error | wc -l
来源：http://dvg.yonumen.top

[R39] 重定向标准输出与错误
来源：http://axz.gogol.net.cn

cmd > out.log 2>&1
来源：http://zbb.yvedp.cn

[R40] 追加写日志
来源：http://auy.ehwqpu.com

echo "log" >> out.log
来源：http://fxq.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://ecn.tianlin.xyz

cmd >/dev/null 2>&1
来源：http://ojo.kuanghao11.cn

[R42] 输入重定向
来源：http://xfi.chenzaomai.com

wc -l < a.txt
来源：http://qzj.0kj1m.cn

[R43] 按名字查找文件
来源：http://upn.xuetiantiany.cn

find . -name "*.log" -type f
来源：http://seu.chenlongwang.top

[R44] 按修改时间查找
来源：http://tbj.cashguo.top

find . -mtime -7 -type f
来源：http://col.pengpengdd.cyou

[R45] 批量删除
来源：http://lyx.vehdjk.com

find . -name "*.tmp" -delete
来源：http://tba.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://voi.jqgufenzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jhn.redwolf501.top

[R47] sed 单行替换
来源：http://bbl.sxryk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pow.ehwqpu.com

[R48] awk 取指定列
来源：http://dnf.zdbjq.cn

awk '{print $1, $3}' a.txt
来源：http://ore.yueranfly.top

[R49] awk 带条件
来源：http://knq.c1oappe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ipa.52xcode.cn

[R50] awk 求和
来源：http://eyg.pycfn.com

awk '{s += $2} END {print s}' a.txt
来源：http://esk.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://rez.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ltx.hywenlv.cn

[R52] 统计行数
来源：http://tal.nanxuanxn.top

wc -l a.txt
来源：http://ngm.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://qkh.zhoulong.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://swb.jinqigfzy.top

[R54] 比较两个文件
来源：http://pjm.hywenlv.cn

diff a.txt b.txt
来源：http://gok.jlsjyb.cn

[R55] 压缩与解压
来源：http://qqc.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jhe.hcnkem.com

[R56] 远程拷贝
来源：http://vrm.fktsv.cn

scp file user@host:/path/
来源：http://vwc.c1oappe.top

[R57] 远程执行命令
来源：http://wxz.fengsongda.top

ssh user@host 'uptime'
来源：http://tln.ydjk.org.cn

[R58] 下载文件
来源：http://lcy.redwolf501.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pzl.dianchejie.cn

[R59] 发 POST JSON
来源：http://fol.shanyushiyangtech.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zbr.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://zpu.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pcf.andypj.xyz

[R61] 磁盘占用
来源：http://wpm.meibo888.top

df -h;  du -sh *
来源：http://nwk.zhengqikj.top

[R62] 找最占空间的文件
来源：http://ukr.ydjk.org.cn

du -ah . | sort -rh | head -10
来源：http://udu.jinghuilouyu.cn

[R63] 内存与进程
来源：http://hki.tanke756.top

free -h;  ps aux | grep nginx
来源：http://jtj.jinyuanbaomall.cn

[R64] 结束进程
来源：http://daa.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://mtd.zhijiandao.cn

[R65] 查看端口占用
来源：http://zaq.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vpl.nwbrower.top

[R66] 定时任务
来源：http://vso.gzhubu.top

crontab -e;  crontab -l
来源：http://jux.havefunace.top

[R67] 生成随机十六进制串
来源：http://ccl.ywan-chungtsiang.top

openssl rand -hex 16
来源：http://kuw.xinyue.icu

[R68] 计算文件校验值
来源：http://ujq.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://arw.guowangkeji.top

[R69] 生成随机密码
来源：http://srr.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://yfy.yj20258888.top

[R70] 时间戳与互转
来源：http://zdz.havefunace.top

date +%s;  date -d @1700000000
来源：http://fgv.ydzc1.top

[R71] 日期格式化
来源：http://umq.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sgo.bjfxy.top

[R72] 等待端口就绪
来源：http://xyu.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://svh.hnqzz.top

[R73] 分割大日志
来源：http://xff.hcnkem.com

split -l 1000 big.log part_
来源：http://jez.xziqi.cn

[R74] 批量重命名
来源：http://sti.jinqigufen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pjn.yj202588.top

[R75] 导出环境变量
来源：http://fdl.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://naz.xziqi.cn

[R76] 使用临时文件
来源：http://mkc.guowangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tdd.316326.xyz

[R77] 读取用户输入
来源：http://vmc.andypj.xyz

read -rp "请输入: " ans
来源：http://pcm.xinyue.icu

[R78] 交互式菜单
来源：http://qpc.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://voc.jiagoushi.top

[R79] 解析命令行选项
来源：http://mio.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pyt.jinghuilouyu.cn

[R80] 查看脚本执行耗时
来源：http://wuv.yongpay.top

time ./run.sh
来源：http://rxt.yueranfly.top

================================================================================
来源：http://yre.shangyingyoupin.top

S. C / C++ 专题
来源：http://uyu.c1oappe.top

================================================================================
来源：http://kuj.chenlongwang.top

[S01] C：Hello World
来源：http://fbd.fehbvm.com

#include <stdio.h>
来源：http://ahs.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qew.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://ucu.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://dfe.kuanghao11.cn

[S03] C：读入整数
来源：http://dte.xylfe.cn

int x; scanf("%d", &x);
来源：http://xlv.cheryme.top

[S04] C：字符串复制
来源：http://pcy.hcnkem.com

char dst[32]; strcpy(dst, "hi");
来源：http://dcs.ehwqpu.com

[S05] C：字符串长度
来源：http://djo.daxiang520.top

strlen(s)
来源：http://kod.zdqjudy.top

[S06] C：字符串比较
来源：http://ris.aizwys.cn

strcmp(a, b) == 0
来源：http://dyk.zdqjudy.top

[S07] C：数组遍历求和
来源：http://gfr.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cbb.pycfn.com

[S08] C：动态内存分配与释放
来源：http://ain.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jmt.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://yka.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blz.hfpthk.cn

[S10] C：指针与解引用
来源：http://dfg.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://wob.hesvh.cn

[S11] C：逐行读文件
来源：http://ejm.jinghuilouyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://gnr.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ezh.52xcode.cn

fclose(f);
来源：http://hjf.jinyuanbaomall.cn

[S12] C：写文件
来源：http://dbg.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://njx.ehwqpu.com

[S13] C：宏定义
来源：http://zly.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wnb.zhoulong.xyz

[S14] C：枚举
来源：http://uyo.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://rfm.zhengqikj.top

[S15] C：类型转换
来源：http://ywj.shuidangran.top

(double) a / b
来源：http://fgj.haohaochexian.top

[S16] C：位操作置位
来源：http://rsm.52xcode.cn

x |= (1 << 3);
来源：http://efn.yuxming.cn

[S17] C：安全拼接字符串
来源：http://fux.yuanzhike.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kor.snrcjt.cn

[S18] C：命令行参数
来源：http://haq.nanxinkj.top

int main(int argc, char **argv)
来源：http://uvi.hammf.cn

[S19] C：快速排序
来源：http://bfo.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://ypk.yj202588.top

[S20] C：二分查找
来源：http://ydy.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dms.ehwqpu.com

[S21] C：字符类别判断
来源：http://fzr.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xjq.sweek.top

[S22] C：字符串转数字
来源：http://xdd.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yjd.fehbvm.com

[S23] C：随机数
来源：http://jwz.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://foz.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://tov.gogol.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tds.zdqjudy.top

[S25] C：内存拷贝
来源：http://tkr.vqdsnc.cn

memcpy(dst, src, n);
来源：http://xfe.quarkkingdee.top

[S26] C：内存清零
来源：http://arv.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://qdf.dashuyun.cn

[S27] C：定义常量
来源：http://psi.wangdashe.top

const double PI = 3.14159;
来源：http://osn.aizwys.cn

[S28] C：静态变量
来源：http://hzd.nanxinkj.top

static int counter = 0;
来源：http://khq.hammf.cn

[S29] C：变参函数
来源：http://fpu.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://epc.meibo888.top

[S30] C：头文件保护
来源：http://jqr.guannengcc.top

#ifndef X_H
来源：http://kjt.tanke756.top

#define X_H
来源：http://cwo.daria6918.cn

#endif
来源：http://mgr.aizwys.cn

[S31] C++：Hello World
来源：http://lrx.yuanzhike.top

#include <iostream>
来源：http://yei.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://vgx.0kj1m.cn

[S32] C++：字符串
来源：http://fba.zhaomingkeji.xyz

std::string s = "hi";  s += "!";
来源：http://vks.fktsv.cn

[S33] C++：vector 增删
来源：http://uet.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jvd.gzhubu.top

[S34] C++：遍历 vector
来源：http://hej.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://ieo.shangyingyoupin.top

[S35] C++：map
来源：http://hsp.zdbjq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://upf.c1oappe.top

[S36] C++：unordered_map
来源：http://vcm.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://woh.yonumen.top

[S37] C++：set
来源：http://nph.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mtd.kuanghao11.cn

[S38] C++：排序
来源：http://iqs.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://vqp.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://cnd.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uls.andypj.xyz

[S40] C++：查找元素
来源：http://qey.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bwp.xingfuxueyuan.xyz

[S41] C++：类与构造函数
来源：http://djg.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hma.hnqzz.top

[S42] C++：继承与虚函数
来源：http://ial.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://scu.haohaochexian.top

[S43] C++：智能指针
来源：http://cux.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://xjc.sysykeji.top

[S44] C++：引用传参
来源：http://cme.sxryk.cn

void inc(int &x) { ++x; }
来源：http://tvz.fanxiaobao.xyz

[S45] C++：lambda
来源：http://uem.nanxinkj.top

auto add = [](int a, int b) { return a + b; };
来源：http://yvj.fzhhl.top

[S46] C++：函数模板
来源：http://wcb.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ncz.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://skm.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://axl.hcnkem.com

[S48] C++：逐行读文件
来源：http://ayi.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://jdq.gotoacloud.top

while (std::getline(in, line)) { }
来源：http://cwc.gzhubu.top

[S49] C++：写文件
来源：http://qns.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qgu.yueranfly.top

[S50] C++：格式化数字
来源：http://cvg.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://teb.cashguo.top

[S51] C++：显式类型转换
来源：http://ayu.tanke756.top

static_cast<double>(a) / b
来源：http://jvd.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://pwg.meibo888.top

int size() const noexcept { return n_; }
来源：http://igj.c1oappe.top

[S53] C++：移动语义
来源：http://vna.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://jyp.sweek.top

[S54] C++：异常处理
来源：http://hxm.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bkn.0kj1m.cn

[S55] C++：结构化绑定
来源：http://wrv.daxiang520.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lnl.sufxvd.cn

[S56] C++：optional
来源：http://cmx.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zjf.hfpthk.cn

[S57] C++：编译期常量
来源：http://stq.gzhubu.top

constexpr int N = 10;
来源：http://ccf.jiagoushi.top

[S58] C++：命名空间
来源：http://tru.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://jky.fengsongda.top

[S59] C++：静态断言
来源：http://afo.jiagoushi.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cwg.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://tmt.zhoulong.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hxl.zhongyouzk.top

================================================================================
来源：http://sid.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lzi.316326.xyz

================================================================================
来源：http://aqv.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://kky.guowangkeji.top

println("Hello")
来源：http://xtl.uphjek.com

[T02] Kotlin：变量
来源：http://zoh.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kpv.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://klw.guannengcc.top

"值: $b"
来源：http://auk.shanyushiyangtech.top

[T04] Kotlin：空安全
来源：http://hqe.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://rwl.jinqigufen.top

[T05] Kotlin：when 表达式
来源：http://iba.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://suw.daxiang520.top

[T06] Kotlin：集合映射
来源：http://oaf.birdmap.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hpw.dianchejie.cn

[T07] Kotlin：集合过滤
来源：http://mzt.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lxu.zycfv.cn

[T08] Kotlin：数据类
来源：http://dqq.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://xtx.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://wun.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://juy.smart0.xyz

[T10] Kotlin：默认参数
来源：http://ujr.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cvw.tarul.cn

[T11] Kotlin：协程
来源：http://yoq.zhengqikj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://odb.xuanzx.com

[T12] Kotlin：解构声明
来源：http://nwo.yuxming.cn

val (a, b) = Pair(1, 2)
来源：http://gqb.vehdjk.com

[T13] Kotlin：只读 Map
来源：http://vcw.sxryk.cn

val m = mapOf("a" to 1)
来源：http://geh.ehwqpu.com

[T14] Kotlin：循环
来源：http://mqq.yuxming.cn

for (i in 1..10) println(i)
来源：http://wio.daria6918.cn

[T15] Kotlin：接口
来源：http://nse.hongshengwenyu.top

interface Shape { fun area(): Double }
来源：http://dio.sxryk.cn

[T16] Swift：Hello World
来源：http://dfx.zycfv.cn

print("Hello")
来源：http://wwm.gzhubu.top


<!-- 参考信息 -->