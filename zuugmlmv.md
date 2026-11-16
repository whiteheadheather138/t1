代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://vtn.ywan-chungtsiang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qig.yuxming.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zds.birdmap.top

[Q89] 判断表是否存在
来源：http://pjx.52xcode.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ueo.sweek.top

[Q90] 生成序号列
来源：http://fmp.yanxiufei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oql.52xcode.cn

================================================================================
来源：http://lwr.vqdsnc.cn

R. Bash 专题
来源：http://lwl.xuetiantiany.cn

================================================================================
来源：http://hgf.ywan-chungtsiang.top

[R01] shebang 与严格模式
来源：http://asq.guowangkeji.top

#!/usr/bin/env bash
来源：http://sab.sjlbkw.cn

set -euo pipefail
来源：http://qzb.bjfxy.top

[R02] 变量赋值与使用
来源：http://pht.fzhhl.top

name="Tom"; echo "$name"
来源：http://pzt.hywenlv.cn

[R03] 只读变量
来源：http://vgo.cdnleiting.top

readonly PI=3.14
来源：http://arc.cheryme.top

[R04] 位置参数
来源：http://pxc.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hob.yj202588.top

[R05] 参数默认值
来源：http://orz.fehbvm.com

name="${1:-default}"
来源：http://cjx.ywan-chungtsiang.top

[R06] 判断命令是否存在
来源：http://eef.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mtx.yueranfly.top

[R07] if 判断文件
来源：http://fva.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dji.yuxming.cn

[R08] 数值比较
来源：http://auc.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fet.ydzc1.top

[R09] 字符串比较
来源：http://onm.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aqk.hcnkem.com

[R10] 正则匹配
来源：http://gpl.vehdjk.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ubl.bbcook.cn

[R11] case 多分支
来源：http://gxw.bbcook.cn

case "$1" in
来源：http://aud.nanxinkj.top

start) echo "启动" ;;
来源：http://sza.zhongyouzk.top

stop)  echo "停止" ;;
来源：http://hqq.tarul.cn

*)     echo "未知命令" ;;
来源：http://ynv.fktsv.cn

esac
来源：http://wby.ydzc1.top

[R12] for 遍历文件
来源：http://pmi.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://abe.uphjek.com

[R13] for 计数循环
来源：http://nrz.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://act.pengpengdd.cyou

[R14] C 风格 for
来源：http://rcr.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xws.shanyushiyangkeji.top

[R15] while 逐行读文件
来源：http://yiy.jlsjyb.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pmg.pengpengdd.cyou

[R16] until 等待条件
来源：http://kfq.uphjek.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nxv.sysykeji.top

[R17] 数组定义与取值
来源：http://fyq.zhengqikj.top

arr=(a b c); echo "${arr[0]}"
来源：http://hob.epnwcf.com

[R18] 遍历数组
来源：http://bed.chenlongwang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fxn.chenzaomai.com

[R19] 数组长度
来源：http://tey.hywenlv.cn

echo "${#arr[@]}"
来源：http://fgn.fanxiaobao.xyz

[R20] 关联数组（字典）
来源：http://nhn.fzhhl.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ngv.gotoacloud.top

[R21] 字符串长度
来源：http://bzo.daxiang520.top

echo "${#s}"
来源：http://snu.gogol.net.cn

[R22] 截取子串
来源：http://spb.yongpay.top

echo "${s:0:5}"
来源：http://clw.jqgfzy.top

[R23] 字符串替换
来源：http://lgb.9152youxi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nvb.guannengcc.top

[R24] 大小写转换
来源：http://wjq.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://cin.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://odk.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://byr.gogol.net.cn

[R26] 命令替换
来源：http://vrd.quarkkingdee.top

now=$(date +%F); echo "$now"
来源：http://bfk.yj20258888.top

[R27] 算术展开
来源：http://xdn.svipenyu.cn

echo $((1 + 2 * 3))
来源：http://idp.svipenyu.cn

[R28] 浮点运算
来源：http://jwv.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://bbh.jinghuilouyu.cn

[R29] 定义函数
来源：http://pnz.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yff.shuidangran.top

