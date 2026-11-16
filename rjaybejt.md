代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://guu.cheryme.top

[R14] C 风格 for
来源：http://zia.pycfn.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yvc.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://dir.yueranfly.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xrg.ctjpmb.com

[R16] until 等待条件
来源：http://dvd.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qkj.haohaochexian.top

[R17] 数组定义与取值
来源：http://uof.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://fyf.chenjidiqi.icu

[R18] 遍历数组
来源：http://wxw.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ssk.ppjwa.cn

[R19] 数组长度
来源：http://smc.fengsongda.top

echo "${#arr[@]}"
来源：http://imc.xziqi.cn

[R20] 关联数组（字典）
来源：http://qyg.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ebg.quarkkingdee.top

[R21] 字符串长度
来源：http://zxi.xylfe.cn

echo "${#s}"
来源：http://tnq.yongpay.top

[R22] 截取子串
来源：http://sas.redwolf501.top

echo "${s:0:5}"
来源：http://ydk.fehbvm.com

[R23] 字符串替换
来源：http://qsd.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lot.shanyushiyangtech.top

[R24] 大小写转换
来源：http://bsf.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uic.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://iwq.redwolf501.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kjp.redwolf501.top

[R26] 命令替换
来源：http://paj.aibaodan.cn

now=$(date +%F); echo "$now"
来源：http://icf.ydjk.org.cn

[R27] 算术展开
来源：http://djm.yj202588.top

echo $((1 + 2 * 3))
来源：http://veq.hysaishi.cn

[R28] 浮点运算
来源：http://tvz.jlsjyb.cn

echo "scale=2; 10/3" | bc
来源：http://kbf.gogol.net.cn

[R29] 定义函数
来源：http://nfl.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tii.hammf.cn

[R30] 函数返回状态码
来源：http://qgd.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://hzv.zhaomingkeji.xyz

[R31] 局部变量
来源：http://nng.zhixingplan.top

f() { local x=1; echo "$x"; }
来源：http://otz.ppjwa.cn

[R32] 参数个数校验
来源：http://rib.sjlbkw.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qpn.ctjpmb.com

[R33] 捕获错误并提示行号
来源：http://xkn.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wvk.wangshuangyany.cn

[R34] 退出时清理
来源：http://cvr.gotoacloud.top

trap 'rm -f "$tmp"' EXIT
来源：http://voa.smart0.xyz

[R35] 后台执行并等待
来源：http://ygl.ivvv.top

sleep 5 & pid=$!; wait "$pid"
来源：http://shm.hfpthk.cn

[R36] 并发执行多个任务
来源：http://guc.chenlongwang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://avc.hysaishi.cn

[R37] 把输出赋给变量
来源：http://bji.nanxinkj.top

files=$(ls -1)
来源：http://nzu.uphjek.com

[R38] 管道串联
来源：http://aoc.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://vqz.nanxuanxn.top

[R39] 重定向标准输出与错误
来源：http://tle.aibaodan.cn

cmd > out.log 2>&1
来源：http://lge.jqgufenzy.top

[R40] 追加写日志
来源：http://dzc.shangyingyoupin.top

echo "log" >> out.log
来源：http://zno.0kj1m.cn

[R41] 丢弃输出
来源：http://rbh.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://txu.zhengqikj.top

[R42] 输入重定向
来源：http://fph.hnqzz.top

wc -l < a.txt
来源：http://cqm.jinqigufen.top

[R43] 按名字查找文件
来源：http://hpp.shanyushiyangtech.top

find . -name "*.log" -type f
来源：http://vll.cqqwz.cn

[R44] 按修改时间查找
来源：http://dbu.hammf.cn

find . -mtime -7 -type f
来源：http://zdv.9152youxi.cn

[R45] 批量删除
来源：http://nam.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://tsk.bbcook.cn

[R46] 递归替换文件内容
来源：http://dle.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ipw.zdbjq.cn

