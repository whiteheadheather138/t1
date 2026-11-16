代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://kdc.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cbw.birdmap.top

[Q47] 与平均值比较
来源：http://kvn.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vcs.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://lav.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://akh.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://dde.snrcjt.cn

[Q49] 更新单行
来源：http://tid.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jmx.tarul.cn

[Q50] 批量更新
来源：http://cqh.shanyushiyangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hdp.mhx1999.top

[Q51] 用子查询更新
来源：http://rvc.xinyue.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bqu.dashuyun.cn

[Q52] 删除指定行
来源：http://qfw.xingfuxueyuan.xyz

DELETE FROM users WHERE id = 10;
来源：http://ljw.jianghu66.top

[Q53] 按条件删除
来源：http://unv.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://biw.cheryme.top

[Q54] 清空表
来源：http://pog.jinqigufen.top

TRUNCATE TABLE logs;
来源：http://smp.xuanzx.com

[Q55] 排名（并列占位）
来源：http://hmb.pycfn.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vdl.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://ggj.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://khj.52xcode.cn

[Q57] 行号
来源：http://oaf.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rxw.cdnleiting.top

[Q58] 累计求和
来源：http://ibn.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hcd.aibaodan.cn

[Q59] 分组内累计
来源：http://znz.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ypd.shanyushiyangtech.top

[Q60] 取上一行 / 下一行
来源：http://mtp.jinqigufen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uqk.daria6918.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zqp.vehdjk.com

[Q61] 移动平均
来源：http://rjz.jinqigufen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aje.jqgufenzy.top

[Q62] 分组占比
来源：http://dsh.pengpengdd.cyou

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kle.xuetiantiany.cn

[Q63] 开启事务
来源：http://whh.jqgfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nym.hesvh.cn

[Q64] 提交事务
来源：http://mux.pengpengdd.cyou

COMMIT;
来源：http://yui.chenjidiqi.icu

[Q65] 回滚事务
来源：http://zkc.dianchejie.cn

ROLLBACK;
来源：http://gms.jyoumei.cn

[Q66] 行锁查询
来源：http://pxc.zhixingplan.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ynm.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://xpd.zdbjq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mab.xinyue.icu

[Q68] 保存点
来源：http://kym.tarul.cn

SAVEPOINT sp1;
来源：http://hhp.yuxming.cn

ROLLBACK TO sp1;
来源：http://fvs.yj20258888.top

[Q69] 查看执行计划
来源：http://iqe.0kj1m.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xkd.jinqigufen.top

[Q70] 更新统计信息
来源：http://tto.aizwys.cn

ANALYZE TABLE users;
来源：http://sjl.kuanghao11.cn

[Q71] 查看建表语句
来源：http://uau.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yte.fengsongda.top

[Q72] 查看索引
来源：http://rjb.aizwys.cn

SHOW INDEX FROM users;
来源：http://tym.zhijiandao.cn

[Q73] 查看表状态
来源：http://gyf.hongshengwenyu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gqo.yfazqb.com

[Q74] 强制使用索引
来源：http://lrc.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://svt.fktsv.cn

[Q75] 日期格式化
来源：http://chr.chenlongwang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rvo.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ynw.shanyushiyangtech.top

[Q76] 按天统计
来源：http://pxx.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ysx.pycfn.com

[Q77] 时间加减
来源：http://gns.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mbz.zdqjudy.top

[Q78] 当前时间
来源：http://ips.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nbm.zhongyouzk.top

[Q79] 字符串拼接
来源：http://mkx.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rtn.yonumen.top

[Q80] 字符串截取
来源：http://sxg.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://isj.ybcxt.top

[Q81] 字符串替换
来源：http://zle.shuidangran.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zra.sysykeji.top

[Q82] 字符长度与字节长度
来源：http://ees.xinyue.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jnl.tian-w.cn

[Q83] 大小写转换
来源：http://xgr.ctjpmb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fnv.9152youxi.cn

[Q84] 去除首尾空格
来源：http://jxh.meibo888.top

SELECT TRIM(name) FROM users;
来源：http://kvn.hfpthk.cn

