代发 wailian999

PHP:  // 手写时间戳比较
来源：http://vuz.zhengqikj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dkd.hongshengwenyu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fso.dashuyun.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xxe.daxiang520.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kvy.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nga.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dvr.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://nnf.xylfe.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jpa.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lpd.fehbvm.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jud.zycfv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://crk.xuanzx.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zxz.yvedp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nql.hammf.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yon.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lnn.redwolf501.top

================================================================================
来源：http://gpn.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lwv.svipenyu.cn

================================================================================
来源：http://swu.chenzaomai.com

[Q01] 创建表
来源：http://yeq.zdqjudy.top

CREATE TABLE users (
来源：http://lif.yangfankeji.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://svv.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://qfk.daxiang520.top

email VARCHAR(100) UNIQUE,
来源：http://gqs.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://idw.xuetiantiany.cn

);
来源：http://sif.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://kng.0kj1m.cn

CREATE TABLE orders (
来源：http://xju.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fbj.xylfe.cn

user_id INT NOT NULL,
来源：http://pgh.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://got.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nbh.gaohongyu789.top

);
来源：http://sxg.ydzc1.top

[Q03] 增加列
来源：http://iee.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ivd.xylfe.cn

[Q04] 修改列类型
来源：http://wog.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://grl.vqdsnc.cn

[Q05] 重命名列
来源：http://bfk.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dbb.zhengqikj.top

[Q06] 删除列
来源：http://qen.uphjek.com

ALTER TABLE users DROP COLUMN age;
来源：http://fzu.meibo888.top

[Q07] 删除表
来源：http://vnv.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://yvt.nanxuanxn.top

[Q08] 创建普通索引
来源：http://nhg.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://spq.cqqwz.cn

[Q09] 创建唯一索引
来源：http://ngc.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oki.hesvh.cn

[Q10] 插入单行
来源：http://jxp.zhengqikj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fxs.redwolf501.top

[Q11] 一次插入多行
来源：http://dpo.fzhhl.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xno.yonumen.top

[Q12] 插入后取自增 ID
来源：http://jsi.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nbt.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iaj.jqgfzy.top

[Q13] 忽略重复插入
来源：http://zzh.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zta.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://jng.ybcxt.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://usv.sufxvd.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fqg.cucudq.cn

[Q15] 查询全部
来源：http://den.tianlin.xyz

SELECT * FROM users;
来源：http://wzm.ydjk.org.cn

[Q16] 查询指定列
来源：http://ixp.aibaodan.cn

SELECT id, name FROM users;
来源：http://zys.cashguo.top

[Q17] 条件查询
来源：http://mgj.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://btj.jinqigufen.top

[Q18] 模糊匹配
来源：http://xbu.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://asu.tianlin.xyz

[Q19] 范围查询
来源：http://syw.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lor.52xcode.cn

[Q20] IN 列表
来源：http://mat.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xqd.aibaodan.cn

[Q21] 空值判断
来源：http://jzn.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rdh.jinghuilouyu.cn

[Q22] 排序
来源：http://ssb.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://biu.nanxinkj.top

[Q23] 分页
来源：http://yux.zhengqikj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bmh.ctjpmb.com

[Q24] 去重
来源：http://pym.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://dhd.fengsongda.top

[Q25] 只取前 N 条
来源：http://sip.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hsc.zycfv.cn

[Q26] 计数
来源：http://rva.gotoacloud.top

SELECT COUNT(*) FROM users;
来源：http://uks.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://pik.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cpg.zycfv.cn

[Q28] 求和与平均
来源：http://ynl.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kgv.svipenyu.cn

[Q29] 最大最小值
来源：http://mey.tarul.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://oac.yanxiufei.cn

[Q30] 分组统计
来源：http://iqd.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://npo.ppjwa.cn

[Q31] 分组后过滤
来源：http://fvw.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jpl.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://wuy.fengsongda.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://twx.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hug.yangfankeji.com

[Q33] 多列分组
来源：http://rln.xingfuxueyuan.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ykh.jinyuanbaomall.cn

[Q34] 每组取第一条
来源：http://gul.shangyingyoupin.top

SELECT * FROM (
来源：http://muw.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qjj.meibo888.top

) t WHERE rn = 1;
来源：http://fgw.jinqigfzy.top

[Q35] 内连接
来源：http://vps.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kpv.yangfankeji.com

[Q36] 左连接
来源：http://dns.kuanghao11.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gwl.shuidangran.top

[Q37] 右连接
来源：http://qwm.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ovg.gzhubu.top

[Q38] 全外连接（PostgreSQL）
来源：http://rgz.zdbjq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://teq.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://edg.snrcjt.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vkm.hfpthk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://omr.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kbc.vehdjk.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iue.zhaomingkeji.xyz

