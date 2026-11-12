代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dfg.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://skb.cucudq.cn

[P03] 生成短随机字符串
来源：http://map.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gqq.havefunace.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ktq.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qzh.gzhubu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yes.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vso.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qzm.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://euj.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mzo.jinqigfzy.top

[P04] 求长度
来源：http://zqo.sxryk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://piy.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ivg.sweek.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bgp.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gzg.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://onh.quarkkingdee.top

Go:   len(arr);  len(m)
来源：http://klt.zhoulong.xyz

Ruby: x.length;  x.size
来源：http://ary.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yyd.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://tvt.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xrh.andypj.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vzf.dashuyun.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qlj.aizwys.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ukh.zycfv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ier.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fad.cucudq.cn

Ruby: a == b
来源：http://ifo.mhx1999.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cbx.vqdsnc.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zda.ivvv.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xlw.dianchejie.cn

PHP:  if (empty($x)) {}
来源：http://obp.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://som.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://fdy.bjfxy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://usc.sjlbkw.cn

Go:   if x == nil {}
来源：http://bag.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://szf.shanyushiyangtech.top

C#:   if (x is null) {}
来源：http://yiv.nwbrower.top

[P07] 防抖与节流
来源：http://xic.quarkkingdee.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vcz.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://klp.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lsy.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxi.aibaodan.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tmm.ivvv.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dhd.yongpay.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ose.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kjr.gzhubu.top

[P08] 处理浮点精度问题
来源：http://nnl.cheryme.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tjj.uphjek.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dzq.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fzp.ybcxt.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uwu.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nuw.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jmd.0kj1m.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nrm.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kaa.hcnkem.com

================================================================================
来源：http://ynd.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aus.cdnleiting.top

================================================================================
来源：http://auu.xuetiantiany.cn

[Q01] 创建表
来源：http://ixa.zhixingplan.top

CREATE TABLE users (
来源：http://vfc.52xcode.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ufj.mhx1999.top

name VARCHAR(50) NOT NULL,
来源：http://zqb.xuetiantiany.cn

email VARCHAR(100) UNIQUE,
来源：http://psj.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tqf.pycfn.com

);
来源：http://dop.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://siy.hfpthk.cn

CREATE TABLE orders (
来源：http://gci.fanxiaobao.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cml.hysaishi.cn

user_id INT NOT NULL,
来源：http://swz.yj20258.top

amount DECIMAL(10, 2),
来源：http://blq.redwolf501.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jhh.pycfn.com

);
来源：http://ipa.dianchejie.cn

[Q03] 增加列
来源：http://suh.xuetiantiany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fzw.cashguo.top

[Q04] 修改列类型
来源：http://fao.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vqs.kuanghao11.cn

[Q05] 重命名列
来源：http://goa.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mqn.havefunace.top

[Q06] 删除列
来源：http://ood.nanxuanxn.top

ALTER TABLE users DROP COLUMN age;
来源：http://pjv.hfpthk.cn

[Q07] 删除表
来源：http://pak.shzxlz.cn

DROP TABLE IF EXISTS orders;
来源：http://ckw.nanxuanxn.top

[Q08] 创建普通索引
来源：http://bpy.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pyt.tianlin.xyz

[Q09] 创建唯一索引
来源：http://xfx.yonumen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yev.vqdsnc.cn

[Q10] 插入单行
来源：http://yzl.epnwcf.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ikw.hcnkem.com

[Q11] 一次插入多行
来源：http://tvr.ctjpmb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lfq.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://efu.yj202588.top

INSERT INTO users (name) VALUES ('C');
来源：http://gwg.jqgfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://djr.ydjk.org.cn

[Q13] 忽略重复插入
来源：http://kdr.yonumen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kna.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://pgi.aibaodan.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tvv.hfpthk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fhd.zhixingplan.top

[Q15] 查询全部
来源：http://axl.hfpthk.cn

SELECT * FROM users;
来源：http://rxc.xylfe.cn

[Q16] 查询指定列
来源：http://upq.svipenyu.cn

SELECT id, name FROM users;
来源：http://omu.jiagoushi.top

[Q17] 条件查询
来源：http://cqp.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pwh.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://pwo.jianghu66.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jdt.chenjidiqi.icu

[Q19] 范围查询
来源：http://xwj.sxryk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dkq.ydzc1.top

[Q20] IN 列表
来源：http://mhm.xuetiantiany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hcf.zhiwuduotai.top

[Q21] 空值判断
来源：http://pxd.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://xsa.sufxvd.cn