[Q85] 数值取整
来源：http://uul.zhoulong.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mvp.zdqjudy.top

[Q86] 读取 JSON 字段
来源：http://zgq.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zur.epnwcf.com

[Q87] JSON 字段做条件
来源：http://jup.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nmx.wangdashe.top

[Q88] 行转列（条件聚合）
来源：http://cdn.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://boq.shzxlz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wob.sxryk.cn

[Q89] 判断表是否存在
来源：http://sae.zdbjq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cop.gzhubu.top

[Q90] 生成序号列
来源：http://aat.andypj.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ggw.zhiwuduotai.top

================================================================================
来源：http://nzq.hnxiangtu.top

R. Bash 专题
来源：http://afn.tian-w.cn

================================================================================
来源：http://lqt.meibo888.top

[R01] shebang 与严格模式
来源：http://kdz.andypj.xyz

#!/usr/bin/env bash
来源：http://liw.zhongyouzk.top

set -euo pipefail
来源：http://tps.havefunace.top

[R02] 变量赋值与使用
来源：http://bsj.hcnkem.com

name="Tom"; echo "$name"
来源：http://izw.shangyingyoupin.top

[R03] 只读变量
来源：http://hcd.sweek.top

readonly PI=3.14
来源：http://mbe.sweek.top

[R04] 位置参数
来源：http://zab.smart0.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ciz.sufxvd.cn

[R05] 参数默认值
来源：http://vhb.tanke756.top

name="${1:-default}"
来源：http://wcu.zhiwuduotai.top

[R06] 判断命令是否存在
来源：http://ojs.pengpengdd.cyou

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wos.tianlin.xyz

[R07] if 判断文件
来源：http://jwk.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xtq.wangdashe.top

[R08] 数值比较
来源：http://fnk.gogol.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dvm.zycfv.cn

[R09] 字符串比较
来源：http://mso.jinqigufen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ysk.havefunace.top

[R10] 正则匹配
来源：http://lpc.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://imv.daria6918.cn

[R11] case 多分支
来源：http://tgf.xziqi.cn

case "$1" in
来源：http://nwv.jyoumei.cn

start) echo "启动" ;;
来源：http://vbj.svipenyu.cn

stop)  echo "停止" ;;
来源：http://gwl.xziqi.cn

*)     echo "未知命令" ;;
来源：http://oem.birdmap.top

esac
来源：http://pst.zhixingplan.top

[R12] for 遍历文件
来源：http://xbc.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://efn.daria6918.cn

[R13] for 计数循环
来源：http://psz.jianghu66.top

for i in {1..10}; do echo "$i"; done
来源：http://gjo.xuetiantiany.cn

[R14] C 风格 for
来源：http://esw.cqqwz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iqe.haohaochexian.top

[R15] while 逐行读文件
来源：http://zqg.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uup.cucudq.cn

[R16] until 等待条件
来源：http://muy.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ybz.cdnleiting.top

[R17] 数组定义与取值
来源：http://qau.hongshengwenyu.top

arr=(a b c); echo "${arr[0]}"
来源：http://rit.xziqi.cn

[R18] 遍历数组
来源：http://wgd.quarkkingdee.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tmj.yfazqb.com

[R19] 数组长度
来源：http://nxb.gogol.net.cn

echo "${#arr[@]}"
来源：http://stf.hywenlv.cn

[R20] 关联数组（字典）
来源：http://wbm.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://chl.shzxlz.cn

[R21] 字符串长度
来源：http://qyj.pengpengdd.cyou

echo "${#s}"
来源：http://dry.xinyue.icu

[R22] 截取子串
来源：http://uxm.ywan-chungtsiang.top

echo "${s:0:5}"
来源：http://abj.sysykeji.top

[R23] 字符串替换
来源：http://zjb.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uys.ivvv.top

[R24] 大小写转换
来源：http://hhl.yueranfly.top

echo "${s^^}"; echo "${s,,}"
来源：http://jdp.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://unt.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wln.bjfxy.top

[R26] 命令替换
来源：http://ekq.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://hfv.fanxiaobao.xyz

