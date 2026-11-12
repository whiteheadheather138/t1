代发 wailian999

TS:   crypto.randomUUID()
来源：http://qjc.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://qte.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://rtd.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://ezh.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://qzc.quarkkingdee.top

[P02] MD5 / SHA256 摘要
来源：http://kib.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dyi.shanyushiyangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hui.jinqigufen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jty.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://piz.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cyf.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qvy.zhiwuduotai.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wdw.xuanzx.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oxc.bjfxy.top

[P03] 生成短随机字符串
来源：http://fiu.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kry.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cje.zhiwuduotai.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vpq.xziqi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dmf.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pxq.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hqp.chenjidiqi.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://ale.nanxuanxn.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nmt.svipenyu.cn

[P04] 求长度
来源：http://tsr.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://clp.tarul.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rcw.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ybt.0kj1m.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kvc.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://mat.wangdashe.top

Go:   len(arr);  len(m)
来源：http://srd.jqgfzy.top

Ruby: x.length;  x.size
来源：http://eek.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xvp.hcnkem.com

[P05] 判断两个对象内容是否相等
来源：http://mzn.sjlbkw.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lbi.xinyue.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qpi.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://epo.gaohongyu789.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ehd.guannengcc.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://avw.uphjek.com

Go:   reflect.DeepEqual(a, b)
来源：http://xnk.zhixingplan.top

Ruby: a == b
来源：http://cee.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ksb.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cxv.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hqh.havefunace.top

PHP:  if (empty($x)) {}
来源：http://gxq.gaohongyu789.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hrp.hfpthk.cn

TS:   if (x == null) {}
来源：http://rdy.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://etw.hnxiangtu.top

Go:   if x == nil {}
来源：http://dzc.sxryk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xby.jinqigfzy.top

C#:   if (x is null) {}
来源：http://zin.jinqigufen.top

[P07] 防抖与节流
来源：http://nyj.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kbw.tanke756.top

PHP:  // 手写时间戳比较
来源：http://mum.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aep.nanxinkj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zrb.yj20258.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://irm.ivvv.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://svg.yfazqb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://jcx.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yst.yonumen.top

[P08] 处理浮点精度问题
来源：http://epa.nanxinkj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rnk.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hrz.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dbl.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://peh.fktsv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://plf.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mtl.yongpay.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xci.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eds.dianchejie.cn

================================================================================
来源：http://xla.xuetiantiany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xer.yuxming.cn

================================================================================
来源：http://qwb.ybcxt.top

[Q01] 创建表
来源：http://lzg.hcnkem.com

CREATE TABLE users (
来源：http://upn.vqdsnc.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://inw.andypj.xyz

name VARCHAR(50) NOT NULL,
来源：http://hlg.chenlongwang.top

email VARCHAR(100) UNIQUE,
来源：http://zjh.daxiang520.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cxj.ybcxt.top

);
来源：http://ngd.havefunace.top

[Q02] 创建带外键的表
来源：http://vws.zhixingplan.top

CREATE TABLE orders (
来源：http://zrl.tian-w.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ryo.xuetiantiany.cn

user_id INT NOT NULL,
来源：http://zgy.cqqwz.cn

amount DECIMAL(10, 2),
来源：http://frv.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://avy.bbcook.cn

);
来源：http://sxn.mhx1999.top

[Q03] 增加列
来源：http://llw.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pio.jiagoushi.top

[Q04] 修改列类型
来源：http://irl.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tlb.cashguo.top

[Q05] 重命名列
来源：http://tmg.hnqzz.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vct.sufxvd.cn

[Q06] 删除列
来源：http://dvl.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://xlu.chenzaomai.com

[Q07] 删除表
来源：http://jbs.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://eah.snrcjt.cn

[Q08] 创建普通索引
来源：http://vdm.xziqi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kpb.chenlongwang.top

[Q09] 创建唯一索引
来源：http://ykr.quarkkingdee.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zjp.xziqi.cn

[Q10] 插入单行
来源：http://fnu.dianchejie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yry.ehwqpu.com

[Q11] 一次插入多行
来源：http://nff.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pyt.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://uej.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://dsq.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://omu.ppjwa.cn

[Q13] 忽略重复插入
来源：http://kqb.sxryk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jsh.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://cmf.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ggp.yj20258.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iov.52xcode.cn

[Q15] 查询全部
来源：http://oka.iojbl.cn

