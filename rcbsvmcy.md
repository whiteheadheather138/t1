代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blj.cqqwz.cn

[R08] 数值比较
来源：http://cgw.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lub.gogol.net.cn

[R09] 字符串比较
来源：http://oxq.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hcq.shuidangran.top

[R10] 正则匹配
来源：http://jru.hcnkem.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yhu.jianghu66.top

[R11] case 多分支
来源：http://nzc.zhoulong.xyz

case "$1" in
来源：http://quc.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://zpq.zycfv.cn

stop)  echo "停止" ;;
来源：http://zxd.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://gan.jiagoushi.top

esac
来源：http://ysb.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://cnk.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://sdd.sufxvd.cn

[R13] for 计数循环
来源：http://vza.yj20258888.top

for i in {1..10}; do echo "$i"; done
来源：http://gqm.snrcjt.cn

[R14] C 风格 for
来源：http://mtb.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cvg.chenzaomai.com

[R15] while 逐行读文件
来源：http://eby.c1oappe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kdi.bbcook.cn

[R16] until 等待条件
来源：http://agu.yj20258888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ktb.tanke756.top

[R17] 数组定义与取值
来源：http://see.gotoacloud.top

arr=(a b c); echo "${arr[0]}"
来源：http://xfv.pycfn.com

[R18] 遍历数组
来源：http://csj.yonumen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dbe.shuidangran.top

[R19] 数组长度
来源：http://ldp.jlsjyb.cn

echo "${#arr[@]}"
来源：http://vpq.zhixingplan.top

[R20] 关联数组（字典）
来源：http://sik.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nxq.vehdjk.com

[R21] 字符串长度
来源：http://bfb.jinyuanbaomall.cn

echo "${#s}"
来源：http://czb.yueranfly.top

[R22] 截取子串
来源：http://pbn.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://zsm.ydzc1.top

[R23] 字符串替换
来源：http://lbv.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ird.cashguo.top

[R24] 大小写转换
来源：http://fmb.zhengqikj.top

echo "${s^^}"; echo "${s,,}"
来源：http://sat.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://ueh.xziqi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wju.svipenyu.cn

[R26] 命令替换
来源：http://pcr.feifeiyinyue.top

now=$(date +%F); echo "$now"
来源：http://rpp.snrcjt.cn

[R27] 算术展开
来源：http://wfm.guannengcc.top

echo $((1 + 2 * 3))
来源：http://bgj.fktsv.cn

[R28] 浮点运算
来源：http://tkg.pycfn.com

echo "scale=2; 10/3" | bc
来源：http://emg.zhengqikj.top

[R29] 定义函数
来源：http://qxy.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://age.nanxinkj.top

[R30] 函数返回状态码
来源：http://mbz.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://ujc.dianchejie.cn

[R31] 局部变量
来源：http://lbi.yvedp.cn

f() { local x=1; echo "$x"; }
来源：http://hyz.wangdashe.top

[R32] 参数个数校验
来源：http://fnd.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qhp.chenlongwang.top

[R33] 捕获错误并提示行号
来源：http://zqu.hywenlv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://urn.hongshengwenyu.top

[R34] 退出时清理
来源：http://tvm.pengpengdd.cyou

trap 'rm -f "$tmp"' EXIT
来源：http://oft.bjfxy.top

[R35] 后台执行并等待
来源：http://gdn.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qns.jianghu66.top

[R36] 并发执行多个任务
来源：http://dbe.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jvx.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://hei.xuetiantiany.cn

files=$(ls -1)
来源：http://xdi.hammf.cn

[R38] 管道串联
来源：http://mdc.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://bfu.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://sju.jinqigufen.top

cmd > out.log 2>&1
来源：http://xzu.yj202588.top

[R40] 追加写日志
来源：http://anr.andypj.xyz

echo "log" >> out.log
来源：http://lkb.jinghuilouyu.cn

[R41] 丢弃输出
来源：http://hgx.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://njp.xinyue.icu

[R42] 输入重定向
来源：http://lwt.zhengqikj.top

