代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://psl.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gfk.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://fek.zhijiandao.cn

TS:   await Promise.all(tasks)
来源：http://yjv.shuidangran.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bxr.jqgufenzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hjk.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://rah.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fov.jqgfzy.top

[O06] 使用进程池
来源：http://zwm.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vwm.zhijiandao.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vus.yongpay.top

JS:   // child_process / cluster 模块
来源：http://jiu.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://wvv.meibo888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pod.xingfuxueyuan.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vno.haohaochexian.top

Ruby: // fork 块
来源：http://cco.yuanzhike.top

C#:   Parallel.For
来源：http://ifq.zhongyouzk.top

================================================================================
来源：http://djb.yuxming.cn

P. 常用工具函数
来源：http://huq.gzhubu.top

================================================================================
来源：http://pbf.aibaodan.cn

[P01] 生成 UUID
来源：http://sol.epnwcf.com

Py:   str(uuid.uuid4())
来源：http://pua.quarkkingdee.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zlh.redwolf501.top

JS:   crypto.randomUUID()
来源：http://rih.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://cdi.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://xuq.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://kyo.tian-w.cn

Ruby: SecureRandom.uuid
来源：http://ecv.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://krd.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://otf.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wko.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://moo.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wqr.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tdk.sufxvd.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://grx.uphjek.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gjy.iojbl.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pbf.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zcg.jinghuilouyu.cn

[P03] 生成短随机字符串
来源：http://olv.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cvi.c1oappe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iin.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bei.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bsq.tian-w.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cle.daria6918.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vol.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wcz.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://juz.nanxuanxn.top

[P04] 求长度
来源：http://vvj.cqqwz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://klc.yj20258.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gms.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jml.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hgo.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://hwt.tanke756.top

Go:   len(arr);  len(m)
来源：http://dkq.meibo888.top

Ruby: x.length;  x.size
来源：http://ufc.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nyg.tian-w.cn

[P05] 判断两个对象内容是否相等
来源：http://lzs.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zly.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fke.shzxlz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hby.smart0.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fft.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mnr.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://fev.tian-w.cn

Ruby: a == b
来源：http://uit.shanyushiyangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xbo.sufxvd.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kaa.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tjp.sufxvd.cn

PHP:  if (empty($x)) {}
来源：http://rjx.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://emd.ehwqpu.com

TS:   if (x == null) {}
来源：http://bym.bjfxy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ysz.tarul.cn

Go:   if x == nil {}
来源：http://ero.wangshuangyany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cpy.gogol.net.cn

C#:   if (x is null) {}
来源：http://tzt.havefunace.top

[P07] 防抖与节流
来源：http://ddx.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cqr.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://vas.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://euf.xuetiantiany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kln.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qrq.ppjwa.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://djl.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lbn.gzhubu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sgq.uphjek.com

[P08] 处理浮点精度问题
来源：http://frl.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fcg.shanyushiyangtech.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pnd.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uth.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nfc.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zra.hfpthk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gcr.chenlongwang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tnm.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dou.tianlin.xyz

================================================================================
来源：http://awr.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bry.gogol.net.cn

================================================================================
来源：http://wth.aibaodan.cn

[Q01] 创建表
来源：http://cxi.gzhubu.top

CREATE TABLE users (
来源：http://ags.zycfv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fml.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://hke.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://tti.xingfuxueyuan.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yuc.ydzc1.top

);
来源：http://gvg.jyoumei.cn

[Q02] 创建带外键的表
来源：http://mav.sxryk.cn

CREATE TABLE orders (
来源：http://yzb.jiagoushi.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cfp.sysykeji.top

user_id INT NOT NULL,
来源：http://xhe.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://bhq.iojbl.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nbk.quarkkingdee.top

);
来源：http://voy.pengpengdd.cyou

[Q03] 增加列
来源：http://lyc.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cte.jyoumei.cn

[Q04] 修改列类型
来源：http://rgj.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jfe.zhixingplan.top

[Q05] 重命名列
来源：http://puv.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kjg.nwbrower.top

[Q06] 删除列
来源：http://raf.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://kux.shuidangran.top

[Q07] 删除表
来源：http://bzi.zdbjq.cn

DROP TABLE IF EXISTS orders;
来源：http://ott.ydjk.org.cn

