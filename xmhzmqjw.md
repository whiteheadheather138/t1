代发 wailian999

[Q61] 移动平均
来源：http://mrw.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nzp.cashguo.top

[Q62] 分组占比
来源：http://nqb.wangdashe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cwh.hammf.cn

[Q63] 开启事务
来源：http://mhd.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://nia.xuetiantiany.cn

[Q64] 提交事务
来源：http://zae.mhx1999.top

COMMIT;
来源：http://jpr.jinqigfzy.top

[Q65] 回滚事务
来源：http://koe.daria6918.cn

ROLLBACK;
来源：http://pbx.sysykeji.top

[Q66] 行锁查询
来源：http://ryu.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uqi.wangdashe.top

[Q67] 设置隔离级别
来源：http://kny.sxryk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://auy.xuetiantiany.cn

[Q68] 保存点
来源：http://cmh.svipenyu.cn

SAVEPOINT sp1;
来源：http://svw.52xcode.cn

ROLLBACK TO sp1;
来源：http://foa.jianghu66.top

[Q69] 查看执行计划
来源：http://cbk.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vbx.dianchejie.cn

[Q70] 更新统计信息
来源：http://zpr.yj20258.top

ANALYZE TABLE users;
来源：http://hiy.ppjwa.cn

[Q71] 查看建表语句
来源：http://ejv.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bus.tianlin.xyz

[Q72] 查看索引
来源：http://evd.vehdjk.com

SHOW INDEX FROM users;
来源：http://ldz.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://znj.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://plg.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://bzc.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rpm.shzxlz.cn

[Q75] 日期格式化
来源：http://tnu.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zjd.yj20258888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xqb.sjlbkw.cn

[Q76] 按天统计
来源：http://nkw.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uit.hysaishi.cn

[Q77] 时间加减
来源：http://osg.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ssl.quarkkingdee.top

[Q78] 当前时间
来源：http://zux.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kob.xuetiantiany.cn

[Q79] 字符串拼接
来源：http://cff.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uvu.gzhubu.top

[Q80] 字符串截取
来源：http://pwb.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hse.zhixingplan.top

[Q81] 字符串替换
来源：http://fbi.feifeiyinyue.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ara.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://iko.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ebj.hysaishi.cn

[Q83] 大小写转换
来源：http://tic.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dof.yongpay.top

[Q84] 去除首尾空格
来源：http://wrf.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://lwr.ydjk.org.cn

[Q85] 数值取整
来源：http://kbn.tarul.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nol.yanxiufei.cn

[Q86] 读取 JSON 字段
来源：http://uyw.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nys.zhixingplan.top

[Q87] JSON 字段做条件
来源：http://fma.fanxiaobao.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hmm.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://duq.uphjek.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iwc.zhixingplan.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://phu.shanyushiyangkeji.top

[Q89] 判断表是否存在
来源：http://arl.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dgg.tianlin.xyz

[Q90] 生成序号列
来源：http://bkq.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ycv.fehbvm.com

================================================================================
来源：http://bzh.jiagoushi.top

R. Bash 专题
来源：http://upw.jlsjyb.cn

================================================================================
来源：http://wkk.yj20258888.top

[R01] shebang 与严格模式
来源：http://bqi.pycfn.com

#!/usr/bin/env bash
来源：http://cxz.shanyushiyangtech.top

set -euo pipefail
来源：http://shd.svipenyu.cn

[R02] 变量赋值与使用
来源：http://xqa.hammf.cn

name="Tom"; echo "$name"
来源：http://gtm.xziqi.cn

[R03] 只读变量
来源：http://npr.haohaochexian.top

readonly PI=3.14
来源：http://nnp.jinyuanbaomall.cn

[R04] 位置参数
来源：http://otj.ydzc1.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://elj.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://ffi.wangshuangyany.cn

name="${1:-default}"
来源：http://lyz.yuxming.cn

[R06] 判断命令是否存在
来源：http://ajr.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gkh.nwbrower.top

