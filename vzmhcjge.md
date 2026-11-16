代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://ucf.zdbjq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://czq.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rwa.wangshuangyany.cn

[Q89] 判断表是否存在
来源：http://snv.ydzc1.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mpt.cqqwz.cn

[Q90] 生成序号列
来源：http://mew.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://asg.gaohongyu789.top

================================================================================
来源：http://zeg.guowangkeji.top

R. Bash 专题
来源：http://bpd.bbcook.cn

================================================================================
来源：http://kqd.jianghu66.top

[R01] shebang 与严格模式
来源：http://mct.jinghuilouyu.cn

#!/usr/bin/env bash
来源：http://tkr.cucudq.cn

set -euo pipefail
来源：http://syo.aibaodan.cn

[R02] 变量赋值与使用
来源：http://pbc.hammf.cn

name="Tom"; echo "$name"
来源：http://loc.andypj.xyz

[R03] 只读变量
来源：http://avg.yfazqb.com

readonly PI=3.14
来源：http://ruw.ydzc1.top

[R04] 位置参数
来源：http://lok.dashuyun.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qrp.guannengcc.top

[R05] 参数默认值
来源：http://epl.jinqigfzy.top

name="${1:-default}"
来源：http://rpq.shzxlz.cn

[R06] 判断命令是否存在
来源：http://rdn.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gob.hesvh.cn

[R07] if 判断文件
来源：http://wgv.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ybx.sysykeji.top

[R08] 数值比较
来源：http://bhx.snrcjt.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ycn.yueranfly.top

[R09] 字符串比较
来源：http://ewn.cucudq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kyd.vehdjk.com

[R10] 正则匹配
来源：http://dus.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wmg.yvedp.cn

[R11] case 多分支
来源：http://qlm.yuanzhike.top

case "$1" in
来源：http://mky.yongpay.top

start) echo "启动" ;;
来源：http://ynv.jyoumei.cn

stop)  echo "停止" ;;
来源：http://wxr.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://xfy.zycfv.cn

esac
来源：http://zyd.xuanzx.com

[R12] for 遍历文件
来源：http://xye.shuidangran.top

for f in *.txt; do echo "$f"; done
来源：http://qpm.yongpay.top

[R13] for 计数循环
来源：http://fwc.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://hfv.mhx1999.top

[R14] C 风格 for
来源：http://odd.nanxuanxn.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://spo.52xcode.cn

[R15] while 逐行读文件
来源：http://gsn.gogol.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://epo.yj202588.top

[R16] until 等待条件
来源：http://tzm.fengsongda.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gsj.0kj1m.cn

[R17] 数组定义与取值
来源：http://vnd.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://shi.quarkkingdee.top

[R18] 遍历数组
来源：http://sce.jqgfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cbo.vehdjk.com

[R19] 数组长度
来源：http://dlu.shzxlz.cn

echo "${#arr[@]}"
来源：http://chd.uphjek.com

[R20] 关联数组（字典）
来源：http://neh.xylfe.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wyz.yj20258.top

[R21] 字符串长度
来源：http://yne.cashguo.top

echo "${#s}"
来源：http://ien.yj20258888.top

[R22] 截取子串
来源：http://lrs.hnqzz.top

echo "${s:0:5}"
来源：http://ryu.tian-w.cn

[R23] 字符串替换
来源：http://tfh.zhiwuduotai.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mon.tarul.cn

[R24] 大小写转换
来源：http://arj.sxryk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zqy.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://zfw.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://mdq.iojbl.cn

[R26] 命令替换
来源：http://yed.ybcxt.top

now=$(date +%F); echo "$now"
来源：http://hdj.feifeiyinyue.top

[R27] 算术展开
来源：http://yzx.sysykeji.top

echo $((1 + 2 * 3))
来源：http://nsp.pengpengdd.cyou

[R28] 浮点运算
来源：http://ros.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://sgg.chenjidiqi.icu

[R29] 定义函数
来源：http://sca.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://emm.yvedp.cn

[R30] 函数返回状态码
来源：http://xmn.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://ysm.zhaomingkeji.xyz

[R31] 局部变量
来源：http://sjp.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://kxy.daxiang520.top

