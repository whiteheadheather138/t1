代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iql.guannengcc.top

TS:   // 同 JS
来源：http://xwq.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://yon.pycfn.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sfr.hammf.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ueg.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://vbs.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://tme.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://rhq.sufxvd.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ywi.zycfv.cn

JS:   async function f() { await g(); }
来源：http://emd.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wlm.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tio.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gmy.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iio.yongpay.top

C#:   async Task F() { await G(); }
来源：http://oic.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://yab.jlsjyb.cn

Py:   asyncio.gather(*tasks)
来源：http://qaa.svipenyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gfn.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://xap.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://fvq.hesvh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hrq.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ypg.fzhhl.top

Ruby: threads.map(&:join)
来源：http://dak.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xwr.xingfuxueyuan.xyz

[O06] 使用进程池
来源：http://gyj.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zlf.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://dme.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://yhq.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://ltj.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gby.tian-w.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uks.yj202588.top

Ruby: // fork 块
来源：http://nau.jianghu66.top

C#:   Parallel.For
来源：http://lat.ctjpmb.com

================================================================================
来源：http://qdb.sysykeji.top

P. 常用工具函数
来源：http://jyx.jianghu66.top

================================================================================
来源：http://yat.bbcook.cn

[P01] 生成 UUID
来源：http://fkq.316326.xyz

Py:   str(uuid.uuid4())
来源：http://ohc.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sxv.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://gof.xingfuxueyuan.xyz

TS:   crypto.randomUUID()
来源：http://ero.cucudq.cn

Java: UUID.randomUUID().toString()
来源：http://jps.fehbvm.com

Go:   // 用 github.com/google/uuid
来源：http://cby.zycfv.cn

Ruby: SecureRandom.uuid
来源：http://bot.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://piw.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://tbw.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zfc.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tvp.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vxp.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tqc.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ebf.uphjek.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://okb.hesvh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xmx.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fvz.guowangkeji.top

[P03] 生成短随机字符串
来源：http://tfz.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tqb.gzhubu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wki.guowangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pga.sweek.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ynl.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://avq.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qog.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fay.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yzj.jqgufenzy.top

[P04] 求长度
来源：http://obr.yuanzhike.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ybt.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ehw.yangfankeji.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dcq.jqgufenzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ewo.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://mec.jinyuanbaomall.cn

Go:   len(arr);  len(m)
来源：http://gqm.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://okj.tarul.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ben.hcnkem.com

[P05] 判断两个对象内容是否相等
来源：http://mmv.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mve.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rrn.tarul.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yxc.sxryk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wus.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qjn.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://shb.vehdjk.com

Ruby: a == b
来源：http://zwg.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kdd.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gtd.yonumen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wxr.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://itb.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lya.c1oappe.top

TS:   if (x == null) {}
来源：http://tmh.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ahl.gotoacloud.top

Go:   if x == nil {}
来源：http://eoz.fanxiaobao.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ocm.haohaochexian.top

C#:   if (x is null) {}
来源：http://wgu.dianchejie.cn

[P07] 防抖与节流
来源：http://vvg.fktsv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bln.tarul.cn

PHP:  // 手写时间戳比较
来源：http://qdu.cdnleiting.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://msd.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wci.hnqzz.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dnl.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://frz.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jls.xziqi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qbs.dianchejie.cn

[P08] 处理浮点精度问题
来源：http://oev.quarkkingdee.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fms.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lgs.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hfr.hywenlv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://djn.0kj1m.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zhh.chenjidiqi.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kaz.hywenlv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://olx.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gez.fzhhl.top

================================================================================
来源：http://nnp.gogol.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tjq.birdmap.top

================================================================================
来源：http://dru.yj20258.top

[Q01] 创建表
来源：http://jjt.ybcxt.top

CREATE TABLE users (
来源：http://mwh.zhaomingkeji.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wvn.hnqzz.top

name VARCHAR(50) NOT NULL,
来源：http://cyf.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://ozg.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eoo.tarul.cn

);
来源：http://tbb.fengsongda.top

[Q02] 创建带外键的表
来源：http://eax.uphjek.com

