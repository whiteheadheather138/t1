代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://qty.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cwe.guannengcc.top

[Q13] 忽略重复插入
来源：http://csw.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eoc.feifeiyinyue.top

[Q14] 存在则更新（upsert）
来源：http://xyz.chenjidiqi.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ttz.ctjpmb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kiq.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://icd.cashguo.top

SELECT * FROM users;
来源：http://rco.jianghu66.top

[Q16] 查询指定列
来源：http://ldf.ydjk.org.cn

SELECT id, name FROM users;
来源：http://kdt.iojbl.cn

[Q17] 条件查询
来源：http://otj.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xqi.ctjpmb.com

[Q18] 模糊匹配
来源：http://kxb.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uqm.fanxiaobao.xyz

[Q19] 范围查询
来源：http://pkt.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lfy.shzxlz.cn

[Q20] IN 列表
来源：http://sbg.ydjk.org.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sim.jqgufenzy.top

[Q21] 空值判断
来源：http://qgf.epnwcf.com

SELECT * FROM users WHERE email IS NULL;
来源：http://biy.chenlongwang.top

[Q22] 排序
来源：http://sjx.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lkk.zhijiandao.cn

[Q23] 分页
来源：http://why.jqgufenzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://izt.shanyushiyangtech.top

[Q24] 去重
来源：http://sea.ywan-chungtsiang.top

SELECT DISTINCT city FROM users;
来源：http://vqo.meibo888.top

[Q25] 只取前 N 条
来源：http://djk.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ihd.epnwcf.com

[Q26] 计数
来源：http://xxc.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://abm.zhengqikj.top

[Q27] 条件计数
来源：http://gcc.hammf.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zrt.ivvv.top

[Q28] 求和与平均
来源：http://cau.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://txm.cashguo.top

[Q29] 最大最小值
来源：http://zcs.jinqigufen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ghh.xuetiantiany.cn

[Q30] 分组统计
来源：http://dbb.pengpengdd.cyou

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hng.cucudq.cn

[Q31] 分组后过滤
来源：http://ckz.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://app.sysykeji.top

[Q32] 分组拼接字符串
来源：http://uxv.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wse.hesvh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xex.guannengcc.top

[Q33] 多列分组
来源：http://qkg.xuanzx.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zux.snrcjt.cn

[Q34] 每组取第一条
来源：http://mlv.cdnleiting.top

SELECT * FROM (
来源：http://kdu.bjfxy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fov.fktsv.cn

) t WHERE rn = 1;
来源：http://meg.gogol.net.cn

[Q35] 内连接
来源：http://exo.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eqt.shuidangran.top

[Q36] 左连接
来源：http://mip.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rko.snrcjt.cn

[Q37] 右连接
来源：http://fsj.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ivd.jianghu66.top

[Q38] 全外连接（PostgreSQL）
来源：http://hnz.tian-w.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kxn.sysykeji.top

[Q39] 自连接（查上下级）
来源：http://qbj.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hvy.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yuw.meibo888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dfr.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qcn.gogol.net.cn

[Q41] 多表连接
来源：http://hcm.tianlin.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://lep.aibaodan.cn

JOIN users u ON u.id = o.user_id
来源：http://dyg.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://igi.yuanzhike.top

[Q42] 连接条件附加过滤
来源：http://fib.nanxinkj.top

SELECT u.name, o.amount FROM users u
来源：http://oyh.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pke.aizwys.cn

[Q43] 标量子查询
来源：http://qrz.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ohc.fktsv.cn

[Q44] IN 子查询
来源：http://dqc.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://esd.cucudq.cn

[Q45] EXISTS 判断存在
来源：http://zqi.fanxiaobao.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eua.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://epg.fzhhl.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qra.ivvv.top

[Q47] 与平均值比较
来源：http://zhs.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ufb.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://isj.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fwi.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://akk.sufxvd.cn

[Q49] 更新单行
来源：http://mgf.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zod.pycfn.com

[Q50] 批量更新
来源：http://rri.ppjwa.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bcc.tanke756.top

[Q51] 用子查询更新
来源：http://ofh.sysykeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kpu.shuidangran.top

[Q52] 删除指定行
来源：http://ijv.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://tuu.yvedp.cn

[Q53] 按条件删除
来源：http://ysp.yj20258.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lmg.hongshengwenyu.top

[Q54] 清空表
来源：http://das.hfpthk.cn

TRUNCATE TABLE logs;
来源：http://lsi.yj202588.top

[Q55] 排名（并列占位）
来源：http://jnh.bjfxy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jei.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://hko.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gjc.chenjidiqi.icu

[Q57] 行号
来源：http://tsk.0kj1m.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hxf.nanxinkj.top

[Q58] 累计求和
来源：http://rgw.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sdg.tanke756.top

[Q59] 分组内累计
来源：http://pba.zycfv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://udf.yj20258.top

[Q60] 取上一行 / 下一行
来源：http://gdm.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xjl.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cmb.dianchejie.cn

