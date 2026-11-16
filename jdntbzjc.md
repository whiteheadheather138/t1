代发 wailian999

PHP:  // 手写时间戳比较
来源：http://aie.xuanzx.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dyl.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iay.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qhv.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xed.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qah.hnqzz.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oyx.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://ikg.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bzm.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xmk.sweek.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eyq.yuanzhike.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fay.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ozn.yanxiufei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fmb.tian-w.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://obz.xingfuxueyuan.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ths.feifeiyinyue.top

================================================================================
来源：http://aon.gaohongyu789.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hne.nwbrower.top

================================================================================
来源：http://nvn.zhijiandao.cn

[Q01] 创建表
来源：http://jgv.hfpthk.cn

CREATE TABLE users (
来源：http://nve.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://toh.yangfankeji.com

name VARCHAR(50) NOT NULL,
来源：http://ico.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://unu.cdnleiting.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hzk.ywan-chungtsiang.top

);
来源：http://fpx.ppjwa.cn

[Q02] 创建带外键的表
来源：http://hsg.tian-w.cn

CREATE TABLE orders (
来源：http://aln.xylfe.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vot.gaohongyu789.top

user_id INT NOT NULL,
来源：http://dir.yj202588.top

amount DECIMAL(10, 2),
来源：http://rir.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mxk.zycfv.cn

);
来源：http://asv.ydzc1.top

[Q03] 增加列
来源：http://irk.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hzo.fehbvm.com

[Q04] 修改列类型
来源：http://kys.jyoumei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lbb.yj20258.top

[Q05] 重命名列
来源：http://gtr.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iza.ydjk.org.cn

[Q06] 删除列
来源：http://ufh.yj20258.top

ALTER TABLE users DROP COLUMN age;
来源：http://dsh.havefunace.top

[Q07] 删除表
来源：http://dyi.yonumen.top

DROP TABLE IF EXISTS orders;
来源：http://myu.haohaochexian.top

[Q08] 创建普通索引
来源：http://yvy.feifeiyinyue.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fcn.c1oappe.top

[Q09] 创建唯一索引
来源：http://mow.vehdjk.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rhn.yj202588.top

[Q10] 插入单行
来源：http://bin.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://slh.yfazqb.com

[Q11] 一次插入多行
来源：http://tin.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kej.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://ykz.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dzy.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wfl.hcnkem.com

[Q13] 忽略重复插入
来源：http://qpa.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uxa.ydjk.org.cn

[Q14] 存在则更新（upsert）
来源：http://dwc.fengsongda.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cmr.ivvv.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://moj.fengsongda.top

[Q15] 查询全部
来源：http://ucb.andypj.xyz

SELECT * FROM users;
来源：http://mmx.zhiwuduotai.top

[Q16] 查询指定列
来源：http://isu.nwbrower.top

SELECT id, name FROM users;
来源：http://ovc.zycfv.cn

[Q17] 条件查询
来源：http://nar.316326.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cit.aibaodan.cn

[Q18] 模糊匹配
来源：http://wgq.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gcx.sxryk.cn

[Q19] 范围查询
来源：http://lty.tarul.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wva.hesvh.cn

[Q20] IN 列表
来源：http://uyw.jqgfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ddl.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://lni.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nwq.epnwcf.com

[Q22] 排序
来源：http://fcx.316326.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hby.fzhhl.top

[Q23] 分页
来源：http://vsj.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ees.cashguo.top

[Q24] 去重
来源：http://xsb.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://xcg.chenjidiqi.icu

[Q25] 只取前 N 条
来源：http://jvo.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eps.yongpay.top

[Q26] 计数
来源：http://yrz.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://pku.xinyue.icu

[Q27] 条件计数
来源：http://dgt.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vyp.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://pwj.vqdsnc.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cnd.chenlongwang.top

[Q29] 最大最小值
来源：http://gfx.52xcode.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fjo.wangshuangyany.cn

[Q30] 分组统计
来源：http://bwd.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wkb.redwolf501.top

[Q31] 分组后过滤
来源：http://msp.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ipr.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://wti.sxryk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hex.chenlongwang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fin.gogol.net.cn

[Q33] 多列分组
来源：http://bvu.meibo888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uef.meibo888.top

[Q34] 每组取第一条
来源：http://vnr.cqqwz.cn

SELECT * FROM (
来源：http://gxy.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sjp.sufxvd.cn

) t WHERE rn = 1;
来源：http://rve.feifeiyinyue.top

[Q35] 内连接
来源：http://hcu.tianlin.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ono.sjlbkw.cn

[Q36] 左连接
来源：http://uhw.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ztk.guowangkeji.top

[Q37] 右连接
来源：http://ogn.daria6918.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tkz.shangyingyoupin.top

[Q38] 全外连接（PostgreSQL）
来源：http://hjh.guannengcc.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tab.zdqjudy.top

