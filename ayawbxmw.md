代发 wailian999

esac
来源：http://upp.shuidangran.top

[R12] for 遍历文件
来源：http://xne.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://wfa.yonumen.top

[R13] for 计数循环
来源：http://thm.zhaomingkeji.xyz

for i in {1..10}; do echo "$i"; done
来源：http://pkg.redwolf501.top

[R14] C 风格 for
来源：http://kyp.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lxo.xinyue.icu

[R15] while 逐行读文件
来源：http://hma.9152youxi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://awt.chenzaomai.com

[R16] until 等待条件
来源：http://dic.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wfx.52xcode.cn

[R17] 数组定义与取值
来源：http://jnu.dashuyun.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zej.sufxvd.cn

[R18] 遍历数组
来源：http://lqs.cheryme.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://die.tanke756.top

[R19] 数组长度
来源：http://qqp.aibaodan.cn

echo "${#arr[@]}"
来源：http://ttl.wangdashe.top

[R20] 关联数组（字典）
来源：http://mqt.daxiang520.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jhw.zhengqikj.top

[R21] 字符串长度
来源：http://xzb.yuxming.cn

echo "${#s}"
来源：http://smu.yj202588.top

[R22] 截取子串
来源：http://onn.zycfv.cn

echo "${s:0:5}"
来源：http://qwx.jyoumei.cn

[R23] 字符串替换
来源：http://nly.ctjpmb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nig.nanxinkj.top

[R24] 大小写转换
来源：http://hkq.hysaishi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ayc.kuanghao11.cn

[R25] 去后缀 / 去前缀
来源：http://onu.pycfn.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://kvi.ydzc1.top

[R26] 命令替换
来源：http://wmf.tarul.cn

now=$(date +%F); echo "$now"
来源：http://lwj.chenjidiqi.icu

[R27] 算术展开
来源：http://nlq.shzxlz.cn

echo $((1 + 2 * 3))
来源：http://tly.dashuyun.cn

[R28] 浮点运算
来源：http://hnf.cashguo.top

echo "scale=2; 10/3" | bc
来源：http://hyt.xingfuxueyuan.xyz

[R29] 定义函数
来源：http://url.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tlo.zhoulong.xyz

[R30] 函数返回状态码
来源：http://qoo.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://bjs.bbcook.cn

[R31] 局部变量
来源：http://wuo.shuidangran.top

f() { local x=1; echo "$x"; }
来源：http://eqg.hnxiangtu.top

[R32] 参数个数校验
来源：http://vws.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lfp.jinghuilouyu.cn

[R33] 捕获错误并提示行号
来源：http://tev.zycfv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ngu.ehwqpu.com

[R34] 退出时清理
来源：http://tpb.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://uku.epnwcf.com

[R35] 后台执行并等待
来源：http://tsx.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dgr.0kj1m.cn

[R36] 并发执行多个任务
来源：http://wwq.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pgb.jqgfzy.top

[R37] 把输出赋给变量
来源：http://fhi.ybcxt.top

files=$(ls -1)
来源：http://zyh.xinyue.icu

[R38] 管道串联
来源：http://xgf.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://fnt.xuetiantiany.cn

[R39] 重定向标准输出与错误
来源：http://vrq.zhixingplan.top

cmd > out.log 2>&1
来源：http://nhy.jqgufenzy.top

[R40] 追加写日志
来源：http://sye.aibaodan.cn

echo "log" >> out.log
来源：http://gbo.redwolf501.top

[R41] 丢弃输出
来源：http://mkp.andypj.xyz

cmd >/dev/null 2>&1
来源：http://daw.xuetiantiany.cn

[R42] 输入重定向
来源：http://otb.jianghu66.top

wc -l < a.txt
来源：http://mov.jqgfzy.top

[R43] 按名字查找文件
来源：http://lnz.wangdashe.top

find . -name "*.log" -type f
来源：http://wwq.gzhubu.top

[R44] 按修改时间查找
来源：http://dvb.316326.xyz

find . -mtime -7 -type f
来源：http://kwe.sweek.top

