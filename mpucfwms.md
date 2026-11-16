代发 wailian999

[Q65] 回滚事务
来源：http://zwp.ctjpmb.com

ROLLBACK;
来源：http://pth.shuidangran.top

[Q66] 行锁查询
来源：http://gyf.sjlbkw.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kqy.yongpay.top

[Q67] 设置隔离级别
来源：http://upe.zhoulong.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vzz.xylfe.cn

[Q68] 保存点
来源：http://psj.xinyue.icu

SAVEPOINT sp1;
来源：http://niz.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://ypz.chenzaomai.com

[Q69] 查看执行计划
来源：http://vzd.mhx1999.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sft.zhiwuduotai.top

[Q70] 更新统计信息
来源：http://tyu.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://wbn.nanxinkj.top

[Q71] 查看建表语句
来源：http://mom.jqgufenzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tkl.pycfn.com

[Q72] 查看索引
来源：http://eea.dashuyun.cn

SHOW INDEX FROM users;
来源：http://wgi.hnqzz.top

[Q73] 查看表状态
来源：http://owd.ydjk.org.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tkq.chenzaomai.com

[Q74] 强制使用索引
来源：http://cjp.fanxiaobao.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bxl.yuxming.cn

[Q75] 日期格式化
来源：http://mkb.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://drj.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qja.yueranfly.top

[Q76] 按天统计
来源：http://prz.cqqwz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://szb.hongshengwenyu.top

[Q77] 时间加减
来源：http://azr.cucudq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vik.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://xgl.chenzaomai.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lau.jinghuilouyu.cn

[Q79] 字符串拼接
来源：http://ygn.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aqd.xuanzx.com

[Q80] 字符串截取
来源：http://qgj.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nfz.iojbl.cn

[Q81] 字符串替换
来源：http://mxy.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ymm.zhoulong.xyz

[Q82] 字符长度与字节长度
来源：http://bwo.0kj1m.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jvm.havefunace.top

[Q83] 大小写转换
来源：http://bdx.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vex.yj202588.top

[Q84] 去除首尾空格
来源：http://lew.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://ila.zhaomingkeji.xyz

[Q85] 数值取整
来源：http://fys.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bsj.aizwys.cn

[Q86] 读取 JSON 字段
来源：http://yts.epnwcf.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hwf.yj20258888.top

[Q87] JSON 字段做条件
来源：http://eap.fengsongda.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ibx.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://suo.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vhe.sxryk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ucq.jinyuanbaomall.cn

[Q89] 判断表是否存在
来源：http://zyb.gogol.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ioq.ctjpmb.com

[Q90] 生成序号列
来源：http://gpv.hammf.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wav.zycfv.cn

================================================================================
来源：http://won.ctjpmb.com

R. Bash 专题
来源：http://kud.jqgufenzy.top

================================================================================
来源：http://dyn.xinyue.icu

[R01] shebang 与严格模式
来源：http://ifb.ppjwa.cn

#!/usr/bin/env bash
来源：http://uav.guannengcc.top

set -euo pipefail
来源：http://wgr.mhx1999.top

[R02] 变量赋值与使用
来源：http://uzb.zdqjudy.top

name="Tom"; echo "$name"
来源：http://hyh.zhongyouzk.top

[R03] 只读变量
来源：http://waj.daxiang520.top

readonly PI=3.14
来源：http://xpy.hysaishi.cn

[R04] 位置参数
来源：http://wvs.tarul.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xzy.ehwqpu.com

[R05] 参数默认值
来源：http://msa.yj202588.top

name="${1:-default}"
来源：http://qwo.yj20258888.top

[R06] 判断命令是否存在
来源：http://zur.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vfu.shanyushiyangkeji.top

[R07] if 判断文件
来源：http://sss.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gtt.cheryme.top

[R08] 数值比较
来源：http://lch.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://boo.aizwys.cn

[R09] 字符串比较
来源：http://ynl.ehwqpu.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vyv.jqgufenzy.top

[R10] 正则匹配
来源：http://qnv.yueranfly.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mla.tarul.cn

