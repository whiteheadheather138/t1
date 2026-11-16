代发 wailian999

ANALYZE TABLE users;
来源：http://kjc.yangfankeji.com

[Q71] 查看建表语句
来源：http://qik.sufxvd.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://faq.xuetiantiany.cn

[Q72] 查看索引
来源：http://mcw.yangfankeji.com

SHOW INDEX FROM users;
来源：http://vjt.yanxiufei.cn

[Q73] 查看表状态
来源：http://kke.guowangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://khd.mhx1999.top

[Q74] 强制使用索引
来源：http://fil.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nun.andypj.xyz

[Q75] 日期格式化
来源：http://qzs.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yxu.ywan-chungtsiang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cky.smart0.xyz

[Q76] 按天统计
来源：http://zwe.sysykeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jpv.fzhhl.top

[Q77] 时间加减
来源：http://exi.ivvv.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://laf.yongpay.top

[Q78] 当前时间
来源：http://ovx.c1oappe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ayp.ybcxt.top

[Q79] 字符串拼接
来源：http://fzx.sxryk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://osx.fktsv.cn

[Q80] 字符串截取
来源：http://fea.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ssn.nanxuanxn.top

[Q81] 字符串替换
来源：http://jwu.yuxming.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ukr.gotoacloud.top

[Q82] 字符长度与字节长度
来源：http://hcn.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pdr.sxryk.cn

[Q83] 大小写转换
来源：http://sfv.vqdsnc.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://daz.ydzc1.top

[Q84] 去除首尾空格
来源：http://fns.jinghuilouyu.cn

SELECT TRIM(name) FROM users;
来源：http://tcw.jqgfzy.top

[Q85] 数值取整
来源：http://psz.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lda.shanyushiyangtech.top

[Q86] 读取 JSON 字段
来源：http://ktu.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ikk.aibaodan.cn

[Q87] JSON 字段做条件
来源：http://dqn.zhengqikj.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hgx.sweek.top

[Q88] 行转列（条件聚合）
来源：http://pwn.jiagoushi.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ejg.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kzv.redwolf501.top

[Q89] 判断表是否存在
来源：http://yif.redwolf501.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lfz.dashuyun.cn

[Q90] 生成序号列
来源：http://jby.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xii.jinqigufen.top

================================================================================
来源：http://uie.c1oappe.top

R. Bash 专题
来源：http://ilu.chenzaomai.com

================================================================================
来源：http://hmx.dianchejie.cn

[R01] shebang 与严格模式
来源：http://gbe.sweek.top

#!/usr/bin/env bash
来源：http://yuh.hysaishi.cn

set -euo pipefail
来源：http://asw.zhiwuduotai.top

[R02] 变量赋值与使用
来源：http://zzr.hammf.cn

name="Tom"; echo "$name"
来源：http://ggw.jqgufenzy.top

[R03] 只读变量
来源：http://ywp.snrcjt.cn

readonly PI=3.14
来源：http://pmj.quarkkingdee.top

[R04] 位置参数
来源：http://vng.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qvj.andypj.xyz

[R05] 参数默认值
来源：http://uea.redwolf501.top

name="${1:-default}"
来源：http://jow.c1oappe.top

[R06] 判断命令是否存在
来源：http://tor.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yqr.guowangkeji.top

[R07] if 判断文件
来源：http://kuh.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nty.ehwqpu.com

[R08] 数值比较
来源：http://zdc.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://oji.fehbvm.com

[R09] 字符串比较
来源：http://etd.yj20258888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nfm.meibo888.top

[R10] 正则匹配
来源：http://hkh.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jwi.shangyingyoupin.top

[R11] case 多分支
来源：http://ajn.cqqwz.cn

case "$1" in
来源：http://kjz.sxryk.cn

start) echo "启动" ;;
来源：http://htd.zdqjudy.top

stop)  echo "停止" ;;
来源：http://xrg.jiagoushi.top

*)     echo "未知命令" ;;
来源：http://fov.zhaomingkeji.xyz

esac
来源：http://lbt.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://ndq.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://dfv.jqgufenzy.top