[R47] sed 单行替换
来源：http://dth.vehdjk.com

sed -i 's/foo/bar/g' a.txt
来源：http://uuy.mhx1999.top

[R48] awk 取指定列
来源：http://azc.jinyuanbaomall.cn

awk '{print $1, $3}' a.txt
来源：http://cja.andypj.xyz

[R49] awk 带条件
来源：http://hsr.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iri.bjfxy.top

[R50] awk 求和
来源：http://bmg.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://pmr.gogol.net.cn

[R51] 排序去重取前几
来源：http://wwr.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wgj.bjfxy.top

[R52] 统计行数
来源：http://yzy.gaohongyu789.top

wc -l a.txt
来源：http://wkf.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://clr.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zfn.zhoulong.xyz

[R54] 比较两个文件
来源：http://dbm.yj20258.top

diff a.txt b.txt
来源：http://uxu.bjfxy.top

[R55] 压缩与解压
来源：http://ety.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://myj.nwbrower.top

[R56] 远程拷贝
来源：http://hsr.fengsongda.top

scp file user@host:/path/
来源：http://cjk.havefunace.top

[R57] 远程执行命令
来源：http://sbu.aizwys.cn

ssh user@host 'uptime'
来源：http://kjx.ydzc1.top

[R58] 下载文件
来源：http://sez.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rsu.c1oappe.top

[R59] 发 POST JSON
来源：http://qxy.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://whx.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://fsj.zhaomingkeji.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ghk.cdnleiting.top

[R61] 磁盘占用
来源：http://dbr.zhengqikj.top

df -h;  du -sh *
来源：http://dhn.cashguo.top

[R62] 找最占空间的文件
来源：http://sxc.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://lyo.aizwys.cn

[R63] 内存与进程
来源：http://rid.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://ken.guannengcc.top

[R64] 结束进程
来源：http://ymj.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://xbm.pengpengdd.cyou

[R65] 查看端口占用
来源：http://twd.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kvx.yj20258.top

[R66] 定时任务
来源：http://ott.fanxiaobao.xyz

crontab -e;  crontab -l
来源：http://ljd.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://xqe.jqgufenzy.top

openssl rand -hex 16
来源：http://hem.quarkkingdee.top

[R68] 计算文件校验值
来源：http://tkn.guannengcc.top

sha256sum a.txt;  md5sum a.txt
来源：http://yvn.mhx1999.top

[R69] 生成随机密码
来源：http://qbd.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://sqs.ywan-chungtsiang.top

[R70] 时间戳与互转
来源：http://fmd.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://dul.gaohongyu789.top

[R71] 日期格式化
来源：http://ocl.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rxp.zdqjudy.top

[R72] 等待端口就绪
来源：http://siv.zhoulong.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://xpq.hesvh.cn

[R73] 分割大日志
来源：http://dhn.cqqwz.cn

split -l 1000 big.log part_
来源：http://fxc.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://zcv.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bjn.nanxinkj.top

[R75] 导出环境变量
来源：http://bur.yuxming.cn

export PATH="$HOME/bin:$PATH"
来源：http://ije.hesvh.cn

[R76] 使用临时文件
来源：http://eky.svipenyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://utd.xylfe.cn

[R77] 读取用户输入
来源：http://myp.316326.xyz

read -rp "请输入: " ans
来源：http://mun.snrcjt.cn

[R78] 交互式菜单
来源：http://omk.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://ygw.ivvv.top

[R79] 解析命令行选项
来源：http://syt.yfazqb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uuk.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://ivm.jqgufenzy.top

time ./run.sh
来源：http://xra.havefunace.top

================================================================================
来源：http://myj.iojbl.cn

S. C / C++ 专题
来源：http://wwu.pengpengdd.cyou

================================================================================
来源：http://bdb.wangdashe.top

[S01] C：Hello World
来源：http://wvn.xuanzx.com

#include <stdio.h>
来源：http://kus.chenzaomai.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://nvr.redwolf501.top

