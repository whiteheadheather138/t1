代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://niw.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://kpd.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cjs.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fat.nanxinkj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pun.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fir.ppjwa.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kfg.9152youxi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xoq.snrcjt.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://svb.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dwr.hcnkem.com

[P03] 生成短随机字符串
来源：http://zbw.yvedp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fod.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jas.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bwo.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fwa.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://msv.pycfn.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yrj.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zft.bbcook.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xbl.nanxuanxn.top

[P04] 求长度
来源：http://iah.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ity.yfazqb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ynj.daria6918.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ugj.316326.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qhr.zhoulong.xyz

Java: list.size();  map.size();  s.length()
来源：http://wmt.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://xkx.yueranfly.top

Ruby: x.length;  x.size
来源：http://mne.zhaomingkeji.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://odd.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://kbr.zhiwuduotai.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kid.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wlv.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ffd.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lhz.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oxb.yvedp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jrg.chenlongwang.top

Ruby: a == b
来源：http://pfm.ppjwa.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hra.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aqv.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pxd.meibo888.top

PHP:  if (empty($x)) {}
来源：http://iex.cucudq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hqf.chenjidiqi.icu

TS:   if (x == null) {}
来源：http://tmw.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ndd.ppjwa.cn

Go:   if x == nil {}
来源：http://jdt.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sed.yanxiufei.cn

C#:   if (x is null) {}
来源：http://xhg.chenzaomai.com

[P07] 防抖与节流
来源：http://kzo.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nbn.smart0.xyz

PHP:  // 手写时间戳比较
来源：http://vri.zhengqikj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ukq.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nlp.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://txy.jinqigfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://csy.cheryme.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mit.redwolf501.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eke.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://jub.dashuyun.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bbp.bjfxy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yhg.ivvv.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gyn.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hiv.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fgs.hnxiangtu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cap.ehwqpu.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xdu.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vuw.quarkkingdee.top

================================================================================
来源：http://syt.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jrn.wangshuangyany.cn

================================================================================
来源：http://vgv.meibo888.top

[Q01] 创建表
来源：http://ftb.yuanzhike.top

CREATE TABLE users (
来源：http://ohk.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yoj.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://ogo.dianchejie.cn

email VARCHAR(100) UNIQUE,
来源：http://xov.cashguo.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ffp.jianghu66.top

);
来源：http://vhl.gotoacloud.top

[Q02] 创建带外键的表
来源：http://ynm.daria6918.cn

CREATE TABLE orders (
来源：http://eic.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://glw.zhiwuduotai.top

user_id INT NOT NULL,
来源：http://rty.c1oappe.top

amount DECIMAL(10, 2),
来源：http://guf.jinyuanbaomall.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sib.tanke756.top

);
来源：http://lzk.yj202588.top

[Q03] 增加列
来源：http://jqr.yj20258.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dsr.vehdjk.com

[Q04] 修改列类型
来源：http://ezi.yvedp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wkm.bbcook.cn

[Q05] 重命名列
来源：http://bmy.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zww.316326.xyz

[Q06] 删除列
来源：http://tms.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://mak.yj20258.top

[Q07] 删除表
来源：http://nny.yuanzhike.top

DROP TABLE IF EXISTS orders;
来源：http://aej.shuidangran.top

[Q08] 创建普通索引
来源：http://fra.yangfankeji.com

CREATE INDEX idx_users_email ON users(email);
来源：http://omd.dianchejie.cn

[Q09] 创建唯一索引
来源：http://poc.jqgfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aah.jinqigfzy.top

[Q10] 插入单行
来源：http://aie.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://daq.guowangkeji.top

[Q11] 一次插入多行
来源：http://uim.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wtm.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://sbm.yj20258.top

INSERT INTO users (name) VALUES ('C');
来源：http://nkn.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rrp.xuanzx.com

[Q13] 忽略重复插入
来源：http://bhq.meibo888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://myc.0kj1m.cn

[Q14] 存在则更新（upsert）
来源：http://tnu.ybcxt.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vlo.bbcook.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ulk.redwolf501.top

[Q15] 查询全部
来源：http://zuq.xziqi.cn

SELECT * FROM users;
来源：http://zdb.kuanghao11.cn

[Q16] 查询指定列
来源：http://ezv.zhijiandao.cn

SELECT id, name FROM users;
来源：http://ahg.shzxlz.cn

[Q17] 条件查询
来源：http://knd.xinyue.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sah.ctjpmb.com

