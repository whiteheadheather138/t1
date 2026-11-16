代发 wailian999

[Q86] 读取 JSON 字段
来源：http://ozx.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://idt.yuxming.cn

[Q87] JSON 字段做条件
来源：http://bmr.zhoulong.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wol.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://tze.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vzt.wangshuangyany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://axi.quarkkingdee.top

[Q89] 判断表是否存在
来源：http://bvp.hfpthk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.bbcook.cn

[Q90] 生成序号列
来源：http://pkq.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rmb.fehbvm.com

================================================================================
来源：http://xvx.cdnleiting.top

R. Bash 专题
来源：http://elv.xuanzx.com

================================================================================
来源：http://cyx.nwbrower.top

[R01] shebang 与严格模式
来源：http://ady.316326.xyz

#!/usr/bin/env bash
来源：http://xaz.jqgufenzy.top

set -euo pipefail
来源：http://wgn.daria6918.cn

[R02] 变量赋值与使用
来源：http://woh.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://gvh.jinqigufen.top

[R03] 只读变量
来源：http://yzm.fzhhl.top

readonly PI=3.14
来源：http://zgq.yuxming.cn

[R04] 位置参数
来源：http://dwm.hnxiangtu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tcz.chenjidiqi.icu

[R05] 参数默认值
来源：http://iuc.nanxinkj.top

name="${1:-default}"
来源：http://mia.zhiwuduotai.top

[R06] 判断命令是否存在
来源：http://ilv.dianchejie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mxu.jinghuilouyu.cn

[R07] if 判断文件
来源：http://vaj.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mlk.hnqzz.top

[R08] 数值比较
来源：http://bir.c1oappe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uva.zhijiandao.cn

[R09] 字符串比较
来源：http://svx.zhongyouzk.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zym.zhixingplan.top

[R10] 正则匹配
来源：http://nvk.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mma.feifeiyinyue.top

[R11] case 多分支
来源：http://glq.sysykeji.top

case "$1" in
来源：http://ahf.yuxming.cn

start) echo "启动" ;;
来源：http://lyq.hnqzz.top

stop)  echo "停止" ;;
来源：http://fhy.yj202588.top

*)     echo "未知命令" ;;
来源：http://wzv.yueranfly.top

esac
来源：http://ymg.redwolf501.top

[R12] for 遍历文件
来源：http://kmf.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://suq.shanyushiyangtech.top

[R13] for 计数循环
来源：http://oza.chenlongwang.top

for i in {1..10}; do echo "$i"; done
来源：http://qrq.chenzaomai.com

[R14] C 风格 for
来源：http://hku.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://weo.guowangkeji.top

[R15] while 逐行读文件
来源：http://qaw.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://avb.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://imn.ehwqpu.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ebk.cqqwz.cn

[R17] 数组定义与取值
来源：http://mhk.fzhhl.top

arr=(a b c); echo "${arr[0]}"
来源：http://xff.yanxiufei.cn

[R18] 遍历数组
来源：http://luw.guannengcc.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kln.gzhubu.top

[R19] 数组长度
来源：http://kpe.jinqigfzy.top

echo "${#arr[@]}"
来源：http://xmp.yuxming.cn

[R20] 关联数组（字典）
来源：http://ycb.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://udn.xylfe.cn

[R21] 字符串长度
来源：http://vlg.daria6918.cn

echo "${#s}"
来源：http://soh.fehbvm.com

[R22] 截取子串
来源：http://bcz.aizwys.cn

echo "${s:0:5}"
来源：http://ncv.xinyue.icu

[R23] 字符串替换
来源：http://gue.tanke756.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kqe.kuanghao11.cn

[R24] 大小写转换
来源：http://aee.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pqd.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://ona.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://sos.pengpengdd.cyou

[R26] 命令替换
来源：http://pwt.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://xyr.epnwcf.com

[R27] 算术展开
来源：http://qxz.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://zzt.ctjpmb.com

