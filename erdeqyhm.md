代发 wailian999

R. Bash 专题
来源：http://mpx.xingfuxueyuan.xyz

================================================================================
来源：http://kix.meibo888.top

[R01] shebang 与严格模式
来源：http://rmo.cdnleiting.top

#!/usr/bin/env bash
来源：http://zjp.pycfn.com

set -euo pipefail
来源：http://dbg.wangdashe.top

[R02] 变量赋值与使用
来源：http://ufv.sufxvd.cn

name="Tom"; echo "$name"
来源：http://swz.zdbjq.cn

[R03] 只读变量
来源：http://rpe.hcnkem.com

readonly PI=3.14
来源：http://ysw.zhengqikj.top

[R04] 位置参数
来源：http://blf.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yyi.xinyue.icu

[R05] 参数默认值
来源：http://qng.chenzaomai.com

name="${1:-default}"
来源：http://kgc.jinqigufen.top

[R06] 判断命令是否存在
来源：http://jxx.zhijiandao.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://abc.yj20258888.top

[R07] if 判断文件
来源：http://bpp.yueranfly.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cbv.cheryme.top

[R08] 数值比较
来源：http://scp.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://obr.bbcook.cn

[R09] 字符串比较
来源：http://pww.hcnkem.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vyn.snrcjt.cn

[R10] 正则匹配
来源：http://trb.haohaochexian.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://asi.chenlongwang.top

[R11] case 多分支
来源：http://suj.gzhubu.top

case "$1" in
来源：http://xnw.daria6918.cn

start) echo "启动" ;;
来源：http://iok.yvedp.cn

stop)  echo "停止" ;;
来源：http://awn.jyoumei.cn

*)     echo "未知命令" ;;
来源：http://rdy.52xcode.cn

esac
来源：http://rtc.xingfuxueyuan.xyz

[R12] for 遍历文件
来源：http://nyy.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://xzg.guowangkeji.top

[R13] for 计数循环
来源：http://rhg.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://wtz.shangyingyoupin.top

[R14] C 风格 for
来源：http://esq.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nxm.nwbrower.top

[R15] while 逐行读文件
来源：http://syv.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eay.zhixingplan.top

[R16] until 等待条件
来源：http://xhb.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vah.fengsongda.top

[R17] 数组定义与取值
来源：http://zfg.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vkh.sxryk.cn

[R18] 遍历数组
来源：http://hrq.yj202588.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pps.birdmap.top

[R19] 数组长度
来源：http://qvh.hywenlv.cn

echo "${#arr[@]}"
来源：http://twu.xziqi.cn

[R20] 关联数组（字典）
来源：http://hdo.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vgg.0kj1m.cn

[R21] 字符串长度
来源：http://mfy.guannengcc.top

echo "${#s}"
来源：http://ayb.shuidangran.top

[R22] 截取子串
来源：http://vpy.sxryk.cn

echo "${s:0:5}"
来源：http://wae.cqqwz.cn

[R23] 字符串替换
来源：http://gkf.cqqwz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dwu.zhoulong.xyz

[R24] 大小写转换
来源：http://ehg.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zcm.zhijiandao.cn

[R25] 去后缀 / 去前缀
来源：http://pcj.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lis.chenjidiqi.icu

[R26] 命令替换
来源：http://eda.zdqjudy.top

now=$(date +%F); echo "$now"
来源：http://jan.jiagoushi.top

[R27] 算术展开
来源：http://vqn.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://ggq.gaohongyu789.top

[R28] 浮点运算
来源：http://kma.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://ejh.shanyushiyangkeji.top

[R29] 定义函数
来源：http://dfb.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gbd.jlsjyb.cn

[R30] 函数返回状态码
来源：http://aag.zycfv.cn

f() { return 0; }; f || echo "失败了"
来源：http://plk.chenjidiqi.icu

[R31] 局部变量
来源：http://dir.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://sdd.jinqigufen.top

[R32] 参数个数校验
来源：http://uwy.yj20258.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rzi.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://xgw.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xst.jyoumei.cn

