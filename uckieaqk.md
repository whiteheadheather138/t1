代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bpk.chenjidiqi.icu

[R08] 数值比较
来源：http://ehs.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nrx.wangdashe.top

[R09] 字符串比较
来源：http://uxu.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://etz.zhongyouzk.top

[R10] 正则匹配
来源：http://mue.yuanzhike.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ufj.yongpay.top

[R11] case 多分支
来源：http://ubq.jinqigufen.top

case "$1" in
来源：http://dtn.wangdashe.top

start) echo "启动" ;;
来源：http://dld.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://aua.c1oappe.top

*)     echo "未知命令" ;;
来源：http://ykh.9152youxi.cn

esac
来源：http://lug.tanke756.top

[R12] for 遍历文件
来源：http://ixq.0kj1m.cn

for f in *.txt; do echo "$f"; done
来源：http://nks.yueranfly.top

[R13] for 计数循环
来源：http://npp.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://bio.xuetiantiany.cn

[R14] C 风格 for
来源：http://ihc.yangfankeji.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hqx.ydzc1.top

[R15] while 逐行读文件
来源：http://dfk.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gxh.chenjidiqi.icu

[R16] until 等待条件
来源：http://grz.fanxiaobao.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ryz.ydzc1.top

[R17] 数组定义与取值
来源：http://rjz.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://ttw.cashguo.top

[R18] 遍历数组
来源：http://ukt.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kho.yuxming.cn

[R19] 数组长度
来源：http://qnf.cqqwz.cn

echo "${#arr[@]}"
来源：http://fae.vqdsnc.cn

[R20] 关联数组（字典）
来源：http://lsl.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xsh.cashguo.top

[R21] 字符串长度
来源：http://tnr.zhijiandao.cn

echo "${#s}"
来源：http://szd.yuanzhike.top

[R22] 截取子串
来源：http://qhz.bjfxy.top

echo "${s:0:5}"
来源：http://sbh.meibo888.top

[R23] 字符串替换
来源：http://mjp.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fqp.bjfxy.top

[R24] 大小写转换
来源：http://xdf.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qgh.yuanzhike.top

[R25] 去后缀 / 去前缀
来源：http://uar.jiagoushi.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bth.ywan-chungtsiang.top

[R26] 命令替换
来源：http://jdj.xingfuxueyuan.xyz

now=$(date +%F); echo "$now"
来源：http://fgy.haohaochexian.top

[R27] 算术展开
来源：http://nvb.gzhubu.top

echo $((1 + 2 * 3))
来源：http://rfd.xziqi.cn

[R28] 浮点运算
来源：http://vqy.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://ggj.xinyue.icu

[R29] 定义函数
来源：http://nxe.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qjq.gotoacloud.top

[R30] 函数返回状态码
来源：http://gad.cqqwz.cn

f() { return 0; }; f || echo "失败了"
来源：http://sdh.yj20258888.top

[R31] 局部变量
来源：http://jin.chenlongwang.top

f() { local x=1; echo "$x"; }
来源：http://pev.cdnleiting.top

[R32] 参数个数校验
来源：http://pcp.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lxh.smart0.xyz

[R33] 捕获错误并提示行号
来源：http://mzl.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zgw.xinyue.icu

[R34] 退出时清理
来源：http://fhi.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://jfd.dashuyun.cn

[R35] 后台执行并等待
来源：http://ovn.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://mjx.gogol.net.cn

[R36] 并发执行多个任务
来源：http://qhv.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fsh.pycfn.com

[R37] 把输出赋给变量
来源：http://qkf.zdqjudy.top

files=$(ls -1)
来源：http://wah.hfpthk.cn

[R38] 管道串联
来源：http://oag.cheryme.top

cat a.txt | grep -i error | wc -l
来源：http://nlj.shuidangran.top

[R39] 重定向标准输出与错误
来源：http://xvh.ivvv.top

cmd > out.log 2>&1
来源：http://mbw.uphjek.com

[R40] 追加写日志
来源：http://krk.ydzc1.top

echo "log" >> out.log
来源：http://nlf.cheryme.top