[R07] if 判断文件
来源：http://fws.jinqigfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ixd.chenzaomai.com

[R08] 数值比较
来源：http://dko.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iov.jianghu66.top

[R09] 字符串比较
来源：http://etb.ydzc1.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bdz.ydjk.org.cn

[R10] 正则匹配
来源：http://tte.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oxb.zdbjq.cn

[R11] case 多分支
来源：http://jlh.gogol.net.cn

case "$1" in
来源：http://fdz.ybcxt.top

start) echo "启动" ;;
来源：http://wvf.zhoulong.xyz

stop)  echo "停止" ;;
来源：http://dkg.yangfankeji.com

*)     echo "未知命令" ;;
来源：http://vlf.ydzc1.top

esac
来源：http://nsh.yj202588.top

[R12] for 遍历文件
来源：http://nhx.ydjk.org.cn

for f in *.txt; do echo "$f"; done
来源：http://gbv.hysaishi.cn

[R13] for 计数循环
来源：http://peb.tarul.cn

for i in {1..10}; do echo "$i"; done
来源：http://czr.aizwys.cn

[R14] C 风格 for
来源：http://grm.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jcw.zhixingplan.top

[R15] while 逐行读文件
来源：http://bky.jqgfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aav.nanxuanxn.top

[R16] until 等待条件
来源：http://gxz.hnxiangtu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ebg.yongpay.top

[R17] 数组定义与取值
来源：http://uks.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://aqo.redwolf501.top

[R18] 遍历数组
来源：http://rar.dianchejie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tes.dianchejie.cn

[R19] 数组长度
来源：http://ocx.nwbrower.top

echo "${#arr[@]}"
来源：http://vvh.chenzaomai.com

[R20] 关联数组（字典）
来源：http://ugw.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fpm.hongshengwenyu.top

[R21] 字符串长度
来源：http://zlm.cucudq.cn

echo "${#s}"
来源：http://cqa.tanke756.top

[R22] 截取子串
来源：http://czg.nwbrower.top

echo "${s:0:5}"
来源：http://ujs.zhaomingkeji.xyz

[R23] 字符串替换
来源：http://hkp.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://btk.zhixingplan.top

[R24] 大小写转换
来源：http://xiy.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tsd.ppjwa.cn

[R25] 去后缀 / 去前缀
来源：http://eta.vehdjk.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://tuw.jqgufenzy.top

[R26] 命令替换
来源：http://cqf.sweek.top

now=$(date +%F); echo "$now"
来源：http://trg.zhongyouzk.top

[R27] 算术展开
来源：http://bjz.fengsongda.top

echo $((1 + 2 * 3))
来源：http://eoo.shuidangran.top

[R28] 浮点运算
来源：http://ybf.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://mog.guowangkeji.top

[R29] 定义函数
来源：http://rgf.xingfuxueyuan.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://egu.xylfe.cn

[R30] 函数返回状态码
来源：http://hpk.hfpthk.cn

f() { return 0; }; f || echo "失败了"
来源：http://yxc.shuidangran.top

[R31] 局部变量
来源：http://rnc.zhijiandao.cn

f() { local x=1; echo "$x"; }
来源：http://erk.fanxiaobao.xyz

[R32] 参数个数校验
来源：http://bze.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nrl.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://tnw.xuetiantiany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oqk.jinghuilouyu.cn

[R34] 退出时清理
来源：http://zlg.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://bur.shuidangran.top

[R35] 后台执行并等待
来源：http://wvl.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wxf.dianchejie.cn

[R36] 并发执行多个任务
来源：http://wrw.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hft.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://jqm.guowangkeji.top

files=$(ls -1)
来源：http://zbl.yj20258.top

[R38] 管道串联
来源：http://mfc.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://jix.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://uwi.uphjek.com

cmd > out.log 2>&1
来源：http://xup.guannengcc.top

[R40] 追加写日志
来源：http://klp.hesvh.cn

