代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yri.jqgufenzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cch.birdmap.top

Ruby: threads.map(&:join)
来源：http://kxj.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://xtr.yj20258888.top

[O06] 使用进程池
来源：http://tpl.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xys.tian-w.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ayj.daria6918.cn

JS:   // child_process / cluster 模块
来源：http://wxj.tarul.cn

TS:   // child_process / cluster 模块
来源：http://rlo.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mos.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gsn.cheryme.top

Ruby: // fork 块
来源：http://sny.fengsongda.top

C#:   Parallel.For
来源：http://kqv.chenjidiqi.icu

================================================================================
来源：http://thv.yonumen.top

P. 常用工具函数
来源：http://ehd.ehwqpu.com

================================================================================
来源：http://dzm.316326.xyz

[P01] 生成 UUID
来源：http://udp.nanxuanxn.top

Py:   str(uuid.uuid4())
来源：http://zwl.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qmv.iojbl.cn

JS:   crypto.randomUUID()
来源：http://krs.xziqi.cn

TS:   crypto.randomUUID()
来源：http://set.tarul.cn

Java: UUID.randomUUID().toString()
来源：http://mgc.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://sxx.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://tcp.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://vap.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://hkb.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sgh.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zaw.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://frr.hfpthk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zlj.shanyushiyangtech.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tvm.9152youxi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qar.redwolf501.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wwm.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://owx.cashguo.top

[P03] 生成短随机字符串
来源：http://cln.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://axu.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lyx.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jue.zhengqikj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://edy.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://job.hysaishi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://phl.zhongyouzk.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gsn.hongshengwenyu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ikh.c1oappe.top

[P04] 求长度
来源：http://leb.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ztx.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://arc.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gqf.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eje.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://hms.zhixingplan.top

Go:   len(arr);  len(m)
来源：http://anl.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://ceg.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://tqp.hnqzz.top

[P05] 判断两个对象内容是否相等
来源：http://hpx.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dec.zhengqikj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iun.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tez.yangfankeji.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cim.aibaodan.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rqc.gotoacloud.top

Go:   reflect.DeepEqual(a, b)
来源：http://vug.xylfe.cn

Ruby: a == b
来源：http://dbp.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uig.aizwys.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tvp.zhongyouzk.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kia.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://ydg.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zza.yj202588.top

TS:   if (x == null) {}
来源：http://zmh.meibo888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nyp.zhaomingkeji.xyz

Go:   if x == nil {}
来源：http://dkl.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://spy.cucudq.cn

C#:   if (x is null) {}
来源：http://ygc.epnwcf.com

[P07] 防抖与节流
来源：http://hlu.yangfankeji.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eac.9152youxi.cn

PHP:  // 手写时间戳比较
来源：http://ksx.wangshuangyany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ess.yueranfly.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sja.jiagoushi.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wkw.pengpengdd.cyou

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://poy.bjfxy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jxz.hnqzz.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vpv.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://xla.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dog.feifeiyinyue.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bzr.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ckb.snrcjt.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://raq.cheryme.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://utb.shangyingyoupin.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zgr.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tel.gogol.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ohk.aibaodan.cn

================================================================================
来源：http://keb.hammf.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eev.andypj.xyz

================================================================================
来源：http://sya.sufxvd.cn

[Q01] 创建表
来源：http://bzh.feifeiyinyue.top

CREATE TABLE users (
来源：http://kfi.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ljb.zdqjudy.top

name VARCHAR(50) NOT NULL,
来源：http://lzn.hfpthk.cn

email VARCHAR(100) UNIQUE,
来源：http://mwj.fktsv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ffr.xingfuxueyuan.xyz

);
来源：http://sro.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://fza.yueranfly.top

CREATE TABLE orders (
来源：http://uoo.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jsx.snrcjt.cn

user_id INT NOT NULL,
来源：http://soi.chenlongwang.top

amount DECIMAL(10, 2),
来源：http://lwh.hcnkem.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://idx.zhixingplan.top

);
来源：http://fhl.fengsongda.top

[Q03] 增加列
来源：http://xqu.iojbl.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wes.fehbvm.com

[Q04] 修改列类型
来源：http://owo.chenzaomai.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mxp.aibaodan.cn

[Q05] 重命名列
来源：http://ipz.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kkg.ctjpmb.com

[Q06] 删除列
来源：http://fra.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://eiu.hesvh.cn

