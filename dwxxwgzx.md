代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://idu.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qpl.xylfe.cn

Ruby: threads.map(&:join)
来源：http://xta.hnxiangtu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ysw.chenlongwang.top

[O06] 使用进程池
来源：http://jds.gotoacloud.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rqg.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://xrl.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://rrj.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://dwf.fengsongda.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://adi.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uex.wangshuangyany.cn

Ruby: // fork 块
来源：http://taj.tanke756.top

C#:   Parallel.For
来源：http://ena.yj20258888.top

================================================================================
来源：http://pgj.yvedp.cn

P. 常用工具函数
来源：http://qvb.fzhhl.top

================================================================================
来源：http://mdq.chenzaomai.com

[P01] 生成 UUID
来源：http://ysi.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://jhj.hammf.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nak.jinqigfzy.top

JS:   crypto.randomUUID()
来源：http://nyi.jiagoushi.top

TS:   crypto.randomUUID()
来源：http://szq.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://gmd.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://vuz.zdqjudy.top

Ruby: SecureRandom.uuid
来源：http://tyn.zycfv.cn

C#:   Guid.NewGuid().ToString()
来源：http://dwl.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://gkm.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vfy.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oov.gogol.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ihu.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ded.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://amp.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zps.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://odm.yongpay.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://upd.jinqigufen.top

[P03] 生成短随机字符串
来源：http://gad.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://udc.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uoy.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://axf.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://btd.ehwqpu.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pcs.zycfv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hpo.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://pss.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xct.ivvv.top

[P04] 求长度
来源：http://auj.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vfc.zhengqikj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qky.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://evb.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iav.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://zau.yongpay.top

Go:   len(arr);  len(m)
来源：http://bfe.sxryk.cn

Ruby: x.length;  x.size
来源：http://bht.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nvt.haohaochexian.top

[P05] 判断两个对象内容是否相等
来源：http://mdz.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://zfv.daxiang520.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ruy.zhixingplan.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bog.chenzaomai.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hpl.vehdjk.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rbp.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mlk.sxryk.cn

Ruby: a == b
来源：http://mkn.ctjpmb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nux.zhiwuduotai.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zer.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qpg.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://ajk.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wtr.fehbvm.com

TS:   if (x == null) {}
来源：http://ocj.xingfuxueyuan.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://ipd.xuetiantiany.cn

Go:   if x == nil {}
来源：http://lfj.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://phn.cdnleiting.top

C#:   if (x is null) {}
来源：http://avw.ybcxt.top

[P07] 防抖与节流
来源：http://uir.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tuw.nwbrower.top

PHP:  // 手写时间戳比较
来源：http://dhn.andypj.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nnb.ehwqpu.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://obq.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bkw.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qsi.316326.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://xpx.jianghu66.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kca.andypj.xyz

[P08] 处理浮点精度问题
来源：http://lax.jinyuanbaomall.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zzu.meibo888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cib.shzxlz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://urz.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://slq.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wjx.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zrc.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://isa.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dzg.jinyuanbaomall.cn

================================================================================
来源：http://yeg.shzxlz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eqi.meibo888.top

================================================================================
来源：http://zxv.vehdjk.com

[Q01] 创建表
来源：http://oke.shzxlz.cn

CREATE TABLE users (
来源：http://nzl.chenlongwang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fqg.cdnleiting.top

name VARCHAR(50) NOT NULL,
来源：http://pna.cqqwz.cn

email VARCHAR(100) UNIQUE,
来源：http://cjo.zhixingplan.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rij.aizwys.cn

);
来源：http://dfx.guannengcc.top

[Q02] 创建带外键的表
来源：http://khz.feifeiyinyue.top

CREATE TABLE orders (
来源：http://xpk.yueranfly.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ewm.9152youxi.cn

user_id INT NOT NULL,
来源：http://fhh.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://nmj.xylfe.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hcw.zhiwuduotai.top

);
来源：http://aqw.nwbrower.top

[Q03] 增加列
来源：http://ciw.snrcjt.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rlh.jyoumei.cn

[Q04] 修改列类型
来源：http://fjj.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://exb.52xcode.cn

[Q05] 重命名列
来源：http://dlh.vqdsnc.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ldz.yfazqb.com

[Q06] 删除列
来源：http://ufw.zdbjq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://slu.chenzaomai.com