[Q61] 移动平均
来源：http://wmm.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qxs.haohaochexian.top

[Q62] 分组占比
来源：http://mme.sxryk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://afs.shzxlz.cn

[Q63] 开启事务
来源：http://tkf.yj202588.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aew.pengpengdd.cyou

[Q64] 提交事务
来源：http://ram.meibo888.top

COMMIT;
来源：http://utb.bbcook.cn

[Q65] 回滚事务
来源：http://amg.chenlongwang.top

ROLLBACK;
来源：http://xxj.sjlbkw.cn

[Q66] 行锁查询
来源：http://vax.cqqwz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aru.yj202588.top

[Q67] 设置隔离级别
来源：http://tmd.birdmap.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sjz.zhoulong.xyz

[Q68] 保存点
来源：http://ovt.uphjek.com

SAVEPOINT sp1;
来源：http://xye.quarkkingdee.top

ROLLBACK TO sp1;
来源：http://miv.tianlin.xyz

[Q69] 查看执行计划
来源：http://qrb.uphjek.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eno.fktsv.cn

[Q70] 更新统计信息
来源：http://nbt.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://flb.cashguo.top

[Q71] 查看建表语句
来源：http://qgn.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vud.fktsv.cn

[Q72] 查看索引
来源：http://mqu.nanxuanxn.top

SHOW INDEX FROM users;
来源：http://bkq.smart0.xyz

[Q73] 查看表状态
来源：http://ydh.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jrl.ydzc1.top

[Q74] 强制使用索引
来源：http://mpf.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vek.meibo888.top

[Q75] 日期格式化
来源：http://jqe.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qcr.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cye.nanxinkj.top

[Q76] 按天统计
来源：http://jfq.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://taw.sufxvd.cn

[Q77] 时间加减
来源：http://eto.shangyingyoupin.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ean.xuetiantiany.cn

[Q78] 当前时间
来源：http://gay.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eaq.quarkkingdee.top

[Q79] 字符串拼接
来源：http://qbx.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vrm.ydjk.org.cn

[Q80] 字符串截取
来源：http://mpv.guannengcc.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ske.zdqjudy.top

[Q81] 字符串替换
来源：http://sgi.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fox.yj20258.top

[Q82] 字符长度与字节长度
来源：http://nne.kuanghao11.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kia.gogol.net.cn

[Q83] 大小写转换
来源：http://lkk.c1oappe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qgw.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://dcd.daxiang520.top

SELECT TRIM(name) FROM users;
来源：http://bdw.meibo888.top

[Q85] 数值取整
来源：http://can.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fgh.cashguo.top

[Q86] 读取 JSON 字段
来源：http://ejw.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xfr.epnwcf.com

[Q87] JSON 字段做条件
来源：http://oeq.bjfxy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pbp.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://iai.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cji.hywenlv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gaq.xziqi.cn

[Q89] 判断表是否存在
来源：http://pwj.hfpthk.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mad.jinqigufen.top

[Q90] 生成序号列
来源：http://nqy.daxiang520.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oxh.zhongyouzk.top

================================================================================
来源：http://boh.shuidangran.top

R. Bash 专题
来源：http://qnx.chenjidiqi.icu

================================================================================
来源：http://otc.yj20258888.top

[R01] shebang 与严格模式
来源：http://lfb.yongpay.top

#!/usr/bin/env bash
来源：http://wyv.sufxvd.cn

set -euo pipefail
来源：http://ngb.zhijiandao.cn

[R02] 变量赋值与使用
来源：http://dyw.hesvh.cn

name="Tom"; echo "$name"
来源：http://wep.jinqigfzy.top

[R03] 只读变量
来源：http://wld.aibaodan.cn

readonly PI=3.14
来源：http://afs.shuidangran.top

[R04] 位置参数
来源：http://fot.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nxu.ivvv.top

[R05] 参数默认值
来源：http://mrt.yj20258.top

name="${1:-default}"
来源：http://zkf.ctjpmb.com

[R06] 判断命令是否存在
来源：http://mqd.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://upr.jinqigufen.top

[R07] if 判断文件
来源：http://gua.hnxiangtu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kye.chenzaomai.com

[R08] 数值比较
来源：http://esn.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tzk.sjlbkw.cn

[R09] 字符串比较
来源：http://vea.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vjh.hywenlv.cn

[R10] 正则匹配
来源：http://onq.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cxp.ydzc1.top

[R11] case 多分支
来源：http://txy.kuanghao11.cn

case "$1" in
来源：http://xdd.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://kqb.tianlin.xyz

stop)  echo "停止" ;;
来源：http://bzl.havefunace.top

*)     echo "未知命令" ;;
来源：http://evi.nwbrower.top

esac
来源：http://qfi.yj202588.top

[R12] for 遍历文件
来源：http://ugw.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://yjb.pengpengdd.cyou

[R13] for 计数循环
来源：http://utk.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://kcq.jqgfzy.top

[R14] C 风格 for
来源：http://ypz.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rhw.ybcxt.top

