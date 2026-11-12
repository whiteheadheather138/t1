代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bbo.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xsy.cucudq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://woh.zycfv.cn

[P04] 求长度
来源：http://vps.9152youxi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://akq.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vlk.guowangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://odf.haohaochexian.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ahg.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://xfr.uphjek.com

Go:   len(arr);  len(m)
来源：http://qez.aizwys.cn

Ruby: x.length;  x.size
来源：http://emw.9152youxi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bmg.hcnkem.com

[P05] 判断两个对象内容是否相等
来源：http://rlj.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rdt.hysaishi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tar.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yct.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hdo.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xln.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ijp.shzxlz.cn

Ruby: a == b
来源：http://cww.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gez.ybcxt.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pdg.cqqwz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rxz.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://lcz.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yhh.0kj1m.cn

TS:   if (x == null) {}
来源：http://lyt.daxiang520.top

Java: if (x == null || x.isEmpty()) {}
来源：http://csq.tian-w.cn

Go:   if x == nil {}
来源：http://yik.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lyx.fengsongda.top

C#:   if (x is null) {}
来源：http://erv.xziqi.cn

[P07] 防抖与节流
来源：http://lze.yuanzhike.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iym.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://gpy.cdnleiting.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://npy.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://svb.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hsz.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qyc.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://zsi.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://frb.nanxinkj.top

[P08] 处理浮点精度问题
来源：http://vcx.yangfankeji.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://snz.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zyl.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wta.zdqjudy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cvh.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://psr.ivvv.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dfz.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vah.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fpc.hnxiangtu.top

================================================================================
来源：http://cnx.hywenlv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vuz.shangyingyoupin.top

================================================================================
来源：http://rub.zhixingplan.top

[Q01] 创建表
来源：http://tgc.zdqjudy.top

CREATE TABLE users (
来源：http://vso.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rbv.hnqzz.top

name VARCHAR(50) NOT NULL,
来源：http://wwh.wangshuangyany.cn

email VARCHAR(100) UNIQUE,
来源：http://omk.hfpthk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lgj.chenjidiqi.icu

);
来源：http://rtp.ppjwa.cn

[Q02] 创建带外键的表
来源：http://wvr.nanxuanxn.top

CREATE TABLE orders (
来源：http://lpn.hnxiangtu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dfh.nanxinkj.top

user_id INT NOT NULL,
来源：http://vyq.zdbjq.cn

amount DECIMAL(10, 2),
来源：http://gmm.zhongyouzk.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iyo.iojbl.cn

);
来源：http://qhk.sxryk.cn

[Q03] 增加列
来源：http://vyl.shuidangran.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qlr.mhx1999.top

[Q04] 修改列类型
来源：http://dkn.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tmo.svipenyu.cn

[Q05] 重命名列
来源：http://whu.chenjidiqi.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zod.gaohongyu789.top

[Q06] 删除列
来源：http://lxc.yuxming.cn

ALTER TABLE users DROP COLUMN age;
来源：http://axp.c1oappe.top

[Q07] 删除表
来源：http://lbj.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://hvv.guannengcc.top

[Q08] 创建普通索引
来源：http://ybt.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ean.316326.xyz

[Q09] 创建唯一索引
来源：http://gtn.zhijiandao.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rcs.52xcode.cn

[Q10] 插入单行
来源：http://ljx.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bww.vqdsnc.cn

[Q11] 一次插入多行
来源：http://lpt.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ipr.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://jeo.vehdjk.com

INSERT INTO users (name) VALUES ('C');
来源：http://jij.aizwys.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://crs.tian-w.cn

[Q13] 忽略重复插入
来源：http://rsk.ehwqpu.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vuo.xylfe.cn

[Q14] 存在则更新（upsert）
来源：http://hva.yonumen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dzs.yangfankeji.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uwj.jinyuanbaomall.cn

[Q15] 查询全部
来源：http://vqc.316326.xyz

SELECT * FROM users;
来源：http://tde.dianchejie.cn

[Q16] 查询指定列
来源：http://gxc.zhongyouzk.top

SELECT id, name FROM users;
来源：http://nlw.jlsjyb.cn

[Q17] 条件查询
来源：http://agm.yj202588.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://biv.chenjidiqi.icu

[Q18] 模糊匹配
来源：http://imq.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hoz.jianghu66.top

[Q19] 范围查询
来源：http://qji.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lqv.shuidangran.top

[Q20] IN 列表
来源：http://dbn.xziqi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pqx.gogol.net.cn

[Q21] 空值判断
来源：http://syb.vqdsnc.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sdk.ydjk.org.cn

[Q22] 排序
来源：http://lsa.jinyuanbaomall.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vic.wangdashe.top

[Q23] 分页
来源：http://cub.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lmq.yvedp.cn

