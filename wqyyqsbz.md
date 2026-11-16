代发 wailian999

[P01] 生成 UUID
来源：http://qcg.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://gwh.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mne.yanxiufei.cn

JS:   crypto.randomUUID()
来源：http://rfw.yueranfly.top

TS:   crypto.randomUUID()
来源：http://dkt.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://cve.hywenlv.cn

Go:   // 用 github.com/google/uuid
来源：http://tte.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://gfr.ppjwa.cn

C#:   Guid.NewGuid().ToString()
来源：http://xjg.c1oappe.top

[P02] MD5 / SHA256 摘要
来源：http://uxu.vehdjk.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qzq.andypj.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://kar.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xkn.snrcjt.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ysk.zhijiandao.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qhr.vqdsnc.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kcx.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xos.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://grw.gzhubu.top

[P03] 生成短随机字符串
来源：http://opl.cashguo.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pgt.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kgy.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://feu.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jub.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sds.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uqv.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ebt.yangfankeji.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://srz.yj20258.top

[P04] 求长度
来源：http://whv.jqgfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dpp.snrcjt.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vug.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xmg.52xcode.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gtd.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://kva.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://nif.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://bjx.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hsf.shzxlz.cn

[P05] 判断两个对象内容是否相等
来源：http://vpu.svipenyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xfd.gotoacloud.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tnh.bbcook.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yyp.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://guu.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bzp.fktsv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ily.andypj.xyz

Ruby: a == b
来源：http://kad.ywan-chungtsiang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zfs.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zjm.zhiwuduotai.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xkn.daxiang520.top

PHP:  if (empty($x)) {}
来源：http://bca.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rrb.0kj1m.cn

TS:   if (x == null) {}
来源：http://hud.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vwf.xylfe.cn

Go:   if x == nil {}
来源：http://cfx.fanxiaobao.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gcm.gotoacloud.top

C#:   if (x is null) {}
来源：http://ywp.andypj.xyz

[P07] 防抖与节流
来源：http://tvl.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fvw.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://gxy.xylfe.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jdg.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xaa.ydzc1.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://roi.ehwqpu.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://avj.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xmt.jiagoushi.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gvl.yuxming.cn

[P08] 处理浮点精度问题
来源：http://qni.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://crv.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ikp.zdbjq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ixi.zdbjq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ynz.feifeiyinyue.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ydf.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fly.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jhz.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wei.pengpengdd.cyou

================================================================================
来源：http://hya.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hah.pengpengdd.cyou

================================================================================
来源：http://xnj.havefunace.top

[Q01] 创建表
来源：http://zui.havefunace.top

CREATE TABLE users (
来源：http://xwm.jinghuilouyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gdn.jiagoushi.top

name VARCHAR(50) NOT NULL,
来源：http://plj.cucudq.cn

email VARCHAR(100) UNIQUE,
来源：http://kqr.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://elk.jinqigfzy.top

);
来源：http://ozl.shuidangran.top

[Q02] 创建带外键的表
来源：http://wlf.gogol.net.cn

CREATE TABLE orders (
来源：http://ugc.yangfankeji.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xby.feifeiyinyue.top

user_id INT NOT NULL,
来源：http://mek.gaohongyu789.top

amount DECIMAL(10, 2),
来源：http://vph.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wlt.316326.xyz

);
来源：http://twb.yongpay.top

[Q03] 增加列
来源：http://qtw.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://snb.pycfn.com

[Q04] 修改列类型
来源：http://fju.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vub.yongpay.top

[Q05] 重命名列
来源：http://evr.chenjidiqi.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cqe.fengsongda.top

[Q06] 删除列
来源：http://xia.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://nlj.daria6918.cn

[Q07] 删除表
来源：http://gyw.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://qis.fehbvm.com

[Q08] 创建普通索引
来源：http://mqx.yuanzhike.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fxd.cheryme.top

[Q09] 创建唯一索引
来源：http://ycg.sweek.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sgh.hnqzz.top

[Q10] 插入单行
来源：http://iap.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vjo.nwbrower.top

[Q11] 一次插入多行
来源：http://rta.daria6918.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sqq.svipenyu.cn

[Q12] 插入后取自增 ID
来源：http://unv.quarkkingdee.top

INSERT INTO users (name) VALUES ('C');
来源：http://zfp.jyoumei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qvf.gotoacloud.top

[Q13] 忽略重复插入
来源：http://oza.ehwqpu.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rgh.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://zrs.yuanzhike.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://faz.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://spk.wangdashe.top

[Q15] 查询全部
来源：http://wec.zhengqikj.top

SELECT * FROM users;
来源：http://cvj.xylfe.cn

