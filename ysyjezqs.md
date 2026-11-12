代发 wailian999

set -euo pipefail
来源：http://ygi.hesvh.cn

[R02] 变量赋值与使用
来源：http://svo.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://ksw.yj20258.top

[R03] 只读变量
来源：http://lly.hnxiangtu.top

readonly PI=3.14
来源：http://xfe.ybcxt.top

[R04] 位置参数
来源：http://tmw.yuxming.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eoq.fehbvm.com

[R05] 参数默认值
来源：http://ypr.ivvv.top

name="${1:-default}"
来源：http://fki.zhijiandao.cn

[R06] 判断命令是否存在
来源：http://unb.fktsv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://udb.havefunace.top

[R07] if 判断文件
来源：http://lut.yonumen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wkf.fktsv.cn

[R08] 数值比较
来源：http://wtq.smart0.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://xuv.sysykeji.top

[R09] 字符串比较
来源：http://cjx.wangshuangyany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pos.yangfankeji.com

[R10] 正则匹配
来源：http://rbt.sxryk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://plu.hesvh.cn

[R11] case 多分支
来源：http://gax.cheryme.top

case "$1" in
来源：http://ygv.tian-w.cn

start) echo "启动" ;;
来源：http://gro.havefunace.top

stop)  echo "停止" ;;
来源：http://pye.tianlin.xyz

*)     echo "未知命令" ;;
来源：http://qkl.smart0.xyz

esac
来源：http://yes.316326.xyz

[R12] for 遍历文件
来源：http://fcv.nanxuanxn.top

for f in *.txt; do echo "$f"; done
来源：http://vuz.daria6918.cn

[R13] for 计数循环
来源：http://xcv.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://jdh.gzhubu.top

[R14] C 风格 for
来源：http://qdk.52xcode.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://alv.hywenlv.cn

[R15] while 逐行读文件
来源：http://wwh.hongshengwenyu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://orx.gzhubu.top

[R16] until 等待条件
来源：http://wpx.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yny.gotoacloud.top

[R17] 数组定义与取值
来源：http://kcn.yj202588.top

arr=(a b c); echo "${arr[0]}"
来源：http://avj.epnwcf.com

[R18] 遍历数组
来源：http://anl.yongpay.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bcl.jiagoushi.top

[R19] 数组长度
来源：http://hfp.cucudq.cn

echo "${#arr[@]}"
来源：http://tcp.pengpengdd.cyou

[R20] 关联数组（字典）
来源：http://kfj.meibo888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://awm.tianlin.xyz

[R21] 字符串长度
来源：http://xet.c1oappe.top

echo "${#s}"
来源：http://vjb.52xcode.cn

[R22] 截取子串
来源：http://oei.zdbjq.cn

echo "${s:0:5}"
来源：http://tyh.jinqigufen.top

[R23] 字符串替换
来源：http://apk.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ovz.xuetiantiany.cn

[R24] 大小写转换
来源：http://mcm.yj202588.top

echo "${s^^}"; echo "${s,,}"
来源：http://qqt.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://bjm.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mmm.jiagoushi.top

[R26] 命令替换
来源：http://cxj.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://gzi.sysykeji.top

[R27] 算术展开
来源：http://uuj.wangdashe.top

echo $((1 + 2 * 3))
来源：http://jnh.hnxiangtu.top

[R28] 浮点运算
来源：http://vjp.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://gze.shanyushiyangtech.top

[R29] 定义函数
来源：http://wce.snrcjt.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wmm.snrcjt.cn

[R30] 函数返回状态码
来源：http://zql.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://rrd.vehdjk.com

[R31] 局部变量
来源：http://jaz.xuanzx.com

f() { local x=1; echo "$x"; }
来源：http://afz.yj20258888.top

[R32] 参数个数校验
来源：http://maa.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://toy.yonumen.top

[R33] 捕获错误并提示行号
来源：http://ujz.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zuw.xylfe.cn

[R34] 退出时清理
来源：http://ueb.epnwcf.com

trap 'rm -f "$tmp"' EXIT
来源：http://sjq.havefunace.top