[Q24] 去重
来源：http://ocj.shuidangran.top

SELECT DISTINCT city FROM users;
来源：http://sni.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://fbs.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dij.gotoacloud.top

[Q26] 计数
来源：http://lqa.zycfv.cn

SELECT COUNT(*) FROM users;
来源：http://tkd.birdmap.top

[Q27] 条件计数
来源：http://rtg.iojbl.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eoj.hesvh.cn

[Q28] 求和与平均
来源：http://nge.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vmo.fengsongda.top

[Q29] 最大最小值
来源：http://spv.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dto.jinqigufen.top

[Q30] 分组统计
来源：http://nci.gogol.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lol.snrcjt.cn

[Q31] 分组后过滤
来源：http://hzk.uphjek.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zbf.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://rdu.mhx1999.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eew.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mjo.aibaodan.cn

[Q33] 多列分组
来源：http://eri.fehbvm.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ogz.yvedp.cn

[Q34] 每组取第一条
来源：http://hgi.hesvh.cn

SELECT * FROM (
来源：http://xgx.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gzj.ybcxt.top

) t WHERE rn = 1;
来源：http://bsa.yonumen.top

[Q35] 内连接
来源：http://jdi.jyoumei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ilf.316326.xyz

[Q36] 左连接
来源：http://kun.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hsg.sufxvd.cn

[Q37] 右连接
来源：http://iau.ybcxt.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://etw.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://tjd.zhixingplan.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ozd.gotoacloud.top

[Q39] 自连接（查上下级）
来源：http://pqg.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://qna.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vza.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mle.yangfankeji.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kml.chenjidiqi.icu

[Q41] 多表连接
来源：http://ssc.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://dlx.fehbvm.com

JOIN users u ON u.id = o.user_id
来源：http://sxk.aizwys.cn

JOIN products p ON p.id = o.product_id;
来源：http://hun.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://cqo.hfpthk.cn

SELECT u.name, o.amount FROM users u
来源：http://zzm.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mdr.tanke756.top

[Q43] 标量子查询
来源：http://pga.cheryme.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hnw.yuxming.cn

[Q44] IN 子查询
来源：http://cxj.ehwqpu.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uzf.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://uex.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://anw.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pqe.hfpthk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vvd.jqgufenzy.top

[Q47] 与平均值比较
来源：http://gch.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ckz.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://dsh.wangshuangyany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qew.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://gzl.nanxinkj.top

[Q49] 更新单行
来源：http://zee.ydjk.org.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://auc.ivvv.top

[Q50] 批量更新
来源：http://myp.xylfe.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rwb.yanxiufei.cn

[Q51] 用子查询更新
来源：http://hho.tarul.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://urm.nwbrower.top

[Q52] 删除指定行
来源：http://qbn.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://rhh.hfpthk.cn

[Q53] 按条件删除
来源：http://kqg.quarkkingdee.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rbk.guannengcc.top

[Q54] 清空表
来源：http://nos.zdbjq.cn

TRUNCATE TABLE logs;
来源：http://uix.cdnleiting.top

[Q55] 排名（并列占位）
来源：http://fdd.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://htr.hammf.cn

[Q56] 密集排名（并列不占位）
来源：http://rpb.feifeiyinyue.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nrl.nwbrower.top

[Q57] 行号
来源：http://lcb.wangdashe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lyz.ehwqpu.com

[Q58] 累计求和
来源：http://qrn.vehdjk.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bsv.cqqwz.cn

[Q59] 分组内累计
来源：http://gsd.bbcook.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xqs.kuanghao11.cn

[Q60] 取上一行 / 下一行
来源：http://dxf.cdnleiting.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zjf.ppjwa.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vfb.mhx1999.top

[Q61] 移动平均
来源：http://rza.bbcook.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zew.xylfe.cn

[Q62] 分组占比
来源：http://tah.xingfuxueyuan.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://are.yanxiufei.cn

[Q63] 开启事务
来源：http://dps.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ygk.jqgfzy.top

[Q64] 提交事务
来源：http://pcs.gzhubu.top

COMMIT;
来源：http://glx.yangfankeji.com

[Q65] 回滚事务
来源：http://qbu.ppjwa.cn

ROLLBACK;
来源：http://kxr.guannengcc.top

[Q66] 行锁查询
来源：http://whp.haohaochexian.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lkz.yj20258888.top

[Q67] 设置隔离级别
来源：http://iti.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rfj.shangyingyoupin.top

[Q68] 保存点
来源：http://atg.sufxvd.cn

SAVEPOINT sp1;
来源：http://zpf.andypj.xyz

ROLLBACK TO sp1;
来源：http://ewj.zhaomingkeji.xyz

