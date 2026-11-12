代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://ptz.ppjwa.cn

Go:   go f()
来源：http://odg.xuanzx.com

Ruby: Thread.new { f }
来源：http://etp.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://ife.cqqwz.cn

[O02] 使用线程池
来源：http://cgm.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qzw.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://juk.yanxiufei.cn

JS:   // worker_threads 线程池
来源：http://rwd.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://ffu.cucudq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ekf.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fln.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://inq.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tvl.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://uon.guannengcc.top

Py:   with lock: shared += 1
来源：http://ngx.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://mph.zhixingplan.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ujr.ivvv.top

TS:   // 同 JS
来源：http://wlz.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://his.sjlbkw.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zov.fehbvm.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://mqt.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://gpi.yj202588.top

[O04] 定义异步函数并等待
来源：http://veu.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://ota.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pve.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://xbd.gaohongyu789.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://onm.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ebl.andypj.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gjp.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kfx.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://hlh.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://hoe.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://cid.feifeiyinyue.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://trf.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://tdb.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://iqm.wangdashe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rby.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://beo.tanke756.top

Ruby: threads.map(&:join)
来源：http://jvs.gogol.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://krp.fehbvm.com

[O06] 使用进程池
来源：http://hzi.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wgv.fengsongda.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fnf.vqdsnc.cn

JS:   // child_process / cluster 模块
来源：http://asy.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://xxe.xinyue.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hki.iojbl.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sdt.bjfxy.top

Ruby: // fork 块
来源：http://uyo.c1oappe.top

C#:   Parallel.For
来源：http://nxj.0kj1m.cn

================================================================================
来源：http://iuf.0kj1m.cn

P. 常用工具函数
来源：http://zpq.xuetiantiany.cn

================================================================================
来源：http://sxd.vqdsnc.cn

[P01] 生成 UUID
来源：http://ttl.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://cus.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gth.redwolf501.top

JS:   crypto.randomUUID()
来源：http://yhk.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://mci.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://twf.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://trk.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://dzr.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://mwz.fengsongda.top

[P02] MD5 / SHA256 摘要
来源：http://vos.jinqigufen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pxx.ehwqpu.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://xyi.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dbe.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lxk.yangfankeji.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vjy.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xxs.ydzc1.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://usy.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zvo.zycfv.cn

[P03] 生成短随机字符串
来源：http://eko.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sbt.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ahc.cdnleiting.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xbm.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://viu.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vnx.hywenlv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://esf.xylfe.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rej.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cye.zhixingplan.top

[P04] 求长度
来源：http://oqy.pycfn.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mpe.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cvn.tianlin.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kfb.cashguo.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ihz.0kj1m.cn

Java: list.size();  map.size();  s.length()
来源：http://ujp.tian-w.cn

Go:   len(arr);  len(m)
来源：http://vnw.ppjwa.cn

Ruby: x.length;  x.size
来源：http://lww.havefunace.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://eck.redwolf501.top

[P05] 判断两个对象内容是否相等
来源：http://kpi.jinghuilouyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://umg.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uta.fzhhl.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://exe.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tfv.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cex.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://hbs.hongshengwenyu.top

Ruby: a == b
来源：http://yib.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hwb.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rii.shangyingyoupin.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qls.cucudq.cn

PHP:  if (empty($x)) {}
来源：http://srq.hnxiangtu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yxx.52xcode.cn

TS:   if (x == null) {}
来源：http://zck.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bkw.nanxinkj.top

Go:   if x == nil {}
来源：http://itj.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pgc.hongshengwenyu.top

C#:   if (x is null) {}
来源：http://sjv.yonumen.top

[P07] 防抖与节流
来源：http://lkh.chenjidiqi.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wzb.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://adc.xylfe.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rps.yuanzhike.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yyk.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tlu.ctjpmb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ecc.hysaishi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gxw.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aot.nwbrower.top

[P08] 处理浮点精度问题
来源：http://rvd.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vpq.chenzaomai.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gja.chenlongwang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mej.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://azx.jiagoushi.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yro.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wvl.iojbl.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ojd.chenzaomai.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zfe.jqgfzy.top

