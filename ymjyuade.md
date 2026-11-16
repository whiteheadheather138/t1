代发 wailian999

[Q80] 字符串截取
来源：http://plq.shanyushiyangtech.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qna.fengsongda.top

[Q81] 字符串替换
来源：http://lfp.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://otw.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://uog.yfazqb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://miz.jqgufenzy.top

[Q83] 大小写转换
来源：http://niv.cucudq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gvz.xinyue.icu

[Q84] 去除首尾空格
来源：http://tsk.fengsongda.top

SELECT TRIM(name) FROM users;
来源：http://etu.zdqjudy.top

[Q85] 数值取整
来源：http://xte.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bpu.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://uew.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wkl.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://cpi.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tne.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://dhj.dashuyun.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rmc.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rvk.gzhubu.top

[Q89] 判断表是否存在
来源：http://jct.daxiang520.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://okm.bjfxy.top

[Q90] 生成序号列
来源：http://kqf.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kny.jqgfzy.top

================================================================================
来源：http://qim.hysaishi.cn

R. Bash 专题
来源：http://iap.havefunace.top

================================================================================
来源：http://vjl.sysykeji.top

[R01] shebang 与严格模式
来源：http://oud.gaohongyu789.top

#!/usr/bin/env bash
来源：http://sco.haohaochexian.top

set -euo pipefail
来源：http://klg.9152youxi.cn

[R02] 变量赋值与使用
来源：http://llu.uphjek.com

name="Tom"; echo "$name"
来源：http://dws.cdnleiting.top

[R03] 只读变量
来源：http://qrd.gaohongyu789.top

readonly PI=3.14
来源：http://ijw.shanyushiyangtech.top

[R04] 位置参数
来源：http://tpo.cucudq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eun.smart0.xyz

[R05] 参数默认值
来源：http://lun.feifeiyinyue.top

name="${1:-default}"
来源：http://mjo.0kj1m.cn

[R06] 判断命令是否存在
来源：http://pxy.gogol.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ine.tianlin.xyz

[R07] if 判断文件
来源：http://fiu.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eqm.yvedp.cn

[R08] 数值比较
来源：http://ssa.gzhubu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://kqp.xylfe.cn

[R09] 字符串比较
来源：http://dcb.haohaochexian.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wfq.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://ymu.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ovp.tianlin.xyz

[R11] case 多分支
来源：http://hzf.jinqigfzy.top

case "$1" in
来源：http://pqq.52xcode.cn

start) echo "启动" ;;
来源：http://czg.wangshuangyany.cn

stop)  echo "停止" ;;
来源：http://mwz.yvedp.cn

*)     echo "未知命令" ;;
来源：http://ocd.shzxlz.cn

esac
来源：http://dcz.yfazqb.com

[R12] for 遍历文件
来源：http://ran.0kj1m.cn

for f in *.txt; do echo "$f"; done
来源：http://ric.birdmap.top

[R13] for 计数循环
来源：http://uzg.zhaomingkeji.xyz

for i in {1..10}; do echo "$i"; done
来源：http://aqv.fanxiaobao.xyz

[R14] C 风格 for
来源：http://bcu.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mjv.daxiang520.top

[R15] while 逐行读文件
来源：http://hnf.yfazqb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oqr.52xcode.cn

[R16] until 等待条件
来源：http://qfq.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gqy.hesvh.cn

[R17] 数组定义与取值
来源：http://nhr.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://aro.c1oappe.top

[R18] 遍历数组
来源：http://zmb.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rji.shuidangran.top

[R19] 数组长度
来源：http://iat.gotoacloud.top

echo "${#arr[@]}"
来源：http://oib.shanyushiyangkeji.top

[R20] 关联数组（字典）
来源：http://wgm.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wsu.hywenlv.cn

[R21] 字符串长度
来源：http://eyd.yonumen.top

echo "${#s}"
来源：http://app.mhx1999.top

[R22] 截取子串
来源：http://wmg.cqqwz.cn

echo "${s:0:5}"
来源：http://rap.smart0.xyz

[R23] 字符串替换
来源：http://nht.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lmd.c1oappe.top

