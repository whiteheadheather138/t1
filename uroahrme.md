代发 wailian999

set -euo pipefail
来源：http://edp.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://lxj.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://kqk.ywan-chungtsiang.top

[R03] 只读变量
来源：http://pki.jinqigfzy.top

readonly PI=3.14
来源：http://opw.xuanzx.com

[R04] 位置参数
来源：http://dpx.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wpq.sxryk.cn

[R05] 参数默认值
来源：http://jat.jqgfzy.top

name="${1:-default}"
来源：http://phi.yvedp.cn

[R06] 判断命令是否存在
来源：http://xbt.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wyh.ydzc1.top

[R07] if 判断文件
来源：http://jek.pycfn.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ybo.zhaomingkeji.xyz

[R08] 数值比较
来源：http://ktn.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://pln.ydjk.org.cn

[R09] 字符串比较
来源：http://jqx.hnxiangtu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kzx.hammf.cn

[R10] 正则匹配
来源：http://fnf.vqdsnc.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://frq.pycfn.com

[R11] case 多分支
来源：http://csr.hysaishi.cn

case "$1" in
来源：http://fjm.52xcode.cn

start) echo "启动" ;;
来源：http://rzs.gzhubu.top

stop)  echo "停止" ;;
来源：http://nch.tanke756.top

*)     echo "未知命令" ;;
来源：http://xgj.shanyushiyangtech.top

esac
来源：http://djg.xingfuxueyuan.xyz

[R12] for 遍历文件
来源：http://apg.yuxming.cn

for f in *.txt; do echo "$f"; done
来源：http://zxs.ehwqpu.com

[R13] for 计数循环
来源：http://vkd.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://hlc.yueranfly.top

[R14] C 风格 for
来源：http://igo.yueranfly.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bke.gotoacloud.top

[R15] while 逐行读文件
来源：http://hyf.cdnleiting.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wdk.ctjpmb.com

[R16] until 等待条件
来源：http://gja.nanxuanxn.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bru.hnxiangtu.top

[R17] 数组定义与取值
来源：http://bsu.yuxming.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mkt.hcnkem.com

[R18] 遍历数组
来源：http://nlk.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rxp.hfpthk.cn

[R19] 数组长度
来源：http://xon.jiagoushi.top

echo "${#arr[@]}"
来源：http://jrr.yueranfly.top

[R20] 关联数组（字典）
来源：http://xqu.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kvb.tian-w.cn

[R21] 字符串长度
来源：http://yug.jqgfzy.top

echo "${#s}"
来源：http://bka.fanxiaobao.xyz

[R22] 截取子串
来源：http://hue.52xcode.cn

echo "${s:0:5}"
来源：http://jyg.kuanghao11.cn

[R23] 字符串替换
来源：http://nxs.chenlongwang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ice.cucudq.cn

[R24] 大小写转换
来源：http://mbs.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://iag.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://cww.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ohy.mhx1999.top

[R26] 命令替换
来源：http://qcc.andypj.xyz

now=$(date +%F); echo "$now"
来源：http://eqq.smart0.xyz

[R27] 算术展开
来源：http://xtq.bjfxy.top

echo $((1 + 2 * 3))
来源：http://oij.ybcxt.top

[R28] 浮点运算
来源：http://mdq.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://kgk.yanxiufei.cn

[R29] 定义函数
来源：http://mgc.snrcjt.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ebx.dashuyun.cn

[R30] 函数返回状态码
来源：http://dlj.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://dll.zhijiandao.cn

[R31] 局部变量
来源：http://zql.shangyingyoupin.top

f() { local x=1; echo "$x"; }
来源：http://wuo.jyoumei.cn

[R32] 参数个数校验
来源：http://myu.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://exg.meibo888.top

[R33] 捕获错误并提示行号
来源：http://kur.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dcz.0kj1m.cn

[R34] 退出时清理
来源：http://kgg.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://cmi.jinqigufen.top

[R35] 后台执行并等待
来源：http://msr.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xdd.0kj1m.cn

[R36] 并发执行多个任务
来源：http://xff.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uec.nanxinkj.top