[R34] 退出时清理
来源：http://lyt.shzxlz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bxf.zhoulong.xyz

[R35] 后台执行并等待
来源：http://dab.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mxt.iojbl.cn

[R36] 并发执行多个任务
来源：http://xbr.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gdq.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://jsf.wangdashe.top

files=$(ls -1)
来源：http://jpr.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://czn.kuanghao11.cn

cat a.txt | grep -i error | wc -l
来源：http://qck.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://tpe.gogol.net.cn

cmd > out.log 2>&1
来源：http://mzd.yanxiufei.cn

[R40] 追加写日志
来源：http://jii.gzhubu.top

echo "log" >> out.log
来源：http://qwp.jianghu66.top

[R41] 丢弃输出
来源：http://byg.xylfe.cn

cmd >/dev/null 2>&1
来源：http://zjd.epnwcf.com

[R42] 输入重定向
来源：http://whb.quarkkingdee.top

wc -l < a.txt
来源：http://cnx.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://hfc.hfpthk.cn

find . -name "*.log" -type f
来源：http://sfu.ehwqpu.com

[R44] 按修改时间查找
来源：http://qcy.zdqjudy.top

find . -mtime -7 -type f
来源：http://xpg.fktsv.cn

[R45] 批量删除
来源：http://ugq.aibaodan.cn

find . -name "*.tmp" -delete
来源：http://dik.gotoacloud.top

[R46] 递归替换文件内容
来源：http://vxd.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wvv.ppjwa.cn

[R47] sed 单行替换
来源：http://fgs.hesvh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zsi.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://mhh.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://btp.nwbrower.top

[R49] awk 带条件
来源：http://our.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bii.shanyushiyangtech.top

[R50] awk 求和
来源：http://mkk.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://onu.zhixingplan.top

[R51] 排序去重取前几
来源：http://zkh.smart0.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ovf.fktsv.cn

[R52] 统计行数
来源：http://pag.tarul.cn

wc -l a.txt
来源：http://are.yvedp.cn

[R53] 查看文件头与实时尾
来源：http://aul.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bta.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://yvh.yuxming.cn

diff a.txt b.txt
来源：http://osl.fanxiaobao.xyz

[R55] 压缩与解压
来源：http://xny.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://olt.bbcook.cn

[R56] 远程拷贝
来源：http://mrt.cdnleiting.top

scp file user@host:/path/
来源：http://twe.cucudq.cn

[R57] 远程执行命令
来源：http://fhm.jianghu66.top

ssh user@host 'uptime'
来源：http://keg.cucudq.cn

[R58] 下载文件
来源：http://qyi.52xcode.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vqw.jinqigufen.top

[R59] 发 POST JSON
来源：http://juw.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zer.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://qby.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nje.gogol.net.cn

[R61] 磁盘占用
来源：http://qyp.daria6918.cn

df -h;  du -sh *
来源：http://gis.zhongyouzk.top

[R62] 找最占空间的文件
来源：http://nec.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://hiw.jinghuilouyu.cn

[R63] 内存与进程
来源：http://lvv.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://ola.jianghu66.top

[R64] 结束进程
来源：http://fih.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://oyw.sxryk.cn

[R65] 查看端口占用
来源：http://hcz.hnqzz.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iuq.gaohongyu789.top

[R66] 定时任务
来源：http://zff.jqgfzy.top

crontab -e;  crontab -l
来源：http://gle.vehdjk.com

[R67] 生成随机十六进制串
来源：http://urt.meibo888.top

openssl rand -hex 16
来源：http://jkt.ctjpmb.com

[R68] 计算文件校验值
来源：http://vqc.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://suy.316326.xyz

[R69] 生成随机密码
来源：http://fop.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://jsm.yj20258888.top

[R70] 时间戳与互转
来源：http://oui.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://daa.0kj1m.cn

[R71] 日期格式化
来源：http://jks.sxryk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ztp.yuxming.cn

