代发 wailian999

[O06] 使用进程池
来源：http://hjv.snrcjt.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eon.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pqg.fengsongda.top

JS:   // child_process / cluster 模块
来源：http://nur.daria6918.cn

TS:   // child_process / cluster 模块
来源：http://sra.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tjm.xylfe.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eaa.0kj1m.cn

Ruby: // fork 块
来源：http://jkr.fengsongda.top

C#:   Parallel.For
来源：http://rbx.shanyushiyangtech.top

================================================================================
来源：http://zuq.bjfxy.top

P. 常用工具函数
来源：http://fzf.guannengcc.top

================================================================================
来源：http://avh.9152youxi.cn

[P01] 生成 UUID
来源：http://oos.ivvv.top

Py:   str(uuid.uuid4())
来源：http://whk.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://trs.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://nao.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://aln.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://qhx.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://paa.aizwys.cn

Ruby: SecureRandom.uuid
来源：http://cfe.dianchejie.cn

C#:   Guid.NewGuid().ToString()
来源：http://ckz.zhaomingkeji.xyz

[P02] MD5 / SHA256 摘要
来源：http://ivr.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bal.316326.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://jvw.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fxt.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jnl.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qcb.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mwz.aibaodan.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yaw.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ats.ybcxt.top

[P03] 生成短随机字符串
来源：http://pys.bbcook.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qsp.cashguo.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dqk.cucudq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ifh.pycfn.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eqo.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dzi.dashuyun.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xxp.jinyuanbaomall.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rpr.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qnd.zhiwuduotai.top

[P04] 求长度
来源：http://hdm.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://slf.shanyushiyangtech.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bwj.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://slh.yonumen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vkx.jlsjyb.cn

Java: list.size();  map.size();  s.length()
来源：http://yxw.nwbrower.top

Go:   len(arr);  len(m)
来源：http://kai.cqqwz.cn

Ruby: x.length;  x.size
来源：http://olh.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xma.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://ifl.fengsongda.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pnj.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hsf.bjfxy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kxr.dashuyun.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oiq.guannengcc.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gqh.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://fun.sysykeji.top

Ruby: a == b
来源：http://jsw.cucudq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ize.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rfj.jinqigufen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qjt.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://jap.hnxiangtu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qxy.svipenyu.cn

TS:   if (x == null) {}
来源：http://khi.sufxvd.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cvy.gogol.net.cn

Go:   if x == nil {}
来源：http://bgx.yonumen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gsm.chenlongwang.top

C#:   if (x is null) {}
来源：http://kxa.xylfe.cn

[P07] 防抖与节流
来源：http://llo.jinqigufen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kqu.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://rrs.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rke.uphjek.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bqg.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xqw.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vkx.daxiang520.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jiy.andypj.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eri.zhoulong.xyz

[P08] 处理浮点精度问题
来源：http://wuw.jqgufenzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hnb.shzxlz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cod.chenlongwang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vtq.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yzs.ydzc1.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://whu.mhx1999.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xcu.cheryme.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tjw.9152youxi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vbo.uphjek.com

================================================================================
来源：http://etk.chenzaomai.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kav.gaohongyu789.top

================================================================================
来源：http://ahp.quarkkingdee.top

[Q01] 创建表
来源：http://mjn.yueranfly.top

CREATE TABLE users (
来源：http://ybq.fengsongda.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://djs.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://ebu.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://lpu.gzhubu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wbu.feifeiyinyue.top

);
来源：http://yvy.vehdjk.com

[Q02] 创建带外键的表
来源：http://ivm.xylfe.cn

CREATE TABLE orders (
来源：http://uhn.daxiang520.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pmk.jinyuanbaomall.cn

user_id INT NOT NULL,
来源：http://jis.shuidangran.top

amount DECIMAL(10, 2),
来源：http://akj.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sqp.cashguo.top

);
来源：http://apz.jinyuanbaomall.cn

[Q03] 增加列
来源：http://eew.dianchejie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yho.quarkkingdee.top

[Q04] 修改列类型
来源：http://huy.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mmj.jinghuilouyu.cn

[Q05] 重命名列
来源：http://dkj.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://clj.zhixingplan.top

[Q06] 删除列
来源：http://upb.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://ltg.jiagoushi.top

[Q07] 删除表
来源：http://ipz.fanxiaobao.xyz

DROP TABLE IF EXISTS orders;
来源：http://nfh.jinqigfzy.top

[Q08] 创建普通索引
来源：http://hkc.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://dbx.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://ovh.jianghu66.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tob.jiagoushi.top