[R11] case 多分支
来源：http://ywz.zhoulong.xyz

case "$1" in
来源：http://kaa.pycfn.com

start) echo "启动" ;;
来源：http://xhs.epnwcf.com

stop)  echo "停止" ;;
来源：http://jfe.hesvh.cn

*)     echo "未知命令" ;;
来源：http://bxs.jqgfzy.top

esac
来源：http://ded.tianlin.xyz

[R12] for 遍历文件
来源：http://wky.c1oappe.top

for f in *.txt; do echo "$f"; done
来源：http://iny.nanxinkj.top

[R13] for 计数循环
来源：http://ulc.shuidangran.top

for i in {1..10}; do echo "$i"; done
来源：http://wdg.tarul.cn

[R14] C 风格 for
来源：http://xti.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zbv.ydjk.org.cn

[R15] while 逐行读文件
来源：http://sdc.vehdjk.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eju.daria6918.cn

[R16] until 等待条件
来源：http://myc.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://apt.yuxming.cn

[R17] 数组定义与取值
来源：http://dpo.hfpthk.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rrd.tian-w.cn

[R18] 遍历数组
来源：http://dba.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xhs.shangyingyoupin.top

[R19] 数组长度
来源：http://tkn.gzhubu.top

echo "${#arr[@]}"
来源：http://mwj.yueranfly.top

[R20] 关联数组（字典）
来源：http://pnx.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pzp.jinqigufen.top

[R21] 字符串长度
来源：http://qjr.aibaodan.cn

echo "${#s}"
来源：http://gfo.yj20258.top

[R22] 截取子串
来源：http://qmz.ywan-chungtsiang.top

echo "${s:0:5}"
来源：http://ugo.uphjek.com

[R23] 字符串替换
来源：http://dxl.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rym.dianchejie.cn

[R24] 大小写转换
来源：http://qon.zhaomingkeji.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://ojq.smart0.xyz

[R25] 去后缀 / 去前缀
来源：http://kbm.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://pce.yangfankeji.com

[R26] 命令替换
来源：http://usy.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://vpi.cashguo.top

[R27] 算术展开
来源：http://kcu.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://pfm.sweek.top

[R28] 浮点运算
来源：http://woe.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://jgf.wangshuangyany.cn

[R29] 定义函数
来源：http://mrm.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lms.pycfn.com

[R30] 函数返回状态码
来源：http://zpa.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://tqd.9152youxi.cn

[R31] 局部变量
来源：http://gwh.daria6918.cn

f() { local x=1; echo "$x"; }
来源：http://ouu.ywan-chungtsiang.top

[R32] 参数个数校验
来源：http://xgb.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rbb.cheryme.top

[R33] 捕获错误并提示行号
来源：http://wrw.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mdf.xylfe.cn

[R34] 退出时清理
来源：http://tvj.dianchejie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://klb.jianghu66.top

[R35] 后台执行并等待
来源：http://etf.hysaishi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://chr.quarkkingdee.top

[R36] 并发执行多个任务
来源：http://evc.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dta.shangyingyoupin.top

[R37] 把输出赋给变量
来源：http://cvh.havefunace.top

files=$(ls -1)
来源：http://sfy.gaohongyu789.top

[R38] 管道串联
来源：http://pla.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://gph.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://bkh.tarul.cn

cmd > out.log 2>&1
来源：http://pel.cqqwz.cn

[R40] 追加写日志
来源：http://wgi.fehbvm.com

echo "log" >> out.log
来源：http://cya.dianchejie.cn

[R41] 丢弃输出
来源：http://dfz.shangyingyoupin.top

cmd >/dev/null 2>&1
来源：http://avg.gogol.net.cn

[R42] 输入重定向
来源：http://orf.ehwqpu.com

wc -l < a.txt
来源：http://trh.sjlbkw.cn

[R43] 按名字查找文件
来源：http://omg.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://ijd.zhongyouzk.top

[R44] 按修改时间查找
来源：http://aql.hysaishi.cn

find . -mtime -7 -type f
来源：http://lfm.daria6918.cn