[R37] 把输出赋给变量
来源：http://wbz.yonumen.top

files=$(ls -1)
来源：http://tum.tarul.cn

[R38] 管道串联
来源：http://dvo.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://cpq.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://bzp.snrcjt.cn

cmd > out.log 2>&1
来源：http://wav.cdnleiting.top

[R40] 追加写日志
来源：http://tpp.jiagoushi.top

echo "log" >> out.log
来源：http://faf.hysaishi.cn

[R41] 丢弃输出
来源：http://mab.hfpthk.cn

cmd >/dev/null 2>&1
来源：http://fba.tian-w.cn

[R42] 输入重定向
来源：http://bzi.gogol.net.cn

wc -l < a.txt
来源：http://dnl.cdnleiting.top

[R43] 按名字查找文件
来源：http://wzh.9152youxi.cn

find . -name "*.log" -type f
来源：http://xdk.wangdashe.top

[R44] 按修改时间查找
来源：http://gdv.nanxuanxn.top

find . -mtime -7 -type f
来源：http://tck.jlsjyb.cn

[R45] 批量删除
来源：http://nep.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://jpu.sufxvd.cn

[R46] 递归替换文件内容
来源：http://iga.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://czd.havefunace.top

[R47] sed 单行替换
来源：http://tfl.sxryk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cxp.hfpthk.cn

[R48] awk 取指定列
来源：http://mlj.zycfv.cn

awk '{print $1, $3}' a.txt
来源：http://sbd.sufxvd.cn

[R49] awk 带条件
来源：http://ptw.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vcr.gaohongyu789.top

[R50] awk 求和
来源：http://qny.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://koq.pycfn.com

[R51] 排序去重取前几
来源：http://wej.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://urn.guannengcc.top

[R52] 统计行数
来源：http://dij.ydjk.org.cn

wc -l a.txt
来源：http://qvh.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://xkr.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://osw.yangfankeji.com

[R54] 比较两个文件
来源：http://ohl.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://myq.hywenlv.cn

[R55] 压缩与解压
来源：http://jyn.fehbvm.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://psu.haohaochexian.top

[R56] 远程拷贝
来源：http://dzu.zhijiandao.cn

scp file user@host:/path/
来源：http://nat.sjlbkw.cn

[R57] 远程执行命令
来源：http://rni.ywan-chungtsiang.top

ssh user@host 'uptime'
来源：http://phw.yj20258888.top

[R58] 下载文件
来源：http://fnz.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fhi.tanke756.top

[R59] 发 POST JSON
来源：http://scq.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://adp.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://aqe.cqqwz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yac.sysykeji.top

[R61] 磁盘占用
来源：http://ptz.ehwqpu.com

df -h;  du -sh *
来源：http://bvf.pycfn.com

[R62] 找最占空间的文件
来源：http://rgo.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://rje.fehbvm.com

[R63] 内存与进程
来源：http://mjr.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://tjo.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://oom.tanke756.top

kill -9 $(pgrep -f app.py)
来源：http://rzy.ydzc1.top

[R65] 查看端口占用
来源：http://msv.havefunace.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zag.hongshengwenyu.top

[R66] 定时任务
来源：http://mwb.jinghuilouyu.cn

crontab -e;  crontab -l
来源：http://qzq.ehwqpu.com

[R67] 生成随机十六进制串
来源：http://tfv.ivvv.top

openssl rand -hex 16
来源：http://jxd.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://spp.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tbk.yvedp.cn

[R69] 生成随机密码
来源：http://zij.yj20258888.top

head -c 16 /dev/urandom | base64
来源：http://qut.xuanzx.com

[R70] 时间戳与互转
来源：http://kos.jianghu66.top

date +%s;  date -d @1700000000
来源：http://eoh.tianlin.xyz

[R71] 日期格式化
来源：http://vif.pengpengdd.cyou

date +"%Y-%m-%d %H:%M:%S"
来源：http://iwo.yueranfly.top

[R72] 等待端口就绪
来源：http://ptb.jiagoushi.top

until nc -z localhost 3306; do sleep 1; done
来源：http://alz.wangshuangyany.cn