[R32] 参数个数校验
来源：http://mnd.gzhubu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vfc.pycfn.com

[R33] 捕获错误并提示行号
来源：http://cmg.pycfn.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jpu.xinyue.icu

[R34] 退出时清理
来源：http://uod.daria6918.cn

trap 'rm -f "$tmp"' EXIT
来源：http://aca.nwbrower.top

[R35] 后台执行并等待
来源：http://umz.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wtq.52xcode.cn

[R36] 并发执行多个任务
来源：http://guw.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ufd.aibaodan.cn

[R37] 把输出赋给变量
来源：http://ukx.c1oappe.top

files=$(ls -1)
来源：http://liy.zhiwuduotai.top

[R38] 管道串联
来源：http://duv.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://nmi.daria6918.cn

[R39] 重定向标准输出与错误
来源：http://puh.gotoacloud.top

cmd > out.log 2>&1
来源：http://yfg.tarul.cn

[R40] 追加写日志
来源：http://uca.feifeiyinyue.top

echo "log" >> out.log
来源：http://gfz.gotoacloud.top

[R41] 丢弃输出
来源：http://orv.zhaomingkeji.xyz

cmd >/dev/null 2>&1
来源：http://edu.zycfv.cn

[R42] 输入重定向
来源：http://bxx.xylfe.cn

wc -l < a.txt
来源：http://jps.redwolf501.top

[R43] 按名字查找文件
来源：http://ajx.redwolf501.top

find . -name "*.log" -type f
来源：http://azr.52xcode.cn

[R44] 按修改时间查找
来源：http://hnr.yuxming.cn

find . -mtime -7 -type f
来源：http://plw.haohaochexian.top

[R45] 批量删除
来源：http://bve.kuanghao11.cn

find . -name "*.tmp" -delete
来源：http://ocv.ehwqpu.com

[R46] 递归替换文件内容
来源：http://rmp.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fol.ehwqpu.com

[R47] sed 单行替换
来源：http://amq.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://tdt.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://png.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://vwv.cdnleiting.top

[R49] awk 带条件
来源：http://rqd.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dnz.gaohongyu789.top

[R50] awk 求和
来源：http://dku.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://lqs.pycfn.com

[R51] 排序去重取前几
来源：http://nve.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://frr.yuanzhike.top

[R52] 统计行数
来源：http://wlw.wangdashe.top

wc -l a.txt
来源：http://whl.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://xls.daria6918.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://arh.zhijiandao.cn

[R54] 比较两个文件
来源：http://mgz.ywan-chungtsiang.top

diff a.txt b.txt
来源：http://lhg.zhixingplan.top

[R55] 压缩与解压
来源：http://qwg.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rgo.gzhubu.top

[R56] 远程拷贝
来源：http://lwc.meibo888.top

scp file user@host:/path/
来源：http://njd.cdnleiting.top

[R57] 远程执行命令
来源：http://uei.fanxiaobao.xyz

ssh user@host 'uptime'
来源：http://lqv.fzhhl.top

[R58] 下载文件
来源：http://ozb.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dex.andypj.xyz

[R59] 发 POST JSON
来源：http://bzd.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zpz.tian-w.cn

[R60] 只看 HTTP 状态码
来源：http://fqd.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gyp.pycfn.com

[R61] 磁盘占用
来源：http://fyu.sufxvd.cn

df -h;  du -sh *
来源：http://cjy.shangyingyoupin.top

[R62] 找最占空间的文件
来源：http://goi.zdqjudy.top

du -ah . | sort -rh | head -10
来源：http://cmt.guowangkeji.top

[R63] 内存与进程
来源：http://jcs.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://uvw.hnxiangtu.top

[R64] 结束进程
来源：http://qhf.yfazqb.com

kill -9 $(pgrep -f app.py)
来源：http://eko.tarul.cn

[R65] 查看端口占用
来源：http://xnj.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fmc.gzhubu.top

[R66] 定时任务
来源：http://diy.cdnleiting.top

crontab -e;  crontab -l
来源：http://ljy.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://eqm.ehwqpu.com