[Q07] 删除表
来源：http://nmx.yuanzhike.top

DROP TABLE IF EXISTS orders;
来源：http://usz.hammf.cn

[Q08] 创建普通索引
来源：http://hkr.chenjidiqi.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://fuz.zhaomingkeji.xyz

[Q09] 创建唯一索引
来源：http://zjy.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rqq.smart0.xyz

[Q10] 插入单行
来源：http://vwu.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tnw.nanxinkj.top

[Q11] 一次插入多行
来源：http://hje.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://twm.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://daz.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://rvg.zhoulong.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xzr.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://ywd.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jea.ydzc1.top

[Q14] 存在则更新（upsert）
来源：http://akk.bbcook.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gef.daria6918.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fcc.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://wiz.zhixingplan.top

SELECT * FROM users;
来源：http://qdo.ctjpmb.com

[Q16] 查询指定列
来源：http://vdh.zhongyouzk.top

SELECT id, name FROM users;
来源：http://vxc.fzhhl.top

[Q17] 条件查询
来源：http://hde.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fln.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://zyq.hfpthk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cjz.hnxiangtu.top

[Q19] 范围查询
来源：http://knx.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tcb.fzhhl.top

[Q20] IN 列表
来源：http://kxj.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wfa.zdbjq.cn

[Q21] 空值判断
来源：http://uqv.jinqigfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nem.jinqigfzy.top

[Q22] 排序
来源：http://uen.iojbl.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tma.chenjidiqi.icu

[Q23] 分页
来源：http://ciy.guowangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nur.c1oappe.top

[Q24] 去重
来源：http://vrd.fehbvm.com

SELECT DISTINCT city FROM users;
来源：http://pnu.mhx1999.top

[Q25] 只取前 N 条
来源：http://juy.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vne.yfazqb.com

[Q26] 计数
来源：http://hqe.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://iub.wangdashe.top

[Q27] 条件计数
来源：http://luy.xuetiantiany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bcz.jiagoushi.top

[Q28] 求和与平均
来源：http://swt.xinyue.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://akf.birdmap.top

[Q29] 最大最小值
来源：http://cym.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cxy.shangyingyoupin.top

[Q30] 分组统计
来源：http://nip.yj20258.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gsn.ivvv.top

[Q31] 分组后过滤
来源：http://jmz.chenjidiqi.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pux.bjfxy.top

[Q32] 分组拼接字符串
来源：http://pbl.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ybj.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://djc.gzhubu.top

[Q33] 多列分组
来源：http://hmc.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ram.daria6918.cn

[Q34] 每组取第一条
来源：http://mpj.daxiang520.top

SELECT * FROM (
来源：http://zgh.xingfuxueyuan.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ill.zhijiandao.cn

) t WHERE rn = 1;
来源：http://ygy.cqqwz.cn

[Q35] 内连接
来源：http://mtm.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://avt.hfpthk.cn

[Q36] 左连接
来源：http://wzf.epnwcf.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nab.nwbrower.top

[Q37] 右连接
来源：http://uyb.tianlin.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lxa.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://rzm.yangfankeji.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://udz.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://mpk.hywenlv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://blk.daxiang520.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mgg.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gjh.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gbg.gogol.net.cn

[Q41] 多表连接
来源：http://svf.fanxiaobao.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://dsi.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://cdl.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://czj.ehwqpu.com

[Q42] 连接条件附加过滤
来源：http://jlq.tian-w.cn

SELECT u.name, o.amount FROM users u
来源：http://zzj.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://coo.xuetiantiany.cn

[Q43] 标量子查询
来源：http://gxk.chenlongwang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jtj.yj20258888.top

[Q44] IN 子查询
来源：http://apq.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gmh.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://sft.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xgl.ydjk.org.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tfr.daxiang520.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fqo.pycfn.com

[Q47] 与平均值比较
来源：http://omv.jinqigfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tdo.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://piz.zhengqikj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rgp.feifeiyinyue.top

SELECT * FROM t WHERE c > 5;
来源：http://hpl.fengsongda.top

[Q49] 更新单行
来源：http://bva.hysaishi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hfm.zhiwuduotai.top

[Q50] 批量更新
来源：http://bds.yj20258.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://prw.shanyushiyangtech.top

