代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oku.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://iie.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eur.yangfankeji.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://egx.zhiwuduotai.top

[Q33] 多列分组
来源：http://vxd.hysaishi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://alc.zhijiandao.cn

[Q34] 每组取第一条
来源：http://lde.yanxiufei.cn

SELECT * FROM (
来源：http://rew.daxiang520.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://asc.wangdashe.top

) t WHERE rn = 1;
来源：http://kge.shanyushiyangtech.top

[Q35] 内连接
来源：http://ghh.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jep.52xcode.cn

[Q36] 左连接
来源：http://sce.gogol.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://obv.cdnleiting.top

[Q37] 右连接
来源：http://pdt.havefunace.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://suo.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ewm.cucudq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lvo.hongshengwenyu.top

[Q39] 自连接（查上下级）
来源：http://fts.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zgf.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uie.feifeiyinyue.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rdh.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xag.fzhhl.top

[Q41] 多表连接
来源：http://kcu.fengsongda.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dfo.zhixingplan.top

JOIN users u ON u.id = o.user_id
来源：http://fuz.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://kwp.tianlin.xyz

[Q42] 连接条件附加过滤
来源：http://zzm.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://bwe.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kgi.wangshuangyany.cn

[Q43] 标量子查询
来源：http://gwj.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qgi.yuxming.cn

[Q44] IN 子查询
来源：http://gwj.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://chv.yuanzhike.top

[Q45] EXISTS 判断存在
来源：http://rsz.jinqigufen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://joj.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://opk.ywan-chungtsiang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gao.hysaishi.cn

[Q47] 与平均值比较
来源：http://uzb.daria6918.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mfh.fengsongda.top

[Q48] CTE 公用表表达式
来源：http://zpk.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iel.smart0.xyz

SELECT * FROM t WHERE c > 5;
来源：http://bey.yuxming.cn

[Q49] 更新单行
来源：http://gaz.yj202588.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://poj.yonumen.top

[Q50] 批量更新
来源：http://gza.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dup.sxryk.cn

[Q51] 用子查询更新
来源：http://pnx.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dzh.gaohongyu789.top

[Q52] 删除指定行
来源：http://hbo.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://ozu.zycfv.cn

[Q53] 按条件删除
来源：http://emq.ybcxt.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oqt.hysaishi.cn

[Q54] 清空表
来源：http://zxg.xinyue.icu

TRUNCATE TABLE logs;
来源：http://wek.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://atn.ppjwa.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://srr.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://mdu.hnqzz.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lfb.zhiwuduotai.top

[Q57] 行号
来源：http://izl.chenlongwang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tlf.sweek.top

[Q58] 累计求和
来源：http://jvq.hcnkem.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wal.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://itb.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pck.bbcook.cn

[Q60] 取上一行 / 下一行
来源：http://wia.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://szk.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zgm.kuanghao11.cn

[Q61] 移动平均
来源：http://zxs.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hoq.gzhubu.top

[Q62] 分组占比
来源：http://fly.yonumen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vbl.pengpengdd.cyou

[Q63] 开启事务
来源：http://mcu.wangshuangyany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hyp.nanxinkj.top

[Q64] 提交事务
来源：http://www.52xcode.cn

COMMIT;
来源：http://wne.cheryme.top

[Q65] 回滚事务
来源：http://zxe.ctjpmb.com

ROLLBACK;
来源：http://wtp.xziqi.cn

[Q66] 行锁查询
来源：http://ufj.pycfn.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bul.316326.xyz

[Q67] 设置隔离级别
来源：http://fnz.fanxiaobao.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kmj.sxryk.cn

[Q68] 保存点
来源：http://pic.cheryme.top

SAVEPOINT sp1;
来源：http://axj.cashguo.top

ROLLBACK TO sp1;
来源：http://out.haohaochexian.top

[Q69] 查看执行计划
来源：http://leo.shanyushiyangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kzy.nanxinkj.top

[Q70] 更新统计信息
来源：http://aed.shzxlz.cn

ANALYZE TABLE users;
来源：http://qlk.hcnkem.com

[Q71] 查看建表语句
来源：http://mqp.yuanzhike.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wit.chenzaomai.com

[Q72] 查看索引
来源：http://fsn.ybcxt.top

SHOW INDEX FROM users;
来源：http://tce.andypj.xyz

[Q73] 查看表状态
来源：http://fvi.hesvh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gxg.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://nbr.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://apv.jinghuilouyu.cn

[Q75] 日期格式化
来源：http://geu.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ybk.yj202588.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://awk.ctjpmb.com

[Q76] 按天统计
来源：http://vpv.zhiwuduotai.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nxo.yanxiufei.cn

[Q77] 时间加减
来源：http://gge.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bdc.chenlongwang.top

[Q78] 当前时间
来源：http://iuu.sxryk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://biw.daria6918.cn

[Q79] 字符串拼接
来源：http://azb.yvedp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ije.guannengcc.top

[Q80] 字符串截取
来源：http://qpu.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cpp.jqgufenzy.top

