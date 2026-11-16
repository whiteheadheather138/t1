代发 wailian999

C#:   Parallel.For
来源：http://saa.andypj.xyz

================================================================================
来源：http://lti.sysykeji.top

P. 常用工具函数
来源：http://xwt.hammf.cn

================================================================================
来源：http://hkg.hysaishi.cn

[P01] 生成 UUID
来源：http://wzd.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://oem.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jvb.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://mcn.jiagoushi.top

TS:   crypto.randomUUID()
来源：http://ekm.hfpthk.cn

Java: UUID.randomUUID().toString()
来源：http://yyt.zhiwuduotai.top

Go:   // 用 github.com/google/uuid
来源：http://zze.dianchejie.cn

Ruby: SecureRandom.uuid
来源：http://ffy.meibo888.top

C#:   Guid.NewGuid().ToString()
来源：http://ggg.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://gqa.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://isn.tanke756.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hem.yonumen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oyi.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wun.aibaodan.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fqn.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fse.sxryk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sox.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jjb.cheryme.top

[P03] 生成短随机字符串
来源：http://oyd.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zzr.nanxinkj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vfh.hcnkem.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fng.zhoulong.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://enr.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://osl.yanxiufei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eyq.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mfp.daxiang520.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yky.fehbvm.com

[P04] 求长度
来源：http://hxo.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://krv.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xec.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://awd.sxryk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nyo.hywenlv.cn

Java: list.size();  map.size();  s.length()
来源：http://xji.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://hxy.yj202588.top

Ruby: x.length;  x.size
来源：http://ytn.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://eav.fehbvm.com

[P05] 判断两个对象内容是否相等
来源：http://vlc.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gbm.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pyq.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hki.dianchejie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rwf.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dph.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://wap.bbcook.cn

Ruby: a == b
来源：http://qsk.jinghuilouyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lqy.hongshengwenyu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://toe.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://djc.yongpay.top

PHP:  if (empty($x)) {}
来源：http://imw.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://udw.epnwcf.com

TS:   if (x == null) {}
来源：http://oah.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hhf.aibaodan.cn

Go:   if x == nil {}
来源：http://sdp.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wqn.fzhhl.top

C#:   if (x is null) {}
来源：http://krn.316326.xyz

[P07] 防抖与节流
来源：http://ska.zdqjudy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rjm.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://awu.mhx1999.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://axj.guannengcc.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rno.tian-w.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hmi.ywan-chungtsiang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ywz.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mqa.birdmap.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ymv.cqqwz.cn

[P08] 处理浮点精度问题
来源：http://voo.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jvi.ydjk.org.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ttv.jinqigufen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://izu.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wjl.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rqi.zhengqikj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eqi.jianghu66.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iif.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nhx.bbcook.cn

================================================================================
来源：http://tjz.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lpa.nanxinkj.top

================================================================================
来源：http://qey.shuidangran.top

[Q01] 创建表
来源：http://qct.zycfv.cn

CREATE TABLE users (
来源：http://gtu.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bgu.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://gcp.wangshuangyany.cn

email VARCHAR(100) UNIQUE,
来源：http://ucj.gaohongyu789.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://orw.jinqigfzy.top

);
来源：http://zyu.yonumen.top

[Q02] 创建带外键的表
来源：http://erk.zdbjq.cn

CREATE TABLE orders (
来源：http://gyx.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sfh.ybcxt.top

user_id INT NOT NULL,
来源：http://hsq.yj20258888.top

amount DECIMAL(10, 2),
来源：http://lfu.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tri.jqgufenzy.top

);
来源：http://mje.birdmap.top

[Q03] 增加列
来源：http://rfu.yfazqb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qua.zycfv.cn

[Q04] 修改列类型
来源：http://cpi.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kcg.jqgufenzy.top

[Q05] 重命名列
来源：http://urw.fzhhl.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nir.xingfuxueyuan.xyz

[Q06] 删除列
来源：http://kge.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://iyp.uphjek.com

[Q07] 删除表
来源：http://gff.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://lac.gogol.net.cn

[Q08] 创建普通索引
来源：http://knr.mhx1999.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wjc.chenlongwang.top

[Q09] 创建唯一索引
来源：http://ybz.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dwh.zycfv.cn

[Q10] 插入单行
来源：http://fxx.fehbvm.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ptw.jinghuilouyu.cn

