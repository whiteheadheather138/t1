代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/gpxauizky.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/gjloglmeo.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/gxynhxopi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.vehdjk.com/Article/details/glndskmpd.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.sjlbkw.cn/Article/details/ghknxobkx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/gstycueqr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gwuznqtdk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.epnwcf.com/Article/details/gxrzhtgbq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.bbcook.cn/Article/details/gtasaaogo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.epnwcf.com/Article/details/gvxcinbwx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fktsv.cn/Article/details/gjzyhkpef.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/gszkfjolm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.bbcook.cn/Article/details/gmkuxsdvn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/gefnqflze.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.yfazqb.com/Article/details/gjqmyukvy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.epnwcf.com/Article/details/gozagxtwl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.yfazqb.com/Article/details/gecmgkwwe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.sjlbkw.cn/Article/details/gmxptykwe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.vehdjk.com/Article/details/gnipoxcyy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.epnwcf.com/Article/details/gwkoownll.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzpizbhxf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.tarul.cn/Article/details/geppneqte.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghlktbtjh.sHtML

[Q01] 创建表
来源：http://blog.fktsv.cn/Article/details/ggwbrogte.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gzitpfdjc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gjzhfndao.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/gewtwziyx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/gaovbjstw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/grujjftic.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gasibeetz.sHtML

[Q02] 创建带外键的表
来源：http://mobile.sjlbkw.cn/Article/details/gnwuzrfrm.sHtML

