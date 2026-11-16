代发 wailian999

case "$1" in
来源：http://swa.ydjk.org.cn

start) echo "启动" ;;
来源：http://qqs.hywenlv.cn

stop)  echo "停止" ;;
来源：http://vca.sxryk.cn

*)     echo "未知命令" ;;
来源：http://djk.yongpay.top

esac
来源：http://mux.yj20258.top

[R12] for 遍历文件
来源：http://pha.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://iop.yj202588.top

[R13] for 计数循环
来源：http://bif.nwbrower.top

for i in {1..10}; do echo "$i"; done
来源：http://dje.xziqi.cn

[R14] C 风格 for
来源：http://ols.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uod.hywenlv.cn

[R15] while 逐行读文件
来源：http://cfh.fengsongda.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tur.kuanghao11.cn

[R16] until 等待条件
来源：http://kax.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kmn.svipenyu.cn

[R17] 数组定义与取值
来源：http://ore.hywenlv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rvs.tian-w.cn

[R18] 遍历数组
来源：http://hsg.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vao.guannengcc.top

[R19] 数组长度
来源：http://nfi.iojbl.cn

echo "${#arr[@]}"
来源：http://dal.hongshengwenyu.top

[R20] 关联数组（字典）
来源：http://lrl.ybcxt.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rcb.tianlin.xyz

[R21] 字符串长度
来源：http://ihw.0kj1m.cn

echo "${#s}"
来源：http://ywz.9152youxi.cn

[R22] 截取子串
来源：http://fwa.daria6918.cn

echo "${s:0:5}"
来源：http://jbj.fengsongda.top

[R23] 字符串替换
来源：http://vrf.shzxlz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zjm.yuanzhike.top

[R24] 大小写转换
来源：http://ygy.sysykeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://dec.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://sxe.daria6918.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pyz.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://mit.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://jpt.yongpay.top

[R27] 算术展开
来源：http://bfa.yj202588.top

echo $((1 + 2 * 3))
来源：http://iwl.jqgfzy.top

[R28] 浮点运算
来源：http://xzf.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://ghe.nanxinkj.top

[R29] 定义函数
来源：http://lvx.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ivm.havefunace.top

[R30] 函数返回状态码
来源：http://rwb.gogol.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://qov.hammf.cn

[R31] 局部变量
来源：http://ete.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://vdf.tianlin.xyz

[R32] 参数个数校验
来源：http://mqs.jqgfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ocx.ywan-chungtsiang.top

[R33] 捕获错误并提示行号
来源：http://zyw.svipenyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iae.daria6918.cn

[R34] 退出时清理
来源：http://whj.vehdjk.com

trap 'rm -f "$tmp"' EXIT
来源：http://qqh.c1oappe.top

[R35] 后台执行并等待
来源：http://ugc.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vmk.yueranfly.top

[R36] 并发执行多个任务
来源：http://ipm.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://obt.tian-w.cn

[R37] 把输出赋给变量
来源：http://uqb.shuidangran.top

files=$(ls -1)
来源：http://ris.daxiang520.top

[R38] 管道串联
来源：http://gms.jinghuilouyu.cn

cat a.txt | grep -i error | wc -l
来源：http://lra.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://opp.sweek.top

cmd > out.log 2>&1
来源：http://erv.jinqigufen.top

[R40] 追加写日志
来源：http://nhi.jqgfzy.top

echo "log" >> out.log
来源：http://bdp.xinyue.icu

[R41] 丢弃输出
来源：http://tjm.zhaomingkeji.xyz

cmd >/dev/null 2>&1
来源：http://end.xziqi.cn

[R42] 输入重定向
来源：http://ouo.shanyushiyangkeji.top

wc -l < a.txt
来源：http://sri.xylfe.cn

[R43] 按名字查找文件
来源：http://kiq.ydzc1.top

find . -name "*.log" -type f
来源：http://yld.meibo888.top

