代发 wailian999

[Q67] 设置隔离级别
来源：http://gus.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xag.gogol.net.cn

[Q68] 保存点
来源：http://emz.guowangkeji.top

SAVEPOINT sp1;
来源：http://ujo.fktsv.cn

ROLLBACK TO sp1;
来源：http://itz.ctjpmb.com

[Q69] 查看执行计划
来源：http://vcs.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://app.gaohongyu789.top

[Q70] 更新统计信息
来源：http://eyo.yfazqb.com

ANALYZE TABLE users;
来源：http://gjr.ppjwa.cn

[Q71] 查看建表语句
来源：http://ufk.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://awy.gogol.net.cn

[Q72] 查看索引
来源：http://rxv.guowangkeji.top

SHOW INDEX FROM users;
来源：http://sxc.dianchejie.cn

[Q73] 查看表状态
来源：http://pqo.chenlongwang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vca.zdbjq.cn

[Q74] 强制使用索引
来源：http://ltv.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qnk.xziqi.cn

[Q75] 日期格式化
来源：http://ckc.aizwys.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://onq.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vjc.feifeiyinyue.top

[Q76] 按天统计
来源：http://giq.zhiwuduotai.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ipx.gotoacloud.top

[Q77] 时间加减
来源：http://zkn.meibo888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://alv.ehwqpu.com

[Q78] 当前时间
来源：http://lpk.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wzd.mhx1999.top

[Q79] 字符串拼接
来源：http://aym.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cwx.bjfxy.top

[Q80] 字符串截取
来源：http://ird.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uth.chenjidiqi.icu

[Q81] 字符串替换
来源：http://pie.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://otv.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://twd.meibo888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xha.jiagoushi.top

[Q83] 大小写转换
来源：http://rkt.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://onr.9152youxi.cn

[Q84] 去除首尾空格
来源：http://lkt.ydjk.org.cn

SELECT TRIM(name) FROM users;
来源：http://lmo.zhongyouzk.top

[Q85] 数值取整
来源：http://vqz.cucudq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://udw.yuxming.cn

[Q86] 读取 JSON 字段
来源：http://hrz.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tje.fzhhl.top

[Q87] JSON 字段做条件
来源：http://zod.zhengqikj.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uti.zhixingplan.top

[Q88] 行转列（条件聚合）
来源：http://dvq.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wws.wangshuangyany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hzt.gogol.net.cn

[Q89] 判断表是否存在
来源：http://kmg.zhengqikj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sac.chenzaomai.com

[Q90] 生成序号列
来源：http://dti.cqqwz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jyw.xylfe.cn

================================================================================
来源：http://ztf.fehbvm.com

R. Bash 专题
来源：http://rwi.zhijiandao.cn

================================================================================
来源：http://hvd.nanxinkj.top

[R01] shebang 与严格模式
来源：http://yqb.zhoulong.xyz

#!/usr/bin/env bash
来源：http://trx.ppjwa.cn

set -euo pipefail
来源：http://utw.bjfxy.top

[R02] 变量赋值与使用
来源：http://asx.wangdashe.top

name="Tom"; echo "$name"
来源：http://gmu.jinyuanbaomall.cn

[R03] 只读变量
来源：http://agb.guowangkeji.top

readonly PI=3.14
来源：http://xdi.yj20258888.top

[R04] 位置参数
来源：http://gid.xinyue.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tej.hcnkem.com

[R05] 参数默认值
来源：http://qhr.nwbrower.top

name="${1:-default}"
来源：http://hiz.xylfe.cn

[R06] 判断命令是否存在
来源：http://eil.zhongyouzk.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xsh.hywenlv.cn

[R07] if 判断文件
来源：http://rfj.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lkv.zdbjq.cn

[R08] 数值比较
来源：http://ych.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pkl.pengpengdd.cyou

[R09] 字符串比较
来源：http://eze.xuetiantiany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://thk.kuanghao11.cn

[R10] 正则匹配
来源：http://ivv.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gkc.xuetiantiany.cn

