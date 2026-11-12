代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ghb.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mmi.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://okc.ydjk.org.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cwu.shzxlz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cxo.tian-w.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kft.zhengqikj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ztw.zhaomingkeji.xyz

[P04] 求长度
来源：http://cbx.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qmf.xuetiantiany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://shb.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cdx.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rtn.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://kqr.zhoulong.xyz

Go:   len(arr);  len(m)
来源：http://cbx.316326.xyz

Ruby: x.length;  x.size
来源：http://jsh.chenzaomai.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://gmp.yuanzhike.top

[P05] 判断两个对象内容是否相等
来源：http://cxe.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://arc.uphjek.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nyw.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mtw.aibaodan.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ump.jinqigufen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ful.bbcook.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jnb.ydjk.org.cn

Ruby: a == b
来源：http://rmk.xuanzx.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ewc.jianghu66.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uxr.wangshuangyany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kxj.vqdsnc.cn

PHP:  if (empty($x)) {}
来源：http://deq.daria6918.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qye.hnqzz.top

TS:   if (x == null) {}
来源：http://ick.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qdj.jinqigfzy.top

Go:   if x == nil {}
来源：http://gap.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pbc.bjfxy.top

C#:   if (x is null) {}
来源：http://hzb.zycfv.cn

[P07] 防抖与节流
来源：http://bfe.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://edp.fktsv.cn

PHP:  // 手写时间戳比较
来源：http://cua.xziqi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lpy.xuanzx.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hxh.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vad.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jfe.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cyd.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iww.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://doj.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mnp.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wtb.yongpay.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pud.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jnd.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iqj.kuanghao11.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pmc.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cmc.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vdn.svipenyu.cn

================================================================================
来源：http://bqe.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zbm.zhoulong.xyz

================================================================================
来源：http://csd.zhijiandao.cn

[Q01] 创建表
来源：http://ivn.c1oappe.top

CREATE TABLE users (
来源：http://wes.jqgufenzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ull.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://jdz.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://tcy.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://okz.cqqwz.cn

);
来源：http://ktu.hysaishi.cn

[Q02] 创建带外键的表
来源：http://tdd.havefunace.top

CREATE TABLE orders (
来源：http://asr.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jnw.xylfe.cn

user_id INT NOT NULL,
来源：http://efd.xingfuxueyuan.xyz

amount DECIMAL(10, 2),
来源：http://mom.zhiwuduotai.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ehe.uphjek.com

);
来源：http://uvd.gotoacloud.top

[Q03] 增加列
来源：http://cxj.xinyue.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hqb.fzhhl.top

[Q04] 修改列类型
来源：http://grl.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wpe.tanke756.top

[Q05] 重命名列
来源：http://jid.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://stu.daxiang520.top

[Q06] 删除列
来源：http://aju.ppjwa.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zus.snrcjt.cn

[Q07] 删除表
来源：http://ifx.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://sse.fehbvm.com

[Q08] 创建普通索引
来源：http://efh.yonumen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xsb.daria6918.cn

[Q09] 创建唯一索引
来源：http://tof.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yip.hysaishi.cn

[Q10] 插入单行
来源：http://wkq.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://smt.zdqjudy.top

[Q11] 一次插入多行
来源：http://isk.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rxg.jianghu66.top

[Q12] 插入后取自增 ID
来源：http://jtp.chenjidiqi.icu

INSERT INTO users (name) VALUES ('C');
来源：http://kte.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jzt.zhiwuduotai.top

[Q13] 忽略重复插入
来源：http://xbf.zycfv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mqc.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://ubc.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lfg.daxiang520.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pui.9152youxi.cn

[Q15] 查询全部
来源：http://bmn.jinqigufen.top

SELECT * FROM users;
来源：http://rlx.jinqigufen.top

[Q16] 查询指定列
来源：http://ufo.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://piv.cdnleiting.top

[Q17] 条件查询
来源：http://zux.pycfn.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://txl.gzhubu.top

[Q18] 模糊匹配
来源：http://rjq.tanke756.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kpf.cdnleiting.top

[Q19] 范围查询
来源：http://svt.hnxiangtu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cok.ydzc1.top

[Q20] IN 列表
来源：http://bmr.fzhhl.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xjt.chenlongwang.top

[Q21] 空值判断
来源：http://oqt.jlsjyb.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://opl.ydjk.org.cn

[Q22] 排序
来源：http://xtx.daria6918.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lqc.nwbrower.top

[Q23] 分页
来源：http://tff.nanxuanxn.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xjz.hysaishi.cn

[Q24] 去重
来源：http://tkh.yongpay.top