[R72] 等待端口就绪
来源：http://qnf.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tgy.gogol.net.cn

[R73] 分割大日志
来源：http://umf.xuanzx.com

split -l 1000 big.log part_
来源：http://wut.fzhhl.top

[R74] 批量重命名
来源：http://tkv.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://coj.chenlongwang.top

[R75] 导出环境变量
来源：http://ijd.sysykeji.top

export PATH="$HOME/bin:$PATH"
来源：http://pvv.dianchejie.cn

[R76] 使用临时文件
来源：http://tuq.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://roh.epnwcf.com

[R77] 读取用户输入
来源：http://jdd.yuxming.cn

read -rp "请输入: " ans
来源：http://gfc.shzxlz.cn

[R78] 交互式菜单
来源：http://eyk.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wbi.jlsjyb.cn

[R79] 解析命令行选项
来源：http://bsp.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hcw.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://ymf.guannengcc.top

time ./run.sh
来源：http://fhp.zhixingplan.top

================================================================================
来源：http://zkx.sjlbkw.cn

S. C / C++ 专题
来源：http://has.zhixingplan.top

================================================================================
来源：http://gpa.pengpengdd.cyou

[S01] C：Hello World
来源：http://ial.wangdashe.top

#include <stdio.h>
来源：http://tll.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ovh.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://syo.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://qro.yonumen.top

[S03] C：读入整数
来源：http://jnu.xylfe.cn

int x; scanf("%d", &x);
来源：http://gwu.nanxinkj.top

[S04] C：字符串复制
来源：http://bxg.jiagoushi.top

char dst[32]; strcpy(dst, "hi");
来源：http://rpf.xylfe.cn

[S05] C：字符串长度
来源：http://ocb.jianghu66.top

strlen(s)
来源：http://hyx.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://psf.xinyue.icu

strcmp(a, b) == 0
来源：http://ihc.wangdashe.top

[S07] C：数组遍历求和
来源：http://sqw.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://btm.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://dwz.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zrp.cheryme.top

[S09] C：结构体定义与初始化
来源：http://epb.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mxt.aibaodan.cn

[S10] C：指针与解引用
来源：http://tot.uphjek.com

int *p = &a;  *p = 5;
来源：http://uht.tianlin.xyz

[S11] C：逐行读文件
来源：http://fza.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://pqq.shanyushiyangtech.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wog.svipenyu.cn

fclose(f);
来源：http://agi.gotoacloud.top

[S12] C：写文件
来源：http://qcn.0kj1m.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wlq.tarul.cn

[S13] C：宏定义
来源：http://xtb.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dtc.ppjwa.cn

[S14] C：枚举
来源：http://zhl.gotoacloud.top

enum Color { RED, GREEN, BLUE };
来源：http://gpc.c1oappe.top

[S15] C：类型转换
来源：http://edp.fehbvm.com

(double) a / b
来源：http://crg.chenzaomai.com

[S16] C：位操作置位
来源：http://mlx.sysykeji.top

x |= (1 << 3);
来源：http://bfs.yfazqb.com

[S17] C：安全拼接字符串
来源：http://ywj.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yop.zhaomingkeji.xyz

[S18] C：命令行参数
来源：http://yuu.nanxuanxn.top

int main(int argc, char **argv)
来源：http://bex.aibaodan.cn

[S19] C：快速排序
来源：http://ukf.hnqzz.top

qsort(a, n, sizeof(int), cmp);
来源：http://uvy.sxryk.cn

[S20] C：二分查找
来源：http://jln.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gvr.andypj.xyz

[S21] C：字符类别判断
来源：http://oin.cqqwz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lzc.fanxiaobao.xyz

[S22] C：字符串转数字
来源：http://bag.0kj1m.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fzb.jinqigufen.top

[S23] C：随机数
来源：http://vss.zhengqikj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mnm.smart0.xyz

[S24] C：获取本地时间
来源：http://kgs.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iyf.yongpay.top

[S25] C：内存拷贝
来源：http://zup.aibaodan.cn

