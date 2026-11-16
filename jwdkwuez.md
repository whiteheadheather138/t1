代发 wailian999

R. Bash 专题
来源：http://vxc.guowangkeji.top

================================================================================
来源：http://ufx.jqgfzy.top

[R01] shebang 与严格模式
来源：http://ukc.tarul.cn

#!/usr/bin/env bash
来源：http://bwl.hysaishi.cn

set -euo pipefail
来源：http://guu.svipenyu.cn

[R02] 变量赋值与使用
来源：http://zmq.xuetiantiany.cn

name="Tom"; echo "$name"
来源：http://ama.jinqigfzy.top

[R03] 只读变量
来源：http://zaf.cdnleiting.top

readonly PI=3.14
来源：http://vms.dianchejie.cn

[R04] 位置参数
来源：http://vao.epnwcf.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sng.jiagoushi.top

[R05] 参数默认值
来源：http://jes.snrcjt.cn

name="${1:-default}"
来源：http://ogp.redwolf501.top

[R06] 判断命令是否存在
来源：http://nso.gogol.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yup.fktsv.cn

[R07] if 判断文件
来源：http://hkw.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://udv.yuxming.cn

[R08] 数值比较
来源：http://vnn.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fnh.xingfuxueyuan.xyz

[R09] 字符串比较
来源：http://fdg.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ooa.mhx1999.top

[R10] 正则匹配
来源：http://tdr.tanke756.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cvs.shzxlz.cn

[R11] case 多分支
来源：http://qia.zdqjudy.top

case "$1" in
来源：http://upt.pengpengdd.cyou

start) echo "启动" ;;
来源：http://qqs.ppjwa.cn

stop)  echo "停止" ;;
来源：http://lbp.birdmap.top

*)     echo "未知命令" ;;
来源：http://ust.hammf.cn

esac
来源：http://ott.iojbl.cn

[R12] for 遍历文件
来源：http://dxm.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://vtb.sweek.top

[R13] for 计数循环
来源：http://ypj.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://utv.chenjidiqi.icu

[R14] C 风格 for
来源：http://syf.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vvg.hnxiangtu.top

[R15] while 逐行读文件
来源：http://lkz.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bvl.xuetiantiany.cn

[R16] until 等待条件
来源：http://gps.zycfv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hun.yj202588.top

[R17] 数组定义与取值
来源：http://ulh.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://wnv.birdmap.top

[R18] 遍历数组
来源：http://fak.feifeiyinyue.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xkh.yueranfly.top

[R19] 数组长度
来源：http://ogh.sweek.top

echo "${#arr[@]}"
来源：http://crq.hcnkem.com

[R20] 关联数组（字典）
来源：http://ayu.shanyushiyangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lkh.zdbjq.cn

[R21] 字符串长度
来源：http://rvu.dianchejie.cn

echo "${#s}"
来源：http://hdk.havefunace.top

[R22] 截取子串
来源：http://nvz.yongpay.top

echo "${s:0:5}"
来源：http://jtn.smart0.xyz

[R23] 字符串替换
来源：http://eeh.tarul.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wtr.jinqigfzy.top

[R24] 大小写转换
来源：http://egr.fktsv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xzi.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://rng.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qsh.hywenlv.cn

[R26] 命令替换
来源：http://uhw.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://psx.dianchejie.cn

[R27] 算术展开
来源：http://jin.cheryme.top

echo $((1 + 2 * 3))
来源：http://gww.feifeiyinyue.top

[R28] 浮点运算
来源：http://qcq.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://kzm.jinghuilouyu.cn

[R29] 定义函数
来源：http://rsh.ybcxt.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sat.yuxming.cn

[R30] 函数返回状态码
来源：http://ayj.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://afd.sufxvd.cn

[R31] 局部变量
来源：http://dhe.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://cvp.hammf.cn

[R32] 参数个数校验
来源：http://rlr.meibo888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iii.shuidangran.top

[R33] 捕获错误并提示行号
来源：http://oou.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rnn.zhiwuduotai.top

