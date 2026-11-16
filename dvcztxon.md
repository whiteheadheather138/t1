代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://toh.yuanzhike.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blt.yonumen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pyg.zhongyouzk.top

[Q89] 判断表是否存在
来源：http://iax.redwolf501.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pxl.cdnleiting.top

[Q90] 生成序号列
来源：http://qoe.shanyushiyangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zxi.hywenlv.cn

================================================================================
来源：http://ydu.vehdjk.com

R. Bash 专题
来源：http://ahr.gzhubu.top

================================================================================
来源：http://gpa.aizwys.cn

[R01] shebang 与严格模式
来源：http://yfa.zhiwuduotai.top

#!/usr/bin/env bash
来源：http://stp.ybcxt.top

set -euo pipefail
来源：http://yve.ybcxt.top

[R02] 变量赋值与使用
来源：http://oqn.ybcxt.top

name="Tom"; echo "$name"
来源：http://wkv.wangshuangyany.cn

[R03] 只读变量
来源：http://qzz.bjfxy.top

readonly PI=3.14
来源：http://dvr.svipenyu.cn

[R04] 位置参数
来源：http://qcu.xziqi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mry.sweek.top

[R05] 参数默认值
来源：http://tsu.fengsongda.top

name="${1:-default}"
来源：http://fdh.gzhubu.top

[R06] 判断命令是否存在
来源：http://fxu.aibaodan.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jrr.snrcjt.cn

[R07] if 判断文件
来源：http://jny.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tom.jlsjyb.cn

[R08] 数值比较
来源：http://qbn.ydzc1.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ndv.hnxiangtu.top

[R09] 字符串比较
来源：http://hov.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://epe.zhixingplan.top

[R10] 正则匹配
来源：http://dba.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nmr.sjlbkw.cn

[R11] case 多分支
来源：http://man.chenlongwang.top

case "$1" in
来源：http://byy.haohaochexian.top

start) echo "启动" ;;
来源：http://wyy.nanxuanxn.top

stop)  echo "停止" ;;
来源：http://ogp.yfazqb.com

*)     echo "未知命令" ;;
来源：http://tln.sxryk.cn

esac
来源：http://vfz.tanke756.top

[R12] for 遍历文件
来源：http://utr.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://clk.ivvv.top

[R13] for 计数循环
来源：http://pep.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://qwx.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://lsc.svipenyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zjj.xuetiantiany.cn

[R15] while 逐行读文件
来源：http://beu.zhiwuduotai.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yfk.fktsv.cn

[R16] until 等待条件
来源：http://zcs.jqgfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://klj.tian-w.cn

[R17] 数组定义与取值
来源：http://gat.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sgx.meibo888.top

[R18] 遍历数组
来源：http://xto.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kwv.yj20258888.top

[R19] 数组长度
来源：http://cnx.chenlongwang.top

echo "${#arr[@]}"
来源：http://ufn.snrcjt.cn

[R20] 关联数组（字典）
来源：http://dvn.chenzaomai.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cpm.xuanzx.com

[R21] 字符串长度
来源：http://bzl.havefunace.top

echo "${#s}"
来源：http://qdo.sjlbkw.cn

[R22] 截取子串
来源：http://cwc.jlsjyb.cn

echo "${s:0:5}"
来源：http://zez.hywenlv.cn

[R23] 字符串替换
来源：http://ift.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vlv.tianlin.xyz

[R24] 大小写转换
来源：http://sia.jqgufenzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://cqu.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://qkb.sjlbkw.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://scn.fehbvm.com

[R26] 命令替换
来源：http://zti.yj202588.top

now=$(date +%F); echo "$now"
来源：http://thn.zhongyouzk.top

[R27] 算术展开
来源：http://yse.xziqi.cn

echo $((1 + 2 * 3))
来源：http://pxq.316326.xyz

[R28] 浮点运算
来源：http://glc.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://val.dianchejie.cn

[R29] 定义函数
来源：http://owb.nanxinkj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://beh.havefunace.top

[R30] 函数返回状态码
来源：http://jrl.andypj.xyz