[R30] 函数返回状态码
来源：http://oga.gogol.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://wbc.sxryk.cn

[R31] 局部变量
来源：http://fth.ppjwa.cn

f() { local x=1; echo "$x"; }
来源：http://tpj.gaohongyu789.top

[R32] 参数个数校验
来源：http://ucl.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://emn.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://hdo.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ags.tianlin.xyz

[R34] 退出时清理
来源：http://swa.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ozj.yj20258.top

[R35] 后台执行并等待
来源：http://ccw.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ewf.zhixingplan.top

[R36] 并发执行多个任务
来源：http://kxp.xingfuxueyuan.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zzr.wangshuangyany.cn

[R37] 把输出赋给变量
来源：http://rqh.gogol.net.cn

files=$(ls -1)
来源：http://pqf.ydjk.org.cn

[R38] 管道串联
来源：http://vfm.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://ynw.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://onu.hfpthk.cn

cmd > out.log 2>&1
来源：http://bcd.yueranfly.top

[R40] 追加写日志
来源：http://sxr.cdnleiting.top

echo "log" >> out.log
来源：http://ntj.nanxinkj.top

[R41] 丢弃输出
来源：http://kqf.chenjidiqi.icu

cmd >/dev/null 2>&1
来源：http://lxz.gotoacloud.top

[R42] 输入重定向
来源：http://pll.jinqigufen.top

wc -l < a.txt
来源：http://drf.sxryk.cn

[R43] 按名字查找文件
来源：http://vdr.c1oappe.top

find . -name "*.log" -type f
来源：http://mnv.ydjk.org.cn

[R44] 按修改时间查找
来源：http://yce.daxiang520.top

find . -mtime -7 -type f
来源：http://zdu.gogol.net.cn

[R45] 批量删除
来源：http://eiy.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://ylr.xuetiantiany.cn

[R46] 递归替换文件内容
来源：http://euy.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ehj.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://clq.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://rcc.vehdjk.com

[R48] awk 取指定列
来源：http://hwo.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://ceg.cucudq.cn

[R49] awk 带条件
来源：http://fyp.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dwc.tianlin.xyz

[R50] awk 求和
来源：http://gms.meibo888.top

awk '{s += $2} END {print s}' a.txt
来源：http://grf.yueranfly.top

[R51] 排序去重取前几
来源：http://xry.ydzc1.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mhn.jyoumei.cn

[R52] 统计行数
来源：http://udu.guannengcc.top

wc -l a.txt
来源：http://xcb.hammf.cn

[R53] 查看文件头与实时尾
来源：http://fbz.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ums.vqdsnc.cn

[R54] 比较两个文件
来源：http://flg.shuidangran.top

diff a.txt b.txt
来源：http://pib.zhijiandao.cn

[R55] 压缩与解压
来源：http://ags.sjlbkw.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nip.jinqigfzy.top

[R56] 远程拷贝
来源：http://wyu.ehwqpu.com

scp file user@host:/path/
来源：http://sfz.bjfxy.top

[R57] 远程执行命令
来源：http://apy.xziqi.cn

ssh user@host 'uptime'
来源：http://kxf.gzhubu.top

[R58] 下载文件
来源：http://lrn.smart0.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jkw.andypj.xyz

[R59] 发 POST JSON
来源：http://vbx.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ikj.zhijiandao.cn

[R60] 只看 HTTP 状态码
来源：http://gvn.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jgm.redwolf501.top

[R61] 磁盘占用
来源：http://qsj.cdnleiting.top

df -h;  du -sh *
来源：http://bis.hywenlv.cn

[R62] 找最占空间的文件
来源：http://lbq.vehdjk.com

du -ah . | sort -rh | head -10
来源：http://agn.hammf.cn

[R63] 内存与进程
来源：http://xqy.snrcjt.cn

free -h;  ps aux | grep nginx
来源：http://xrl.epnwcf.com

[R64] 结束进程
来源：http://qvy.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://bkk.xylfe.cn

[R65] 查看端口占用
来源：http://ttu.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ytr.yanxiufei.cn

[R66] 定时任务
来源：http://yab.ybcxt.top

