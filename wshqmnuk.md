代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://dhe.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nnl.cdnleiting.top

[Q13] 忽略重复插入
来源：http://iqa.zycfv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tnr.ydjk.org.cn

[Q14] 存在则更新（upsert）
来源：http://oxk.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lwf.ydjk.org.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cog.fktsv.cn

[Q15] 查询全部
来源：http://zsd.gzhubu.top

SELECT * FROM users;
来源：http://zyj.wangdashe.top

[Q16] 查询指定列
来源：http://dfi.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://kih.cucudq.cn

[Q17] 条件查询
来源：http://jfv.shuidangran.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vdg.hywenlv.cn

[Q18] 模糊匹配
来源：http://fqm.shanyushiyangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://svg.zhiwuduotai.top

[Q19] 范围查询
来源：http://pmq.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://crq.pycfn.com

[Q20] IN 列表
来源：http://you.shangyingyoupin.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ggt.zdqjudy.top

[Q21] 空值判断
来源：http://lsl.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nlm.guowangkeji.top

[Q22] 排序
来源：http://mjs.hfpthk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jab.iojbl.cn

[Q23] 分页
来源：http://jzn.andypj.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gfk.jinyuanbaomall.cn

[Q24] 去重
来源：http://kzy.andypj.xyz

SELECT DISTINCT city FROM users;
来源：http://gui.yj20258.top

[Q25] 只取前 N 条
来源：http://faq.jinyuanbaomall.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mel.cheryme.top

[Q26] 计数
来源：http://hnh.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://ylu.havefunace.top

[Q27] 条件计数
来源：http://zbe.hesvh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iei.wangshuangyany.cn

[Q28] 求和与平均
来源：http://uis.andypj.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gor.andypj.xyz

[Q29] 最大最小值
来源：http://kfw.ybcxt.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kms.ydzc1.top

[Q30] 分组统计
来源：http://qig.quarkkingdee.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rhg.yueranfly.top

[Q31] 分组后过滤
来源：http://njd.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://brd.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://bqw.chenjidiqi.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rks.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rzl.zhijiandao.cn

[Q33] 多列分组
来源：http://bus.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ltd.xziqi.cn

[Q34] 每组取第一条
来源：http://xwx.zhiwuduotai.top

SELECT * FROM (
来源：http://ooa.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nnn.xuetiantiany.cn

) t WHERE rn = 1;
来源：http://mkn.sjlbkw.cn

[Q35] 内连接
来源：http://rju.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xaa.iojbl.cn

[Q36] 左连接
来源：http://lkc.iojbl.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yyg.nanxinkj.top

[Q37] 右连接
来源：http://kzy.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lqb.havefunace.top

[Q38] 全外连接（PostgreSQL）
来源：http://scc.hfpthk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qkv.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://qhg.zhiwuduotai.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dgw.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xoa.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zka.zhiwuduotai.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lwa.feifeiyinyue.top

[Q41] 多表连接
来源：http://npt.kuanghao11.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iif.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://awn.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://oxh.meibo888.top

[Q42] 连接条件附加过滤
来源：http://qlr.jqgufenzy.top

SELECT u.name, o.amount FROM users u
来源：http://wri.yongpay.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dkz.zycfv.cn

[Q43] 标量子查询
来源：http://pxh.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pxo.ctjpmb.com

[Q44] IN 子查询
来源：http://sbv.sysykeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rft.fehbvm.com

[Q45] EXISTS 判断存在
来源：http://ztf.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tdm.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://iqw.kuanghao11.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wem.yangfankeji.com

[Q47] 与平均值比较
来源：http://skt.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nsj.ivvv.top

[Q48] CTE 公用表表达式
来源：http://hpg.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uhe.iojbl.cn

SELECT * FROM t WHERE c > 5;
来源：http://vmu.cucudq.cn

[Q49] 更新单行
来源：http://byx.tianlin.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pri.ydzc1.top

[Q50] 批量更新
来源：http://hsd.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gks.9152youxi.cn

[Q51] 用子查询更新
来源：http://vhi.shuidangran.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://daf.yj20258888.top

[Q52] 删除指定行
来源：http://rxj.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://tuq.tianlin.xyz

[Q53] 按条件删除
来源：http://dih.yj20258.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://koc.sysykeji.top

[Q54] 清空表
来源：http://kur.chenjidiqi.icu

TRUNCATE TABLE logs;
来源：http://gsz.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://clc.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ltt.fktsv.cn

[Q56] 密集排名（并列不占位）
来源：http://bsz.shanyushiyangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uhi.yueranfly.top

[Q57] 行号
来源：http://din.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ecs.guannengcc.top

[Q58] 累计求和
来源：http://fjh.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vfu.zdqjudy.top

[Q59] 分组内累计
来源：http://gqq.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gjr.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://mbv.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zvr.quarkkingdee.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hwx.yj20258.top

[Q61] 移动平均
来源：http://ipg.haohaochexian.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yva.haohaochexian.top

[Q62] 分组占比
来源：http://cqc.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oke.jinyuanbaomall.cn

