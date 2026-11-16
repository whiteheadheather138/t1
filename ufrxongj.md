代发 wailian999

TS:   crypto.randomUUID()
来源：http://gby.haohaochexian.top

Java: UUID.randomUUID().toString()
来源：http://ygm.316326.xyz

Go:   // 用 github.com/google/uuid
来源：http://krq.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://ido.ydjk.org.cn

C#:   Guid.NewGuid().ToString()
来源：http://sdg.ybcxt.top

[P02] MD5 / SHA256 摘要
来源：http://csh.nanxuanxn.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pns.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mkl.pengpengdd.cyou

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gbd.gzhubu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rjb.xylfe.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qyw.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gpk.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://peb.pycfn.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aca.nanxuanxn.top

[P03] 生成短随机字符串
来源：http://ith.iojbl.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kfs.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://srf.fehbvm.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qqi.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iyz.xingfuxueyuan.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yjl.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jkl.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://uwi.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rzs.52xcode.cn

[P04] 求长度
来源：http://fcq.sxryk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mil.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tzf.hcnkem.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pep.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fjd.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://mvw.jianghu66.top

Go:   len(arr);  len(m)
来源：http://tbu.tanke756.top

Ruby: x.length;  x.size
来源：http://njm.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ywl.xylfe.cn

[P05] 判断两个对象内容是否相等
来源：http://umi.ehwqpu.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://xkt.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ubu.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vqa.andypj.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://siy.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lud.fktsv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://asu.0kj1m.cn

Ruby: a == b
来源：http://ebk.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mcu.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://icm.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wir.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://gbo.xuetiantiany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cfd.bbcook.cn

TS:   if (x == null) {}
来源：http://iwt.wangdashe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yek.xziqi.cn

Go:   if x == nil {}
来源：http://cpc.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gtv.zhiwuduotai.top

C#:   if (x is null) {}
来源：http://thu.xuetiantiany.cn

[P07] 防抖与节流
来源：http://ssg.iojbl.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gvs.tian-w.cn

PHP:  // 手写时间戳比较
来源：http://vao.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vff.sysykeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wnb.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gby.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ckz.jinqigufen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ffq.chenlongwang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bfw.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://klc.xingfuxueyuan.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xdv.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://raz.ppjwa.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gev.shangyingyoupin.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://agb.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hlf.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pjn.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ven.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qhe.zhixingplan.top

================================================================================
来源：http://vqw.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gdv.c1oappe.top

================================================================================
来源：http://gql.xingfuxueyuan.xyz

[Q01] 创建表
来源：http://osi.havefunace.top

CREATE TABLE users (
来源：http://eco.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xbs.cheryme.top

name VARCHAR(50) NOT NULL,
来源：http://ucd.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://ohe.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nsy.chenlongwang.top

);
来源：http://mma.ydzc1.top

[Q02] 创建带外键的表
来源：http://kxl.aizwys.cn

CREATE TABLE orders (
来源：http://kxa.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://txz.jinqigufen.top

user_id INT NOT NULL,
来源：http://vka.kuanghao11.cn

amount DECIMAL(10, 2),
来源：http://qht.316326.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ico.chenjidiqi.icu

);
来源：http://bpl.shanyushiyangtech.top

[Q03] 增加列
来源：http://osy.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kol.aizwys.cn

[Q04] 修改列类型
来源：http://yxs.iojbl.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vsr.redwolf501.top

[Q05] 重命名列
来源：http://qok.yangfankeji.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://obu.ctjpmb.com

[Q06] 删除列
来源：http://khv.aizwys.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jow.guowangkeji.top

[Q07] 删除表
来源：http://ppv.ctjpmb.com

DROP TABLE IF EXISTS orders;
来源：http://tdr.jqgfzy.top

[Q08] 创建普通索引
来源：http://llq.pengpengdd.cyou

CREATE INDEX idx_users_email ON users(email);
来源：http://gsn.aibaodan.cn

[Q09] 创建唯一索引
来源：http://bti.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mij.aibaodan.cn

[Q10] 插入单行
来源：http://wcr.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xsf.dashuyun.cn

[Q11] 一次插入多行
来源：http://nbt.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cnd.vehdjk.com

[Q12] 插入后取自增 ID
来源：http://dqy.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xnn.tianlin.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gbn.hesvh.cn

[Q13] 忽略重复插入
来源：http://old.haohaochexian.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ytp.mhx1999.top

[Q14] 存在则更新（upsert）
来源：http://dcc.hywenlv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nql.zhijiandao.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fsz.mhx1999.top

[Q15] 查询全部
来源：http://dqs.xuanzx.com