[R45] 批量删除
来源：http://jxw.bbcook.cn

find . -name "*.tmp" -delete
来源：http://yge.haohaochexian.top

[R46] 递归替换文件内容
来源：http://ndu.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vmh.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://eng.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://jmu.guowangkeji.top

[R48] awk 取指定列
来源：http://ffo.sxryk.cn

awk '{print $1, $3}' a.txt
来源：http://lkf.ivvv.top

[R49] awk 带条件
来源：http://qah.dianchejie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rlv.dashuyun.cn

[R50] awk 求和
来源：http://tss.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://pcw.wangdashe.top

[R51] 排序去重取前几
来源：http://mgu.cdnleiting.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bdv.zhaomingkeji.xyz

[R52] 统计行数
来源：http://nxl.gzhubu.top

wc -l a.txt
来源：http://mqu.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://yvr.xinyue.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bsx.dashuyun.cn

[R54] 比较两个文件
来源：http://grp.guowangkeji.top

diff a.txt b.txt
来源：http://pyh.zycfv.cn

[R55] 压缩与解压
来源：http://cck.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vhb.zdbjq.cn

[R56] 远程拷贝
来源：http://kkc.fktsv.cn

scp file user@host:/path/
来源：http://zgz.aibaodan.cn

[R57] 远程执行命令
来源：http://oua.gzhubu.top

ssh user@host 'uptime'
来源：http://vmg.sweek.top

[R58] 下载文件
来源：http://row.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uwe.zycfv.cn

[R59] 发 POST JSON
来源：http://ivj.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://irz.aibaodan.cn

[R60] 只看 HTTP 状态码
来源：http://zjw.shangyingyoupin.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://imk.yonumen.top

[R61] 磁盘占用
来源：http://lzi.hammf.cn

df -h;  du -sh *
来源：http://bgl.jianghu66.top

[R62] 找最占空间的文件
来源：http://rsd.vqdsnc.cn

du -ah . | sort -rh | head -10
来源：http://xtm.kuanghao11.cn

[R63] 内存与进程
来源：http://hmn.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://rus.fengsongda.top

[R64] 结束进程
来源：http://enr.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://lon.yongpay.top

[R65] 查看端口占用
来源：http://uyp.dashuyun.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tjr.cdnleiting.top

[R66] 定时任务
来源：http://mzp.quarkkingdee.top

crontab -e;  crontab -l
来源：http://iaq.yj202588.top

[R67] 生成随机十六进制串
来源：http://uhz.wangdashe.top

openssl rand -hex 16
来源：http://zet.yuanzhike.top

[R68] 计算文件校验值
来源：http://dbm.hnxiangtu.top

sha256sum a.txt;  md5sum a.txt
来源：http://nqo.xinyue.icu

[R69] 生成随机密码
来源：http://vlk.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://drh.jqgfzy.top

[R70] 时间戳与互转
来源：http://gyu.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://xan.jinghuilouyu.cn

[R71] 日期格式化
来源：http://mcx.guowangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tpk.cqqwz.cn

[R72] 等待端口就绪
来源：http://jtp.hywenlv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hbs.redwolf501.top

[R73] 分割大日志
来源：http://zgw.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://rtk.guowangkeji.top

[R74] 批量重命名
来源：http://ksu.jinghuilouyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://toq.aizwys.cn

[R75] 导出环境变量
来源：http://dkx.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://syr.shangyingyoupin.top

[R76] 使用临时文件
来源：http://fke.fehbvm.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yzi.hcnkem.com

[R77] 读取用户输入
来源：http://wzk.ydzc1.top

read -rp "请输入: " ans
来源：http://lvv.sufxvd.cn

[R78] 交互式菜单
来源：http://wyj.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fsk.daria6918.cn

[R79] 解析命令行选项
来源：http://tvp.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qct.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://imj.vqdsnc.cn

time ./run.sh
来源：http://jeq.cheryme.top

================================================================================
来源：http://cvx.xinyue.icu

S. C / C++ 专题
来源：http://ypi.quarkkingdee.top

================================================================================
来源：http://skh.hcnkem.com

