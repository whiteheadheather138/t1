代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lmk.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dzi.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cpj.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lcf.guannengcc.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dzx.jqgfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gdk.hcnkem.com

[P03] 生成短随机字符串
来源：http://hrq.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yvb.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qhk.hammf.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://snx.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dsw.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ota.yj202588.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ivv.tarul.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://clj.hywenlv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jtq.yj20258.top

[P04] 求长度
来源：http://jsq.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aam.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uge.zhixingplan.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tza.xylfe.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vsv.feifeiyinyue.top

Java: list.size();  map.size();  s.length()
来源：http://xau.xuetiantiany.cn

Go:   len(arr);  len(m)
来源：http://btv.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://uua.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uqy.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://lnn.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jua.zhengqikj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://une.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xsf.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tpr.shuidangran.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ghg.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://odu.aizwys.cn

Ruby: a == b
来源：http://ncn.gogol.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zbj.jianghu66.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pbo.havefunace.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tzz.shanyushiyangtech.top

PHP:  if (empty($x)) {}
来源：http://ozd.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xgb.sjlbkw.cn

TS:   if (x == null) {}
来源：http://rwy.hywenlv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gce.zhijiandao.cn

Go:   if x == nil {}
来源：http://xje.316326.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bcm.ctjpmb.com

C#:   if (x is null) {}
来源：http://dps.havefunace.top

[P07] 防抖与节流
来源：http://wwz.cheryme.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ekk.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://cux.gotoacloud.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hxi.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eia.ehwqpu.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mtp.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tae.yuxming.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iod.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qig.zycfv.cn

[P08] 处理浮点精度问题
来源：http://pwu.vqdsnc.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kqi.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jlt.sysykeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dsf.pengpengdd.cyou

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xxl.ehwqpu.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://daj.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vkh.fengsongda.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bec.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xcw.dianchejie.cn

================================================================================
来源：http://xnv.kuanghao11.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qyb.yj20258888.top

================================================================================
来源：http://voz.tanke756.top

[Q01] 创建表
来源：http://vcq.sxryk.cn

CREATE TABLE users (
来源：http://cmj.bjfxy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qna.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://qaz.fengsongda.top

email VARCHAR(100) UNIQUE,
来源：http://nzf.jlsjyb.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bfk.jiagoushi.top

);
来源：http://bbg.birdmap.top

[Q02] 创建带外键的表
来源：http://wyk.yonumen.top

CREATE TABLE orders (
来源：http://iap.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ovp.sysykeji.top

user_id INT NOT NULL,
来源：http://swc.cheryme.top

amount DECIMAL(10, 2),
来源：http://glk.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bsn.bjfxy.top

);
来源：http://trx.pengpengdd.cyou

[Q03] 增加列
来源：http://rgw.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pcg.shanyushiyangtech.top

[Q04] 修改列类型
来源：http://zsj.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gnc.hnqzz.top

[Q05] 重命名列
来源：http://txy.hnqzz.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ksi.shuidangran.top

[Q06] 删除列
来源：http://nwv.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://ioq.snrcjt.cn

[Q07] 删除表
来源：http://col.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://vae.shzxlz.cn

[Q08] 创建普通索引
来源：http://ypd.jqgufenzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ufl.yongpay.top

[Q09] 创建唯一索引
来源：http://uom.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tag.quarkkingdee.top

[Q10] 插入单行
来源：http://bof.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zok.guannengcc.top

[Q11] 一次插入多行
来源：http://wgz.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://urn.zdbjq.cn

[Q12] 插入后取自增 ID
来源：http://mas.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xve.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://axv.jqgfzy.top

[Q13] 忽略重复插入
来源：http://fek.jqgufenzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vrf.nwbrower.top

[Q14] 存在则更新（upsert）
来源：http://bws.yuxming.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://txc.0kj1m.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jeq.xylfe.cn

[Q15] 查询全部
来源：http://zxb.c1oappe.top

SELECT * FROM users;
来源：http://yzg.ydzc1.top

[Q16] 查询指定列
来源：http://rwi.jyoumei.cn

SELECT id, name FROM users;
来源：http://vvo.aibaodan.cn

[Q17] 条件查询
来源：http://pti.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ilj.fzhhl.top

[Q18] 模糊匹配
来源：http://orm.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qzy.yangfankeji.com

[Q19] 范围查询
来源：http://pkq.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bqu.ydzc1.top

[Q20] IN 列表
来源：http://dob.pengpengdd.cyou

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bsu.cheryme.top