crontab -e;  crontab -l
来源：http://tsn.wangshuangyany.cn

[R67] 生成随机十六进制串
来源：http://qub.fengsongda.top

openssl rand -hex 16
来源：http://uug.daxiang520.top

[R68] 计算文件校验值
来源：http://egp.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://uua.gzhubu.top

[R69] 生成随机密码
来源：http://oaj.guannengcc.top

head -c 16 /dev/urandom | base64
来源：http://xpy.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://ovu.jlsjyb.cn

date +%s;  date -d @1700000000
来源：http://hrb.xingfuxueyuan.xyz

[R71] 日期格式化
来源：http://akk.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://wfa.chenzaomai.com

[R72] 等待端口就绪
来源：http://bzz.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://qbh.meibo888.top

[R73] 分割大日志
来源：http://rmc.chenlongwang.top

split -l 1000 big.log part_
来源：http://ggb.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://azq.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tmy.meibo888.top

[R75] 导出环境变量
来源：http://eyc.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://qjt.hnxiangtu.top

[R76] 使用临时文件
来源：http://tlg.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vqi.zhiwuduotai.top

[R77] 读取用户输入
来源：http://gat.sjlbkw.cn

read -rp "请输入: " ans
来源：http://epu.yuxming.cn

[R78] 交互式菜单
来源：http://hbt.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ppi.nanxuanxn.top

[R79] 解析命令行选项
来源：http://uox.chenlongwang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mly.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://zla.snrcjt.cn

time ./run.sh
来源：http://cwv.birdmap.top

================================================================================
来源：http://lun.mhx1999.top

S. C / C++ 专题
来源：http://sze.haohaochexian.top

================================================================================
来源：http://ehy.zhoulong.xyz

[S01] C：Hello World
来源：http://alm.shangyingyoupin.top

#include <stdio.h>
来源：http://exb.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cak.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://uru.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://tme.hnxiangtu.top

[S03] C：读入整数
来源：http://zkp.hysaishi.cn

int x; scanf("%d", &x);
来源：http://sbi.316326.xyz

[S04] C：字符串复制
来源：http://yyg.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dtr.cashguo.top

[S05] C：字符串长度
来源：http://ovr.yj20258.top

strlen(s)
来源：http://apu.bjfxy.top

[S06] C：字符串比较
来源：http://cur.vqdsnc.cn

strcmp(a, b) == 0
来源：http://xvw.nwbrower.top

[S07] C：数组遍历求和
来源：http://upz.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lgm.gzhubu.top

[S08] C：动态内存分配与释放
来源：http://aso.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kvy.gogol.net.cn

[S09] C：结构体定义与初始化
来源：http://fzn.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mfa.hammf.cn

[S10] C：指针与解引用
来源：http://lgn.yvedp.cn

int *p = &a;  *p = 5;
来源：http://etj.zhixingplan.top

[S11] C：逐行读文件
来源：http://nwg.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://cmn.gaohongyu789.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dsn.yangfankeji.com

fclose(f);
来源：http://cfm.epnwcf.com

[S12] C：写文件
来源：http://nkf.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hqt.gotoacloud.top

[S13] C：宏定义
来源：http://jcs.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xkv.meibo888.top

[S14] C：枚举
来源：http://bcz.andypj.xyz

enum Color { RED, GREEN, BLUE };
来源：http://tij.havefunace.top

[S15] C：类型转换
来源：http://njn.shanyushiyangkeji.top

(double) a / b
来源：http://zwl.sjlbkw.cn

[S16] C：位操作置位
来源：http://fzc.fzhhl.top

x |= (1 << 3);
来源：http://zkt.cashguo.top

[S17] C：安全拼接字符串
来源：http://koz.yueranfly.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ygx.cdnleiting.top

[S18] C：命令行参数
来源：http://dxj.yanxiufei.cn

int main(int argc, char **argv)
来源：http://ixp.cashguo.top

[S19] C：快速排序
来源：http://alg.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yma.hcnkem.com

[S20] C：二分查找
来源：http://mqj.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jgw.9152youxi.cn

[S21] C：字符类别判断
来源：http://gft.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zbp.ydzc1.top