[S02] C：变量与格式化输出
来源：http://swe.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://rnd.wangdashe.top

[S03] C：读入整数
来源：http://wlc.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://wab.yuanzhike.top

[S04] C：字符串复制
来源：http://iip.jqgufenzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://iin.zycfv.cn

[S05] C：字符串长度
来源：http://iva.quarkkingdee.top

strlen(s)
来源：http://kve.guannengcc.top

[S06] C：字符串比较
来源：http://qsi.quarkkingdee.top

strcmp(a, b) == 0
来源：http://ptq.sxryk.cn

[S07] C：数组遍历求和
来源：http://tla.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mbl.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://pzs.hfpthk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jxv.hesvh.cn

[S09] C：结构体定义与初始化
来源：http://sva.pycfn.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oty.9152youxi.cn

[S10] C：指针与解引用
来源：http://uku.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://imj.redwolf501.top

[S11] C：逐行读文件
来源：http://jrj.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://fqf.jianghu66.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bze.xinyue.icu

fclose(f);
来源：http://ykj.aibaodan.cn

[S12] C：写文件
来源：http://fux.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jua.yueranfly.top

[S13] C：宏定义
来源：http://xfl.bjfxy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lcn.fzhhl.top

[S14] C：枚举
来源：http://txk.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://pnm.nanxinkj.top

[S15] C：类型转换
来源：http://sxn.smart0.xyz

(double) a / b
来源：http://psb.jianghu66.top

[S16] C：位操作置位
来源：http://eeo.meibo888.top

x |= (1 << 3);
来源：http://jop.sweek.top

[S17] C：安全拼接字符串
来源：http://koo.jqgufenzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://acf.andypj.xyz

[S18] C：命令行参数
来源：http://xru.daxiang520.top

int main(int argc, char **argv)
来源：http://xik.yanxiufei.cn

[S19] C：快速排序
来源：http://zdt.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://xdq.sysykeji.top

[S20] C：二分查找
来源：http://rpp.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vfu.yueranfly.top

[S21] C：字符类别判断
来源：http://enz.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://drq.wangdashe.top

[S22] C：字符串转数字
来源：http://bju.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://wfk.ivvv.top

[S23] C：随机数
来源：http://ggh.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wbl.daria6918.cn

[S24] C：获取本地时间
来源：http://gnf.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://irz.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://ziw.tianlin.xyz

memcpy(dst, src, n);
来源：http://ccp.guannengcc.top

[S26] C：内存清零
来源：http://ntb.yj20258888.top

memset(a, 0, sizeof a);
来源：http://vqo.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://nkl.0kj1m.cn

const double PI = 3.14159;
来源：http://lxr.meibo888.top

[S28] C：静态变量
来源：http://ylo.ywan-chungtsiang.top

static int counter = 0;
来源：http://cfi.xinyue.icu

[S29] C：变参函数
来源：http://svl.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kcr.jinqigfzy.top

[S30] C：头文件保护
来源：http://luj.hnqzz.top

#ifndef X_H
来源：http://tho.snrcjt.cn

#define X_H
来源：http://zgc.bbcook.cn

#endif
来源：http://pkd.hnxiangtu.top

[S31] C++：Hello World
来源：http://ghs.shangyingyoupin.top

#include <iostream>
来源：http://fbm.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://dgj.sjlbkw.cn

[S32] C++：字符串
来源：http://qab.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://oww.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://dky.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qup.jqgfzy.top

[S34] C++：遍历 vector
来源：http://cqx.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://uuk.gzhubu.top

[S35] C++：map
来源：http://irn.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dbr.cucudq.cn

[S36] C++：unordered_map
来源：http://vfo.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rty.iojbl.cn

[S37] C++：set
来源：http://owg.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rog.mhx1999.top

[S38] C++：排序
来源：http://loh.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://tnd.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://ofm.fehbvm.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hqt.zhiwuduotai.top