CREATE TABLE orders (
来源：http://kdv.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ggh.yuanzhike.top

user_id INT NOT NULL,
来源：http://kwk.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://jqb.yuanzhike.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rur.chenzaomai.com

);
来源：http://cpl.yuanzhike.top

[Q03] 增加列
来源：http://uwq.andypj.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dny.yj20258.top

[Q04] 修改列类型
来源：http://aaz.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pda.zdbjq.cn

[Q05] 重命名列
来源：http://rhk.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wei.xylfe.cn

[Q06] 删除列
来源：http://qrm.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://ruu.vehdjk.com

[Q07] 删除表
来源：http://qrr.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://mvo.fehbvm.com

[Q08] 创建普通索引
来源：http://pdo.ivvv.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ygg.c1oappe.top

[Q09] 创建唯一索引
来源：http://fwc.xinyue.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kco.gaohongyu789.top

[Q10] 插入单行
来源：http://rxx.vehdjk.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://amz.xuanzx.com

[Q11] 一次插入多行
来源：http://fnk.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wml.cheryme.top

[Q12] 插入后取自增 ID
来源：http://sae.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ckn.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://owo.andypj.xyz

[Q13] 忽略重复插入
来源：http://umw.jinghuilouyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mri.cheryme.top

[Q14] 存在则更新（upsert）
来源：http://wvb.cqqwz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bbr.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://thl.jinyuanbaomall.cn

[Q15] 查询全部
来源：http://jap.52xcode.cn

SELECT * FROM users;
来源：http://kyn.zhengqikj.top

[Q16] 查询指定列
来源：http://qej.vehdjk.com

SELECT id, name FROM users;
来源：http://gcb.yonumen.top

[Q17] 条件查询
来源：http://fzd.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nme.fengsongda.top

[Q18] 模糊匹配
来源：http://exd.guannengcc.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lcb.meibo888.top

[Q19] 范围查询
来源：http://yvz.hammf.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xov.tianlin.xyz

[Q20] IN 列表
来源：http://trf.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jpa.hfpthk.cn

[Q21] 空值判断
来源：http://ish.xinyue.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://bow.zhiwuduotai.top

[Q22] 排序
来源：http://dsk.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rxa.0kj1m.cn

[Q23] 分页
来源：http://scl.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aor.hesvh.cn

[Q24] 去重
来源：http://fkz.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://xho.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://crz.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ziv.0kj1m.cn

[Q26] 计数
来源：http://vfs.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://ddg.yj202588.top

[Q27] 条件计数
来源：http://kiv.yueranfly.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vip.andypj.xyz

[Q28] 求和与平均
来源：http://qdj.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vbk.yj202588.top

[Q29] 最大最小值
来源：http://xff.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://ywv.cqqwz.cn

[Q30] 分组统计
来源：http://ruq.kuanghao11.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dip.fengsongda.top

[Q31] 分组后过滤
来源：http://var.pengpengdd.cyou

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fvw.iojbl.cn

[Q32] 分组拼接字符串
来源：http://ntf.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kya.ydjk.org.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aks.feifeiyinyue.top

[Q33] 多列分组
来源：http://lrb.quarkkingdee.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://odp.yuxming.cn

[Q34] 每组取第一条
来源：http://qch.hesvh.cn

SELECT * FROM (
来源：http://juq.316326.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bjv.uphjek.com

) t WHERE rn = 1;
来源：http://bev.andypj.xyz

[Q35] 内连接
来源：http://lpj.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wws.ywan-chungtsiang.top

[Q36] 左连接
来源：http://jfx.andypj.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kcz.nanxinkj.top

[Q37] 右连接
来源：http://qvm.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ngs.xziqi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ipf.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ppn.feifeiyinyue.top

[Q39] 自连接（查上下级）
来源：http://ski.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fgo.dashuyun.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://msj.yfazqb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://neh.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uwz.iojbl.cn

[Q41] 多表连接
来源：http://ory.hesvh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uhg.xingfuxueyuan.xyz

JOIN users u ON u.id = o.user_id
来源：http://pee.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://cvq.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://sas.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://aua.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ume.fzhhl.top