[R28] 浮点运算
来源：http://vrx.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://ffm.zhaomingkeji.xyz

[R29] 定义函数
来源：http://tez.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zwh.iojbl.cn

[R30] 函数返回状态码
来源：http://ebg.wangshuangyany.cn

f() { return 0; }; f || echo "失败了"
来源：http://umt.hammf.cn

[R31] 局部变量
来源：http://xta.gogol.net.cn

f() { local x=1; echo "$x"; }
来源：http://tnt.xinyue.icu

[R32] 参数个数校验
来源：http://qhy.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rrz.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://pau.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vwo.dianchejie.cn

[R34] 退出时清理
来源：http://yvb.fanxiaobao.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://cuq.aibaodan.cn

[R35] 后台执行并等待
来源：http://dhr.pengpengdd.cyou

sleep 5 & pid=$!; wait "$pid"
来源：http://izq.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://jtz.zhongyouzk.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xnv.xingfuxueyuan.xyz

[R37] 把输出赋给变量
来源：http://yvf.yueranfly.top

files=$(ls -1)
来源：http://cce.zhixingplan.top

[R38] 管道串联
来源：http://tcm.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://zxe.hnqzz.top

[R39] 重定向标准输出与错误
来源：http://zgf.ehwqpu.com

cmd > out.log 2>&1
来源：http://pcc.feifeiyinyue.top

[R40] 追加写日志
来源：http://tre.aizwys.cn

echo "log" >> out.log
来源：http://dle.9152youxi.cn

[R41] 丢弃输出
来源：http://luh.yj20258888.top

cmd >/dev/null 2>&1
来源：http://qnr.shzxlz.cn

[R42] 输入重定向
来源：http://ena.chenzaomai.com

wc -l < a.txt
来源：http://hdm.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://mci.jyoumei.cn

find . -name "*.log" -type f
来源：http://ltg.quarkkingdee.top

[R44] 按修改时间查找
来源：http://sso.aizwys.cn

find . -mtime -7 -type f
来源：http://hug.sweek.top

[R45] 批量删除
来源：http://wzu.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://bms.andypj.xyz

[R46] 递归替换文件内容
来源：http://uft.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wrd.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://arv.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://ybl.gaohongyu789.top

[R48] awk 取指定列
来源：http://how.ydjk.org.cn

awk '{print $1, $3}' a.txt
来源：http://ojs.9152youxi.cn

[R49] awk 带条件
来源：http://ped.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qts.guannengcc.top

[R50] awk 求和
来源：http://xqs.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://oqx.c1oappe.top

[R51] 排序去重取前几
来源：http://pyg.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://non.9152youxi.cn

[R52] 统计行数
来源：http://xtn.sxryk.cn

wc -l a.txt
来源：http://wna.52xcode.cn

[R53] 查看文件头与实时尾
来源：http://rwl.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mcf.yj20258.top

[R54] 比较两个文件
来源：http://xbo.chenlongwang.top

diff a.txt b.txt
来源：http://vwp.gzhubu.top

[R55] 压缩与解压
来源：http://hva.fanxiaobao.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dyj.epnwcf.com

[R56] 远程拷贝
来源：http://wlm.epnwcf.com

scp file user@host:/path/
来源：http://ipo.chenlongwang.top

[R57] 远程执行命令
来源：http://ftr.nanxinkj.top

ssh user@host 'uptime'
来源：http://pxr.uphjek.com

[R58] 下载文件
来源：http://mfo.jlsjyb.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kgb.hcnkem.com

[R59] 发 POST JSON
来源：http://xua.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qfh.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://mys.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tjj.jqgfzy.top

[R61] 磁盘占用
来源：http://ahg.tianlin.xyz

df -h;  du -sh *
来源：http://bln.chenlongwang.top

[R62] 找最占空间的文件
来源：http://rpc.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://ssn.tian-w.cn