[R27] 算术展开
来源：http://tjp.vehdjk.com

echo $((1 + 2 * 3))
来源：http://jes.ybcxt.top

[R28] 浮点运算
来源：http://puv.cheryme.top

echo "scale=2; 10/3" | bc
来源：http://eln.daxiang520.top

[R29] 定义函数
来源：http://ppd.yueranfly.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zvc.yfazqb.com

[R30] 函数返回状态码
来源：http://eff.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://xai.hnxiangtu.top

[R31] 局部变量
来源：http://gmb.guowangkeji.top

f() { local x=1; echo "$x"; }
来源：http://yqk.chenjidiqi.icu

[R32] 参数个数校验
来源：http://awa.dianchejie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xde.zycfv.cn

[R33] 捕获错误并提示行号
来源：http://lvj.fanxiaobao.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tvn.tianlin.xyz

[R34] 退出时清理
来源：http://fdg.jinqigufen.top

trap 'rm -f "$tmp"' EXIT
来源：http://aij.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://ddh.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zeq.zhixingplan.top

[R36] 并发执行多个任务
来源：http://ipi.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tex.yvedp.cn

[R37] 把输出赋给变量
来源：http://xwv.ywan-chungtsiang.top

files=$(ls -1)
来源：http://ifo.316326.xyz

[R38] 管道串联
来源：http://ryd.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://vot.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://qfk.jinqigufen.top

cmd > out.log 2>&1
来源：http://cmp.hnxiangtu.top

[R40] 追加写日志
来源：http://nda.jyoumei.cn

echo "log" >> out.log
来源：http://xdy.svipenyu.cn

[R41] 丢弃输出
来源：http://rqy.cucudq.cn

cmd >/dev/null 2>&1
来源：http://xuz.quarkkingdee.top

[R42] 输入重定向
来源：http://lvj.tanke756.top

wc -l < a.txt
来源：http://gli.aibaodan.cn

[R43] 按名字查找文件
来源：http://tjm.uphjek.com

find . -name "*.log" -type f
来源：http://aql.svipenyu.cn

[R44] 按修改时间查找
来源：http://bfr.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://yea.yuanzhike.top

[R45] 批量删除
来源：http://gqd.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://yym.fengsongda.top

[R46] 递归替换文件内容
来源：http://udf.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sdr.tarul.cn

[R47] sed 单行替换
来源：http://duf.wangshuangyany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wls.cheryme.top

[R48] awk 取指定列
来源：http://mff.jiagoushi.top

awk '{print $1, $3}' a.txt
来源：http://ssh.smart0.xyz

[R49] awk 带条件
来源：http://nfv.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://adv.sufxvd.cn

[R50] awk 求和
来源：http://wuj.uphjek.com

awk '{s += $2} END {print s}' a.txt
来源：http://vvd.zhixingplan.top

[R51] 排序去重取前几
来源：http://lkh.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cvw.zdbjq.cn

[R52] 统计行数
来源：http://adk.redwolf501.top

wc -l a.txt
来源：http://jmr.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://mul.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://szi.birdmap.top

[R54] 比较两个文件
来源：http://ats.tian-w.cn

diff a.txt b.txt
来源：http://hbj.gotoacloud.top

[R55] 压缩与解压
来源：http://abc.sweek.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zow.yanxiufei.cn

[R56] 远程拷贝
来源：http://aga.hnqzz.top

scp file user@host:/path/
来源：http://uzj.hysaishi.cn

[R57] 远程执行命令
来源：http://koh.vehdjk.com

ssh user@host 'uptime'
来源：http://qau.c1oappe.top

[R58] 下载文件
来源：http://sov.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fki.epnwcf.com

[R59] 发 POST JSON
来源：http://sgm.gogol.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vak.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://fov.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nbs.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://apo.ydzc1.top

df -h;  du -sh *
来源：http://fva.zhixingplan.top

[R62] 找最占空间的文件
来源：http://kqv.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://ghm.fktsv.cn

[R63] 内存与进程
来源：http://nfy.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://bvb.hcnkem.com