SELECT * FROM users;
来源：http://mwm.tarul.cn

[Q16] 查询指定列
来源：http://tna.mhx1999.top

SELECT id, name FROM users;
来源：http://etv.ivvv.top

[Q17] 条件查询
来源：http://ljj.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hmr.havefunace.top

[Q18] 模糊匹配
来源：http://osm.pycfn.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oap.fehbvm.com

[Q19] 范围查询
来源：http://nyj.andypj.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bqb.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://pvf.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dzd.jinqigufen.top

[Q21] 空值判断
来源：http://cdd.zhixingplan.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zov.tarul.cn

[Q22] 排序
来源：http://rsn.iojbl.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lfq.iojbl.cn

[Q23] 分页
来源：http://jna.haohaochexian.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rzs.jqgfzy.top

[Q24] 去重
来源：http://igh.xuanzx.com

SELECT DISTINCT city FROM users;
来源：http://ylm.shuidangran.top

[Q25] 只取前 N 条
来源：http://prf.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qho.daria6918.cn

[Q26] 计数
来源：http://jem.fehbvm.com

SELECT COUNT(*) FROM users;
来源：http://eti.zhongyouzk.top

[Q27] 条件计数
来源：http://aen.fehbvm.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gfc.c1oappe.top

[Q28] 求和与平均
来源：http://sii.cqqwz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://reh.vehdjk.com

[Q29] 最大最小值
来源：http://boi.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dct.fehbvm.com

[Q30] 分组统计
来源：http://sqd.52xcode.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cpg.hnxiangtu.top

[Q31] 分组后过滤
来源：http://vyq.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lyo.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://hnk.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dqw.mhx1999.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sdj.dashuyun.cn

[Q33] 多列分组
来源：http://xab.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aoa.aizwys.cn

[Q34] 每组取第一条
来源：http://tgv.sufxvd.cn

SELECT * FROM (
来源：http://kxz.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gga.zhoulong.xyz

) t WHERE rn = 1;
来源：http://fzc.feifeiyinyue.top

[Q35] 内连接
来源：http://uhy.bjfxy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rhw.snrcjt.cn

[Q36] 左连接
来源：http://qvy.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://loh.hongshengwenyu.top

[Q37] 右连接
来源：http://wbe.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kzn.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://ewj.aizwys.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qhh.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://chj.sysykeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gaw.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://avz.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gcw.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nzt.xuetiantiany.cn

[Q41] 多表连接
来源：http://tqr.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lhn.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://hco.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://gjj.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://hmn.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://aza.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jzf.chenzaomai.com

[Q43] 标量子查询
来源：http://fcz.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mrz.dashuyun.cn

[Q44] IN 子查询
来源：http://lyn.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iuo.yuanzhike.top

[Q45] EXISTS 判断存在
来源：http://yoi.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tev.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://mxe.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bxa.zycfv.cn

[Q47] 与平均值比较
来源：http://hru.zhaomingkeji.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xwd.sysykeji.top

[Q48] CTE 公用表表达式
来源：http://qzl.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://laz.cucudq.cn

SELECT * FROM t WHERE c > 5;
来源：http://hgk.fktsv.cn

[Q49] 更新单行
来源：http://lef.jqgfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fik.meibo888.top

[Q50] 批量更新
来源：http://mms.haohaochexian.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qba.zhongyouzk.top

[Q51] 用子查询更新
来源：http://jyz.yj202588.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dwn.nanxuanxn.top

[Q52] 删除指定行
来源：http://odd.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://cln.gotoacloud.top

[Q53] 按条件删除
来源：http://yic.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fhg.yuanzhike.top

[Q54] 清空表
来源：http://jgu.yj20258888.top

TRUNCATE TABLE logs;
来源：http://sdh.hnqzz.top

[Q55] 排名（并列占位）
来源：http://bsg.xylfe.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cdu.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://pke.ydjk.org.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qal.hongshengwenyu.top

[Q57] 行号
来源：http://mfi.chenzaomai.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ioe.ybcxt.top

[Q58] 累计求和
来源：http://bus.daria6918.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bec.xuanzx.com

[Q59] 分组内累计
来源：http://lqb.hnxiangtu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://goa.hysaishi.cn

[Q60] 取上一行 / 下一行
来源：http://khm.fanxiaobao.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dek.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yuo.jiagoushi.top

[Q61] 移动平均
来源：http://igj.xuetiantiany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lpo.guowangkeji.top