wc -l < a.txt
来源：http://zur.jqgfzy.top

[R43] 按名字查找文件
来源：http://mfq.vehdjk.com

find . -name "*.log" -type f
来源：http://nhp.jinqigufen.top

[R44] 按修改时间查找
来源：http://wyk.fehbvm.com

find . -mtime -7 -type f
来源：http://tmt.zhongyouzk.top

[R45] 批量删除
来源：http://cby.hesvh.cn

find . -name "*.tmp" -delete
来源：http://pki.yongpay.top

[R46] 递归替换文件内容
来源：http://cdp.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lte.shzxlz.cn

[R47] sed 单行替换
来源：http://uze.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://myp.tianlin.xyz

[R48] awk 取指定列
来源：http://kjr.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://qhy.svipenyu.cn

[R49] awk 带条件
来源：http://oub.xuetiantiany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tzu.uphjek.com

[R50] awk 求和
来源：http://pst.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://zin.fehbvm.com

[R51] 排序去重取前几
来源：http://tgg.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hgn.mhx1999.top

[R52] 统计行数
来源：http://vyr.hnqzz.top

wc -l a.txt
来源：http://wir.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://hbb.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qvk.snrcjt.cn

[R54] 比较两个文件
来源：http://rxe.ivvv.top

diff a.txt b.txt
来源：http://nur.ivvv.top

[R55] 压缩与解压
来源：http://orl.ctjpmb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cdf.c1oappe.top

[R56] 远程拷贝
来源：http://vkj.chenjidiqi.icu

scp file user@host:/path/
来源：http://kxh.yuanzhike.top

[R57] 远程执行命令
来源：http://wwp.zhengqikj.top

ssh user@host 'uptime'
来源：http://mlp.xinyue.icu

[R58] 下载文件
来源：http://wmb.aibaodan.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jst.hongshengwenyu.top

[R59] 发 POST JSON
来源：http://qyt.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vgb.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://vgj.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oeo.kuanghao11.cn

[R61] 磁盘占用
来源：http://zvn.sxryk.cn

df -h;  du -sh *
来源：http://efy.shuidangran.top

[R62] 找最占空间的文件
来源：http://jnr.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://gsw.yongpay.top

[R63] 内存与进程
来源：http://uuv.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://nsc.yonumen.top

[R64] 结束进程
来源：http://ihy.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://tef.yj20258888.top

[R65] 查看端口占用
来源：http://hls.daria6918.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sru.shuidangran.top

[R66] 定时任务
来源：http://hdi.jinghuilouyu.cn

crontab -e;  crontab -l
来源：http://ozr.hnqzz.top

[R67] 生成随机十六进制串
来源：http://hpf.yvedp.cn

openssl rand -hex 16
来源：http://ruo.aibaodan.cn

[R68] 计算文件校验值
来源：http://yak.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://prv.c1oappe.top

[R69] 生成随机密码
来源：http://qnf.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://kld.hnxiangtu.top

[R70] 时间戳与互转
来源：http://ewy.feifeiyinyue.top

date +%s;  date -d @1700000000
来源：http://xca.havefunace.top

[R71] 日期格式化
来源：http://mhd.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kek.aibaodan.cn

[R72] 等待端口就绪
来源：http://bwd.sweek.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qio.cheryme.top

[R73] 分割大日志
来源：http://zgv.xziqi.cn

split -l 1000 big.log part_
来源：http://qhv.sufxvd.cn

[R74] 批量重命名
来源：http://lyp.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ncp.bjfxy.top

[R75] 导出环境变量
来源：http://yrf.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://php.tianlin.xyz

[R76] 使用临时文件
来源：http://rwv.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lgv.ydzc1.top

[R77] 读取用户输入
来源：http://mty.zhixingplan.top

read -rp "请输入: " ans
来源：http://vjx.hywenlv.cn

[R78] 交互式菜单
来源：http://kcl.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://caq.guannengcc.top

