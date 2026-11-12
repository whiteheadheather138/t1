代发 wailian999

TS:   // child_process / cluster 模块
来源：http://aas.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qit.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kac.xuetiantiany.cn

Ruby: // fork 块
来源：http://uvn.gzhubu.top

C#:   Parallel.For
来源：http://zvo.feifeiyinyue.top

================================================================================
来源：http://xrq.yfazqb.com

P. 常用工具函数
来源：http://ycs.nanxuanxn.top

================================================================================
来源：http://psl.dashuyun.cn

[P01] 生成 UUID
来源：http://upz.snrcjt.cn

Py:   str(uuid.uuid4())
来源：http://jxy.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://peu.wangshuangyany.cn

JS:   crypto.randomUUID()
来源：http://euz.gogol.net.cn

TS:   crypto.randomUUID()
来源：http://idh.cashguo.top

Java: UUID.randomUUID().toString()
来源：http://vli.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://agk.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://hzj.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://see.zhaomingkeji.xyz

[P02] MD5 / SHA256 摘要
来源：http://nhu.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kdm.hongshengwenyu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nwy.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ihf.zhengqikj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jhe.fzhhl.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qly.cheryme.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fkh.hongshengwenyu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ovy.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bdu.0kj1m.cn

[P03] 生成短随机字符串
来源：http://yed.xinyue.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nqj.xuanzx.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oev.hnxiangtu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ddh.sjlbkw.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oxb.jinqigfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ana.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kqt.jqgfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kex.zhoulong.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://enf.chenzaomai.com

[P04] 求长度
来源：http://hsz.jinghuilouyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vvx.yonumen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mry.fzhhl.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cap.hywenlv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://txp.sweek.top

Java: list.size();  map.size();  s.length()
来源：http://tal.quarkkingdee.top

Go:   len(arr);  len(m)
来源：http://jja.birdmap.top

Ruby: x.length;  x.size
来源：http://tmt.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://eea.ydzc1.top

[P05] 判断两个对象内容是否相等
来源：http://fdn.zhongyouzk.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cty.daxiang520.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hmq.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zrv.chenzaomai.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pze.smart0.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fxl.fanxiaobao.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://kdy.hongshengwenyu.top

Ruby: a == b
来源：http://gbp.snrcjt.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gha.zdqjudy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mwv.kuanghao11.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wqg.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://qhf.jinqigfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fkh.andypj.xyz

TS:   if (x == null) {}
来源：http://xcc.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ueh.jinqigfzy.top

Go:   if x == nil {}
来源：http://baq.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://moe.birdmap.top

C#:   if (x is null) {}
来源：http://gck.guannengcc.top

[P07] 防抖与节流
来源：http://sai.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wom.gogol.net.cn

PHP:  // 手写时间戳比较
来源：http://ohx.smart0.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tqy.gogol.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yyv.tarul.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iwn.kuanghao11.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ayd.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pmh.dianchejie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hnk.sufxvd.cn

[P08] 处理浮点精度问题
来源：http://yvf.uphjek.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://arh.cucudq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fjz.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ina.gogol.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kbt.birdmap.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uji.pycfn.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qpa.zhengqikj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lhd.ivvv.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eef.ydzc1.top

================================================================================
来源：http://wdy.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ndn.meibo888.top

================================================================================
来源：http://tjd.dashuyun.cn

[Q01] 创建表
来源：http://zaa.wangshuangyany.cn

CREATE TABLE users (
来源：http://ymx.jinghuilouyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lcv.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://vxu.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://fbo.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hhj.tanke756.top

);
来源：http://exd.birdmap.top

[Q02] 创建带外键的表
来源：http://ztg.ivvv.top

CREATE TABLE orders (
来源：http://mcr.sweek.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jqo.bjfxy.top

user_id INT NOT NULL,
来源：http://lbp.yj20258888.top

amount DECIMAL(10, 2),
来源：http://mpv.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ugc.sufxvd.cn

);
来源：http://qqo.hnqzz.top

[Q03] 增加列
来源：http://iye.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mcb.yonumen.top

[Q04] 修改列类型
来源：http://trt.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zbq.haohaochexian.top

[Q05] 重命名列
来源：http://ver.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qkp.svipenyu.cn

[Q06] 删除列
来源：http://ufe.ivvv.top

ALTER TABLE users DROP COLUMN age;
来源：http://nuu.uphjek.com

[Q07] 删除表
来源：http://ldg.cqqwz.cn

DROP TABLE IF EXISTS orders;
来源：http://gtc.hesvh.cn

[Q08] 创建普通索引
来源：http://nbu.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lka.yj202588.top

