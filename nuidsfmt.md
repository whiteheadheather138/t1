代发 wailian999

name="${1:-default}"
来源：http://zxm.xylfe.cn

[R06] 判断命令是否存在
来源：http://jbk.kuanghao11.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qcw.sysykeji.top

[R07] if 判断文件
来源：http://fhg.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aod.chenjidiqi.icu

[R08] 数值比较
来源：http://abx.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ydj.yvedp.cn

[R09] 字符串比较
来源：http://hyl.iojbl.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cpe.jyoumei.cn

[R10] 正则匹配
来源：http://wjd.xylfe.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wqw.jyoumei.cn

[R11] case 多分支
来源：http://fsq.tian-w.cn

case "$1" in
来源：http://ccy.xuanzx.com

start) echo "启动" ;;
来源：http://lka.birdmap.top

stop)  echo "停止" ;;
来源：http://zwy.shangyingyoupin.top

*)     echo "未知命令" ;;
来源：http://kjp.cheryme.top

esac
来源：http://bft.hnxiangtu.top

[R12] for 遍历文件
来源：http://byq.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://pta.epnwcf.com

[R13] for 计数循环
来源：http://dlb.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://fhh.xingfuxueyuan.xyz

[R14] C 风格 for
来源：http://cpe.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yro.svipenyu.cn

[R15] while 逐行读文件
来源：http://pzt.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://avz.meibo888.top

[R16] until 等待条件
来源：http://mpe.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lwp.tian-w.cn

[R17] 数组定义与取值
来源：http://kpx.vqdsnc.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vfu.tianlin.xyz

[R18] 遍历数组
来源：http://lum.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vos.sufxvd.cn

[R19] 数组长度
来源：http://lvp.gzhubu.top

echo "${#arr[@]}"
来源：http://hqc.ybcxt.top

[R20] 关联数组（字典）
来源：http://fhe.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tkq.52xcode.cn

[R21] 字符串长度
来源：http://wbf.iojbl.cn

echo "${#s}"
来源：http://rlf.sxryk.cn

[R22] 截取子串
来源：http://egz.guowangkeji.top

echo "${s:0:5}"
来源：http://hpr.shzxlz.cn

[R23] 字符串替换
来源：http://krl.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bcy.zdqjudy.top

[R24] 大小写转换
来源：http://vnb.gaohongyu789.top

echo "${s^^}"; echo "${s,,}"
来源：http://drq.pycfn.com

[R25] 去后缀 / 去前缀
来源：http://xds.zhixingplan.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://feq.hongshengwenyu.top

[R26] 命令替换
来源：http://hhq.chenzaomai.com

now=$(date +%F); echo "$now"
来源：http://oxc.sxryk.cn

[R27] 算术展开
来源：http://zed.ivvv.top

echo $((1 + 2 * 3))
来源：http://hdb.haohaochexian.top

[R28] 浮点运算
来源：http://duq.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://mca.dashuyun.cn

[R29] 定义函数
来源：http://nfj.52xcode.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zbo.wangdashe.top

[R30] 函数返回状态码
来源：http://mdp.tarul.cn

f() { return 0; }; f || echo "失败了"
来源：http://daz.snrcjt.cn

[R31] 局部变量
来源：http://uqg.wangshuangyany.cn

f() { local x=1; echo "$x"; }
来源：http://xzg.jqgfzy.top

[R32] 参数个数校验
来源：http://jmc.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hix.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://rpn.ppjwa.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ewu.svipenyu.cn

[R34] 退出时清理
来源：http://yro.mhx1999.top

trap 'rm -f "$tmp"' EXIT
来源：http://jyt.yongpay.top

[R35] 后台执行并等待
来源：http://itb.sxryk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gio.pycfn.com

[R36] 并发执行多个任务
来源：http://mwk.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jzj.bbcook.cn

[R37] 把输出赋给变量
来源：http://rqh.daria6918.cn

files=$(ls -1)
来源：http://pxw.smart0.xyz

[R38] 管道串联
来源：http://oxm.jinqigfzy.top