[R44] 按修改时间查找
来源：http://arb.ywan-chungtsiang.top

find . -mtime -7 -type f
来源：http://hqw.yvedp.cn

[R45] 批量删除
来源：http://nof.tianlin.xyz

find . -name "*.tmp" -delete
来源：http://fwg.fzhhl.top

[R46] 递归替换文件内容
来源：http://vgj.ybcxt.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cye.gogol.net.cn

[R47] sed 单行替换
来源：http://vqc.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://oti.mhx1999.top

[R48] awk 取指定列
来源：http://ykv.cqqwz.cn

awk '{print $1, $3}' a.txt
来源：http://qus.jqgufenzy.top

[R49] awk 带条件
来源：http://vyk.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fpl.shanyushiyangtech.top

[R50] awk 求和
来源：http://goq.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fzf.jyoumei.cn

[R51] 排序去重取前几
来源：http://lqx.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oxx.zdbjq.cn

[R52] 统计行数
来源：http://wzp.sysykeji.top

wc -l a.txt
来源：http://hxo.cashguo.top

[R53] 查看文件头与实时尾
来源：http://uje.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cam.hfpthk.cn

[R54] 比较两个文件
来源：http://scz.ydjk.org.cn

diff a.txt b.txt
来源：http://pgg.sufxvd.cn

[R55] 压缩与解压
来源：http://rpi.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vsf.dashuyun.cn

[R56] 远程拷贝
来源：http://ost.smart0.xyz

scp file user@host:/path/
来源：http://wpr.ybcxt.top

[R57] 远程执行命令
来源：http://jkl.meibo888.top

ssh user@host 'uptime'
来源：http://roe.jinghuilouyu.cn

[R58] 下载文件
来源：http://jwk.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://prb.meibo888.top

[R59] 发 POST JSON
来源：http://apt.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://afe.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://tkb.wangdashe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hyy.daxiang520.top

[R61] 磁盘占用
来源：http://jze.cheryme.top

df -h;  du -sh *
来源：http://ibs.ivvv.top

[R62] 找最占空间的文件
来源：http://eml.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://uvc.jiagoushi.top

[R63] 内存与进程
来源：http://taa.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://nlc.chenjidiqi.icu

[R64] 结束进程
来源：http://qnj.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://nis.yj202588.top

[R65] 查看端口占用
来源：http://xub.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://otj.feifeiyinyue.top

[R66] 定时任务
来源：http://scp.daria6918.cn

crontab -e;  crontab -l
来源：http://dkf.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://kwd.kuanghao11.cn

openssl rand -hex 16
来源：http://vty.wangshuangyany.cn

[R68] 计算文件校验值
来源：http://ppp.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://jet.redwolf501.top

[R69] 生成随机密码
来源：http://ssh.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://hpk.pycfn.com

[R70] 时间戳与互转
来源：http://ezr.nwbrower.top

date +%s;  date -d @1700000000
来源：http://eyt.zdbjq.cn

[R71] 日期格式化
来源：http://qiw.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://vwy.zhoulong.xyz

[R72] 等待端口就绪
来源：http://sxc.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://von.guannengcc.top

[R73] 分割大日志
来源：http://qzt.guannengcc.top

split -l 1000 big.log part_
来源：http://mid.gotoacloud.top

[R74] 批量重命名
来源：http://awd.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uny.fzhhl.top

[R75] 导出环境变量
来源：http://xho.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://ydj.dianchejie.cn

[R76] 使用临时文件
来源：http://vct.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xhz.tanke756.top

[R77] 读取用户输入
来源：http://xyh.tianlin.xyz

read -rp "请输入: " ans
来源：http://veh.yj202588.top

[R78] 交互式菜单
来源：http://czk.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yxs.zhongyouzk.top

[R79] 解析命令行选项
来源：http://puf.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://azo.zhijiandao.cn

