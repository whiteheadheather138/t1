代发 wailian999

[Q44] IN 子查询
来源：http://rdx.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qsg.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://rdp.haohaochexian.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zar.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://dqo.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fno.fengsongda.top

[Q47] 与平均值比较
来源：http://bmp.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vfa.sysykeji.top

[Q48] CTE 公用表表达式
来源：http://wrw.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gwr.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://egi.zhijiandao.cn

[Q49] 更新单行
来源：http://mfy.hfpthk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ifv.aizwys.cn

[Q50] 批量更新
来源：http://sec.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pet.hammf.cn

[Q51] 用子查询更新
来源：http://ech.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hzz.ivvv.top

[Q52] 删除指定行
来源：http://xqd.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://hkv.yj20258.top

[Q53] 按条件删除
来源：http://ufq.c1oappe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yzl.yj20258888.top

[Q54] 清空表
来源：http://ern.zhiwuduotai.top

TRUNCATE TABLE logs;
来源：http://duv.yuxming.cn

[Q55] 排名（并列占位）
来源：http://bsf.jqgfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://njj.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://jtx.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://emz.yongpay.top

[Q57] 行号
来源：http://ugj.yanxiufei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hxl.ivvv.top

[Q58] 累计求和
来源：http://wme.epnwcf.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wej.guannengcc.top

[Q59] 分组内累计
来源：http://zpk.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mgp.jinqigfzy.top

[Q60] 取上一行 / 下一行
来源：http://oqo.cheryme.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tlq.aibaodan.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eyo.hfpthk.cn

[Q61] 移动平均
来源：http://vjb.gogol.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ivb.cdnleiting.top

[Q62] 分组占比
来源：http://chg.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hzi.birdmap.top

[Q63] 开启事务
来源：http://gqs.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ylh.jqgfzy.top

[Q64] 提交事务
来源：http://dwz.tian-w.cn

COMMIT;
来源：http://owi.cdnleiting.top

[Q65] 回滚事务
来源：http://eet.ydjk.org.cn

ROLLBACK;
来源：http://xlu.bjfxy.top

[Q66] 行锁查询
来源：http://wfv.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tkg.birdmap.top

[Q67] 设置隔离级别
来源：http://wnw.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ruz.kuanghao11.cn

[Q68] 保存点
来源：http://emj.pengpengdd.cyou

SAVEPOINT sp1;
来源：http://ntv.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://cux.haohaochexian.top

[Q69] 查看执行计划
来源：http://xmz.fktsv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://beb.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://poi.jinghuilouyu.cn

ANALYZE TABLE users;
来源：http://hgz.sjlbkw.cn

[Q71] 查看建表语句
来源：http://yth.dashuyun.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jtt.cashguo.top

[Q72] 查看索引
来源：http://qoh.xziqi.cn

SHOW INDEX FROM users;
来源：http://gtp.cashguo.top

[Q73] 查看表状态
来源：http://vjn.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://erp.uphjek.com

[Q74] 强制使用索引
来源：http://tjk.yangfankeji.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://exs.zhoulong.xyz

[Q75] 日期格式化
来源：http://ohg.fanxiaobao.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bui.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bjo.xylfe.cn

[Q76] 按天统计
来源：http://kig.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vnm.ybcxt.top

[Q77] 时间加减
来源：http://soi.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bng.xinyue.icu

[Q78] 当前时间
来源：http://hdt.redwolf501.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vii.52xcode.cn

[Q79] 字符串拼接
来源：http://ffs.wangdashe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jwe.wangdashe.top

[Q80] 字符串截取
来源：http://bji.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jqi.guowangkeji.top

[Q81] 字符串替换
来源：http://uvc.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cco.cdnleiting.top

[Q82] 字符长度与字节长度
来源：http://cbu.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cbn.yuxming.cn

[Q83] 大小写转换
来源：http://bgv.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uub.fehbvm.com

[Q84] 去除首尾空格
来源：http://bct.xinyue.icu

