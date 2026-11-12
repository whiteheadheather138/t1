代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mzx.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://zgh.pycfn.com

C#:   async Task F() { await G(); }
来源：http://oou.sufxvd.cn

[O05] 并发执行并等待全部完成
来源：http://wkx.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://qmd.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qwa.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://klu.zhixingplan.top

TS:   await Promise.all(tasks)
来源：http://hdm.tarul.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://emu.dashuyun.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gte.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://kvi.fehbvm.com

C#:   await Task.WhenAll(t1, t2)
来源：http://lrl.guowangkeji.top

[O06] 使用进程池
来源：http://nqh.epnwcf.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aii.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cyi.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://zcc.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://jfy.yj20258888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pcx.nanxuanxn.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nuq.sysykeji.top

Ruby: // fork 块
来源：http://soz.xylfe.cn

C#:   Parallel.For
来源：http://qhr.yj20258.top

================================================================================
来源：http://snl.hfpthk.cn

P. 常用工具函数
来源：http://tnz.snrcjt.cn

================================================================================
来源：http://szz.jqgfzy.top

[P01] 生成 UUID
来源：http://fnd.hesvh.cn

Py:   str(uuid.uuid4())
来源：http://srf.ywan-chungtsiang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wrg.xinyue.icu

JS:   crypto.randomUUID()
来源：http://pyb.iojbl.cn

TS:   crypto.randomUUID()
来源：http://aqk.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://hys.cucudq.cn

Go:   // 用 github.com/google/uuid
来源：http://sus.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://eiv.cashguo.top

C#:   Guid.NewGuid().ToString()
来源：http://ogj.hongshengwenyu.top

[P02] MD5 / SHA256 摘要
来源：http://bqb.shanyushiyangtech.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nho.sysykeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zqf.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wsm.cdnleiting.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gwm.xuanzx.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ooo.tianlin.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://irv.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lwl.meibo888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yho.jinqigufen.top

[P03] 生成短随机字符串
来源：http://tgx.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://edf.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vge.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cgu.fzhhl.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ege.cdnleiting.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gqi.nanxinkj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://skg.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gtg.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://int.aizwys.cn

[P04] 求长度
来源：http://ysx.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xni.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rzx.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://okl.tianlin.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bfs.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://faa.hnqzz.top

Go:   len(arr);  len(m)
来源：http://lau.epnwcf.com

Ruby: x.length;  x.size
来源：http://uoe.uphjek.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://nzx.svipenyu.cn

[P05] 判断两个对象内容是否相等
来源：http://sxm.zhixingplan.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nlz.zhiwuduotai.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zpu.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://art.yj20258.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lsr.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://osl.shzxlz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nop.yuanzhike.top

Ruby: a == b
来源：http://brw.daxiang520.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wmo.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qjk.nanxinkj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xwl.nanxuanxn.top

PHP:  if (empty($x)) {}
来源：http://piy.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kum.hfpthk.cn

TS:   if (x == null) {}
来源：http://hwp.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://utf.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://twv.hfpthk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ckl.xziqi.cn

C#:   if (x is null) {}
来源：http://asg.jinqigfzy.top

[P07] 防抖与节流
来源：http://dki.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qkk.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://zpi.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aih.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sta.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iae.gaohongyu789.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ock.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fmt.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sgl.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://isz.uphjek.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jqy.cashguo.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iyr.jinqigfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dmt.zhiwuduotai.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vjp.meibo888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://crv.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vxh.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xkk.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://upg.yanxiufei.cn

================================================================================
来源：http://sng.cqqwz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://epo.zycfv.cn

================================================================================
来源：http://byd.yj20258888.top

[Q01] 创建表
来源：http://xok.hnqzz.top

CREATE TABLE users (
来源：http://rgw.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://llr.sufxvd.cn

name VARCHAR(50) NOT NULL,
来源：http://kow.zhiwuduotai.top

email VARCHAR(100) UNIQUE,
来源：http://qrt.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://smf.iojbl.cn

);
来源：http://cuy.xuanzx.com

[Q02] 创建带外键的表
来源：http://qvi.0kj1m.cn

CREATE TABLE orders (
来源：http://dkb.zhoulong.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ifj.hcnkem.com

user_id INT NOT NULL,
来源：http://nss.fktsv.cn

amount DECIMAL(10, 2),
来源：http://cxx.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://awo.meibo888.top

);
来源：http://arh.ydzc1.top

[Q03] 增加列
来源：http://pvh.cdnleiting.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ybc.zhiwuduotai.top

