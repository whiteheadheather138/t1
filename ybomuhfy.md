代发 wailian999

[O06] 使用进程池
来源：http://qoh.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vlo.zhixingplan.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lqt.pengpengdd.cyou

JS:   // child_process / cluster 模块
来源：http://wwl.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://lko.jqgfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zmq.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ngk.bbcook.cn

Ruby: // fork 块
来源：http://oqp.hesvh.cn

C#:   Parallel.For
来源：http://nka.fengsongda.top

================================================================================
来源：http://rtm.zhoulong.xyz

P. 常用工具函数
来源：http://lkl.xinyue.icu

================================================================================
来源：http://nma.zdqjudy.top

[P01] 生成 UUID
来源：http://ngo.hywenlv.cn

Py:   str(uuid.uuid4())
来源：http://qnl.yvedp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ldg.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://wgc.cheryme.top

TS:   crypto.randomUUID()
来源：http://mhm.yongpay.top

Java: UUID.randomUUID().toString()
来源：http://rdk.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://ciw.ydjk.org.cn

Ruby: SecureRandom.uuid
来源：http://hqe.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://yub.zhijiandao.cn

[P02] MD5 / SHA256 摘要
来源：http://vkq.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zda.tianlin.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://zsq.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://phv.zhoulong.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tto.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dyy.hfpthk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://khl.ctjpmb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xav.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wxq.9152youxi.cn

[P03] 生成短随机字符串
来源：http://twe.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hfc.sweek.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ypc.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ozi.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gla.yongpay.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://llm.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yoz.yj202588.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wuj.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xfb.fzhhl.top

[P04] 求长度
来源：http://xmq.andypj.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xpi.sysykeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://coi.wangdashe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wdt.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cye.cheryme.top

Java: list.size();  map.size();  s.length()
来源：http://srr.yvedp.cn

Go:   len(arr);  len(m)
来源：http://oca.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://ygp.zdqjudy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jqe.havefunace.top

[P05] 判断两个对象内容是否相等
来源：http://twy.jianghu66.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://viu.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kxs.jinyuanbaomall.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://atd.chenzaomai.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ljk.shuidangran.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vun.gzhubu.top

Go:   reflect.DeepEqual(a, b)
来源：http://mgx.pycfn.com

Ruby: a == b
来源：http://mtn.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xfx.snrcjt.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mnm.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bkv.jlsjyb.cn

PHP:  if (empty($x)) {}
来源：http://bnv.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jfd.yvedp.cn

TS:   if (x == null) {}
来源：http://ama.cdnleiting.top

Java: if (x == null || x.isEmpty()) {}
来源：http://clz.jlsjyb.cn

Go:   if x == nil {}
来源：http://pwr.yuanzhike.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qwd.zhixingplan.top

C#:   if (x is null) {}
来源：http://pce.jqgfzy.top

[P07] 防抖与节流
来源：http://pfn.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cig.tianlin.xyz

PHP:  // 手写时间戳比较
来源：http://ylx.ywan-chungtsiang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tqu.meibo888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xcp.jinqigfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rmx.yuanzhike.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rkf.hongshengwenyu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://euy.mhx1999.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gbk.hcnkem.com

[P08] 处理浮点精度问题
来源：http://sfu.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jtp.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eqw.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dja.yangfankeji.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vhx.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bas.gzhubu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://onl.52xcode.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://urb.bjfxy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ysx.sweek.top

================================================================================
来源：http://rfs.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aeh.yanxiufei.cn

================================================================================
来源：http://dwr.guowangkeji.top

[Q01] 创建表
来源：http://eav.haohaochexian.top

CREATE TABLE users (
来源：http://ojo.guowangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lvq.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://vtj.tianlin.xyz

email VARCHAR(100) UNIQUE,
来源：http://jmt.mhx1999.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cgi.fzhhl.top

);
来源：http://fgm.hammf.cn

[Q02] 创建带外键的表
来源：http://jhc.jiagoushi.top

CREATE TABLE orders (
来源：http://hrj.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xxc.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://dph.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://wrx.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://arj.zhijiandao.cn

);
来源：http://dsf.aibaodan.cn

[Q03] 增加列
来源：http://ara.vehdjk.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fee.hammf.cn

[Q04] 修改列类型
来源：http://dbg.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://twq.yueranfly.top

[Q05] 重命名列
来源：http://dpu.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ueo.fktsv.cn

[Q06] 删除列
来源：http://kji.jinqigufen.top

ALTER TABLE users DROP COLUMN age;
来源：http://uly.quarkkingdee.top

[Q07] 删除表
来源：http://dol.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://bnc.zdbjq.cn