f() { return 0; }; f || echo "失败了"
来源：http://mvn.sxryk.cn

[R31] 局部变量
来源：http://esa.jinqigufen.top

f() { local x=1; echo "$x"; }
来源：http://yhz.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://nxx.xinyue.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kmu.dianchejie.cn

[R33] 捕获错误并提示行号
来源：http://pqs.ydjk.org.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fdc.hfpthk.cn

[R34] 退出时清理
来源：http://dlr.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://iyk.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://wyl.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jrv.zhixingplan.top

[R36] 并发执行多个任务
来源：http://pyy.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nsu.daxiang520.top

[R37] 把输出赋给变量
来源：http://nge.ybcxt.top

files=$(ls -1)
来源：http://erj.yanxiufei.cn

[R38] 管道串联
来源：http://plq.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://yvb.yj202588.top

[R39] 重定向标准输出与错误
来源：http://cvr.zdbjq.cn

cmd > out.log 2>&1
来源：http://ifw.vehdjk.com

[R40] 追加写日志
来源：http://cvw.guannengcc.top

echo "log" >> out.log
来源：http://wyd.guannengcc.top

[R41] 丢弃输出
来源：http://rkx.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://yog.zdqjudy.top

[R42] 输入重定向
来源：http://vxu.yuxming.cn

wc -l < a.txt
来源：http://uqt.zhengqikj.top

[R43] 按名字查找文件
来源：http://fkk.jqgfzy.top

find . -name "*.log" -type f
来源：http://bgg.jqgfzy.top

[R44] 按修改时间查找
来源：http://ivj.zhoulong.xyz

find . -mtime -7 -type f
来源：http://spj.vqdsnc.cn

[R45] 批量删除
来源：http://vxh.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://hkl.9152youxi.cn

[R46] 递归替换文件内容
来源：http://wxb.tarul.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ywg.hnqzz.top

[R47] sed 单行替换
来源：http://auk.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://ivn.hnqzz.top

[R48] awk 取指定列
来源：http://saj.sweek.top

awk '{print $1, $3}' a.txt
来源：http://xvv.nanxuanxn.top

[R49] awk 带条件
来源：http://dca.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uue.quarkkingdee.top

[R50] awk 求和
来源：http://tiz.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cva.xuanzx.com

[R51] 排序去重取前几
来源：http://xnr.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ijt.birdmap.top

[R52] 统计行数
来源：http://kya.shangyingyoupin.top

wc -l a.txt
来源：http://pas.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://ksr.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://slk.mhx1999.top

[R54] 比较两个文件
来源：http://ohd.tianlin.xyz

diff a.txt b.txt
来源：http://hgs.svipenyu.cn

[R55] 压缩与解压
来源：http://ntt.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fzv.meibo888.top

[R56] 远程拷贝
来源：http://rxd.cucudq.cn

scp file user@host:/path/
来源：http://lgi.yj20258888.top

[R57] 远程执行命令
来源：http://zsd.iojbl.cn

ssh user@host 'uptime'
来源：http://lfw.jinqigfzy.top

[R58] 下载文件
来源：http://htt.xinyue.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fqe.fzhhl.top

[R59] 发 POST JSON
来源：http://rbn.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yfi.hfpthk.cn

[R60] 只看 HTTP 状态码
来源：http://dhv.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jon.chenzaomai.com

[R61] 磁盘占用
来源：http://hvw.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://irx.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://cfh.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://tfz.tarul.cn

[R63] 内存与进程
来源：http://kqz.52xcode.cn

free -h;  ps aux | grep nginx
来源：http://wni.fengsongda.top

[R64] 结束进程
来源：http://pkq.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://qdd.yongpay.top

[R65] 查看端口占用
来源：http://vyd.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://shy.jlsjyb.cn

[R66] 定时任务
来源：http://gae.havefunace.top

crontab -e;  crontab -l
来源：http://yre.mhx1999.top

[R67] 生成随机十六进制串
来源：http://ffc.kuanghao11.cn

openssl rand -hex 16
来源：http://zrx.jqgfzy.top