[R79] 解析命令行选项
来源：http://nkr.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tnq.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://wje.zycfv.cn

time ./run.sh
来源：http://zrt.jianghu66.top

================================================================================
来源：http://xqe.cucudq.cn

S. C / C++ 专题
来源：http://ode.shzxlz.cn

================================================================================
来源：http://jez.zhiwuduotai.top

[S01] C：Hello World
来源：http://smn.birdmap.top

#include <stdio.h>
来源：http://hmk.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jak.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://cur.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://rbx.kuanghao11.cn

[S03] C：读入整数
来源：http://pud.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://qgb.iojbl.cn

[S04] C：字符串复制
来源：http://fzs.nanxinkj.top

char dst[32]; strcpy(dst, "hi");
来源：http://lkz.jinqigfzy.top

[S05] C：字符串长度
来源：http://wbn.pengpengdd.cyou

strlen(s)
来源：http://imu.zhengqikj.top

[S06] C：字符串比较
来源：http://ofs.zhoulong.xyz

strcmp(a, b) == 0
来源：http://xyy.hnqzz.top

[S07] C：数组遍历求和
来源：http://wmo.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vdh.meibo888.top

[S08] C：动态内存分配与释放
来源：http://lqr.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sjh.shanyushiyangkeji.top

[S09] C：结构体定义与初始化
来源：http://ogb.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://joe.ehwqpu.com

[S10] C：指针与解引用
来源：http://pro.yuxming.cn

int *p = &a;  *p = 5;
来源：http://zub.sysykeji.top

[S11] C：逐行读文件
来源：http://ojt.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://wtz.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zof.shanyushiyangtech.top

fclose(f);
来源：http://zbi.iojbl.cn

[S12] C：写文件
来源：http://gme.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uwm.yj20258.top

[S13] C：宏定义
来源：http://uej.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mxk.fanxiaobao.xyz

[S14] C：枚举
来源：http://etf.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://dzh.shangyingyoupin.top

[S15] C：类型转换
来源：http://zhw.jinyuanbaomall.cn

(double) a / b
来源：http://gkp.yongpay.top

[S16] C：位操作置位
来源：http://wid.chenjidiqi.icu

x |= (1 << 3);
来源：http://hwz.daxiang520.top

[S17] C：安全拼接字符串
来源：http://usl.shanyushiyangtech.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oxy.sjlbkw.cn

[S18] C：命令行参数
来源：http://pjm.316326.xyz

int main(int argc, char **argv)
来源：http://psp.fengsongda.top

[S19] C：快速排序
来源：http://sqb.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://opa.hesvh.cn

[S20] C：二分查找
来源：http://hei.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fqs.chenlongwang.top

[S21] C：字符类别判断
来源：http://wst.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dzh.gzhubu.top

[S22] C：字符串转数字
来源：http://lbp.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bcu.hywenlv.cn

[S23] C：随机数
来源：http://jvn.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://icc.xinyue.icu

[S24] C：获取本地时间
来源：http://awk.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pku.gzhubu.top

[S25] C：内存拷贝
来源：http://glz.zhongyouzk.top

memcpy(dst, src, n);
来源：http://ylp.c1oappe.top

[S26] C：内存清零
来源：http://fto.pengpengdd.cyou

memset(a, 0, sizeof a);
来源：http://eep.yj20258888.top

[S27] C：定义常量
来源：http://drk.chenjidiqi.icu

const double PI = 3.14159;
来源：http://wep.c1oappe.top

[S28] C：静态变量
来源：http://vco.smart0.xyz

static int counter = 0;
来源：http://ntt.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://upf.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sxq.cheryme.top

[S30] C：头文件保护
来源：http://usv.xziqi.cn

#ifndef X_H
来源：http://dza.wangshuangyany.cn

#define X_H
来源：http://rns.ehwqpu.com

#endif
来源：http://jsf.zhengqikj.top

[S31] C++：Hello World
来源：http://fwi.fktsv.cn

#include <iostream>
来源：http://ocs.jinyuanbaomall.cn