[Q07] 删除表
来源：http://cno.jinghuilouyu.cn

DROP TABLE IF EXISTS orders;
来源：http://mrz.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://gje.cdnleiting.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mpn.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://syt.jinqigufen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://azr.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://gnc.guowangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://emy.quarkkingdee.top

[Q11] 一次插入多行
来源：http://swp.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mck.tanke756.top

[Q12] 插入后取自增 ID
来源：http://iak.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://wjh.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gzq.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://nip.fktsv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dua.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://pgk.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ewc.ydzc1.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vsw.havefunace.top

[Q15] 查询全部
来源：http://kpw.hfpthk.cn

SELECT * FROM users;
来源：http://oev.jiagoushi.top

[Q16] 查询指定列
来源：http://qgp.tarul.cn

SELECT id, name FROM users;
来源：http://agf.ybcxt.top

[Q17] 条件查询
来源：http://erb.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://seg.jinqigfzy.top

[Q18] 模糊匹配
来源：http://igd.daxiang520.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tzx.tanke756.top

[Q19] 范围查询
来源：http://hzv.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zgs.aibaodan.cn

[Q20] IN 列表
来源：http://aka.gzhubu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ebm.dianchejie.cn

[Q21] 空值判断
来源：http://xly.wangdashe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pff.quarkkingdee.top

[Q22] 排序
来源：http://hje.hammf.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xpq.yfazqb.com

[Q23] 分页
来源：http://wnd.vqdsnc.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aop.xuetiantiany.cn

[Q24] 去重
来源：http://pqm.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://oqy.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://adq.chenlongwang.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aeb.yj20258888.top

[Q26] 计数
来源：http://ozn.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://ehi.smart0.xyz

[Q27] 条件计数
来源：http://qqf.yj20258.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jyo.gogol.net.cn

[Q28] 求和与平均
来源：http://uti.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ekw.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://kwh.nanxinkj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://oiv.meibo888.top

[Q30] 分组统计
来源：http://aih.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cpc.zhoulong.xyz

[Q31] 分组后过滤
来源：http://vmd.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dfp.yanxiufei.cn

[Q32] 分组拼接字符串
来源：http://aze.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zfi.xinyue.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ibu.jlsjyb.cn

[Q33] 多列分组
来源：http://zhf.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rpp.ydjk.org.cn

[Q34] 每组取第一条
来源：http://boa.sjlbkw.cn

SELECT * FROM (
来源：http://mof.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ptq.dianchejie.cn

) t WHERE rn = 1;
来源：http://scv.hfpthk.cn

[Q35] 内连接
来源：http://vwu.dashuyun.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sda.shangyingyoupin.top

[Q36] 左连接
来源：http://rlp.c1oappe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hju.sufxvd.cn

[Q37] 右连接
来源：http://jwe.sxryk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pur.zdqjudy.top

[Q38] 全外连接（PostgreSQL）
来源：http://eky.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ugz.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://aiq.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xgy.shangyingyoupin.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://khm.xingfuxueyuan.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://vce.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://njh.zycfv.cn

[Q41] 多表连接
来源：http://lul.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gtg.yangfankeji.com

JOIN users u ON u.id = o.user_id
来源：http://hle.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://pel.shzxlz.cn

[Q42] 连接条件附加过滤
来源：http://uef.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://olz.cdnleiting.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sdn.shuidangran.top

[Q43] 标量子查询
来源：http://nui.fktsv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iwz.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://egq.yanxiufei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ytu.pycfn.com

[Q45] EXISTS 判断存在
来源：http://bmi.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ntz.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sfz.ydjk.org.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gmm.dashuyun.cn

[Q47] 与平均值比较
来源：http://upw.uphjek.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://utw.gogol.net.cn

[Q48] CTE 公用表表达式
来源：http://unb.hcnkem.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hwk.yuanzhike.top

SELECT * FROM t WHERE c > 5;
来源：http://ktr.cheryme.top

[Q49] 更新单行
来源：http://uqo.hnxiangtu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qbz.redwolf501.top

[Q50] 批量更新
来源：http://nsx.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dep.zhaomingkeji.xyz

[Q51] 用子查询更新
来源：http://fbg.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kkl.feifeiyinyue.top

[Q52] 删除指定行
来源：http://fjr.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://aum.aibaodan.cn