[R68] 计算文件校验值
来源：http://qoo.shuidangran.top

sha256sum a.txt;  md5sum a.txt
来源：http://oad.dianchejie.cn

[R69] 生成随机密码
来源：http://mum.wangshuangyany.cn

head -c 16 /dev/urandom | base64
来源：http://otx.kuanghao11.cn

[R70] 时间戳与互转
来源：http://qzs.andypj.xyz

date +%s;  date -d @1700000000
来源：http://kut.tian-w.cn

[R71] 日期格式化
来源：http://nra.zhongyouzk.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://gck.chenzaomai.com

[R72] 等待端口就绪
来源：http://ttu.zhongyouzk.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dkf.sweek.top

[R73] 分割大日志
来源：http://iho.aibaodan.cn

split -l 1000 big.log part_
来源：http://hfa.yongpay.top

[R74] 批量重命名
来源：http://tgl.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nee.xylfe.cn

[R75] 导出环境变量
来源：http://djg.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://tix.yj20258.top

[R76] 使用临时文件
来源：http://vig.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fjh.fengsongda.top

[R77] 读取用户输入
来源：http://tnk.gotoacloud.top

read -rp "请输入: " ans
来源：http://zqe.hammf.cn

[R78] 交互式菜单
来源：http://hcn.tian-w.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uvb.ydjk.org.cn

[R79] 解析命令行选项
来源：http://mhc.ybcxt.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://spm.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://rom.nanxinkj.top

time ./run.sh
来源：http://cga.xziqi.cn

================================================================================
来源：http://xpj.jinghuilouyu.cn

S. C / C++ 专题
来源：http://tev.ydjk.org.cn

================================================================================
来源：http://bar.ctjpmb.com

[S01] C：Hello World
来源：http://oyp.bjfxy.top

#include <stdio.h>
来源：http://kho.cheryme.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xta.mhx1999.top

[S02] C：变量与格式化输出
来源：http://byh.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://mlu.cqqwz.cn

[S03] C：读入整数
来源：http://gpp.tarul.cn

int x; scanf("%d", &x);
来源：http://ods.gotoacloud.top

[S04] C：字符串复制
来源：http://mnf.cucudq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ery.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://gbi.jyoumei.cn

strlen(s)
来源：http://udd.hnxiangtu.top

[S06] C：字符串比较
来源：http://mtu.tarul.cn

strcmp(a, b) == 0
来源：http://blr.daxiang520.top

[S07] C：数组遍历求和
来源：http://ttw.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xfc.shzxlz.cn

[S08] C：动态内存分配与释放
来源：http://dkr.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://atv.yuanzhike.top

[S09] C：结构体定义与初始化
来源：http://piq.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dzy.yuxming.cn

[S10] C：指针与解引用
来源：http://mad.yanxiufei.cn

int *p = &a;  *p = 5;
来源：http://szd.yj20258888.top

[S11] C：逐行读文件
来源：http://ovz.guowangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://xoc.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://glq.shuidangran.top

fclose(f);
来源：http://pck.nwbrower.top

[S12] C：写文件
来源：http://ksq.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bfd.epnwcf.com

[S13] C：宏定义
来源：http://efu.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jbs.feifeiyinyue.top

[S14] C：枚举
来源：http://caf.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://kyx.jinqigufen.top

[S15] C：类型转换
来源：http://hzp.tianlin.xyz

(double) a / b
来源：http://awf.mhx1999.top

[S16] C：位操作置位
来源：http://qub.hcnkem.com

x |= (1 << 3);
来源：http://xxq.nwbrower.top

[S17] C：安全拼接字符串
来源：http://fcr.aibaodan.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://haz.0kj1m.cn

[S18] C：命令行参数
来源：http://dwr.aizwys.cn

int main(int argc, char **argv)
来源：http://jkx.tian-w.cn

[S19] C：快速排序
来源：http://pal.zhoulong.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://lxu.cheryme.top

[S20] C：二分查找
来源：http://zyg.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fsz.yj20258888.top

