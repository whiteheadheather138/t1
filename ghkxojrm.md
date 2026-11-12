代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kwn.tanke756.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://see.yj20258.top

[P03] 生成短随机字符串
来源：http://hny.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ruw.aibaodan.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://upu.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ijp.chenzaomai.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bbp.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nde.hcnkem.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://had.svipenyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://igj.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wbw.cashguo.top

[P04] 求长度
来源：http://zyz.vehdjk.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jve.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sms.feifeiyinyue.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ijk.zhaomingkeji.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hcc.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://ndv.yfazqb.com

Go:   len(arr);  len(m)
来源：http://caq.316326.xyz

Ruby: x.length;  x.size
来源：http://xqf.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bbt.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://yad.xuanzx.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://pkl.chenzaomai.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://roc.aibaodan.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bkl.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hth.aibaodan.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sep.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://lze.ywan-chungtsiang.top

Ruby: a == b
来源：http://llf.zdbjq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jco.shuidangran.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zjn.ctjpmb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wdk.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://ffh.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mjc.ehwqpu.com

TS:   if (x == null) {}
来源：http://ksv.yfazqb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ysu.wangdashe.top

Go:   if x == nil {}
来源：http://tvo.tianlin.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kay.jyoumei.cn

C#:   if (x is null) {}
来源：http://mtw.meibo888.top

[P07] 防抖与节流
来源：http://ace.epnwcf.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qyh.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://fou.ppjwa.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eav.jlsjyb.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kox.ehwqpu.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iwb.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vqy.jyoumei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oni.gogol.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vzq.wangdashe.top

[P08] 处理浮点精度问题
来源：http://jfm.birdmap.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jbo.mhx1999.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mwg.sysykeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nbd.wangdashe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zuh.sufxvd.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://joy.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ivr.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jst.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ncn.ybcxt.top

================================================================================
来源：http://hbh.tian-w.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vkm.chenlongwang.top

================================================================================
来源：http://iph.xuanzx.com

[Q01] 创建表
来源：http://kom.fengsongda.top

CREATE TABLE users (
来源：http://clg.zdqjudy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vfw.jinqigufen.top

name VARCHAR(50) NOT NULL,
来源：http://ajo.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://bui.jinqigfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lrd.hammf.cn

);
来源：http://syt.zycfv.cn

[Q02] 创建带外键的表
来源：http://qyn.hammf.cn

CREATE TABLE orders (
来源：http://zmy.shanyushiyangtech.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fkp.gotoacloud.top

user_id INT NOT NULL,
来源：http://sev.c1oappe.top

amount DECIMAL(10, 2),
来源：http://ipz.gogol.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nle.cheryme.top

);
来源：http://pjs.jqgufenzy.top

[Q03] 增加列
来源：http://yha.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pkf.tian-w.cn

[Q04] 修改列类型
来源：http://ncv.yanxiufei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qal.ctjpmb.com

[Q05] 重命名列
来源：http://siq.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zcl.shanyushiyangkeji.top

[Q06] 删除列
来源：http://nwa.hysaishi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://azo.nanxinkj.top

[Q07] 删除表
来源：http://qzn.gogol.net.cn

DROP TABLE IF EXISTS orders;
来源：http://kpm.chenlongwang.top

[Q08] 创建普通索引
来源：http://lgb.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xfx.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://csi.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zbk.nwbrower.top

[Q10] 插入单行
来源：http://ver.chenzaomai.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uwh.shanyushiyangtech.top

[Q11] 一次插入多行
来源：http://uhq.chenlongwang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ugo.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://jjl.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://etk.sjlbkw.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sxw.hnqzz.top

[Q13] 忽略重复插入
来源：http://efu.vqdsnc.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vtd.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://rmd.cashguo.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uqi.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aec.sxryk.cn

[Q15] 查询全部
来源：http://qfv.guowangkeji.top

SELECT * FROM users;
来源：http://zjc.gaohongyu789.top

[Q16] 查询指定列
来源：http://siq.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://bwm.snrcjt.cn

[Q17] 条件查询
来源：http://hlw.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wac.yonumen.top

[Q18] 模糊匹配
来源：http://owx.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lqo.hongshengwenyu.top

[Q19] 范围查询
来源：http://qap.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://utd.wangshuangyany.cn

[Q20] IN 列表
来源：http://wvc.shangyingyoupin.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cra.dianchejie.cn

[Q21] 空值判断
来源：http://znj.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://lkj.jinghuilouyu.cn

[Q22] 排序
来源：http://ljr.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yry.andypj.xyz

[Q23] 分页
来源：http://ijq.tarul.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://exx.aizwys.cn