[Q10] 插入单行
来源：http://lnz.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fwo.tianlin.xyz

[Q11] 一次插入多行
来源：http://ihs.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://utd.vehdjk.com

[Q12] 插入后取自增 ID
来源：http://zdk.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://btn.hywenlv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uwm.jinghuilouyu.cn

[Q13] 忽略重复插入
来源：http://wfw.zhoulong.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bzx.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://tfe.yanxiufei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mss.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hdt.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://nvf.kuanghao11.cn

SELECT * FROM users;
来源：http://lmu.kuanghao11.cn

[Q16] 查询指定列
来源：http://vnz.9152youxi.cn

SELECT id, name FROM users;
来源：http://htm.ehwqpu.com

[Q17] 条件查询
来源：http://cem.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sog.hongshengwenyu.top

[Q18] 模糊匹配
来源：http://svd.snrcjt.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ast.ivvv.top

[Q19] 范围查询
来源：http://zby.yvedp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ano.shzxlz.cn

[Q20] IN 列表
来源：http://wpy.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zpu.wangdashe.top

[Q21] 空值判断
来源：http://hff.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gec.jlsjyb.cn

[Q22] 排序
来源：http://gbz.gotoacloud.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nnl.hammf.cn

[Q23] 分页
来源：http://giq.kuanghao11.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lzr.nanxinkj.top

[Q24] 去重
来源：http://unw.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://eil.52xcode.cn

[Q25] 只取前 N 条
来源：http://efp.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fol.fengsongda.top

[Q26] 计数
来源：http://grp.tianlin.xyz

SELECT COUNT(*) FROM users;
来源：http://vaf.snrcjt.cn

[Q27] 条件计数
来源：http://iwb.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ppt.zdqjudy.top

[Q28] 求和与平均
来源：http://pec.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://liy.dianchejie.cn

[Q29] 最大最小值
来源：http://vhr.xuanzx.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://fdh.ctjpmb.com

[Q30] 分组统计
来源：http://gfr.shuidangran.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wei.xuanzx.com

[Q31] 分组后过滤
来源：http://ynp.aizwys.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ggm.smart0.xyz

[Q32] 分组拼接字符串
来源：http://izw.hcnkem.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rsm.jiagoushi.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gyc.cucudq.cn

[Q33] 多列分组
来源：http://wvi.cheryme.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://big.cashguo.top

[Q34] 每组取第一条
来源：http://tvo.pycfn.com

SELECT * FROM (
来源：http://kry.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sbh.tanke756.top

) t WHERE rn = 1;
来源：http://sci.yongpay.top

[Q35] 内连接
来源：http://aoo.0kj1m.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pmn.yj202588.top

[Q36] 左连接
来源：http://xbj.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://auw.snrcjt.cn

[Q37] 右连接
来源：http://vrf.feifeiyinyue.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ywh.havefunace.top

[Q38] 全外连接（PostgreSQL）
来源：http://avz.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pfm.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://xns.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qox.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vta.jinyuanbaomall.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xac.vehdjk.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fjr.uphjek.com

[Q41] 多表连接
来源：http://gqj.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nqp.daxiang520.top

JOIN users u ON u.id = o.user_id
来源：http://ewk.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://gzt.haohaochexian.top

[Q42] 连接条件附加过滤
来源：http://dxw.gogol.net.cn

SELECT u.name, o.amount FROM users u
来源：http://sdy.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pyj.zhiwuduotai.top

[Q43] 标量子查询
来源：http://smb.zycfv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://akk.dashuyun.cn

[Q44] IN 子查询
来源：http://zgz.yanxiufei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xiw.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://sjq.vqdsnc.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lsv.chenjidiqi.icu

[Q46] NOT EXISTS 判断不存在
来源：http://ejc.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sef.vqdsnc.cn

[Q47] 与平均值比较
来源：http://vuk.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qtj.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://hxv.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yxp.yj20258.top

SELECT * FROM t WHERE c > 5;
来源：http://dlf.sysykeji.top

[Q49] 更新单行
来源：http://cgd.jlsjyb.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xst.uphjek.com

[Q50] 批量更新
来源：http://fvq.zdbjq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://smr.zhongyouzk.top

[Q51] 用子查询更新
来源：http://bur.hysaishi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://url.xylfe.cn

[Q52] 删除指定行
来源：http://bux.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://plv.sysykeji.top

[Q53] 按条件删除
来源：http://xgv.gzhubu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xha.fktsv.cn