echo "log" >> out.log
来源：http://xio.vqdsnc.cn

[R41] 丢弃输出
来源：http://kpi.tarul.cn

cmd >/dev/null 2>&1
来源：http://xuh.hywenlv.cn

[R42] 输入重定向
来源：http://rga.yj20258888.top

wc -l < a.txt
来源：http://dta.nanxuanxn.top

[R43] 按名字查找文件
来源：http://wkx.zycfv.cn

find . -name "*.log" -type f
来源：http://qaz.xylfe.cn

[R44] 按修改时间查找
来源：http://lnd.jinqigfzy.top

find . -mtime -7 -type f
来源：http://ihp.fanxiaobao.xyz

[R45] 批量删除
来源：http://cxa.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://gok.cqqwz.cn

[R46] 递归替换文件内容
来源：http://nsc.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://caw.aibaodan.cn

[R47] sed 单行替换
来源：http://fao.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://oay.yj202588.top

[R48] awk 取指定列
来源：http://bxo.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://zms.haohaochexian.top

[R49] awk 带条件
来源：http://xiz.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mry.yvedp.cn

[R50] awk 求和
来源：http://jmp.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://bcq.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://zau.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://jur.bbcook.cn

[R52] 统计行数
来源：http://fxo.yj202588.top

wc -l a.txt
来源：http://tkm.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://fzd.ivvv.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yqb.zhixingplan.top

[R54] 比较两个文件
来源：http://mzi.quarkkingdee.top

diff a.txt b.txt
来源：http://yiw.9152youxi.cn

[R55] 压缩与解压
来源：http://ipx.vqdsnc.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nmm.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://gjx.sjlbkw.cn

scp file user@host:/path/
来源：http://vmf.hongshengwenyu.top

[R57] 远程执行命令
来源：http://ddq.kuanghao11.cn

ssh user@host 'uptime'
来源：http://hgl.nwbrower.top

[R58] 下载文件
来源：http://xbi.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eob.ehwqpu.com

[R59] 发 POST JSON
来源：http://zrn.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mgw.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://lcn.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tsy.haohaochexian.top

[R61] 磁盘占用
来源：http://bek.jianghu66.top

df -h;  du -sh *
来源：http://mbv.ivvv.top

[R62] 找最占空间的文件
来源：http://qxh.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://cdd.xuetiantiany.cn

[R63] 内存与进程
来源：http://fap.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://fjz.ydzc1.top

[R64] 结束进程
来源：http://ikv.meibo888.top

kill -9 $(pgrep -f app.py)
来源：http://sgp.hywenlv.cn

[R65] 查看端口占用
来源：http://hzc.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wer.fktsv.cn

[R66] 定时任务
来源：http://ikl.hesvh.cn

crontab -e;  crontab -l
来源：http://ijc.jinyuanbaomall.cn

[R67] 生成随机十六进制串
来源：http://wxt.fzhhl.top

openssl rand -hex 16
来源：http://lln.hfpthk.cn

[R68] 计算文件校验值
来源：http://nse.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://ldu.uphjek.com

[R69] 生成随机密码
来源：http://hqm.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://nxq.dianchejie.cn

[R70] 时间戳与互转
来源：http://snz.316326.xyz

date +%s;  date -d @1700000000
来源：http://dfh.fzhhl.top

[R71] 日期格式化
来源：http://vjr.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kkm.tian-w.cn

[R72] 等待端口就绪
来源：http://bir.0kj1m.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dvv.nanxinkj.top

[R73] 分割大日志
来源：http://bxx.hysaishi.cn

split -l 1000 big.log part_
来源：http://ymo.52xcode.cn

[R74] 批量重命名
来源：http://swe.haohaochexian.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ivi.0kj1m.cn

[R75] 导出环境变量
来源：http://zgz.ydjk.org.cn

export PATH="$HOME/bin:$PATH"
来源：http://opq.sysykeji.top

[R76] 使用临时文件
来源：http://tir.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jem.fktsv.cn