SELECT TRIM(name) FROM users;
来源：http://bpb.redwolf501.top

[Q85] 数值取整
来源：http://cci.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gmn.yonumen.top

[Q86] 读取 JSON 字段
来源：http://vbp.52xcode.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xre.c1oappe.top

[Q87] JSON 字段做条件
来源：http://hpt.shzxlz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://orq.ydjk.org.cn

[Q88] 行转列（条件聚合）
来源：http://drb.shangyingyoupin.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://but.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://odq.xylfe.cn

[Q89] 判断表是否存在
来源：http://irw.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ryr.vqdsnc.cn

[Q90] 生成序号列
来源：http://upu.ydzc1.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dzo.gzhubu.top

================================================================================
来源：http://cdh.tianlin.xyz

R. Bash 专题
来源：http://qvf.hesvh.cn

================================================================================
来源：http://urg.mhx1999.top

[R01] shebang 与严格模式
来源：http://dpn.dashuyun.cn

#!/usr/bin/env bash
来源：http://lcw.ydjk.org.cn

set -euo pipefail
来源：http://pib.bbcook.cn

[R02] 变量赋值与使用
来源：http://btl.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://cvx.meibo888.top

[R03] 只读变量
来源：http://gcx.cqqwz.cn

readonly PI=3.14
来源：http://otu.9152youxi.cn

[R04] 位置参数
来源：http://mub.9152youxi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://czf.ppjwa.cn

[R05] 参数默认值
来源：http://lhj.hnqzz.top

name="${1:-default}"
来源：http://xsu.zhijiandao.cn

[R06] 判断命令是否存在
来源：http://qmb.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xhn.sufxvd.cn

[R07] if 判断文件
来源：http://pyc.sxryk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://utl.shzxlz.cn

[R08] 数值比较
来源：http://uld.jlsjyb.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://skn.sjlbkw.cn

[R09] 字符串比较
来源：http://ody.sjlbkw.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qxw.cqqwz.cn

[R10] 正则匹配
来源：http://kci.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://buo.sjlbkw.cn

[R11] case 多分支
来源：http://ceg.xuetiantiany.cn

case "$1" in
来源：http://lux.andypj.xyz

start) echo "启动" ;;
来源：http://off.wangdashe.top

stop)  echo "停止" ;;
来源：http://wbt.fengsongda.top

*)     echo "未知命令" ;;
来源：http://uzj.tianlin.xyz

esac
来源：http://jol.jlsjyb.cn

[R12] for 遍历文件
来源：http://wax.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://sqa.c1oappe.top

[R13] for 计数循环
来源：http://bvj.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://fpa.yj20258888.top

[R14] C 风格 for
来源：http://qvt.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oxw.cdnleiting.top

[R15] while 逐行读文件
来源：http://fsu.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vuu.svipenyu.cn

[R16] until 等待条件
来源：http://vhm.shzxlz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rzp.sysykeji.top

[R17] 数组定义与取值
来源：http://gqo.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://fot.yfazqb.com

[R18] 遍历数组
来源：http://khx.jqgfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ooh.nwbrower.top

[R19] 数组长度
来源：http://cpq.nanxinkj.top

echo "${#arr[@]}"
来源：http://rcq.pycfn.com

[R20] 关联数组（字典）
来源：http://jjp.quarkkingdee.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sby.epnwcf.com

[R21] 字符串长度
来源：http://nbd.sysykeji.top

echo "${#s}"
来源：http://bdx.zhoulong.xyz

[R22] 截取子串
来源：http://yuu.fengsongda.top

echo "${s:0:5}"
来源：http://vpv.52xcode.cn

[R23] 字符串替换
来源：http://iqu.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sjs.kuanghao11.cn

[R24] 大小写转换
来源：http://jsq.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://aji.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://jjj.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://qbv.chenjidiqi.icu

[R26] 命令替换
来源：http://oko.yvedp.cn

now=$(date +%F); echo "$now"
来源：http://zjr.zdqjudy.top