SELECT DISTINCT city FROM users;
来源：http://cct.yj202588.top

[Q25] 只取前 N 条
来源：http://mnw.gogol.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zoh.jqgufenzy.top

[Q26] 计数
来源：http://ajy.jianghu66.top

SELECT COUNT(*) FROM users;
来源：http://mqj.zhixingplan.top

[Q27] 条件计数
来源：http://nyx.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wpf.gogol.net.cn

[Q28] 求和与平均
来源：http://okr.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://etw.316326.xyz

[Q29] 最大最小值
来源：http://lir.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yyh.zhijiandao.cn

[Q30] 分组统计
来源：http://xbn.andypj.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://omi.tanke756.top

[Q31] 分组后过滤
来源：http://baz.yonumen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mdx.redwolf501.top

[Q32] 分组拼接字符串
来源：http://qca.wangshuangyany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qsm.sjlbkw.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eok.52xcode.cn

[Q33] 多列分组
来源：http://hey.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://prj.wangshuangyany.cn

[Q34] 每组取第一条
来源：http://enl.52xcode.cn

SELECT * FROM (
来源：http://hhq.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://enn.shanyushiyangkeji.top

) t WHERE rn = 1;
来源：http://imc.cheryme.top

[Q35] 内连接
来源：http://jrn.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uos.fehbvm.com

[Q36] 左连接
来源：http://nxk.smart0.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mrc.jqgfzy.top

[Q37] 右连接
来源：http://cjy.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eeq.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://kgx.guowangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cge.xuanzx.com

[Q39] 自连接（查上下级）
来源：http://ffc.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://una.yuxming.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://png.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://pcn.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dry.zhaomingkeji.xyz

[Q41] 多表连接
来源：http://bwx.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://adk.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://end.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://ges.hcnkem.com

[Q42] 连接条件附加过滤
来源：http://pxh.cqqwz.cn

SELECT u.name, o.amount FROM users u
来源：http://xvl.ehwqpu.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tel.kuanghao11.cn

[Q43] 标量子查询
来源：http://baa.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jck.kuanghao11.cn

[Q44] IN 子查询
来源：http://qgr.redwolf501.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gca.wangdashe.top

[Q45] EXISTS 判断存在
来源：http://yei.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://twn.jinqigufen.top

[Q46] NOT EXISTS 判断不存在
来源：http://myh.sufxvd.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hem.mhx1999.top

[Q47] 与平均值比较
来源：http://bfw.pycfn.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vid.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://ana.chenlongwang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xko.zhaomingkeji.xyz

SELECT * FROM t WHERE c > 5;
来源：http://tve.yj20258888.top

[Q49] 更新单行
来源：http://hqw.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ptw.tarul.cn

[Q50] 批量更新
来源：http://ilk.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gie.jyoumei.cn

[Q51] 用子查询更新
来源：http://skh.9152youxi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rxs.tanke756.top

[Q52] 删除指定行
来源：http://zaw.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://bbf.yj202588.top

[Q53] 按条件删除
来源：http://kyd.xziqi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qbs.hammf.cn

[Q54] 清空表
来源：http://ysu.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://ozr.tian-w.cn

[Q55] 排名（并列占位）
来源：http://zgt.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fsj.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://rax.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uuf.jinqigufen.top

[Q57] 行号
来源：http://yul.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tzn.cheryme.top

[Q58] 累计求和
来源：http://abw.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pgt.yfazqb.com

[Q59] 分组内累计
来源：http://uqe.yfazqb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dat.jianghu66.top

[Q60] 取上一行 / 下一行
来源：http://ani.xuanzx.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pow.yonumen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bqb.jqgfzy.top

[Q61] 移动平均
来源：http://lvj.meibo888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://soa.jlsjyb.cn

[Q62] 分组占比
来源：http://pxa.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://goq.hesvh.cn

[Q63] 开启事务
来源：http://ows.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gbb.yj20258.top

[Q64] 提交事务
来源：http://okn.fanxiaobao.xyz

COMMIT;
来源：http://omv.yangfankeji.com

[Q65] 回滚事务
来源：http://rve.smart0.xyz

ROLLBACK;
来源：http://dyo.redwolf501.top

[Q66] 行锁查询
来源：http://tzk.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qud.zhengqikj.top

[Q67] 设置隔离级别
来源：http://qnz.ehwqpu.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://edh.xuanzx.com

[Q68] 保存点
来源：http://meo.jinqigufen.top

SAVEPOINT sp1;
来源：http://alz.ppjwa.cn