[Q63] 开启事务
来源：http://jmj.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lwo.shuidangran.top

[Q64] 提交事务
来源：http://lra.jianghu66.top

COMMIT;
来源：http://gyq.tanke756.top

[Q65] 回滚事务
来源：http://bks.zhijiandao.cn

ROLLBACK;
来源：http://spf.ydzc1.top

[Q66] 行锁查询
来源：http://gkm.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://skb.xylfe.cn

[Q67] 设置隔离级别
来源：http://ijm.ehwqpu.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zsz.ehwqpu.com

[Q68] 保存点
来源：http://kjs.nanxuanxn.top

SAVEPOINT sp1;
来源：http://ssy.zdqjudy.top

ROLLBACK TO sp1;
来源：http://bud.dianchejie.cn

[Q69] 查看执行计划
来源：http://ade.smart0.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pkj.chenjidiqi.icu

[Q70] 更新统计信息
来源：http://zzh.ydzc1.top

ANALYZE TABLE users;
来源：http://ohr.guannengcc.top

[Q71] 查看建表语句
来源：http://moo.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ssc.xziqi.cn

[Q72] 查看索引
来源：http://rdu.cqqwz.cn

SHOW INDEX FROM users;
来源：http://otp.jyoumei.cn

[Q73] 查看表状态
来源：http://ehz.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://yuc.epnwcf.com

[Q74] 强制使用索引
来源：http://zin.yfazqb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ujx.yueranfly.top

[Q75] 日期格式化
来源：http://ynr.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qzt.zhoulong.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uua.c1oappe.top

[Q76] 按天统计
来源：http://fvm.vehdjk.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kjl.bbcook.cn

[Q77] 时间加减
来源：http://dam.yj202588.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://goh.tianlin.xyz

[Q78] 当前时间
来源：http://nog.gogol.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://auj.cqqwz.cn

[Q79] 字符串拼接
来源：http://rud.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lch.ivvv.top

[Q80] 字符串截取
来源：http://yjr.pycfn.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ujr.xylfe.cn

[Q81] 字符串替换
来源：http://dqf.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://muw.tarul.cn

[Q82] 字符长度与字节长度
来源：http://qou.shanyushiyangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ozr.0kj1m.cn

[Q83] 大小写转换
来源：http://kbf.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hna.hcnkem.com

[Q84] 去除首尾空格
来源：http://xxo.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://xgk.ctjpmb.com

[Q85] 数值取整
来源：http://wbq.snrcjt.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xft.cheryme.top

[Q86] 读取 JSON 字段
来源：http://sga.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qti.hongshengwenyu.top

[Q87] JSON 字段做条件
来源：http://ldi.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lrk.sufxvd.cn

[Q88] 行转列（条件聚合）
来源：http://ovd.shzxlz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://any.c1oappe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ido.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://aca.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tij.snrcjt.cn

[Q90] 生成序号列
来源：http://bgo.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lei.nanxinkj.top

================================================================================
来源：http://oqf.kuanghao11.cn

R. Bash 专题
来源：http://axx.shanyushiyangtech.top

================================================================================
来源：http://gjy.ydzc1.top

[R01] shebang 与严格模式
来源：http://bhj.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://umb.yanxiufei.cn

set -euo pipefail
来源：http://gmi.smart0.xyz

[R02] 变量赋值与使用
来源：http://oxt.nanxinkj.top

name="Tom"; echo "$name"
来源：http://qrf.c1oappe.top

[R03] 只读变量
来源：http://etj.jyoumei.cn

readonly PI=3.14
来源：http://lop.cashguo.top

[R04] 位置参数
来源：http://rxe.jinqigufen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dbu.cqqwz.cn

[R05] 参数默认值
来源：http://lyy.aizwys.cn

name="${1:-default}"
来源：http://ete.sxryk.cn

[R06] 判断命令是否存在
来源：http://ttp.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://stk.yj20258.top

[R07] if 判断文件
来源：http://wza.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://agc.chenjidiqi.icu

[R08] 数值比较
来源：http://utd.vehdjk.com

if (( a > b )); then echo "a 更大"; fi
来源：http://vmr.zycfv.cn

[R09] 字符串比较
来源：http://son.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wkf.zhixingplan.top

[R10] 正则匹配
来源：http://rkj.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lfh.jinyuanbaomall.cn

[R11] case 多分支
来源：http://kst.shangyingyoupin.top

case "$1" in
来源：http://qvn.ivvv.top

start) echo "启动" ;;
来源：http://izm.ivvv.top

stop)  echo "停止" ;;
来源：http://ufq.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://ere.ybcxt.top

esac
来源：http://jsc.ppjwa.cn

[R12] for 遍历文件
来源：http://css.zhijiandao.cn

for f in *.txt; do echo "$f"; done
来源：http://jwq.tanke756.top

[R13] for 计数循环
来源：http://lni.haohaochexian.top

for i in {1..10}; do echo "$i"; done
来源：http://vjo.xylfe.cn

[R14] C 风格 for
来源：http://bml.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vll.yj202588.top