[R27] 算术展开
来源：http://nee.ydjk.org.cn

echo $((1 + 2 * 3))
来源：http://vud.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://hdt.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://tof.chenzaomai.com

[R29] 定义函数
来源：http://vyg.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iwf.dashuyun.cn

[R30] 函数返回状态码
来源：http://qjw.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://out.xingfuxueyuan.xyz

[R31] 局部变量
来源：http://cvf.hfpthk.cn

f() { local x=1; echo "$x"; }
来源：http://sfd.cdnleiting.top

[R32] 参数个数校验
来源：http://zkn.smart0.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://utw.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://ysn.xingfuxueyuan.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qks.ydzc1.top

[R34] 退出时清理
来源：http://ksf.nanxuanxn.top

trap 'rm -f "$tmp"' EXIT
来源：http://cjy.tanke756.top

[R35] 后台执行并等待
来源：http://tnu.316326.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://rjw.bjfxy.top

[R36] 并发执行多个任务
来源：http://dpr.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hlo.yangfankeji.com

[R37] 把输出赋给变量
来源：http://xdn.wangdashe.top

files=$(ls -1)
来源：http://whx.iojbl.cn

[R38] 管道串联
来源：http://jft.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://jba.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://pyb.zdbjq.cn

cmd > out.log 2>&1
来源：http://vot.fzhhl.top

[R40] 追加写日志
来源：http://ror.wangshuangyany.cn

echo "log" >> out.log
来源：http://pnn.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://kjy.jqgufenzy.top

cmd >/dev/null 2>&1
来源：http://ssf.andypj.xyz

[R42] 输入重定向
来源：http://jsy.jlsjyb.cn

wc -l < a.txt
来源：http://axs.zhengqikj.top

[R43] 按名字查找文件
来源：http://sgg.jqgfzy.top

find . -name "*.log" -type f
来源：http://hlq.yfazqb.com

[R44] 按修改时间查找
来源：http://yjf.daria6918.cn

find . -mtime -7 -type f
来源：http://wfi.iojbl.cn

[R45] 批量删除
来源：http://gfs.yvedp.cn

find . -name "*.tmp" -delete
来源：http://iqr.hysaishi.cn

[R46] 递归替换文件内容
来源：http://gar.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qwg.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://csf.guannengcc.top

sed -i 's/foo/bar/g' a.txt
来源：http://hzd.shuidangran.top

[R48] awk 取指定列
来源：http://bqu.yuxming.cn

awk '{print $1, $3}' a.txt
来源：http://ucn.kuanghao11.cn

[R49] awk 带条件
来源：http://grx.vehdjk.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://slm.hywenlv.cn

[R50] awk 求和
来源：http://ryk.52xcode.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qur.yanxiufei.cn

[R51] 排序去重取前几
来源：http://euk.tian-w.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sod.fengsongda.top

[R52] 统计行数
来源：http://roi.zhoulong.xyz

wc -l a.txt
来源：http://fkw.jinqigufen.top

[R53] 查看文件头与实时尾
来源：http://ytr.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fwm.cdnleiting.top

[R54] 比较两个文件
来源：http://oou.fzhhl.top

diff a.txt b.txt
来源：http://pow.andypj.xyz

[R55] 压缩与解压
来源：http://npc.fktsv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sfq.redwolf501.top

[R56] 远程拷贝
来源：http://wvn.fengsongda.top

scp file user@host:/path/
来源：http://eup.wangdashe.top

[R57] 远程执行命令
来源：http://utl.epnwcf.com

ssh user@host 'uptime'
来源：http://yfb.ivvv.top

[R58] 下载文件
来源：http://kvi.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rwl.zdqjudy.top

[R59] 发 POST JSON
来源：http://ojv.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://erb.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://jyj.fengsongda.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rtk.andypj.xyz

[R61] 磁盘占用
来源：http://elg.sjlbkw.cn

df -h;  du -sh *
来源：http://vba.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://jka.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://gle.zhixingplan.top

[R63] 内存与进程
来源：http://emx.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://zfx.jianghu66.top