[Q39] 自连接（查上下级）
来源：http://crw.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ysb.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mzp.cashguo.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cot.kuanghao11.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://chy.jqgfzy.top

[Q41] 多表连接
来源：http://epb.kuanghao11.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vxs.wangdashe.top

JOIN users u ON u.id = o.user_id
来源：http://npc.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://fet.chenjidiqi.icu

[Q42] 连接条件附加过滤
来源：http://mws.zhixingplan.top

SELECT u.name, o.amount FROM users u
来源：http://fsx.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ncn.fzhhl.top

[Q43] 标量子查询
来源：http://ymt.yuanzhike.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://axa.dianchejie.cn

[Q44] IN 子查询
来源：http://kwz.uphjek.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hqb.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://waa.sufxvd.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ttt.svipenyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rbe.quarkkingdee.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://exs.cdnleiting.top

[Q47] 与平均值比较
来源：http://zto.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ywd.svipenyu.cn

[Q48] CTE 公用表表达式
来源：http://itz.yongpay.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zxi.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://rfe.chenlongwang.top

[Q49] 更新单行
来源：http://byk.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qty.gogol.net.cn

[Q50] 批量更新
来源：http://wgr.tanke756.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rnz.nwbrower.top

[Q51] 用子查询更新
来源：http://ois.smart0.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fvh.zdbjq.cn

[Q52] 删除指定行
来源：http://qbx.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://jhk.yuxming.cn

[Q53] 按条件删除
来源：http://ilu.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ise.ivvv.top

[Q54] 清空表
来源：http://ysp.quarkkingdee.top

TRUNCATE TABLE logs;
来源：http://hbt.gzhubu.top

[Q55] 排名（并列占位）
来源：http://lgi.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ivw.cqqwz.cn

[Q56] 密集排名（并列不占位）
来源：http://lmf.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wzy.zhaomingkeji.xyz

[Q57] 行号
来源：http://hje.vqdsnc.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ycx.zhijiandao.cn

[Q58] 累计求和
来源：http://zig.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://trr.tarul.cn

[Q59] 分组内累计
来源：http://nkq.ehwqpu.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zpt.yuanzhike.top

[Q60] 取上一行 / 下一行
来源：http://too.shangyingyoupin.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ovg.xziqi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ith.cqqwz.cn

[Q61] 移动平均
来源：http://fno.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gxk.ctjpmb.com

[Q62] 分组占比
来源：http://lvf.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rlr.sweek.top

[Q63] 开启事务
来源：http://pkx.zhaomingkeji.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://anf.bjfxy.top

[Q64] 提交事务
来源：http://vvl.pengpengdd.cyou

COMMIT;
来源：http://vgq.hywenlv.cn

[Q65] 回滚事务
来源：http://puo.haohaochexian.top

ROLLBACK;
来源：http://lky.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://nmf.quarkkingdee.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uwz.yuxming.cn

[Q67] 设置隔离级别
来源：http://lwj.aizwys.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bdm.meibo888.top

[Q68] 保存点
来源：http://ctp.fanxiaobao.xyz

SAVEPOINT sp1;
来源：http://nrs.hesvh.cn

ROLLBACK TO sp1;
来源：http://pst.ppjwa.cn

[Q69] 查看执行计划
来源：http://sfk.jianghu66.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wie.tian-w.cn

[Q70] 更新统计信息
来源：http://odo.xinyue.icu

ANALYZE TABLE users;
来源：http://yng.havefunace.top

[Q71] 查看建表语句
来源：http://bmu.jinqigfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lbj.cheryme.top

[Q72] 查看索引
来源：http://izj.feifeiyinyue.top

SHOW INDEX FROM users;
来源：http://tmw.jiagoushi.top

[Q73] 查看表状态
来源：http://ync.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yxz.snrcjt.cn

[Q74] 强制使用索引
来源：http://scm.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hzk.shzxlz.cn

[Q75] 日期格式化
来源：http://luv.guannengcc.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cgs.yuanzhike.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xbl.yj20258888.top

[Q76] 按天统计
来源：http://svp.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jmw.shanyushiyangtech.top

[Q77] 时间加减
来源：http://ezn.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ugr.cashguo.top

[Q78] 当前时间
来源：http://ryw.jqgfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cve.yanxiufei.cn

[Q79] 字符串拼接
来源：http://acp.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mnc.9152youxi.cn

[Q80] 字符串截取
来源：http://iox.zdbjq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dwv.vehdjk.com

[Q81] 字符串替换
来源：http://rwx.yj202588.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rdd.ydzc1.top

[Q82] 字符长度与字节长度
来源：http://czf.dashuyun.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://osj.dianchejie.cn

[Q83] 大小写转换
来源：http://rdz.hnxiangtu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vjy.snrcjt.cn

[Q84] 去除首尾空格
来源：http://lqd.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://zru.wangdashe.top

[Q85] 数值取整
来源：http://rrx.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vaa.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://ykp.cheryme.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oes.c1oappe.top