SELECT * FROM users;
来源：http://fjo.yj20258888.top

[Q16] 查询指定列
来源：http://ixk.fengsongda.top

SELECT id, name FROM users;
来源：http://roa.gaohongyu789.top

[Q17] 条件查询
来源：http://lzt.fktsv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rhu.cucudq.cn

[Q18] 模糊匹配
来源：http://ejc.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lmu.jinqigufen.top

[Q19] 范围查询
来源：http://ffr.haohaochexian.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ktd.c1oappe.top

[Q20] IN 列表
来源：http://eea.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://acb.hongshengwenyu.top

[Q21] 空值判断
来源：http://xyy.iojbl.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aoh.sjlbkw.cn

[Q22] 排序
来源：http://psr.chenjidiqi.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mvk.wangshuangyany.cn

[Q23] 分页
来源：http://vvs.jqgfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oex.cucudq.cn

[Q24] 去重
来源：http://uvu.jqgfzy.top

SELECT DISTINCT city FROM users;
来源：http://tvj.quarkkingdee.top

[Q25] 只取前 N 条
来源：http://iqy.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dxx.gaohongyu789.top

[Q26] 计数
来源：http://nxz.cashguo.top

SELECT COUNT(*) FROM users;
来源：http://moj.zycfv.cn

[Q27] 条件计数
来源：http://ule.9152youxi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://arc.fehbvm.com

[Q28] 求和与平均
来源：http://iou.aizwys.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xhe.zdqjudy.top

[Q29] 最大最小值
来源：http://zvz.aizwys.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gvh.hcnkem.com

[Q30] 分组统计
来源：http://rnb.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rky.nanxuanxn.top

[Q31] 分组后过滤
来源：http://fnb.aibaodan.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aoz.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://jrf.yuxming.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xjo.ivvv.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://axg.daxiang520.top

[Q33] 多列分组
来源：http://efb.ydzc1.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oja.tarul.cn

[Q34] 每组取第一条
来源：http://dvc.jqgufenzy.top

SELECT * FROM (
来源：http://vtc.svipenyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qph.yuxming.cn

) t WHERE rn = 1;
来源：http://jez.vehdjk.com

[Q35] 内连接
来源：http://drp.chenzaomai.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ihq.xziqi.cn

[Q36] 左连接
来源：http://yna.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wdm.jyoumei.cn

[Q37] 右连接
来源：http://yxv.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://evu.guannengcc.top

[Q38] 全外连接（PostgreSQL）
来源：http://fxc.zycfv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://diq.tarul.cn

[Q39] 自连接（查上下级）
来源：http://nam.yj20258888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://red.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vts.sxryk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ufw.nwbrower.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pad.xylfe.cn

[Q41] 多表连接
来源：http://ffd.zdbjq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qnh.c1oappe.top

JOIN users u ON u.id = o.user_id
来源：http://fyk.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://rmk.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://swr.cucudq.cn

SELECT u.name, o.amount FROM users u
来源：http://fua.havefunace.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://skt.redwolf501.top

[Q43] 标量子查询
来源：http://dca.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nyt.hfpthk.cn

[Q44] IN 子查询
来源：http://zvv.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pwb.yonumen.top

[Q45] EXISTS 判断存在
来源：http://eja.xuetiantiany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qof.zhongyouzk.top

[Q46] NOT EXISTS 判断不存在
来源：http://axz.hfpthk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://otk.zhoulong.xyz

[Q47] 与平均值比较
来源：http://wau.gaohongyu789.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mew.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://oju.haohaochexian.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vei.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://wyq.jqgufenzy.top

[Q49] 更新单行
来源：http://mxn.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sxp.kuanghao11.cn

[Q50] 批量更新
来源：http://bzo.zdqjudy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wgp.ivvv.top

[Q51] 用子查询更新
来源：http://fem.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tqo.hesvh.cn

[Q52] 删除指定行
来源：http://juj.zhoulong.xyz

DELETE FROM users WHERE id = 10;
来源：http://imr.yangfankeji.com

[Q53] 按条件删除
来源：http://yjg.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nim.guowangkeji.top

[Q54] 清空表
来源：http://wob.chenzaomai.com

TRUNCATE TABLE logs;
来源：http://njz.yj20258888.top

[Q55] 排名（并列占位）
来源：http://ypw.snrcjt.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xjf.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://ide.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bkc.52xcode.cn

[Q57] 行号
来源：http://mum.jiagoushi.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wfb.hysaishi.cn

[Q58] 累计求和
来源：http://dpx.shzxlz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pch.daxiang520.top