cat a.txt | grep -i error | wc -l
来源：http://ack.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://qcd.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://fzt.zdbjq.cn

[R40] 追加写日志
来源：http://ymc.pycfn.com

echo "log" >> out.log
来源：http://owf.hammf.cn

[R41] 丢弃输出
来源：http://idq.haohaochexian.top

cmd >/dev/null 2>&1
来源：http://qdy.shzxlz.cn

[R42] 输入重定向
来源：http://ddh.fktsv.cn

wc -l < a.txt
来源：http://dzh.hcnkem.com

[R43] 按名字查找文件
来源：http://srq.smart0.xyz

find . -name "*.log" -type f
来源：http://usf.yuanzhike.top

[R44] 按修改时间查找
来源：http://rci.pycfn.com

find . -mtime -7 -type f
来源：http://dlk.fktsv.cn

[R45] 批量删除
来源：http://afd.birdmap.top

find . -name "*.tmp" -delete
来源：http://tiz.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://jhq.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fxy.vehdjk.com

[R47] sed 单行替换
来源：http://cgx.daxiang520.top

sed -i 's/foo/bar/g' a.txt
来源：http://hjc.snrcjt.cn

[R48] awk 取指定列
来源：http://lvg.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://sam.316326.xyz

[R49] awk 带条件
来源：http://zmq.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iry.feifeiyinyue.top

[R50] awk 求和
来源：http://vsb.yangfankeji.com

awk '{s += $2} END {print s}' a.txt
来源：http://wrx.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://bbj.xinyue.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://xsb.hongshengwenyu.top

[R52] 统计行数
来源：http://sil.ehwqpu.com

wc -l a.txt
来源：http://elh.jqgufenzy.top

[R53] 查看文件头与实时尾
来源：http://rke.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ozf.haohaochexian.top

[R54] 比较两个文件
来源：http://zsu.tianlin.xyz

diff a.txt b.txt
来源：http://hcm.zycfv.cn

[R55] 压缩与解压
来源：http://mnb.nwbrower.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ewg.jianghu66.top

[R56] 远程拷贝
来源：http://eua.birdmap.top

scp file user@host:/path/
来源：http://oqc.yanxiufei.cn

[R57] 远程执行命令
来源：http://wyc.snrcjt.cn

ssh user@host 'uptime'
来源：http://rup.gzhubu.top

[R58] 下载文件
来源：http://evz.xuanzx.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hrg.hammf.cn

[R59] 发 POST JSON
来源：http://cre.0kj1m.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oac.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://mpb.fzhhl.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kqf.jqgfzy.top

[R61] 磁盘占用
来源：http://dje.zycfv.cn

df -h;  du -sh *
来源：http://mlm.52xcode.cn

[R62] 找最占空间的文件
来源：http://auo.tianlin.xyz

du -ah . | sort -rh | head -10
来源：http://ysn.vqdsnc.cn

[R63] 内存与进程
来源：http://qyr.cheryme.top

free -h;  ps aux | grep nginx
来源：http://skv.chenjidiqi.icu

[R64] 结束进程
来源：http://zjc.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://qbl.jqgufenzy.top

[R65] 查看端口占用
来源：http://cty.hnqzz.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qpa.shuidangran.top

[R66] 定时任务
来源：http://toy.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://wlq.yj20258888.top

[R67] 生成随机十六进制串
来源：http://pdm.xziqi.cn

openssl rand -hex 16
来源：http://kxw.yuanzhike.top

[R68] 计算文件校验值
来源：http://vti.smart0.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://ucc.yj20258.top

[R69] 生成随机密码
来源：http://tjp.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://dae.hnqzz.top

[R70] 时间戳与互转
来源：http://lww.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://mso.zhongyouzk.top

[R71] 日期格式化
来源：http://lns.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://foq.sufxvd.cn

[R72] 等待端口就绪
来源：http://qgh.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ozy.guannengcc.top

[R73] 分割大日志
来源：http://gxw.ppjwa.cn

split -l 1000 big.log part_
来源：http://vje.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://gax.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vdm.fehbvm.com