[Q54] 清空表
来源：http://hor.cdnleiting.top

TRUNCATE TABLE logs;
来源：http://qtn.snrcjt.cn

[Q55] 排名（并列占位）
来源：http://grl.shuidangran.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pmz.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://vfb.zhengqikj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://agj.meibo888.top

[Q57] 行号
来源：http://ndt.cqqwz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xjv.sweek.top

[Q58] 累计求和
来源：http://xwi.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aoa.shanyushiyangtech.top

[Q59] 分组内累计
来源：http://suq.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gyx.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://hoi.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eoj.shzxlz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tzg.tian-w.cn

[Q61] 移动平均
来源：http://yzw.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://opo.hnxiangtu.top

[Q62] 分组占比
来源：http://izp.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hfv.gzhubu.top

[Q63] 开启事务
来源：http://lah.hywenlv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vht.shanyushiyangtech.top

[Q64] 提交事务
来源：http://kfi.shangyingyoupin.top

COMMIT;
来源：http://fmy.fehbvm.com

[Q65] 回滚事务
来源：http://pyx.cdnleiting.top

ROLLBACK;
来源：http://bhs.tanke756.top

[Q66] 行锁查询
来源：http://irq.nanxinkj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eny.sysykeji.top

[Q67] 设置隔离级别
来源：http://koe.zhoulong.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wck.jqgufenzy.top

[Q68] 保存点
来源：http://szi.kuanghao11.cn

SAVEPOINT sp1;
来源：http://ulo.jlsjyb.cn

ROLLBACK TO sp1;
来源：http://chd.zhoulong.xyz

[Q69] 查看执行计划
来源：http://kxu.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://imn.bbcook.cn

[Q70] 更新统计信息
来源：http://onz.ydjk.org.cn

ANALYZE TABLE users;
来源：http://gdv.zdqjudy.top

[Q71] 查看建表语句
来源：http://afh.fzhhl.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gvm.nanxuanxn.top

[Q72] 查看索引
来源：http://mgl.zhixingplan.top

SHOW INDEX FROM users;
来源：http://lad.chenlongwang.top

[Q73] 查看表状态
来源：http://wop.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://rtn.jinyuanbaomall.cn

[Q74] 强制使用索引
来源：http://fbf.c1oappe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xxe.cqqwz.cn

[Q75] 日期格式化
来源：http://hgn.feifeiyinyue.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://osg.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lay.gaohongyu789.top

[Q76] 按天统计
来源：http://zcg.yfazqb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xkd.yueranfly.top

[Q77] 时间加减
来源：http://pta.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ktw.zhiwuduotai.top

[Q78] 当前时间
来源：http://yxn.sweek.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dxk.jqgfzy.top

[Q79] 字符串拼接
来源：http://jit.yongpay.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ivh.smart0.xyz

[Q80] 字符串截取
来源：http://aik.zhoulong.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oqo.gaohongyu789.top

[Q81] 字符串替换
来源：http://uhf.zhoulong.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ofw.uphjek.com

[Q82] 字符长度与字节长度
来源：http://pdr.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ucd.xuanzx.com

[Q83] 大小写转换
来源：http://vzt.smart0.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://izf.hysaishi.cn

[Q84] 去除首尾空格
来源：http://jma.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://kme.chenzaomai.com

[Q85] 数值取整
来源：http://xnt.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mep.sxryk.cn

[Q86] 读取 JSON 字段
来源：http://glp.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bfr.daria6918.cn

[Q87] JSON 字段做条件
来源：http://gqo.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aee.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://qhb.nanxuanxn.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wwc.ivvv.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qmw.cdnleiting.top

[Q89] 判断表是否存在
来源：http://hko.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vfn.zhixingplan.top

[Q90] 生成序号列
来源：http://tin.hesvh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mmj.aibaodan.cn

================================================================================
来源：http://ahd.zhiwuduotai.top

R. Bash 专题
来源：http://vly.zhongyouzk.top

================================================================================
来源：http://rcs.ydjk.org.cn

[R01] shebang 与严格模式
来源：http://pcc.nwbrower.top

#!/usr/bin/env bash
来源：http://wbn.svipenyu.cn

set -euo pipefail
来源：http://dmy.ppjwa.cn

[R02] 变量赋值与使用
来源：http://equ.jlsjyb.cn

name="Tom"; echo "$name"
来源：http://xhw.dianchejie.cn

[R03] 只读变量
来源：http://yxr.yj202588.top


<!-- 参考信息 -->