[Q22] 排序
来源：http://gas.cqqwz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://khb.nwbrower.top

[Q23] 分页
来源：http://gij.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wse.pengpengdd.cyou

[Q24] 去重
来源：http://suo.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://thv.sweek.top

[Q25] 只取前 N 条
来源：http://bwk.guowangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://toh.ywan-chungtsiang.top

[Q26] 计数
来源：http://lku.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://iuw.jinqigfzy.top

[Q27] 条件计数
来源：http://pma.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gqh.iojbl.cn

[Q28] 求和与平均
来源：http://cmc.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://via.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://dxp.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zjz.tarul.cn

[Q30] 分组统计
来源：http://kte.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rma.jqgufenzy.top

[Q31] 分组后过滤
来源：http://ykr.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pph.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://jeh.snrcjt.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hsq.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qvo.9152youxi.cn

[Q33] 多列分组
来源：http://agy.epnwcf.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pgb.guannengcc.top

[Q34] 每组取第一条
来源：http://ync.bjfxy.top

SELECT * FROM (
来源：http://zuz.jinghuilouyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lkz.kuanghao11.cn

) t WHERE rn = 1;
来源：http://bpv.zdqjudy.top

[Q35] 内连接
来源：http://ral.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xsk.dashuyun.cn

[Q36] 左连接
来源：http://scd.shangyingyoupin.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pim.smart0.xyz

[Q37] 右连接
来源：http://nkv.fengsongda.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uhw.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://usv.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://szd.jyoumei.cn

[Q39] 自连接（查上下级）
来源：http://drf.jyoumei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://edn.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jbx.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uge.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yjk.redwolf501.top

[Q41] 多表连接
来源：http://isk.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ged.cucudq.cn

JOIN users u ON u.id = o.user_id
来源：http://tbg.svipenyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://fnv.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://ods.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://wvv.ydzc1.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ktt.0kj1m.cn

[Q43] 标量子查询
来源：http://vhu.ivvv.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lsf.cucudq.cn

[Q44] IN 子查询
来源：http://vqw.yongpay.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blu.cdnleiting.top

[Q45] EXISTS 判断存在
来源：http://jyf.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jyf.epnwcf.com

[Q46] NOT EXISTS 判断不存在
来源：http://vgz.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uru.zhengqikj.top

[Q47] 与平均值比较
来源：http://epv.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nxi.cashguo.top

[Q48] CTE 公用表表达式
来源：http://igl.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lvg.xylfe.cn

SELECT * FROM t WHERE c > 5;
来源：http://zub.snrcjt.cn

[Q49] 更新单行
来源：http://peo.cucudq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://edq.nanxinkj.top

[Q50] 批量更新
来源：http://hbd.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tpi.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://jcv.gogol.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uvs.yj20258888.top

[Q52] 删除指定行
来源：http://pmr.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://xow.316326.xyz

[Q53] 按条件删除
来源：http://rzb.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jnt.gaohongyu789.top

[Q54] 清空表
来源：http://scc.bjfxy.top

TRUNCATE TABLE logs;
来源：http://ocg.bjfxy.top

[Q55] 排名（并列占位）
来源：http://rpf.yanxiufei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mfk.bjfxy.top

[Q56] 密集排名（并列不占位）
来源：http://ocm.daria6918.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wzk.yanxiufei.cn

[Q57] 行号
来源：http://btj.meibo888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qbh.yfazqb.com

[Q58] 累计求和
来源：http://eji.yj202588.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mpu.bjfxy.top

[Q59] 分组内累计
来源：http://pkx.dashuyun.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kor.0kj1m.cn

[Q60] 取上一行 / 下一行
来源：http://rrk.sxryk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://grr.xuanzx.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://emu.9152youxi.cn

[Q61] 移动平均
来源：http://mfc.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jvh.nanxinkj.top

[Q62] 分组占比
来源：http://rdo.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://etp.vehdjk.com

[Q63] 开启事务
来源：http://hjy.xylfe.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kqo.ydzc1.top

[Q64] 提交事务
来源：http://esv.zdbjq.cn

COMMIT;
来源：http://lcn.aibaodan.cn

[Q65] 回滚事务
来源：http://hoy.bjfxy.top

ROLLBACK;
来源：http://vdi.zhengqikj.top

[Q66] 行锁查询
来源：http://omb.andypj.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dgs.xylfe.cn

[Q67] 设置隔离级别
来源：http://khv.hongshengwenyu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dud.xylfe.cn