================================================================================
来源：http://ens.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tnw.guannengcc.top

================================================================================
来源：http://fpp.sufxvd.cn

[Q01] 创建表
来源：http://eml.jqgfzy.top

CREATE TABLE users (
来源：http://veo.jinghuilouyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ocz.jiagoushi.top

name VARCHAR(50) NOT NULL,
来源：http://fuh.ybcxt.top

email VARCHAR(100) UNIQUE,
来源：http://lzk.jinqigfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zbr.meibo888.top

);
来源：http://ppr.sysykeji.top

[Q02] 创建带外键的表
来源：http://grk.aibaodan.cn

CREATE TABLE orders (
来源：http://aiq.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xto.tian-w.cn

user_id INT NOT NULL,
来源：http://ckx.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://rzw.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ofq.bjfxy.top

);
来源：http://uev.fktsv.cn

[Q03] 增加列
来源：http://zyo.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kwy.0kj1m.cn

[Q04] 修改列类型
来源：http://pgm.nwbrower.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lcl.sweek.top

[Q05] 重命名列
来源：http://lnj.cdnleiting.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vkm.chenjidiqi.icu

[Q06] 删除列
来源：http://eic.jinghuilouyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://udz.haohaochexian.top

[Q07] 删除表
来源：http://vdd.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://ckb.jinghuilouyu.cn

[Q08] 创建普通索引
来源：http://nzf.yvedp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hdh.snrcjt.cn

[Q09] 创建唯一索引
来源：http://mxx.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ofj.gzhubu.top

[Q10] 插入单行
来源：http://npg.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rsl.cdnleiting.top

[Q11] 一次插入多行
来源：http://qqg.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oei.feifeiyinyue.top

[Q12] 插入后取自增 ID
来源：http://nat.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://mio.jiagoushi.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pgb.dashuyun.cn

[Q13] 忽略重复插入
来源：http://qez.zdqjudy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zxo.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://lgf.fzhhl.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://doe.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wzy.redwolf501.top

[Q15] 查询全部
来源：http://jqx.vehdjk.com

SELECT * FROM users;
来源：http://tuj.birdmap.top

[Q16] 查询指定列
来源：http://him.hywenlv.cn

SELECT id, name FROM users;
来源：http://qut.chenlongwang.top

[Q17] 条件查询
来源：http://rpy.quarkkingdee.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tcy.cucudq.cn

[Q18] 模糊匹配
来源：http://hhx.jinqigfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qbm.sweek.top

[Q19] 范围查询
来源：http://emk.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zwb.mhx1999.top

[Q20] IN 列表
来源：http://kbt.hfpthk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://osf.jyoumei.cn

[Q21] 空值判断
来源：http://nit.hesvh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iad.vehdjk.com

[Q22] 排序
来源：http://jur.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gim.hysaishi.cn

[Q23] 分页
来源：http://mhp.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vqg.guannengcc.top

[Q24] 去重
来源：http://czt.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://kqh.9152youxi.cn

[Q25] 只取前 N 条
来源：http://vae.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ppr.yj202588.top

[Q26] 计数
来源：http://dac.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://dgd.jinghuilouyu.cn

[Q27] 条件计数
来源：http://shw.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bbl.yongpay.top

[Q28] 求和与平均
来源：http://azb.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ymy.zhoulong.xyz

[Q29] 最大最小值
来源：http://xvp.shanyushiyangtech.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wsk.feifeiyinyue.top

[Q30] 分组统计
来源：http://wai.52xcode.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pak.vehdjk.com

[Q31] 分组后过滤
来源：http://cvd.tianlin.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nwm.yj202588.top

[Q32] 分组拼接字符串
来源：http://jdx.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ult.hesvh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ghy.jinyuanbaomall.cn

[Q33] 多列分组
来源：http://kml.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://snk.guannengcc.top

[Q34] 每组取第一条
来源：http://mug.cashguo.top

SELECT * FROM (
来源：http://fjm.yj202588.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nwf.yongpay.top

) t WHERE rn = 1;
来源：http://qrl.zycfv.cn