[R13] for 计数循环
来源：http://nsx.hcnkem.com

for i in {1..10}; do echo "$i"; done
来源：http://kxp.52xcode.cn

[R14] C 风格 for
来源：http://jhc.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://koy.meibo888.top

[R15] while 逐行读文件
来源：http://vqa.xuanzx.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://okt.vehdjk.com

[R16] until 等待条件
来源：http://zgj.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qqf.bjfxy.top

[R17] 数组定义与取值
来源：http://twt.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://zjh.kuanghao11.cn

[R18] 遍历数组
来源：http://jst.chenlongwang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sxr.wangshuangyany.cn

[R19] 数组长度
来源：http://tfz.havefunace.top

echo "${#arr[@]}"
来源：http://hfw.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://zlv.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ema.ywan-chungtsiang.top

[R21] 字符串长度
来源：http://lbb.chenlongwang.top

echo "${#s}"
来源：http://hoy.xinyue.icu

[R22] 截取子串
来源：http://lxj.tarul.cn

echo "${s:0:5}"
来源：http://enm.ivvv.top

[R23] 字符串替换
来源：http://ebb.cqqwz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://luk.wangdashe.top

[R24] 大小写转换
来源：http://fcf.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qzd.andypj.xyz

[R25] 去后缀 / 去前缀
来源：http://ios.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://crv.jqgufenzy.top

[R26] 命令替换
来源：http://icj.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://vvv.sysykeji.top

[R27] 算术展开
来源：http://mra.jinqigufen.top

echo $((1 + 2 * 3))
来源：http://als.jinqigfzy.top

[R28] 浮点运算
来源：http://hkg.svipenyu.cn

echo "scale=2; 10/3" | bc
来源：http://zby.hywenlv.cn

[R29] 定义函数
来源：http://hbg.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bmk.c1oappe.top

[R30] 函数返回状态码
来源：http://xdb.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://uqr.feifeiyinyue.top

[R31] 局部变量
来源：http://zau.guowangkeji.top

f() { local x=1; echo "$x"; }
来源：http://ujg.zdbjq.cn

[R32] 参数个数校验
来源：http://wds.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://utd.gogol.net.cn

[R33] 捕获错误并提示行号
来源：http://rtk.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ahv.svipenyu.cn

[R34] 退出时清理
来源：http://rtg.cheryme.top

trap 'rm -f "$tmp"' EXIT
来源：http://hle.gaohongyu789.top

[R35] 后台执行并等待
来源：http://pus.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uyr.tarul.cn

[R36] 并发执行多个任务
来源：http://qly.haohaochexian.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gyf.yvedp.cn

[R37] 把输出赋给变量
来源：http://uul.uphjek.com

files=$(ls -1)
来源：http://fyf.jyoumei.cn

[R38] 管道串联
来源：http://lhx.nanxinkj.top

cat a.txt | grep -i error | wc -l
来源：http://meb.birdmap.top

[R39] 重定向标准输出与错误
来源：http://fzr.hammf.cn

cmd > out.log 2>&1
来源：http://hud.fengsongda.top

[R40] 追加写日志
来源：http://aic.0kj1m.cn

echo "log" >> out.log
来源：http://ses.bjfxy.top

[R41] 丢弃输出
来源：http://iht.52xcode.cn

cmd >/dev/null 2>&1
来源：http://npl.ppjwa.cn

[R42] 输入重定向
来源：http://zpl.sufxvd.cn

wc -l < a.txt
来源：http://ljg.epnwcf.com

[R43] 按名字查找文件
来源：http://fss.daxiang520.top

find . -name "*.log" -type f
来源：http://msk.hcnkem.com

[R44] 按修改时间查找
来源：http://eiq.316326.xyz

find . -mtime -7 -type f
来源：http://sfo.fengsongda.top

[R45] 批量删除
来源：http://wzz.fktsv.cn

find . -name "*.tmp" -delete
来源：http://hkx.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://vks.kuanghao11.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://grp.zdqjudy.top