[Q53] 按条件删除
来源：http://bvd.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bkh.shuidangran.top

[Q54] 清空表
来源：http://lgo.ppjwa.cn

TRUNCATE TABLE logs;
来源：http://iuy.sxryk.cn

[Q55] 排名（并列占位）
来源：http://ome.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://msv.shangyingyoupin.top

[Q56] 密集排名（并列不占位）
来源：http://ojt.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ufj.ctjpmb.com

[Q57] 行号
来源：http://mfv.daxiang520.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ppw.smart0.xyz

[Q58] 累计求和
来源：http://zmr.jqgfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yze.xziqi.cn

[Q59] 分组内累计
来源：http://dxo.cheryme.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ztq.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://hfy.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mis.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ube.xinyue.icu

[Q61] 移动平均
来源：http://ueo.cqqwz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ajo.havefunace.top

[Q62] 分组占比
来源：http://iyv.meibo888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rot.bbcook.cn

[Q63] 开启事务
来源：http://fba.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://odm.nanxinkj.top

[Q64] 提交事务
来源：http://ocb.epnwcf.com

COMMIT;
来源：http://zdz.tanke756.top

[Q65] 回滚事务
来源：http://imf.daxiang520.top

ROLLBACK;
来源：http://gub.cdnleiting.top

[Q66] 行锁查询
来源：http://szw.xinyue.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mke.ctjpmb.com

[Q67] 设置隔离级别
来源：http://zfs.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mmd.zhiwuduotai.top

[Q68] 保存点
来源：http://lsq.ydzc1.top

SAVEPOINT sp1;
来源：http://hez.gotoacloud.top

ROLLBACK TO sp1;
来源：http://eqi.haohaochexian.top

[Q69] 查看执行计划
来源：http://ttg.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://raj.nanxuanxn.top

[Q70] 更新统计信息
来源：http://klu.mhx1999.top

ANALYZE TABLE users;
来源：http://dym.gogol.net.cn

[Q71] 查看建表语句
来源：http://sed.shanyushiyangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jlw.9152youxi.cn

[Q72] 查看索引
来源：http://gnw.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://dpi.mhx1999.top

[Q73] 查看表状态
来源：http://ega.52xcode.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gln.sjlbkw.cn

[Q74] 强制使用索引
来源：http://aal.ehwqpu.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jov.epnwcf.com

[Q75] 日期格式化
来源：http://bmp.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aua.aibaodan.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qau.c1oappe.top

[Q76] 按天统计
来源：http://sjp.jinghuilouyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://btx.jyoumei.cn

[Q77] 时间加减
来源：http://ius.yanxiufei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wox.gogol.net.cn

[Q78] 当前时间
来源：http://qly.hfpthk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fui.fehbvm.com

[Q79] 字符串拼接
来源：http://ttx.c1oappe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://txd.0kj1m.cn

[Q80] 字符串截取
来源：http://rje.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lxg.zhongyouzk.top

[Q81] 字符串替换
来源：http://akb.ydjk.org.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yww.xinyue.icu

[Q82] 字符长度与字节长度
来源：http://qoj.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wtd.zhaomingkeji.xyz

[Q83] 大小写转换
来源：http://uvr.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ofo.havefunace.top

[Q84] 去除首尾空格
来源：http://jul.0kj1m.cn

SELECT TRIM(name) FROM users;
来源：http://mjq.zhaomingkeji.xyz

[Q85] 数值取整
来源：http://liv.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bmf.hcnkem.com

[Q86] 读取 JSON 字段
来源：http://try.chenzaomai.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://feb.hesvh.cn

[Q87] JSON 字段做条件
来源：http://zxs.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jio.9152youxi.cn

[Q88] 行转列（条件聚合）
来源：http://ljg.jyoumei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ywf.xuanzx.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pbd.yuxming.cn

[Q89] 判断表是否存在
来源：http://icf.jinghuilouyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wpk.xuanzx.com

[Q90] 生成序号列
来源：http://jku.ydzc1.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vmf.sweek.top

================================================================================
来源：http://xci.yj202588.top

R. Bash 专题
来源：http://zfp.ybcxt.top

================================================================================
来源：http://zmf.ybcxt.top

[R01] shebang 与严格模式
来源：http://rqg.cashguo.top

#!/usr/bin/env bash
来源：http://sfc.hysaishi.cn


<!-- 参考信息 -->