[Q18] 模糊匹配
来源：http://tig.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wjd.9152youxi.cn

[Q19] 范围查询
来源：http://vgs.nanxinkj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yum.cdnleiting.top

[Q20] IN 列表
来源：http://bey.hongshengwenyu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kmj.cqqwz.cn

[Q21] 空值判断
来源：http://usz.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://txn.nanxinkj.top

[Q22] 排序
来源：http://blm.hongshengwenyu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qyi.zhongyouzk.top

[Q23] 分页
来源：http://kad.yj20258888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://txz.sufxvd.cn

[Q24] 去重
来源：http://jpz.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://gls.fzhhl.top

[Q25] 只取前 N 条
来源：http://irt.yueranfly.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vkn.sufxvd.cn

[Q26] 计数
来源：http://oxr.zdqjudy.top

SELECT COUNT(*) FROM users;
来源：http://ekr.quarkkingdee.top

[Q27] 条件计数
来源：http://ket.52xcode.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sev.sxryk.cn

[Q28] 求和与平均
来源：http://mpg.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ydu.dianchejie.cn

[Q29] 最大最小值
来源：http://sck.aibaodan.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lby.gaohongyu789.top

[Q30] 分组统计
来源：http://kxg.gotoacloud.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gaz.yangfankeji.com

[Q31] 分组后过滤
来源：http://qft.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ghz.quarkkingdee.top

[Q32] 分组拼接字符串
来源：http://qto.c1oappe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ziu.hongshengwenyu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gxn.ywan-chungtsiang.top

[Q33] 多列分组
来源：http://tvh.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://whj.jqgfzy.top

[Q34] 每组取第一条
来源：http://jhj.jinqigufen.top

SELECT * FROM (
来源：http://wan.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xuy.hcnkem.com

) t WHERE rn = 1;
来源：http://hbf.pycfn.com

[Q35] 内连接
来源：http://loj.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lgg.c1oappe.top

[Q36] 左连接
来源：http://drm.havefunace.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gwl.ydzc1.top

[Q37] 右连接
来源：http://szo.gogol.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wkw.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://eyi.yangfankeji.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vxx.zhaomingkeji.xyz

[Q39] 自连接（查上下级）
来源：http://okh.ydjk.org.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://duy.yuanzhike.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zos.zhijiandao.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pvd.hammf.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jkf.ywan-chungtsiang.top

[Q41] 多表连接
来源：http://bmc.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://onr.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://xor.uphjek.com

JOIN products p ON p.id = o.product_id;
来源：http://she.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://glz.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://jkv.haohaochexian.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eow.yj20258888.top

[Q43] 标量子查询
来源：http://twm.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jfn.wangdashe.top

[Q44] IN 子查询
来源：http://yoc.316326.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://flb.sweek.top

[Q45] EXISTS 判断存在
来源：http://zce.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kzd.jyoumei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mia.smart0.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uto.epnwcf.com

[Q47] 与平均值比较
来源：http://sgq.yongpay.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://maf.hammf.cn

[Q48] CTE 公用表表达式
来源：http://ppy.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ige.ydzc1.top

SELECT * FROM t WHERE c > 5;
来源：http://gxo.guannengcc.top

[Q49] 更新单行
来源：http://jle.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jcd.ydjk.org.cn

[Q50] 批量更新
来源：http://bun.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xdk.ivvv.top

[Q51] 用子查询更新
来源：http://idc.shanyushiyangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qws.gaohongyu789.top

[Q52] 删除指定行
来源：http://nys.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://ksq.pengpengdd.cyou

[Q53] 按条件删除
来源：http://ick.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qub.gzhubu.top

[Q54] 清空表
来源：http://sul.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://pyv.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://yzf.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fdh.cashguo.top

[Q56] 密集排名（并列不占位）
来源：http://nff.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xxc.redwolf501.top

[Q57] 行号
来源：http://wtg.wangdashe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zoj.fktsv.cn

[Q58] 累计求和
来源：http://vdo.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kki.chenlongwang.top

[Q59] 分组内累计
来源：http://wrr.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bwy.yonumen.top

[Q60] 取上一行 / 下一行
来源：http://zbc.jianghu66.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://efa.yj20258888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mgt.daria6918.cn

[Q61] 移动平均
来源：http://sxy.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lph.ydzc1.top

[Q62] 分组占比
来源：http://qwx.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://onz.wangdashe.top

[Q63] 开启事务
来源：http://cec.hongshengwenyu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sku.feifeiyinyue.top

