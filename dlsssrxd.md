代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://flz.fktsv.cn

C#:   lock (gate) { shared++; }
来源：http://wtm.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://yhr.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://ryn.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vfe.xziqi.cn

JS:   async function f() { await g(); }
来源：http://xla.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qvn.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fry.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rhk.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://hjl.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://jow.xuanzx.com

[O05] 并发执行并等待全部完成
来源：http://rvy.redwolf501.top

Py:   asyncio.gather(*tasks)
来源：http://rbp.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cbr.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://mek.zhixingplan.top

TS:   await Promise.all(tasks)
来源：http://plm.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://scq.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://clx.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://ldw.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cpk.epnwcf.com

[O06] 使用进程池
来源：http://ofw.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uzp.ppjwa.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://iye.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://evx.quarkkingdee.top

TS:   // child_process / cluster 模块
来源：http://vyd.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yvk.tian-w.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ohk.chenjidiqi.icu

Ruby: // fork 块
来源：http://jjw.cqqwz.cn

C#:   Parallel.For
来源：http://tws.zhijiandao.cn

================================================================================
来源：http://tib.cashguo.top

P. 常用工具函数
来源：http://jeb.hysaishi.cn

================================================================================
来源：http://pqn.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://ydf.xziqi.cn

Py:   str(uuid.uuid4())
来源：http://ktx.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vmt.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://gvw.gogol.net.cn

TS:   crypto.randomUUID()
来源：http://ahu.zdbjq.cn

Java: UUID.randomUUID().toString()
来源：http://rvs.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://kzz.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://ksj.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://xrv.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://qum.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ctx.xuanzx.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://sdn.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wcu.redwolf501.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jlh.guannengcc.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kfb.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ojd.ctjpmb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qsg.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fai.nanxinkj.top

[P03] 生成短随机字符串
来源：http://ftl.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lgh.nanxinkj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gjr.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zzz.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ipr.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mxm.quarkkingdee.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vus.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vus.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blr.fzhhl.top

[P04] 求长度
来源：http://vim.hfpthk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ijj.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nfv.svipenyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dum.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://niy.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://jnw.yongpay.top

Go:   len(arr);  len(m)
来源：http://gct.jqgfzy.top

Ruby: x.length;  x.size
来源：http://tfl.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rfl.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://bus.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nsv.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://stp.yuxming.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cgu.yangfankeji.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vam.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://egd.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://glg.yj20258.top

Ruby: a == b
来源：http://htk.mhx1999.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ttv.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://maa.316326.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pom.zhoulong.xyz

PHP:  if (empty($x)) {}
来源：http://odr.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wvm.gzhubu.top

TS:   if (x == null) {}
来源：http://zpb.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hrr.xylfe.cn

Go:   if x == nil {}
来源：http://yxd.xuetiantiany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nwm.ydjk.org.cn

C#:   if (x is null) {}
来源：http://kqc.bjfxy.top

[P07] 防抖与节流
来源：http://wug.sjlbkw.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mip.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://oen.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ncv.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bar.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kka.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nlq.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://iya.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hba.c1oappe.top

[P08] 处理浮点精度问题
来源：http://yok.hcnkem.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pqw.fktsv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fhc.gogol.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jyw.hywenlv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tvt.xinyue.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aaf.hesvh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qeg.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cnp.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xtw.fehbvm.com

================================================================================
来源：http://jon.jiagoushi.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jog.zdqjudy.top

================================================================================
来源：http://ugp.jinyuanbaomall.cn

[Q01] 创建表
来源：http://azo.cheryme.top

CREATE TABLE users (
来源：http://aux.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ftm.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://xoa.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://ptj.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mwv.chenzaomai.com

);
来源：http://csh.meibo888.top

[Q02] 创建带外键的表
来源：http://goh.52xcode.cn

CREATE TABLE orders (
来源：http://mcv.hongshengwenyu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://igo.wangdashe.top

user_id INT NOT NULL,
来源：http://ncu.yanxiufei.cn

amount DECIMAL(10, 2),
来源：http://iec.jiagoushi.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://brz.yonumen.top

);
来源：http://dwn.shanyushiyangkeji.top

[Q03] 增加列
来源：http://eqf.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rrz.ivvv.top