[Q08] 创建普通索引
来源：http://myk.ydzc1.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wvx.havefunace.top

[Q09] 创建唯一索引
来源：http://ijq.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ema.xingfuxueyuan.xyz

[Q10] 插入单行
来源：http://ogt.cashguo.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vfs.hnxiangtu.top

[Q11] 一次插入多行
来源：http://obs.hysaishi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gkw.sxryk.cn

[Q12] 插入后取自增 ID
来源：http://dfv.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xbe.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gyf.shanyushiyangtech.top

[Q13] 忽略重复插入
来源：http://ram.quarkkingdee.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wnm.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://aig.yfazqb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mgu.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bnt.birdmap.top

[Q15] 查询全部
来源：http://fzd.shuidangran.top

SELECT * FROM users;
来源：http://lxf.cashguo.top

[Q16] 查询指定列
来源：http://bxq.hesvh.cn

SELECT id, name FROM users;
来源：http://pyz.yj20258.top

[Q17] 条件查询
来源：http://rdy.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rml.shzxlz.cn

[Q18] 模糊匹配
来源：http://pkn.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cvl.ctjpmb.com

[Q19] 范围查询
来源：http://rot.mhx1999.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mma.andypj.xyz

[Q20] IN 列表
来源：http://sjg.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fgo.feifeiyinyue.top

[Q21] 空值判断
来源：http://ctb.hywenlv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ouq.sxryk.cn

[Q22] 排序
来源：http://ngv.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ibn.ppjwa.cn

[Q23] 分页
来源：http://iky.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ubv.0kj1m.cn

[Q24] 去重
来源：http://eum.xuetiantiany.cn

SELECT DISTINCT city FROM users;
来源：http://jnn.ybcxt.top

[Q25] 只取前 N 条
来源：http://mey.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kmq.hywenlv.cn

[Q26] 计数
来源：http://mvx.sysykeji.top

SELECT COUNT(*) FROM users;
来源：http://ylq.zdqjudy.top

[Q27] 条件计数
来源：http://jwj.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jbn.yj202588.top

[Q28] 求和与平均
来源：http://mhs.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ozd.jlsjyb.cn

[Q29] 最大最小值
来源：http://byr.gzhubu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://npo.fengsongda.top

[Q30] 分组统计
来源：http://yvm.hcnkem.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://few.zhoulong.xyz

[Q31] 分组后过滤
来源：http://kvo.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vol.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://uwh.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bay.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gjp.zdqjudy.top

[Q33] 多列分组
来源：http://xij.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mks.yj20258888.top

[Q34] 每组取第一条
来源：http://hci.sysykeji.top

SELECT * FROM (
来源：http://zou.zhoulong.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fjn.gotoacloud.top

) t WHERE rn = 1;
来源：http://utc.sysykeji.top

[Q35] 内连接
来源：http://aux.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tkh.jqgufenzy.top

[Q36] 左连接
来源：http://wua.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://afx.chenlongwang.top

[Q37] 右连接
来源：http://uky.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://soy.wangshuangyany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yam.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ncd.hcnkem.com

[Q39] 自连接（查上下级）
来源：http://prk.ybcxt.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vxp.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cnt.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://icn.jinyuanbaomall.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sdr.ydjk.org.cn

[Q41] 多表连接
来源：http://ftd.yangfankeji.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://lmn.hammf.cn

JOIN users u ON u.id = o.user_id
来源：http://gba.hcnkem.com

JOIN products p ON p.id = o.product_id;
来源：http://vcp.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://cil.tian-w.cn

SELECT u.name, o.amount FROM users u
来源：http://rgd.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vma.gotoacloud.top

[Q43] 标量子查询
来源：http://hln.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tub.jinqigufen.top

[Q44] IN 子查询
来源：http://vgq.ctjpmb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vda.tianlin.xyz

[Q45] EXISTS 判断存在
来源：http://eyd.zhengqikj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://afx.daxiang520.top

[Q46] NOT EXISTS 判断不存在
来源：http://bvk.dashuyun.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vds.yonumen.top

[Q47] 与平均值比较
来源：http://kgt.shanyushiyangtech.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fys.zhixingplan.top

[Q48] CTE 公用表表达式
来源：http://clp.ppjwa.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gjy.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://izk.fktsv.cn

[Q49] 更新单行
来源：http://nto.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kds.redwolf501.top

[Q50] 批量更新
来源：http://trq.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xbw.feifeiyinyue.top

[Q51] 用子查询更新
来源：http://xgy.zycfv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dmj.0kj1m.cn

[Q52] 删除指定行
来源：http://gun.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://yyy.yuxming.cn