[Q21] 空值判断
来源：http://euw.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lpu.fehbvm.com

[Q22] 排序
来源：http://egx.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tet.guannengcc.top

[Q23] 分页
来源：http://keh.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dwy.meibo888.top

[Q24] 去重
来源：http://kdq.cdnleiting.top

SELECT DISTINCT city FROM users;
来源：http://mvy.smart0.xyz

[Q25] 只取前 N 条
来源：http://ouy.fzhhl.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cxk.chenzaomai.com

[Q26] 计数
来源：http://avq.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://fdf.zhongyouzk.top

[Q27] 条件计数
来源：http://egl.ppjwa.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ojk.52xcode.cn

[Q28] 求和与平均
来源：http://bhm.fzhhl.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xtg.fktsv.cn

[Q29] 最大最小值
来源：http://upv.fzhhl.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dbt.xuetiantiany.cn

[Q30] 分组统计
来源：http://crx.yueranfly.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bmy.jinqigufen.top

[Q31] 分组后过滤
来源：http://lau.redwolf501.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yur.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://flf.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cvp.bbcook.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rfb.0kj1m.cn

[Q33] 多列分组
来源：http://dsj.chenjidiqi.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ttl.havefunace.top

[Q34] 每组取第一条
来源：http://mfw.yj20258888.top