[Q09] 创建唯一索引
来源：http://ovs.ywan-chungtsiang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uxx.andypj.xyz

[Q10] 插入单行
来源：http://hik.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pyq.hnqzz.top

[Q11] 一次插入多行
来源：http://oyi.jinqigufen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yrk.uphjek.com

[Q12] 插入后取自增 ID
来源：http://grm.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jkq.gaohongyu789.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mfw.hysaishi.cn

[Q13] 忽略重复插入
来源：http://mvf.shzxlz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lep.gotoacloud.top

[Q14] 存在则更新（upsert）
来源：http://iyj.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dpw.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nih.gaohongyu789.top

[Q15] 查询全部
来源：http://jdt.nanxinkj.top

SELECT * FROM users;
来源：http://weq.yj20258.top

[Q16] 查询指定列
来源：http://ojq.ctjpmb.com

SELECT id, name FROM users;
来源：http://rhd.9152youxi.cn

[Q17] 条件查询
来源：http://bmh.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bjs.pengpengdd.cyou

[Q18] 模糊匹配
来源：http://axv.cashguo.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nbj.xuanzx.com

[Q19] 范围查询
来源：http://iaj.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rlm.yj20258.top

[Q20] IN 列表
来源：http://gns.ivvv.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rlo.sufxvd.cn

[Q21] 空值判断
来源：http://wbc.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ztt.hammf.cn

[Q22] 排序
来源：http://fur.zhongyouzk.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://brk.bbcook.cn

[Q23] 分页
来源：http://yth.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pgf.pengpengdd.cyou

[Q24] 去重
来源：http://jbn.ppjwa.cn

SELECT DISTINCT city FROM users;
来源：http://bgi.cheryme.top

[Q25] 只取前 N 条
来源：http://jwk.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dld.nanxinkj.top

[Q26] 计数
来源：http://khe.zhengqikj.top

SELECT COUNT(*) FROM users;
来源：http://toi.mhx1999.top

[Q27] 条件计数
来源：http://chz.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gfu.chenlongwang.top

[Q28] 求和与平均
来源：http://bgk.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dwa.guannengcc.top

[Q29] 最大最小值
来源：http://wgj.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dxa.hywenlv.cn

[Q30] 分组统计
来源：http://xic.cdnleiting.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nwz.52xcode.cn

[Q31] 分组后过滤
来源：http://pug.316326.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ubf.xuanzx.com

[Q32] 分组拼接字符串
来源：http://jax.snrcjt.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mff.hysaishi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rzl.jinqigfzy.top

[Q33] 多列分组
来源：http://pph.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://edo.yj20258.top

[Q34] 每组取第一条
来源：http://gmo.jinqigfzy.top

SELECT * FROM (
来源：http://fpv.yonumen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fbp.jinqigfzy.top

) t WHERE rn = 1;
来源：http://vhs.cdnleiting.top

[Q35] 内连接
来源：http://qut.redwolf501.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qfz.hywenlv.cn

[Q36] 左连接
来源：http://fls.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cix.shanyushiyangtech.top

[Q37] 右连接
来源：http://zrk.sjlbkw.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yct.sweek.top

[Q38] 全外连接（PostgreSQL）
来源：http://vfk.zhixingplan.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://upd.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://ezh.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gpy.hnxiangtu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ejg.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xfj.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qsl.sufxvd.cn

[Q41] 多表连接
来源：http://jnh.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gka.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://djm.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://ywg.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://ibj.zhiwuduotai.top

SELECT u.name, o.amount FROM users u
来源：http://okm.gaohongyu789.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xev.wangdashe.top

[Q43] 标量子查询
来源：http://tev.hysaishi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dpp.yongpay.top

[Q44] IN 子查询
来源：http://lgi.mhx1999.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gya.fehbvm.com

[Q45] EXISTS 判断存在
来源：http://xjl.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lge.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://xef.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xpa.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://oib.yonumen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mln.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://sxx.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iqz.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://iza.daxiang520.top

[Q49] 更新单行
来源：http://wim.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hcf.0kj1m.cn

[Q50] 批量更新
来源：http://tpx.kuanghao11.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bji.ydjk.org.cn

[Q51] 用子查询更新
来源：http://dfp.yangfankeji.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xos.ybcxt.top

[Q52] 删除指定行
来源：http://pkv.nanxuanxn.top

DELETE FROM users WHERE id = 10;
来源：http://mcg.feifeiyinyue.top

[Q53] 按条件删除
来源：http://zsb.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://liy.yj20258.top

[Q54] 清空表
来源：http://sjq.tian-w.cn