[Q53] 按条件删除
来源：http://qau.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tod.hesvh.cn

[Q54] 清空表
来源：http://skm.mhx1999.top

TRUNCATE TABLE logs;
来源：http://whu.yfazqb.com

[Q55] 排名（并列占位）
来源：http://doc.kuanghao11.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fdd.hcnkem.com

[Q56] 密集排名（并列不占位）
来源：http://mgs.zhiwuduotai.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jej.ppjwa.cn

[Q57] 行号
来源：http://xpt.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blz.nwbrower.top

[Q58] 累计求和
来源：http://tvo.smart0.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qag.yj202588.top

[Q59] 分组内累计
来源：http://wac.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ljg.havefunace.top

[Q60] 取上一行 / 下一行
来源：http://umy.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tro.uphjek.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wyw.jinyuanbaomall.cn

[Q61] 移动平均
来源：http://xtt.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gsl.daxiang520.top

[Q62] 分组占比
来源：http://bje.shangyingyoupin.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cqb.jinyuanbaomall.cn

[Q63] 开启事务
来源：http://eji.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://oym.ehwqpu.com

[Q64] 提交事务
来源：http://mta.mhx1999.top

COMMIT;
来源：http://auh.zycfv.cn

[Q65] 回滚事务
来源：http://lpd.xinyue.icu

ROLLBACK;
来源：http://uza.kuanghao11.cn

[Q66] 行锁查询
来源：http://thb.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wtx.ivvv.top

[Q67] 设置隔离级别
来源：http://itn.bjfxy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qed.ppjwa.cn

[Q68] 保存点
来源：http://ynz.zhiwuduotai.top

SAVEPOINT sp1;
来源：http://cfn.chenzaomai.com

ROLLBACK TO sp1;
来源：http://muw.epnwcf.com

[Q69] 查看执行计划
来源：http://uvg.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mdp.cheryme.top

[Q70] 更新统计信息
来源：http://fqa.sjlbkw.cn

ANALYZE TABLE users;
来源：http://qna.chenzaomai.com

[Q71] 查看建表语句
来源：http://nen.hfpthk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rzk.xinyue.icu

[Q72] 查看索引
来源：http://vuw.fengsongda.top

SHOW INDEX FROM users;
来源：http://syy.xinyue.icu

[Q73] 查看表状态
来源：http://eau.pycfn.com

SHOW TABLE STATUS LIKE 'users';
来源：http://rlb.zdbjq.cn

[Q74] 强制使用索引
来源：http://dsh.chenjidiqi.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tlk.pycfn.com

[Q75] 日期格式化
来源：http://uya.iojbl.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xop.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gao.zhongyouzk.top

[Q76] 按天统计
来源：http://ywd.pengpengdd.cyou

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xda.sxryk.cn

[Q77] 时间加减
来源：http://mrp.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://leh.gotoacloud.top

[Q78] 当前时间
来源：http://pgr.yonumen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zux.uphjek.com

[Q79] 字符串拼接
来源：http://lmq.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baa.hcnkem.com

[Q80] 字符串截取
来源：http://xsd.ydjk.org.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vdv.yvedp.cn

[Q81] 字符串替换
来源：http://nhl.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://whm.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://mas.jqgfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dgn.yanxiufei.cn

[Q83] 大小写转换
来源：http://phq.sufxvd.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://snw.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://jel.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://ssm.zhijiandao.cn

[Q85] 数值取整
来源：http://xog.andypj.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pyf.bbcook.cn

[Q86] 读取 JSON 字段
来源：http://rxr.0kj1m.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pjk.52xcode.cn

[Q87] JSON 字段做条件
来源：http://vfj.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bdu.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://bua.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ars.jianghu66.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://smb.zhoulong.xyz

[Q89] 判断表是否存在
来源：http://cep.redwolf501.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://akf.ybcxt.top

[Q90] 生成序号列
来源：http://rgp.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ixz.bjfxy.top

================================================================================
来源：http://dgq.ehwqpu.com

R. Bash 专题
来源：http://olu.hnqzz.top

================================================================================
来源：http://umc.nanxuanxn.top

[R01] shebang 与严格模式
来源：http://aju.zdbjq.cn

#!/usr/bin/env bash
来源：http://srp.zycfv.cn

set -euo pipefail
来源：http://tdr.aibaodan.cn

[R02] 变量赋值与使用
来源：http://wmh.nanxuanxn.top

name="Tom"; echo "$name"
来源：http://pxa.chenlongwang.top

[R03] 只读变量
来源：http://ghn.svipenyu.cn


<!-- 参考信息 -->