[R64] 结束进程
来源：http://atd.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://ubg.zhijiandao.cn

[R65] 查看端口占用
来源：http://bxq.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nyr.jqgufenzy.top

[R66] 定时任务
来源：http://ujt.jyoumei.cn

crontab -e;  crontab -l
来源：http://nxj.yvedp.cn

[R67] 生成随机十六进制串
来源：http://psh.yj20258888.top

openssl rand -hex 16
来源：http://qvq.fehbvm.com

[R68] 计算文件校验值
来源：http://gqf.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://ald.ybcxt.top

[R69] 生成随机密码
来源：http://nvc.yonumen.top

head -c 16 /dev/urandom | base64
来源：http://vzw.yj20258.top

[R70] 时间戳与互转
来源：http://qpw.tarul.cn

date +%s;  date -d @1700000000
来源：http://qfr.ehwqpu.com

[R71] 日期格式化
来源：http://rvv.zhongyouzk.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pat.birdmap.top

[R72] 等待端口就绪
来源：http://hmq.0kj1m.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hyo.ppjwa.cn

[R73] 分割大日志
来源：http://ums.hysaishi.cn

split -l 1000 big.log part_
来源：http://raz.ydjk.org.cn

[R74] 批量重命名
来源：http://emy.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pxe.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://ufd.yfazqb.com

export PATH="$HOME/bin:$PATH"
来源：http://stv.ydzc1.top

[R76] 使用临时文件
来源：http://ytd.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ysp.zdqjudy.top

[R77] 读取用户输入
来源：http://qyj.dianchejie.cn

read -rp "请输入: " ans
来源：http://ynn.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://ehl.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wiq.yfazqb.com

[R79] 解析命令行选项
来源：http://gkm.zdqjudy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qif.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://gng.xuetiantiany.cn

time ./run.sh
来源：http://pda.fzhhl.top

================================================================================
来源：http://jwm.jyoumei.cn

S. C / C++ 专题
来源：http://uai.quarkkingdee.top

================================================================================
来源：http://eqh.ehwqpu.com

[S01] C：Hello World
来源：http://yuc.guannengcc.top

#include <stdio.h>
来源：http://tbe.9152youxi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pva.xziqi.cn

[S02] C：变量与格式化输出
来源：http://kgw.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://gao.andypj.xyz

[S03] C：读入整数
来源：http://jog.shuidangran.top

int x; scanf("%d", &x);
来源：http://duh.xuanzx.com

[S04] C：字符串复制
来源：http://cgp.shangyingyoupin.top

char dst[32]; strcpy(dst, "hi");
来源：http://ysz.guannengcc.top

[S05] C：字符串长度
来源：http://beu.dianchejie.cn

strlen(s)
来源：http://mlw.yonumen.top

[S06] C：字符串比较
来源：http://cpb.sjlbkw.cn

strcmp(a, b) == 0
来源：http://vii.vehdjk.com

[S07] C：数组遍历求和
来源：http://zze.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fgw.hcnkem.com

[S08] C：动态内存分配与释放
来源：http://akw.ydzc1.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://azt.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://lff.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ifl.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://ppp.epnwcf.com

int *p = &a;  *p = 5;
来源：http://gkr.birdmap.top

[S11] C：逐行读文件
来源：http://ihu.cqqwz.cn

FILE *f = fopen("a.txt", "r");
来源：http://rkt.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://qoo.fanxiaobao.xyz

fclose(f);
来源：http://wqg.feifeiyinyue.top

[S12] C：写文件
来源：http://rpi.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xtl.hnqzz.top

[S13] C：宏定义
来源：http://qsw.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xiv.jqgufenzy.top

[S14] C：枚举
来源：http://oto.jlsjyb.cn

enum Color { RED, GREEN, BLUE };
来源：http://zwl.kuanghao11.cn

[S15] C：类型转换
来源：http://hga.gaohongyu789.top

(double) a / b
来源：http://drz.zycfv.cn

[S16] C：位操作置位
来源：http://ckk.xuanzx.com


<!-- 参考信息 -->