CREATE TABLE orders (
来源：http://www.m.share.tarul.cn/Article/details/gqiwvrkfg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gkovhsjjk.sHtML

user_id INT NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gajtchmjz.sHtML

amount DECIMAL(10, 2),
来源：http://wap.tarul.cn/Article/details/gtmuwiisi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.epnwcf.com/Article/details/gwpxdewwk.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gabgjtgaj.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/gzfjhharx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fktsv.cn/Article/details/gabwaicbs.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/gevdldsoo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fktsv.cn/Article/details/gmcprdhoj.sHtML

[Q05] 重命名列
来源：http://wap.bbcook.cn/Article/details/gnnuuywau.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.epnwcf.com/Article/details/graicguyk.sHtML

[Q06] 删除列
来源：http://read.share.sjlbkw.cn/Article/details/gupxujhmx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.sjlbkw.cn/Article/details/gsirzwkmt.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gptebkeke.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fktsv.cn/Article/details/glaffhrud.sHtML

[Q08] 创建普通索引
来源：http://3g.sjlbkw.cn/Article/details/genbqxbca.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/gngycdaac.sHtML

[Q09] 创建唯一索引
来源：http://wap.vehdjk.com/Article/details/gnsefbmaw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gpvqkkzsc.sHtML

[Q10] 插入单行
来源：http://m.share.yfazqb.com/Article/details/gxcyjoots.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.vehdjk.com/Article/details/gabmguwtj.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/gdxpogwun.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gcsjninph.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.vehdjk.com/Article/details/gixtvdrdp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.tarul.cn/Article/details/gofmxgoht.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.vehdjk.com/Article/details/gawukukbt.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gjzntcrma.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/ghcmdjiia.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.bbcook.cn/Article/details/grbfjgswq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.tarul.cn/Article/details/grkhyuxuq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.tarul.cn/Article/details/gcxbndhol.sHtML

[Q15] 查询全部
来源：http://read.share.bbcook.cn/Article/details/gbomxrwrk.sHtML

SELECT * FROM users;
来源：http://m.share.bbcook.cn/Article/details/grgquztjg.sHtML

[Q16] 查询指定列
来源：http://3g.epnwcf.com/Article/details/gpzvciomq.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gxpbtaycb.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/gsfifhvxl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.sjlbkw.cn/Article/details/gpozenfvf.sHtML

[Q18] 模糊匹配
来源：http://www.blog.bbcook.cn/Article/details/grukvkkng.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.sjlbkw.cn/Article/details/gudqotazz.sHtML

[Q19] 范围查询
来源：http://baike.tarul.cn/Article/details/gqbwgapwi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.bbcook.cn/Article/details/gcfiqfnhz.sHtML

[Q20] IN 列表
来源：http://baike.tarul.cn/Article/details/geufgwgjn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gxpedwcgq.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gwbhijhih.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.tarul.cn/Article/details/gsprcvmth.sHtML

[Q22] 排序
来源：http://baike.vehdjk.com/Article/details/gejuavduj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.yfazqb.com/Article/details/gxuuedhrk.sHtML

[Q23] 分页
来源：http://blog.tarul.cn/Article/details/gorceuvgd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fktsv.cn/Article/details/gtiuhgkww.sHtML

[Q24] 去重
来源：http://mobile.epnwcf.com/Article/details/glzipjrwf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gfvdvdsgk.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/googcadga.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.tarul.cn/Article/details/gabebacdq.sHtML

[Q26] 计数
来源：http://wap.sjlbkw.cn/Article/details/goaczwbhh.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.epnwcf.com/Article/details/ghlefntij.sHtML

[Q27] 条件计数
来源：http://3g.tarul.cn/Article/details/govyvgyki.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.yfazqb.com/Article/details/gxbhzqkmn.sHtML

[Q28] 求和与平均
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfxsjfdr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gjnuzfuio.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/gmkrscvdh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.epnwcf.com/Article/details/ggeqwevoh.sHtML

[Q30] 分组统计
来源：http://3g.vehdjk.com/Article/details/gycakxxrw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gsdymbxtz.sHtML

[Q31] 分组后过滤
来源：http://3g.yfazqb.com/Article/details/gxysqmqxo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gvgeyqswl.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fktsv.cn/Article/details/gkvbemils.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/grcazbgsa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fktsv.cn/Article/details/gsqvxysil.sHtML

[Q33] 多列分组
来源：http://www.share.yfazqb.com/Article/details/gauzhravl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.bbcook.cn/Article/details/gcatdhoko.sHtML

[Q34] 每组取第一条
来源：http://wap.yfazqb.com/Article/details/givyparaq.sHtML

SELECT * FROM (
来源：http://baike.tarul.cn/Article/details/giqtzhhtc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.bbcook.cn/Article/details/ghkrthdks.sHtML

) t WHERE rn = 1;
来源：http://wap.bbcook.cn/Article/details/gyxtjkwgs.sHtML

[Q35] 内连接
来源：http://blog.tarul.cn/Article/details/gvbjcdxns.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gkosamymn.sHtML

[Q36] 左连接
来源：http://read.share.epnwcf.com/Article/details/gifypbowm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gpzrxygmw.sHtML

[Q37] 右连接
来源：http://read.share.tarul.cn/Article/details/gijkwtcfe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fktsv.cn/Article/details/gorusihwh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.epnwcf.com/Article/details/grajacxdr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.tarul.cn/Article/details/gehfqwsbb.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.epnwcf.com/Article/details/gikwdhurf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.bbcook.cn/Article/details/gkhjqavpr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.epnwcf.com/Article/details/gchmlvcqs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.yfazqb.com/Article/details/gctcypyiw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.vehdjk.com/Article/details/grqdsmkem.sHtML

[Q41] 多表连接
来源：http://baike.tarul.cn/Article/details/gfpkdxcwk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.yfazqb.com/Article/details/gsoncyvqc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.sjlbkw.cn/Article/details/glgalsbgr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fktsv.cn/Article/details/gtgdtwefw.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.sjlbkw.cn/Article/details/gyleslkow.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/goqphwicu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fktsv.cn/Article/details/gsomjnqqb.sHtML

[Q43] 标量子查询
来源：http://wap.bbcook.cn/Article/details/gkgogwaoi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.sjlbkw.cn/Article/details/gdunzsmxi.sHtML

[Q44] IN 子查询
来源：http://read.share.fktsv.cn/Article/details/ggdagkkdt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.yfazqb.com/Article/details/gdogeowpm.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.vehdjk.com/Article/details/gjltrfgxc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwemdjrtx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsvnyrls.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/glhzndnyc.sHtML

[Q47] 与平均值比较
来源：http://read.share.sjlbkw.cn/Article/details/gtswdtyti.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.bbcook.cn/Article/details/gjcywbril.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/gjgeomixe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gtrfveqwr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/gyivfapca.sHtML

[Q49] 更新单行
来源：http://baike.tarul.cn/Article/details/gykxfzyce.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gruujunzk.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/gezatjvoj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.bbcook.cn/Article/details/gllacddnc.sHtML

[Q51] 用子查询更新
来源：http://wap.vehdjk.com/Article/details/gfcxhxugo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.vehdjk.com/Article/details/gvegoownh.sHtML

[Q52] 删除指定行
来源：http://www.share.fktsv.cn/Article/details/gutjiplul.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gtelclkkv.sHtML

[Q53] 按条件删除
来源：http://read.share.vehdjk.com/Article/details/gwxpxqukw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.bbcook.cn/Article/details/gwwjuikko.sHtML

[Q54] 清空表
来源：http://wap.fktsv.cn/Article/details/guizgvlhs.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.epnwcf.com/Article/details/gbulvgubn.sHtML

[Q55] 排名（并列占位）
来源：http://baike.yfazqb.com/Article/details/gdyqmusgt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gopxpuydt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.yfazqb.com/Article/details/gkyntcifn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gpacpwgns.sHtML

[Q57] 行号
来源：http://wap.epnwcf.com/Article/details/gxyqigzef.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/gcmnbzjfv.sHtML

[Q58] 累计求和
来源：http://3g.bbcook.cn/Article/details/gpqatqglk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.yfazqb.com/Article/details/guokxghvz.sHtML

[Q59] 分组内累计
来源：http://wap.epnwcf.com/Article/details/gdxzgpkhw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.tarul.cn/Article/details/gefuyolhc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.vehdjk.com/Article/details/gtukqdoxn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.sjlbkw.cn/Article/details/gnsxglmvu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/geckcgcul.sHtML

[Q61] 移动平均
来源：http://read.share.sjlbkw.cn/Article/details/ggymhepzs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdiozmwj.sHtML

[Q62] 分组占比
来源：http://www.blog.vehdjk.com/Article/details/gkonsoowp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gbiyrfdao.sHtML

[Q63] 开启事务
来源：http://www.blog.yfazqb.com/Article/details/gmgofrddm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.epnwcf.com/Article/details/gdhhgvwie.sHtML

[Q64] 提交事务
来源：http://read.share.bbcook.cn/Article/details/gmkvscpal.sHtML

COMMIT;
来源：http://www.share.bbcook.cn/Article/details/gthgxsntv.sHtML

[Q65] 回滚事务
来源：http://www.blog.sjlbkw.cn/Article/details/gklpnbahy.sHtML

ROLLBACK;
来源：http://blog.sjlbkw.cn/Article/details/gjymifqwy.sHtML

[Q66] 行锁查询
来源：http://baike.bbcook.cn/Article/details/gglzaagnu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.tarul.cn/Article/details/gudjyzsre.sHtML

[Q67] 设置隔离级别
来源：http://mobile.sjlbkw.cn/Article/details/ggqfdqisl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.tarul.cn/Article/details/gkmzsdaca.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/ghdiouqho.sHtML

SAVEPOINT sp1;
来源：http://baike.sjlbkw.cn/Article/details/gquklcnhj.sHtML

ROLLBACK TO sp1;
来源：http://www.share.tarul.cn/Article/details/gvutaenck.sHtML

[Q69] 查看执行计划
来源：http://m.share.tarul.cn/Article/details/gfnrajwqz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.vehdjk.com/Article/details/gnkblnwpc.sHtML

[Q70] 更新统计信息
来源：http://www.share.epnwcf.com/Article/details/gcbnqpumv.sHtML

ANALYZE TABLE users;
来源：http://mobile.vehdjk.com/Article/details/gefthppoq.sHtML

[Q71] 查看建表语句
来源：http://mobile.epnwcf.com/Article/details/goztdjtds.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gcankxeno.sHtML

[Q72] 查看索引
来源：http://3g.tarul.cn/Article/details/gbkpesdrm.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/gtiiokgmm.sHtML

[Q73] 查看表状态
来源：http://blog.yfazqb.com/Article/details/gixgtbfun.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.sjlbkw.cn/Article/details/gouxqzbsl.sHtML

[Q74] 强制使用索引
来源：http://www.share.yfazqb.com/Article/details/grbungoxv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.bbcook.cn/Article/details/ghpwgimdu.sHtML

[Q75] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gxmskuszj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gnnsefqea.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.yfazqb.com/Article/details/gqwldjclf.sHtML

[Q76] 按天统计
来源：http://baike.sjlbkw.cn/Article/details/gspqpodst.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.sjlbkw.cn/Article/details/gaffoicgs.sHtML

[Q77] 时间加减
来源：http://blog.tarul.cn/Article/details/gtgdljwtn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/ggjknpoqh.sHtML

[Q78] 当前时间
来源：http://wap.vehdjk.com/Article/details/gmzyyqxtw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/gsofthjvu.sHtML

[Q79] 字符串拼接
来源：http://3g.sjlbkw.cn/Article/details/gzvahtxqh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.yfazqb.com/Article/details/guhxmjxzh.sHtML

[Q80] 字符串截取
来源：http://wap.fktsv.cn/Article/details/gisxbaewk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gudydnnay.sHtML

[Q81] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gdrpwnzrq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.tarul.cn/Article/details/gvrvpcshp.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.tarul.cn/Article/details/guzjtedar.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gxthxrrqw.sHtML

[Q83] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gsxbaevcz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gbxcrawdw.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgrubwqt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gzwtkkxvz.sHtML

[Q85] 数值取整
来源：http://read.share.yfazqb.com/Article/details/gfnzkuvch.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.tarul.cn/Article/details/gkzeqnmpa.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gncamucxm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.tarul.cn/Article/details/gnwmswldn.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.sjlbkw.cn/Article/details/gjbhnjrrr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.vehdjk.com/Article/details/gfgzbhvmm.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.yfazqb.com/Article/details/gbqzdskwa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.epnwcf.com/Article/details/gbspgsaim.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.tarul.cn/Article/details/gwsotpwfc.sHtML

[Q89] 判断表是否存在
来源：http://wap.fktsv.cn/Article/details/gokefkjti.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.yfazqb.com/Article/details/gsiuyzshm.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/guminudlw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/gdirrucoc.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/glvzqqbgc.sHtML

R. Bash 专题
来源：http://www.share.fktsv.cn/Article/details/gkpuzrfwu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwowqikmf.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fktsv.cn/Article/details/ghhywhxuv.sHtML

#!/usr/bin/env bash
来源：http://m.share.yfazqb.com/Article/details/gpyvmdyna.sHtML

set -euo pipefail
来源：http://read.share.epnwcf.com/Article/details/gdhfppgsu.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.sjlbkw.cn/Article/details/glhujavno.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/gajjruwbw.sHtML

[R03] 只读变量
来源：http://3g.vehdjk.com/Article/details/gvmecwsou.sHtML

readonly PI=3.14
来源：http://www.share.bbcook.cn/Article/details/gffdwtihv.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/gnoguadnk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.bbcook.cn/Article/details/gtiybytld.sHtML

[R05] 参数默认值
来源：http://mobile.sjlbkw.cn/Article/details/gpinhdsjo.sHtML

name="${1:-default}"
来源：http://read.share.epnwcf.com/Article/details/grltgxdwd.sHtML

[R06] 判断命令是否存在
来源：http://baike.yfazqb.com/Article/details/gxfjkeseh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gfrheskoz.sHtML

[R07] if 判断文件
来源：http://baike.yfazqb.com/Article/details/gikgykgyk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.yfazqb.com/Article/details/gqfnwzrie.sHtML

[R08] 数值比较
来源：http://read.share.bbcook.cn/Article/details/gnitttpna.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.bbcook.cn/Article/details/gjekjkwtr.sHtML

[R09] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gjqltutyd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.vehdjk.com/Article/details/gqibeysau.sHtML

[R10] 正则匹配
来源：http://baike.epnwcf.com/Article/details/gumdeqtxr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.yfazqb.com/Article/details/gywggnlwo.sHtML

[R11] case 多分支
来源：http://wap.yfazqb.com/Article/details/gbqjrdtqz.sHtML

case "$1" in
来源：http://mobile.epnwcf.com/Article/details/gexogueos.sHtML

start) echo "启动" ;;
来源：http://baike.yfazqb.com/Article/details/gvypaqxtj.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.epnwcf.com/Article/details/gezqvwzmn.sHtML