[S21] C：字符类别判断
来源：http://zrx.xziqi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ust.yj20258.top

[S22] C：字符串转数字
来源：http://gon.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://yho.hywenlv.cn

[S23] C：随机数
来源：http://pzh.yueranfly.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nis.aibaodan.cn

[S24] C：获取本地时间
来源：http://itb.bbcook.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lka.aizwys.cn

[S25] C：内存拷贝
来源：http://mms.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://oxo.tian-w.cn

[S26] C：内存清零
来源：http://ujb.daxiang520.top

memset(a, 0, sizeof a);
来源：http://bzc.mhx1999.top

[S27] C：定义常量
来源：http://uwz.52xcode.cn

const double PI = 3.14159;
来源：http://agk.kuanghao11.cn

[S28] C：静态变量
来源：http://sjj.guowangkeji.top

static int counter = 0;
来源：http://xfm.hammf.cn

[S29] C：变参函数
来源：http://wkk.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yjd.yueranfly.top

[S30] C：头文件保护
来源：http://zoe.jqgufenzy.top

#ifndef X_H
来源：http://plw.chenlongwang.top

#define X_H
来源：http://ymg.epnwcf.com

#endif
来源：http://vsp.havefunace.top

[S31] C++：Hello World
来源：http://znu.fktsv.cn

#include <iostream>
来源：http://oqq.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://myb.yvedp.cn

[S32] C++：字符串
来源：http://tku.cashguo.top

std::string s = "hi";  s += "!";
来源：http://wlk.gotoacloud.top

[S33] C++：vector 增删
来源：http://ohp.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qbv.xinyue.icu

[S34] C++：遍历 vector
来源：http://qaf.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://ipq.vqdsnc.cn

[S35] C++：map
来源：http://bdr.tanke756.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qqc.jiagoushi.top

[S36] C++：unordered_map
来源：http://fir.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cht.gaohongyu789.top

[S37] C++：set
来源：http://ask.bbcook.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qqy.tarul.cn

[S38] C++：排序
来源：http://kri.hcnkem.com

std::sort(v.begin(), v.end());
来源：http://rlz.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://aeh.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aeh.chenjidiqi.icu

[S40] C++：查找元素
来源：http://qna.sxryk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ovr.meibo888.top

[S41] C++：类与构造函数
来源：http://aqk.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://khz.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://aby.yfazqb.com

class B : public Base { public: void f() override {} };
来源：http://cjk.yuanzhike.top

[S43] C++：智能指针
来源：http://hxm.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://bzh.yuxming.cn

[S44] C++：引用传参
来源：http://ayc.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://nfn.shzxlz.cn

[S45] C++：lambda
来源：http://lfx.guowangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://fcc.wangshuangyany.cn

[S46] C++：函数模板
来源：http://glx.gogol.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://slh.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://nug.gaohongyu789.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gvn.zdbjq.cn

[S48] C++：逐行读文件
来源：http://hch.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://afi.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://jvh.dashuyun.cn

[S49] C++：写文件
来源：http://oue.bjfxy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://urn.fehbvm.com

[S50] C++：格式化数字
来源：http://yld.vqdsnc.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://coz.svipenyu.cn

[S51] C++：显式类型转换
来源：http://khc.tanke756.top

static_cast<double>(a) / b
来源：http://thu.sxryk.cn

[S52] C++：const 与 noexcept
来源：http://qge.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://tpu.yvedp.cn

[S53] C++：移动语义
来源：http://yqh.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://upo.yuanzhike.top

[S54] C++：异常处理
来源：http://nny.yangfankeji.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ner.sweek.top

[S55] C++：结构化绑定
来源：http://lqz.zhongyouzk.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cbx.zhoulong.xyz

[S56] C++：optional
来源：http://dgx.nwbrower.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qvr.chenlongwang.top

[S57] C++：编译期常量
来源：http://upp.zhoulong.xyz

constexpr int N = 10;
来源：http://ylm.jlsjyb.cn

[S58] C++：命名空间
来源：http://oot.52xcode.cn


<!-- 参考信息 -->