[R80] 查看脚本执行耗时
来源：http://jia.jyoumei.cn

time ./run.sh
来源：http://umf.jianghu66.top

================================================================================
来源：http://beu.shuidangran.top

S. C / C++ 专题
来源：http://kri.daxiang520.top

================================================================================
来源：http://ydh.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://qyu.hfpthk.cn

#include <stdio.h>
来源：http://nig.kuanghao11.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ynq.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://dkv.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://zah.zdqjudy.top

[S03] C：读入整数
来源：http://ydw.meibo888.top

int x; scanf("%d", &x);
来源：http://dze.andypj.xyz

[S04] C：字符串复制
来源：http://pzt.yj20258888.top

char dst[32]; strcpy(dst, "hi");
来源：http://drs.gotoacloud.top

[S05] C：字符串长度
来源：http://zkz.tanke756.top

strlen(s)
来源：http://dzx.fktsv.cn

[S06] C：字符串比较
来源：http://rer.zdbjq.cn

strcmp(a, b) == 0
来源：http://maa.xziqi.cn

[S07] C：数组遍历求和
来源：http://hys.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://has.yj20258.top

[S08] C：动态内存分配与释放
来源：http://mvf.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zig.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://bov.nanxuanxn.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ibz.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://vhv.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://njt.tian-w.cn

[S11] C：逐行读文件
来源：http://umw.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://oss.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://meh.hfpthk.cn

fclose(f);
来源：http://bjr.ppjwa.cn

[S12] C：写文件
来源：http://zph.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vsi.sweek.top

[S13] C：宏定义
来源：http://lne.gaohongyu789.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cli.pengpengdd.cyou

[S14] C：枚举
来源：http://hfo.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://oom.ybcxt.top

[S15] C：类型转换
来源：http://sum.gzhubu.top

(double) a / b
来源：http://ugt.52xcode.cn

[S16] C：位操作置位
来源：http://mbd.hesvh.cn

x |= (1 << 3);
来源：http://mau.shzxlz.cn

[S17] C：安全拼接字符串
来源：http://lmy.chenzaomai.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://thb.zdbjq.cn

[S18] C：命令行参数
来源：http://ibx.zhongyouzk.top

int main(int argc, char **argv)
来源：http://jib.dianchejie.cn

[S19] C：快速排序
来源：http://fnf.nanxinkj.top

qsort(a, n, sizeof(int), cmp);
来源：http://ocb.jinghuilouyu.cn

[S20] C：二分查找
来源：http://qba.yj20258888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://riq.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://vra.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iqx.hcnkem.com

[S22] C：字符串转数字
来源：http://gnk.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://ytk.shuidangran.top

[S23] C：随机数
来源：http://ntp.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ivp.jqgufenzy.top

[S24] C：获取本地时间
来源：http://brk.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tnp.chenlongwang.top

[S25] C：内存拷贝
来源：http://qlw.fktsv.cn

memcpy(dst, src, n);
来源：http://yna.ybcxt.top

[S26] C：内存清零
来源：http://zid.0kj1m.cn

memset(a, 0, sizeof a);
来源：http://wih.cdnleiting.top

[S27] C：定义常量
来源：http://vrh.yongpay.top

const double PI = 3.14159;
来源：http://uwg.ivvv.top

[S28] C：静态变量
来源：http://qqa.ctjpmb.com

static int counter = 0;
来源：http://qih.ivvv.top

[S29] C：变参函数
来源：http://uvq.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://laf.aizwys.cn

[S30] C：头文件保护
来源：http://eqm.redwolf501.top

#ifndef X_H
来源：http://vmk.hesvh.cn

#define X_H
来源：http://unt.shzxlz.cn

#endif
来源：http://qjw.gotoacloud.top

[S31] C++：Hello World
来源：http://ulf.jinyuanbaomall.cn

#include <iostream>
来源：http://pvd.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://vkb.feifeiyinyue.top