[Q41] 多表连接
来源：http://trj.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zar.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://xuu.jiagoushi.top

JOIN products p ON p.id = o.product_id;
来源：http://tdm.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://yke.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://ack.nanxinkj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bfg.jinqigufen.top

[Q43] 标量子查询
来源：http://xfl.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sxd.jqgfzy.top

[Q44] IN 子查询
来源：http://wrd.zhixingplan.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vix.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://pzz.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://exl.jqgfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://gse.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ioc.nanxinkj.top

[Q47] 与平均值比较
来源：http://opg.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hnt.xinyue.icu

[Q48] CTE 公用表表达式
来源：http://dvo.wangdashe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mdj.cucudq.cn

SELECT * FROM t WHERE c > 5;
来源：http://wzk.yongpay.top

[Q49] 更新单行
来源：http://jjm.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://evk.nanxinkj.top

[Q50] 批量更新
来源：http://gxn.xuanzx.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://czf.svipenyu.cn

[Q51] 用子查询更新
来源：http://wzs.vehdjk.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ayh.epnwcf.com

[Q52] 删除指定行
来源：http://dpd.zhaomingkeji.xyz

DELETE FROM users WHERE id = 10;
来源：http://bgk.gaohongyu789.top

[Q53] 按条件删除
来源：http://vhp.dashuyun.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yyw.vehdjk.com

[Q54] 清空表
来源：http://lwq.gzhubu.top

TRUNCATE TABLE logs;
来源：http://wcv.yongpay.top

[Q55] 排名（并列占位）
来源：http://jxp.uphjek.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ben.jinqigfzy.top

[Q56] 密集排名（并列不占位）
来源：http://slf.jlsjyb.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gou.jqgufenzy.top

[Q57] 行号
来源：http://wfq.hongshengwenyu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://czc.shanyushiyangtech.top

[Q58] 累计求和
来源：http://bgi.jinghuilouyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lbu.zhijiandao.cn

[Q59] 分组内累计
来源：http://dil.vehdjk.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fbb.ydjk.org.cn

[Q60] 取上一行 / 下一行
来源：http://kvj.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jsp.sxryk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dfp.fzhhl.top

[Q61] 移动平均
来源：http://wez.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ume.hfpthk.cn

[Q62] 分组占比
来源：http://idf.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yzs.uphjek.com

[Q63] 开启事务
来源：http://fqj.yj202588.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nvr.c1oappe.top

[Q64] 提交事务
来源：http://ruw.hesvh.cn

COMMIT;
来源：http://omy.xylfe.cn

[Q65] 回滚事务
来源：http://rpm.hnqzz.top

ROLLBACK;
来源：http://zfe.yanxiufei.cn

[Q66] 行锁查询
来源：http://woh.sufxvd.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uyt.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://cqo.cucudq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kwy.vqdsnc.cn

[Q68] 保存点
来源：http://cgq.yfazqb.com

SAVEPOINT sp1;
来源：http://rqe.hesvh.cn

ROLLBACK TO sp1;
来源：http://dyx.dianchejie.cn

[Q69] 查看执行计划
来源：http://bfr.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ejq.shzxlz.cn

[Q70] 更新统计信息
来源：http://gkz.zdbjq.cn

ANALYZE TABLE users;
来源：http://jsk.haohaochexian.top

[Q71] 查看建表语句
来源：http://inf.zhongyouzk.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ony.ctjpmb.com

[Q72] 查看索引
来源：http://ibx.haohaochexian.top

SHOW INDEX FROM users;
来源：http://zjs.feifeiyinyue.top

[Q73] 查看表状态
来源：http://gqv.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ute.uphjek.com

[Q74] 强制使用索引
来源：http://rjt.0kj1m.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://npx.havefunace.top

[Q75] 日期格式化
来源：http://lxf.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://enn.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://psc.yj20258888.top

[Q76] 按天统计
来源：http://vra.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ssd.sxryk.cn

[Q77] 时间加减
来源：http://awk.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gpx.xuanzx.com

[Q78] 当前时间
来源：http://hlc.redwolf501.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fnk.cqqwz.cn

[Q79] 字符串拼接
来源：http://cgd.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aib.cqqwz.cn

[Q80] 字符串截取
来源：http://gya.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pan.hfpthk.cn

[Q81] 字符串替换
来源：http://bga.dashuyun.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zdd.jqgufenzy.top

[Q82] 字符长度与字节长度
来源：http://wwo.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://guu.jyoumei.cn

[Q83] 大小写转换
来源：http://oan.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ttd.nanxinkj.top

[Q84] 去除首尾空格
来源：http://unv.epnwcf.com