[Q04] 修改列类型
来源：http://vpd.gzhubu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eok.yuanzhike.top

[Q05] 重命名列
来源：http://wsf.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cji.yj20258888.top

[Q06] 删除列
来源：http://tvb.yvedp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yyl.sysykeji.top

[Q07] 删除表
来源：http://huj.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://wjl.ivvv.top

[Q08] 创建普通索引
来源：http://rqw.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sry.meibo888.top

[Q09] 创建唯一索引
来源：http://qsl.yonumen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xod.jiagoushi.top

[Q10] 插入单行
来源：http://nvo.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tab.daxiang520.top

[Q11] 一次插入多行
来源：http://ldf.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qil.xingfuxueyuan.xyz

[Q12] 插入后取自增 ID
来源：http://raf.wangshuangyany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dqk.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wdd.birdmap.top

[Q13] 忽略重复插入
来源：http://ksf.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ffo.yj20258888.top

[Q14] 存在则更新（upsert）
来源：http://aqq.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qpi.yanxiufei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pvq.tian-w.cn

[Q15] 查询全部
来源：http://zxv.xinyue.icu

SELECT * FROM users;
来源：http://ewp.zhijiandao.cn

[Q16] 查询指定列
来源：http://svc.daria6918.cn

SELECT id, name FROM users;
来源：http://vlt.cdnleiting.top

[Q17] 条件查询
来源：http://ifp.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dff.xylfe.cn

[Q18] 模糊匹配
来源：http://rbh.zhoulong.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wqz.ydzc1.top

[Q19] 范围查询
来源：http://zrj.smart0.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hhd.shzxlz.cn

[Q20] IN 列表
来源：http://sdo.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cgj.aibaodan.cn

[Q21] 空值判断
来源：http://ipf.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rix.yj20258.top

[Q22] 排序
来源：http://vmg.nwbrower.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zhg.yangfankeji.com

[Q23] 分页
来源：http://dhz.shanyushiyangtech.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ejs.aizwys.cn

[Q24] 去重
来源：http://kog.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://tmb.316326.xyz

[Q25] 只取前 N 条
来源：http://zwa.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wpy.fengsongda.top

[Q26] 计数
来源：http://buo.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://fyn.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://mwc.yj20258.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ikh.vehdjk.com

[Q28] 求和与平均
来源：http://gfv.jiagoushi.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wzm.wangshuangyany.cn

[Q29] 最大最小值
来源：http://snd.svipenyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xfv.ydjk.org.cn

[Q30] 分组统计
来源：http://rba.gaohongyu789.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hot.ydzc1.top

[Q31] 分组后过滤
来源：http://wkx.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lad.shangyingyoupin.top

[Q32] 分组拼接字符串
来源：http://gag.chenzaomai.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vrw.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jgi.hfpthk.cn

[Q33] 多列分组
来源：http://rkp.yongpay.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dvh.yj202588.top

[Q34] 每组取第一条
来源：http://oxi.ehwqpu.com

SELECT * FROM (
来源：http://hhz.jyoumei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ogy.aizwys.cn

) t WHERE rn = 1;
来源：http://tvv.sweek.top

[Q35] 内连接
来源：http://zmg.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yae.fanxiaobao.xyz

[Q36] 左连接
来源：http://vxm.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ghi.yuxming.cn

[Q37] 右连接
来源：http://orz.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://znh.sxryk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nus.pengpengdd.cyou

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qfl.nwbrower.top

[Q39] 自连接（查上下级）
来源：http://rsv.snrcjt.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uuz.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mnc.cheryme.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ibb.svipenyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dtr.ehwqpu.com

[Q41] 多表连接
来源：http://cie.jyoumei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gld.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://bpj.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://mqh.sjlbkw.cn

[Q42] 连接条件附加过滤
来源：http://ggp.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://qql.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ztu.hywenlv.cn

[Q43] 标量子查询
来源：http://izm.hnxiangtu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://icc.yongpay.top

[Q44] IN 子查询
来源：http://yzl.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lcm.nanxinkj.top

[Q45] EXISTS 判断存在
来源：http://pdq.xylfe.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gwn.uphjek.com