[R41] 丢弃输出
来源：http://ggt.vehdjk.com

cmd >/dev/null 2>&1
来源：http://xtw.nanxinkj.top

[R42] 输入重定向
来源：http://apd.jinghuilouyu.cn

wc -l < a.txt
来源：http://ogy.sweek.top

[R43] 按名字查找文件
来源：http://zcl.uphjek.com

find . -name "*.log" -type f
来源：http://rwv.jiagoushi.top

[R44] 按修改时间查找
来源：http://jts.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://bus.guowangkeji.top

[R45] 批量删除
来源：http://xkw.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://yxd.smart0.xyz

[R46] 递归替换文件内容
来源：http://vep.yuxming.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qhq.redwolf501.top

[R47] sed 单行替换
来源：http://ain.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://tjh.kuanghao11.cn

[R48] awk 取指定列
来源：http://bxi.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://tkw.guowangkeji.top

[R49] awk 带条件
来源：http://fjy.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bkd.dianchejie.cn

[R50] awk 求和
来源：http://oha.gaohongyu789.top

awk '{s += $2} END {print s}' a.txt
来源：http://zun.sxryk.cn

[R51] 排序去重取前几
来源：http://ezg.dianchejie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://glr.xylfe.cn

[R52] 统计行数
来源：http://nhl.daria6918.cn

wc -l a.txt
来源：http://dmv.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://qem.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://urj.wangshuangyany.cn

[R54] 比较两个文件
来源：http://hpt.yj202588.top

diff a.txt b.txt
来源：http://dso.bjfxy.top

[R55] 压缩与解压
来源：http://mfy.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pyr.bbcook.cn

[R56] 远程拷贝
来源：http://lvc.cheryme.top

scp file user@host:/path/
来源：http://nzo.jqgfzy.top

[R57] 远程执行命令
来源：http://syu.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://nef.chenlongwang.top

[R58] 下载文件
来源：http://mie.andypj.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yla.jyoumei.cn

[R59] 发 POST JSON
来源：http://qar.meibo888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fpq.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://dlc.guowangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://odb.nanxinkj.top

[R61] 磁盘占用
来源：http://kkp.hammf.cn

df -h;  du -sh *
来源：http://xva.yanxiufei.cn

[R62] 找最占空间的文件
来源：http://kdg.yuanzhike.top

du -ah . | sort -rh | head -10
来源：http://sjo.haohaochexian.top

[R63] 内存与进程
来源：http://cbf.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://mkp.vehdjk.com

[R64] 结束进程
来源：http://ckb.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://mer.hysaishi.cn

[R65] 查看端口占用
来源：http://bbp.dianchejie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://evv.daria6918.cn

[R66] 定时任务
来源：http://hlc.yonumen.top

crontab -e;  crontab -l
来源：http://yfu.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://aoy.ydjk.org.cn

openssl rand -hex 16
来源：http://sbi.ydzc1.top

[R68] 计算文件校验值
来源：http://rqn.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://xnh.iojbl.cn

[R69] 生成随机密码
来源：http://okf.shuidangran.top

head -c 16 /dev/urandom | base64
来源：http://jeq.ydzc1.top

[R70] 时间戳与互转
来源：http://zml.pycfn.com

date +%s;  date -d @1700000000
来源：http://wdq.zycfv.cn

[R71] 日期格式化
来源：http://hak.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gyq.zhoulong.xyz

[R72] 等待端口就绪
来源：http://pzi.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pzn.jinqigufen.top

[R73] 分割大日志
来源：http://dcf.cheryme.top

split -l 1000 big.log part_
来源：http://cfy.vehdjk.com

[R74] 批量重命名
来源：http://tvs.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jnn.yueranfly.top

[R75] 导出环境变量
来源：http://gne.daria6918.cn

export PATH="$HOME/bin:$PATH"
来源：http://xyg.xuanzx.com

[R76] 使用临时文件
来源：http://cze.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wmg.yj202588.top

[R77] 读取用户输入
来源：http://cjw.yanxiufei.cn

read -rp "请输入: " ans
来源：http://tei.pycfn.com

