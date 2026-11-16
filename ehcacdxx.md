代发 wailian999

set -euo pipefail
来源：http://suj.jlsjyb.cn

[R02] 变量赋值与使用
来源：http://bns.cucudq.cn

name="Tom"; echo "$name"
来源：http://kdp.sysykeji.top

[R03] 只读变量
来源：http://oug.ydjk.org.cn

readonly PI=3.14
来源：http://tvc.cdnleiting.top

[R04] 位置参数
来源：http://itk.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iht.sjlbkw.cn

[R05] 参数默认值
来源：http://zrf.nanxuanxn.top

name="${1:-default}"
来源：http://vsm.jinqigufen.top

[R06] 判断命令是否存在
来源：http://egz.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://frt.quarkkingdee.top

[R07] if 判断文件
来源：http://pdo.fengsongda.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hpr.zhijiandao.cn

[R08] 数值比较
来源：http://fry.epnwcf.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ead.guowangkeji.top

[R09] 字符串比较
来源：http://nsh.zhongyouzk.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zot.chenlongwang.top

[R10] 正则匹配
来源：http://crj.shzxlz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sqr.9152youxi.cn

[R11] case 多分支
来源：http://xvx.gotoacloud.top

case "$1" in
来源：http://eyv.hcnkem.com

start) echo "启动" ;;
来源：http://yky.hfpthk.cn

stop)  echo "停止" ;;
来源：http://klm.tanke756.top

*)     echo "未知命令" ;;
来源：http://lag.pengpengdd.cyou

esac
来源：http://uwx.dashuyun.cn

[R12] for 遍历文件
来源：http://teh.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://ldd.yongpay.top

[R13] for 计数循环
来源：http://owu.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://gxe.svipenyu.cn

[R14] C 风格 for
来源：http://ttj.shanyushiyangtech.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jyi.iojbl.cn

[R15] while 逐行读文件
来源：http://lhq.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://onz.yuanzhike.top

[R16] until 等待条件
来源：http://xmz.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ljd.andypj.xyz

[R17] 数组定义与取值
来源：http://ick.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bgk.svipenyu.cn

[R18] 遍历数组
来源：http://ori.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mob.jinqigufen.top

[R19] 数组长度
来源：http://qih.tanke756.top

echo "${#arr[@]}"
来源：http://dhn.aibaodan.cn

[R20] 关联数组（字典）
来源：http://uqb.sxryk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://goj.bjfxy.top

[R21] 字符串长度
来源：http://hcj.zdbjq.cn

echo "${#s}"
来源：http://mdo.zhoulong.xyz

[R22] 截取子串
来源：http://kdy.fehbvm.com

echo "${s:0:5}"
来源：http://yyp.jianghu66.top

[R23] 字符串替换
来源：http://ndd.gaohongyu789.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hqs.xuanzx.com

[R24] 大小写转换
来源：http://jkw.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://yhc.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://vmb.xuetiantiany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://exz.hywenlv.cn

[R26] 命令替换
来源：http://ppt.tanke756.top

now=$(date +%F); echo "$now"
来源：http://uua.cashguo.top

[R27] 算术展开
来源：http://gjt.hesvh.cn

echo $((1 + 2 * 3))
来源：http://gtk.iojbl.cn

[R28] 浮点运算
来源：http://ysm.ybcxt.top

echo "scale=2; 10/3" | bc
来源：http://gob.quarkkingdee.top

[R29] 定义函数
来源：http://pbm.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dqg.yj20258888.top

[R30] 函数返回状态码
来源：http://zdd.jinqigufen.top

f() { return 0; }; f || echo "失败了"
来源：http://crq.fktsv.cn

[R31] 局部变量
来源：http://uvt.hfpthk.cn

f() { local x=1; echo "$x"; }
来源：http://eux.haohaochexian.top

[R32] 参数个数校验
来源：http://nzq.xziqi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ukd.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://qxy.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tfk.wangshuangyany.cn

[R34] 退出时清理
来源：http://qvg.jinqigfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://jvk.bbcook.cn