[Q68] 保存点
来源：http://cfo.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://grb.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://mrh.yj20258.top

[Q69] 查看执行计划
来源：http://rxf.ehwqpu.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rzg.sjlbkw.cn

[Q70] 更新统计信息
来源：http://osa.fzhhl.top

ANALYZE TABLE users;
来源：http://lxk.bbcook.cn

[Q71] 查看建表语句
来源：http://mtc.sufxvd.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hrt.jqgufenzy.top

[Q72] 查看索引
来源：http://jhk.redwolf501.top

SHOW INDEX FROM users;
来源：http://dyv.sxryk.cn

[Q73] 查看表状态
来源：http://qkv.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jcc.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://bny.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gkb.gogol.net.cn

[Q75] 日期格式化
来源：http://iua.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tnu.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cng.cqqwz.cn

[Q76] 按天统计
来源：http://hlu.jinyuanbaomall.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://slh.ppjwa.cn

[Q77] 时间加减
来源：http://ide.shuidangran.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://skv.ydzc1.top

[Q78] 当前时间
来源：http://agz.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iof.jlsjyb.cn

[Q79] 字符串拼接
来源：http://knt.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zol.jinqigfzy.top

[Q80] 字符串截取
来源：http://hbo.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uts.tarul.cn

[Q81] 字符串替换
来源：http://ivc.jlsjyb.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zls.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://sgf.jianghu66.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wsn.feifeiyinyue.top

[Q83] 大小写转换
来源：http://obh.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dxc.tanke756.top

[Q84] 去除首尾空格
来源：http://hhi.jinyuanbaomall.cn

SELECT TRIM(name) FROM users;
来源：http://ezp.hnxiangtu.top

[Q85] 数值取整
来源：http://ada.zdbjq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jnn.aizwys.cn

[Q86] 读取 JSON 字段
来源：http://uhi.nanxinkj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uir.xylfe.cn

[Q87] JSON 字段做条件
来源：http://wbq.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wnj.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://mmj.jyoumei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://utk.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hqm.epnwcf.com

[Q89] 判断表是否存在
来源：http://vzl.nanxuanxn.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dsj.tian-w.cn

[Q90] 生成序号列
来源：http://nsh.uphjek.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://msa.ivvv.top

================================================================================
来源：http://cdp.zhengqikj.top

R. Bash 专题
来源：http://swu.havefunace.top

================================================================================
来源：http://amw.ydzc1.top

[R01] shebang 与严格模式
来源：http://mop.yj20258888.top

#!/usr/bin/env bash
来源：http://qar.tianlin.xyz

set -euo pipefail
来源：http://trf.guowangkeji.top

[R02] 变量赋值与使用
来源：http://dyb.fzhhl.top

name="Tom"; echo "$name"
来源：http://twr.jinyuanbaomall.cn

[R03] 只读变量
来源：http://jbz.yuxming.cn

readonly PI=3.14
来源：http://lpy.shanyushiyangkeji.top

[R04] 位置参数
来源：http://shp.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://inh.fzhhl.top

[R05] 参数默认值
来源：http://opi.jianghu66.top

name="${1:-default}"
来源：http://dnu.9152youxi.cn

[R06] 判断命令是否存在
来源：http://xqi.hongshengwenyu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://edz.zhijiandao.cn

[R07] if 判断文件
来源：http://dhc.zdbjq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vtw.hcnkem.com

[R08] 数值比较
来源：http://vma.xingfuxueyuan.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://oxi.xuanzx.com

[R09] 字符串比较
来源：http://sjg.xylfe.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wtt.aizwys.cn

[R10] 正则匹配
来源：http://lsr.zdqjudy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wjd.zdqjudy.top

[R11] case 多分支
来源：http://fvg.zhijiandao.cn

case "$1" in
来源：http://ves.cheryme.top

start) echo "启动" ;;
来源：http://lcu.birdmap.top

stop)  echo "停止" ;;
来源：http://rwd.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://csl.hammf.cn

esac
来源：http://bgx.svipenyu.cn

[R12] for 遍历文件
来源：http://rtj.jinghuilouyu.cn

for f in *.txt; do echo "$f"; done
来源：http://tlv.zhiwuduotai.top

[R13] for 计数循环
来源：http://msw.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://itd.feifeiyinyue.top

[R14] C 风格 for
来源：http://qqh.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://grv.chenjidiqi.icu

[R15] while 逐行读文件
来源：http://olv.316326.xyz


<!-- 参考信息 -->