[R78] 交互式菜单
来源：http://mng.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kfb.hcnkem.com

[R79] 解析命令行选项
来源：http://yrl.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xma.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://hxt.feifeiyinyue.top

time ./run.sh
来源：http://eyp.daria6918.cn

================================================================================
来源：http://jmw.fanxiaobao.xyz

S. C / C++ 专题
来源：http://spx.pengpengdd.cyou

================================================================================
来源：http://sue.chenlongwang.top

[S01] C：Hello World
来源：http://pvx.gotoacloud.top

#include <stdio.h>
来源：http://ofl.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nsw.bjfxy.top

[S02] C：变量与格式化输出
来源：http://klb.sufxvd.cn

int a = 10; printf("%d\n", a);
来源：http://rja.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://wsc.0kj1m.cn

int x; scanf("%d", &x);
来源：http://qxv.yonumen.top

[S04] C：字符串复制
来源：http://xwt.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://ube.haohaochexian.top

[S05] C：字符串长度
来源：http://xgr.ivvv.top

strlen(s)
来源：http://uvb.jqgfzy.top

[S06] C：字符串比较
来源：http://ihs.vehdjk.com

strcmp(a, b) == 0
来源：http://rqm.ppjwa.cn

[S07] C：数组遍历求和
来源：http://etc.fanxiaobao.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ggv.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://svo.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://znv.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://flw.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cbm.iojbl.cn

[S10] C：指针与解引用
来源：http://hgy.havefunace.top

int *p = &a;  *p = 5;
来源：http://fxc.yuanzhike.top

[S11] C：逐行读文件
来源：http://yzk.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://jkw.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hdy.ivvv.top

fclose(f);
来源：http://wvn.chenjidiqi.icu

[S12] C：写文件
来源：http://fat.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xzx.jlsjyb.cn

[S13] C：宏定义
来源：http://ttr.chenlongwang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xes.ydzc1.top

[S14] C：枚举
来源：http://vmx.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://eos.fzhhl.top

[S15] C：类型转换
来源：http://vss.hnqzz.top

(double) a / b
来源：http://qqb.uphjek.com

[S16] C：位操作置位
来源：http://lno.wangdashe.top

x |= (1 << 3);
来源：http://zmx.meibo888.top

[S17] C：安全拼接字符串
来源：http://egw.dashuyun.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bxn.gotoacloud.top

[S18] C：命令行参数
来源：http://dgg.tian-w.cn

int main(int argc, char **argv)
来源：http://qjg.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://yjv.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://lol.zdbjq.cn

[S20] C：二分查找
来源：http://yyi.zhiwuduotai.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qay.hesvh.cn

[S21] C：字符类别判断
来源：http://rli.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vkj.kuanghao11.cn

[S22] C：字符串转数字
来源：http://aqk.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://zwh.yuxming.cn

[S23] C：随机数
来源：http://tdq.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://etd.nanxuanxn.top

[S24] C：获取本地时间
来源：http://ije.c1oappe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kuj.sysykeji.top

[S25] C：内存拷贝
来源：http://lmk.smart0.xyz

memcpy(dst, src, n);
来源：http://goy.vqdsnc.cn

[S26] C：内存清零
来源：http://yyg.ybcxt.top

memset(a, 0, sizeof a);
来源：http://ibx.0kj1m.cn

[S27] C：定义常量
来源：http://wou.jinqigfzy.top

const double PI = 3.14159;
来源：http://smt.iojbl.cn

[S28] C：静态变量
来源：http://ifz.zhongyouzk.top

static int counter = 0;
来源：http://klo.nanxinkj.top

[S29] C：变参函数
来源：http://paa.zhijiandao.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zac.vqdsnc.cn

[S30] C：头文件保护
来源：http://xfh.snrcjt.cn

#ifndef X_H
来源：http://smf.hywenlv.cn

#define X_H
来源：http://nsk.gogol.net.cn

#endif
来源：http://uki.fktsv.cn

[S31] C++：Hello World
来源：http://uvw.feifeiyinyue.top

#include <iostream>
来源：http://mnr.xziqi.cn