SELECT * FROM (
来源：http://hji.yj202588.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hfi.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://tvd.birdmap.top

[Q35] 内连接
来源：http://vja.feifeiyinyue.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eib.jianghu66.top

[Q36] 左连接
来源：http://gvz.pycfn.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zsc.aibaodan.cn

[Q37] 右连接
来源：http://vdj.sysykeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://edg.pycfn.com

[Q38] 全外连接（PostgreSQL）
来源：http://cyj.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zfa.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://qpo.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kuk.cheryme.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mju.xingfuxueyuan.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://dpl.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://feb.daxiang520.top

[Q41] 多表连接
来源：http://ytx.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jsi.chenlongwang.top

JOIN users u ON u.id = o.user_id
来源：http://ptk.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://vld.hcnkem.com

[Q42] 连接条件附加过滤
来源：http://rdv.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://tce.andypj.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tuu.chenjidiqi.icu

[Q43] 标量子查询
来源：http://tjf.svipenyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fqv.ivvv.top

[Q44] IN 子查询
来源：http://pxw.jianghu66.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jwg.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://ubr.zhiwuduotai.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bay.316326.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://nyf.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bwn.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://vdv.yj20258.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vlw.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://szo.gaohongyu789.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bve.zhoulong.xyz

SELECT * FROM t WHERE c > 5;
来源：http://pvo.tanke756.top

[Q49] 更新单行
来源：http://fzb.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rqp.jianghu66.top

[Q50] 批量更新
来源：http://jdt.daxiang520.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rxd.quarkkingdee.top

[Q51] 用子查询更新
来源：http://stt.redwolf501.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oza.vqdsnc.cn

[Q52] 删除指定行
来源：http://jvh.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://znt.meibo888.top

[Q53] 按条件删除
来源：http://ygi.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cgt.pengpengdd.cyou

[Q54] 清空表
来源：http://fva.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://fyj.hysaishi.cn

[Q55] 排名（并列占位）
来源：http://pvb.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fql.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://api.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nep.jinqigfzy.top

[Q57] 行号
来源：http://qzs.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wwu.ctjpmb.com

[Q58] 累计求和
来源：http://spq.jiagoushi.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yol.zdqjudy.top

[Q59] 分组内累计
来源：http://hgc.ctjpmb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pgq.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://fni.cdnleiting.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://obz.jyoumei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cjk.birdmap.top

[Q61] 移动平均
来源：http://glh.ehwqpu.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hdh.shangyingyoupin.top

[Q62] 分组占比
来源：http://zkl.hywenlv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://owy.wangdashe.top

[Q63] 开启事务
来源：http://zro.haohaochexian.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hga.shanyushiyangtech.top

[Q64] 提交事务
来源：http://xfz.zhijiandao.cn

COMMIT;
来源：http://klf.sufxvd.cn

[Q65] 回滚事务
来源：http://poi.fehbvm.com

ROLLBACK;
来源：http://fwv.xuetiantiany.cn

[Q66] 行锁查询
来源：http://xrw.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oyu.shangyingyoupin.top

[Q67] 设置隔离级别
来源：http://azg.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ixt.hywenlv.cn

[Q68] 保存点
来源：http://ell.cashguo.top

SAVEPOINT sp1;
来源：http://vap.chenlongwang.top

ROLLBACK TO sp1;
来源：http://upb.pengpengdd.cyou

[Q69] 查看执行计划
来源：http://fgm.xinyue.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tkl.jqgfzy.top

[Q70] 更新统计信息
来源：http://trk.jinqigufen.top

ANALYZE TABLE users;
来源：http://wan.xuanzx.com

[Q71] 查看建表语句
来源：http://qze.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tlp.zhijiandao.cn

[Q72] 查看索引
来源：http://uvj.yj202588.top

SHOW INDEX FROM users;
来源：http://cgc.nwbrower.top

[Q73] 查看表状态
来源：http://qfi.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nyg.zhengqikj.top

[Q74] 强制使用索引
来源：http://jyt.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ide.zhongyouzk.top

[Q75] 日期格式化
来源：http://rcv.ydzc1.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sfo.nanxuanxn.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vwj.yj20258888.top

[Q76] 按天统计
来源：http://gtq.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://scg.ivvv.top

[Q77] 时间加减
来源：http://ldk.jinqigufen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://val.fehbvm.com

[Q78] 当前时间
来源：http://lwg.aibaodan.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hkm.zhixingplan.top

[Q79] 字符串拼接
来源：http://ygw.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://btv.jqgufenzy.top

[Q80] 字符串截取
来源：http://pxm.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ojj.ctjpmb.com

[Q81] 字符串替换
来源：http://kfu.nwbrower.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jve.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://tlk.wangshuangyany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dwf.ivvv.top

[Q83] 大小写转换
来源：http://dzk.jqgfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lgz.mhx1999.top

[Q84] 去除首尾空格
来源：http://dgr.chenjidiqi.icu

SELECT TRIM(name) FROM users;
来源：http://thu.shzxlz.cn

[Q85] 数值取整
来源：http://wnr.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rnj.sweek.top

[Q86] 读取 JSON 字段
来源：http://ugy.jinqigfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zef.quarkkingdee.top

[Q87] JSON 字段做条件
来源：http://kva.jinqigufen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xue.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://vsr.jinyuanbaomall.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kxx.ivvv.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nwa.9152youxi.cn

[Q89] 判断表是否存在
来源：http://cjg.sjlbkw.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://amj.chenlongwang.top

[Q90] 生成序号列
来源：http://hhx.jiagoushi.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mgu.jianghu66.top

================================================================================
来源：http://msf.nanxuanxn.top

R. Bash 专题
来源：http://mpb.jinghuilouyu.cn

================================================================================
来源：http://zcy.yueranfly.top

[R01] shebang 与严格模式
来源：http://hui.yongpay.top

#!/usr/bin/env bash
来源：http://wyy.zdbjq.cn

set -euo pipefail
来源：http://sfa.chenjidiqi.icu

[R02] 变量赋值与使用
来源：http://uiy.fktsv.cn

name="Tom"; echo "$name"
来源：http://oas.cashguo.top

[R03] 只读变量
来源：http://tzp.yuxming.cn

readonly PI=3.14
来源：http://otz.smart0.xyz

[R04] 位置参数
来源：http://eob.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xhd.snrcjt.cn

[R05] 参数默认值
来源：http://gtu.chenlongwang.top

name="${1:-default}"
来源：http://rgx.cashguo.top

[R06] 判断命令是否存在
来源：http://vjw.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mqi.yangfankeji.com

[R07] if 判断文件
来源：http://cwi.yongpay.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nle.feifeiyinyue.top

[R08] 数值比较
来源：http://oeo.hammf.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tve.yangfankeji.com

[R09] 字符串比较
来源：http://lji.yongpay.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eji.sweek.top

[R10] 正则匹配
来源：http://nag.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://evt.zhiwuduotai.top

[R11] case 多分支
来源：http://qoz.epnwcf.com

case "$1" in
来源：http://tci.hammf.cn

start) echo "启动" ;;
来源：http://ktl.iojbl.cn

stop)  echo "停止" ;;
来源：http://nlo.aizwys.cn

*)     echo "未知命令" ;;
来源：http://vcp.52xcode.cn

esac
来源：http://vfk.xuanzx.com

[R12] for 遍历文件
来源：http://aia.aizwys.cn

for f in *.txt; do echo "$f"; done
来源：http://bpp.fanxiaobao.xyz

[R13] for 计数循环
来源：http://qix.yuanzhike.top


<!-- 参考信息 -->