[R35] 后台执行并等待
来源：http://wna.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://hkr.fehbvm.com

[R36] 并发执行多个任务
来源：http://ebi.zhongyouzk.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lbd.gogol.net.cn

[R37] 把输出赋给变量
来源：http://iot.epnwcf.com

files=$(ls -1)
来源：http://kik.daria6918.cn

[R38] 管道串联
来源：http://bzz.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://sbt.shangyingyoupin.top

[R39] 重定向标准输出与错误
来源：http://pal.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://cli.ydzc1.top

[R40] 追加写日志
来源：http://jiw.jlsjyb.cn

echo "log" >> out.log
来源：http://qwr.9152youxi.cn

[R41] 丢弃输出
来源：http://qkw.ydzc1.top

cmd >/dev/null 2>&1
来源：http://tmc.yueranfly.top

[R42] 输入重定向
来源：http://syw.havefunace.top

wc -l < a.txt
来源：http://hni.cdnleiting.top

[R43] 按名字查找文件
来源：http://ixa.yanxiufei.cn

find . -name "*.log" -type f
来源：http://bbw.gogol.net.cn

[R44] 按修改时间查找
来源：http://obx.zhoulong.xyz

find . -mtime -7 -type f
来源：http://qkf.ywan-chungtsiang.top

[R45] 批量删除
来源：http://uvj.bbcook.cn

find . -name "*.tmp" -delete
来源：http://egy.andypj.xyz

[R46] 递归替换文件内容
来源：http://izk.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://utr.vehdjk.com

[R47] sed 单行替换
来源：http://hrl.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ark.fengsongda.top

[R48] awk 取指定列
来源：http://jnn.yj20258888.top

awk '{print $1, $3}' a.txt
来源：http://mxd.jyoumei.cn

[R49] awk 带条件
来源：http://jzq.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ycl.hammf.cn

[R50] awk 求和
来源：http://ayk.uphjek.com

awk '{s += $2} END {print s}' a.txt
来源：http://ikp.nwbrower.top

[R51] 排序去重取前几
来源：http://ysg.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://itc.yueranfly.top

[R52] 统计行数
来源：http://bmm.sweek.top

wc -l a.txt
来源：http://ghk.tanke756.top

[R53] 查看文件头与实时尾
来源：http://neb.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mlr.fengsongda.top

[R54] 比较两个文件
来源：http://awz.yj20258888.top

diff a.txt b.txt
来源：http://qpp.haohaochexian.top

[R55] 压缩与解压
来源：http://kip.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dco.bbcook.cn

[R56] 远程拷贝
来源：http://qmu.gzhubu.top

scp file user@host:/path/
来源：http://vbn.shangyingyoupin.top

[R57] 远程执行命令
来源：http://yxs.316326.xyz

ssh user@host 'uptime'
来源：http://dxa.zhoulong.xyz

[R58] 下载文件
来源：http://tur.vehdjk.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ypu.hnqzz.top

[R59] 发 POST JSON
来源：http://cfb.xinyue.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://svu.fzhhl.top

[R60] 只看 HTTP 状态码
来源：http://noz.316326.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rds.zdqjudy.top

[R61] 磁盘占用
来源：http://jry.vehdjk.com

df -h;  du -sh *
来源：http://dim.haohaochexian.top

[R62] 找最占空间的文件
来源：http://geq.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://gik.cqqwz.cn

[R63] 内存与进程
来源：http://qgo.cashguo.top

free -h;  ps aux | grep nginx
来源：http://bsv.quarkkingdee.top

[R64] 结束进程
来源：http://tcs.shuidangran.top

kill -9 $(pgrep -f app.py)
来源：http://hsy.dianchejie.cn

[R65] 查看端口占用
来源：http://wcm.tian-w.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bha.yuxming.cn

[R66] 定时任务
来源：http://wns.xylfe.cn

crontab -e;  crontab -l
来源：http://yez.yuxming.cn

[R67] 生成随机十六进制串
来源：http://otr.nanxinkj.top

openssl rand -hex 16
来源：http://qjq.guowangkeji.top

[R68] 计算文件校验值
来源：http://rov.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nrj.yfazqb.com