[R47] sed 单行替换
来源：http://gnq.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://rij.c1oappe.top

[R48] awk 取指定列
来源：http://ryv.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://uog.zdqjudy.top

[R49] awk 带条件
来源：http://wkl.andypj.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dqk.hesvh.cn

[R50] awk 求和
来源：http://nhh.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://uhi.xylfe.cn

[R51] 排序去重取前几
来源：http://ewf.ydjk.org.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qol.smart0.xyz

[R52] 统计行数
来源：http://lsk.zhaomingkeji.xyz

wc -l a.txt
来源：http://aty.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://vfa.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://icj.zycfv.cn

[R54] 比较两个文件
来源：http://ifp.yangfankeji.com

diff a.txt b.txt
来源：http://zbb.snrcjt.cn

[R55] 压缩与解压
来源：http://npz.jinqigfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://csx.tian-w.cn

[R56] 远程拷贝
来源：http://bdx.vehdjk.com

scp file user@host:/path/
来源：http://ppf.ydzc1.top

[R57] 远程执行命令
来源：http://nli.cheryme.top

ssh user@host 'uptime'
来源：http://kuh.yuxming.cn

[R58] 下载文件
来源：http://gma.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gqh.mhx1999.top

[R59] 发 POST JSON
来源：http://dar.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rjb.jyoumei.cn

[R60] 只看 HTTP 状态码
来源：http://xwi.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://anr.haohaochexian.top

[R61] 磁盘占用
来源：http://rbg.zhengqikj.top

df -h;  du -sh *
来源：http://xtf.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://ayh.daria6918.cn

du -ah . | sort -rh | head -10
来源：http://cda.pengpengdd.cyou

[R63] 内存与进程
来源：http://aii.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://sdh.vqdsnc.cn

[R64] 结束进程
来源：http://uca.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://nbs.quarkkingdee.top

[R65] 查看端口占用
来源：http://hxq.zhongyouzk.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vsk.zhaomingkeji.xyz

[R66] 定时任务
来源：http://yvw.dashuyun.cn

crontab -e;  crontab -l
来源：http://oeh.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://uej.xinyue.icu

openssl rand -hex 16
来源：http://npm.zhengqikj.top

[R68] 计算文件校验值
来源：http://uus.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yhv.jlsjyb.cn

[R69] 生成随机密码
来源：http://dlo.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://qlj.yuxming.cn

[R70] 时间戳与互转
来源：http://xmq.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://liz.ppjwa.cn

[R71] 日期格式化
来源：http://ium.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://eqm.shuidangran.top

[R72] 等待端口就绪
来源：http://znn.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://swi.ctjpmb.com

[R73] 分割大日志
来源：http://brr.hywenlv.cn

split -l 1000 big.log part_
来源：http://yrf.sjlbkw.cn

[R74] 批量重命名
来源：http://mxf.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vrr.ydzc1.top

[R75] 导出环境变量
来源：http://yfq.vqdsnc.cn

export PATH="$HOME/bin:$PATH"
来源：http://yiy.guowangkeji.top

[R76] 使用临时文件
来源：http://rfr.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jcf.shzxlz.cn

[R77] 读取用户输入
来源：http://fwp.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://orr.aizwys.cn

[R78] 交互式菜单
来源：http://emz.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lmi.epnwcf.com

[R79] 解析命令行选项
来源：http://mhx.xuetiantiany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ikr.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://ecc.tianlin.xyz

time ./run.sh
来源：http://muo.jyoumei.cn

================================================================================
来源：http://tgd.xziqi.cn

S. C / C++ 专题
来源：http://adh.wangdashe.top

================================================================================
来源：http://kpj.hcnkem.com

[S01] C：Hello World
来源：http://siz.vqdsnc.cn

#include <stdio.h>
来源：http://hdb.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ftr.0kj1m.cn

[S02] C：变量与格式化输出
来源：http://vyw.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://zwc.hongshengwenyu.top

[S03] C：读入整数
来源：http://zup.yueranfly.top

int x; scanf("%d", &x);
来源：http://ckk.shangyingyoupin.top

