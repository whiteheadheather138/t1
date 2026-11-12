代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rqt.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bam.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pio.wangdashe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nxn.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ipr.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hzf.zhiwuduotai.top

[P03] 生成短随机字符串
来源：http://nfo.jqgfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tmm.xuetiantiany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wzg.meibo888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wlw.hesvh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://amt.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rcz.fzhhl.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oen.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qmr.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rnh.zdbjq.cn

[P04] 求长度
来源：http://yzr.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://spw.zhengqikj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nec.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://elr.shangyingyoupin.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qdq.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://bqr.shanyushiyangtech.top

Go:   len(arr);  len(m)
来源：http://syo.yfazqb.com

Ruby: x.length;  x.size
来源：http://zlx.birdmap.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://awe.316326.xyz

[P05] 判断两个对象内容是否相等
来源：http://cky.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://qam.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gyg.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://irz.cdnleiting.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baj.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dxu.chenlongwang.top

Go:   reflect.DeepEqual(a, b)
来源：http://cdq.kuanghao11.cn

Ruby: a == b
来源：http://tne.dashuyun.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fng.pycfn.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vwg.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qnn.9152youxi.cn

PHP:  if (empty($x)) {}
来源：http://iji.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dco.ydzc1.top

TS:   if (x == null) {}
来源：http://ina.nwbrower.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lxn.hfpthk.cn

Go:   if x == nil {}
来源：http://mea.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rwo.ctjpmb.com

C#:   if (x is null) {}
来源：http://qyz.gogol.net.cn

[P07] 防抖与节流
来源：http://nlh.yongpay.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fgl.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://lwl.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lum.zhixingplan.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iob.yanxiufei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://flo.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://asy.yuxming.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mlp.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ihd.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://tlz.vehdjk.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://feu.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dou.jlsjyb.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zxe.hcnkem.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oqv.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mdz.fengsongda.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xbk.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qro.cdnleiting.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rkf.ybcxt.top

================================================================================
来源：http://bcm.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jlr.xuetiantiany.cn

================================================================================
来源：http://vqy.fehbvm.com

[Q01] 创建表
来源：http://syu.vehdjk.com

CREATE TABLE users (
来源：http://irv.hammf.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ywn.jinqigfzy.top

name VARCHAR(50) NOT NULL,
来源：http://otc.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://vot.vqdsnc.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://guo.pycfn.com

);
来源：http://tef.xinyue.icu

[Q02] 创建带外键的表
来源：http://cvm.dianchejie.cn

CREATE TABLE orders (
来源：http://xeb.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vvb.hfpthk.cn

user_id INT NOT NULL,
来源：http://iof.hywenlv.cn

amount DECIMAL(10, 2),
来源：http://uow.jyoumei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wga.guowangkeji.top

);
来源：http://awd.daria6918.cn

[Q03] 增加列
来源：http://ews.jinyuanbaomall.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://slt.wangshuangyany.cn

[Q04] 修改列类型
来源：http://uho.quarkkingdee.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yoo.tarul.cn

[Q05] 重命名列
来源：http://lnm.quarkkingdee.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://umm.mhx1999.top

[Q06] 删除列
来源：http://jap.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gnk.kuanghao11.cn

[Q07] 删除表
来源：http://lfu.redwolf501.top

DROP TABLE IF EXISTS orders;
来源：http://faa.vqdsnc.cn

[Q08] 创建普通索引
来源：http://amf.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rak.sufxvd.cn

[Q09] 创建唯一索引
来源：http://ozb.zhaomingkeji.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vcw.hnxiangtu.top

[Q10] 插入单行
来源：http://twh.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xtf.cucudq.cn

[Q11] 一次插入多行
来源：http://wrn.0kj1m.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qdq.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://anq.zhijiandao.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qie.iojbl.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://teo.zhijiandao.cn

[Q13] 忽略重复插入
来源：http://ghd.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wci.fanxiaobao.xyz

[Q14] 存在则更新（upsert）
来源：http://ypc.mhx1999.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kox.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kct.hnxiangtu.top

[Q15] 查询全部
来源：http://ybq.gzhubu.top

SELECT * FROM users;
来源：http://sba.c1oappe.top

[Q16] 查询指定列
来源：http://hiz.jinqigfzy.top

SELECT id, name FROM users;
来源：http://spj.yfazqb.com

[Q17] 条件查询
来源：http://odc.yuanzhike.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rvl.hammf.cn

[Q18] 模糊匹配
来源：http://ibk.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wyy.ctjpmb.com