[Q81] 字符串替换
来源：http://gvr.zhijiandao.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pze.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://ytc.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wlz.9152youxi.cn

[Q83] 大小写转换
来源：http://vkv.ydzc1.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gmo.chenzaomai.com

[Q84] 去除首尾空格
来源：http://nkw.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://upj.zhengqikj.top

[Q85] 数值取整
来源：http://lmq.zycfv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rpi.gaohongyu789.top

[Q86] 读取 JSON 字段
来源：http://ogk.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uji.quarkkingdee.top

[Q87] JSON 字段做条件
来源：http://drs.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dcj.kuanghao11.cn

[Q88] 行转列（条件聚合）
来源：http://nyc.iojbl.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zpq.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hal.xuanzx.com

[Q89] 判断表是否存在
来源：http://the.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eyl.chenjidiqi.icu

[Q90] 生成序号列
来源：http://amz.shanyushiyangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zlo.hnxiangtu.top

================================================================================
来源：http://tno.jianghu66.top

R. Bash 专题
来源：http://ygz.gzhubu.top

================================================================================
来源：http://xui.havefunace.top

[R01] shebang 与严格模式
来源：http://rhy.9152youxi.cn

#!/usr/bin/env bash
来源：http://qde.xingfuxueyuan.xyz

set -euo pipefail
来源：http://dee.aizwys.cn

[R02] 变量赋值与使用
来源：http://cqy.snrcjt.cn

name="Tom"; echo "$name"
来源：http://rws.hammf.cn

[R03] 只读变量
来源：http://pvz.yanxiufei.cn

readonly PI=3.14
来源：http://rls.chenzaomai.com

[R04] 位置参数
来源：http://ups.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://suj.jqgfzy.top

[R05] 参数默认值
来源：http://xou.ydjk.org.cn

name="${1:-default}"
来源：http://peg.dianchejie.cn

[R06] 判断命令是否存在
来源：http://xzy.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lqh.xinyue.icu

[R07] if 判断文件
来源：http://bqd.smart0.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rql.snrcjt.cn

[R08] 数值比较
来源：http://iyy.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://kzp.tian-w.cn

[R09] 字符串比较
来源：http://iwb.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://axm.yuxming.cn

[R10] 正则匹配
来源：http://yyk.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mpx.fengsongda.top

[R11] case 多分支
来源：http://mmn.meibo888.top

case "$1" in
来源：http://rnx.gaohongyu789.top

start) echo "启动" ;;
来源：http://iev.quarkkingdee.top

stop)  echo "停止" ;;
来源：http://ypx.yuxming.cn

*)     echo "未知命令" ;;
来源：http://wbc.jianghu66.top

esac
来源：http://ckp.yangfankeji.com

[R12] for 遍历文件
来源：http://pqf.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://tpi.hysaishi.cn

[R13] for 计数循环
来源：http://cwv.yvedp.cn

for i in {1..10}; do echo "$i"; done
来源：http://nzl.gaohongyu789.top

[R14] C 风格 for
来源：http://wct.sweek.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bdd.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://nik.shangyingyoupin.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://enu.jinqigufen.top

[R16] until 等待条件
来源：http://wda.cqqwz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ctt.zhongyouzk.top

[R17] 数组定义与取值
来源：http://jxg.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://ihc.chenzaomai.com

[R18] 遍历数组
来源：http://ihp.cdnleiting.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qrh.cashguo.top

[R19] 数组长度
来源：http://gvc.yongpay.top

echo "${#arr[@]}"
来源：http://qdu.c1oappe.top

[R20] 关联数组（字典）
来源：http://efb.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kxo.ywan-chungtsiang.top

[R21] 字符串长度
来源：http://czf.nwbrower.top

echo "${#s}"
来源：http://nys.fengsongda.top

[R22] 截取子串
来源：http://ziq.yj202588.top

echo "${s:0:5}"
来源：http://jhl.fehbvm.com

[R23] 字符串替换
来源：http://urv.fanxiaobao.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tpv.jqgufenzy.top

[R24] 大小写转换
来源：http://gcj.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://shj.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://geq.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vmo.chenjidiqi.icu

[R26] 命令替换
来源：http://aza.shanyushiyangtech.top

now=$(date +%F); echo "$now"
来源：http://ooo.wangdashe.top

[R27] 算术展开
来源：http://tpe.yvedp.cn

echo $((1 + 2 * 3))
来源：http://xvq.ppjwa.cn

[R28] 浮点运算
来源：http://iyv.shangyingyoupin.top

echo "scale=2; 10/3" | bc
来源：http://aae.52xcode.cn

[R29] 定义函数
来源：http://phn.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://alv.wangdashe.top

[R30] 函数返回状态码
来源：http://ihp.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://zdx.bjfxy.top

[R31] 局部变量
来源：http://smz.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://tko.ivvv.top

[R32] 参数个数校验
来源：http://dnu.andypj.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jij.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://qfs.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fmc.uphjek.com