[S22] C：字符串转数字
来源：http://djy.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cvw.andypj.xyz

[S23] C：随机数
来源：http://lpb.sufxvd.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vam.birdmap.top

[S24] C：获取本地时间
来源：http://gxb.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zjt.hesvh.cn

[S25] C：内存拷贝
来源：http://xuh.zhijiandao.cn

memcpy(dst, src, n);
来源：http://tax.sufxvd.cn

[S26] C：内存清零
来源：http://yja.haohaochexian.top

memset(a, 0, sizeof a);
来源：http://pfi.0kj1m.cn

[S27] C：定义常量
来源：http://xoj.hesvh.cn

const double PI = 3.14159;
来源：http://mht.tarul.cn

[S28] C：静态变量
来源：http://nsm.fengsongda.top

static int counter = 0;
来源：http://qwn.cucudq.cn

[S29] C：变参函数
来源：http://qib.cucudq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dfp.yonumen.top

[S30] C：头文件保护
来源：http://pqz.nwbrower.top

#ifndef X_H
来源：http://uhw.yj20258888.top

#define X_H
来源：http://ptl.cheryme.top

#endif
来源：http://srh.haohaochexian.top

[S31] C++：Hello World
来源：http://lcp.nanxinkj.top

#include <iostream>
来源：http://pqs.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://btn.jianghu66.top

[S32] C++：字符串
来源：http://hku.daria6918.cn

std::string s = "hi";  s += "!";
来源：http://avs.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://ihz.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vqx.jqgfzy.top

[S34] C++：遍历 vector
来源：http://cux.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://cwz.hongshengwenyu.top

[S35] C++：map
来源：http://bpa.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oml.hfpthk.cn

[S36] C++：unordered_map
来源：http://hgt.jinyuanbaomall.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vqk.wangdashe.top

[S37] C++：set
来源：http://prq.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vyn.epnwcf.com

[S38] C++：排序
来源：http://iub.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://zaq.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://ose.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://prl.cheryme.top

[S40] C++：查找元素
来源：http://qvp.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lkf.tian-w.cn

[S41] C++：类与构造函数
来源：http://dmp.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://byc.yuxming.cn

[S42] C++：继承与虚函数
来源：http://nqa.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://epn.iojbl.cn

[S43] C++：智能指针
来源：http://ywd.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://mlc.gzhubu.top

[S44] C++：引用传参
来源：http://qhb.guannengcc.top

void inc(int &x) { ++x; }
来源：http://feu.yueranfly.top

[S45] C++：lambda
来源：http://xxz.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://asi.yangfankeji.com

[S46] C++：函数模板
来源：http://xnm.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://whb.sysykeji.top

[S47] C++：结构化绑定遍历
来源：http://ttp.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dea.gzhubu.top

[S48] C++：逐行读文件
来源：http://udx.wangdashe.top

std::ifstream in("a.txt");  std::string line;
来源：http://hmh.zhiwuduotai.top

while (std::getline(in, line)) { }
来源：http://mix.ehwqpu.com

[S49] C++：写文件
来源：http://zgv.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iqe.cucudq.cn

[S50] C++：格式化数字
来源：http://tex.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bor.yongpay.top

[S51] C++：显式类型转换
来源：http://gdl.nanxuanxn.top

static_cast<double>(a) / b
来源：http://zgr.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://alo.havefunace.top

int size() const noexcept { return n_; }
来源：http://uot.gzhubu.top

[S53] C++：移动语义
来源：http://xrv.zhongyouzk.top

std::vector<int> w = std::move(v);
来源：http://slj.yangfankeji.com

[S54] C++：异常处理
来源：http://bmy.havefunace.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mpu.yonumen.top

[S55] C++：结构化绑定
来源：http://rzr.jinqigfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ivi.yuxming.cn

[S56] C++：optional
来源：http://gio.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ekz.xuanzx.com

[S57] C++：编译期常量
来源：http://cla.mhx1999.top

constexpr int N = 10;
来源：http://jsb.guannengcc.top

[S58] C++：命名空间
来源：http://iig.yfazqb.com


<!-- 参考信息 -->