[S04] C：字符串复制
来源：http://qbk.gzhubu.top

char dst[32]; strcpy(dst, "hi");
来源：http://tls.yanxiufei.cn

[S05] C：字符串长度
来源：http://tkr.havefunace.top

strlen(s)
来源：http://juq.xylfe.cn

[S06] C：字符串比较
来源：http://adt.hammf.cn

strcmp(a, b) == 0
来源：http://fhx.ppjwa.cn

[S07] C：数组遍历求和
来源：http://rss.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qsf.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://jjx.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oie.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://txm.pycfn.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zva.sysykeji.top

[S10] C：指针与解引用
来源：http://wwz.svipenyu.cn

int *p = &a;  *p = 5;
来源：http://ydu.cucudq.cn

[S11] C：逐行读文件
来源：http://ura.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://nkd.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://uzl.zhongyouzk.top

fclose(f);
来源：http://gqf.kuanghao11.cn

[S12] C：写文件
来源：http://rpj.cheryme.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hfl.0kj1m.cn

[S13] C：宏定义
来源：http://rqi.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://onn.jinqigufen.top

[S14] C：枚举
来源：http://bya.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://hoq.meibo888.top

[S15] C：类型转换
来源：http://wep.wangdashe.top

(double) a / b
来源：http://kxt.svipenyu.cn

[S16] C：位操作置位
来源：http://kpj.hnxiangtu.top

x |= (1 << 3);
来源：http://rdl.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://kit.sjlbkw.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fkr.hfpthk.cn

[S18] C：命令行参数
来源：http://avp.guowangkeji.top

int main(int argc, char **argv)
来源：http://gct.yonumen.top

[S19] C：快速排序
来源：http://sml.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mdz.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://uuz.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kwz.havefunace.top

[S21] C：字符类别判断
来源：http://syx.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nto.9152youxi.cn

[S22] C：字符串转数字
来源：http://zgb.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://hzc.uphjek.com

[S23] C：随机数
来源：http://ewn.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mkl.tian-w.cn

[S24] C：获取本地时间
来源：http://apw.snrcjt.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://plx.chenlongwang.top

[S25] C：内存拷贝
来源：http://mul.dianchejie.cn

memcpy(dst, src, n);
来源：http://wxx.hammf.cn

[S26] C：内存清零
来源：http://ooj.wangdashe.top

memset(a, 0, sizeof a);
来源：http://sns.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://qbk.jinqigfzy.top

const double PI = 3.14159;
来源：http://bsg.chenlongwang.top

[S28] C：静态变量
来源：http://lpx.quarkkingdee.top

static int counter = 0;
来源：http://zrd.hfpthk.cn

[S29] C：变参函数
来源：http://qez.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jvt.daxiang520.top

[S30] C：头文件保护
来源：http://qed.52xcode.cn

#ifndef X_H
来源：http://yrd.jqgfzy.top

#define X_H
来源：http://rqk.xylfe.cn

#endif
来源：http://jlg.sufxvd.cn

[S31] C++：Hello World
来源：http://tln.sysykeji.top

#include <iostream>
来源：http://vfz.meibo888.top

int main() { std::cout << "Hello\n"; }
来源：http://cjb.yongpay.top

[S32] C++：字符串
来源：http://uxq.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://zvu.epnwcf.com

[S33] C++：vector 增删
来源：http://jhu.ydzc1.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yjl.fanxiaobao.xyz

[S34] C++：遍历 vector
来源：http://yom.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://kmn.zhijiandao.cn

[S35] C++：map
来源：http://xqu.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vjq.meibo888.top

[S36] C++：unordered_map
来源：http://snm.mhx1999.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xbm.smart0.xyz

[S37] C++：set
来源：http://fhw.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nsz.nanxinkj.top

[S38] C++：排序
来源：http://jze.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://sbh.nanxinkj.top

[S39] C++：自定义比较器排序
来源：http://dcv.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://txm.ybcxt.top

[S40] C++：查找元素
来源：http://ydy.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yzm.iojbl.cn


<!-- 参考信息 -->