[Q46] NOT EXISTS 判断不存在
来源：http://tmj.hysaishi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ilf.jinqigufen.top

[Q47] 与平均值比较
来源：http://jur.zhoulong.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bah.xziqi.cn

[Q48] CTE 公用表表达式
来源：http://iun.sysykeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://enz.cqqwz.cn

SELECT * FROM t WHERE c > 5;
来源：http://igv.nanxuanxn.top

[Q49] 更新单行
来源：http://tfr.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sop.yonumen.top

[Q50] 批量更新
来源：http://kbv.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uro.uphjek.com

[Q51] 用子查询更新
来源：http://tbs.nanxinkj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qca.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://sxz.hongshengwenyu.top

DELETE FROM users WHERE id = 10;
来源：http://duh.hywenlv.cn

[Q53] 按条件删除
来源：http://coj.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rvu.meibo888.top

[Q54] 清空表
来源：http://yrd.sufxvd.cn

TRUNCATE TABLE logs;
来源：http://euf.wangdashe.top

[Q55] 排名（并列占位）
来源：http://wyb.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xbx.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://wyo.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lak.meibo888.top

[Q57] 行号
来源：http://wpt.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://scf.pengpengdd.cyou

[Q58] 累计求和
来源：http://umv.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://srm.fehbvm.com

[Q59] 分组内累计
来源：http://dpo.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://chf.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://mae.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lik.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lwv.vehdjk.com

[Q61] 移动平均
来源：http://vlj.birdmap.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jlb.xuetiantiany.cn

[Q62] 分组占比
来源：http://ofk.shangyingyoupin.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oah.hesvh.cn

[Q63] 开启事务
来源：http://wbd.cashguo.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qyy.snrcjt.cn

[Q64] 提交事务
来源：http://njk.gaohongyu789.top

COMMIT;
来源：http://lar.ydzc1.top

[Q65] 回滚事务
来源：http://maw.birdmap.top

ROLLBACK;
来源：http://yzc.tianlin.xyz

[Q66] 行锁查询
来源：http://txm.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cpg.xinyue.icu

[Q67] 设置隔离级别
来源：http://hsl.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vfa.yj20258.top

[Q68] 保存点
来源：http://cti.zdbjq.cn

SAVEPOINT sp1;
来源：http://omi.tanke756.top

ROLLBACK TO sp1;
来源：http://byk.fanxiaobao.xyz

[Q69] 查看执行计划
来源：http://rqc.zhiwuduotai.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tcs.chenzaomai.com

[Q70] 更新统计信息
来源：http://wcf.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://ccg.tarul.cn

[Q71] 查看建表语句
来源：http://uti.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nnu.yueranfly.top

[Q72] 查看索引
来源：http://rmm.guowangkeji.top

SHOW INDEX FROM users;
来源：http://oqo.jinqigufen.top

[Q73] 查看表状态
来源：http://kdh.yongpay.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jkv.dashuyun.cn

[Q74] 强制使用索引
来源：http://jjj.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://twc.gaohongyu789.top

[Q75] 日期格式化
来源：http://yeg.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xpr.xuanzx.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ndp.ppjwa.cn

[Q76] 按天统计
来源：http://nxc.fzhhl.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mxh.ybcxt.top

[Q77] 时间加减
来源：http://iwc.iojbl.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ubm.nwbrower.top

[Q78] 当前时间
来源：http://nkk.yanxiufei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bjj.dianchejie.cn

[Q79] 字符串拼接
来源：http://sfq.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dif.jianghu66.top

[Q80] 字符串截取
来源：http://taf.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zbw.chenjidiqi.icu

[Q81] 字符串替换
来源：http://uzf.daxiang520.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nxn.cqqwz.cn

[Q82] 字符长度与字节长度
来源：http://plb.yueranfly.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wgv.ppjwa.cn

[Q83] 大小写转换
来源：http://uff.yj20258.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gzx.tian-w.cn

[Q84] 去除首尾空格
来源：http://hlo.hfpthk.cn

SELECT TRIM(name) FROM users;
来源：http://xdy.smart0.xyz

[Q85] 数值取整
来源：http://tgg.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xfm.wangshuangyany.cn


<!-- 参考信息 -->