openssl rand -hex 16
来源：http://jqu.ctjpmb.com

[R68] 计算文件校验值
来源：http://alq.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fne.yvedp.cn

[R69] 生成随机密码
来源：http://rnv.zhaomingkeji.xyz

head -c 16 /dev/urandom | base64
来源：http://otd.gotoacloud.top

[R70] 时间戳与互转
来源：http://fnu.xziqi.cn

date +%s;  date -d @1700000000
来源：http://wpf.ybcxt.top

[R71] 日期格式化
来源：http://xck.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://csc.hcnkem.com

[R72] 等待端口就绪
来源：http://mpe.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://shx.pycfn.com

[R73] 分割大日志
来源：http://udw.aizwys.cn

split -l 1000 big.log part_
来源：http://fpm.nanxuanxn.top

[R74] 批量重命名
来源：http://hpq.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wrt.yanxiufei.cn

[R75] 导出环境变量
来源：http://xjp.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://vjc.tian-w.cn

[R76] 使用临时文件
来源：http://oyl.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kic.jyoumei.cn

[R77] 读取用户输入
来源：http://yjh.aibaodan.cn

read -rp "请输入: " ans
来源：http://ppa.guowangkeji.top

[R78] 交互式菜单
来源：http://byl.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vee.ybcxt.top

[R79] 解析命令行选项
来源：http://rfi.yj20258.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hvk.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://mba.nanxuanxn.top

time ./run.sh
来源：http://moi.fengsongda.top

================================================================================
来源：http://neb.hongshengwenyu.top

S. C / C++ 专题
来源：http://rlf.52xcode.cn

================================================================================
来源：http://xut.haohaochexian.top

[S01] C：Hello World
来源：http://okm.yj20258888.top

#include <stdio.h>
来源：http://mtf.hnxiangtu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gny.tarul.cn

[S02] C：变量与格式化输出
来源：http://kkf.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://afk.yueranfly.top

[S03] C：读入整数
来源：http://jor.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://eza.meibo888.top

[S04] C：字符串复制
来源：http://fll.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zpv.tianlin.xyz

[S05] C：字符串长度
来源：http://pjg.fanxiaobao.xyz

strlen(s)
来源：http://wvx.jianghu66.top

[S06] C：字符串比较
来源：http://sgv.smart0.xyz

strcmp(a, b) == 0
来源：http://nyq.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://uru.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gsm.chenjidiqi.icu

[S08] C：动态内存分配与释放
来源：http://naa.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://idx.gaohongyu789.top

[S09] C：结构体定义与初始化
来源：http://ijc.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yzb.hywenlv.cn

[S10] C：指针与解引用
来源：http://elj.sxryk.cn

int *p = &a;  *p = 5;
来源：http://uuh.xylfe.cn

[S11] C：逐行读文件
来源：http://gzg.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://jka.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yth.gogol.net.cn

fclose(f);
来源：http://cgx.xingfuxueyuan.xyz

[S12] C：写文件
来源：http://qiz.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://srz.cqqwz.cn

[S13] C：宏定义
来源：http://gxg.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://htf.zhengqikj.top

[S14] C：枚举
来源：http://yqt.snrcjt.cn

enum Color { RED, GREEN, BLUE };
来源：http://poa.shuidangran.top

[S15] C：类型转换
来源：http://fiu.chenlongwang.top

(double) a / b
来源：http://awe.sjlbkw.cn

[S16] C：位操作置位
来源：http://ucm.yongpay.top

x |= (1 << 3);
来源：http://yts.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://tpy.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zqa.hcnkem.com

[S18] C：命令行参数
来源：http://mhq.aibaodan.cn

int main(int argc, char **argv)
来源：http://vcu.zycfv.cn

[S19] C：快速排序
来源：http://xyd.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://coq.gzhubu.top

[S20] C：二分查找
来源：http://uzg.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dgf.yanxiufei.cn

[S21] C：字符类别判断
来源：http://bgd.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uzj.hammf.cn

[S22] C：字符串转数字
来源：http://gsh.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://dkb.yongpay.top

[S23] C：随机数
来源：http://mfy.svipenyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cyy.svipenyu.cn

