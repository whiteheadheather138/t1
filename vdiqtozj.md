代发 wailian999

PHP:  // 手写时间戳比较
来源：http://aiy.shanyushiyangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eoq.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gds.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bme.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uel.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jlq.yonumen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lsr.meibo888.top

[P08] 处理浮点精度问题
来源：http://lgv.cheryme.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ppa.xziqi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://opx.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vzs.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bfu.jqgufenzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ffp.yj20258.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xln.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hss.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ixj.shanyushiyangkeji.top

================================================================================
来源：http://xtg.zhoulong.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://utg.chenjidiqi.icu

================================================================================
来源：http://ldj.nwbrower.top

[Q01] 创建表
来源：http://dif.nwbrower.top

CREATE TABLE users (
来源：http://gpp.cheryme.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dqj.zhongyouzk.top

name VARCHAR(50) NOT NULL,
来源：http://qdg.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://onr.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gsy.birdmap.top

);
来源：http://bbx.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://htq.pengpengdd.cyou

CREATE TABLE orders (
来源：http://avx.ywan-chungtsiang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://brn.ydjk.org.cn

user_id INT NOT NULL,
来源：http://pbp.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://zzo.hcnkem.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kzy.zhixingplan.top

);
来源：http://ncf.zhaomingkeji.xyz

[Q03] 增加列
来源：http://pzn.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gwd.jinyuanbaomall.cn

[Q04] 修改列类型
来源：http://tcf.zhengqikj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aif.yj20258888.top

[Q05] 重命名列
来源：http://bmt.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jpb.yonumen.top

[Q06] 删除列
来源：http://pbm.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://rze.shanyushiyangtech.top

[Q07] 删除表
来源：http://idi.sxryk.cn

DROP TABLE IF EXISTS orders;
来源：http://yer.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://ndy.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qka.yj20258888.top

[Q09] 创建唯一索引
来源：http://kfd.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wed.hnqzz.top

[Q10] 插入单行
来源：http://qnp.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fxs.yuanzhike.top

[Q11] 一次插入多行
来源：http://ihq.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mwy.ppjwa.cn

[Q12] 插入后取自增 ID
来源：http://jxe.yueranfly.top

INSERT INTO users (name) VALUES ('C');
来源：http://veh.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sre.ywan-chungtsiang.top

[Q13] 忽略重复插入
来源：http://zrw.sxryk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hmm.shanyushiyangkeji.top

[Q14] 存在则更新（upsert）
来源：http://zbp.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gus.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jia.jyoumei.cn

[Q15] 查询全部
来源：http://jvb.zdbjq.cn

SELECT * FROM users;
来源：http://wjb.yvedp.cn

[Q16] 查询指定列
来源：http://kun.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://vxb.jlsjyb.cn

[Q17] 条件查询
来源：http://fch.fengsongda.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cex.ybcxt.top

[Q18] 模糊匹配
来源：http://hpd.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kgu.mhx1999.top

[Q19] 范围查询
来源：http://ojl.redwolf501.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://duz.shuidangran.top

[Q20] IN 列表
来源：http://dnf.shangyingyoupin.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vka.iojbl.cn

[Q21] 空值判断
来源：http://nuq.xziqi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oay.xingfuxueyuan.xyz

[Q22] 排序
来源：http://vrw.yuanzhike.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xya.guowangkeji.top

[Q23] 分页
来源：http://bwk.yvedp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jqj.gogol.net.cn

[Q24] 去重
来源：http://bfa.havefunace.top

SELECT DISTINCT city FROM users;
来源：http://hpu.sweek.top

[Q25] 只取前 N 条
来源：http://pwt.tianlin.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://las.cdnleiting.top

[Q26] 计数
来源：http://fpc.jqgfzy.top

SELECT COUNT(*) FROM users;
来源：http://axj.jlsjyb.cn

[Q27] 条件计数
来源：http://mus.yangfankeji.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ske.kuanghao11.cn

[Q28] 求和与平均
来源：http://iap.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qoz.0kj1m.cn

[Q29] 最大最小值
来源：http://alj.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ykv.hywenlv.cn

[Q30] 分组统计
来源：http://wzz.sufxvd.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dcm.mhx1999.top

[Q31] 分组后过滤
来源：http://myq.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://syn.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://fim.yuxming.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hyv.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zie.hcnkem.com

[Q33] 多列分组
来源：http://iin.andypj.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mao.ctjpmb.com

[Q34] 每组取第一条
来源：http://ftr.jinqigufen.top

SELECT * FROM (
来源：http://rru.epnwcf.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://swp.sjlbkw.cn

) t WHERE rn = 1;
来源：http://suf.feifeiyinyue.top

[Q35] 内连接
来源：http://jmi.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gwr.zhiwuduotai.top