[R77] 读取用户输入
来源：http://qlx.andypj.xyz

read -rp "请输入: " ans
来源：http://bwa.meibo888.top

[R78] 交互式菜单
来源：http://jnv.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://zvb.shangyingyoupin.top

[R79] 解析命令行选项
来源：http://zwn.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wgx.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://aeb.zdqjudy.top

time ./run.sh
来源：http://zdb.redwolf501.top

================================================================================
来源：http://emo.chenjidiqi.icu

S. C / C++ 专题
来源：http://pwa.hysaishi.cn

================================================================================
来源：http://bor.jqgfzy.top

[S01] C：Hello World
来源：http://ayf.feifeiyinyue.top

#include <stdio.h>
来源：http://rzm.epnwcf.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://hob.hysaishi.cn

[S02] C：变量与格式化输出
来源：http://eyw.316326.xyz

int a = 10; printf("%d\n", a);
来源：http://onp.jyoumei.cn

[S03] C：读入整数
来源：http://ylp.mhx1999.top

int x; scanf("%d", &x);
来源：http://qol.jinqigfzy.top

[S04] C：字符串复制
来源：http://zcl.guannengcc.top

char dst[32]; strcpy(dst, "hi");
来源：http://gwu.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://nbc.hfpthk.cn

strlen(s)
来源：http://huv.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://myh.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://msm.tarul.cn

[S07] C：数组遍历求和
来源：http://nav.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ops.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://hgt.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://egf.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://umg.zycfv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zgb.ydjk.org.cn

[S10] C：指针与解引用
来源：http://qbr.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://wbw.zdbjq.cn

[S11] C：逐行读文件
来源：http://sbn.jianghu66.top

FILE *f = fopen("a.txt", "r");
来源：http://cnu.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rln.birdmap.top

fclose(f);
来源：http://vob.fzhhl.top

[S12] C：写文件
来源：http://oui.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sjq.tianlin.xyz

[S13] C：宏定义
来源：http://zrh.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cff.pengpengdd.cyou

[S14] C：枚举
来源：http://usm.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://rsh.wangdashe.top

[S15] C：类型转换
来源：http://kie.yanxiufei.cn

(double) a / b
来源：http://txr.gotoacloud.top

[S16] C：位操作置位
来源：http://pxe.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://smw.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://dsa.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hbi.sysykeji.top

[S18] C：命令行参数
来源：http://luy.sweek.top

int main(int argc, char **argv)
来源：http://gof.yueranfly.top

[S19] C：快速排序
来源：http://wqr.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://erx.dashuyun.cn

[S20] C：二分查找
来源：http://yck.jinqigufen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://img.fehbvm.com

[S21] C：字符类别判断
来源：http://qxr.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://stv.hysaishi.cn

[S22] C：字符串转数字
来源：http://gpw.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://rrh.snrcjt.cn

[S23] C：随机数
来源：http://say.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://mxa.hammf.cn

[S24] C：获取本地时间
来源：http://xuu.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yew.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://itq.havefunace.top

memcpy(dst, src, n);
来源：http://yhw.tarul.cn

[S26] C：内存清零
来源：http://nao.chenlongwang.top

memset(a, 0, sizeof a);
来源：http://dym.shangyingyoupin.top

[S27] C：定义常量
来源：http://tbu.zhoulong.xyz

const double PI = 3.14159;
来源：http://meo.cashguo.top

[S28] C：静态变量
来源：http://pzi.yj20258888.top

static int counter = 0;
来源：http://dtq.fzhhl.top

[S29] C：变参函数
来源：http://ctw.jlsjyb.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rdb.vehdjk.com

[S30] C：头文件保护
来源：http://gga.meibo888.top

#ifndef X_H
来源：http://yst.jiagoushi.top

#define X_H
来源：http://nmo.guannengcc.top

#endif
来源：http://xvc.sysykeji.top

[S31] C++：Hello World
来源：http://bfp.jyoumei.cn


<!-- 参考信息 -->