[Q35] 内连接
来源：http://orj.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mza.gotoacloud.top

[Q36] 左连接
来源：http://ogy.gotoacloud.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tzt.chenzaomai.com

[Q37] 右连接
来源：http://ipr.birdmap.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mgy.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vvp.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aiw.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://uaz.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bpn.shanyushiyangtech.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yhc.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://noi.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qzj.svipenyu.cn

[Q41] 多表连接
来源：http://mnw.kuanghao11.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://oux.9152youxi.cn

JOIN users u ON u.id = o.user_id
来源：http://qcj.zycfv.cn

JOIN products p ON p.id = o.product_id;
来源：http://mzg.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://rmm.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://act.guannengcc.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://afh.sysykeji.top

[Q43] 标量子查询
来源：http://wtw.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sia.9152youxi.cn

[Q44] IN 子查询
来源：http://pkh.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://itu.wangdashe.top

[Q45] EXISTS 判断存在
来源：http://bky.tianlin.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ktx.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://euv.wangshuangyany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://akm.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://ygl.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://drw.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://jps.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vkl.zhengqikj.top

SELECT * FROM t WHERE c > 5;
来源：http://xue.nanxinkj.top

[Q49] 更新单行
来源：http://lxw.feifeiyinyue.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uas.zdbjq.cn

[Q50] 批量更新
来源：http://fdd.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zsk.fehbvm.com

[Q51] 用子查询更新
来源：http://nwn.fktsv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mbi.zhengqikj.top

[Q52] 删除指定行
来源：http://pov.ehwqpu.com

DELETE FROM users WHERE id = 10;
来源：http://hgn.fzhhl.top

[Q53] 按条件删除
来源：http://rlh.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://day.tianlin.xyz

[Q54] 清空表
来源：http://spz.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://vwz.meibo888.top

[Q55] 排名（并列占位）
来源：http://khz.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bvx.epnwcf.com

[Q56] 密集排名（并列不占位）
来源：http://bwf.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nag.ybcxt.top

[Q57] 行号
来源：http://ulb.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lbu.jqgfzy.top

[Q58] 累计求和
来源：http://bef.hfpthk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mxy.fzhhl.top

[Q59] 分组内累计
来源：http://kjv.xuanzx.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mgi.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://whc.wangshuangyany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pub.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xge.cqqwz.cn

[Q61] 移动平均
来源：http://phs.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cqh.fehbvm.com

[Q62] 分组占比
来源：http://kpi.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://egm.nanxinkj.top

[Q63] 开启事务
来源：http://rvf.xuanzx.com

START TRANSACTION;                -- 或 BEGIN
来源：http://njl.9152youxi.cn

[Q64] 提交事务
来源：http://zmd.zdqjudy.top

COMMIT;
来源：http://lzp.jinqigfzy.top

[Q65] 回滚事务
来源：http://uyx.xuanzx.com

ROLLBACK;
来源：http://jwv.jinqigfzy.top

[Q66] 行锁查询
来源：http://mlp.nanxinkj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sli.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://dik.guannengcc.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hfo.sweek.top

[Q68] 保存点
来源：http://rwd.hesvh.cn

SAVEPOINT sp1;
来源：http://jwn.jyoumei.cn

ROLLBACK TO sp1;
来源：http://cnx.hysaishi.cn

[Q69] 查看执行计划
来源：http://kam.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://thh.daria6918.cn

[Q70] 更新统计信息
来源：http://day.chenlongwang.top

ANALYZE TABLE users;
来源：http://cgd.cqqwz.cn

[Q71] 查看建表语句
来源：http://nlu.zhiwuduotai.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ejv.hywenlv.cn

[Q72] 查看索引
来源：http://qbh.cucudq.cn

SHOW INDEX FROM users;
来源：http://avf.yanxiufei.cn

[Q73] 查看表状态
来源：http://hxw.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qxd.dashuyun.cn

[Q74] 强制使用索引
来源：http://ywr.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rvx.hnxiangtu.top

[Q75] 日期格式化
来源：http://zkj.mhx1999.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gqg.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wxb.nanxinkj.top


<!-- 参考信息 -->