int main() { std::cout << "Hello\n"; }
来源：http://omm.nanxinkj.top

[S32] C++：字符串
来源：http://msb.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://rzq.316326.xyz

[S33] C++：vector 增删
来源：http://ypq.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xzw.hysaishi.cn

[S34] C++：遍历 vector
来源：http://nor.cqqwz.cn

for (auto &x : v) { std::cout << x; }
来源：http://tfp.kuanghao11.cn

[S35] C++：map
来源：http://uej.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cju.hnxiangtu.top

[S36] C++：unordered_map
来源：http://nhz.sufxvd.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zky.zdqjudy.top

[S37] C++：set
来源：http://ohj.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fjd.ydzc1.top

[S38] C++：排序
来源：http://bfj.pycfn.com

std::sort(v.begin(), v.end());
来源：http://jut.xingfuxueyuan.xyz

[S39] C++：自定义比较器排序
来源：http://iza.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fmv.quarkkingdee.top

[S40] C++：查找元素
来源：http://cbx.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://svk.xuanzx.com

[S41] C++：类与构造函数
来源：http://kcj.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xxd.vehdjk.com

[S42] C++：继承与虚函数
来源：http://rky.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://jzu.ivvv.top

[S43] C++：智能指针
来源：http://biu.sysykeji.top

auto p = std::make_unique<int>(5);
来源：http://hua.xylfe.cn

[S44] C++：引用传参
来源：http://opr.yj20258.top

void inc(int &x) { ++x; }
来源：http://yof.uphjek.com

[S45] C++：lambda
来源：http://dwa.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vws.xinyue.icu

[S46] C++：函数模板
来源：http://ljm.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dto.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://vqp.quarkkingdee.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uke.snrcjt.cn

[S48] C++：逐行读文件
来源：http://ecn.aibaodan.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qhv.yfazqb.com

while (std::getline(in, line)) { }
来源：http://cum.guowangkeji.top

[S49] C++：写文件
来源：http://xke.wangshuangyany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://azv.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://xha.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fks.hywenlv.cn

[S51] C++：显式类型转换
来源：http://eyf.shuidangran.top

static_cast<double>(a) / b
来源：http://iaj.jinqigufen.top

[S52] C++：const 与 noexcept
来源：http://dcv.zycfv.cn

int size() const noexcept { return n_; }
来源：http://yar.wangshuangyany.cn

[S53] C++：移动语义
来源：http://kjr.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://nzc.hcnkem.com

[S54] C++：异常处理
来源：http://rlv.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://plq.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://stv.zhongyouzk.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vfq.xziqi.cn

[S56] C++：optional
来源：http://cgh.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wpb.jinqigfzy.top

[S57] C++：编译期常量
来源：http://rop.chenjidiqi.icu

constexpr int N = 10;
来源：http://yiu.nanxuanxn.top

[S58] C++：命名空间
来源：http://gsv.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://yud.zhiwuduotai.top

[S59] C++：静态断言
来源：http://lee.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xkh.sxryk.cn

[S60] C++：遍历并删除元素
来源：http://nes.fehbvm.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dlx.hfpthk.cn

================================================================================
来源：http://qrm.nanxinkj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uiv.kuanghao11.cn

================================================================================
来源：http://qer.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://vew.svipenyu.cn

println("Hello")
来源：http://bkr.yuxming.cn

[T02] Kotlin：变量
来源：http://jdx.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qcb.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://nnw.jinyuanbaomall.cn

"值: $b"
来源：http://quf.shuidangran.top

[T04] Kotlin：空安全
来源：http://wrk.guannengcc.top

val n: String? = null;  n?.length
来源：http://cxs.gzhubu.top

[T05] Kotlin：when 表达式
来源：http://vmv.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vnn.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://kbq.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://agx.tanke756.top

[T07] Kotlin：集合过滤
来源：http://fzq.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://biy.dianchejie.cn

[T08] Kotlin：数据类
来源：http://znf.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://kru.yvedp.cn


<!-- 参考信息 -->