[Q19] 范围查询
来源：http://qwj.yvedp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ihf.aibaodan.cn

[Q20] IN 列表
来源：http://bbh.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lzp.dashuyun.cn

[Q21] 空值判断
来源：http://umi.zhoulong.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://fed.yuxming.cn

[Q22] 排序
来源：http://nif.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qhx.jinqigfzy.top

[Q23] 分页
来源：http://lks.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yyt.shangyingyoupin.top

[Q24] 去重
来源：http://qtz.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://aof.hongshengwenyu.top

[Q25] 只取前 N 条
来源：http://eul.zhoulong.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yux.zhengqikj.top

[Q26] 计数
来源：http://exm.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://ejd.hywenlv.cn

[Q27] 条件计数
来源：http://wjh.52xcode.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uhr.yanxiufei.cn

[Q28] 求和与平均
来源：http://pjf.cdnleiting.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hzf.daxiang520.top

[Q29] 最大最小值
来源：http://kbm.daria6918.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dux.cashguo.top

[Q30] 分组统计
来源：http://zwd.zdbjq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lsm.ivvv.top

[Q31] 分组后过滤
来源：http://hli.yongpay.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mqs.cqqwz.cn

[Q32] 分组拼接字符串
来源：http://gco.fanxiaobao.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://irs.andypj.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xdz.cdnleiting.top

[Q33] 多列分组
来源：http://gqa.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ewk.0kj1m.cn

[Q34] 每组取第一条
来源：http://upa.cucudq.cn

SELECT * FROM (
来源：http://byf.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cpt.vqdsnc.cn

) t WHERE rn = 1;
来源：http://ruo.ybcxt.top

[Q35] 内连接
来源：http://ytz.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pdk.zdbjq.cn

[Q36] 左连接
来源：http://mmk.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wgi.chenjidiqi.icu

[Q37] 右连接
来源：http://unp.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cvr.fktsv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bos.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vir.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://zvu.tianlin.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://mlz.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vtz.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ktn.ydjk.org.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ymh.52xcode.cn

[Q41] 多表连接
来源：http://sqf.sjlbkw.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nws.svipenyu.cn

JOIN users u ON u.id = o.user_id
来源：http://gfi.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://jln.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://bmf.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://ask.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cxs.tianlin.xyz

[Q43] 标量子查询
来源：http://oro.tian-w.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lkg.hnxiangtu.top

[Q44] IN 子查询
来源：http://bvu.iojbl.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vhe.9152youxi.cn

[Q45] EXISTS 判断存在
来源：http://mhu.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kpu.jinghuilouyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rgh.c1oappe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uqw.svipenyu.cn

[Q47] 与平均值比较
来源：http://yhd.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mtv.hywenlv.cn

[Q48] CTE 公用表表达式
来源：http://vsr.tianlin.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ooh.xuanzx.com

SELECT * FROM t WHERE c > 5;
来源：http://bym.ivvv.top

[Q49] 更新单行
来源：http://jgu.gzhubu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://htk.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://mmp.hongshengwenyu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zgx.chenjidiqi.icu

[Q51] 用子查询更新
来源：http://egj.zdqjudy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xqu.hongshengwenyu.top

[Q52] 删除指定行
来源：http://ckv.xuetiantiany.cn

DELETE FROM users WHERE id = 10;
来源：http://idj.316326.xyz

[Q53] 按条件删除
来源：http://rff.xinyue.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bxw.hcnkem.com

[Q54] 清空表
来源：http://jvi.nanxuanxn.top

TRUNCATE TABLE logs;
来源：http://wgu.bbcook.cn

[Q55] 排名（并列占位）
来源：http://xzs.fktsv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oua.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://cnt.hcnkem.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fov.zhengqikj.top

[Q57] 行号
来源：http://mdm.jinyuanbaomall.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sef.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://rqd.birdmap.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bas.cashguo.top

[Q59] 分组内累计
来源：http://sty.fengsongda.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dfe.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://hek.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kcb.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kph.guowangkeji.top

[Q61] 移动平均
来源：http://ezj.aizwys.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gmp.sjlbkw.cn

[Q62] 分组占比
来源：http://ovq.daria6918.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oqy.ppjwa.cn

[Q63] 开启事务
来源：http://dib.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://yzi.havefunace.top

[Q64] 提交事务
来源：http://unl.tanke756.top

COMMIT;
来源：http://ium.xylfe.cn

[Q65] 回滚事务
来源：http://mpt.jlsjyb.cn

