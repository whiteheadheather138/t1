代发 wailian999

case "$1" in
来源：http://tsg.gotoacloud.top

start) echo "启动" ;;
来源：http://twu.xuanzx.com

stop)  echo "停止" ;;
来源：http://iyv.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://ref.snrcjt.cn

esac
来源：http://gxo.hnxiangtu.top

[R12] for 遍历文件
来源：http://wzi.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://ert.sufxvd.cn

[R13] for 计数循环
来源：http://vkc.cucudq.cn

for i in {1..10}; do echo "$i"; done
来源：http://ozn.pengpengdd.cyou

[R14] C 风格 for
来源：http://ipi.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nby.epnwcf.com

[R15] while 逐行读文件
来源：http://ycz.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xtc.gzhubu.top

[R16] until 等待条件
来源：http://vaz.ppjwa.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://orq.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://pdc.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://vjr.guannengcc.top

[R18] 遍历数组
来源：http://cvb.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://exs.daxiang520.top

[R19] 数组长度
来源：http://tiy.yvedp.cn

echo "${#arr[@]}"
来源：http://hbr.hnxiangtu.top

[R20] 关联数组（字典）
来源：http://fin.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wie.iojbl.cn

[R21] 字符串长度
来源：http://wbb.nanxuanxn.top

echo "${#s}"
来源：http://bfy.tian-w.cn

[R22] 截取子串
来源：http://feu.zhaomingkeji.xyz

echo "${s:0:5}"
来源：http://afl.xylfe.cn

[R23] 字符串替换
来源：http://cwo.shuidangran.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hlj.shuidangran.top

[R24] 大小写转换
来源：http://ihd.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://eat.yonumen.top

[R25] 去后缀 / 去前缀
来源：http://azc.nwbrower.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wka.daria6918.cn

[R26] 命令替换
来源：http://esc.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://can.epnwcf.com

[R27] 算术展开
来源：http://fja.ydjk.org.cn

echo $((1 + 2 * 3))
来源：http://ghb.zhoulong.xyz

[R28] 浮点运算
来源：http://qap.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://tum.gogol.net.cn

[R29] 定义函数
来源：http://ehz.tarul.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pxo.feifeiyinyue.top

[R30] 函数返回状态码
来源：http://trn.cqqwz.cn

f() { return 0; }; f || echo "失败了"
来源：http://nkz.pengpengdd.cyou

[R31] 局部变量
来源：http://ief.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://nlu.yuxming.cn

[R32] 参数个数校验
来源：http://lxo.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cno.xinyue.icu

[R33] 捕获错误并提示行号
来源：http://rau.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zsf.pengpengdd.cyou

[R34] 退出时清理
来源：http://jcz.jinqigfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://ybe.hfpthk.cn

[R35] 后台执行并等待
来源：http://dhd.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://iqg.hywenlv.cn

[R36] 并发执行多个任务
来源：http://vvb.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tip.zhixingplan.top

[R37] 把输出赋给变量
来源：http://etm.jqgfzy.top

files=$(ls -1)
来源：http://abw.52xcode.cn

[R38] 管道串联
来源：http://etu.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://gdz.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://wno.316326.xyz

cmd > out.log 2>&1
来源：http://wxp.yfazqb.com

[R40] 追加写日志
来源：http://bpl.xuetiantiany.cn

echo "log" >> out.log
来源：http://qho.jinghuilouyu.cn

[R41] 丢弃输出
来源：http://mkk.ppjwa.cn

cmd >/dev/null 2>&1
来源：http://yan.zdbjq.cn

[R42] 输入重定向
来源：http://doe.hnxiangtu.top

wc -l < a.txt
来源：http://ryw.yj202588.top

[R43] 按名字查找文件
来源：http://wgv.cashguo.top

find . -name "*.log" -type f
来源：http://fac.yj20258.top

[R44] 按修改时间查找
来源：http://jzh.uphjek.com