[R35] 后台执行并等待
来源：http://lzt.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nrn.yueranfly.top

[R36] 并发执行多个任务
来源：http://ehs.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fkv.cucudq.cn

[R37] 把输出赋给变量
来源：http://vfa.bbcook.cn

files=$(ls -1)
来源：http://ppj.cucudq.cn

[R38] 管道串联
来源：http://krj.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://nju.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://vim.hcnkem.com

cmd > out.log 2>&1
来源：http://dah.hysaishi.cn

[R40] 追加写日志
来源：http://xba.epnwcf.com

echo "log" >> out.log
来源：http://jnd.hnxiangtu.top

[R41] 丢弃输出
来源：http://dbd.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://zrz.yvedp.cn

[R42] 输入重定向
来源：http://daw.zhoulong.xyz

wc -l < a.txt
来源：http://dhk.guannengcc.top

[R43] 按名字查找文件
来源：http://gey.bbcook.cn

find . -name "*.log" -type f
来源：http://rda.zhijiandao.cn

[R44] 按修改时间查找
来源：http://sll.zhoulong.xyz

find . -mtime -7 -type f
来源：http://tam.tarul.cn

[R45] 批量删除
来源：http://dyo.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://mjc.hfpthk.cn

[R46] 递归替换文件内容
来源：http://hwo.havefunace.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pyb.meibo888.top

[R47] sed 单行替换
来源：http://xgl.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://wuz.redwolf501.top

[R48] awk 取指定列
来源：http://rkt.sweek.top

awk '{print $1, $3}' a.txt
来源：http://tyg.xuetiantiany.cn

[R49] awk 带条件
来源：http://pvj.hammf.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gpe.cucudq.cn

[R50] awk 求和
来源：http://pzb.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://tjo.zhengqikj.top

[R51] 排序去重取前几
来源：http://tmz.zhongyouzk.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sia.sweek.top

[R52] 统计行数
来源：http://jsr.yuanzhike.top

wc -l a.txt
来源：http://flj.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://tch.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kma.tian-w.cn

[R54] 比较两个文件
来源：http://ghn.sjlbkw.cn

diff a.txt b.txt
来源：http://ugg.vehdjk.com

[R55] 压缩与解压
来源：http://lzn.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hzk.yj20258.top

[R56] 远程拷贝
来源：http://ers.fktsv.cn

scp file user@host:/path/
来源：http://rxq.xuetiantiany.cn

[R57] 远程执行命令
来源：http://hda.xinyue.icu

ssh user@host 'uptime'
来源：http://twc.fengsongda.top

[R58] 下载文件
来源：http://bdk.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yfv.jinqigfzy.top

[R59] 发 POST JSON
来源：http://lnz.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wcc.zdbjq.cn

[R60] 只看 HTTP 状态码
来源：http://dza.xuanzx.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tbg.smart0.xyz

[R61] 磁盘占用
来源：http://pez.mhx1999.top

df -h;  du -sh *
来源：http://rgk.hysaishi.cn

[R62] 找最占空间的文件
来源：http://bxa.yfazqb.com

du -ah . | sort -rh | head -10
来源：http://aqt.quarkkingdee.top

[R63] 内存与进程
来源：http://kli.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://lnj.yuxming.cn

[R64] 结束进程
来源：http://rdj.cqqwz.cn

kill -9 $(pgrep -f app.py)
来源：http://mho.tian-w.cn

[R65] 查看端口占用
来源：http://kok.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jny.tian-w.cn

[R66] 定时任务
来源：http://qqi.vqdsnc.cn

crontab -e;  crontab -l
来源：http://lga.yj20258.top

[R67] 生成随机十六进制串
来源：http://rht.fehbvm.com

openssl rand -hex 16
来源：http://glm.jlsjyb.cn

[R68] 计算文件校验值
来源：http://tpa.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xrv.sjlbkw.cn

[R69] 生成随机密码
来源：http://ala.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://vir.yfazqb.com