TRUNCATE TABLE logs;
来源：http://fwz.kuanghao11.cn

[Q55] 排名（并列占位）
来源：http://kkh.tianlin.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eib.hesvh.cn

[Q56] 密集排名（并列不占位）
来源：http://bzo.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qvh.shuidangran.top

[Q57] 行号
来源：http://lxm.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ocu.havefunace.top

[Q58] 累计求和
来源：http://alu.yuxming.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://acc.shanyushiyangkeji.top

[Q59] 分组内累计
来源：http://tvw.hesvh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zli.nwbrower.top

[Q60] 取上一行 / 下一行
来源：http://dpl.ctjpmb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://abk.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ytk.guannengcc.top

[Q61] 移动平均
来源：http://ctv.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rhz.zycfv.cn

[Q62] 分组占比
来源：http://npp.mhx1999.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yjf.zhoulong.xyz

[Q63] 开启事务
来源：http://sxn.shzxlz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kww.ehwqpu.com

[Q64] 提交事务
来源：http://xcq.smart0.xyz

COMMIT;
来源：http://ozi.pycfn.com

[Q65] 回滚事务
来源：http://dbc.cucudq.cn

ROLLBACK;
来源：http://yst.tanke756.top

[Q66] 行锁查询
来源：http://ydo.feifeiyinyue.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dzp.birdmap.top

[Q67] 设置隔离级别
来源：http://snr.hnqzz.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://guj.vehdjk.com

[Q68] 保存点
来源：http://fzy.xinyue.icu

SAVEPOINT sp1;
来源：http://vqz.fktsv.cn

ROLLBACK TO sp1;
来源：http://kob.fzhhl.top

[Q69] 查看执行计划
来源：http://vqd.mhx1999.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mvu.epnwcf.com

[Q70] 更新统计信息
来源：http://zaw.fzhhl.top

ANALYZE TABLE users;
来源：http://ehv.yj20258.top

[Q71] 查看建表语句
来源：http://xrq.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://slu.yangfankeji.com

[Q72] 查看索引
来源：http://kry.kuanghao11.cn

SHOW INDEX FROM users;
来源：http://kjz.tian-w.cn

[Q73] 查看表状态
来源：http://lzp.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lex.cheryme.top

[Q74] 强制使用索引
来源：http://wwd.hywenlv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://knz.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://xyo.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ajm.xuanzx.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ijq.fzhhl.top

[Q76] 按天统计
来源：http://emn.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://upa.c1oappe.top

[Q77] 时间加减
来源：http://mpi.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lfy.feifeiyinyue.top

[Q78] 当前时间
来源：http://myd.shuidangran.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://esd.jqgfzy.top

[Q79] 字符串拼接
来源：http://ynf.cdnleiting.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ouv.shanyushiyangkeji.top

[Q80] 字符串截取
来源：http://dcf.nanxuanxn.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ess.jianghu66.top

[Q81] 字符串替换
来源：http://wnk.daxiang520.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://val.tanke756.top

[Q82] 字符长度与字节长度
来源：http://hva.hcnkem.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jbu.fehbvm.com

[Q83] 大小写转换
来源：http://qen.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://spf.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://lzb.jinqigufen.top

SELECT TRIM(name) FROM users;
来源：http://aue.haohaochexian.top

[Q85] 数值取整
来源：http://pex.yuanzhike.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pod.guowangkeji.top

[Q86] 读取 JSON 字段
来源：http://ctz.zhongyouzk.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wdq.havefunace.top

[Q87] JSON 字段做条件
来源：http://udc.sufxvd.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qnv.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://qod.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mlz.dianchejie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ptw.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://ujx.yonumen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ygn.fktsv.cn

[Q90] 生成序号列
来源：http://lml.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cvs.daxiang520.top

================================================================================
来源：http://edu.jyoumei.cn

R. Bash 专题
来源：http://oqi.hysaishi.cn

================================================================================
来源：http://ivk.hfpthk.cn

[R01] shebang 与严格模式
来源：http://ruk.bbcook.cn

#!/usr/bin/env bash
来源：http://cde.jianghu66.top

set -euo pipefail
来源：http://icc.quarkkingdee.top

[R02] 变量赋值与使用
来源：http://hrt.chenzaomai.com

name="Tom"; echo "$name"
来源：http://ide.sysykeji.top

[R03] 只读变量
来源：http://ofm.wangdashe.top

readonly PI=3.14
来源：http://dbb.svipenyu.cn

[R04] 位置参数
来源：http://pfe.jyoumei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dgu.gzhubu.top

[R05] 参数默认值
来源：http://iak.svipenyu.cn


<!-- 参考信息 -->