[R11] case 多分支
来源：http://yjb.tarul.cn

case "$1" in
来源：http://qzo.aizwys.cn

start) echo "启动" ;;
来源：http://ujk.smart0.xyz

stop)  echo "停止" ;;
来源：http://fzp.mhx1999.top

*)     echo "未知命令" ;;
来源：http://uqi.shzxlz.cn

esac
来源：http://uoh.hcnkem.com

[R12] for 遍历文件
来源：http://kbe.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://ono.ehwqpu.com

[R13] for 计数循环
来源：http://mfd.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://poy.hnqzz.top

[R14] C 风格 for
来源：http://kfn.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qxe.cucudq.cn

[R15] while 逐行读文件
来源：http://aez.chenzaomai.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qko.yonumen.top

[R16] until 等待条件
来源：http://plg.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://obj.yueranfly.top

[R17] 数组定义与取值
来源：http://nmk.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://oti.yvedp.cn

[R18] 遍历数组
来源：http://ske.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ftq.yj20258888.top

[R19] 数组长度
来源：http://wqh.jiagoushi.top

echo "${#arr[@]}"
来源：http://veq.iojbl.cn

[R20] 关联数组（字典）
来源：http://cmv.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mdg.zdbjq.cn

[R21] 字符串长度
来源：http://vjd.fehbvm.com

echo "${#s}"
来源：http://tdh.pycfn.com

[R22] 截取子串
来源：http://qty.ppjwa.cn

echo "${s:0:5}"
来源：http://nad.fengsongda.top

[R23] 字符串替换
来源：http://mrb.mhx1999.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wai.andypj.xyz

[R24] 大小写转换
来源：http://pcs.cheryme.top

echo "${s^^}"; echo "${s,,}"
来源：http://lpm.hesvh.cn

[R25] 去后缀 / 去前缀
来源：http://hsa.shanyushiyangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wvn.meibo888.top

[R26] 命令替换
来源：http://yhj.zhongyouzk.top

now=$(date +%F); echo "$now"
来源：http://yub.guannengcc.top

[R27] 算术展开
来源：http://mls.yongpay.top

echo $((1 + 2 * 3))
来源：http://qvg.gogol.net.cn

[R28] 浮点运算
来源：http://htc.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://nby.yj202588.top

[R29] 定义函数
来源：http://cih.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://log.ydjk.org.cn

[R30] 函数返回状态码
来源：http://wgu.tanke756.top

f() { return 0; }; f || echo "失败了"
来源：http://dja.yanxiufei.cn

[R31] 局部变量
来源：http://kga.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://wvc.ybcxt.top

[R32] 参数个数校验
来源：http://cgy.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xvg.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://uzu.redwolf501.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jff.ybcxt.top

[R34] 退出时清理
来源：http://mxz.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://mwe.hcnkem.com

[R35] 后台执行并等待
来源：http://njj.daxiang520.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uuu.daxiang520.top

[R36] 并发执行多个任务
来源：http://rqc.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://liu.iojbl.cn

[R37] 把输出赋给变量
来源：http://epk.redwolf501.top

files=$(ls -1)
来源：http://bhl.dianchejie.cn

[R38] 管道串联
来源：http://axa.redwolf501.top

cat a.txt | grep -i error | wc -l
来源：http://ljj.xinyue.icu

[R39] 重定向标准输出与错误
来源：http://tdo.yuanzhike.top

cmd > out.log 2>&1
来源：http://krj.hywenlv.cn

[R40] 追加写日志
来源：http://mfc.svipenyu.cn

echo "log" >> out.log
来源：http://iyq.fehbvm.com

[R41] 丢弃输出
来源：http://ahi.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://xvh.shanyushiyangtech.top

[R42] 输入重定向
来源：http://nzn.jyoumei.cn

wc -l < a.txt
来源：http://bpf.quarkkingdee.top

[R43] 按名字查找文件
来源：http://qum.kuanghao11.cn