[Q69] 查看执行计划
来源：http://mso.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kqd.guannengcc.top

[Q70] 更新统计信息
来源：http://don.sufxvd.cn

ANALYZE TABLE users;
来源：http://wej.hfpthk.cn

[Q71] 查看建表语句
来源：http://bup.yongpay.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://opy.dashuyun.cn

[Q72] 查看索引
来源：http://hqz.birdmap.top

SHOW INDEX FROM users;
来源：http://rrg.bbcook.cn

[Q73] 查看表状态
来源：http://xpo.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kxt.sysykeji.top

[Q74] 强制使用索引
来源：http://ieu.vqdsnc.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jrv.tian-w.cn

[Q75] 日期格式化
来源：http://obd.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qti.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ffu.aizwys.cn

[Q76] 按天统计
来源：http://mri.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rqc.uphjek.com

[Q77] 时间加减
来源：http://gzk.ywan-chungtsiang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ukc.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://ees.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nrp.dianchejie.cn

[Q79] 字符串拼接
来源：http://mkh.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ctc.ehwqpu.com

[Q80] 字符串截取
来源：http://vbt.xingfuxueyuan.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aoo.hammf.cn

[Q81] 字符串替换
来源：http://lej.hcnkem.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ykq.cheryme.top

[Q82] 字符长度与字节长度
来源：http://czz.fengsongda.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rpe.yuxming.cn

[Q83] 大小写转换
来源：http://wck.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tep.sxryk.cn

[Q84] 去除首尾空格
来源：http://gwv.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://bbw.zhijiandao.cn

[Q85] 数值取整
来源：http://qub.sjlbkw.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zhc.hammf.cn

[Q86] 读取 JSON 字段
来源：http://ekx.zhijiandao.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rpa.zhiwuduotai.top

[Q87] JSON 字段做条件
来源：http://tfb.jiagoushi.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eoq.feifeiyinyue.top

[Q88] 行转列（条件聚合）
来源：http://pad.ppjwa.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://twc.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xfr.gogol.net.cn

[Q89] 判断表是否存在
来源：http://whm.daria6918.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mog.tian-w.cn

[Q90] 生成序号列
来源：http://bcr.jiagoushi.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tmf.zhoulong.xyz

================================================================================
来源：http://mzi.cheryme.top

R. Bash 专题
来源：http://bhy.birdmap.top

================================================================================
来源：http://oab.jinyuanbaomall.cn

[R01] shebang 与严格模式
来源：http://kcm.andypj.xyz

#!/usr/bin/env bash
来源：http://rjn.hcnkem.com

set -euo pipefail
来源：http://alz.hysaishi.cn

[R02] 变量赋值与使用
来源：http://vcv.tianlin.xyz

name="Tom"; echo "$name"
来源：http://rji.chenzaomai.com

[R03] 只读变量
来源：http://qva.cqqwz.cn

readonly PI=3.14
来源：http://dao.52xcode.cn

[R04] 位置参数
来源：http://grn.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fvo.nanxuanxn.top

[R05] 参数默认值
来源：http://gtw.shanyushiyangkeji.top

name="${1:-default}"
来源：http://txi.nwbrower.top

[R06] 判断命令是否存在
来源：http://pho.tianlin.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zup.xylfe.cn

[R07] if 判断文件
来源：http://goo.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jvw.ivvv.top

[R08] 数值比较
来源：http://qkb.jqgfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yqp.0kj1m.cn

[R09] 字符串比较
来源：http://cyt.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jqs.vqdsnc.cn

[R10] 正则匹配
来源：http://fut.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jva.smart0.xyz

[R11] case 多分支
来源：http://phx.zdqjudy.top

case "$1" in
来源：http://nzc.hnxiangtu.top

start) echo "启动" ;;
来源：http://uaz.quarkkingdee.top

stop)  echo "停止" ;;
来源：http://izs.fktsv.cn

*)     echo "未知命令" ;;
来源：http://gif.nwbrower.top

esac
来源：http://qbw.tianlin.xyz

[R12] for 遍历文件
来源：http://vxe.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://htp.hywenlv.cn

[R13] for 计数循环
来源：http://faz.shanyushiyangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://mai.wangshuangyany.cn

[R14] C 风格 for
来源：http://nji.xingfuxueyuan.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://urc.guannengcc.top

[R15] while 逐行读文件
来源：http://pat.shanyushiyangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xpc.shzxlz.cn

[R16] until 等待条件
来源：http://sad.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rod.daria6918.cn

[R17] 数组定义与取值
来源：http://zvu.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ppq.52xcode.cn

[R18] 遍历数组
来源：http://asp.ydzc1.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qta.chenzaomai.com

[R19] 数组长度
来源：http://ygr.snrcjt.cn


<!-- 参考信息 -->