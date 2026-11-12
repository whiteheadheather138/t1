代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://rdy.shuidangran.top

Go:   len(arr);  len(m)
来源：http://jiy.c1oappe.top

Ruby: x.length;  x.size
来源：http://xtp.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zll.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://rlj.zhijiandao.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pdm.ydjk.org.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bms.fehbvm.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://djy.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://odo.cdnleiting.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kyr.yonumen.top

Go:   reflect.DeepEqual(a, b)
来源：http://wzx.zdbjq.cn

Ruby: a == b
来源：http://say.smart0.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lzv.chenzaomai.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tdj.gzhubu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uxs.zhengqikj.top

PHP:  if (empty($x)) {}
来源：http://hxq.pengpengdd.cyou

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://olq.xuetiantiany.cn

TS:   if (x == null) {}
来源：http://rpu.jyoumei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://izq.aizwys.cn

Go:   if x == nil {}
来源：http://ipp.hesvh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lox.0kj1m.cn

C#:   if (x is null) {}
来源：http://oeh.uphjek.com

[P07] 防抖与节流
来源：http://rdm.xinyue.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://utn.hammf.cn

PHP:  // 手写时间戳比较
来源：http://eig.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fxq.gogol.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://azw.daxiang520.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hfr.yanxiufei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bga.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pqq.xinyue.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jvr.yfazqb.com

[P08] 处理浮点精度问题
来源：http://pby.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iwd.yvedp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xkl.cheryme.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qnl.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sdh.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ebx.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dke.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lyt.yj20258.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tyx.yvedp.cn

================================================================================
来源：http://gpt.hnqzz.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iob.birdmap.top

================================================================================
来源：http://big.52xcode.cn

[Q01] 创建表
来源：http://cfq.cqqwz.cn

CREATE TABLE users (
来源：http://izb.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tpd.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://xah.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://aft.hnqzz.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xib.epnwcf.com

);
来源：http://rsu.yvedp.cn

[Q02] 创建带外键的表
来源：http://lpy.wangdashe.top

CREATE TABLE orders (
来源：http://dsj.tian-w.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blz.xuetiantiany.cn

user_id INT NOT NULL,
来源：http://irp.zhixingplan.top

amount DECIMAL(10, 2),
来源：http://djp.zdbjq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hwd.birdmap.top

);
来源：http://jdd.sweek.top

[Q03] 增加列
来源：http://utn.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bwi.yangfankeji.com

[Q04] 修改列类型
来源：http://pjd.ywan-chungtsiang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kwm.ivvv.top

[Q05] 重命名列
来源：http://bib.cdnleiting.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ldd.hesvh.cn

[Q06] 删除列
来源：http://mop.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://mmh.xylfe.cn

[Q07] 删除表
来源：http://qqo.yfazqb.com

DROP TABLE IF EXISTS orders;
来源：http://rew.jinqigfzy.top

[Q08] 创建普通索引
来源：http://dli.havefunace.top

CREATE INDEX idx_users_email ON users(email);
来源：http://plb.aibaodan.cn

[Q09] 创建唯一索引
来源：http://iuf.yanxiufei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://due.hnxiangtu.top

[Q10] 插入单行
来源：http://kfa.hfpthk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fjm.fzhhl.top

[Q11] 一次插入多行
来源：http://dpe.iojbl.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jfd.yueranfly.top

[Q12] 插入后取自增 ID
来源：http://jgn.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://qsv.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://koz.guannengcc.top

[Q13] 忽略重复插入
来源：http://gqs.xylfe.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://okm.uphjek.com

[Q14] 存在则更新（upsert）
来源：http://sly.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ear.yongpay.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ctn.shuidangran.top

[Q15] 查询全部
来源：http://iwl.ctjpmb.com

SELECT * FROM users;
来源：http://tqk.xuanzx.com

[Q16] 查询指定列
来源：http://vcs.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://yzm.yj20258888.top

[Q17] 条件查询
来源：http://paz.zhaomingkeji.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ajf.nanxinkj.top

[Q18] 模糊匹配
来源：http://sno.quarkkingdee.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gih.sxryk.cn

[Q19] 范围查询
来源：http://ozg.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cyc.gaohongyu789.top

[Q20] IN 列表
来源：http://wgx.tanke756.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qyy.nwbrower.top

[Q21] 空值判断
来源：http://ktf.zhoulong.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://hli.xylfe.cn

[Q22] 排序
来源：http://nay.cqqwz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wxy.xinyue.icu

[Q23] 分页
来源：http://orp.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bta.jqgufenzy.top

[Q24] 去重
来源：http://jci.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://kiu.316326.xyz

[Q25] 只取前 N 条
来源：http://nnx.fktsv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://plz.jyoumei.cn

[Q26] 计数
来源：http://cct.yueranfly.top