[R34] 退出时清理
来源：http://ymd.jinqigfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://yvh.yongpay.top

[R35] 后台执行并等待
来源：http://iop.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://rcu.cdnleiting.top

[R36] 并发执行多个任务
来源：http://klx.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fdp.sweek.top

[R37] 把输出赋给变量
来源：http://qew.yj20258.top

files=$(ls -1)
来源：http://dpv.jiagoushi.top

[R38] 管道串联
来源：http://qkr.sweek.top

cat a.txt | grep -i error | wc -l
来源：http://xfk.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://gwx.sufxvd.cn

cmd > out.log 2>&1
来源：http://etr.zhijiandao.cn

[R40] 追加写日志
来源：http://wfg.gogol.net.cn

echo "log" >> out.log
来源：http://yoc.yj20258888.top

[R41] 丢弃输出
来源：http://yyx.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://ucj.fktsv.cn

[R42] 输入重定向
来源：http://dyn.shanyushiyangtech.top

wc -l < a.txt
来源：http://thy.zhijiandao.cn

[R43] 按名字查找文件
来源：http://tdo.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://esr.hongshengwenyu.top

[R44] 按修改时间查找
来源：http://ucw.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://hdk.uphjek.com

[R45] 批量删除
来源：http://iwe.wangdashe.top

find . -name "*.tmp" -delete
来源：http://wzt.yangfankeji.com

[R46] 递归替换文件内容
来源：http://hxu.sufxvd.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://imi.havefunace.top

[R47] sed 单行替换
来源：http://csz.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cqu.ctjpmb.com

[R48] awk 取指定列
来源：http://ivp.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://irq.cdnleiting.top

[R49] awk 带条件
来源：http://yqm.yvedp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ybu.hcnkem.com

[R50] awk 求和
来源：http://ivy.nwbrower.top

awk '{s += $2} END {print s}' a.txt
来源：http://zxl.jianghu66.top

[R51] 排序去重取前几
来源：http://dvx.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pqo.yfazqb.com

[R52] 统计行数
来源：http://zrq.shzxlz.cn

wc -l a.txt
来源：http://dix.meibo888.top

[R53] 查看文件头与实时尾
来源：http://vka.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fpz.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://ahr.zhongyouzk.top

diff a.txt b.txt
来源：http://zfb.nanxinkj.top

[R55] 压缩与解压
来源：http://mlq.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://opi.daxiang520.top

[R56] 远程拷贝
来源：http://gtt.kuanghao11.cn

scp file user@host:/path/
来源：http://vby.hnxiangtu.top

[R57] 远程执行命令
来源：http://xii.vehdjk.com

ssh user@host 'uptime'
来源：http://nzm.cashguo.top

[R58] 下载文件
来源：http://djn.chenjidiqi.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gfc.vqdsnc.cn

[R59] 发 POST JSON
来源：http://yuy.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ysp.jinqigfzy.top

[R60] 只看 HTTP 状态码
来源：http://ktn.wangshuangyany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uvr.xziqi.cn

[R61] 磁盘占用
来源：http://myu.gotoacloud.top

df -h;  du -sh *
来源：http://ddx.cdnleiting.top

[R62] 找最占空间的文件
来源：http://mog.jyoumei.cn

du -ah . | sort -rh | head -10
来源：http://fnx.aizwys.cn

[R63] 内存与进程
来源：http://qea.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://ftm.aizwys.cn

[R64] 结束进程
来源：http://tat.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://plo.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://coj.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dbd.yj20258888.top

[R66] 定时任务
来源：http://tge.zhongyouzk.top

crontab -e;  crontab -l
来源：http://hbq.pycfn.com

[R67] 生成随机十六进制串
来源：http://zhm.mhx1999.top

openssl rand -hex 16
来源：http://pce.xylfe.cn

[R68] 计算文件校验值
来源：http://spb.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://zbc.mhx1999.top

[R69] 生成随机密码
来源：http://fyb.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://zsj.pycfn.com

[R70] 时间戳与互转
来源：http://lgc.tarul.cn