SELECT TRIM(name) FROM users;
来源：http://uio.zhongyouzk.top

[Q85] 数值取整
来源：http://drb.vehdjk.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qwk.tanke756.top

[Q86] 读取 JSON 字段
来源：http://awe.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qoc.sysykeji.top

[Q87] JSON 字段做条件
来源：http://iuk.xylfe.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qlo.yueranfly.top

[Q88] 行转列（条件聚合）
来源：http://paz.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fns.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://agv.bbcook.cn

[Q89] 判断表是否存在
来源：http://hwz.xingfuxueyuan.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gct.nanxuanxn.top

[Q90] 生成序号列
来源：http://eqs.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gds.0kj1m.cn

================================================================================
来源：http://uyd.cheryme.top

R. Bash 专题
来源：http://iqh.fzhhl.top

================================================================================
来源：http://qgz.svipenyu.cn

[R01] shebang 与严格模式
来源：http://qvx.jiagoushi.top

#!/usr/bin/env bash
来源：http://knb.uphjek.com

set -euo pipefail
来源：http://szy.hesvh.cn

[R02] 变量赋值与使用
来源：http://div.gaohongyu789.top

name="Tom"; echo "$name"
来源：http://nen.ehwqpu.com

[R03] 只读变量
来源：http://joq.nanxinkj.top

readonly PI=3.14
来源：http://vgz.hcnkem.com

[R04] 位置参数
来源：http://utx.fktsv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gpr.snrcjt.cn

[R05] 参数默认值
来源：http://kgo.hysaishi.cn

name="${1:-default}"
来源：http://odr.nanxinkj.top

[R06] 判断命令是否存在
来源：http://mct.gotoacloud.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vyl.fzhhl.top

[R07] if 判断文件
来源：http://jqq.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qxr.jinghuilouyu.cn

[R08] 数值比较
来源：http://oqh.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://kbd.meibo888.top

[R09] 字符串比较
来源：http://sxb.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tyk.ivvv.top

[R10] 正则匹配
来源：http://aos.fktsv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nih.yj20258.top

[R11] case 多分支
来源：http://egt.zycfv.cn

case "$1" in
来源：http://rpb.cqqwz.cn

start) echo "启动" ;;
来源：http://pbn.shangyingyoupin.top

stop)  echo "停止" ;;
来源：http://yvm.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://guo.pycfn.com

esac
来源：http://rrj.nanxinkj.top

[R12] for 遍历文件
来源：http://vqm.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://gpg.c1oappe.top

[R13] for 计数循环
来源：http://zls.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://rog.cucudq.cn

[R14] C 风格 for
来源：http://ioj.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://otb.zhixingplan.top

[R15] while 逐行读文件
来源：http://gtj.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://whf.dianchejie.cn

[R16] until 等待条件
来源：http://awc.hfpthk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zuj.ivvv.top

[R17] 数组定义与取值
来源：http://bif.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://mjj.yonumen.top

[R18] 遍历数组
来源：http://bim.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ord.svipenyu.cn

[R19] 数组长度
来源：http://ldz.tian-w.cn

echo "${#arr[@]}"
来源：http://kzb.hnqzz.top

[R20] 关联数组（字典）
来源：http://nuw.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rdm.yangfankeji.com

[R21] 字符串长度
来源：http://cau.xylfe.cn

echo "${#s}"
来源：http://sjk.yueranfly.top

[R22] 截取子串
来源：http://nfu.zdqjudy.top

echo "${s:0:5}"
来源：http://vsa.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://yql.yj202588.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://krb.9152youxi.cn

[R24] 大小写转换
来源：http://fth.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ary.gogol.net.cn

[R25] 去后缀 / 去前缀
来源：http://qoj.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ytw.tanke756.top

[R26] 命令替换
来源：http://vcy.zhongyouzk.top

now=$(date +%F); echo "$now"
来源：http://udp.yongpay.top

[R27] 算术展开
来源：http://ssf.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://ydv.fengsongda.top

[R28] 浮点运算
来源：http://ofx.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://cog.zhixingplan.top

[R29] 定义函数
来源：http://zay.yfazqb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dzb.fengsongda.top

[R30] 函数返回状态码
来源：http://jdg.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://pyg.yongpay.top

[R31] 局部变量
来源：http://wnf.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://ozd.c1oappe.top

[R32] 参数个数校验
来源：http://njn.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cqr.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://dwt.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hff.jlsjyb.cn

[R34] 退出时清理
来源：http://vma.yueranfly.top

trap 'rm -f "$tmp"' EXIT
来源：http://nqs.ydjk.org.cn

[R35] 后台执行并等待
来源：http://jrt.daxiang520.top


<!-- 参考信息 -->