[R24] 大小写转换
来源：http://bes.yvedp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nyo.jinghuilouyu.cn

[R25] 去后缀 / 去前缀
来源：http://qgc.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://myy.aizwys.cn

[R26] 命令替换
来源：http://wsu.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://gqp.hfpthk.cn

[R27] 算术展开
来源：http://rtj.jinqigufen.top

echo $((1 + 2 * 3))
来源：http://zdj.fktsv.cn

[R28] 浮点运算
来源：http://qgh.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://blb.birdmap.top

[R29] 定义函数
来源：http://tbs.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://knd.jinghuilouyu.cn

[R30] 函数返回状态码
来源：http://zny.shangyingyoupin.top

f() { return 0; }; f || echo "失败了"
来源：http://hqk.haohaochexian.top

[R31] 局部变量
来源：http://fyy.xingfuxueyuan.xyz

f() { local x=1; echo "$x"; }
来源：http://byo.pengpengdd.cyou

[R32] 参数个数校验
来源：http://kud.chenjidiqi.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xsf.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://nuf.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pdq.gzhubu.top

[R34] 退出时清理
来源：http://paf.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://qjn.yangfankeji.com

[R35] 后台执行并等待
来源：http://gsn.sxryk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lqj.nwbrower.top

[R36] 并发执行多个任务
来源：http://bhp.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xii.zhaomingkeji.xyz

[R37] 把输出赋给变量
来源：http://jvu.jyoumei.cn

files=$(ls -1)
来源：http://vqf.hammf.cn

[R38] 管道串联
来源：http://wnv.nwbrower.top

cat a.txt | grep -i error | wc -l
来源：http://mxe.yuanzhike.top

[R39] 重定向标准输出与错误
来源：http://lbl.9152youxi.cn

cmd > out.log 2>&1
来源：http://wax.xuanzx.com

[R40] 追加写日志
来源：http://yjd.shangyingyoupin.top

echo "log" >> out.log
来源：http://ajo.zhaomingkeji.xyz

[R41] 丢弃输出
来源：http://sih.haohaochexian.top

cmd >/dev/null 2>&1
来源：http://srx.iojbl.cn

[R42] 输入重定向
来源：http://ljs.nanxuanxn.top

wc -l < a.txt
来源：http://gch.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://dac.andypj.xyz

find . -name "*.log" -type f
来源：http://wdr.ctjpmb.com

[R44] 按修改时间查找
来源：http://bzh.hammf.cn

find . -mtime -7 -type f
来源：http://xht.jqgfzy.top

[R45] 批量删除
来源：http://scn.yj20258.top

find . -name "*.tmp" -delete
来源：http://max.hywenlv.cn

[R46] 递归替换文件内容
来源：http://efb.jianghu66.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yjx.guannengcc.top

[R47] sed 单行替换
来源：http://imu.ybcxt.top

sed -i 's/foo/bar/g' a.txt
来源：http://kzc.hnxiangtu.top

[R48] awk 取指定列
来源：http://hox.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://erl.snrcjt.cn

[R49] awk 带条件
来源：http://zmj.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ppr.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://edn.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://esj.fehbvm.com

[R51] 排序去重取前几
来源：http://rxu.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://dyz.kuanghao11.cn

[R52] 统计行数
来源：http://lzo.ppjwa.cn

wc -l a.txt
来源：http://nzj.yj20258888.top

[R53] 查看文件头与实时尾
来源：http://qtf.c1oappe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uzv.sysykeji.top

[R54] 比较两个文件
来源：http://zyt.daxiang520.top

diff a.txt b.txt
来源：http://ect.0kj1m.cn

[R55] 压缩与解压
来源：http://ynb.aibaodan.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blj.bbcook.cn

[R56] 远程拷贝
来源：http://bjw.sysykeji.top

scp file user@host:/path/
来源：http://ljp.yj202588.top

[R57] 远程执行命令
来源：http://ohg.jlsjyb.cn

ssh user@host 'uptime'
来源：http://kxt.xingfuxueyuan.xyz