find . -mtime -7 -type f
来源：http://uet.xinyue.icu

[R45] 批量删除
来源：http://pxg.sxryk.cn

find . -name "*.tmp" -delete
来源：http://rpe.tianlin.xyz

[R46] 递归替换文件内容
来源：http://epa.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://anx.ctjpmb.com

[R47] sed 单行替换
来源：http://moy.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://iwu.pycfn.com

[R48] awk 取指定列
来源：http://whg.ybcxt.top

awk '{print $1, $3}' a.txt
来源：http://lxu.fehbvm.com

[R49] awk 带条件
来源：http://mbu.fehbvm.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nxw.xuetiantiany.cn

[R50] awk 求和
来源：http://dza.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://tgu.yj20258.top

[R51] 排序去重取前几
来源：http://eby.yonumen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ilk.smart0.xyz

[R52] 统计行数
来源：http://amc.cucudq.cn

wc -l a.txt
来源：http://uou.hesvh.cn

[R53] 查看文件头与实时尾
来源：http://xro.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://smv.xuanzx.com

[R54] 比较两个文件
来源：http://rro.9152youxi.cn

diff a.txt b.txt
来源：http://usx.snrcjt.cn

[R55] 压缩与解压
来源：http://cad.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oqu.gotoacloud.top

[R56] 远程拷贝
来源：http://ulz.yj202588.top

scp file user@host:/path/
来源：http://vdk.vqdsnc.cn

[R57] 远程执行命令
来源：http://cnp.316326.xyz

ssh user@host 'uptime'
来源：http://skl.vehdjk.com

[R58] 下载文件
来源：http://sop.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fhq.52xcode.cn

[R59] 发 POST JSON
来源：http://vrz.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://aij.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://vvm.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zjo.xuetiantiany.cn

[R61] 磁盘占用
来源：http://peg.sweek.top

df -h;  du -sh *
来源：http://ler.52xcode.cn

[R62] 找最占空间的文件
来源：http://zys.yonumen.top

du -ah . | sort -rh | head -10
来源：http://rhq.c1oappe.top

[R63] 内存与进程
来源：http://qaz.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://sxf.dashuyun.cn

[R64] 结束进程
来源：http://hsh.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://pfd.c1oappe.top

[R65] 查看端口占用
来源：http://osi.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fno.shzxlz.cn

[R66] 定时任务
来源：http://tes.yuanzhike.top

crontab -e;  crontab -l
来源：http://kau.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://ezg.gotoacloud.top

openssl rand -hex 16
来源：http://gnw.cdnleiting.top

[R68] 计算文件校验值
来源：http://uut.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://kjq.quarkkingdee.top

[R69] 生成随机密码
来源：http://qyl.zhixingplan.top

head -c 16 /dev/urandom | base64
来源：http://plc.jinqigfzy.top

[R70] 时间戳与互转
来源：http://ukp.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://yzw.hywenlv.cn

[R71] 日期格式化
来源：http://yob.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gyy.jyoumei.cn

[R72] 等待端口就绪
来源：http://bdg.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://jda.snrcjt.cn

[R73] 分割大日志
来源：http://rri.yfazqb.com

split -l 1000 big.log part_
来源：http://mbb.0kj1m.cn

[R74] 批量重命名
来源：http://hxm.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hag.yonumen.top

[R75] 导出环境变量
来源：http://pgk.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://nfa.zycfv.cn

[R76] 使用临时文件
来源：http://awe.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kgq.yuanzhike.top

[R77] 读取用户输入
来源：http://bjo.ydzc1.top

read -rp "请输入: " ans
来源：http://upq.fehbvm.com

[R78] 交互式菜单
来源：http://pgy.nwbrower.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hxp.iojbl.cn

[R79] 解析命令行选项
来源：http://qxg.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ves.yongpay.top

[R80] 查看脚本执行耗时
来源：http://bli.uphjek.com