SELECT COUNT(*) FROM users;
来源：http://mac.zycfv.cn

[Q27] 条件计数
来源：http://mwz.hongshengwenyu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ldm.hysaishi.cn

[Q28] 求和与平均
来源：http://nfv.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uks.cucudq.cn

[Q29] 最大最小值
来源：http://nbw.ctjpmb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://snb.ehwqpu.com

[Q30] 分组统计
来源：http://lvz.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fie.dashuyun.cn

[Q31] 分组后过滤
来源：http://oen.yanxiufei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wqw.cashguo.top

[Q32] 分组拼接字符串
来源：http://tvg.haohaochexian.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mle.yuanzhike.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mbh.gogol.net.cn

[Q33] 多列分组
来源：http://gbh.jqgufenzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cyf.cheryme.top

[Q34] 每组取第一条
来源：http://qwx.zhixingplan.top

SELECT * FROM (
来源：http://xat.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://afx.hongshengwenyu.top

) t WHERE rn = 1;
来源：http://exi.guowangkeji.top

[Q35] 内连接
来源：http://ecc.9152youxi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rlq.fehbvm.com

[Q36] 左连接
来源：http://zzn.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://res.tianlin.xyz

[Q37] 右连接
来源：http://oge.nwbrower.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oan.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://pwp.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://onx.jqgfzy.top

[Q39] 自连接（查上下级）
来源：http://hwy.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://neg.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dbz.zhixingplan.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fcn.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vrx.aibaodan.cn

[Q41] 多表连接
来源：http://eau.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://eii.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://zas.gogol.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://goz.feifeiyinyue.top

[Q42] 连接条件附加过滤
来源：http://jon.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://ujw.hesvh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zmt.quarkkingdee.top

[Q43] 标量子查询
来源：http://qly.shanyushiyangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wfj.shangyingyoupin.top

[Q44] IN 子查询
来源：http://ggj.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ypc.jyoumei.cn

[Q45] EXISTS 判断存在
来源：http://lnz.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://azh.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://spi.vqdsnc.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mes.hysaishi.cn

[Q47] 与平均值比较
来源：http://hqe.havefunace.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xmr.redwolf501.top

[Q48] CTE 公用表表达式
来源：http://ocf.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ndy.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://chu.zhoulong.xyz

[Q49] 更新单行
来源：http://nnk.ctjpmb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://par.jqgufenzy.top

[Q50] 批量更新
来源：http://nul.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ksz.guowangkeji.top

[Q51] 用子查询更新
来源：http://cpf.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mvl.sweek.top

[Q52] 删除指定行
来源：http://icv.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://bzq.iojbl.cn

[Q53] 按条件删除
来源：http://qfk.tarul.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sza.yj20258888.top

[Q54] 清空表
来源：http://mbv.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://hrv.gogol.net.cn

[Q55] 排名（并列占位）
来源：http://aec.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://znf.ybcxt.top

[Q56] 密集排名（并列不占位）
来源：http://lto.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hkx.pengpengdd.cyou

[Q57] 行号
来源：http://ufk.guowangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pua.aibaodan.cn

[Q58] 累计求和
来源：http://fmn.gotoacloud.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xgl.gogol.net.cn

[Q59] 分组内累计
来源：http://nfs.fanxiaobao.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aso.andypj.xyz

[Q60] 取上一行 / 下一行
来源：http://bkl.zdqjudy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yne.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cef.chenzaomai.com

[Q61] 移动平均
来源：http://efn.zhengqikj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://clg.daxiang520.top

[Q62] 分组占比
来源：http://dok.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dox.snrcjt.cn

[Q63] 开启事务
来源：http://nes.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://phs.jlsjyb.cn

[Q64] 提交事务
来源：http://psr.hcnkem.com

COMMIT;
来源：http://bss.nanxuanxn.top

[Q65] 回滚事务
来源：http://zny.xylfe.cn

ROLLBACK;
来源：http://bts.zhoulong.xyz

[Q66] 行锁查询
来源：http://ogv.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rns.nwbrower.top

[Q67] 设置隔离级别
来源：http://buu.guowangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sag.chenjidiqi.icu

[Q68] 保存点
来源：http://mwp.xylfe.cn

SAVEPOINT sp1;
来源：http://wjj.hfpthk.cn

ROLLBACK TO sp1;
来源：http://tey.fehbvm.com

[Q69] 查看执行计划
来源：http://yps.zhijiandao.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eqq.sysykeji.top

[Q70] 更新统计信息
来源：http://uov.sufxvd.cn

ANALYZE TABLE users;
来源：http://vmy.ydzc1.top

[Q71] 查看建表语句
来源：http://ckf.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://knt.hammf.cn

[Q72] 查看索引
来源：http://sho.cdnleiting.top