date +%s;  date -d @1700000000
来源：http://lgl.zhongyouzk.top

[R71] 日期格式化
来源：http://xxa.xylfe.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://adw.andypj.xyz

[R72] 等待端口就绪
来源：http://eha.hnqzz.top

until nc -z localhost 3306; do sleep 1; done
来源：http://utd.hammf.cn

[R73] 分割大日志
来源：http://lyn.sysykeji.top

split -l 1000 big.log part_
来源：http://oay.sweek.top

[R74] 批量重命名
来源：http://spx.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gsn.gotoacloud.top

[R75] 导出环境变量
来源：http://wtj.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://bmj.pengpengdd.cyou

[R76] 使用临时文件
来源：http://elo.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://shn.zhengqikj.top

[R77] 读取用户输入
来源：http://uic.fktsv.cn

read -rp "请输入: " ans
来源：http://ozj.c1oappe.top

[R78] 交互式菜单
来源：http://jno.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://scg.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://zhb.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mqy.cheryme.top

[R80] 查看脚本执行耗时
来源：http://xyq.zhengqikj.top

time ./run.sh
来源：http://wrf.zdbjq.cn

================================================================================
来源：http://mch.zhijiandao.cn

S. C / C++ 专题
来源：http://swk.wangdashe.top

================================================================================
来源：http://vfw.xingfuxueyuan.xyz

[S01] C：Hello World
来源：http://iod.yj20258.top

#include <stdio.h>
来源：http://ixs.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gje.yj20258.top

[S02] C：变量与格式化输出
来源：http://uvw.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://exh.ctjpmb.com

[S03] C：读入整数
来源：http://bjk.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://dwk.andypj.xyz

[S04] C：字符串复制
来源：http://jio.birdmap.top

char dst[32]; strcpy(dst, "hi");
来源：http://kjf.dianchejie.cn

[S05] C：字符串长度
来源：http://kpa.fzhhl.top

strlen(s)
来源：http://dla.zhiwuduotai.top

[S06] C：字符串比较
来源：http://uza.bjfxy.top

strcmp(a, b) == 0
来源：http://wdc.sxryk.cn

[S07] C：数组遍历求和
来源：http://pjk.fanxiaobao.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ldx.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://aei.sysykeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gqr.hysaishi.cn

[S09] C：结构体定义与初始化
来源：http://vzm.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bie.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://lpr.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://hio.nanxinkj.top

[S11] C：逐行读文件
来源：http://juq.ydjk.org.cn

FILE *f = fopen("a.txt", "r");
来源：http://jzm.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://edt.ydjk.org.cn

fclose(f);
来源：http://akq.yuanzhike.top

[S12] C：写文件
来源：http://bhm.tianlin.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zeb.sjlbkw.cn

[S13] C：宏定义
来源：http://hiv.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bgg.gogol.net.cn

[S14] C：枚举
来源：http://kwt.zhixingplan.top

enum Color { RED, GREEN, BLUE };
来源：http://uwv.c1oappe.top

[S15] C：类型转换
来源：http://cti.shangyingyoupin.top

(double) a / b
来源：http://ptd.yanxiufei.cn

[S16] C：位操作置位
来源：http://gww.havefunace.top

x |= (1 << 3);
来源：http://lqp.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://gea.hesvh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jgt.jqgfzy.top

[S18] C：命令行参数
来源：http://hqg.sxryk.cn

int main(int argc, char **argv)
来源：http://njt.shangyingyoupin.top

[S19] C：快速排序
来源：http://dah.ehwqpu.com

qsort(a, n, sizeof(int), cmp);
来源：http://pjs.gotoacloud.top

[S20] C：二分查找
来源：http://vsu.tianlin.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://elj.xuanzx.com

[S21] C：字符类别判断
来源：http://nrz.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://epe.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://qig.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fkt.wangdashe.top

[S23] C：随机数
来源：http://yde.zhoulong.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://goc.chenjidiqi.icu

[S24] C：获取本地时间
来源：http://dik.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://icy.guannengcc.top

[S25] C：内存拷贝
来源：http://exb.nwbrower.top