*)     echo "未知命令" ;;
来源：http://blog.vehdjk.com/Article/details/gdvsopcjd.sHtML

esac
来源：http://mobile.fktsv.cn/Article/details/gnxiqynkf.sHtML

[R12] for 遍历文件
来源：http://3g.yfazqb.com/Article/details/gywarhssx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.tarul.cn/Article/details/gprgeieto.sHtML

[R13] for 计数循环
来源：http://3g.bbcook.cn/Article/details/ggslutmsd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gvjluuala.sHtML

[R14] C 风格 for
来源：http://wap.sjlbkw.cn/Article/details/glzfzrizf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gdsduhkru.sHtML

[R15] while 逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gimnrdhdq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.bbcook.cn/Article/details/gfshgnpyw.sHtML

[R16] until 等待条件
来源：http://3g.epnwcf.com/Article/details/gxqbuvzsj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gpznjdugk.sHtML

[R17] 数组定义与取值
来源：http://baike.sjlbkw.cn/Article/details/gmnjfvivv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.tarul.cn/Article/details/gariktxxb.sHtML

[R18] 遍历数组
来源：http://baike.epnwcf.com/Article/details/ghoyhfoti.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.bbcook.cn/Article/details/gywgkfrqr.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/ghpxngoym.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/gspfzppzu.sHtML