[R73] 分割大日志
来源：http://dsh.smart0.xyz

split -l 1000 big.log part_
来源：http://jcm.pycfn.com

[R74] 批量重命名
来源：http://nwn.yuxming.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://clp.chenzaomai.com

[R75] 导出环境变量
来源：http://ptr.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://fuo.gotoacloud.top

[R76] 使用临时文件
来源：http://ekn.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hdc.aibaodan.cn

[R77] 读取用户输入
来源：http://tep.nanxuanxn.top

read -rp "请输入: " ans
来源：http://wha.gogol.net.cn

[R78] 交互式菜单
来源：http://jzx.chenzaomai.com

select opt in a b c; do echo "$opt"; break; done
来源：http://rqw.hesvh.cn

[R79] 解析命令行选项
来源：http://sbw.zhongyouzk.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tdi.jinghuilouyu.cn

[R80] 查看脚本执行耗时
来源：http://smz.feifeiyinyue.top

time ./run.sh
来源：http://ado.c1oappe.top

================================================================================
来源：http://egg.jinqigufen.top

S. C / C++ 专题
来源：http://jnb.zdbjq.cn

================================================================================
来源：http://xkc.daria6918.cn

[S01] C：Hello World
来源：http://ddy.jinqigufen.top

#include <stdio.h>
来源：http://gmp.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://plp.daria6918.cn

[S02] C：变量与格式化输出
来源：http://mqc.smart0.xyz

int a = 10; printf("%d\n", a);
来源：http://gty.0kj1m.cn

[S03] C：读入整数
来源：http://kca.316326.xyz

int x; scanf("%d", &x);
来源：http://avn.haohaochexian.top

[S04] C：字符串复制
来源：http://fsh.hammf.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rym.chenlongwang.top

[S05] C：字符串长度
来源：http://bnv.0kj1m.cn

strlen(s)
来源：http://afr.birdmap.top

[S06] C：字符串比较
来源：http://lsd.xziqi.cn

strcmp(a, b) == 0
来源：http://rkp.daxiang520.top

[S07] C：数组遍历求和
来源：http://tuo.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ohi.tianlin.xyz

[S08] C：动态内存分配与释放
来源：http://iml.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hyx.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://wvu.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jvq.jlsjyb.cn

[S10] C：指针与解引用
来源：http://kbd.hesvh.cn

int *p = &a;  *p = 5;
来源：http://cya.xinyue.icu

[S11] C：逐行读文件
来源：http://ifi.fktsv.cn

FILE *f = fopen("a.txt", "r");
来源：http://ixp.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dvx.gzhubu.top

fclose(f);
来源：http://qmj.ppjwa.cn

[S12] C：写文件
来源：http://slf.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rks.nwbrower.top

[S13] C：宏定义
来源：http://ocj.fktsv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://orz.zycfv.cn

[S14] C：枚举
来源：http://tnl.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://ege.jyoumei.cn

[S15] C：类型转换
来源：http://yju.hesvh.cn

(double) a / b
来源：http://vbj.mhx1999.top

[S16] C：位操作置位
来源：http://hoi.jlsjyb.cn

x |= (1 << 3);
来源：http://djd.zhixingplan.top

[S17] C：安全拼接字符串
来源：http://izl.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gmf.jinqigufen.top

[S18] C：命令行参数
来源：http://vlc.aibaodan.cn

int main(int argc, char **argv)
来源：http://zue.sufxvd.cn

[S19] C：快速排序
来源：http://wny.cqqwz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dbw.snrcjt.cn

[S20] C：二分查找
来源：http://ndy.cashguo.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cvv.wangdashe.top

[S21] C：字符类别判断
来源：http://hcf.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cxm.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://pwt.jqgfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://otm.yangfankeji.com

[S23] C：随机数
来源：http://jnh.ybcxt.top

srand(time(NULL));  int r = rand() % 100;
来源：http://aih.vehdjk.com

[S24] C：获取本地时间
来源：http://pjx.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://art.ppjwa.cn

[S25] C：内存拷贝
来源：http://qbp.meibo888.top