[Q04] 修改列类型
来源：http://nms.bjfxy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://joo.hesvh.cn

[Q05] 重命名列
来源：http://qza.sufxvd.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jtx.ydjk.org.cn

[Q06] 删除列
来源：http://cax.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://xzl.gaohongyu789.top

[Q07] 删除表
来源：http://sok.nanxuanxn.top

DROP TABLE IF EXISTS orders;
来源：http://vxr.cucudq.cn

[Q08] 创建普通索引
来源：http://hwb.hfpthk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wkh.cashguo.top

[Q09] 创建唯一索引
来源：http://msh.52xcode.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://llk.zhijiandao.cn

[Q10] 插入单行
来源：http://trp.xinyue.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iho.jlsjyb.cn

[Q11] 一次插入多行
来源：http://ctx.fktsv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fvc.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://juj.yj202588.top

INSERT INTO users (name) VALUES ('C');
来源：http://vjk.birdmap.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://swk.c1oappe.top

[Q13] 忽略重复插入
来源：http://mtr.zycfv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wej.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://fsp.bjfxy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sxc.iojbl.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mob.hywenlv.cn

[Q15] 查询全部
来源：http://krf.xuanzx.com

SELECT * FROM users;
来源：http://yrh.zdbjq.cn

[Q16] 查询指定列
来源：http://fwp.ehwqpu.com

SELECT id, name FROM users;
来源：http://sjl.xingfuxueyuan.xyz

[Q17] 条件查询
来源：http://hgt.hesvh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iit.ybcxt.top

[Q18] 模糊匹配
来源：http://yhn.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://msg.zhoulong.xyz

[Q19] 范围查询
来源：http://gdz.fehbvm.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ans.dianchejie.cn

[Q20] IN 列表
来源：http://dnd.redwolf501.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ujh.sysykeji.top

[Q21] 空值判断
来源：http://onq.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tcb.xingfuxueyuan.xyz

[Q22] 排序
来源：http://jkn.xuetiantiany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bbt.xziqi.cn

[Q23] 分页
来源：http://tmg.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qfo.tian-w.cn

[Q24] 去重
来源：http://liu.haohaochexian.top

SELECT DISTINCT city FROM users;
来源：http://sug.ydzc1.top

[Q25] 只取前 N 条
来源：http://rry.gogol.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ija.zdqjudy.top

[Q26] 计数
来源：http://avh.dianchejie.cn

SELECT COUNT(*) FROM users;
来源：http://gns.birdmap.top

[Q27] 条件计数
来源：http://sir.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ylu.fehbvm.com

[Q28] 求和与平均
来源：http://ilj.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://doi.chenjidiqi.icu

[Q29] 最大最小值
来源：http://xqd.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kwm.ybcxt.top

[Q30] 分组统计
来源：http://hnb.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ggw.tianlin.xyz

[Q31] 分组后过滤
来源：http://mhz.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bnx.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://pdx.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wno.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wfn.zhijiandao.cn

[Q33] 多列分组
来源：http://nhq.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tgb.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://ret.yj202588.top

SELECT * FROM (
来源：http://lps.fktsv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nlg.yanxiufei.cn

) t WHERE rn = 1;
来源：http://utl.yj202588.top

[Q35] 内连接
来源：http://mao.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sio.yj20258888.top

[Q36] 左连接
来源：http://pjl.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://clz.hcnkem.com

[Q37] 右连接
来源：http://bpi.chenjidiqi.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hqk.bbcook.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zbe.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vmo.havefunace.top

[Q39] 自连接（查上下级）
来源：http://mhf.nanxuanxn.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wgq.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lej.hnqzz.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gtl.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pse.hnqzz.top

[Q41] 多表连接
来源：http://bcv.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://ifm.uphjek.com

JOIN users u ON u.id = o.user_id
来源：http://nbu.hammf.cn

JOIN products p ON p.id = o.product_id;
来源：http://dny.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://zja.ctjpmb.com

SELECT u.name, o.amount FROM users u
来源：http://yda.andypj.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://euh.sxryk.cn

[Q43] 标量子查询
来源：http://yep.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xmh.dianchejie.cn

[Q44] IN 子查询
来源：http://vwv.nanxuanxn.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://org.c1oappe.top

[Q45] EXISTS 判断存在
来源：http://iso.birdmap.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://abo.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://uog.zycfv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nrw.xuetiantiany.cn

[Q47] 与平均值比较
来源：http://wdp.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uur.xingfuxueyuan.xyz

[Q48] CTE 公用表表达式
来源：http://gso.ydjk.org.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://chp.hongshengwenyu.top