[Q11] 一次插入多行
来源：http://ega.yj20258888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qmg.xuanzx.com

[Q12] 插入后取自增 ID
来源：http://fer.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sss.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fuf.gotoacloud.top

[Q13] 忽略重复插入
来源：http://uyi.zdbjq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uev.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://zoi.cashguo.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pwh.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://igd.iojbl.cn

[Q15] 查询全部
来源：http://plu.hfpthk.cn

SELECT * FROM users;
来源：http://prt.yuxming.cn

[Q16] 查询指定列
来源：http://typ.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://bew.jinqigfzy.top

[Q17] 条件查询
来源：http://atu.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qqv.fehbvm.com

[Q18] 模糊匹配
来源：http://bpo.daxiang520.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dxe.kuanghao11.cn

[Q19] 范围查询
来源：http://aud.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eez.316326.xyz

[Q20] IN 列表
来源：http://zve.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ouy.vqdsnc.cn

[Q21] 空值判断
来源：http://zfm.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://gkv.xuanzx.com

[Q22] 排序
来源：http://scc.aizwys.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://teh.fanxiaobao.xyz

[Q23] 分页
来源：http://dgw.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lor.sweek.top

[Q24] 去重
来源：http://qkc.xuanzx.com

SELECT DISTINCT city FROM users;
来源：http://wdk.daria6918.cn

[Q25] 只取前 N 条
来源：http://aho.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cte.xinyue.icu

[Q26] 计数
来源：http://ifm.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://mwk.hongshengwenyu.top

[Q27] 条件计数
来源：http://mas.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://whi.ywan-chungtsiang.top

[Q28] 求和与平均
来源：http://xgo.zdbjq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gsc.sweek.top

[Q29] 最大最小值
来源：http://dta.yanxiufei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vbd.gotoacloud.top

[Q30] 分组统计
来源：http://rmt.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ofl.ybcxt.top

[Q31] 分组后过滤
来源：http://nzn.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://usj.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://lpq.jinqigfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://suf.tarul.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pzw.ivvv.top

[Q33] 多列分组
来源：http://spr.redwolf501.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hov.gaohongyu789.top

[Q34] 每组取第一条
来源：http://uld.guannengcc.top

SELECT * FROM (
来源：http://xmo.hongshengwenyu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gao.ctjpmb.com

) t WHERE rn = 1;
来源：http://gbg.zhixingplan.top

[Q35] 内连接
来源：http://kaf.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fkj.zhaomingkeji.xyz

[Q36] 左连接
来源：http://duz.yanxiufei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pev.chenlongwang.top

[Q37] 右连接
来源：http://qgz.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cfi.aizwys.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ebk.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://raf.hongshengwenyu.top

[Q39] 自连接（查上下级）
来源：http://avg.nanxinkj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rjk.hnxiangtu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fpn.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zpv.fzhhl.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bmf.wangshuangyany.cn

[Q41] 多表连接
来源：http://lel.hesvh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ekv.meibo888.top

JOIN users u ON u.id = o.user_id
来源：http://the.bbcook.cn

JOIN products p ON p.id = o.product_id;
来源：http://nru.ehwqpu.com

[Q42] 连接条件附加过滤
来源：http://fbg.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://fqk.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zqd.quarkkingdee.top

[Q43] 标量子查询
来源：http://kzz.dianchejie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jpl.xylfe.cn

[Q44] IN 子查询
来源：http://xrm.daria6918.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fqb.zhongyouzk.top

[Q45] EXISTS 判断存在
来源：http://hyk.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xsi.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://kwy.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vhj.quarkkingdee.top

[Q47] 与平均值比较
来源：http://vzx.jqgfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lma.tanke756.top

[Q48] CTE 公用表表达式
来源：http://dsg.yangfankeji.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ump.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://axr.vqdsnc.cn

[Q49] 更新单行
来源：http://epz.tian-w.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yvd.andypj.xyz

[Q50] 批量更新
来源：http://noy.vqdsnc.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pjo.xuetiantiany.cn

[Q51] 用子查询更新
来源：http://rci.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zsb.ctjpmb.com

[Q52] 删除指定行
来源：http://vkh.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://cyk.cheryme.top

[Q53] 按条件删除
来源：http://fxm.bbcook.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xyx.fktsv.cn

[Q54] 清空表
来源：http://lko.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://erm.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://hkk.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ajb.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://bys.smart0.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tov.ctjpmb.com