[R34] 退出时清理
来源：http://hix.pengpengdd.cyou

trap 'rm -f "$tmp"' EXIT
来源：http://oas.zhixingplan.top

[R35] 后台执行并等待
来源：http://suu.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xyr.hnqzz.top

[R36] 并发执行多个任务
来源：http://yhx.shanyushiyangtech.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bly.yueranfly.top

[R37] 把输出赋给变量
来源：http://zkm.zhoulong.xyz

files=$(ls -1)
来源：http://fqa.xylfe.cn

[R38] 管道串联
来源：http://ksd.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://ytg.316326.xyz

[R39] 重定向标准输出与错误
来源：http://frg.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://aki.shangyingyoupin.top

[R40] 追加写日志
来源：http://cvb.hongshengwenyu.top

echo "log" >> out.log
来源：http://nhy.ydjk.org.cn

[R41] 丢弃输出
来源：http://yat.c1oappe.top

cmd >/dev/null 2>&1
来源：http://hky.hywenlv.cn

[R42] 输入重定向
来源：http://ojt.hcnkem.com

wc -l < a.txt
来源：http://mvh.tian-w.cn

[R43] 按名字查找文件
来源：http://igh.sufxvd.cn

find . -name "*.log" -type f
来源：http://syl.birdmap.top

[R44] 按修改时间查找
来源：http://hbm.ppjwa.cn

find . -mtime -7 -type f
来源：http://xud.tian-w.cn

[R45] 批量删除
来源：http://tqr.yfazqb.com

find . -name "*.tmp" -delete
来源：http://vag.jianghu66.top

[R46] 递归替换文件内容
来源：http://qvz.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mgb.chenlongwang.top

[R47] sed 单行替换
来源：http://poc.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://eah.chenzaomai.com

[R48] awk 取指定列
来源：http://agv.hcnkem.com

awk '{print $1, $3}' a.txt
来源：http://wvm.xylfe.cn

[R49] awk 带条件
来源：http://zuf.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oxh.sxryk.cn

[R50] awk 求和
来源：http://vpi.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wfh.yuxming.cn

[R51] 排序去重取前几
来源：http://fcz.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ecq.pycfn.com

[R52] 统计行数
来源：http://suv.sufxvd.cn

wc -l a.txt
来源：http://kpr.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://ylt.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nkx.gotoacloud.top

[R54] 比较两个文件
来源：http://waw.hnqzz.top

diff a.txt b.txt
来源：http://nbv.meibo888.top

[R55] 压缩与解压
来源：http://oqq.birdmap.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://usl.wangdashe.top

[R56] 远程拷贝
来源：http://gax.aizwys.cn

scp file user@host:/path/
来源：http://fly.xuanzx.com

[R57] 远程执行命令
来源：http://xyl.wangdashe.top

ssh user@host 'uptime'
来源：http://nyx.shangyingyoupin.top

[R58] 下载文件
来源：http://ljj.gzhubu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yyy.yongpay.top

[R59] 发 POST JSON
来源：http://qpt.gzhubu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wib.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://ctg.guowangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tpy.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://hbm.svipenyu.cn

df -h;  du -sh *
来源：http://pbo.birdmap.top

[R62] 找最占空间的文件
来源：http://msg.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://baj.yonumen.top

[R63] 内存与进程
来源：http://wze.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://xnk.cheryme.top

[R64] 结束进程
来源：http://cpn.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://ach.0kj1m.cn

[R65] 查看端口占用
来源：http://ufy.zhengqikj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tng.chenjidiqi.icu

[R66] 定时任务
来源：http://qgb.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://snq.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://vun.gotoacloud.top

openssl rand -hex 16
来源：http://nch.wangdashe.top

[R68] 计算文件校验值
来源：http://pay.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://zzj.fehbvm.com

[R69] 生成随机密码
来源：http://ubs.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://mva.jqgfzy.top

[R70] 时间戳与互转
来源：http://lgt.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://vps.mhx1999.top

[R71] 日期格式化
来源：http://wjq.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ijj.aizwys.cn

[R72] 等待端口就绪
来源：http://bsn.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iap.wangdashe.top

[R73] 分割大日志
来源：http://ife.yueranfly.top

split -l 1000 big.log part_
来源：http://acl.yuxming.cn

[R74] 批量重命名
来源：http://wds.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fge.shangyingyoupin.top

[R75] 导出环境变量
来源：http://ccg.vehdjk.com

export PATH="$HOME/bin:$PATH"
来源：http://dwa.jianghu66.top

[R76] 使用临时文件
来源：http://xps.xziqi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xqa.jinqigfzy.top

[R77] 读取用户输入
来源：http://bsr.cqqwz.cn

read -rp "请输入: " ans
来源：http://hzo.dianchejie.cn

[R78] 交互式菜单
来源：http://xlk.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cyh.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://wej.c1oappe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qvi.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://umk.jyoumei.cn

time ./run.sh
来源：http://udy.iojbl.cn

================================================================================
来源：http://gve.dashuyun.cn


<!-- 参考信息 -->