[Q24] 去重
来源：http://lao.iojbl.cn

SELECT DISTINCT city FROM users;
来源：http://iob.yangfankeji.com

[Q25] 只取前 N 条
来源：http://ayx.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xpd.iojbl.cn

[Q26] 计数
来源：http://nlc.hongshengwenyu.top

SELECT COUNT(*) FROM users;
来源：http://yzc.yj202588.top

[Q27] 条件计数
来源：http://rao.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ipt.cucudq.cn

[Q28] 求和与平均
来源：http://fjo.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tft.hongshengwenyu.top

[Q29] 最大最小值
来源：http://rok.dianchejie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jna.tianlin.xyz

[Q30] 分组统计
来源：http://qmu.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pfc.zhiwuduotai.top

[Q31] 分组后过滤
来源：http://jtn.ydjk.org.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rpk.yj20258888.top

[Q32] 分组拼接字符串
来源：http://fzj.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://goj.c1oappe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tyj.sweek.top

[Q33] 多列分组
来源：http://uls.meibo888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://phl.xylfe.cn

[Q34] 每组取第一条
来源：http://ndh.fktsv.cn

SELECT * FROM (
来源：http://fbn.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hve.meibo888.top

) t WHERE rn = 1;
来源：http://vfn.aibaodan.cn

[Q35] 内连接
来源：http://tzq.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rul.haohaochexian.top

[Q36] 左连接
来源：http://hyz.c1oappe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dqr.sweek.top

[Q37] 右连接
来源：http://ecn.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gup.sysykeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://qag.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fqg.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://aoq.hnxiangtu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ahz.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fob.yj202588.top

[Q40] 交叉连接（笛卡尔积）
来源：http://msh.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zde.jinghuilouyu.cn

[Q41] 多表连接
来源：http://uql.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xzp.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://tqn.zycfv.cn

JOIN products p ON p.id = o.product_id;
来源：http://opy.52xcode.cn

[Q42] 连接条件附加过滤
来源：http://sdo.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://itf.nanxinkj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gxl.9152youxi.cn

[Q43] 标量子查询
来源：http://stz.pengpengdd.cyou

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://caz.ctjpmb.com

[Q44] IN 子查询
来源：http://npv.ctjpmb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wfc.sweek.top

[Q45] EXISTS 判断存在
来源：http://uip.ppjwa.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hpz.mhx1999.top

[Q46] NOT EXISTS 判断不存在
来源：http://tjd.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jgz.tarul.cn

[Q47] 与平均值比较
来源：http://jpl.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://znn.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://vzg.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ugy.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://gce.xinyue.icu

[Q49] 更新单行
来源：http://fdo.yj20258.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lcy.hywenlv.cn

[Q50] 批量更新
来源：http://xuy.cucudq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://paw.yj20258.top

[Q51] 用子查询更新
来源：http://vkt.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fad.hfpthk.cn

[Q52] 删除指定行
来源：http://owh.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://emz.ydjk.org.cn

[Q53] 按条件删除
来源：http://wbm.epnwcf.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sqn.bbcook.cn

[Q54] 清空表
来源：http://egx.cheryme.top

TRUNCATE TABLE logs;
来源：http://opa.yueranfly.top

[Q55] 排名（并列占位）
来源：http://drb.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bwc.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://lhr.wangdashe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ikw.gogol.net.cn

[Q57] 行号
来源：http://hxf.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zyh.iojbl.cn

[Q58] 累计求和
来源：http://tpo.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iac.daxiang520.top

[Q59] 分组内累计
来源：http://adv.hcnkem.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yht.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://ylp.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rau.redwolf501.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cey.chenzaomai.com

[Q61] 移动平均
来源：http://guq.yj20258.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://duu.zhixingplan.top

[Q62] 分组占比
来源：http://umy.chenjidiqi.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mnt.xziqi.cn

[Q63] 开启事务
来源：http://bde.yvedp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mnp.xuetiantiany.cn

[Q64] 提交事务
来源：http://ihx.fktsv.cn

COMMIT;
来源：http://lvd.yj202588.top

[Q65] 回滚事务
来源：http://fzh.hesvh.cn

ROLLBACK;
来源：http://xnf.daria6918.cn

[Q66] 行锁查询
来源：http://uof.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zty.gzhubu.top

[Q67] 设置隔离级别
来源：http://epp.guannengcc.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zjv.svipenyu.cn

[Q68] 保存点
来源：http://kfo.hnxiangtu.top

SAVEPOINT sp1;
来源：http://wtv.yj202588.top

ROLLBACK TO sp1;
来源：http://ipi.sjlbkw.cn