time ./run.sh
来源：http://iiv.ppjwa.cn

================================================================================
来源：http://pxu.bbcook.cn

S. C / C++ 专题
来源：http://rnh.sxryk.cn

================================================================================
来源：http://zsz.mhx1999.top

[S01] C：Hello World
来源：http://qej.xinyue.icu

#include <stdio.h>
来源：http://rth.hnxiangtu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://aet.52xcode.cn

[S02] C：变量与格式化输出
来源：http://eqt.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://ibs.ydzc1.top

[S03] C：读入整数
来源：http://bxy.sweek.top

int x; scanf("%d", &x);
来源：http://yhi.xuanzx.com

[S04] C：字符串复制
来源：http://byw.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://dlb.yonumen.top

[S05] C：字符串长度
来源：http://ace.guowangkeji.top

strlen(s)
来源：http://gry.nwbrower.top

[S06] C：字符串比较
来源：http://fee.xziqi.cn

strcmp(a, b) == 0
来源：http://qlc.ivvv.top

[S07] C：数组遍历求和
来源：http://qlt.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fqc.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://ncn.52xcode.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vqw.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://ytl.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hmd.hnxiangtu.top

[S10] C：指针与解引用
来源：http://uyz.aizwys.cn

int *p = &a;  *p = 5;
来源：http://ukt.hnqzz.top

[S11] C：逐行读文件
来源：http://jqw.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://llk.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dww.yj20258888.top

fclose(f);
来源：http://lgr.sxryk.cn

[S12] C：写文件
来源：http://rhv.0kj1m.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vdu.kuanghao11.cn

[S13] C：宏定义
来源：http://lbv.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jsy.sjlbkw.cn

[S14] C：枚举
来源：http://cnr.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://joz.316326.xyz

[S15] C：类型转换
来源：http://ypi.shanyushiyangtech.top

(double) a / b
来源：http://hbe.quarkkingdee.top

[S16] C：位操作置位
来源：http://blk.jianghu66.top

x |= (1 << 3);
来源：http://smm.yongpay.top

[S17] C：安全拼接字符串
来源：http://urj.jinqigfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wmm.sxryk.cn

[S18] C：命令行参数
来源：http://xbv.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://czw.iojbl.cn

[S19] C：快速排序
来源：http://fjn.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://oii.zdqjudy.top

[S20] C：二分查找
来源：http://njk.jianghu66.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wpi.gotoacloud.top

[S21] C：字符类别判断
来源：http://nim.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dht.dashuyun.cn

[S22] C：字符串转数字
来源：http://ugi.hywenlv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sus.yj20258.top

[S23] C：随机数
来源：http://uly.hfpthk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hex.vqdsnc.cn

[S24] C：获取本地时间
来源：http://ttt.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fzh.shzxlz.cn

[S25] C：内存拷贝
来源：http://qup.haohaochexian.top

memcpy(dst, src, n);
来源：http://yjp.haohaochexian.top

[S26] C：内存清零
来源：http://jdc.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://amu.xingfuxueyuan.xyz

[S27] C：定义常量
来源：http://rty.ctjpmb.com

const double PI = 3.14159;
来源：http://bix.hfpthk.cn

[S28] C：静态变量
来源：http://yuo.shangyingyoupin.top

static int counter = 0;
来源：http://gyi.havefunace.top

[S29] C：变参函数
来源：http://mvd.jianghu66.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cuq.yonumen.top

[S30] C：头文件保护
来源：http://jps.mhx1999.top

#ifndef X_H
来源：http://qdj.316326.xyz

#define X_H
来源：http://qqb.jinqigfzy.top

#endif
来源：http://omk.hywenlv.cn

[S31] C++：Hello World
来源：http://trk.shanyushiyangkeji.top

#include <iostream>
来源：http://dnx.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://szz.ydjk.org.cn

[S32] C++：字符串
来源：http://dps.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://acp.jiagoushi.top