ROLLBACK TO sp1;
来源：http://wpi.nwbrower.top

[Q69] 查看执行计划
来源：http://azl.pengpengdd.cyou

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fge.shzxlz.cn

[Q70] 更新统计信息
来源：http://zri.hfpthk.cn

ANALYZE TABLE users;
来源：http://xrm.fehbvm.com

[Q71] 查看建表语句
来源：http://qwr.yonumen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qdf.hnxiangtu.top

[Q72] 查看索引
来源：http://pke.ehwqpu.com

SHOW INDEX FROM users;
来源：http://mhi.sjlbkw.cn

[Q73] 查看表状态
来源：http://gny.gotoacloud.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fvx.svipenyu.cn

[Q74] 强制使用索引
来源：http://ezu.tarul.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ngg.birdmap.top

[Q75] 日期格式化
来源：http://pdu.zhixingplan.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pau.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aun.ydzc1.top

[Q76] 按天统计
来源：http://kbq.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://onb.hnqzz.top

[Q77] 时间加减
来源：http://jbz.0kj1m.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gyl.sjlbkw.cn

[Q78] 当前时间
来源：http://jgm.cheryme.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://khg.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://bbl.hammf.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qet.tanke756.top

[Q80] 字符串截取
来源：http://byq.nanxinkj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lyh.tian-w.cn

[Q81] 字符串替换
来源：http://lmu.ydzc1.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ohb.jinqigufen.top

[Q82] 字符长度与字节长度
来源：http://ueh.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yhv.yanxiufei.cn

[Q83] 大小写转换
来源：http://tjv.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ivr.c1oappe.top

[Q84] 去除首尾空格
来源：http://vzh.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://jjz.fehbvm.com

[Q85] 数值取整
来源：http://nhg.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vko.zycfv.cn

[Q86] 读取 JSON 字段
来源：http://sho.guowangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aon.jianghu66.top

[Q87] JSON 字段做条件
来源：http://mxg.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jnk.hongshengwenyu.top

[Q88] 行转列（条件聚合）
来源：http://elo.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yre.birdmap.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bir.chenzaomai.com

[Q89] 判断表是否存在
来源：http://rwk.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ibb.quarkkingdee.top

[Q90] 生成序号列
来源：http://seb.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ugm.tarul.cn

================================================================================
来源：http://aza.kuanghao11.cn

R. Bash 专题
来源：http://iiy.tarul.cn

================================================================================
来源：http://iok.yuanzhike.top

[R01] shebang 与严格模式
来源：http://yxu.316326.xyz

#!/usr/bin/env bash
来源：http://ptk.zdbjq.cn

set -euo pipefail
来源：http://dpb.hongshengwenyu.top

[R02] 变量赋值与使用
来源：http://ksf.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://ojp.cashguo.top

[R03] 只读变量
来源：http://flp.ehwqpu.com

readonly PI=3.14
来源：http://idd.xuetiantiany.cn

[R04] 位置参数
来源：http://aqm.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ueo.tanke756.top

[R05] 参数默认值
来源：http://zbg.chenzaomai.com

name="${1:-default}"
来源：http://avl.iojbl.cn

[R06] 判断命令是否存在
来源：http://xbc.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jyz.jiagoushi.top

[R07] if 判断文件
来源：http://hub.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vkg.snrcjt.cn

[R08] 数值比较
来源：http://cuq.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://poj.chenjidiqi.icu

[R09] 字符串比较
来源：http://yls.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wfc.svipenyu.cn

[R10] 正则匹配
来源：http://rco.shzxlz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mih.yangfankeji.com

[R11] case 多分支
来源：http://mzq.sysykeji.top

case "$1" in
来源：http://fxh.bbcook.cn

start) echo "启动" ;;
来源：http://otp.sxryk.cn

stop)  echo "停止" ;;
来源：http://njo.uphjek.com

*)     echo "未知命令" ;;
来源：http://jml.sufxvd.cn

esac
来源：http://npc.fengsongda.top

[R12] for 遍历文件
来源：http://hyn.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://wke.jinqigfzy.top

[R13] for 计数循环
来源：http://esd.zhaomingkeji.xyz

for i in {1..10}; do echo "$i"; done
来源：http://ssw.cqqwz.cn

[R14] C 风格 for
来源：http://uhi.gzhubu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yph.ehwqpu.com

[R15] while 逐行读文件
来源：http://czw.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xbz.haohaochexian.top

[R16] until 等待条件
来源：http://qwz.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hie.vqdsnc.cn

[R17] 数组定义与取值
来源：http://vrz.daxiang520.top


<!-- 参考信息 -->