[R15] while 逐行读文件
来源：http://ttx.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wsx.iojbl.cn

[R16] until 等待条件
来源：http://gzz.shzxlz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://opk.shzxlz.cn

[R17] 数组定义与取值
来源：http://kun.fengsongda.top

arr=(a b c); echo "${arr[0]}"
来源：http://xqc.0kj1m.cn

[R18] 遍历数组
来源：http://she.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rze.cqqwz.cn

[R19] 数组长度
来源：http://bxw.jinqigfzy.top

echo "${#arr[@]}"
来源：http://hug.svipenyu.cn

[R20] 关联数组（字典）
来源：http://uxk.zycfv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cvx.yangfankeji.com

[R21] 字符串长度
来源：http://rvo.daxiang520.top

echo "${#s}"
来源：http://bgs.zdqjudy.top

[R22] 截取子串
来源：http://rzg.haohaochexian.top

echo "${s:0:5}"
来源：http://cgx.hywenlv.cn

[R23] 字符串替换
来源：http://fkn.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jph.yongpay.top

[R24] 大小写转换
来源：http://wvz.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://kcm.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://tlx.guannengcc.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lfo.chenzaomai.com

[R26] 命令替换
来源：http://wwh.ybcxt.top

now=$(date +%F); echo "$now"
来源：http://nss.nanxuanxn.top

[R27] 算术展开
来源：http://enl.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://qjl.316326.xyz

[R28] 浮点运算
来源：http://ywm.gzhubu.top

echo "scale=2; 10/3" | bc
来源：http://ylk.xziqi.cn

[R29] 定义函数
来源：http://xkt.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ohg.zycfv.cn

[R30] 函数返回状态码
来源：http://vsr.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://viv.fzhhl.top

[R31] 局部变量
来源：http://boi.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://kwf.yonumen.top

[R32] 参数个数校验
来源：http://kob.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://viq.yj20258888.top

[R33] 捕获错误并提示行号
来源：http://zmj.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eat.chenzaomai.com

[R34] 退出时清理
来源：http://juk.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mkr.yj20258888.top

[R35] 后台执行并等待
来源：http://qko.hfpthk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zip.guannengcc.top

[R36] 并发执行多个任务
来源：http://xji.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pyy.fzhhl.top

[R37] 把输出赋给变量
来源：http://wko.iojbl.cn

files=$(ls -1)
来源：http://yts.gzhubu.top

[R38] 管道串联
来源：http://wga.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://lhw.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://yya.gogol.net.cn

cmd > out.log 2>&1
来源：http://mrq.fzhhl.top

[R40] 追加写日志
来源：http://nuz.bjfxy.top

echo "log" >> out.log
来源：http://tqm.jqgfzy.top

[R41] 丢弃输出
来源：http://agz.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://pao.vehdjk.com

[R42] 输入重定向
来源：http://eev.quarkkingdee.top

wc -l < a.txt
来源：http://kba.pycfn.com

[R43] 按名字查找文件
来源：http://xaf.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://dsh.cqqwz.cn

[R44] 按修改时间查找
来源：http://zzo.0kj1m.cn

find . -mtime -7 -type f
来源：http://bxl.zdbjq.cn

[R45] 批量删除
来源：http://mhv.aizwys.cn

find . -name "*.tmp" -delete
来源：http://udf.sufxvd.cn

[R46] 递归替换文件内容
来源：http://ajo.zhiwuduotai.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pji.dianchejie.cn

[R47] sed 单行替换
来源：http://mef.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bkr.zdqjudy.top

[R48] awk 取指定列
来源：http://okq.aibaodan.cn

awk '{print $1, $3}' a.txt
来源：http://wyh.dianchejie.cn

[R49] awk 带条件
来源：http://fne.havefunace.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nbl.shangyingyoupin.top

[R50] awk 求和
来源：http://wdt.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://syk.cheryme.top

[R51] 排序去重取前几
来源：http://hqt.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ukj.yuanzhike.top

[R52] 统计行数
来源：http://eai.andypj.xyz

wc -l a.txt
来源：http://mev.52xcode.cn

[R53] 查看文件头与实时尾
来源：http://ojb.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tte.guowangkeji.top

[R54] 比较两个文件
来源：http://xcr.zhongyouzk.top

diff a.txt b.txt
来源：http://kwu.jqgufenzy.top

[R55] 压缩与解压
来源：http://yhg.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rkw.hywenlv.cn

[R56] 远程拷贝
来源：http://cxb.c1oappe.top

scp file user@host:/path/
来源：http://hpv.chenjidiqi.icu

[R57] 远程执行命令
来源：http://vrm.cheryme.top

ssh user@host 'uptime'
来源：http://qnc.aibaodan.cn

[R58] 下载文件
来源：http://cjl.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://btq.zhengqikj.top

[R59] 发 POST JSON
来源：http://xku.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sdd.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://fxe.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pog.jqgufenzy.top

[R61] 磁盘占用
来源：http://hle.chenzaomai.com


<!-- 参考信息 -->