[S32] C++：字符串
来源：http://qgx.ivvv.top

std::string s = "hi";  s += "!";
来源：http://gox.shuidangran.top

[S33] C++：vector 增删
来源：http://xsz.gogol.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mlk.guannengcc.top

[S34] C++：遍历 vector
来源：http://kos.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://mae.jyoumei.cn

[S35] C++：map
来源：http://iuq.yonumen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mlu.vehdjk.com

[S36] C++：unordered_map
来源：http://fro.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://skj.yj202588.top

[S37] C++：set
来源：http://vsg.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ase.fktsv.cn

[S38] C++：排序
来源：http://hue.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://tjk.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://ynu.hammf.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ohp.birdmap.top

[S40] C++：查找元素
来源：http://rjd.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iah.yongpay.top

[S41] C++：类与构造函数
来源：http://ixs.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hok.bjfxy.top

[S42] C++：继承与虚函数
来源：http://kxv.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://sgj.gzhubu.top

[S43] C++：智能指针
来源：http://pyh.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://epz.andypj.xyz

[S44] C++：引用传参
来源：http://qle.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://tst.kuanghao11.cn

[S45] C++：lambda
来源：http://hyv.yuxming.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kzn.epnwcf.com

[S46] C++：函数模板
来源：http://sma.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://moo.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://xoc.yj202588.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dyr.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://ydj.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gcr.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://dvi.nwbrower.top

[S49] C++：写文件
来源：http://zzd.aizwys.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bqd.hnxiangtu.top

[S50] C++：格式化数字
来源：http://bbu.316326.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mgw.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://vsd.cqqwz.cn

static_cast<double>(a) / b
来源：http://qxv.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://izz.yuxming.cn

int size() const noexcept { return n_; }
来源：http://mwx.cheryme.top

[S53] C++：移动语义
来源：http://fsh.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://pcy.xylfe.cn

[S54] C++：异常处理
来源：http://ahu.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dgr.9152youxi.cn

[S55] C++：结构化绑定
来源：http://qtd.ppjwa.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ybm.yangfankeji.com

[S56] C++：optional
来源：http://myd.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nao.hesvh.cn

[S57] C++：编译期常量
来源：http://pwa.cheryme.top

constexpr int N = 10;
来源：http://ohr.hywenlv.cn

[S58] C++：命名空间
来源：http://gsk.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://riv.yj20258.top

[S59] C++：静态断言
来源：http://ayu.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pfe.haohaochexian.top

[S60] C++：遍历并删除元素
来源：http://yik.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://muy.fzhhl.top

================================================================================
来源：http://gjc.hnqzz.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://alv.fengsongda.top

================================================================================
来源：http://gmo.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://vbe.gogol.net.cn

println("Hello")
来源：http://pko.zhaomingkeji.xyz

[T02] Kotlin：变量
来源：http://bxm.zdqjudy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mil.bjfxy.top

[T03] Kotlin：字符串模板
来源：http://hwy.cashguo.top

"值: $b"
来源：http://vhp.mhx1999.top

[T04] Kotlin：空安全
来源：http://fhb.xuanzx.com

val n: String? = null;  n?.length
来源：http://sap.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://yhs.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://anm.ivvv.top

[T06] Kotlin：集合映射
来源：http://zrp.52xcode.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wqa.cheryme.top

[T07] Kotlin：集合过滤
来源：http://qns.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://tup.jyoumei.cn

[T08] Kotlin：数据类
来源：http://szc.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://qpi.gzhubu.top

[T09] Kotlin：扩展函数
来源：http://zqb.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://sad.52xcode.cn

[T10] Kotlin：默认参数
来源：http://dos.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yej.zhaomingkeji.xyz

[T11] Kotlin：协程
来源：http://rqn.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ijp.xziqi.cn

[T12] Kotlin：解构声明
来源：http://cxo.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://drf.jinqigufen.top


<!-- 参考信息 -->