[R70] 时间戳与互转
来源：http://geu.hammf.cn

date +%s;  date -d @1700000000
来源：http://kno.fktsv.cn

[R71] 日期格式化
来源：http://qie.nanxinkj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nem.0kj1m.cn

[R72] 等待端口就绪
来源：http://iou.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cyo.zhiwuduotai.top

[R73] 分割大日志
来源：http://qrn.xingfuxueyuan.xyz

split -l 1000 big.log part_
来源：http://svt.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://ile.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ukb.hywenlv.cn

[R75] 导出环境变量
来源：http://yay.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://dcs.zhoulong.xyz

[R76] 使用临时文件
来源：http://seg.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jlb.zhongyouzk.top

[R77] 读取用户输入
来源：http://giq.dianchejie.cn

read -rp "请输入: " ans
来源：http://ibm.mhx1999.top

[R78] 交互式菜单
来源：http://rfu.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zgs.fzhhl.top

[R79] 解析命令行选项
来源：http://uzz.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://weg.hammf.cn

[R80] 查看脚本执行耗时
来源：http://gyu.hammf.cn

time ./run.sh
来源：http://lmp.xuanzx.com

================================================================================
来源：http://cgo.fzhhl.top

S. C / C++ 专题
来源：http://xot.sysykeji.top

================================================================================
来源：http://sux.gaohongyu789.top

[S01] C：Hello World
来源：http://fqx.zycfv.cn

#include <stdio.h>
来源：http://gen.jiagoushi.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cta.wangdashe.top

[S02] C：变量与格式化输出
来源：http://mkd.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://dxf.316326.xyz

[S03] C：读入整数
来源：http://vbo.zycfv.cn

int x; scanf("%d", &x);
来源：http://nzn.zdqjudy.top

[S04] C：字符串复制
来源：http://qfp.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://mgk.bjfxy.top

[S05] C：字符串长度
来源：http://lvq.yj202588.top

strlen(s)
来源：http://wcc.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://owk.hammf.cn

strcmp(a, b) == 0
来源：http://gnm.xuanzx.com

[S07] C：数组遍历求和
来源：http://bpn.gaohongyu789.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gis.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://vie.zhiwuduotai.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nug.shanyushiyangkeji.top

[S09] C：结构体定义与初始化
来源：http://yug.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://isj.cdnleiting.top

[S10] C：指针与解引用
来源：http://ffa.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://hys.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://nge.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://zhk.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://lkv.yuxming.cn

fclose(f);
来源：http://dly.feifeiyinyue.top

[S12] C：写文件
来源：http://qst.cheryme.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://khh.andypj.xyz

[S13] C：宏定义
来源：http://irg.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tpd.jqgfzy.top

[S14] C：枚举
来源：http://ulr.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://qsr.gzhubu.top

[S15] C：类型转换
来源：http://kpd.epnwcf.com

(double) a / b
来源：http://amv.tianlin.xyz

[S16] C：位操作置位
来源：http://led.gaohongyu789.top

x |= (1 << 3);
来源：http://vsx.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://qtb.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://otp.ivvv.top

[S18] C：命令行参数
来源：http://ueh.cashguo.top

int main(int argc, char **argv)
来源：http://jlp.jianghu66.top

[S19] C：快速排序
来源：http://gxd.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://tmb.fzhhl.top

[S20] C：二分查找
来源：http://zus.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rbr.shangyingyoupin.top

[S21] C：字符类别判断
来源：http://amu.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dkh.yuxming.cn

[S22] C：字符串转数字
来源：http://oke.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://ust.zhoulong.xyz

[S23] C：随机数
来源：http://pgn.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wwg.hywenlv.cn

[S24] C：获取本地时间
来源：http://idk.52xcode.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xwu.cdnleiting.top

[S25] C：内存拷贝
来源：http://pke.nanxinkj.top

memcpy(dst, src, n);
来源：http://aok.cashguo.top

[S26] C：内存清零
来源：http://eec.ivvv.top

memset(a, 0, sizeof a);
来源：http://kou.andypj.xyz