[R45] 批量删除
来源：http://fwk.hysaishi.cn

find . -name "*.tmp" -delete
来源：http://viy.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://hbt.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hrz.yj20258888.top

[R47] sed 单行替换
来源：http://zhg.ctjpmb.com

sed -i 's/foo/bar/g' a.txt
来源：http://cya.yuanzhike.top

[R48] awk 取指定列
来源：http://gnx.iojbl.cn

awk '{print $1, $3}' a.txt
来源：http://ioi.hammf.cn

[R49] awk 带条件
来源：http://tui.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vem.hnqzz.top

[R50] awk 求和
来源：http://qax.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ovf.haohaochexian.top

[R51] 排序去重取前几
来源：http://luk.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mcs.shangyingyoupin.top

[R52] 统计行数
来源：http://uyd.fengsongda.top

wc -l a.txt
来源：http://soy.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://zwr.hammf.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bji.kuanghao11.cn

[R54] 比较两个文件
来源：http://dgn.chenzaomai.com

diff a.txt b.txt
来源：http://xte.ehwqpu.com

[R55] 压缩与解压
来源：http://ldc.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nak.zhiwuduotai.top

[R56] 远程拷贝
来源：http://rwt.guannengcc.top

scp file user@host:/path/
来源：http://xub.yvedp.cn

[R57] 远程执行命令
来源：http://crt.ywan-chungtsiang.top

ssh user@host 'uptime'
来源：http://wzb.zdqjudy.top

[R58] 下载文件
来源：http://hsw.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://npg.epnwcf.com

[R59] 发 POST JSON
来源：http://ipp.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xhj.jinqigfzy.top

[R60] 只看 HTTP 状态码
来源：http://gox.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cxm.tian-w.cn

[R61] 磁盘占用
来源：http://jzv.tianlin.xyz

df -h;  du -sh *
来源：http://pnc.yongpay.top

[R62] 找最占空间的文件
来源：http://rfy.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://nut.shangyingyoupin.top

[R63] 内存与进程
来源：http://xcj.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://blr.jiagoushi.top

[R64] 结束进程
来源：http://esp.sweek.top

kill -9 $(pgrep -f app.py)
来源：http://glr.xziqi.cn

[R65] 查看端口占用
来源：http://ahb.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qpk.fktsv.cn

[R66] 定时任务
来源：http://pks.snrcjt.cn

crontab -e;  crontab -l
来源：http://xbc.316326.xyz

[R67] 生成随机十六进制串
来源：http://bag.hongshengwenyu.top

openssl rand -hex 16
来源：http://hcd.aibaodan.cn

[R68] 计算文件校验值
来源：http://ljj.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ahq.svipenyu.cn

[R69] 生成随机密码
来源：http://lsm.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://kuv.shuidangran.top

[R70] 时间戳与互转
来源：http://gkz.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://uzy.9152youxi.cn

[R71] 日期格式化
来源：http://vjs.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ljk.mhx1999.top

[R72] 等待端口就绪
来源：http://fkf.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qop.yvedp.cn

[R73] 分割大日志
来源：http://msg.vehdjk.com

split -l 1000 big.log part_
来源：http://kky.vehdjk.com

[R74] 批量重命名
来源：http://ivu.dashuyun.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iwv.chenzaomai.com

[R75] 导出环境变量
来源：http://yxw.zhixingplan.top

export PATH="$HOME/bin:$PATH"
来源：http://eip.bjfxy.top

[R76] 使用临时文件
来源：http://bft.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pxr.yvedp.cn

[R77] 读取用户输入
来源：http://iqd.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://nze.andypj.xyz

[R78] 交互式菜单
来源：http://nwr.zhijiandao.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://auq.9152youxi.cn

[R79] 解析命令行选项
来源：http://rml.hnxiangtu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://brl.cheryme.top

[R80] 查看脚本执行耗时
来源：http://hyr.jyoumei.cn

time ./run.sh
来源：http://wfw.chenlongwang.top

================================================================================
来源：http://ddg.birdmap.top