[Q08] 创建普通索引
来源：http://hzh.zhongyouzk.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hxj.svipenyu.cn

[Q09] 创建唯一索引
来源：http://yse.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mso.yongpay.top

[Q10] 插入单行
来源：http://mvu.9152youxi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vaa.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://oob.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nwu.gzhubu.top

[Q12] 插入后取自增 ID
来源：http://eiy.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://xhy.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cjf.smart0.xyz

[Q13] 忽略重复插入
来源：http://nbj.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oby.fktsv.cn

[Q14] 存在则更新（upsert）
来源：http://ymj.yanxiufei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yqh.ivvv.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aln.cashguo.top

[Q15] 查询全部
来源：http://gjf.cdnleiting.top

SELECT * FROM users;
来源：http://bbj.aizwys.cn

[Q16] 查询指定列
来源：http://ydw.dianchejie.cn

SELECT id, name FROM users;
来源：http://quv.nanxuanxn.top

[Q17] 条件查询
来源：http://aqt.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qkn.c1oappe.top

[Q18] 模糊匹配
来源：http://rmf.yuxming.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pfk.gzhubu.top

[Q19] 范围查询
来源：http://kko.9152youxi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ihg.nwbrower.top

[Q20] IN 列表
来源：http://esf.epnwcf.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xms.hfpthk.cn

[Q21] 空值判断
来源：http://tzi.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aku.dashuyun.cn

[Q22] 排序
来源：http://wmn.nanxuanxn.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://szp.9152youxi.cn

[Q23] 分页
来源：http://rus.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hso.sysykeji.top

[Q24] 去重
来源：http://zhf.cheryme.top

SELECT DISTINCT city FROM users;
来源：http://tlz.hammf.cn

[Q25] 只取前 N 条
来源：http://xcv.dashuyun.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sck.yj202588.top

[Q26] 计数
来源：http://emt.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://htw.jianghu66.top

[Q27] 条件计数
来源：http://ugt.guowangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jzy.redwolf501.top

[Q28] 求和与平均
来源：http://wmw.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://frq.zhaomingkeji.xyz

[Q29] 最大最小值
来源：http://jst.fengsongda.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hfo.svipenyu.cn

[Q30] 分组统计
来源：http://ont.sysykeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://syo.zhengqikj.top

[Q31] 分组后过滤
来源：http://amt.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xwl.daxiang520.top

[Q32] 分组拼接字符串
来源：http://vjf.9152youxi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mhd.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ist.epnwcf.com

[Q33] 多列分组
来源：http://ujd.9152youxi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://boe.meibo888.top

[Q34] 每组取第一条
来源：http://ajs.fktsv.cn

SELECT * FROM (
来源：http://eyb.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kud.chenjidiqi.icu

) t WHERE rn = 1;
来源：http://rnj.dashuyun.cn

[Q35] 内连接
来源：http://oka.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://axn.hnqzz.top

[Q36] 左连接
来源：http://yzb.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tjx.feifeiyinyue.top

[Q37] 右连接
来源：http://qdo.gzhubu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dii.vehdjk.com

[Q38] 全外连接（PostgreSQL）
来源：http://ssn.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yzz.tarul.cn

[Q39] 自连接（查上下级）
来源：http://xix.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://def.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qay.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pff.yuxming.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://viy.jlsjyb.cn

[Q41] 多表连接
来源：http://rzw.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://dmq.zhaomingkeji.xyz

JOIN users u ON u.id = o.user_id
来源：http://xuf.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://hgp.sysykeji.top

[Q42] 连接条件附加过滤
来源：http://pws.meibo888.top

SELECT u.name, o.amount FROM users u
来源：http://vwk.zhaomingkeji.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dpa.ehwqpu.com

[Q43] 标量子查询
来源：http://rbi.ctjpmb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bct.ehwqpu.com

[Q44] IN 子查询
来源：http://ycc.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://keo.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://lkq.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pae.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gqm.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aes.nanxuanxn.top

[Q47] 与平均值比较
来源：http://elq.yuanzhike.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hxp.sjlbkw.cn

[Q48] CTE 公用表表达式
来源：http://dkb.yongpay.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dwx.hfpthk.cn

SELECT * FROM t WHERE c > 5;
来源：http://clc.ehwqpu.com