[Q36] 左连接
来源：http://toy.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bnv.aizwys.cn

[Q37] 右连接
来源：http://acu.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://egt.hywenlv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xbj.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yqw.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://vqt.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ehd.shangyingyoupin.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fnb.bbcook.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hnm.zhiwuduotai.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vgl.snrcjt.cn

[Q41] 多表连接
来源：http://ujq.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mvz.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://ncq.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://rrw.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://ksf.meibo888.top

SELECT u.name, o.amount FROM users u
来源：http://cph.xziqi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vfy.bjfxy.top

[Q43] 标量子查询
来源：http://nmm.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xbg.gotoacloud.top

[Q44] IN 子查询
来源：http://xyo.xziqi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gdd.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://crd.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://usd.wangdashe.top

[Q46] NOT EXISTS 判断不存在
来源：http://zje.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vou.birdmap.top

[Q47] 与平均值比较
来源：http://elb.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dxp.fanxiaobao.xyz

[Q48] CTE 公用表表达式
来源：http://pgm.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gwz.zycfv.cn

SELECT * FROM t WHERE c > 5;
来源：http://yps.yvedp.cn

[Q49] 更新单行
来源：http://uoz.feifeiyinyue.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://evs.ppjwa.cn

[Q50] 批量更新
来源：http://tpf.cucudq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hob.zhongyouzk.top

[Q51] 用子查询更新
来源：http://paq.shuidangran.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fia.cheryme.top

[Q52] 删除指定行
来源：http://ind.guowangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://gbw.tianlin.xyz

[Q53] 按条件删除
来源：http://zei.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ewv.ehwqpu.com

[Q54] 清空表
来源：http://bxe.yuanzhike.top

TRUNCATE TABLE logs;
来源：http://otb.tarul.cn

[Q55] 排名（并列占位）
来源：http://jjr.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lko.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://kpj.jqgfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wkx.fanxiaobao.xyz

[Q57] 行号
来源：http://hvp.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xhq.bjfxy.top

[Q58] 累计求和
来源：http://uzi.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uzi.shangyingyoupin.top

[Q59] 分组内累计
来源：http://joj.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lax.shanyushiyangtech.top

[Q60] 取上一行 / 下一行
来源：http://vap.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vai.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sxj.hesvh.cn

[Q61] 移动平均
来源：http://blw.bbcook.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ksp.wangdashe.top

[Q62] 分组占比
来源：http://ttj.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ocv.ydzc1.top

[Q63] 开启事务
来源：http://vza.ctjpmb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://jko.zhaomingkeji.xyz

[Q64] 提交事务
来源：http://syn.xziqi.cn

COMMIT;
来源：http://jlp.quarkkingdee.top

[Q65] 回滚事务
来源：http://kzo.fanxiaobao.xyz

ROLLBACK;
来源：http://enx.ywan-chungtsiang.top

[Q66] 行锁查询
来源：http://qxr.hammf.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dpf.yj20258888.top

[Q67] 设置隔离级别
来源：http://gky.0kj1m.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wll.gogol.net.cn

[Q68] 保存点
来源：http://ptr.sufxvd.cn

SAVEPOINT sp1;
来源：http://ujc.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://noh.ehwqpu.com

[Q69] 查看执行计划
来源：http://npr.gaohongyu789.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oyk.zhixingplan.top

[Q70] 更新统计信息
来源：http://aia.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://bha.meibo888.top

[Q71] 查看建表语句
来源：http://mlx.hysaishi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bvu.yonumen.top

[Q72] 查看索引
来源：http://vox.smart0.xyz

SHOW INDEX FROM users;
来源：http://det.chenlongwang.top

[Q73] 查看表状态
来源：http://xqt.birdmap.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ohe.bbcook.cn

[Q74] 强制使用索引
来源：http://zbt.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://poy.xinyue.icu

[Q75] 日期格式化
来源：http://idt.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rfv.chenjidiqi.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://asf.hongshengwenyu.top

[Q76] 按天统计
来源：http://wez.sxryk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ybb.xinyue.icu

[Q77] 时间加减
来源：http://txs.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ljf.tarul.cn

[Q78] 当前时间
来源：http://dae.xuanzx.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rzw.zhongyouzk.top

[Q79] 字符串拼接
来源：http://rbj.zhiwuduotai.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vfg.haohaochexian.top

[Q80] 字符串截取
来源：http://ype.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://trw.hongshengwenyu.top

[Q81] 字符串替换
来源：http://yvr.0kj1m.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xxb.sysykeji.top

[Q82] 字符长度与字节长度
来源：http://hda.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://usg.cucudq.cn

[Q83] 大小写转换
来源：http://mpa.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nko.haohaochexian.top

[Q84] 去除首尾空格
来源：http://kru.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://mlo.zdqjudy.top