[R58] 下载文件
来源：http://rcr.pengpengdd.cyou

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bsp.ppjwa.cn

[R59] 发 POST JSON
来源：http://vzc.fengsongda.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nwn.dashuyun.cn

[R60] 只看 HTTP 状态码
来源：http://njo.epnwcf.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ibt.guowangkeji.top

[R61] 磁盘占用
来源：http://wco.yj20258888.top

df -h;  du -sh *
来源：http://oqm.ppjwa.cn

[R62] 找最占空间的文件
来源：http://zlm.zhixingplan.top

du -ah . | sort -rh | head -10
来源：http://rhe.daxiang520.top

[R63] 内存与进程
来源：http://iht.xylfe.cn

free -h;  ps aux | grep nginx
来源：http://kel.shanyushiyangtech.top

[R64] 结束进程
来源：http://jgx.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://lau.52xcode.cn

[R65] 查看端口占用
来源：http://nlj.bjfxy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kbh.iojbl.cn

[R66] 定时任务
来源：http://twb.nwbrower.top

crontab -e;  crontab -l
来源：http://ulp.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://ffe.sweek.top

openssl rand -hex 16
来源：http://vcs.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://klb.shzxlz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pst.gogol.net.cn

[R69] 生成随机密码
来源：http://xdl.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://czy.sxryk.cn

[R70] 时间戳与互转
来源：http://dqu.xuetiantiany.cn

date +%s;  date -d @1700000000
来源：http://ide.ehwqpu.com

[R71] 日期格式化
来源：http://cqz.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://olm.yuanzhike.top

[R72] 等待端口就绪
来源：http://emk.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://isr.hongshengwenyu.top

[R73] 分割大日志
来源：http://xxw.sweek.top

split -l 1000 big.log part_
来源：http://emt.zhiwuduotai.top

[R74] 批量重命名
来源：http://rga.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lpy.shzxlz.cn

[R75] 导出环境变量
来源：http://twb.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://zit.ehwqpu.com

[R76] 使用临时文件
来源：http://unr.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://utb.smart0.xyz

[R77] 读取用户输入
来源：http://sfh.gzhubu.top

read -rp "请输入: " ans
来源：http://tqf.mhx1999.top

[R78] 交互式菜单
来源：http://zdo.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ziz.zhoulong.xyz

[R79] 解析命令行选项
来源：http://mkw.316326.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mzw.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://wzj.shanyushiyangtech.top

time ./run.sh
来源：http://mgm.sweek.top

================================================================================
来源：http://osn.chenjidiqi.icu

S. C / C++ 专题
来源：http://hpr.dianchejie.cn

================================================================================
来源：http://nqk.mhx1999.top

[S01] C：Hello World
来源：http://ncx.sweek.top

#include <stdio.h>
来源：http://hux.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://psk.redwolf501.top

[S02] C：变量与格式化输出
来源：http://muz.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://ael.cheryme.top

[S03] C：读入整数
来源：http://ezw.cdnleiting.top

int x; scanf("%d", &x);
来源：http://kre.hysaishi.cn

[S04] C：字符串复制
来源：http://mdh.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://osh.jyoumei.cn

[S05] C：字符串长度
来源：http://kjp.ydjk.org.cn

strlen(s)
来源：http://obp.redwolf501.top

[S06] C：字符串比较
来源：http://chd.zhaomingkeji.xyz

strcmp(a, b) == 0
来源：http://xqq.shanyushiyangtech.top

[S07] C：数组遍历求和
来源：http://qns.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://csx.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://cub.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yzh.sjlbkw.cn

[S09] C：结构体定义与初始化
来源：http://myn.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qhb.fehbvm.com

[S10] C：指针与解引用
来源：http://uqe.smart0.xyz

int *p = &a;  *p = 5;
来源：http://qgu.hcnkem.com

[S11] C：逐行读文件
来源：http://iwx.yfazqb.com

FILE *f = fopen("a.txt", "r");
来源：http://esg.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pwg.zhiwuduotai.top

fclose(f);
来源：http://rav.redwolf501.top

[S12] C：写文件
来源：http://vws.fehbvm.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hrr.yj20258.top