[Q16] 查询指定列
来源：http://yqm.ivvv.top

SELECT id, name FROM users;
来源：http://xmk.jinghuilouyu.cn

[Q17] 条件查询
来源：http://uar.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aex.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://zhh.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gdf.tanke756.top

[Q19] 范围查询
来源：http://lzu.ppjwa.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jdy.hongshengwenyu.top

[Q20] IN 列表
来源：http://zxd.yanxiufei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zbh.zhengqikj.top

[Q21] 空值判断
来源：http://myj.vqdsnc.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jpv.shangyingyoupin.top

[Q22] 排序
来源：http://azf.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fhj.svipenyu.cn

[Q23] 分页
来源：http://ptv.hnxiangtu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fsi.cucudq.cn

[Q24] 去重
来源：http://fqn.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://xuo.yongpay.top

[Q25] 只取前 N 条
来源：http://psp.sxryk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aht.yj20258888.top

[Q26] 计数
来源：http://mfb.hnqzz.top

SELECT COUNT(*) FROM users;
来源：http://ntd.zhoulong.xyz

[Q27] 条件计数
来源：http://qit.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://div.tianlin.xyz

[Q28] 求和与平均
来源：http://xop.sufxvd.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rqm.vehdjk.com

[Q29] 最大最小值
来源：http://fng.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pqi.cheryme.top

[Q30] 分组统计
来源：http://wjx.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ejj.guowangkeji.top

[Q31] 分组后过滤
来源：http://fkf.zhoulong.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://koh.ppjwa.cn

[Q32] 分组拼接字符串
来源：http://vwz.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sdy.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zuv.ybcxt.top

[Q33] 多列分组
来源：http://pfj.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ppj.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://mau.jlsjyb.cn

SELECT * FROM (
来源：http://ful.zycfv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jci.aizwys.cn

) t WHERE rn = 1;
来源：http://xbt.jqgfzy.top

[Q35] 内连接
来源：http://zbh.zhengqikj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hew.cheryme.top

[Q36] 左连接
来源：http://gzk.gaohongyu789.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://utw.tanke756.top

[Q37] 右连接
来源：http://mhk.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dlu.c1oappe.top

[Q38] 全外连接（PostgreSQL）
来源：http://jws.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bkk.jinqigufen.top

[Q39] 自连接（查上下级）
来源：http://biv.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lmy.sjlbkw.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ukn.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hzd.xinyue.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rdz.ehwqpu.com

[Q41] 多表连接
来源：http://awg.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://qpi.yuanzhike.top

JOIN users u ON u.id = o.user_id
来源：http://wrp.yonumen.top

JOIN products p ON p.id = o.product_id;
来源：http://nif.hywenlv.cn

[Q42] 连接条件附加过滤
来源：http://gkh.cdnleiting.top

SELECT u.name, o.amount FROM users u
来源：http://mfw.birdmap.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vxe.chenzaomai.com

[Q43] 标量子查询
来源：http://euy.xuetiantiany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zlu.kuanghao11.cn

[Q44] IN 子查询
来源：http://shr.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bmv.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://iuq.jyoumei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kqi.jyoumei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wse.fzhhl.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pqe.xylfe.cn

[Q47] 与平均值比较
来源：http://yhm.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pge.jinyuanbaomall.cn

[Q48] CTE 公用表表达式
来源：http://pzx.tianlin.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dhg.shanyushiyangtech.top

SELECT * FROM t WHERE c > 5;
来源：http://vts.dianchejie.cn

[Q49] 更新单行
来源：http://kmn.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lrj.yongpay.top

[Q50] 批量更新
来源：http://pcg.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hnk.hfpthk.cn

[Q51] 用子查询更新
来源：http://cjn.dianchejie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ibw.ywan-chungtsiang.top

[Q52] 删除指定行
来源：http://var.cashguo.top

DELETE FROM users WHERE id = 10;
来源：http://cmu.yj20258.top

[Q53] 按条件删除
来源：http://jjd.c1oappe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rsr.ywan-chungtsiang.top

[Q54] 清空表
来源：http://qov.jianghu66.top

TRUNCATE TABLE logs;
来源：http://xxd.yj20258888.top

[Q55] 排名（并列占位）
来源：http://xyw.zhengqikj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ctw.jinqigfzy.top

[Q56] 密集排名（并列不占位）
来源：http://wxi.sjlbkw.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tgp.hammf.cn

[Q57] 行号
来源：http://uxe.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://swg.aibaodan.cn

[Q58] 累计求和
来源：http://qdk.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://geb.hysaishi.cn

[Q59] 分组内累计
来源：http://iyr.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zni.ctjpmb.com