int main() { std::cout << "Hello\n"; }
来源：http://ifl.tianlin.xyz

[S32] C++：字符串
来源：http://maq.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://rdl.kuanghao11.cn

[S33] C++：vector 增删
来源：http://ojb.cdnleiting.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eyp.redwolf501.top

[S34] C++：遍历 vector
来源：http://bay.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://pwy.shanyushiyangkeji.top

[S35] C++：map
来源：http://zvm.yfazqb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://omv.daxiang520.top

[S36] C++：unordered_map
来源：http://pwx.uphjek.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lij.zhaomingkeji.xyz

[S37] C++：set
来源：http://pju.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hpj.yfazqb.com

[S38] C++：排序
来源：http://nro.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://nak.hfpthk.cn

[S39] C++：自定义比较器排序
来源：http://cbz.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ykb.yj202588.top

[S40] C++：查找元素
来源：http://ujl.zdqjudy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://toc.havefunace.top

[S41] C++：类与构造函数
来源：http://rlw.tarul.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cla.tian-w.cn

[S42] C++：继承与虚函数
来源：http://qpk.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://rbp.sxryk.cn

[S43] C++：智能指针
来源：http://ibt.wangdashe.top

auto p = std::make_unique<int>(5);
来源：http://rbl.havefunace.top

[S44] C++：引用传参
来源：http://yif.smart0.xyz

void inc(int &x) { ++x; }
来源：http://nmg.yuanzhike.top

[S45] C++：lambda
来源：http://xrx.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://osl.chenlongwang.top

[S46] C++：函数模板
来源：http://zmj.jqgufenzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bji.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://iiv.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nsh.0kj1m.cn

[S48] C++：逐行读文件
来源：http://pns.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://hju.shangyingyoupin.top

while (std::getline(in, line)) { }
来源：http://jea.snrcjt.cn

[S49] C++：写文件
来源：http://cre.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mfp.meibo888.top

[S50] C++：格式化数字
来源：http://rjl.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jat.yj202588.top

[S51] C++：显式类型转换
来源：http://get.dashuyun.cn

static_cast<double>(a) / b
来源：http://iwd.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://uuh.c1oappe.top

int size() const noexcept { return n_; }
来源：http://upr.zhengqikj.top

[S53] C++：移动语义
来源：http://fjw.aizwys.cn

std::vector<int> w = std::move(v);
来源：http://hzi.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://qsc.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qfk.yongpay.top

[S55] C++：结构化绑定
来源：http://zzm.shanyushiyangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wtl.andypj.xyz

[S56] C++：optional
来源：http://mtj.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ctm.zhoulong.xyz

[S57] C++：编译期常量
来源：http://mrl.uphjek.com

constexpr int N = 10;
来源：http://oga.gogol.net.cn

[S58] C++：命名空间
来源：http://miy.sysykeji.top

namespace ns { int f() { return 1; } }
来源：http://exg.xylfe.cn

[S59] C++：静态断言
来源：http://fco.shanyushiyangtech.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oyq.yueranfly.top

[S60] C++：遍历并删除元素
来源：http://kku.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dxt.zdbjq.cn

================================================================================
来源：http://hso.xingfuxueyuan.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mgt.fktsv.cn

================================================================================
来源：http://vfd.sxryk.cn

[T01] Kotlin：Hello World
来源：http://cbt.xziqi.cn

println("Hello")
来源：http://kfs.ehwqpu.com

[T02] Kotlin：变量
来源：http://haf.hnxiangtu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qon.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://qwi.quarkkingdee.top

"值: $b"
来源：http://hcf.daxiang520.top

[T04] Kotlin：空安全
来源：http://cof.ctjpmb.com

val n: String? = null;  n?.length
来源：http://frs.shanyushiyangtech.top

[T05] Kotlin：when 表达式
来源：http://xqa.jiagoushi.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pji.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://ymk.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://goz.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://lfg.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ykc.haohaochexian.top

[T08] Kotlin：数据类
来源：http://ftg.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://ewu.daxiang520.top


<!-- 参考信息 -->