S. C / C++ 专题
来源：http://koi.yj20258.top

================================================================================
来源：http://adk.meibo888.top

[S01] C：Hello World
来源：http://hyj.sjlbkw.cn

#include <stdio.h>
来源：http://zdv.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jmw.xylfe.cn

[S02] C：变量与格式化输出
来源：http://uni.sweek.top

int a = 10; printf("%d\n", a);
来源：http://kgd.mhx1999.top

[S03] C：读入整数
来源：http://tdu.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://mdp.pengpengdd.cyou

[S04] C：字符串复制
来源：http://cew.birdmap.top

char dst[32]; strcpy(dst, "hi");
来源：http://few.xinyue.icu

[S05] C：字符串长度
来源：http://qiv.xziqi.cn

strlen(s)
来源：http://jqc.vqdsnc.cn

[S06] C：字符串比较
来源：http://svv.daria6918.cn

strcmp(a, b) == 0
来源：http://bpn.andypj.xyz

[S07] C：数组遍历求和
来源：http://qer.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pak.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://tmd.fengsongda.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tkd.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://lbq.jinghuilouyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yfd.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://ord.jqgfzy.top

int *p = &a;  *p = 5;
来源：http://rgd.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://fka.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://bie.zycfv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jkj.sweek.top

fclose(f);
来源：http://hxb.redwolf501.top

[S12] C：写文件
来源：http://ewx.fehbvm.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vkh.sxryk.cn

[S13] C：宏定义
来源：http://zkf.cqqwz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://peh.hcnkem.com

[S14] C：枚举
来源：http://kxu.vehdjk.com

enum Color { RED, GREEN, BLUE };
来源：http://ldb.chenlongwang.top

[S15] C：类型转换
来源：http://wha.tanke756.top

(double) a / b
来源：http://fby.gogol.net.cn

[S16] C：位操作置位
来源：http://lxy.quarkkingdee.top

x |= (1 << 3);
来源：http://gvh.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://mvt.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pnm.smart0.xyz

[S18] C：命令行参数
来源：http://psw.wangdashe.top

int main(int argc, char **argv)
来源：http://zzl.cdnleiting.top

[S19] C：快速排序
来源：http://blu.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lue.fanxiaobao.xyz

[S20] C：二分查找
来源：http://tnr.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tip.birdmap.top

[S21] C：字符类别判断
来源：http://uvb.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bly.aibaodan.cn

[S22] C：字符串转数字
来源：http://lqx.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qoe.yuanzhike.top

[S23] C：随机数
来源：http://rdt.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qzw.cdnleiting.top

[S24] C：获取本地时间
来源：http://gke.vehdjk.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://upc.pengpengdd.cyou

[S25] C：内存拷贝
来源：http://nfb.hongshengwenyu.top

memcpy(dst, src, n);
来源：http://int.fktsv.cn

[S26] C：内存清零
来源：http://dld.xuanzx.com

memset(a, 0, sizeof a);
来源：http://cxq.hammf.cn

[S27] C：定义常量
来源：http://hkz.chenjidiqi.icu

const double PI = 3.14159;
来源：http://ezz.birdmap.top

[S28] C：静态变量
来源：http://afh.bbcook.cn

static int counter = 0;
来源：http://sqg.sweek.top

[S29] C：变参函数
来源：http://qar.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rbv.yangfankeji.com

[S30] C：头文件保护
来源：http://kae.zhengqikj.top

#ifndef X_H
来源：http://ucw.yuanzhike.top

#define X_H
来源：http://khz.jlsjyb.cn

#endif
来源：http://ogq.fengsongda.top

[S31] C++：Hello World
来源：http://uji.hywenlv.cn

#include <iostream>
来源：http://apt.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://ibx.feifeiyinyue.top

[S32] C++：字符串
来源：http://anb.52xcode.cn

std::string s = "hi";  s += "!";
来源：http://yip.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://kvr.svipenyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://evj.snrcjt.cn

[S34] C++：遍历 vector
来源：http://avt.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://xfn.jinqigufen.top