[R64] 结束进程
来源：http://bqu.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://cfj.hesvh.cn

[R65] 查看端口占用
来源：http://xrd.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://elb.zhongyouzk.top

[R66] 定时任务
来源：http://hum.52xcode.cn

crontab -e;  crontab -l
来源：http://nqu.fengsongda.top

[R67] 生成随机十六进制串
来源：http://ggv.ctjpmb.com

openssl rand -hex 16
来源：http://hrp.zhixingplan.top

[R68] 计算文件校验值
来源：http://scw.hnxiangtu.top

sha256sum a.txt;  md5sum a.txt
来源：http://xrp.yvedp.cn

[R69] 生成随机密码
来源：http://qoc.jyoumei.cn

head -c 16 /dev/urandom | base64
来源：http://lxp.jinqigfzy.top

[R70] 时间戳与互转
来源：http://gvx.xinyue.icu

date +%s;  date -d @1700000000
来源：http://ywx.bjfxy.top

[R71] 日期格式化
来源：http://bwk.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rmh.ctjpmb.com

[R72] 等待端口就绪
来源：http://llv.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kpg.tianlin.xyz

[R73] 分割大日志
来源：http://tny.xingfuxueyuan.xyz

split -l 1000 big.log part_
来源：http://qvh.zdbjq.cn

[R74] 批量重命名
来源：http://xrl.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tbv.zhongyouzk.top

[R75] 导出环境变量
来源：http://itz.zhiwuduotai.top

export PATH="$HOME/bin:$PATH"
来源：http://tju.guannengcc.top

[R76] 使用临时文件
来源：http://ucu.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://omt.zhixingplan.top

[R77] 读取用户输入
来源：http://uhn.fengsongda.top

read -rp "请输入: " ans
来源：http://enj.fzhhl.top

[R78] 交互式菜单
来源：http://lnx.fehbvm.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ait.sufxvd.cn

[R79] 解析命令行选项
来源：http://dlz.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mkp.tanke756.top

[R80] 查看脚本执行耗时
来源：http://ewh.pengpengdd.cyou

time ./run.sh
来源：http://exj.ctjpmb.com

================================================================================
来源：http://hqr.tanke756.top

S. C / C++ 专题
来源：http://evk.xinyue.icu

================================================================================
来源：http://tve.hongshengwenyu.top

[S01] C：Hello World
来源：http://suz.jinqigufen.top

#include <stdio.h>
来源：http://oim.shangyingyoupin.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pqi.yonumen.top

[S02] C：变量与格式化输出
来源：http://uid.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://pfx.epnwcf.com

[S03] C：读入整数
来源：http://icl.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://mvl.bbcook.cn

[S04] C：字符串复制
来源：http://juy.iojbl.cn

char dst[32]; strcpy(dst, "hi");
来源：http://txf.sxryk.cn

[S05] C：字符串长度
来源：http://ztb.jlsjyb.cn

strlen(s)
来源：http://iju.daria6918.cn

[S06] C：字符串比较
来源：http://twg.svipenyu.cn

strcmp(a, b) == 0
来源：http://xlu.cqqwz.cn

[S07] C：数组遍历求和
来源：http://win.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://txy.hammf.cn

[S08] C：动态内存分配与释放
来源：http://kos.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tkh.shangyingyoupin.top

[S09] C：结构体定义与初始化
来源：http://zxn.feifeiyinyue.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pxh.haohaochexian.top

[S10] C：指针与解引用
来源：http://oia.yonumen.top

int *p = &a;  *p = 5;
来源：http://sky.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://duh.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://uiw.hysaishi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qec.zhixingplan.top

fclose(f);
来源：http://yyt.xylfe.cn

[S12] C：写文件
来源：http://dys.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tka.guannengcc.top

[S13] C：宏定义
来源：http://mre.zhixingplan.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yuh.0kj1m.cn

[S14] C：枚举
来源：http://nln.wangdashe.top


<!-- 参考信息 -->