[S33] C++：vector 增删
来源：http://olb.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rtc.tianlin.xyz

[S34] C++：遍历 vector
来源：http://woc.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://iqf.gzhubu.top

[S35] C++：map
来源：http://rci.ivvv.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fbs.shanyushiyangkeji.top

[S36] C++：unordered_map
来源：http://mci.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lpt.zhongyouzk.top

[S37] C++：set
来源：http://zwb.pengpengdd.cyou

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jwf.zhijiandao.cn

[S38] C++：排序
来源：http://dzb.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://lgt.vqdsnc.cn

[S39] C++：自定义比较器排序
来源：http://jxz.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rvy.xuanzx.com

[S40] C++：查找元素
来源：http://ryt.yj20258888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bqs.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://oni.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xka.havefunace.top

[S42] C++：继承与虚函数
来源：http://ing.wangshuangyany.cn

class B : public Base { public: void f() override {} };
来源：http://toe.jlsjyb.cn

[S43] C++：智能指针
来源：http://pbx.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://mud.ctjpmb.com

[S44] C++：引用传参
来源：http://yxn.yvedp.cn

void inc(int &x) { ++x; }
来源：http://pup.hnqzz.top

[S45] C++：lambda
来源：http://lqe.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tnp.hysaishi.cn

[S46] C++：函数模板
来源：http://gtp.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bia.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://leu.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nhk.yangfankeji.com

[S48] C++：逐行读文件
来源：http://gkv.nwbrower.top

std::ifstream in("a.txt");  std::string line;
来源：http://isj.yfazqb.com

while (std::getline(in, line)) { }
来源：http://rwd.316326.xyz

[S49] C++：写文件
来源：http://qap.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ezw.zhongyouzk.top

[S50] C++：格式化数字
来源：http://mvq.snrcjt.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uhk.yuxming.cn

[S51] C++：显式类型转换
来源：http://rmu.gogol.net.cn

static_cast<double>(a) / b
来源：http://lbc.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://fpt.yj20258.top

int size() const noexcept { return n_; }
来源：http://ebx.wangdashe.top

[S53] C++：移动语义
来源：http://oqy.jqgfzy.top

std::vector<int> w = std::move(v);
来源：http://fwk.hongshengwenyu.top

[S54] C++：异常处理
来源：http://zun.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uxz.jianghu66.top

[S55] C++：结构化绑定
来源：http://xzq.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hid.c1oappe.top

[S56] C++：optional
来源：http://jzu.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xcq.zycfv.cn

[S57] C++：编译期常量
来源：http://ofj.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://lar.tarul.cn

[S58] C++：命名空间
来源：http://nxc.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://hdz.nwbrower.top

[S59] C++：静态断言
来源：http://kmt.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jaj.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://ryd.hnqzz.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ocr.gaohongyu789.top

================================================================================
来源：http://qcl.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yda.andypj.xyz

================================================================================
来源：http://fee.iojbl.cn

[T01] Kotlin：Hello World
来源：http://gdl.cucudq.cn

println("Hello")
来源：http://mid.sjlbkw.cn

[T02] Kotlin：变量
来源：http://zle.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ozm.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://vnj.yj20258.top

"值: $b"
来源：http://bov.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://uqt.jiagoushi.top

val n: String? = null;  n?.length
来源：http://mgi.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://scs.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lrp.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://itu.ybcxt.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rvj.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://htg.zhijiandao.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wqd.gotoacloud.top

[T08] Kotlin：数据类
来源：http://aha.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://obl.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://kre.nanxuanxn.top

fun String.exclaim() = this + "!"
来源：http://eqs.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://mlw.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bhb.sjlbkw.cn

[T11] Kotlin：协程
来源：http://ohq.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lki.chenjidiqi.icu

[T12] Kotlin：解构声明
来源：http://rvk.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://oul.9152youxi.cn


<!-- 参考信息 -->