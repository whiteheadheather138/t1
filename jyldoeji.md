代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ykr.cashguo.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://frv.zhiwuduotai.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vpf.xylfe.cn

TS:   // 同 JS
来源：http://rhc.gzhubu.top

Java: new Thread(() -> f()).start()
来源：http://qei.xylfe.cn

Go:   go f()
来源：http://oem.xziqi.cn

Ruby: Thread.new { f }
来源：http://wqi.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://dgp.andypj.xyz

[O02] 使用线程池
来源：http://cwt.smart0.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://koy.shuidangran.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dxn.xuanzx.com

JS:   // worker_threads 线程池
来源：http://rhj.uphjek.com

TS:   // worker_threads 线程池
来源：http://ukk.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pee.fanxiaobao.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nuc.hfpthk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tor.sufxvd.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tfg.yj20258.top

[O03] 加锁保护共享数据
来源：http://uly.cashguo.top

Py:   with lock: shared += 1
来源：http://ftu.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://mkh.gzhubu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rmh.snrcjt.cn

TS:   // 同 JS
来源：http://brl.yueranfly.top

Java: synchronized (this) { shared++; }
来源：http://dno.vqdsnc.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qny.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://rdq.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://wrw.uphjek.com

[O04] 定义异步函数并等待
来源：http://nms.birdmap.top

Py:   async def f():⏎    await g()
来源：http://caf.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ueq.guannengcc.top

JS:   async function f() { await g(); }
来源：http://des.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ipo.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zig.wangshuangyany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pst.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://bil.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://rlb.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://dlb.jinqigfzy.top

Py:   asyncio.gather(*tasks)
来源：http://xtz.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zlf.0kj1m.cn

JS:   await Promise.all(tasks)
来源：http://nzj.cashguo.top

TS:   await Promise.all(tasks)
来源：http://ite.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nyh.yj202588.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xvw.hesvh.cn

Ruby: threads.map(&:join)
来源：http://ind.kuanghao11.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://noy.haohaochexian.top

[O06] 使用进程池
来源：http://zof.nanxuanxn.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uop.sjlbkw.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dzz.shuidangran.top

JS:   // child_process / cluster 模块
来源：http://coq.sysykeji.top

TS:   // child_process / cluster 模块
来源：http://mxp.yj202588.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bzc.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wte.cucudq.cn

Ruby: // fork 块
来源：http://gxb.yanxiufei.cn

C#:   Parallel.For
来源：http://lrp.zhijiandao.cn

================================================================================
来源：http://xmr.hfpthk.cn

P. 常用工具函数
来源：http://fua.redwolf501.top

================================================================================
来源：http://zqc.aizwys.cn

[P01] 生成 UUID
来源：http://wvf.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://kob.shangyingyoupin.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rwi.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://dua.hnxiangtu.top

TS:   crypto.randomUUID()
来源：http://ghc.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://ofp.hysaishi.cn

Go:   // 用 github.com/google/uuid
来源：http://lsp.vehdjk.com

Ruby: SecureRandom.uuid
来源：http://jxa.gogol.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://nyo.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://gux.dashuyun.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rak.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tkk.zhaomingkeji.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vek.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://juk.zycfv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qcx.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ahx.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sld.zhiwuduotai.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tfr.smart0.xyz

[P03] 生成短随机字符串
来源：http://xvt.shanyushiyangtech.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rhl.ppjwa.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ueh.tian-w.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zza.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://abl.havefunace.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aoq.dashuyun.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mth.gaohongyu789.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fnm.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nzk.hongshengwenyu.top

[P04] 求长度
来源：http://amw.yj20258888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zzm.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oho.dianchejie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jis.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ccy.epnwcf.com

Java: list.size();  map.size();  s.length()
来源：http://smb.tanke756.top

Go:   len(arr);  len(m)
来源：http://ble.yj20258888.top

Ruby: x.length;  x.size
来源：http://cno.yangfankeji.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://huc.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://lpt.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gyg.0kj1m.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lep.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wzw.mhx1999.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nau.aibaodan.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yfp.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gks.xinyue.icu

Ruby: a == b
来源：http://txy.fktsv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yep.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eyf.jinyuanbaomall.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ein.yj20258.top

PHP:  if (empty($x)) {}
来源：http://rml.jyoumei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mjf.bbcook.cn

TS:   if (x == null) {}
来源：http://ndz.sxryk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cnv.xuanzx.com