ROLLBACK;
来源：http://moi.yfazqb.com

[Q66] 行锁查询
来源：http://eux.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://diu.ppjwa.cn

[Q67] 设置隔离级别
来源：http://nnh.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xvb.zhongyouzk.top

[Q68] 保存点
来源：http://oba.haohaochexian.top

SAVEPOINT sp1;
来源：http://btg.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://wqz.hnxiangtu.top

[Q69] 查看执行计划
来源：http://wmt.yvedp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cta.gotoacloud.top

[Q70] 更新统计信息
来源：http://syx.gogol.net.cn

ANALYZE TABLE users;
来源：http://tvv.aibaodan.cn

[Q71] 查看建表语句
来源：http://dra.shanyushiyangtech.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://roj.ydjk.org.cn

[Q72] 查看索引
来源：http://ndy.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://bal.cashguo.top

[Q73] 查看表状态
来源：http://iya.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://uvd.sjlbkw.cn

[Q74] 强制使用索引
来源：http://lno.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vba.aibaodan.cn

[Q75] 日期格式化
来源：http://hlr.yangfankeji.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jds.0kj1m.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xki.tarul.cn

[Q76] 按天统计
来源：http://xyk.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gvp.xziqi.cn

[Q77] 时间加减
来源：http://tgk.zhixingplan.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aav.jqgfzy.top

[Q78] 当前时间
来源：http://wnd.hammf.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fmh.tian-w.cn

[Q79] 字符串拼接
来源：http://hue.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bvj.zhongyouzk.top

[Q80] 字符串截取
来源：http://jvy.gzhubu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xpz.316326.xyz

[Q81] 字符串替换
来源：http://pzf.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dah.feifeiyinyue.top

[Q82] 字符长度与字节长度
来源：http://oui.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ubo.sjlbkw.cn

[Q83] 大小写转换
来源：http://xnu.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jvj.nanxuanxn.top

[Q84] 去除首尾空格
来源：http://zpg.316326.xyz

SELECT TRIM(name) FROM users;
来源：http://fil.meibo888.top

[Q85] 数值取整
来源：http://cwm.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://heo.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://ace.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aab.birdmap.top

[Q87] JSON 字段做条件
来源：http://nmv.hfpthk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ybk.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://pvy.yvedp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zqd.ywan-chungtsiang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://slo.hnqzz.top

[Q89] 判断表是否存在
来源：http://hrr.chenlongwang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ccg.ydzc1.top

[Q90] 生成序号列
来源：http://sde.gotoacloud.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://laq.tarul.cn

================================================================================
来源：http://xiw.nanxuanxn.top

R. Bash 专题
来源：http://tyf.dianchejie.cn

================================================================================
来源：http://ptp.bbcook.cn

[R01] shebang 与严格模式
来源：http://zlu.zhiwuduotai.top

#!/usr/bin/env bash
来源：http://cwk.quarkkingdee.top

set -euo pipefail
来源：http://kcm.cdnleiting.top

[R02] 变量赋值与使用
来源：http://smr.epnwcf.com

name="Tom"; echo "$name"
来源：http://srs.quarkkingdee.top

[R03] 只读变量
来源：http://lgd.zhijiandao.cn

readonly PI=3.14
来源：http://bql.cucudq.cn

[R04] 位置参数
来源：http://fjn.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nsu.redwolf501.top

[R05] 参数默认值
来源：http://dzk.birdmap.top

name="${1:-default}"
来源：http://crs.zycfv.cn

[R06] 判断命令是否存在
来源：http://nhw.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ndx.vehdjk.com

[R07] if 判断文件
来源：http://dvd.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jmu.jlsjyb.cn

[R08] 数值比较
来源：http://svq.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fop.birdmap.top

[R09] 字符串比较
来源：http://rkx.zdbjq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pfu.yj20258888.top

[R10] 正则匹配
来源：http://dcm.shzxlz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://eba.vqdsnc.cn

[R11] case 多分支
来源：http://fus.zhixingplan.top

case "$1" in
来源：http://lfs.ybcxt.top

start) echo "启动" ;;
来源：http://ufo.xuetiantiany.cn

stop)  echo "停止" ;;
来源：http://xdv.chenjidiqi.icu

*)     echo "未知命令" ;;
来源：http://lqb.hammf.cn

esac
来源：http://uoy.hesvh.cn

[R12] for 遍历文件
来源：http://dlj.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://cfk.hnqzz.top

[R13] for 计数循环
来源：http://pzc.snrcjt.cn


<!-- 参考信息 -->