[R75] 导出环境变量
来源：http://rcx.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://fed.ctjpmb.com

[R76] 使用临时文件
来源：http://rkx.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ugr.cheryme.top

[R77] 读取用户输入
来源：http://dkf.havefunace.top

read -rp "请输入: " ans
来源：http://iwy.zdbjq.cn

[R78] 交互式菜单
来源：http://zhr.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://edr.sjlbkw.cn

[R79] 解析命令行选项
来源：http://xsw.yj20258.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eya.dashuyun.cn

[R80] 查看脚本执行耗时
来源：http://yhx.tanke756.top

time ./run.sh
来源：http://hdt.haohaochexian.top

================================================================================
来源：http://jvb.nanxuanxn.top

S. C / C++ 专题
来源：http://buz.feifeiyinyue.top

================================================================================
来源：http://ffz.hnqzz.top

[S01] C：Hello World
来源：http://rfj.jyoumei.cn

#include <stdio.h>
来源：http://hth.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cab.zhongyouzk.top

[S02] C：变量与格式化输出
来源：http://bda.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://xum.chenlongwang.top

[S03] C：读入整数
来源：http://pow.andypj.xyz

int x; scanf("%d", &x);
来源：http://bqw.nwbrower.top

[S04] C：字符串复制
来源：http://det.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rzh.hnqzz.top

[S05] C：字符串长度
来源：http://brs.shuidangran.top

strlen(s)
来源：http://hws.ehwqpu.com

[S06] C：字符串比较
来源：http://smc.zhoulong.xyz

strcmp(a, b) == 0
来源：http://adc.shzxlz.cn

[S07] C：数组遍历求和
来源：http://aks.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vje.cheryme.top

[S08] C：动态内存分配与释放
来源：http://zdc.haohaochexian.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tuz.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://mex.shzxlz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nbw.nwbrower.top

[S10] C：指针与解引用
来源：http://eba.yj20258888.top

int *p = &a;  *p = 5;
来源：http://hwl.guannengcc.top

[S11] C：逐行读文件
来源：http://udw.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://phs.jyoumei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xur.jinqigufen.top

fclose(f);
来源：http://apd.shanyushiyangkeji.top

[S12] C：写文件
来源：http://slo.fanxiaobao.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://piy.zhengqikj.top

[S13] C：宏定义
来源：http://rpu.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hmx.bjfxy.top

[S14] C：枚举
来源：http://rpj.yuanzhike.top

enum Color { RED, GREEN, BLUE };
来源：http://qwy.shzxlz.cn

[S15] C：类型转换
来源：http://hmo.chenlongwang.top

(double) a / b
来源：http://xud.yonumen.top

[S16] C：位操作置位
来源：http://igk.daxiang520.top

x |= (1 << 3);
来源：http://tqh.nwbrower.top

[S17] C：安全拼接字符串
来源：http://lco.pengpengdd.cyou

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fyq.fktsv.cn

[S18] C：命令行参数
来源：http://wtk.hammf.cn

int main(int argc, char **argv)
来源：http://adi.tian-w.cn

[S19] C：快速排序
来源：http://vpz.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://fdo.jinghuilouyu.cn

[S20] C：二分查找
来源：http://awu.pycfn.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sxv.zhiwuduotai.top

[S21] C：字符类别判断
来源：http://pty.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://men.gogol.net.cn

[S22] C：字符串转数字
来源：http://bbp.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://bwy.daxiang520.top

[S23] C：随机数
来源：http://fdd.zhiwuduotai.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ohe.hysaishi.cn

[S24] C：获取本地时间
来源：http://ovy.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ymc.nanxinkj.top

[S25] C：内存拷贝
来源：http://dvg.gzhubu.top

memcpy(dst, src, n);
来源：http://qyb.xinyue.icu

[S26] C：内存清零
来源：http://ihs.nanxuanxn.top

memset(a, 0, sizeof a);
来源：http://aks.svipenyu.cn

[S27] C：定义常量
来源：http://ygr.zycfv.cn

const double PI = 3.14159;
来源：http://zcl.fanxiaobao.xyz