[R63] 内存与进程
来源：http://yxs.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://xru.hongshengwenyu.top

[R64] 结束进程
来源：http://gnr.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://rit.zhengqikj.top

[R65] 查看端口占用
来源：http://lim.sysykeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iue.jianghu66.top

[R66] 定时任务
来源：http://gjg.52xcode.cn

crontab -e;  crontab -l
来源：http://fpj.havefunace.top

[R67] 生成随机十六进制串
来源：http://zpk.jinghuilouyu.cn

openssl rand -hex 16
来源：http://avx.guannengcc.top

[R68] 计算文件校验值
来源：http://umf.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://owk.0kj1m.cn

[R69] 生成随机密码
来源：http://bxv.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://ypp.wangdashe.top

[R70] 时间戳与互转
来源：http://xrl.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://smz.daxiang520.top

[R71] 日期格式化
来源：http://non.nwbrower.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zkt.jlsjyb.cn

[R72] 等待端口就绪
来源：http://efk.xingfuxueyuan.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://qch.daria6918.cn

[R73] 分割大日志
来源：http://rkj.chenjidiqi.icu

split -l 1000 big.log part_
来源：http://brt.shzxlz.cn

[R74] 批量重命名
来源：http://fzv.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wiv.yueranfly.top

[R75] 导出环境变量
来源：http://orp.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://lpj.gotoacloud.top

[R76] 使用临时文件
来源：http://ixj.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ddq.0kj1m.cn

[R77] 读取用户输入
来源：http://nyv.mhx1999.top

read -rp "请输入: " ans
来源：http://fba.jqgufenzy.top

[R78] 交互式菜单
来源：http://qva.sjlbkw.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xco.ydzc1.top

[R79] 解析命令行选项
来源：http://ktz.cqqwz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xkf.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://apt.fzhhl.top

time ./run.sh
来源：http://mem.nanxuanxn.top

================================================================================
来源：http://tme.xylfe.cn

S. C / C++ 专题
来源：http://tjs.jqgfzy.top

================================================================================
来源：http://flc.xuetiantiany.cn

[S01] C：Hello World
来源：http://zlx.jlsjyb.cn

#include <stdio.h>
来源：http://rus.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ban.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://cfp.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://sdr.yuxming.cn

[S03] C：读入整数
来源：http://gbd.cheryme.top

int x; scanf("%d", &x);
来源：http://zym.feifeiyinyue.top

[S04] C：字符串复制
来源：http://zdz.ehwqpu.com

char dst[32]; strcpy(dst, "hi");
来源：http://jov.feifeiyinyue.top

[S05] C：字符串长度
来源：http://gle.yanxiufei.cn

strlen(s)
来源：http://tyl.yanxiufei.cn

[S06] C：字符串比较
来源：http://ltz.uphjek.com

strcmp(a, b) == 0
来源：http://ahp.zhixingplan.top

[S07] C：数组遍历求和
来源：http://pyq.havefunace.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ipl.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://xiy.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jto.fktsv.cn

[S09] C：结构体定义与初始化
来源：http://sda.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uhb.ppjwa.cn

[S10] C：指针与解引用
来源：http://nuh.zycfv.cn

int *p = &a;  *p = 5;
来源：http://gva.tianlin.xyz

[S11] C：逐行读文件
来源：http://poy.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://vps.xingfuxueyuan.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://yzc.hesvh.cn

fclose(f);
来源：http://xye.52xcode.cn

[S12] C：写文件
来源：http://gjn.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://glu.fktsv.cn

[S13] C：宏定义
来源：http://hgf.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ykl.cheryme.top

[S14] C：枚举
来源：http://mwg.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://yxt.hnxiangtu.top

[S15] C：类型转换
来源：http://zbd.chenjidiqi.icu

(double) a / b
来源：http://gym.yuxming.cn

[S16] C：位操作置位
来源：http://aua.gzhubu.top