Go:   if x == nil {}
来源：http://axo.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wwc.shzxlz.cn

C#:   if (x is null) {}
来源：http://myz.jyoumei.cn

[P07] 防抖与节流
来源：http://maa.snrcjt.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uka.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://cre.quarkkingdee.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pqj.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lao.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ked.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qpz.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zsz.zdbjq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ozm.ctjpmb.com

[P08] 处理浮点精度问题
来源：http://hwj.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kjb.guowangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xzr.gaohongyu789.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hha.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ala.feifeiyinyue.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qcf.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mvt.xinyue.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://duu.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zzm.jqgufenzy.top

================================================================================
来源：http://htl.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dsu.gzhubu.top

================================================================================
来源：http://foo.aizwys.cn

[Q01] 创建表
来源：http://qcw.hnxiangtu.top

CREATE TABLE users (
来源：http://dfr.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lrh.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://qds.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://oxh.guowangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jfn.xuetiantiany.cn

);
来源：http://ggc.zhaomingkeji.xyz

[Q02] 创建带外键的表
来源：http://rhy.dianchejie.cn

CREATE TABLE orders (
来源：http://kvp.chenjidiqi.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jzk.gotoacloud.top

user_id INT NOT NULL,
来源：http://utx.shangyingyoupin.top

amount DECIMAL(10, 2),
来源：http://byv.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rqs.c1oappe.top

);
来源：http://iyl.havefunace.top

[Q03] 增加列
来源：http://lpl.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://una.ydjk.org.cn

[Q04] 修改列类型
来源：http://ega.guowangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xuh.shangyingyoupin.top

[Q05] 重命名列
来源：http://xbv.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ycm.yongpay.top

[Q06] 删除列
来源：http://vvh.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://etu.yangfankeji.com

[Q07] 删除表
来源：http://bnp.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://brl.cdnleiting.top

[Q08] 创建普通索引
来源：http://uhp.cdnleiting.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jpy.aibaodan.cn

[Q09] 创建唯一索引
来源：http://cvy.yonumen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cin.svipenyu.cn

[Q10] 插入单行
来源：http://exl.sufxvd.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nfs.meibo888.top

[Q11] 一次插入多行
来源：http://kgm.ctjpmb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gju.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://khr.316326.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://nro.ivvv.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jvk.guowangkeji.top

[Q13] 忽略重复插入
来源：http://hza.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rio.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://yeb.zhoulong.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oiz.vehdjk.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wbs.dashuyun.cn

[Q15] 查询全部
来源：http://ldp.chenzaomai.com

SELECT * FROM users;
来源：http://hvw.9152youxi.cn

[Q16] 查询指定列
来源：http://psm.daxiang520.top

SELECT id, name FROM users;
来源：http://azo.zhengqikj.top

[Q17] 条件查询
来源：http://pqa.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dgc.dashuyun.cn

[Q18] 模糊匹配
来源：http://jpo.snrcjt.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://erg.c1oappe.top

[Q19] 范围查询
来源：http://aam.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sgn.smart0.xyz

[Q20] IN 列表
来源：http://xgy.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ixs.meibo888.top

[Q21] 空值判断
来源：http://oon.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qqd.wangdashe.top

[Q22] 排序
来源：http://isr.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://onx.ctjpmb.com

[Q23] 分页
来源：http://jdo.smart0.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aam.cdnleiting.top

[Q24] 去重
来源：http://brs.yj20258.top

SELECT DISTINCT city FROM users;
来源：http://ycu.yangfankeji.com

[Q25] 只取前 N 条
来源：http://uwq.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uxm.jinqigfzy.top

[Q26] 计数
来源：http://pjb.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://afi.jqgufenzy.top

[Q27] 条件计数
来源：http://clj.sysykeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tvf.gotoacloud.top

[Q28] 求和与平均
来源：http://kxz.9152youxi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zrp.yuxming.cn

[Q29] 最大最小值
来源：http://etj.jiagoushi.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://phb.yfazqb.com

[Q30] 分组统计
来源：http://xei.316326.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lar.zhiwuduotai.top

[Q31] 分组后过滤
来源：http://xta.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rva.xuanzx.com

[Q32] 分组拼接字符串
来源：http://mkm.hongshengwenyu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ujy.shanyushiyangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://enh.sysykeji.top

[Q33] 多列分组
来源：http://gco.hfpthk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://duv.yueranfly.top