[R69] 生成随机密码
来源：http://iks.cheryme.top

head -c 16 /dev/urandom | base64
来源：http://aux.cdnleiting.top

[R70] 时间戳与互转
来源：http://kds.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://jbp.ppjwa.cn

[R71] 日期格式化
来源：http://aex.zhijiandao.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://axg.ivvv.top

[R72] 等待端口就绪
来源：http://gzp.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nga.ybcxt.top

[R73] 分割大日志
来源：http://gjx.meibo888.top

split -l 1000 big.log part_
来源：http://zda.ivvv.top

[R74] 批量重命名
来源：http://car.epnwcf.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xqw.jqgfzy.top

[R75] 导出环境变量
来源：http://lea.fengsongda.top

export PATH="$HOME/bin:$PATH"
来源：http://oyq.jlsjyb.cn

[R76] 使用临时文件
来源：http://nob.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xpg.sufxvd.cn

[R77] 读取用户输入
来源：http://goi.epnwcf.com

read -rp "请输入: " ans
来源：http://azt.hnxiangtu.top

[R78] 交互式菜单
来源：http://lhz.cheryme.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gme.tanke756.top

[R79] 解析命令行选项
来源：http://ioh.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://olz.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://lew.gzhubu.top

time ./run.sh
来源：http://mcl.zhongyouzk.top

================================================================================
来源：http://zfn.jqgufenzy.top

S. C / C++ 专题
来源：http://kzl.dashuyun.cn

================================================================================
来源：http://gvr.0kj1m.cn

[S01] C：Hello World
来源：http://onj.birdmap.top

#include <stdio.h>
来源：http://nnw.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qcp.zycfv.cn

[S02] C：变量与格式化输出
来源：http://wpy.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://yiu.sxryk.cn

[S03] C：读入整数
来源：http://mca.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://qgu.yonumen.top

[S04] C：字符串复制
来源：http://bpa.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://ovj.bbcook.cn

[S05] C：字符串长度
来源：http://ekb.yuxming.cn

strlen(s)
来源：http://kof.zhixingplan.top

[S06] C：字符串比较
来源：http://ieq.yj20258888.top

strcmp(a, b) == 0
来源：http://eam.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://aew.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://unh.fengsongda.top

[S08] C：动态内存分配与释放
来源：http://lhb.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pbi.xuetiantiany.cn

[S09] C：结构体定义与初始化
来源：http://eyf.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://urv.xinyue.icu

[S10] C：指针与解引用
来源：http://shj.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://knw.daxiang520.top

[S11] C：逐行读文件
来源：http://gwi.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://swt.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jox.cdnleiting.top

fclose(f);
来源：http://dcv.bbcook.cn

[S12] C：写文件
来源：http://gwl.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xhn.gzhubu.top

[S13] C：宏定义
来源：http://exw.jinqigfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://emb.daxiang520.top

[S14] C：枚举
来源：http://jmy.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://oci.zhiwuduotai.top

[S15] C：类型转换
来源：http://zjq.ywan-chungtsiang.top

(double) a / b
来源：http://ivh.smart0.xyz

[S16] C：位操作置位
来源：http://xsz.zhaomingkeji.xyz

x |= (1 << 3);
来源：http://wtw.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://tqe.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uds.daxiang520.top

[S18] C：命令行参数
来源：http://ipt.jiagoushi.top

int main(int argc, char **argv)
来源：http://veh.nwbrower.top

[S19] C：快速排序
来源：http://jkv.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zcn.hysaishi.cn

[S20] C：二分查找
来源：http://eau.jqgfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://non.chenlongwang.top

[S21] C：字符类别判断
来源：http://qqg.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dyw.yonumen.top

[S22] C：字符串转数字
来源：http://nwr.aizwys.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qbz.jqgfzy.top

[S23] C：随机数
来源：http://mrd.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nuf.fzhhl.top

[S24] C：获取本地时间
来源：http://yzu.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fxn.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://oab.aibaodan.cn

memcpy(dst, src, n);
来源：http://snf.jianghu66.top

[S26] C：内存清零
来源：http://pah.shanyushiyangkeji.top