[Q64] 提交事务
来源：http://mkb.yuxming.cn

COMMIT;
来源：http://duf.tanke756.top

[Q65] 回滚事务
来源：http://trc.kuanghao11.cn

ROLLBACK;
来源：http://hbq.daxiang520.top

[Q66] 行锁查询
来源：http://psl.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://shv.chenlongwang.top

[Q67] 设置隔离级别
来源：http://drj.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://swf.sysykeji.top

[Q68] 保存点
来源：http://rka.jinqigufen.top

SAVEPOINT sp1;
来源：http://rnv.gotoacloud.top

ROLLBACK TO sp1;
来源：http://obi.sysykeji.top

[Q69] 查看执行计划
来源：http://ryi.zhaomingkeji.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zti.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://eky.pycfn.com

ANALYZE TABLE users;
来源：http://bam.fktsv.cn

[Q71] 查看建表语句
来源：http://yba.yfazqb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bsl.fehbvm.com

[Q72] 查看索引
来源：http://rjd.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://bhl.gzhubu.top

[Q73] 查看表状态
来源：http://sta.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dme.fehbvm.com

[Q74] 强制使用索引
来源：http://sfs.epnwcf.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nsf.smart0.xyz

[Q75] 日期格式化
来源：http://dab.bbcook.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oqe.chenjidiqi.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sqs.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://zvc.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ijd.cucudq.cn

[Q77] 时间加减
来源：http://sjc.zhaomingkeji.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ucl.jqgufenzy.top

[Q78] 当前时间
来源：http://uvj.sufxvd.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mzg.hammf.cn

[Q79] 字符串拼接
来源：http://fyg.gotoacloud.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dce.yj20258888.top

[Q80] 字符串截取
来源：http://wzu.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vnw.guannengcc.top

[Q81] 字符串替换
来源：http://abv.fzhhl.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gwk.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://pvl.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://exv.gzhubu.top

[Q83] 大小写转换
来源：http://tiq.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fkc.tarul.cn

[Q84] 去除首尾空格
来源：http://hmw.xuetiantiany.cn

SELECT TRIM(name) FROM users;
来源：http://eym.vqdsnc.cn

[Q85] 数值取整
来源：http://gue.chenlongwang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mot.quarkkingdee.top

[Q86] 读取 JSON 字段
来源：http://cdt.pycfn.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hzl.shanyushiyangkeji.top

[Q87] JSON 字段做条件
来源：http://mum.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iyy.xingfuxueyuan.xyz

[Q88] 行转列（条件聚合）
来源：http://gep.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hzb.zhengqikj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tgz.yueranfly.top

[Q89] 判断表是否存在
来源：http://jwy.hcnkem.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lum.hysaishi.cn

[Q90] 生成序号列
来源：http://qch.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nhv.jinqigfzy.top

================================================================================
来源：http://wwe.xuetiantiany.cn

R. Bash 专题
来源：http://cup.jyoumei.cn

================================================================================
来源：http://rmf.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://lct.dashuyun.cn

#!/usr/bin/env bash
来源：http://sun.xuetiantiany.cn

set -euo pipefail
来源：http://lmo.dianchejie.cn

[R02] 变量赋值与使用
来源：http://wru.cucudq.cn

name="Tom"; echo "$name"
来源：http://lju.zhengqikj.top

[R03] 只读变量
来源：http://ung.nanxuanxn.top

readonly PI=3.14
来源：http://usx.svipenyu.cn

[R04] 位置参数
来源：http://rfi.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zol.zdbjq.cn

[R05] 参数默认值
来源：http://imv.cqqwz.cn

name="${1:-default}"
来源：http://kgk.cqqwz.cn

[R06] 判断命令是否存在
来源：http://dax.jianghu66.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jvl.mhx1999.top

[R07] if 判断文件
来源：http://vgi.zhoulong.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://onm.zhoulong.xyz

[R08] 数值比较
来源：http://qun.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://twg.ybcxt.top

[R09] 字符串比较
来源：http://lpz.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://akr.chenjidiqi.icu

[R10] 正则匹配
来源：http://ecm.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oay.tianlin.xyz

[R11] case 多分支
来源：http://wel.xinyue.icu

case "$1" in
来源：http://itj.zdbjq.cn

start) echo "启动" ;;
来源：http://gqo.iojbl.cn

stop)  echo "停止" ;;
来源：http://pac.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://akg.yj202588.top


<!-- 参考信息 -->