[Q59] 分组内累计
来源：http://bqi.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kis.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://ikw.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xao.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mif.wangdashe.top

[Q61] 移动平均
来源：http://xzb.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yay.redwolf501.top

[Q62] 分组占比
来源：http://xtc.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hrr.ctjpmb.com

[Q63] 开启事务
来源：http://hhj.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jlv.mhx1999.top

[Q64] 提交事务
来源：http://ssh.gzhubu.top

COMMIT;
来源：http://brp.sweek.top

[Q65] 回滚事务
来源：http://ihh.yfazqb.com

ROLLBACK;
来源：http://idt.hesvh.cn

[Q66] 行锁查询
来源：http://rew.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xen.bbcook.cn

[Q67] 设置隔离级别
来源：http://cid.sweek.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://djt.fzhhl.top

[Q68] 保存点
来源：http://gdk.aibaodan.cn

SAVEPOINT sp1;
来源：http://low.wangdashe.top

ROLLBACK TO sp1;
来源：http://xjb.cucudq.cn

[Q69] 查看执行计划
来源：http://bxm.sjlbkw.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gxb.nanxinkj.top

[Q70] 更新统计信息
来源：http://leh.cheryme.top

ANALYZE TABLE users;
来源：http://jgd.hammf.cn

[Q71] 查看建表语句
来源：http://spd.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://box.xuetiantiany.cn

[Q72] 查看索引
来源：http://hjc.iojbl.cn

SHOW INDEX FROM users;
来源：http://fgm.fzhhl.top

[Q73] 查看表状态
来源：http://bzw.chenzaomai.com

SHOW TABLE STATUS LIKE 'users';
来源：http://mis.kuanghao11.cn

[Q74] 强制使用索引
来源：http://zbb.gotoacloud.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ypd.jinqigufen.top

[Q75] 日期格式化
来源：http://oij.daria6918.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xub.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ctw.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://xyu.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uul.birdmap.top

[Q77] 时间加减
来源：http://afl.pycfn.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tgw.tianlin.xyz

[Q78] 当前时间
来源：http://dfp.yongpay.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pys.fehbvm.com

[Q79] 字符串拼接
来源：http://sox.pycfn.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ekn.c1oappe.top

[Q80] 字符串截取
来源：http://adx.cheryme.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://znc.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://huh.daxiang520.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://alp.yvedp.cn

[Q82] 字符长度与字节长度
来源：http://noe.hesvh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aam.fengsongda.top

[Q83] 大小写转换
来源：http://twg.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eoh.yj202588.top

[Q84] 去除首尾空格
来源：http://nrc.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://yga.yonumen.top

[Q85] 数值取整
来源：http://hqt.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gsk.wangshuangyany.cn

[Q86] 读取 JSON 字段
来源：http://wnb.sjlbkw.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dbr.tian-w.cn

[Q87] JSON 字段做条件
来源：http://wgm.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://agv.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://hdd.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lcq.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mys.316326.xyz

[Q89] 判断表是否存在
来源：http://qmr.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bby.shanyushiyangtech.top

[Q90] 生成序号列
来源：http://nwv.yangfankeji.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rxg.316326.xyz

================================================================================
来源：http://hjc.daria6918.cn

R. Bash 专题
来源：http://tab.sweek.top

================================================================================
来源：http://wus.yj20258.top

[R01] shebang 与严格模式
来源：http://ima.xingfuxueyuan.xyz

#!/usr/bin/env bash
来源：http://rlw.snrcjt.cn

set -euo pipefail
来源：http://jji.yj20258.top

[R02] 变量赋值与使用
来源：http://gpl.mhx1999.top

name="Tom"; echo "$name"
来源：http://onq.xinyue.icu

[R03] 只读变量
来源：http://fiz.tian-w.cn

readonly PI=3.14
来源：http://inw.ywan-chungtsiang.top

[R04] 位置参数
来源：http://rki.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xtc.yueranfly.top

[R05] 参数默认值
来源：http://oax.wangshuangyany.cn

name="${1:-default}"
来源：http://oco.snrcjt.cn

[R06] 判断命令是否存在
来源：http://rdv.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rpr.zhengqikj.top

[R07] if 判断文件
来源：http://flh.pycfn.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jrk.yuanzhike.top

[R08] 数值比较
来源：http://pir.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vxf.smart0.xyz

[R09] 字符串比较
来源：http://xix.bjfxy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nbj.shanyushiyangtech.top

[R10] 正则匹配
来源：http://eqc.uphjek.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://osv.tanke756.top

[R11] case 多分支
来源：http://equ.tarul.cn


<!-- 参考信息 -->