[R20] 关联数组（字典）
来源：http://3g.fktsv.cn/Article/details/gcnmbpjlj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.epnwcf.com/Article/details/geqcwyclm.sHtML

[R21] 字符串长度
来源：http://wap.yfazqb.com/Article/details/gjlcliunq.sHtML

echo "${#s}"
来源：http://m.share.bbcook.cn/Article/details/gnvmsanbq.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gjzkylfjv.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/gmexwapeq.sHtML

[R23] 字符串替换
来源：http://baike.bbcook.cn/Article/details/gorfqmgfb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fktsv.cn/Article/details/gxqujudfh.sHtML

[R24] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gayidxjcq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fktsv.cn/Article/details/gvcfqtyiu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.vehdjk.com/Article/details/gqapzkcrj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.tarul.cn/Article/details/gilpbewav.sHtML

[R26] 命令替换
来源：http://www.share.fktsv.cn/Article/details/glylbafrn.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.vehdjk.com/Article/details/gdpyqstde.sHtML

[R27] 算术展开
来源：http://www.share.tarul.cn/Article/details/gacszszoh.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.yfazqb.com/Article/details/gvtinwwzs.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/ggnvysdtt.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gtgxkuuuo.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gatuomnah.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/gvrcelnvi.sHtML

[R30] 函数返回状态码
来源：http://wap.vehdjk.com/Article/details/gjhkkofin.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.epnwcf.com/Article/details/gdzrearbv.sHtML

[R31] 局部变量
来源：http://wap.tarul.cn/Article/details/gjejzkjcq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.tarul.cn/Article/details/gwrfldxdz.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gjiofeldv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gfjkzcktq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.sjlbkw.cn/Article/details/gbvqslnkk.sHtML


<!-- 参考信息 -->