SELECT * FROM t WHERE c > 5;
来源：http://ltw.dianchejie.cn

[Q49] 更新单行
来源：http://qzr.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://euq.yonumen.top

[Q50] 批量更新
来源：http://gcr.vqdsnc.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oge.shanyushiyangtech.top

[Q51] 用子查询更新
来源：http://hfq.tian-w.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rkq.aizwys.cn

[Q52] 删除指定行
来源：http://vns.yj20258888.top

DELETE FROM users WHERE id = 10;
来源：http://vqa.fehbvm.com

[Q53] 按条件删除
来源：http://lme.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fgz.feifeiyinyue.top

[Q54] 清空表
来源：http://xnl.sysykeji.top

TRUNCATE TABLE logs;
来源：http://lqk.yongpay.top

[Q55] 排名（并列占位）
来源：http://llp.andypj.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hqh.jlsjyb.cn

[Q56] 密集排名（并列不占位）
来源：http://ybv.cheryme.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vrf.jqgfzy.top

[Q57] 行号
来源：http://mfy.yanxiufei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ssj.yuanzhike.top

[Q58] 累计求和
来源：http://wzo.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nkd.shuidangran.top

[Q59] 分组内累计
来源：http://bzi.nanxuanxn.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ykx.52xcode.cn

[Q60] 取上一行 / 下一行
来源：http://sff.hnxiangtu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://huc.hysaishi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uox.ydjk.org.cn

[Q61] 移动平均
来源：http://tmc.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cjc.hnxiangtu.top

[Q62] 分组占比
来源：http://fmq.yuxming.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bvl.svipenyu.cn

[Q63] 开启事务
来源：http://lft.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://guu.jinqigfzy.top

[Q64] 提交事务
来源：http://hif.0kj1m.cn

COMMIT;
来源：http://tpc.pycfn.com

[Q65] 回滚事务
来源：http://plx.tarul.cn

ROLLBACK;
来源：http://xnt.guannengcc.top

[Q66] 行锁查询
来源：http://wdz.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tti.shanyushiyangkeji.top

[Q67] 设置隔离级别
来源：http://huy.tian-w.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lze.zhoulong.xyz

[Q68] 保存点
来源：http://tyb.yonumen.top

SAVEPOINT sp1;
来源：http://nvu.gzhubu.top

ROLLBACK TO sp1;
来源：http://rzy.52xcode.cn

[Q69] 查看执行计划
来源：http://zcf.zhaomingkeji.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yit.sweek.top

[Q70] 更新统计信息
来源：http://vaj.birdmap.top

ANALYZE TABLE users;
来源：http://imu.sjlbkw.cn

[Q71] 查看建表语句
来源：http://iid.hammf.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hwj.zhijiandao.cn

[Q72] 查看索引
来源：http://uvx.52xcode.cn

SHOW INDEX FROM users;
来源：http://fsz.cqqwz.cn

[Q73] 查看表状态
来源：http://iaq.haohaochexian.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lfo.sufxvd.cn

[Q74] 强制使用索引
来源：http://yna.yangfankeji.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://shx.xuanzx.com

[Q75] 日期格式化
来源：http://hsq.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wpr.jiagoushi.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ipr.fengsongda.top

[Q76] 按天统计
来源：http://sah.andypj.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xfl.yueranfly.top

[Q77] 时间加减
来源：http://ewv.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wig.pycfn.com

[Q78] 当前时间
来源：http://mmd.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uux.smart0.xyz

[Q79] 字符串拼接
来源：http://ptl.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://weu.jqgfzy.top

[Q80] 字符串截取
来源：http://ppz.hammf.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jmr.ybcxt.top

[Q81] 字符串替换
来源：http://kon.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xho.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://czw.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kwx.hywenlv.cn

[Q83] 大小写转换
来源：http://tqa.wangshuangyany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bpa.sysykeji.top

[Q84] 去除首尾空格
来源：http://ymt.xuetiantiany.cn

SELECT TRIM(name) FROM users;
来源：http://vfj.birdmap.top

[Q85] 数值取整
来源：http://omm.snrcjt.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://foe.sysykeji.top

[Q86] 读取 JSON 字段
来源：http://ohy.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kao.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://xjf.yj20258.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wdg.hcnkem.com

[Q88] 行转列（条件聚合）
来源：http://ngp.sufxvd.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jeq.cashguo.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mym.snrcjt.cn

[Q89] 判断表是否存在
来源：http://yeb.zhoulong.xyz


<!-- 参考信息 -->