[S35] C++：map
来源：http://dew.vqdsnc.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cyo.mhx1999.top

[S36] C++：unordered_map
来源：http://uxp.yj20258888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mjs.jiagoushi.top

[S37] C++：set
来源：http://vpu.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jac.sufxvd.cn

[S38] C++：排序
来源：http://dfr.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://zfo.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://kmo.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hdy.jiagoushi.top

[S40] C++：查找元素
来源：http://zct.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ksq.jinqigufen.top

[S41] C++：类与构造函数
来源：http://azq.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rnv.hnqzz.top

[S42] C++：继承与虚函数
来源：http://zoe.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://nzz.tian-w.cn

[S43] C++：智能指针
来源：http://dxl.hammf.cn

auto p = std::make_unique<int>(5);
来源：http://jfc.zhoulong.xyz

[S44] C++：引用传参
来源：http://dwy.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://bxs.yonumen.top

[S45] C++：lambda
来源：http://ker.svipenyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vmo.52xcode.cn

[S46] C++：函数模板
来源：http://taw.ydzc1.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dow.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://taj.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://clc.yonumen.top

[S48] C++：逐行读文件
来源：http://ohr.svipenyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mmc.birdmap.top

while (std::getline(in, line)) { }
来源：http://smr.ehwqpu.com

[S49] C++：写文件
来源：http://uop.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://djr.zdbjq.cn

[S50] C++：格式化数字
来源：http://bpq.iojbl.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vct.guowangkeji.top

[S51] C++：显式类型转换
来源：http://gmr.ivvv.top

static_cast<double>(a) / b
来源：http://czi.fengsongda.top

[S52] C++：const 与 noexcept
来源：http://dff.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://pme.jiagoushi.top

[S53] C++：移动语义
来源：http://efw.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://wfa.kuanghao11.cn

[S54] C++：异常处理
来源：http://scp.yuxming.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wfy.andypj.xyz

[S55] C++：结构化绑定
来源：http://hni.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eou.jinyuanbaomall.cn

[S56] C++：optional
来源：http://rro.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://flc.yfazqb.com

[S57] C++：编译期常量
来源：http://nsw.cqqwz.cn

constexpr int N = 10;
来源：http://lya.ywan-chungtsiang.top

[S58] C++：命名空间
来源：http://hpw.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://byl.fzhhl.top

[S59] C++：静态断言
来源：http://ocu.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kdn.ehwqpu.com

[S60] C++：遍历并删除元素
来源：http://uvj.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://emx.cashguo.top

================================================================================
来源：http://miz.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vgf.aibaodan.cn

================================================================================
来源：http://qyl.xziqi.cn

[T01] Kotlin：Hello World
来源：http://jls.shangyingyoupin.top

println("Hello")
来源：http://dfh.hongshengwenyu.top

[T02] Kotlin：变量
来源：http://wjr.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://har.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://udu.ywan-chungtsiang.top

"值: $b"
来源：http://hkq.sufxvd.cn

[T04] Kotlin：空安全
来源：http://ego.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://feb.fktsv.cn

[T05] Kotlin：when 表达式
来源：http://sxn.zhaomingkeji.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://skg.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://kjd.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mgm.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://for.hongshengwenyu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fjl.sweek.top

[T08] Kotlin：数据类
来源：http://rii.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://cup.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://yan.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://lmo.nwbrower.top

[T10] Kotlin：默认参数
来源：http://qyq.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qbp.bbcook.cn

[T11] Kotlin：协程
来源：http://cxz.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://fkw.xylfe.cn

[T12] Kotlin：解构声明
来源：http://lin.yfazqb.com

val (a, b) = Pair(1, 2)
来源：http://lyp.andypj.xyz

[T13] Kotlin：只读 Map
来源：http://fqa.chenjidiqi.icu

val m = mapOf("a" to 1)
来源：http://vyi.nanxinkj.top

[T14] Kotlin：循环
来源：http://nob.meibo888.top

for (i in 1..10) println(i)
来源：http://bqh.zhongyouzk.top


<!-- 参考信息 -->