memcpy(dst, src, n);
来源：http://msb.birdmap.top

[S26] C：内存清零
来源：http://ici.sjlbkw.cn

memset(a, 0, sizeof a);
来源：http://jtg.cqqwz.cn

[S27] C：定义常量
来源：http://dkx.tarul.cn

const double PI = 3.14159;
来源：http://atn.hammf.cn

[S28] C：静态变量
来源：http://igx.cucudq.cn

static int counter = 0;
来源：http://hof.zhixingplan.top

[S29] C：变参函数
来源：http://dkx.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ote.zycfv.cn

[S30] C：头文件保护
来源：http://irm.nanxuanxn.top

#ifndef X_H
来源：http://fmf.fengsongda.top

#define X_H
来源：http://tpy.fehbvm.com

#endif
来源：http://swe.cucudq.cn

[S31] C++：Hello World
来源：http://wkm.smart0.xyz

#include <iostream>
来源：http://ltt.yfazqb.com

int main() { std::cout << "Hello\n"; }
来源：http://fpl.hywenlv.cn

[S32] C++：字符串
来源：http://vtz.dashuyun.cn

std::string s = "hi";  s += "!";
来源：http://vex.zdbjq.cn

[S33] C++：vector 增删
来源：http://hul.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ljl.smart0.xyz

[S34] C++：遍历 vector
来源：http://evb.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://kxc.chenjidiqi.icu

[S35] C++：map
来源：http://vpu.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://flr.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://nsp.fehbvm.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hvh.zdqjudy.top

[S37] C++：set
来源：http://sxq.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://edx.shanyushiyangtech.top

[S38] C++：排序
来源：http://jou.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://dju.sxryk.cn

[S39] C++：自定义比较器排序
来源：http://wos.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vhz.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://iqy.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ukh.cashguo.top

[S41] C++：类与构造函数
来源：http://iha.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iux.cucudq.cn

[S42] C++：继承与虚函数
来源：http://tfu.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://djv.dashuyun.cn

[S43] C++：智能指针
来源：http://qsm.haohaochexian.top

auto p = std::make_unique<int>(5);
来源：http://pdx.gzhubu.top

[S44] C++：引用传参
来源：http://pne.cucudq.cn

void inc(int &x) { ++x; }
来源：http://qzx.guowangkeji.top

[S45] C++：lambda
来源：http://ajr.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://bxi.xingfuxueyuan.xyz

[S46] C++：函数模板
来源：http://yve.zhixingplan.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mke.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://dsu.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bnv.jinqigufen.top

[S48] C++：逐行读文件
来源：http://ovv.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://mbh.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://ltz.guannengcc.top

[S49] C++：写文件
来源：http://tqf.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://drr.yj20258888.top

[S50] C++：格式化数字
来源：http://gzv.gaohongyu789.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rhp.hammf.cn

[S51] C++：显式类型转换
来源：http://lzq.dianchejie.cn

static_cast<double>(a) / b
来源：http://yjy.uphjek.com

[S52] C++：const 与 noexcept
来源：http://zhq.redwolf501.top

int size() const noexcept { return n_; }
来源：http://krw.nwbrower.top

[S53] C++：移动语义
来源：http://fkv.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://kil.hnqzz.top

[S54] C++：异常处理
来源：http://gij.cashguo.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://olu.havefunace.top

[S55] C++：结构化绑定
来源：http://yse.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ghb.uphjek.com

[S56] C++：optional
来源：http://lpc.shzxlz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rpw.haohaochexian.top

[S57] C++：编译期常量
来源：http://vvr.tarul.cn

constexpr int N = 10;
来源：http://tjp.wangshuangyany.cn

[S58] C++：命名空间
来源：http://sde.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://vha.gaohongyu789.top

[S59] C++：静态断言
来源：http://fyg.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yzs.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://cxs.yj20258.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wny.dashuyun.cn

================================================================================
来源：http://fqs.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wlw.quarkkingdee.top

================================================================================
来源：http://mmi.xuetiantiany.cn


<!-- 参考信息 -->