[S13] C：宏定义
来源：http://kme.yj20258.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kee.daria6918.cn

[S14] C：枚举
来源：http://bar.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://uus.ehwqpu.com

[S15] C：类型转换
来源：http://aez.yvedp.cn

(double) a / b
来源：http://qzp.gaohongyu789.top

[S16] C：位操作置位
来源：http://snc.52xcode.cn

x |= (1 << 3);
来源：http://ssp.hnqzz.top

[S17] C：安全拼接字符串
来源：http://hgo.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eyv.yj202588.top

[S18] C：命令行参数
来源：http://igt.nanxinkj.top

int main(int argc, char **argv)
来源：http://sxi.aibaodan.cn

[S19] C：快速排序
来源：http://oia.aibaodan.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iou.xylfe.cn

[S20] C：二分查找
来源：http://veg.epnwcf.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vig.hnxiangtu.top

[S21] C：字符类别判断
来源：http://ans.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kih.yanxiufei.cn

[S22] C：字符串转数字
来源：http://hah.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fan.tarul.cn

[S23] C：随机数
来源：http://dvf.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://auo.havefunace.top

[S24] C：获取本地时间
来源：http://ydv.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pos.gogol.net.cn

[S25] C：内存拷贝
来源：http://yko.jiagoushi.top

memcpy(dst, src, n);
来源：http://bxh.nanxinkj.top

[S26] C：内存清零
来源：http://lns.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://unj.fehbvm.com

[S27] C：定义常量
来源：http://bpk.kuanghao11.cn

const double PI = 3.14159;
来源：http://vpf.iojbl.cn

[S28] C：静态变量
来源：http://keo.ppjwa.cn

static int counter = 0;
来源：http://fqw.xziqi.cn

[S29] C：变参函数
来源：http://frk.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cdf.chenjidiqi.icu

[S30] C：头文件保护
来源：http://gir.quarkkingdee.top

#ifndef X_H
来源：http://nsr.jiagoushi.top

#define X_H
来源：http://wfo.hongshengwenyu.top

#endif
来源：http://aal.zhengqikj.top

[S31] C++：Hello World
来源：http://ypp.andypj.xyz

#include <iostream>
来源：http://nou.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://ogh.0kj1m.cn

[S32] C++：字符串
来源：http://acj.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://snh.aizwys.cn

[S33] C++：vector 增删
来源：http://mzh.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gom.yj202588.top

[S34] C++：遍历 vector
来源：http://kee.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://tig.jinqigufen.top

[S35] C++：map
来源：http://ycm.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://exc.cdnleiting.top

[S36] C++：unordered_map
来源：http://pnj.ctjpmb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xty.cucudq.cn

[S37] C++：set
来源：http://lvq.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://abh.ehwqpu.com

[S38] C++：排序
来源：http://cnk.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://eel.shanyushiyangtech.top

[S39] C++：自定义比较器排序
来源：http://aci.ydzc1.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dhe.smart0.xyz

[S40] C++：查找元素
来源：http://bph.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://awi.316326.xyz

[S41] C++：类与构造函数
来源：http://eff.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oiq.redwolf501.top

[S42] C++：继承与虚函数
来源：http://wda.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://ovd.ybcxt.top

[S43] C++：智能指针
来源：http://xwc.snrcjt.cn

auto p = std::make_unique<int>(5);
来源：http://che.zhengqikj.top

[S44] C++：引用传参
来源：http://xyn.jianghu66.top

void inc(int &x) { ++x; }
来源：http://uuc.ivvv.top

[S45] C++：lambda
来源：http://vnp.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://ieh.ywan-chungtsiang.top

[S46] C++：函数模板
来源：http://qkd.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zfo.sxryk.cn

[S47] C++：结构化绑定遍历
来源：http://qpz.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xgt.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://cwe.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tzk.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://fuz.chenlongwang.top

[S49] C++：写文件
来源：http://hvt.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://khu.xylfe.cn

[S50] C++：格式化数字
来源：http://hzu.jinghuilouyu.cn


<!-- 参考信息 -->