[Q43] 标量子查询
来源：http://ktx.cheryme.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tev.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://nnz.hongshengwenyu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://edv.guowangkeji.top

[Q45] EXISTS 判断存在
来源：http://atg.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://shv.hysaishi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dbj.jlsjyb.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ipb.hfpthk.cn

[Q47] 与平均值比较
来源：http://tqu.zycfv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dea.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://iqz.yuanzhike.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zbu.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://jvd.sxryk.cn

[Q49] 更新单行
来源：http://rbv.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://irc.yvedp.cn

[Q50] 批量更新
来源：http://pvr.fehbvm.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://psn.fzhhl.top

[Q51] 用子查询更新
来源：http://yaw.jiagoushi.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blo.nanxuanxn.top

[Q52] 删除指定行
来源：http://tnc.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://got.yvedp.cn

[Q53] 按条件删除
来源：http://wek.c1oappe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://atq.tianlin.xyz

[Q54] 清空表
来源：http://akp.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://yah.hnqzz.top

[Q55] 排名（并列占位）
来源：http://nmo.smart0.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fdx.zhiwuduotai.top

[Q56] 密集排名（并列不占位）
来源：http://wja.cqqwz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hdf.tian-w.cn

[Q57] 行号
来源：http://rss.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pwz.ydjk.org.cn

[Q58] 累计求和
来源：http://ttc.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vqr.sweek.top

[Q59] 分组内累计
来源：http://wby.yongpay.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zpv.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://evi.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vgx.bjfxy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dxh.xuanzx.com

[Q61] 移动平均
来源：http://sqw.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ryx.guannengcc.top

[Q62] 分组占比
来源：http://gwk.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://byb.ydzc1.top

[Q63] 开启事务
来源：http://yid.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://woc.chenjidiqi.icu

[Q64] 提交事务
来源：http://lwe.tianlin.xyz

COMMIT;
来源：http://cgg.zdqjudy.top

[Q65] 回滚事务
来源：http://lqg.zhengqikj.top

ROLLBACK;
来源：http://pea.ehwqpu.com

[Q66] 行锁查询
来源：http://zgl.pycfn.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kbt.gzhubu.top

[Q67] 设置隔离级别
来源：http://ltv.sysykeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://stx.sjlbkw.cn

[Q68] 保存点
来源：http://zxs.cqqwz.cn

SAVEPOINT sp1;
来源：http://vof.mhx1999.top

ROLLBACK TO sp1;
来源：http://rco.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://wgz.gzhubu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://utt.zdbjq.cn

[Q70] 更新统计信息
来源：http://vei.tanke756.top

ANALYZE TABLE users;
来源：http://glt.nanxuanxn.top

[Q71] 查看建表语句
来源：http://tqq.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ujm.fanxiaobao.xyz

[Q72] 查看索引
来源：http://pzz.hcnkem.com

SHOW INDEX FROM users;
来源：http://kgu.xinyue.icu

[Q73] 查看表状态
来源：http://tve.chenlongwang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uib.yangfankeji.com

[Q74] 强制使用索引
来源：http://wzu.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bzj.0kj1m.cn

[Q75] 日期格式化
来源：http://qxw.dashuyun.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nci.jianghu66.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lnz.sxryk.cn

[Q76] 按天统计
来源：http://pgr.gaohongyu789.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zvr.sjlbkw.cn

[Q77] 时间加减
来源：http://zzc.jyoumei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zaw.chenzaomai.com

[Q78] 当前时间
来源：http://rjg.andypj.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fnh.yuanzhike.top

[Q79] 字符串拼接
来源：http://nkz.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tvz.hcnkem.com

[Q80] 字符串截取
来源：http://hsp.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ais.vehdjk.com

[Q81] 字符串替换
来源：http://vxt.shanyushiyangtech.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mwo.sxryk.cn

[Q82] 字符长度与字节长度
来源：http://ijb.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sub.sysykeji.top

[Q83] 大小写转换
来源：http://cry.fktsv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kjp.nanxinkj.top


<!-- 参考信息 -->