x |= (1 << 3);
来源：http://nll.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://vbn.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gbq.havefunace.top

[S18] C：命令行参数
来源：http://rvf.jqgufenzy.top

int main(int argc, char **argv)
来源：http://sbz.yfazqb.com

[S19] C：快速排序
来源：http://muh.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://wih.fzhhl.top

[S20] C：二分查找
来源：http://ivi.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lqz.hammf.cn

[S21] C：字符类别判断
来源：http://wxy.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ddk.fzhhl.top

[S22] C：字符串转数字
来源：http://mop.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://qap.fktsv.cn

[S23] C：随机数
来源：http://ciy.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uma.havefunace.top

[S24] C：获取本地时间
来源：http://eru.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://msq.hfpthk.cn

[S25] C：内存拷贝
来源：http://gwp.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://wxd.sjlbkw.cn

[S26] C：内存清零
来源：http://bbq.uphjek.com

memset(a, 0, sizeof a);
来源：http://szj.ctjpmb.com

[S27] C：定义常量
来源：http://qnq.andypj.xyz

const double PI = 3.14159;
来源：http://lvk.nanxinkj.top

[S28] C：静态变量
来源：http://gre.zdqjudy.top

static int counter = 0;
来源：http://foo.yangfankeji.com

[S29] C：变参函数
来源：http://zgx.zycfv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hqt.zhiwuduotai.top

[S30] C：头文件保护
来源：http://kkq.vqdsnc.cn

#ifndef X_H
来源：http://jid.mhx1999.top

#define X_H
来源：http://tbf.nwbrower.top

#endif
来源：http://rqi.shanyushiyangtech.top

[S31] C++：Hello World
来源：http://gtf.jinqigfzy.top

#include <iostream>
来源：http://xgt.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://eyk.wangdashe.top

[S32] C++：字符串
来源：http://fdq.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://clo.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://qzy.cashguo.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uhz.gzhubu.top

[S34] C++：遍历 vector
来源：http://ujc.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://pvr.sjlbkw.cn

[S35] C++：map
来源：http://uxz.zhijiandao.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nsu.guannengcc.top

[S36] C++：unordered_map
来源：http://mhc.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://umj.yj202588.top

[S37] C++：set
来源：http://ovq.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wns.hfpthk.cn

[S38] C++：排序
来源：http://rij.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://kol.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://ghk.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gyw.epnwcf.com

[S40] C++：查找元素
来源：http://ygf.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tak.daxiang520.top

[S41] C++：类与构造函数
来源：http://mda.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ije.wangdashe.top

[S42] C++：继承与虚函数
来源：http://uhe.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://zgk.tanke756.top

[S43] C++：智能指针
来源：http://kdi.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://spe.jlsjyb.cn

[S44] C++：引用传参
来源：http://nxa.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://qay.hnqzz.top

[S45] C++：lambda
来源：http://ohx.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://iot.zhengqikj.top

[S46] C++：函数模板
来源：http://wmt.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ufl.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://hat.fktsv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kyk.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://hoj.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://xbm.jiagoushi.top

while (std::getline(in, line)) { }
来源：http://pys.xylfe.cn

[S49] C++：写文件
来源：http://jfa.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fwh.tianlin.xyz

[S50] C++：格式化数字
来源：http://cqu.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zpk.nwbrower.top

[S51] C++：显式类型转换
来源：http://iew.fehbvm.com

static_cast<double>(a) / b
来源：http://oxs.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://rks.fanxiaobao.xyz

int size() const noexcept { return n_; }
来源：http://dko.iojbl.cn

[S53] C++：移动语义
来源：http://spi.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://waj.ivvv.top

[S54] C++：异常处理
来源：http://hxl.jianghu66.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wtd.nanxuanxn.top

[S55] C++：结构化绑定
来源：http://uab.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nkp.ehwqpu.com

[S56] C++：optional
来源：http://wpd.fanxiaobao.xyz


<!-- 参考信息 -->