SHOW INDEX FROM users;
来源：http://rba.haohaochexian.top

[Q73] 查看表状态
来源：http://oor.guannengcc.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ayt.yueranfly.top

[Q74] 强制使用索引
来源：http://tlo.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vxa.quarkkingdee.top

[Q75] 日期格式化
来源：http://ivx.ybcxt.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mzk.yuxming.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cah.zhoulong.xyz

[Q76] 按天统计
来源：http://cxh.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bag.daxiang520.top

[Q77] 时间加减
来源：http://vxl.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://egt.yj202588.top

[Q78] 当前时间
来源：http://blq.zhiwuduotai.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uwt.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://wqe.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pun.mhx1999.top

[Q80] 字符串截取
来源：http://rca.pengpengdd.cyou

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vpg.sysykeji.top

[Q81] 字符串替换
来源：http://rqu.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blt.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://nke.ppjwa.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ivy.zhaomingkeji.xyz

[Q83] 大小写转换
来源：http://nlk.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tyu.shanyushiyangkeji.top

[Q84] 去除首尾空格
来源：http://wub.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://dkl.ivvv.top

[Q85] 数值取整
来源：http://rxe.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jno.zhengqikj.top

[Q86] 读取 JSON 字段
来源：http://eyn.yangfankeji.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gdf.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://pie.zhiwuduotai.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://acm.jlsjyb.cn

[Q88] 行转列（条件聚合）
来源：http://mxb.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bls.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tdz.cheryme.top

[Q89] 判断表是否存在
来源：http://ytx.hnxiangtu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fxh.shzxlz.cn

[Q90] 生成序号列
来源：http://lhs.tian-w.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xlb.aibaodan.cn

================================================================================
来源：http://fum.gzhubu.top

R. Bash 专题
来源：http://xhr.haohaochexian.top

================================================================================
来源：http://ubw.fengsongda.top

[R01] shebang 与严格模式
来源：http://rsp.ydzc1.top

#!/usr/bin/env bash
来源：http://sdb.cashguo.top

set -euo pipefail
来源：http://ryj.havefunace.top

[R02] 变量赋值与使用
来源：http://hpb.dianchejie.cn

name="Tom"; echo "$name"
来源：http://mhf.pycfn.com

[R03] 只读变量
来源：http://tsb.fengsongda.top

readonly PI=3.14
来源：http://hba.daxiang520.top

[R04] 位置参数
来源：http://obl.zdqjudy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lmn.fzhhl.top

[R05] 参数默认值
来源：http://jis.jlsjyb.cn

name="${1:-default}"
来源：http://yvs.haohaochexian.top

[R06] 判断命令是否存在
来源：http://rmt.gogol.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nht.iojbl.cn

[R07] if 判断文件
来源：http://kro.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://txs.vehdjk.com

[R08] 数值比较
来源：http://oka.cheryme.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tey.316326.xyz

[R09] 字符串比较
来源：http://yxh.wangshuangyany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://heu.ppjwa.cn

[R10] 正则匹配
来源：http://rbx.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uji.gzhubu.top

[R11] case 多分支
来源：http://ynt.yangfankeji.com

case "$1" in
来源：http://xzp.quarkkingdee.top

start) echo "启动" ;;
来源：http://kez.smart0.xyz

stop)  echo "停止" ;;
来源：http://sug.sweek.top

*)     echo "未知命令" ;;
来源：http://dtb.yj20258.top

esac
来源：http://wid.nanxinkj.top

[R12] for 遍历文件
来源：http://fkn.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://hlz.dianchejie.cn

[R13] for 计数循环
来源：http://mwz.jyoumei.cn

for i in {1..10}; do echo "$i"; done
来源：http://ivn.meibo888.top

[R14] C 风格 for
来源：http://tjq.jinyuanbaomall.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xvi.0kj1m.cn

[R15] while 逐行读文件
来源：http://igj.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://egp.yonumen.top

[R16] until 等待条件
来源：http://ghw.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://guu.zhaomingkeji.xyz

[R17] 数组定义与取值
来源：http://bwz.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://yfw.shangyingyoupin.top

[R18] 遍历数组
来源：http://lng.bbcook.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nlc.meibo888.top

[R19] 数组长度
来源：http://ppl.cqqwz.cn

echo "${#arr[@]}"
来源：http://kth.epnwcf.com

[R20] 关联数组（字典）
来源：http://zsa.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qcz.gaohongyu789.top

[R21] 字符串长度
来源：http://sjg.vehdjk.com

echo "${#s}"
来源：http://sfd.yuxming.cn

[R22] 截取子串
来源：http://jyc.hywenlv.cn

echo "${s:0:5}"
来源：http://jpz.quarkkingdee.top

[R23] 字符串替换
来源：http://ihj.guowangkeji.top


<!-- 参考信息 -->