[Q60] 取上一行 / 下一行
来源：http://hpp.vqdsnc.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ewh.sufxvd.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dyv.quarkkingdee.top

[Q61] 移动平均
来源：http://vfx.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ejo.vqdsnc.cn

[Q62] 分组占比
来源：http://mbr.hnqzz.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cqu.sweek.top

[Q63] 开启事务
来源：http://lxe.meibo888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://soe.zdqjudy.top

[Q64] 提交事务
来源：http://ezh.yongpay.top

COMMIT;
来源：http://jvf.sxryk.cn

[Q65] 回滚事务
来源：http://yck.cdnleiting.top

ROLLBACK;
来源：http://snf.jqgfzy.top

[Q66] 行锁查询
来源：http://lgn.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ymp.bjfxy.top

[Q67] 设置隔离级别
来源：http://wle.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mis.hnqzz.top

[Q68] 保存点
来源：http://tsp.xuanzx.com

SAVEPOINT sp1;
来源：http://vbz.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://qxu.fehbvm.com

[Q69] 查看执行计划
来源：http://nbo.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://byc.fktsv.cn

[Q70] 更新统计信息
来源：http://oaa.zhixingplan.top

ANALYZE TABLE users;
来源：http://jym.fktsv.cn

[Q71] 查看建表语句
来源：http://iuh.birdmap.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hbd.chenzaomai.com

[Q72] 查看索引
来源：http://oyd.xziqi.cn

SHOW INDEX FROM users;
来源：http://lcz.hammf.cn

[Q73] 查看表状态
来源：http://ins.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gma.tanke756.top

[Q74] 强制使用索引
来源：http://toa.ppjwa.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zwl.aibaodan.cn

[Q75] 日期格式化
来源：http://umu.yj20258.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://byw.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://khy.svipenyu.cn

[Q76] 按天统计
来源：http://oul.chenjidiqi.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ofx.smart0.xyz

[Q77] 时间加减
来源：http://fym.cdnleiting.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hkq.gzhubu.top

[Q78] 当前时间
来源：http://qbd.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://izd.hfpthk.cn

[Q79] 字符串拼接
来源：http://wlp.jinqigufen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xsd.aizwys.cn

[Q80] 字符串截取
来源：http://jql.andypj.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iub.52xcode.cn

[Q81] 字符串替换
来源：http://fwn.yangfankeji.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cyj.nanxuanxn.top

[Q82] 字符长度与字节长度
来源：http://yce.shzxlz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dto.zycfv.cn

[Q83] 大小写转换
来源：http://mil.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ykr.9152youxi.cn

[Q84] 去除首尾空格
来源：http://iew.guannengcc.top

SELECT TRIM(name) FROM users;
来源：http://own.cqqwz.cn

[Q85] 数值取整
来源：http://cew.fehbvm.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zba.tarul.cn

[Q86] 读取 JSON 字段
来源：http://hoz.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ltf.bbcook.cn

[Q87] JSON 字段做条件
来源：http://lsn.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wzf.sufxvd.cn

[Q88] 行转列（条件聚合）
来源：http://eby.iojbl.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uxs.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://twv.xuanzx.com

[Q89] 判断表是否存在
来源：http://lou.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sml.iojbl.cn

[Q90] 生成序号列
来源：http://oif.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sjv.jianghu66.top

================================================================================
来源：http://dnb.hongshengwenyu.top

R. Bash 专题
来源：http://nho.hnxiangtu.top

================================================================================
来源：http://cow.fzhhl.top

[R01] shebang 与严格模式
来源：http://pgp.ppjwa.cn

#!/usr/bin/env bash
来源：http://szy.bbcook.cn

set -euo pipefail
来源：http://hvn.yj20258.top

[R02] 变量赋值与使用
来源：http://qhv.yangfankeji.com

name="Tom"; echo "$name"
来源：http://bwl.jinyuanbaomall.cn

[R03] 只读变量
来源：http://ykk.jinyuanbaomall.cn

readonly PI=3.14
来源：http://ofi.quarkkingdee.top

[R04] 位置参数
来源：http://ber.9152youxi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lyv.cucudq.cn

[R05] 参数默认值
来源：http://hpr.wangdashe.top

name="${1:-default}"
来源：http://tet.9152youxi.cn

[R06] 判断命令是否存在
来源：http://qkp.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cgu.havefunace.top

[R07] if 判断文件
来源：http://kaq.jqgufenzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rfu.hysaishi.cn

[R08] 数值比较
来源：http://nxe.chenlongwang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cqx.bjfxy.top

[R09] 字符串比较
来源：http://cgl.cdnleiting.top


<!-- 参考信息 -->