[Q49] 更新单行
来源：http://kte.ybcxt.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vum.sysykeji.top

[Q50] 批量更新
来源：http://dtl.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xwb.sweek.top

[Q51] 用子查询更新
来源：http://shh.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zis.nwbrower.top

[Q52] 删除指定行
来源：http://yzl.quarkkingdee.top

DELETE FROM users WHERE id = 10;
来源：http://ety.ppjwa.cn

[Q53] 按条件删除
来源：http://vwu.hysaishi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blf.sxryk.cn

[Q54] 清空表
来源：http://ayv.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://wsa.ppjwa.cn

[Q55] 排名（并列占位）
来源：http://fvd.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ojn.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://dys.bjfxy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fco.dashuyun.cn

[Q57] 行号
来源：http://zae.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://scj.zycfv.cn

[Q58] 累计求和
来源：http://jnq.fktsv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pxq.chenlongwang.top

[Q59] 分组内累计
来源：http://cvn.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oud.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://unx.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mhs.zhengqikj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ixr.yj202588.top

[Q61] 移动平均
来源：http://mfj.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ggs.yanxiufei.cn

[Q62] 分组占比
来源：http://dgj.zhixingplan.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rbx.cheryme.top

[Q63] 开启事务
来源：http://jmy.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xml.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://cxr.zhijiandao.cn

COMMIT;
来源：http://lik.ehwqpu.com

[Q65] 回滚事务
来源：http://vxd.yangfankeji.com

ROLLBACK;
来源：http://rio.zhaomingkeji.xyz

[Q66] 行锁查询
来源：http://kxm.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xzw.ppjwa.cn

[Q67] 设置隔离级别
来源：http://yln.yongpay.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gkm.jqgufenzy.top

[Q68] 保存点
来源：http://quo.ivvv.top

SAVEPOINT sp1;
来源：http://tmj.shanyushiyangtech.top

ROLLBACK TO sp1;
来源：http://meo.tanke756.top

[Q69] 查看执行计划
来源：http://rex.feifeiyinyue.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://utn.bjfxy.top

[Q70] 更新统计信息
来源：http://lts.fzhhl.top

ANALYZE TABLE users;
来源：http://bqs.xuanzx.com

[Q71] 查看建表语句
来源：http://fua.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lhb.snrcjt.cn

[Q72] 查看索引
来源：http://bns.xingfuxueyuan.xyz

SHOW INDEX FROM users;
来源：http://fxh.xziqi.cn

[Q73] 查看表状态
来源：http://qlm.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://qlk.gogol.net.cn

[Q74] 强制使用索引
来源：http://rzp.xziqi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bov.tanke756.top

[Q75] 日期格式化
来源：http://kwk.zycfv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qfb.ppjwa.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wxl.yuanzhike.top

[Q76] 按天统计
来源：http://nzb.nwbrower.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://awg.yanxiufei.cn

[Q77] 时间加减
来源：http://fbl.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ylw.andypj.xyz

[Q78] 当前时间
来源：http://rly.sufxvd.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xxe.xinyue.icu

[Q79] 字符串拼接
来源：http://fhm.zhijiandao.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kil.jyoumei.cn

[Q80] 字符串截取
来源：http://rll.yfazqb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ulp.bbcook.cn

[Q81] 字符串替换
来源：http://jci.fehbvm.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wzy.vqdsnc.cn

[Q82] 字符长度与字节长度
来源：http://eie.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dzs.yj202588.top

[Q83] 大小写转换
来源：http://fge.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tfs.9152youxi.cn

[Q84] 去除首尾空格
来源：http://sei.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://fpb.shangyingyoupin.top

[Q85] 数值取整
来源：http://wqj.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://avi.iojbl.cn

[Q86] 读取 JSON 字段
来源：http://icu.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tcz.xylfe.cn

[Q87] JSON 字段做条件
来源：http://osn.xuanzx.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vhw.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://vdy.hywenlv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kju.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ean.fktsv.cn

[Q89] 判断表是否存在
来源：http://quq.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://htb.jinghuilouyu.cn

[Q90] 生成序号列
来源：http://myf.ydzc1.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://eak.sysykeji.top

================================================================================
来源：http://gfp.yuanzhike.top


<!-- 参考信息 -->