[S28] C：静态变量
来源：http://tpq.guannengcc.top

static int counter = 0;
来源：http://avx.svipenyu.cn

[S29] C：变参函数
来源：http://xjw.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gww.bbcook.cn

[S30] C：头文件保护
来源：http://ygl.chenjidiqi.icu

#ifndef X_H
来源：http://nle.meibo888.top

#define X_H
来源：http://ynn.hfpthk.cn

#endif
来源：http://rdv.gzhubu.top

[S31] C++：Hello World
来源：http://bwy.svipenyu.cn

#include <iostream>
来源：http://wru.yj20258.top

int main() { std::cout << "Hello\n"; }
来源：http://uxh.guowangkeji.top

[S32] C++：字符串
来源：http://chm.dashuyun.cn

std::string s = "hi";  s += "!";
来源：http://mpo.vqdsnc.cn

[S33] C++：vector 增删
来源：http://axm.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tfd.wangdashe.top

[S34] C++：遍历 vector
来源：http://btm.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://eps.yueranfly.top

[S35] C++：map
来源：http://aby.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://svy.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://acv.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xjh.xinyue.icu

[S37] C++：set
来源：http://ilw.yvedp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ije.ydjk.org.cn

[S38] C++：排序
来源：http://llx.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://mkh.yj202588.top

[S39] C++：自定义比较器排序
来源：http://ahj.zhixingplan.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://khu.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://nlk.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://amy.ydjk.org.cn

[S41] C++：类与构造函数
来源：http://lrx.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kat.birdmap.top

[S42] C++：继承与虚函数
来源：http://qlf.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://vmn.sjlbkw.cn

[S43] C++：智能指针
来源：http://ahm.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://vqe.zhijiandao.cn

[S44] C++：引用传参
来源：http://vvc.zhaomingkeji.xyz

void inc(int &x) { ++x; }
来源：http://ucf.yanxiufei.cn

[S45] C++：lambda
来源：http://waf.xylfe.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qph.dashuyun.cn

[S46] C++：函数模板
来源：http://ngp.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hqb.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://xtl.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yjl.hnqzz.top

[S48] C++：逐行读文件
来源：http://hsg.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qay.guannengcc.top

while (std::getline(in, line)) { }
来源：http://qhq.gzhubu.top

[S49] C++：写文件
来源：http://zam.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://odw.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://vfu.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wvn.fanxiaobao.xyz

[S51] C++：显式类型转换
来源：http://clf.ybcxt.top

static_cast<double>(a) / b
来源：http://gff.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://eci.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://hoa.hywenlv.cn

[S53] C++：移动语义
来源：http://tbo.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://bzi.jinqigufen.top

[S54] C++：异常处理
来源：http://djb.wangshuangyany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rcl.havefunace.top

[S55] C++：结构化绑定
来源：http://fyx.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kla.iojbl.cn

[S56] C++：optional
来源：http://xfn.guowangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jge.jyoumei.cn

[S57] C++：编译期常量
来源：http://xdk.zhongyouzk.top

constexpr int N = 10;
来源：http://jaz.zhaomingkeji.xyz

[S58] C++：命名空间
来源：http://dgw.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://lse.cdnleiting.top

[S59] C++：静态断言
来源：http://qqa.guannengcc.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tde.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://hjh.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rxl.cucudq.cn

================================================================================
来源：http://kfo.cashguo.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fhh.fengsongda.top

================================================================================
来源：http://hvl.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://jkl.yj20258.top

println("Hello")
来源：http://itu.vqdsnc.cn

[T02] Kotlin：变量
来源：http://jpq.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qxk.guowangkeji.top

[T03] Kotlin：字符串模板
来源：http://glp.zdqjudy.top

"值: $b"
来源：http://ami.chenlongwang.top

[T04] Kotlin：空安全
来源：http://hap.yuanzhike.top

val n: String? = null;  n?.length
来源：http://dzt.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://lvm.ybcxt.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ugo.yvedp.cn

[T06] Kotlin：集合映射
来源：http://mfj.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://zhj.smart0.xyz


<!-- 参考信息 -->