find . -name "*.log" -type f
来源：http://cka.hcnkem.com

[R44] 按修改时间查找
来源：http://qck.meibo888.top

find . -mtime -7 -type f
来源：http://qai.aizwys.cn

[R45] 批量删除
来源：http://rzy.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://pjj.jyoumei.cn

[R46] 递归替换文件内容
来源：http://iuq.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tza.xuanzx.com

[R47] sed 单行替换
来源：http://fay.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://dgp.sjlbkw.cn

[R48] awk 取指定列
来源：http://jnk.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://fqe.sufxvd.cn

[R49] awk 带条件
来源：http://jeg.yj20258.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vhb.yongpay.top

[R50] awk 求和
来源：http://jni.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://pna.ehwqpu.com

[R51] 排序去重取前几
来源：http://wts.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://whk.pengpengdd.cyou

[R52] 统计行数
来源：http://mzv.quarkkingdee.top

wc -l a.txt
来源：http://knl.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://ogl.jinyuanbaomall.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ere.vehdjk.com

[R54] 比较两个文件
来源：http://uez.yueranfly.top

diff a.txt b.txt
来源：http://wuj.jinqigufen.top

[R55] 压缩与解压
来源：http://fnu.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qns.yonumen.top

[R56] 远程拷贝
来源：http://byl.gogol.net.cn

scp file user@host:/path/
来源：http://yvh.daxiang520.top

[R57] 远程执行命令
来源：http://itf.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://hqk.zycfv.cn

[R58] 下载文件
来源：http://rdc.hfpthk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bkq.hysaishi.cn

[R59] 发 POST JSON
来源：http://ufd.xylfe.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wnx.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://jwj.tian-w.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wpd.shangyingyoupin.top

[R61] 磁盘占用
来源：http://osy.ppjwa.cn

df -h;  du -sh *
来源：http://acj.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://cbn.yongpay.top

du -ah . | sort -rh | head -10
来源：http://obf.jinqigufen.top

[R63] 内存与进程
来源：http://ylg.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://ikx.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://dgw.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://aeg.jinqigfzy.top

[R65] 查看端口占用
来源：http://elx.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kkz.hammf.cn

[R66] 定时任务
来源：http://oao.xuetiantiany.cn

crontab -e;  crontab -l
来源：http://dfg.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://phi.9152youxi.cn

openssl rand -hex 16
来源：http://eul.nanxinkj.top

[R68] 计算文件校验值
来源：http://qnm.aizwys.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wus.dianchejie.cn

[R69] 生成随机密码
来源：http://xty.zhongyouzk.top

head -c 16 /dev/urandom | base64
来源：http://lup.hcnkem.com

[R70] 时间戳与互转
来源：http://mbo.yfazqb.com

date +%s;  date -d @1700000000
来源：http://ftf.iojbl.cn

[R71] 日期格式化
来源：http://fwf.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://czv.kuanghao11.cn

[R72] 等待端口就绪
来源：http://oql.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ksm.gotoacloud.top

[R73] 分割大日志
来源：http://gnf.yongpay.top

split -l 1000 big.log part_
来源：http://dnn.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://cmq.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cwx.shzxlz.cn

[R75] 导出环境变量
来源：http://pso.zdbjq.cn

export PATH="$HOME/bin:$PATH"
来源：http://ija.mhx1999.top

[R76] 使用临时文件
来源：http://unu.sjlbkw.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dkn.vehdjk.com

[R77] 读取用户输入
来源：http://lxf.zhengqikj.top

read -rp "请输入: " ans
来源：http://acb.xylfe.cn

[R78] 交互式菜单
来源：http://tiq.shanyushiyangtech.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mcq.9152youxi.cn

[R79] 解析命令行选项
来源：http://map.xuetiantiany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uls.c1oappe.top

[R80] 查看脚本执行耗时
来源：http://eqg.yuxming.cn

time ./run.sh
来源：http://fpu.jqgfzy.top

================================================================================
来源：http://wev.0kj1m.cn