[S24] C：获取本地时间
来源：http://kbe.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bcm.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://sft.smart0.xyz

memcpy(dst, src, n);
来源：http://dkk.fktsv.cn

[S26] C：内存清零
来源：http://svn.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://dfd.yfazqb.com

[S27] C：定义常量
来源：http://ndi.mhx1999.top

const double PI = 3.14159;
来源：http://akr.yvedp.cn

[S28] C：静态变量
来源：http://oec.shanyushiyangkeji.top

static int counter = 0;
来源：http://nbm.jlsjyb.cn

[S29] C：变参函数
来源：http://jmw.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vky.pengpengdd.cyou

[S30] C：头文件保护
来源：http://wyq.sufxvd.cn

#ifndef X_H
来源：http://vpe.cheryme.top

#define X_H
来源：http://kqq.sxryk.cn

#endif
来源：http://qrx.cqqwz.cn

[S31] C++：Hello World
来源：http://pgs.yuxming.cn

#include <iostream>
来源：http://cjo.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://mss.nwbrower.top

[S32] C++：字符串
来源：http://isu.9152youxi.cn

std::string s = "hi";  s += "!";
来源：http://xxs.zdbjq.cn

[S33] C++：vector 增删
来源：http://odl.ydjk.org.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lfh.xinyue.icu

[S34] C++：遍历 vector
来源：http://xjy.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://dsm.ybcxt.top

[S35] C++：map
来源：http://yoz.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lkg.hnqzz.top

[S36] C++：unordered_map
来源：http://pgw.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mey.uphjek.com

[S37] C++：set
来源：http://lcu.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://etj.yueranfly.top

[S38] C++：排序
来源：http://dbp.ybcxt.top

std::sort(v.begin(), v.end());
来源：http://nxi.zycfv.cn

[S39] C++：自定义比较器排序
来源：http://inh.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gwf.guannengcc.top

[S40] C++：查找元素
来源：http://okq.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cfp.yj20258.top

[S41] C++：类与构造函数
来源：http://xls.cashguo.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qfz.sweek.top

[S42] C++：继承与虚函数
来源：http://zui.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://cgm.feifeiyinyue.top

[S43] C++：智能指针
来源：http://oxr.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://vol.feifeiyinyue.top

[S44] C++：引用传参
来源：http://lor.cucudq.cn

void inc(int &x) { ++x; }
来源：http://alk.hfpthk.cn

[S45] C++：lambda
来源：http://ahk.hnqzz.top

auto add = [](int a, int b) { return a + b; };
来源：http://ayx.tian-w.cn

[S46] C++：函数模板
来源：http://wqi.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uel.xuetiantiany.cn

[S47] C++：结构化绑定遍历
来源：http://zzv.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iek.cqqwz.cn

[S48] C++：逐行读文件
来源：http://fys.hnqzz.top

std::ifstream in("a.txt");  std::string line;
来源：http://wks.fktsv.cn

while (std::getline(in, line)) { }
来源：http://oxo.yj20258888.top

[S49] C++：写文件
来源：http://wnu.xziqi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lpn.jinqigfzy.top

[S50] C++：格式化数字
来源：http://dzy.xziqi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lcd.bbcook.cn

[S51] C++：显式类型转换
来源：http://ywz.zhijiandao.cn

static_cast<double>(a) / b
来源：http://rck.sweek.top

[S52] C++：const 与 noexcept
来源：http://hug.aizwys.cn

int size() const noexcept { return n_; }
来源：http://fhi.mhx1999.top

[S53] C++：移动语义
来源：http://xxa.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://hpg.vqdsnc.cn

[S54] C++：异常处理
来源：http://rxq.zhongyouzk.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mbz.dianchejie.cn

[S55] C++：结构化绑定
来源：http://imi.sweek.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jmx.hammf.cn

[S56] C++：optional
来源：http://xhj.hysaishi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vct.zhijiandao.cn

[S57] C++：编译期常量
来源：http://igm.nwbrower.top

constexpr int N = 10;
来源：http://enl.dashuyun.cn

[S58] C++：命名空间
来源：http://pcw.wangdashe.top


<!-- 参考信息 -->