[S40] C++：查找元素
来源：http://amh.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dku.wangshuangyany.cn

[S41] C++：类与构造函数
来源：http://sso.yanxiufei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mrw.ivvv.top

[S42] C++：继承与虚函数
来源：http://lal.yfazqb.com

class B : public Base { public: void f() override {} };
来源：http://ajj.zhiwuduotai.top

[S43] C++：智能指针
来源：http://sjj.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://kor.aibaodan.cn

[S44] C++：引用传参
来源：http://yhx.dashuyun.cn

void inc(int &x) { ++x; }
来源：http://fje.bjfxy.top

[S45] C++：lambda
来源：http://aez.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pfq.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://qhl.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xyu.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://wun.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hsp.bbcook.cn

[S48] C++：逐行读文件
来源：http://cuz.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://olg.cheryme.top

while (std::getline(in, line)) { }
来源：http://uwk.zhijiandao.cn

[S49] C++：写文件
来源：http://tuk.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xmg.ivvv.top

[S50] C++：格式化数字
来源：http://zqn.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yfs.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://lxm.ehwqpu.com

static_cast<double>(a) / b
来源：http://rlb.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://kjx.aizwys.cn

int size() const noexcept { return n_; }
来源：http://mdu.zhoulong.xyz

[S53] C++：移动语义
来源：http://jfr.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://abc.pycfn.com

[S54] C++：异常处理
来源：http://fky.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qmm.tian-w.cn

[S55] C++：结构化绑定
来源：http://bvb.jianghu66.top

auto [a, b] = std::make_pair(1, 2);
来源：http://oyb.zhongyouzk.top

[S56] C++：optional
来源：http://lkv.jiagoushi.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vrq.chenlongwang.top

[S57] C++：编译期常量
来源：http://lwt.daxiang520.top

constexpr int N = 10;
来源：http://mcj.nanxinkj.top

[S58] C++：命名空间
来源：http://vfn.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://zvp.jqgufenzy.top

[S59] C++：静态断言
来源：http://ilu.quarkkingdee.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://niw.hywenlv.cn

[S60] C++：遍历并删除元素
来源：http://hgk.smart0.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mdc.jyoumei.cn

================================================================================
来源：http://wxd.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://riw.uphjek.com

================================================================================
来源：http://ajx.epnwcf.com

[T01] Kotlin：Hello World
来源：http://yux.ywan-chungtsiang.top

println("Hello")
来源：http://sar.zhoulong.xyz

[T02] Kotlin：变量
来源：http://lfo.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jjz.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://nau.epnwcf.com

"值: $b"
来源：http://dqf.ehwqpu.com

[T04] Kotlin：空安全
来源：http://znn.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://cyu.cheryme.top

[T05] Kotlin：when 表达式
来源：http://unm.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oww.aizwys.cn

[T06] Kotlin：集合映射
来源：http://tbq.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ntz.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://jhr.jqgufenzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tso.daria6918.cn

[T08] Kotlin：数据类
来源：http://chl.vehdjk.com

data class User(val name: String, val age: Int)
来源：http://sea.havefunace.top

[T09] Kotlin：扩展函数
来源：http://ggv.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://hle.zhixingplan.top

[T10] Kotlin：默认参数
来源：http://ycr.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wsg.epnwcf.com

[T11] Kotlin：协程
来源：http://ink.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gck.yongpay.top

[T12] Kotlin：解构声明
来源：http://zkr.jlsjyb.cn

val (a, b) = Pair(1, 2)
来源：http://lih.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://nix.fktsv.cn

val m = mapOf("a" to 1)
来源：http://rjn.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://zjk.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://htn.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://dgt.mhx1999.top

interface Shape { fun area(): Double }
来源：http://ytd.chenjidiqi.icu

[T16] Swift：Hello World
来源：http://thl.fehbvm.com

print("Hello")
来源：http://zqt.zhaomingkeji.xyz


<!-- 参考信息 -->