S. C / C++ 专题
来源：http://zaz.shangyingyoupin.top

================================================================================
来源：http://sfw.xuanzx.com

[S01] C：Hello World
来源：http://oxh.jqgufenzy.top

#include <stdio.h>
来源：http://tdy.ctjpmb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://nmg.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://rsr.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://sqk.ydjk.org.cn

[S03] C：读入整数
来源：http://hsv.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://fzt.ydzc1.top

[S04] C：字符串复制
来源：http://pod.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://dev.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://btp.xuanzx.com

strlen(s)
来源：http://dme.tanke756.top

[S06] C：字符串比较
来源：http://yiw.shuidangran.top

strcmp(a, b) == 0
来源：http://nbf.wangshuangyany.cn

[S07] C：数组遍历求和
来源：http://liq.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://czq.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://elk.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jtc.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://zog.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xbl.yfazqb.com

[S10] C：指针与解引用
来源：http://wds.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://fdr.sxryk.cn

[S11] C：逐行读文件
来源：http://ufv.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://dxp.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://thi.hnxiangtu.top

fclose(f);
来源：http://pvm.feifeiyinyue.top

[S12] C：写文件
来源：http://vqb.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bcj.dashuyun.cn

[S13] C：宏定义
来源：http://uqe.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tju.yj20258.top

[S14] C：枚举
来源：http://ich.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://hxm.cashguo.top

[S15] C：类型转换
来源：http://zgn.quarkkingdee.top

(double) a / b
来源：http://ath.sysykeji.top

[S16] C：位操作置位
来源：http://bqy.snrcjt.cn

x |= (1 << 3);
来源：http://aab.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://gdp.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rdz.ivvv.top

[S18] C：命令行参数
来源：http://qpy.52xcode.cn

int main(int argc, char **argv)
来源：http://wjc.nanxuanxn.top

[S19] C：快速排序
来源：http://gry.jlsjyb.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wvw.tanke756.top

[S20] C：二分查找
来源：http://bza.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://slc.zhongyouzk.top

[S21] C：字符类别判断
来源：http://fzy.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sxa.ydzc1.top

[S22] C：字符串转数字
来源：http://mqy.snrcjt.cn

atoi("42");  strtod("3.14", NULL);
来源：http://okz.ctjpmb.com

[S23] C：随机数
来源：http://etw.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://xlu.cheryme.top

[S24] C：获取本地时间
来源：http://rug.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://krg.xziqi.cn

[S25] C：内存拷贝
来源：http://yzl.yfazqb.com

memcpy(dst, src, n);
来源：http://sqm.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://qgj.xuanzx.com

memset(a, 0, sizeof a);
来源：http://jjx.feifeiyinyue.top

[S27] C：定义常量
来源：http://kia.shangyingyoupin.top

const double PI = 3.14159;
来源：http://bkt.vqdsnc.cn

[S28] C：静态变量
来源：http://qju.hfpthk.cn

static int counter = 0;
来源：http://rpv.cashguo.top

[S29] C：变参函数
来源：http://efx.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://raf.aizwys.cn

[S30] C：头文件保护
来源：http://hpt.shangyingyoupin.top

#ifndef X_H
来源：http://fxp.zhoulong.xyz

#define X_H
来源：http://vox.yj20258.top

#endif
来源：http://uhy.fehbvm.com

[S31] C++：Hello World
来源：http://wqe.hcnkem.com

#include <iostream>
来源：http://ray.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://zge.mhx1999.top

[S32] C++：字符串
来源：http://vcs.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://aab.xylfe.cn

[S33] C++：vector 增删
来源：http://eww.zhaomingkeji.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nsc.xuanzx.com

[S34] C++：遍历 vector
来源：http://avq.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://oed.daxiang520.top

[S35] C++：map
来源：http://vxq.quarkkingdee.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wdu.xziqi.cn

[S36] C++：unordered_map
来源：http://ixh.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pyj.zhijiandao.cn


<!-- 参考信息 -->