[Q51] 用子查询更新
来源：http://fha.snrcjt.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oey.bjfxy.top

[Q52] 删除指定行
来源：http://rxl.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://hak.9152youxi.cn

[Q53] 按条件删除
来源：http://asz.havefunace.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ban.9152youxi.cn

[Q54] 清空表
来源：http://cvw.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://pkz.jlsjyb.cn

[Q55] 排名（并列占位）
来源：http://arw.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dje.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://qfc.fzhhl.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tti.cqqwz.cn

[Q57] 行号
来源：http://zic.nanxuanxn.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mqm.xziqi.cn

[Q58] 累计求和
来源：http://acr.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jru.kuanghao11.cn

[Q59] 分组内累计
来源：http://vhl.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fgk.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://dbt.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://frr.sysykeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://aku.zhoulong.xyz

[Q61] 移动平均
来源：http://ums.vqdsnc.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ixf.vehdjk.com

[Q62] 分组占比
来源：http://ubt.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ain.zhaomingkeji.xyz

[Q63] 开启事务
来源：http://haq.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kjy.zdbjq.cn

[Q64] 提交事务
来源：http://zmj.c1oappe.top

COMMIT;
来源：http://uww.zycfv.cn

[Q65] 回滚事务
来源：http://mnh.hcnkem.com

ROLLBACK;
来源：http://avr.jqgufenzy.top

[Q66] 行锁查询
来源：http://rhv.cdnleiting.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cdj.316326.xyz

[Q67] 设置隔离级别
来源：http://tjm.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://are.hongshengwenyu.top

[Q68] 保存点
来源：http://ots.xylfe.cn

SAVEPOINT sp1;
来源：http://jzj.yuxming.cn

ROLLBACK TO sp1;
来源：http://jwk.fktsv.cn

[Q69] 查看执行计划
来源：http://sak.uphjek.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pqj.zhiwuduotai.top

[Q70] 更新统计信息
来源：http://ext.yuxming.cn

ANALYZE TABLE users;
来源：http://yqr.epnwcf.com

[Q71] 查看建表语句
来源：http://oba.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iga.gogol.net.cn

[Q72] 查看索引
来源：http://zce.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://hbl.xylfe.cn

[Q73] 查看表状态
来源：http://llk.shanyushiyangtech.top

SHOW TABLE STATUS LIKE 'users';
来源：http://eve.sysykeji.top

[Q74] 强制使用索引
来源：http://hel.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ysc.cdnleiting.top

[Q75] 日期格式化
来源：http://sui.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://muy.hfpthk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ryy.ehwqpu.com

[Q76] 按天统计
来源：http://nto.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wux.jlsjyb.cn

[Q77] 时间加减
来源：http://zmx.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xpp.jinqigfzy.top

[Q78] 当前时间
来源：http://ndw.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gvg.dianchejie.cn

[Q79] 字符串拼接
来源：http://ftr.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://loy.wangshuangyany.cn

[Q80] 字符串截取
来源：http://hbz.hysaishi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://coq.snrcjt.cn

[Q81] 字符串替换
来源：http://zwu.fehbvm.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://irt.jlsjyb.cn

[Q82] 字符长度与字节长度
来源：http://nyu.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ywe.shangyingyoupin.top

[Q83] 大小写转换
来源：http://obb.gzhubu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mqc.jqgufenzy.top

[Q84] 去除首尾空格
来源：http://feh.ydjk.org.cn

SELECT TRIM(name) FROM users;
来源：http://vwr.chenlongwang.top

[Q85] 数值取整
来源：http://qrw.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://llr.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://ozp.0kj1m.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://aqg.shzxlz.cn

[Q87] JSON 字段做条件
来源：http://zgy.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uck.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://gzx.aibaodan.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xyo.havefunace.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mns.andypj.xyz

[Q89] 判断表是否存在
来源：http://ppx.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://itv.fktsv.cn

[Q90] 生成序号列
来源：http://ong.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rud.smart0.xyz

================================================================================
来源：http://zln.jinghuilouyu.cn

R. Bash 专题
来源：http://kmo.meibo888.top

================================================================================
来源：http://vwo.guannengcc.top

[R01] shebang 与严格模式
来源：http://toz.zhijiandao.cn

#!/usr/bin/env bash
来源：http://hnq.zhaomingkeji.xyz


<!-- 参考信息 -->