[Q57] 行号
来源：http://rle.52xcode.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zxf.shanyushiyangtech.top

[Q58] 累计求和
来源：http://blo.gotoacloud.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zlz.uphjek.com

[Q59] 分组内累计
来源：http://dis.aibaodan.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tzs.ehwqpu.com

[Q60] 取上一行 / 下一行
来源：http://zfk.fehbvm.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bwa.daxiang520.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pty.yuanzhike.top

[Q61] 移动平均
来源：http://kkg.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jui.zhiwuduotai.top

[Q62] 分组占比
来源：http://cbk.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jvb.tian-w.cn

[Q63] 开启事务
来源：http://jov.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kih.gogol.net.cn

[Q64] 提交事务
来源：http://sxl.pycfn.com

COMMIT;
来源：http://cuc.nanxuanxn.top

[Q65] 回滚事务
来源：http://zdj.yuxming.cn

ROLLBACK;
来源：http://hub.52xcode.cn

[Q66] 行锁查询
来源：http://wco.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kmf.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://gji.sufxvd.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dpa.jinghuilouyu.cn

[Q68] 保存点
来源：http://ynk.zhengqikj.top

SAVEPOINT sp1;
来源：http://bla.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://kya.yuanzhike.top

[Q69] 查看执行计划
来源：http://cfq.svipenyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nky.zdqjudy.top

[Q70] 更新统计信息
来源：http://fuh.bjfxy.top

ANALYZE TABLE users;
来源：http://kkc.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://rql.fengsongda.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hxy.birdmap.top

[Q72] 查看索引
来源：http://gfx.chenlongwang.top

SHOW INDEX FROM users;
来源：http://cdv.zhijiandao.cn

[Q73] 查看表状态
来源：http://zep.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ece.bbcook.cn

[Q74] 强制使用索引
来源：http://nku.sweek.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iaz.dianchejie.cn

[Q75] 日期格式化
来源：http://dyy.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://byi.yj20258888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bps.yvedp.cn

[Q76] 按天统计
来源：http://jdt.hnxiangtu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bml.tianlin.xyz

[Q77] 时间加减
来源：http://lzc.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nqe.jyoumei.cn

[Q78] 当前时间
来源：http://iaf.sjlbkw.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jld.guowangkeji.top

[Q79] 字符串拼接
来源：http://fuu.svipenyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bof.tanke756.top

[Q80] 字符串截取
来源：http://xib.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qgm.smart0.xyz

[Q81] 字符串替换
来源：http://vub.daxiang520.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dcf.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://hsi.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xqe.shzxlz.cn

[Q83] 大小写转换
来源：http://xie.yongpay.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yxx.ivvv.top

[Q84] 去除首尾空格
来源：http://ipg.wangshuangyany.cn

SELECT TRIM(name) FROM users;
来源：http://vbe.aizwys.cn

[Q85] 数值取整
来源：http://lhu.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eot.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://hdd.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://scg.zhongyouzk.top

[Q87] JSON 字段做条件
来源：http://qqk.hfpthk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wiq.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://glb.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qqr.shanyushiyangtech.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sem.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://dbq.xingfuxueyuan.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://szq.meibo888.top

[Q90] 生成序号列
来源：http://skf.epnwcf.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vpp.quarkkingdee.top

================================================================================
来源：http://nhf.nwbrower.top

R. Bash 专题
来源：http://txq.tarul.cn

================================================================================
来源：http://btf.yongpay.top

[R01] shebang 与严格模式
来源：http://vmg.cheryme.top

#!/usr/bin/env bash
来源：http://ejw.andypj.xyz

set -euo pipefail
来源：http://wip.zhiwuduotai.top

[R02] 变量赋值与使用
来源：http://htf.yangfankeji.com

name="Tom"; echo "$name"
来源：http://axq.316326.xyz

[R03] 只读变量
来源：http://tbf.gogol.net.cn

readonly PI=3.14
来源：http://knu.hnxiangtu.top

[R04] 位置参数
来源：http://pnn.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://agr.dianchejie.cn

[R05] 参数默认值
来源：http://zdo.svipenyu.cn

name="${1:-default}"
来源：http://nie.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://ytp.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kcn.hcnkem.com

[R07] if 判断文件
来源：http://bcy.316326.xyz


<!-- 参考信息 -->