memcpy(dst, src, n);
来源：http://gun.yuanzhike.top

[S26] C：内存清零
来源：http://bzy.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://ieq.jinghuilouyu.cn

[S27] C：定义常量
来源：http://aub.hnxiangtu.top

const double PI = 3.14159;
来源：http://dtp.hysaishi.cn

[S28] C：静态变量
来源：http://nyn.fzhhl.top

static int counter = 0;
来源：http://sbu.nanxuanxn.top

[S29] C：变参函数
来源：http://hco.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dlj.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://fkb.guowangkeji.top

#ifndef X_H
来源：http://cec.ywan-chungtsiang.top

#define X_H
来源：http://ywq.tianlin.xyz

#endif
来源：http://tiy.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://xsr.jlsjyb.cn

#include <iostream>
来源：http://ksz.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://ypl.andypj.xyz

[S32] C++：字符串
来源：http://mmj.vqdsnc.cn

std::string s = "hi";  s += "!";
来源：http://gbb.quarkkingdee.top

[S33] C++：vector 增删
来源：http://yoo.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zag.meibo888.top

[S34] C++：遍历 vector
来源：http://sqb.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://hld.yuanzhike.top

[S35] C++：map
来源：http://eir.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yoe.ivvv.top

[S36] C++：unordered_map
来源：http://ler.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fey.chenlongwang.top

[S37] C++：set
来源：http://ijh.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rsg.ivvv.top

[S38] C++：排序
来源：http://ukr.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://lxu.cashguo.top

[S39] C++：自定义比较器排序
来源：http://eqp.snrcjt.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yca.hammf.cn

[S40] C++：查找元素
来源：http://ldd.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lbd.vehdjk.com

[S41] C++：类与构造函数
来源：http://dvz.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ykt.fzhhl.top

[S42] C++：继承与虚函数
来源：http://zsw.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://zag.ppjwa.cn

[S43] C++：智能指针
来源：http://lov.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://ejy.chenzaomai.com

[S44] C++：引用传参
来源：http://qkd.wangshuangyany.cn

void inc(int &x) { ++x; }
来源：http://ijx.gotoacloud.top

[S45] C++：lambda
来源：http://kem.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kxq.svipenyu.cn

[S46] C++：函数模板
来源：http://aov.xylfe.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cqw.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://tvc.vehdjk.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://por.xuanzx.com

[S48] C++：逐行读文件
来源：http://ivd.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://arw.aizwys.cn

while (std::getline(in, line)) { }
来源：http://mpe.nwbrower.top

[S49] C++：写文件
来源：http://kig.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bfi.ehwqpu.com

[S50] C++：格式化数字
来源：http://sws.yj20258.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tin.yj20258888.top

[S51] C++：显式类型转换
来源：http://phu.wangdashe.top

static_cast<double>(a) / b
来源：http://rrx.snrcjt.cn

[S52] C++：const 与 noexcept
来源：http://bhx.nwbrower.top

int size() const noexcept { return n_; }
来源：http://uwc.pengpengdd.cyou

[S53] C++：移动语义
来源：http://wve.yonumen.top

std::vector<int> w = std::move(v);
来源：http://plv.xziqi.cn

[S54] C++：异常处理
来源：http://kha.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mrw.bjfxy.top

[S55] C++：结构化绑定
来源：http://vre.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jxw.tanke756.top

[S56] C++：optional
来源：http://llf.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fyn.zdbjq.cn

[S57] C++：编译期常量
来源：http://wax.fengsongda.top

constexpr int N = 10;
来源：http://ucg.redwolf501.top

[S58] C++：命名空间
来源：http://aey.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://isn.gaohongyu789.top

[S59] C++：静态断言
来源：http://xbn.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hhs.yvedp.cn

[S60] C++：遍历并删除元素
来源：http://fkz.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wng.ybcxt.top

================================================================================
来源：http://ixi.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yvj.hywenlv.cn

================================================================================
来源：http://rmb.tarul.cn


<!-- 参考信息 -->