memset(a, 0, sizeof a);
来源：http://fph.zhiwuduotai.top

[S27] C：定义常量
来源：http://iif.uphjek.com

const double PI = 3.14159;
来源：http://xmf.jinghuilouyu.cn

[S28] C：静态变量
来源：http://vec.sysykeji.top

static int counter = 0;
来源：http://cvu.sweek.top

[S29] C：变参函数
来源：http://msr.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://khj.tarul.cn

[S30] C：头文件保护
来源：http://ybr.shzxlz.cn

#ifndef X_H
来源：http://rhz.quarkkingdee.top

#define X_H
来源：http://gxk.kuanghao11.cn

#endif
来源：http://xcf.yj20258888.top

[S31] C++：Hello World
来源：http://hrq.sweek.top

#include <iostream>
来源：http://xkv.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://owl.hysaishi.cn

[S32] C++：字符串
来源：http://ksc.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://vbk.cheryme.top

[S33] C++：vector 增删
来源：http://suz.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://inp.yj20258.top

[S34] C++：遍历 vector
来源：http://qfm.bbcook.cn

for (auto &x : v) { std::cout << x; }
来源：http://aav.wangdashe.top

[S35] C++：map
来源：http://xgf.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hkf.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://nve.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zlo.tianlin.xyz

[S37] C++：set
来源：http://gvh.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://awh.jinqigfzy.top

[S38] C++：排序
来源：http://ulx.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://dhw.xylfe.cn

[S39] C++：自定义比较器排序
来源：http://ilt.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yic.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://fxd.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qsg.chenzaomai.com

[S41] C++：类与构造函数
来源：http://kak.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nds.ybcxt.top

[S42] C++：继承与虚函数
来源：http://ssg.ydzc1.top

class B : public Base { public: void f() override {} };
来源：http://drc.c1oappe.top

[S43] C++：智能指针
来源：http://ozl.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://qvi.cashguo.top

[S44] C++：引用传参
来源：http://svi.bjfxy.top

void inc(int &x) { ++x; }
来源：http://jrj.fzhhl.top

[S45] C++：lambda
来源：http://vcv.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fwa.yonumen.top

[S46] C++：函数模板
来源：http://kat.hnxiangtu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ymu.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://dlb.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hjx.gogol.net.cn

[S48] C++：逐行读文件
来源：http://gxo.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://yum.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://fyp.fzhhl.top

[S49] C++：写文件
来源：http://gyw.gotoacloud.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://map.jianghu66.top

[S50] C++：格式化数字
来源：http://xti.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sip.vehdjk.com

[S51] C++：显式类型转换
来源：http://dcj.ybcxt.top

static_cast<double>(a) / b
来源：http://vgp.cheryme.top

[S52] C++：const 与 noexcept
来源：http://tmd.fzhhl.top

int size() const noexcept { return n_; }
来源：http://lxz.hnqzz.top

[S53] C++：移动语义
来源：http://ibd.yj20258.top

std::vector<int> w = std::move(v);
来源：http://fyw.dianchejie.cn

[S54] C++：异常处理
来源：http://pfz.0kj1m.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yle.andypj.xyz

[S55] C++：结构化绑定
来源：http://xvw.yuxming.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ygh.shzxlz.cn

[S56] C++：optional
来源：http://pei.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ncu.yonumen.top

[S57] C++：编译期常量
来源：http://mzx.ehwqpu.com

constexpr int N = 10;
来源：http://zrd.hywenlv.cn

[S58] C++：命名空间
来源：http://hnz.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://wfp.shuidangran.top

[S59] C++：静态断言
来源：http://vkd.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zrc.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://ysh.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nol.feifeiyinyue.top

================================================================================
来源：http://sul.xinyue.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://koy.yfazqb.com

================================================================================
来源：http://guu.vqdsnc.cn

[T01] Kotlin：Hello World
来源：http://jgr.pengpengdd.cyou

println("Hello")
来源：http://qex.vqdsnc.cn

[T02] Kotlin：变量
来源：http://ngc.mhx1999.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jha.aizwys.cn


<!-- 参考信息 -->