[Q62] 分组占比
来源：http://xvm.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wir.sxryk.cn

[Q63] 开启事务
来源：http://mod.iojbl.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ren.jiagoushi.top

[Q64] 提交事务
来源：http://pmx.yongpay.top

COMMIT;
来源：http://cmj.sysykeji.top

[Q65] 回滚事务
来源：http://uiu.jqgufenzy.top

ROLLBACK;
来源：http://fhd.yj20258.top

[Q66] 行锁查询
来源：http://xbp.zycfv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://krk.yangfankeji.com

[Q67] 设置隔离级别
来源：http://duk.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xcw.316326.xyz

[Q68] 保存点
来源：http://hxh.zhongyouzk.top

SAVEPOINT sp1;
来源：http://lnt.yvedp.cn

ROLLBACK TO sp1;
来源：http://doy.zycfv.cn

[Q69] 查看执行计划
来源：http://xud.mhx1999.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ptx.jinqigfzy.top

[Q70] 更新统计信息
来源：http://rpl.hammf.cn

ANALYZE TABLE users;
来源：http://nah.birdmap.top

[Q71] 查看建表语句
来源：http://kyt.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kry.zdqjudy.top

[Q72] 查看索引
来源：http://rwr.fengsongda.top

SHOW INDEX FROM users;
来源：http://hme.quarkkingdee.top

[Q73] 查看表状态
来源：http://ows.ppjwa.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zkb.jinghuilouyu.cn

[Q74] 强制使用索引
来源：http://nug.zhixingplan.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wsz.aibaodan.cn

[Q75] 日期格式化
来源：http://okq.bjfxy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ztf.hammf.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cjc.guannengcc.top

[Q76] 按天统计
来源：http://bqa.hnxiangtu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tta.c1oappe.top

[Q77] 时间加减
来源：http://vby.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://apg.jinghuilouyu.cn

[Q78] 当前时间
来源：http://ymg.ywan-chungtsiang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mjh.hfpthk.cn

[Q79] 字符串拼接
来源：http://oev.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mjd.zhengqikj.top

[Q80] 字符串截取
来源：http://mly.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qju.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://sji.zhaomingkeji.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://byk.yanxiufei.cn

[Q82] 字符长度与字节长度
来源：http://tsr.nwbrower.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bto.cdnleiting.top

[Q83] 大小写转换
来源：http://yjj.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mvf.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://ttu.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://qmu.9152youxi.cn

[Q85] 数值取整
来源：http://cxe.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://umw.chenlongwang.top

[Q86] 读取 JSON 字段
来源：http://ztr.ctjpmb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ybw.hcnkem.com

[Q87] JSON 字段做条件
来源：http://wew.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dtn.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://mbs.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gdg.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://npt.yonumen.top

[Q89] 判断表是否存在
来源：http://rpa.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zez.yj202588.top

[Q90] 生成序号列
来源：http://iom.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uvp.yfazqb.com

================================================================================
来源：http://ggn.jinqigufen.top

R. Bash 专题
来源：http://jnu.feifeiyinyue.top

================================================================================
来源：http://woj.sxryk.cn

[R01] shebang 与严格模式
来源：http://szo.zhengqikj.top

#!/usr/bin/env bash
来源：http://mvr.316326.xyz

set -euo pipefail
来源：http://fib.jqgfzy.top

[R02] 变量赋值与使用
来源：http://xzz.chenzaomai.com

name="Tom"; echo "$name"
来源：http://bzw.316326.xyz

[R03] 只读变量
来源：http://tei.haohaochexian.top

readonly PI=3.14
来源：http://lzs.xylfe.cn

[R04] 位置参数
来源：http://mwg.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xbd.hfpthk.cn

[R05] 参数默认值
来源：http://fnb.bbcook.cn

name="${1:-default}"
来源：http://ybm.ybcxt.top

[R06] 判断命令是否存在
来源：http://sqf.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tff.mhx1999.top

[R07] if 判断文件
来源：http://fnp.guannengcc.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wpq.yj20258.top

[R08] 数值比较
来源：http://unb.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ywg.zhoulong.xyz

[R09] 字符串比较
来源：http://guy.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wbz.yj20258.top

[R10] 正则匹配
来源：http://bmb.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ipx.pycfn.com

[R11] case 多分支
来源：http://cqq.c1oappe.top


<!-- 参考信息 -->