[R15] while 逐行读文件
来源：http://osy.c1oappe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tdh.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://szl.pycfn.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iwz.hnxiangtu.top

[R17] 数组定义与取值
来源：http://ivt.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://dzl.zhijiandao.cn

[R18] 遍历数组
来源：http://vkq.sysykeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nsg.aizwys.cn

[R19] 数组长度
来源：http://tsp.zhiwuduotai.top

echo "${#arr[@]}"
来源：http://rck.snrcjt.cn

[R20] 关联数组（字典）
来源：http://kou.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yes.xingfuxueyuan.xyz

[R21] 字符串长度
来源：http://lkj.xingfuxueyuan.xyz

echo "${#s}"
来源：http://umt.yangfankeji.com

[R22] 截取子串
来源：http://zec.yanxiufei.cn

echo "${s:0:5}"
来源：http://fyb.xuetiantiany.cn

[R23] 字符串替换
来源：http://nsf.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hlj.daxiang520.top

[R24] 大小写转换
来源：http://ahm.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cpi.52xcode.cn

[R25] 去后缀 / 去前缀
来源：http://pfi.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jri.vehdjk.com

[R26] 命令替换
来源：http://kfi.pengpengdd.cyou

now=$(date +%F); echo "$now"
来源：http://qng.chenlongwang.top

[R27] 算术展开
来源：http://dpc.birdmap.top

echo $((1 + 2 * 3))
来源：http://dcq.yuxming.cn

[R28] 浮点运算
来源：http://bzm.fzhhl.top

echo "scale=2; 10/3" | bc
来源：http://rgv.pengpengdd.cyou

[R29] 定义函数
来源：http://ibx.redwolf501.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iaf.316326.xyz

[R30] 函数返回状态码
来源：http://lbi.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://jfr.zhengqikj.top

[R31] 局部变量
来源：http://tek.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://buh.jqgufenzy.top

[R32] 参数个数校验
来源：http://iyv.zhiwuduotai.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ygy.gaohongyu789.top

[R33] 捕获错误并提示行号
来源：http://wkn.yuxming.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ubk.aizwys.cn

[R34] 退出时清理
来源：http://wth.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://vab.gogol.net.cn

[R35] 后台执行并等待
来源：http://vzw.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qdd.9152youxi.cn

[R36] 并发执行多个任务
来源：http://eph.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mbo.cucudq.cn

[R37] 把输出赋给变量
来源：http://pka.fanxiaobao.xyz

files=$(ls -1)
来源：http://huc.shanyushiyangkeji.top

[R38] 管道串联
来源：http://rnl.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://tda.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://ytw.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://cwa.kuanghao11.cn

[R40] 追加写日志
来源：http://nvi.cqqwz.cn

echo "log" >> out.log
来源：http://oey.tarul.cn

[R41] 丢弃输出
来源：http://gyk.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://zro.jinqigfzy.top

[R42] 输入重定向
来源：http://wxp.daxiang520.top

wc -l < a.txt
来源：http://hon.sweek.top

[R43] 按名字查找文件
来源：http://wkr.cqqwz.cn

find . -name "*.log" -type f
来源：http://vqg.shanyushiyangkeji.top

[R44] 按修改时间查找
来源：http://jty.gotoacloud.top

find . -mtime -7 -type f
来源：http://xhx.havefunace.top

[R45] 批量删除
来源：http://lor.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://kdg.hfpthk.cn

[R46] 递归替换文件内容
来源：http://ffp.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bfs.zdqjudy.top

[R47] sed 单行替换
来源：http://nvv.fanxiaobao.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://xnz.redwolf501.top

[R48] awk 取指定列
来源：http://mbf.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://tkg.zhongyouzk.top

[R49] awk 带条件
来源：http://fuc.tanke756.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bjv.sjlbkw.cn

[R50] awk 求和
来源：http://cuc.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://suw.cucudq.cn

[R51] 排序去重取前几
来源：http://jdk.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://bsu.vehdjk.com

[R52] 统计行数
来源：http://dbz.hysaishi.cn

wc -l a.txt
来源：http://jzz.xuanzx.com

[R53] 查看文件头与实时尾
来源：http://wkc.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://atq.fehbvm.com

[R54] 比较两个文件
来源：http://pno.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://ebg.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://uqu.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nqo.vqdsnc.cn

[R56] 远程拷贝
来源：http://meg.yueranfly.top

scp file user@host:/path/
来源：http://iix.guannengcc.top

[R57] 远程执行命令
来源：http://erh.jlsjyb.cn

ssh user@host 'uptime'
来源：http://xpl.tanke756.top

[R58] 下载文件
来源：http://eqv.vqdsnc.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rtw.zdbjq.cn

[R59] 发 POST JSON
来源：http://awk.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mqe.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://yaz.ydjk.org.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://voi.sxryk.cn

[R61] 磁盘占用
来源：http://you.jinghuilouyu.cn


<!-- 参考信息 -->