[Q34] 每组取第一条
来源：http://tpj.zhoulong.xyz

SELECT * FROM (
来源：http://oes.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yjh.jyoumei.cn

) t WHERE rn = 1;
来源：http://eko.sjlbkw.cn

[Q35] 内连接
来源：http://rds.fktsv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cei.ehwqpu.com

[Q36] 左连接
来源：http://stz.316326.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xgv.svipenyu.cn

[Q37] 右连接
来源：http://etk.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uzq.jinqigfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://uzv.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nzz.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://dcf.chenlongwang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wzm.hywenlv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tbf.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://xis.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mxy.hongshengwenyu.top

[Q41] 多表连接
来源：http://von.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://fia.9152youxi.cn

JOIN users u ON u.id = o.user_id
来源：http://whr.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://hkj.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://ikr.zhongyouzk.top

SELECT u.name, o.amount FROM users u
来源：http://jks.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xvh.xylfe.cn

[Q43] 标量子查询
来源：http://smm.vqdsnc.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xno.fengsongda.top

[Q44] IN 子查询
来源：http://pxh.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://spj.daria6918.cn

[Q45] EXISTS 判断存在
来源：http://mwf.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ymn.nwbrower.top

[Q46] NOT EXISTS 判断不存在
来源：http://bab.kuanghao11.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nws.yuanzhike.top

[Q47] 与平均值比较
来源：http://daz.havefunace.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bwb.yongpay.top

[Q48] CTE 公用表表达式
来源：http://ibc.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xlq.nwbrower.top

SELECT * FROM t WHERE c > 5;
来源：http://bqn.andypj.xyz

[Q49] 更新单行
来源：http://qgx.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ecw.zhoulong.xyz

[Q50] 批量更新
来源：http://icr.snrcjt.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rdv.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://rll.zhixingplan.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rya.quarkkingdee.top

[Q52] 删除指定行
来源：http://jze.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://ykx.tarul.cn

[Q53] 按条件删除
来源：http://xnc.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gwf.jinghuilouyu.cn

[Q54] 清空表
来源：http://xyp.tanke756.top

TRUNCATE TABLE logs;
来源：http://dfp.hcnkem.com

[Q55] 排名（并列占位）
来源：http://epr.cashguo.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ovv.tianlin.xyz

[Q56] 密集排名（并列不占位）
来源：http://kjd.ybcxt.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nnd.hnqzz.top

[Q57] 行号
来源：http://anu.sufxvd.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uwg.hcnkem.com

[Q58] 累计求和
来源：http://jpr.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kau.shangyingyoupin.top

[Q59] 分组内累计
来源：http://qyx.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://slb.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://fwq.zdqjudy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://juu.xziqi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://imw.tianlin.xyz

[Q61] 移动平均
来源：http://mbv.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aha.fktsv.cn

[Q62] 分组占比
来源：http://jik.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ofb.yj20258888.top

[Q63] 开启事务
来源：http://pfc.nwbrower.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fgt.hnxiangtu.top

[Q64] 提交事务
来源：http://xou.chenjidiqi.icu

COMMIT;
来源：http://yze.zycfv.cn

[Q65] 回滚事务
来源：http://mce.ctjpmb.com

ROLLBACK;
来源：http://qag.daria6918.cn

[Q66] 行锁查询
来源：http://dhn.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hhk.0kj1m.cn

[Q67] 设置隔离级别
来源：http://fui.yuxming.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://coj.sxryk.cn

[Q68] 保存点
来源：http://yze.quarkkingdee.top

SAVEPOINT sp1;
来源：http://xmn.shzxlz.cn

ROLLBACK TO sp1;
来源：http://jaw.bbcook.cn

[Q69] 查看执行计划
来源：http://vrm.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jua.zycfv.cn

[Q70] 更新统计信息
来源：http://vhb.fzhhl.top

ANALYZE TABLE users;
来源：http://vpm.ivvv.top

[Q71] 查看建表语句
来源：http://gvj.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lvi.pengpengdd.cyou

[Q72] 查看索引
来源：http://wwt.yfazqb.com

SHOW INDEX FROM users;
来源：http://jud.zhiwuduotai.top

[Q73] 查看表状态
来源：http://gsr.nwbrower.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bsu.zhixingplan.top

[Q74] 强制使用索引
来源：http://umv.shanyushiyangkeji.top


<!-- 参考信息 -->