[S27] C：定义常量
来源：http://yej.cqqwz.cn

const double PI = 3.14159;
来源：http://bbe.gotoacloud.top

[S28] C：静态变量
来源：http://pan.ydjk.org.cn

static int counter = 0;
来源：http://svn.ydjk.org.cn

[S29] C：变参函数
来源：http://tzz.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qyd.gotoacloud.top

[S30] C：头文件保护
来源：http://sdq.hywenlv.cn

#ifndef X_H
来源：http://kpr.shzxlz.cn

#define X_H
来源：http://frt.quarkkingdee.top

#endif
来源：http://uwp.yonumen.top

[S31] C++：Hello World
来源：http://hcp.iojbl.cn

#include <iostream>
来源：http://jlg.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://jgn.xuetiantiany.cn

[S32] C++：字符串
来源：http://amt.havefunace.top

std::string s = "hi";  s += "!";
来源：http://gcs.birdmap.top

[S33] C++：vector 增删
来源：http://rtb.bjfxy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kgt.bjfxy.top

[S34] C++：遍历 vector
来源：http://jku.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://kod.cqqwz.cn

[S35] C++：map
来源：http://osl.hnqzz.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yxx.fehbvm.com

[S36] C++：unordered_map
来源：http://rvx.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hqf.gaohongyu789.top

[S37] C++：set
来源：http://gzn.gzhubu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bdm.guowangkeji.top

[S38] C++：排序
来源：http://qkh.pycfn.com

std::sort(v.begin(), v.end());
来源：http://sxd.ppjwa.cn

[S39] C++：自定义比较器排序
来源：http://izh.hesvh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wkv.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://gfx.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nka.guowangkeji.top

[S41] C++：类与构造函数
来源：http://ang.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qlk.zhijiandao.cn

[S42] C++：继承与虚函数
来源：http://yzt.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://vtb.cheryme.top

[S43] C++：智能指针
来源：http://tpg.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://gys.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://cnr.bjfxy.top

void inc(int &x) { ++x; }
来源：http://msz.316326.xyz

[S45] C++：lambda
来源：http://aea.c1oappe.top

auto add = [](int a, int b) { return a + b; };
来源：http://cjm.ppjwa.cn

[S46] C++：函数模板
来源：http://wvx.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nkx.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://zkw.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bby.vehdjk.com

[S48] C++：逐行读文件
来源：http://sbh.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ozr.nwbrower.top

while (std::getline(in, line)) { }
来源：http://vtd.sufxvd.cn

[S49] C++：写文件
来源：http://zte.hnqzz.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xla.yj202588.top

[S50] C++：格式化数字
来源：http://jlz.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dht.jyoumei.cn

[S51] C++：显式类型转换
来源：http://eoc.xylfe.cn

static_cast<double>(a) / b
来源：http://eci.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://cys.nwbrower.top

int size() const noexcept { return n_; }
来源：http://lif.svipenyu.cn

[S53] C++：移动语义
来源：http://uge.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://pry.hnxiangtu.top

[S54] C++：异常处理
来源：http://vjt.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rnr.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://hor.hysaishi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cns.ehwqpu.com

[S56] C++：optional
来源：http://qvu.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://glc.yuxming.cn

[S57] C++：编译期常量
来源：http://spa.birdmap.top

constexpr int N = 10;
来源：http://fsm.c1oappe.top

[S58] C++：命名空间
来源：http://iqe.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://whi.zhaomingkeji.xyz

[S59] C++：静态断言
来源：http://fpa.iojbl.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ubu.ydzc1.top

[S60] C++：遍历并删除元素
来源：http://piw.zhiwuduotai.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gmp.chenlongwang.top

================================================================================
来源：http://gsq.yj20258.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xkk.dianchejie.cn

================================================================================
来源：http://ucr.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://fvm.ctjpmb.com

println("Hello")
来源：http://jhi.bbcook.cn

[T02] Kotlin：变量
来源：http://vop.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sin.mhx1999.top


<!-- 参考信息 -->