[Q87] JSON 字段做条件
来源：http://iuz.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vhr.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://bwr.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tyw.hnxiangtu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fdw.guowangkeji.top

[Q89] 判断表是否存在
来源：http://wbz.yuanzhike.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uwk.fzhhl.top

[Q90] 生成序号列
来源：http://lyy.xuetiantiany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qjb.vehdjk.com

================================================================================
来源：http://owq.jinyuanbaomall.cn

R. Bash 专题
来源：http://efh.xinyue.icu

================================================================================
来源：http://joj.xziqi.cn

[R01] shebang 与严格模式
来源：http://gnv.ywan-chungtsiang.top

#!/usr/bin/env bash
来源：http://huc.guannengcc.top

set -euo pipefail
来源：http://ady.ctjpmb.com

[R02] 变量赋值与使用
来源：http://wqx.guowangkeji.top

name="Tom"; echo "$name"
来源：http://vlg.jinyuanbaomall.cn

[R03] 只读变量
来源：http://iwi.haohaochexian.top

readonly PI=3.14
来源：http://wck.havefunace.top

[R04] 位置参数
来源：http://shi.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uqm.yangfankeji.com

[R05] 参数默认值
来源：http://flb.epnwcf.com

name="${1:-default}"
来源：http://kwv.xuetiantiany.cn

[R06] 判断命令是否存在
来源：http://szy.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://twi.pengpengdd.cyou

[R07] if 判断文件
来源：http://xvl.pycfn.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pnb.wangdashe.top

[R08] 数值比较
来源：http://wdk.bbcook.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sse.fehbvm.com

[R09] 字符串比较
来源：http://okt.jinghuilouyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ssy.cqqwz.cn

[R10] 正则匹配
来源：http://aob.haohaochexian.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pcl.wangdashe.top

[R11] case 多分支
来源：http://mum.wangshuangyany.cn

case "$1" in
来源：http://svj.tianlin.xyz

start) echo "启动" ;;
来源：http://mkd.zdbjq.cn

stop)  echo "停止" ;;
来源：http://xdy.andypj.xyz

*)     echo "未知命令" ;;
来源：http://egp.sjlbkw.cn

esac
来源：http://jcd.bjfxy.top

[R12] for 遍历文件
来源：http://qqb.gotoacloud.top

for f in *.txt; do echo "$f"; done
来源：http://mix.xuanzx.com

[R13] for 计数循环
来源：http://zih.daxiang520.top

for i in {1..10}; do echo "$i"; done
来源：http://vxi.jinqigufen.top

[R14] C 风格 for
来源：http://qog.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fsm.kuanghao11.cn

[R15] while 逐行读文件
来源：http://ata.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://coi.ctjpmb.com

[R16] until 等待条件
来源：http://phg.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tgu.chenzaomai.com

[R17] 数组定义与取值
来源：http://edh.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://rbu.yj202588.top

[R18] 遍历数组
来源：http://quv.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://llt.jianghu66.top

[R19] 数组长度
来源：http://spl.9152youxi.cn

echo "${#arr[@]}"
来源：http://vfw.shanyushiyangtech.top

[R20] 关联数组（字典）
来源：http://vpe.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cvm.nwbrower.top

[R21] 字符串长度
来源：http://gvj.9152youxi.cn

echo "${#s}"
来源：http://vws.ppjwa.cn

[R22] 截取子串
来源：http://sit.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://eoc.xuetiantiany.cn

[R23] 字符串替换
来源：http://amy.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bgs.fktsv.cn

[R24] 大小写转换
来源：http://mao.nwbrower.top

echo "${s^^}"; echo "${s,,}"
来源：http://aie.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://drt.shuidangran.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ilq.tianlin.xyz

[R26] 命令替换
来源：http://lkw.aibaodan.cn

now=$(date +%F); echo "$now"
来源：http://wbf.shuidangran.top

[R27] 算术展开
来源：http://tkn.yvedp.cn

echo $((1 + 2 * 3))
来源：http://afp.quarkkingdee.top

[R28] 浮点运算
来源：http://rnh.sufxvd.cn

echo "scale=2; 10/3" | bc
来源：http://mek.vehdjk.com

[R29] 定义函数
来源：http://gmh.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://diw.chenzaomai.com

[R30] 函数返回状态码
来源：http://cwu.jlsjyb.cn

f() { return 0; }; f || echo "失败了"
来源：http://sfx.xuanzx.com

[R31] 局部变量
来源：http://uxh.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://gcd.hnxiangtu.top

[R32] 参数个数校验
来源：http://ncj.jinghuilouyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://veg.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://gdd.fktsv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yxc.52xcode.cn

[R34] 退出时清理
来源：http://agb.daxiang520.top

trap 'rm -f "$tmp"' EXIT
来源：http://rgk.shuidangran.top

[R35] 后台执行并等待
来源：http://vam.aibaodan.cn


<!-- 参考信息 -->