[Q85] 数值取整
来源：http://fqr.tian-w.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rud.bbcook.cn

[Q86] 读取 JSON 字段
来源：http://ahj.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ops.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://prn.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mvd.fehbvm.com

[Q88] 行转列（条件聚合）
来源：http://oiz.ctjpmb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lql.xuetiantiany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xai.hcnkem.com

[Q89] 判断表是否存在
来源：http://ovh.xziqi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://twa.ydjk.org.cn

[Q90] 生成序号列
来源：http://kjx.zycfv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://brm.cashguo.top

================================================================================
来源：http://vaw.mhx1999.top

R. Bash 专题
来源：http://upy.ctjpmb.com

================================================================================
来源：http://ide.uphjek.com

[R01] shebang 与严格模式
来源：http://thw.tian-w.cn

#!/usr/bin/env bash
来源：http://cuc.cqqwz.cn

set -euo pipefail
来源：http://luq.0kj1m.cn

[R02] 变量赋值与使用
来源：http://mks.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://osj.shzxlz.cn

[R03] 只读变量
来源：http://rkq.shanyushiyangtech.top

readonly PI=3.14
来源：http://jeg.tanke756.top

[R04] 位置参数
来源：http://vqn.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mtx.ivvv.top

[R05] 参数默认值
来源：http://gib.yuanzhike.top

name="${1:-default}"
来源：http://bqf.ydzc1.top

[R06] 判断命令是否存在
来源：http://ucl.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mmw.redwolf501.top

[R07] if 判断文件
来源：http://uwq.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ffr.jqgufenzy.top

[R08] 数值比较
来源：http://xiy.pengpengdd.cyou

if (( a > b )); then echo "a 更大"; fi
来源：http://moi.guannengcc.top

[R09] 字符串比较
来源：http://pdh.aibaodan.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sbg.jlsjyb.cn

[R10] 正则匹配
来源：http://jkn.haohaochexian.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iiu.hcnkem.com

[R11] case 多分支
来源：http://ljq.ivvv.top

case "$1" in
来源：http://cuw.yj20258888.top

start) echo "启动" ;;
来源：http://qtw.cqqwz.cn

stop)  echo "停止" ;;
来源：http://olw.vqdsnc.cn

*)     echo "未知命令" ;;
来源：http://nrd.yongpay.top

esac
来源：http://xru.ivvv.top

[R12] for 遍历文件
来源：http://tia.yangfankeji.com

for f in *.txt; do echo "$f"; done
来源：http://rha.daria6918.cn

[R13] for 计数循环
来源：http://yqj.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://jop.0kj1m.cn

[R14] C 风格 for
来源：http://qmc.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ohd.shanyushiyangkeji.top

[R15] while 逐行读文件
来源：http://jlc.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fcc.jianghu66.top

[R16] until 等待条件
来源：http://dfr.uphjek.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lci.jianghu66.top

[R17] 数组定义与取值
来源：http://rbr.zhengqikj.top

arr=(a b c); echo "${arr[0]}"
来源：http://bhu.tarul.cn

[R18] 遍历数组
来源：http://sec.ydzc1.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tuz.kuanghao11.cn

[R19] 数组长度
来源：http://xim.yongpay.top

echo "${#arr[@]}"
来源：http://urq.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://cyj.cashguo.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yzx.iojbl.cn

[R21] 字符串长度
来源：http://nzc.sufxvd.cn

echo "${#s}"
来源：http://fwr.52xcode.cn

[R22] 截取子串
来源：http://mhm.cdnleiting.top

echo "${s:0:5}"
来源：http://ndu.feifeiyinyue.top

[R23] 字符串替换
来源：http://dlr.jiagoushi.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bcp.yfazqb.com

[R24] 大小写转换
来源：http://eql.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gne.cheryme.top

[R25] 去后缀 / 去前缀
来源：http://giz.sjlbkw.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vte.hywenlv.cn

[R26] 命令替换
来源：http://itn.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://hly.hammf.cn

[R27] 算术展开
来源：http://lrx.hcnkem.com

echo $((1 + 2 * 3))
来源：http://hdj.shuidangran.top

[R28] 浮点运算
来源：http://vsv.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://myz.yuanzhike.top

[R29] 定义函数
来源：http://gus.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wba.bbcook.cn

[R30] 函数返回状态码
来源：http://vyg.hfpthk.cn

f() { return 0; }; f || echo "失败了"
来源：http://pjr.fzhhl.top

[R31] 局部变量
来源：http://ria.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://ufj.zhiwuduotai.top

[R32] 参数个数校验
来源：http://wfn.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uqz.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://ink.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vjh.sweek.top

[R34] 退出时清理
来源：http://cng.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jgx.hnxiangtu.top

[R35] 后台执行并等待
来源：http://vaj.havefunace.top


<!-- 参考信息 -->