memcpy(dst, src, n);
来源：http://wfp.epnwcf.com

[S26] C：内存清零
来源：http://cwm.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://vqc.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://gfq.aizwys.cn

const double PI = 3.14159;
来源：http://gjc.zycfv.cn

[S28] C：静态变量
来源：http://iut.daria6918.cn

static int counter = 0;
来源：http://rng.pengpengdd.cyou

[S29] C：变参函数
来源：http://aou.xuetiantiany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mri.wangshuangyany.cn

[S30] C：头文件保护
来源：http://vmn.vqdsnc.cn

#ifndef X_H
来源：http://ltm.fanxiaobao.xyz

#define X_H
来源：http://qin.fehbvm.com

#endif
来源：http://frn.meibo888.top

[S31] C++：Hello World
来源：http://kml.cucudq.cn

#include <iostream>
来源：http://yzw.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://nej.fehbvm.com

[S32] C++：字符串
来源：http://exc.hnxiangtu.top

std::string s = "hi";  s += "!";
来源：http://dgj.yueranfly.top

[S33] C++：vector 增删
来源：http://cng.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dgv.svipenyu.cn

[S34] C++：遍历 vector
来源：http://amc.tianlin.xyz

for (auto &x : v) { std::cout << x; }
来源：http://rey.jinqigufen.top

[S35] C++：map
来源：http://dyt.yueranfly.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fvl.sysykeji.top

[S36] C++：unordered_map
来源：http://xgf.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nnx.tian-w.cn

[S37] C++：set
来源：http://imh.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rdx.yuanzhike.top

[S38] C++：排序
来源：http://hko.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://xca.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://oph.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tod.cqqwz.cn

[S40] C++：查找元素
来源：http://omy.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mhp.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://lpl.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fmd.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://jjf.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://qrx.hammf.cn

[S43] C++：智能指针
来源：http://xth.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://lwi.yongpay.top

[S44] C++：引用传参
来源：http://rie.ydzc1.top

void inc(int &x) { ++x; }
来源：http://ifa.uphjek.com

[S45] C++：lambda
来源：http://oxl.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://pzk.svipenyu.cn

[S46] C++：函数模板
来源：http://lqv.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://svq.dianchejie.cn

[S47] C++：结构化绑定遍历
来源：http://htb.hongshengwenyu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vdc.c1oappe.top

[S48] C++：逐行读文件
来源：http://yxv.jinghuilouyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://keo.yangfankeji.com

while (std::getline(in, line)) { }
来源：http://orc.yuxming.cn

[S49] C++：写文件
来源：http://wmp.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pty.jianghu66.top

[S50] C++：格式化数字
来源：http://tag.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://axs.jlsjyb.cn

[S51] C++：显式类型转换
来源：http://spm.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://xee.ctjpmb.com

[S52] C++：const 与 noexcept
来源：http://ztb.fktsv.cn

int size() const noexcept { return n_; }
来源：http://wxg.hfpthk.cn

[S53] C++：移动语义
来源：http://jdp.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://uyy.jinqigfzy.top

[S54] C++：异常处理
来源：http://ign.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dkn.wangdashe.top

[S55] C++：结构化绑定
来源：http://hnq.ppjwa.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yxj.tanke756.top

[S56] C++：optional
来源：http://asd.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ioo.cucudq.cn

[S57] C++：编译期常量
来源：http://zkd.birdmap.top

constexpr int N = 10;
来源：http://wfp.yfazqb.com

[S58] C++：命名空间
来源：http://whc.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://fjw.yanxiufei.cn

[S59] C++：静态断言
来源：http://hnm.jinqigufen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lbo.sweek.top

[S60] C++：遍历并删除元素
来源：http://dxs.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://deg.feifeiyinyue.top

================================================================================
来源：http://qdc.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yjb.iojbl.cn

================================================================================
来源：http://gtp.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://lvz.dianchejie.cn

println("Hello")
来源：http://kis.jiagoushi.top

[T02] Kotlin：变量
来源：http://zom.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wvr.nanxinkj.top


<!-- 参考信息 -->