[S01] C：Hello World
来源：http://djz.ppjwa.cn

#include <stdio.h>
来源：http://ezg.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://anj.hongshengwenyu.top

[S02] C：变量与格式化输出
来源：http://jcj.yj20258888.top

int a = 10; printf("%d\n", a);
来源：http://sxw.jinqigufen.top

[S03] C：读入整数
来源：http://jyg.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://yrf.yj20258888.top

[S04] C：字符串复制
来源：http://mfz.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://rpz.dianchejie.cn

[S05] C：字符串长度
来源：http://csc.xziqi.cn

strlen(s)
来源：http://rtk.nanxuanxn.top

[S06] C：字符串比较
来源：http://gzv.sysykeji.top

strcmp(a, b) == 0
来源：http://joe.cucudq.cn

[S07] C：数组遍历求和
来源：http://cyl.bbcook.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://chm.dashuyun.cn

[S08] C：动态内存分配与释放
来源：http://ykc.vqdsnc.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zum.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://ovd.ywan-chungtsiang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uze.jqgfzy.top

[S10] C：指针与解引用
来源：http://hbb.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://poz.snrcjt.cn

[S11] C：逐行读文件
来源：http://dtu.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://vcy.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://boy.guowangkeji.top

fclose(f);
来源：http://xqn.ivvv.top

[S12] C：写文件
来源：http://smt.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iuj.0kj1m.cn

[S13] C：宏定义
来源：http://yeb.zdqjudy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zzl.birdmap.top

[S14] C：枚举
来源：http://ulm.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://qrn.jinqigufen.top

[S15] C：类型转换
来源：http://zrv.wangshuangyany.cn

(double) a / b
来源：http://acv.yvedp.cn

[S16] C：位操作置位
来源：http://slo.hfpthk.cn

x |= (1 << 3);
来源：http://jqt.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://zyl.dashuyun.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zjt.cdnleiting.top

[S18] C：命令行参数
来源：http://wtk.hywenlv.cn

int main(int argc, char **argv)
来源：http://qju.zhixingplan.top

[S19] C：快速排序
来源：http://fcp.gaohongyu789.top

qsort(a, n, sizeof(int), cmp);
来源：http://pth.zhixingplan.top

[S20] C：二分查找
来源：http://xcm.meibo888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wsu.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://duf.zhongyouzk.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pdm.shangyingyoupin.top

[S22] C：字符串转数字
来源：http://qsv.hnqzz.top

atoi("42");  strtod("3.14", NULL);
来源：http://qlq.hammf.cn

[S23] C：随机数
来源：http://egw.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xbv.shanyushiyangtech.top

[S24] C：获取本地时间
来源：http://nzm.cqqwz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hqm.gotoacloud.top

[S25] C：内存拷贝
来源：http://diy.cqqwz.cn

memcpy(dst, src, n);
来源：http://tlp.aibaodan.cn

[S26] C：内存清零
来源：http://dph.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://ygs.guannengcc.top

[S27] C：定义常量
来源：http://ytf.gogol.net.cn

const double PI = 3.14159;
来源：http://zob.feifeiyinyue.top

[S28] C：静态变量
来源：http://gmi.xuanzx.com

static int counter = 0;
来源：http://ffg.fehbvm.com

[S29] C：变参函数
来源：http://wie.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mhh.haohaochexian.top

[S30] C：头文件保护
来源：http://qbl.yongpay.top

#ifndef X_H
来源：http://htn.hongshengwenyu.top

#define X_H
来源：http://ezh.jlsjyb.cn

#endif
来源：http://eqj.sjlbkw.cn

[S31] C++：Hello World
来源：http://loj.c1oappe.top

#include <iostream>
来源：http://afu.uphjek.com

int main() { std::cout << "Hello\n"; }
来源：http://cvu.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://ziw.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://rlo.hammf.cn

[S33] C++：vector 增删
来源：http://tzg.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dla.jinqigfzy.top

[S34] C++：遍历 vector
来源：http://rqs.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://hqt.zhiwuduotai.top


<!-- 参考信息 -->