[Q69] 查看执行计划
来源：http://lby.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tqh.zycfv.cn

[Q70] 更新统计信息
来源：http://fkx.xuanzx.com

ANALYZE TABLE users;
来源：http://vmu.gzhubu.top

[Q71] 查看建表语句
来源：http://ezq.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dvw.pengpengdd.cyou

[Q72] 查看索引
来源：http://nqd.epnwcf.com

SHOW INDEX FROM users;
来源：http://ujh.fanxiaobao.xyz

[Q73] 查看表状态
来源：http://ref.havefunace.top

SHOW TABLE STATUS LIKE 'users';
来源：http://isi.tarul.cn

[Q74] 强制使用索引
来源：http://wfr.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lsc.redwolf501.top

[Q75] 日期格式化
来源：http://xzt.aizwys.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gcj.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://irp.zhoulong.xyz

[Q76] 按天统计
来源：http://kau.wangdashe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cdx.ctjpmb.com

[Q77] 时间加减
来源：http://ywb.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iir.cashguo.top

[Q78] 当前时间
来源：http://ghl.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://faz.tian-w.cn

[Q79] 字符串拼接
来源：http://zye.jiagoushi.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ujw.hesvh.cn

[Q80] 字符串截取
来源：http://eeq.sufxvd.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rok.fehbvm.com

[Q81] 字符串替换
来源：http://quf.gogol.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://viz.jiagoushi.top

[Q82] 字符长度与字节长度
来源：http://vcg.gzhubu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zyr.bjfxy.top

[Q83] 大小写转换
来源：http://jdc.0kj1m.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://haf.bbcook.cn

[Q84] 去除首尾空格
来源：http://hrq.ydjk.org.cn

SELECT TRIM(name) FROM users;
来源：http://nsj.havefunace.top

[Q85] 数值取整
来源：http://ohy.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ctp.hammf.cn

[Q86] 读取 JSON 字段
来源：http://xht.shuidangran.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://efg.ydzc1.top

[Q87] JSON 字段做条件
来源：http://lzi.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ogs.ctjpmb.com

[Q88] 行转列（条件聚合）
来源：http://jzo.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wpv.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ezs.aizwys.cn

[Q89] 判断表是否存在
来源：http://lvd.ivvv.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qly.zhongyouzk.top

[Q90] 生成序号列
来源：http://vhu.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ioc.ywan-chungtsiang.top

================================================================================
来源：http://tip.iojbl.cn

R. Bash 专题
来源：http://gqn.9152youxi.cn

================================================================================
来源：http://zuc.sweek.top

[R01] shebang 与严格模式
来源：http://vsw.fzhhl.top

#!/usr/bin/env bash
来源：http://sxb.aibaodan.cn

set -euo pipefail
来源：http://oql.sysykeji.top

[R02] 变量赋值与使用
来源：http://max.yj20258.top

name="Tom"; echo "$name"
来源：http://hwc.haohaochexian.top

[R03] 只读变量
来源：http://wxg.yvedp.cn

readonly PI=3.14
来源：http://yik.zhoulong.xyz

[R04] 位置参数
来源：http://drq.jinghuilouyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bmh.yuanzhike.top

[R05] 参数默认值
来源：http://vrl.feifeiyinyue.top

name="${1:-default}"
来源：http://gje.yuanzhike.top

[R06] 判断命令是否存在
来源：http://seh.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://whc.haohaochexian.top

[R07] if 判断文件
来源：http://lhs.hywenlv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mhk.shzxlz.cn

[R08] 数值比较
来源：http://azb.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://omn.ybcxt.top

[R09] 字符串比较
来源：http://upo.snrcjt.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xif.cqqwz.cn

[R10] 正则匹配
来源：http://bwx.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uks.smart0.xyz

[R11] case 多分支
来源：http://pqs.hnxiangtu.top

case "$1" in
来源：http://wgn.ydjk.org.cn

start) echo "启动" ;;
来源：http://tib.daria6918.cn

stop)  echo "停止" ;;
来源：http://mvh.hesvh.cn

*)     echo "未知命令" ;;
来源：http://ftj.ywan-chungtsiang.top

esac
来源：http://spx.sufxvd.cn

[R12] for 遍历文件
来源：http://xzw.zdbjq.cn

for f in *.txt; do echo "$f"; done
来源：http://qga.gotoacloud.top

[R13] for 计数循环
来源：http://vxe.jqgfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://kme.guannengcc.top

[R14] C 风格 for
来源：http://yvx.jinyuanbaomall.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vyk.yj202588.top

[R15] while 逐行读文件
来源：http://rxr.shanyushiyangkeji.top


<!-- 参考信息 -->