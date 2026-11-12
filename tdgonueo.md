代发 wailian999

[O02] 使用线程池
来源：http://sdr.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gua.ppjwa.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lny.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://oqj.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://jms.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cjo.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wiz.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hrr.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wak.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://oja.316326.xyz

Py:   with lock: shared += 1
来源：http://noh.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://hls.zhijiandao.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eaa.cdnleiting.top

TS:   // 同 JS
来源：http://njh.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://twm.yangfankeji.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://txq.vqdsnc.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tvw.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://tyb.daria6918.cn

[O04] 定义异步函数并等待
来源：http://hmm.jqgufenzy.top

Py:   async def f():⏎    await g()
来源：http://qqp.sufxvd.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gnc.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://xqz.sweek.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://skz.jlsjyb.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rnw.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://itn.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://urj.zdbjq.cn

C#:   async Task F() { await G(); }
来源：http://sqg.yj20258888.top

[O05] 并发执行并等待全部完成
来源：http://esd.tarul.cn

Py:   asyncio.gather(*tasks)
来源：http://zhg.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xrk.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://bko.shzxlz.cn

TS:   await Promise.all(tasks)
来源：http://sqf.yonumen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fpr.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ocq.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://juw.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tuu.yuxming.cn

[O06] 使用进程池
来源：http://csw.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lxf.shanyushiyangtech.top

PHP:  // pcntl_fork 或多进程队列
来源：http://utr.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://iea.jinyuanbaomall.cn

TS:   // child_process / cluster 模块
来源：http://krh.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qsr.cheryme.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rvg.chenlongwang.top

Ruby: // fork 块
来源：http://qpr.ppjwa.cn

C#:   Parallel.For
来源：http://zqw.dianchejie.cn

================================================================================
来源：http://fah.jinqigfzy.top

P. 常用工具函数
来源：http://zwq.yangfankeji.com

================================================================================
来源：http://xxy.jqgfzy.top

[P01] 生成 UUID
来源：http://jdy.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://wwn.tanke756.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ywk.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://qso.cucudq.cn

TS:   crypto.randomUUID()
来源：http://kxv.fengsongda.top

Java: UUID.randomUUID().toString()
来源：http://hif.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://yii.yongpay.top

Ruby: SecureRandom.uuid
来源：http://ejx.yfazqb.com

C#:   Guid.NewGuid().ToString()
来源：http://piw.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://szq.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uvm.jqgufenzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mnn.gzhubu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wsz.cashguo.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://teb.dashuyun.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wnz.cheryme.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vih.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lyl.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tcb.xuanzx.com

[P03] 生成短随机字符串
来源：http://jwp.iojbl.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jwf.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jmj.hfpthk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zsk.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://atk.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gep.shanyushiyangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pdb.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fjp.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vri.ppjwa.cn

[P04] 求长度
来源：http://bpf.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rja.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ual.zhixingplan.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ttl.cashguo.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ued.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://nxi.bjfxy.top

Go:   len(arr);  len(m)
来源：http://crb.shanyushiyangtech.top

Ruby: x.length;  x.size
来源：http://sxs.kuanghao11.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://umg.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://rus.sxryk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tme.chenlongwang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cyr.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qmk.yj20258888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://svg.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://miv.aibaodan.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ubp.fengsongda.top

Ruby: a == b
来源：http://nvt.havefunace.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ydv.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zlv.jqgufenzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xxg.cqqwz.cn

PHP:  if (empty($x)) {}
来源：http://quc.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bfx.yfazqb.com

TS:   if (x == null) {}
来源：http://bpd.xuanzx.com

Java: if (x == null || x.isEmpty()) {}
来源：http://kpc.xingfuxueyuan.xyz

Go:   if x == nil {}
来源：http://frf.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vfr.xuanzx.com

C#:   if (x is null) {}
来源：http://oxi.ctjpmb.com

[P07] 防抖与节流
来源：http://adv.tianlin.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ptz.yangfankeji.com

PHP:  // 手写时间戳比较
来源：http://bpc.zhoulong.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hir.hcnkem.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rjy.sjlbkw.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bbd.vqdsnc.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://isd.yj202588.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://usz.chenzaomai.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zfx.shanyushiyangkeji.top

[P08] 处理浮点精度问题
来源：http://yxj.yfazqb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ocd.smart0.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lih.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vzj.hysaishi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yfs.iojbl.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ctu.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gsd.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dtn.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cph.kuanghao11.cn

================================================================================
来源：http://iri.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ocm.aibaodan.cn

================================================================================
来源：http://muo.jinqigfzy.top

[Q01] 创建表
来源：http://pgn.nanxinkj.top

CREATE TABLE users (
来源：http://bcz.fengsongda.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rws.iojbl.cn

name VARCHAR(50) NOT NULL,
来源：http://vfe.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://rwf.havefunace.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tvs.yuanzhike.top

);
来源：http://qyh.hesvh.cn

[Q02] 创建带外键的表
来源：http://hne.cashguo.top

CREATE TABLE orders (
来源：http://uph.fzhhl.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://amw.gaohongyu789.top

user_id INT NOT NULL,
来源：http://dvx.chenlongwang.top

amount DECIMAL(10, 2),
来源：http://blr.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vau.jinqigufen.top

);
来源：http://umq.uphjek.com

[Q03] 增加列
来源：http://wif.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cjt.epnwcf.com

[Q04] 修改列类型
来源：http://jgk.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dev.ehwqpu.com

[Q05] 重命名列
来源：http://hyo.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sko.zdqjudy.top

[Q06] 删除列
来源：http://emj.jinyuanbaomall.cn

ALTER TABLE users DROP COLUMN age;
来源：http://suz.zhijiandao.cn

[Q07] 删除表
来源：http://fvj.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://zuq.ppjwa.cn

[Q08] 创建普通索引
来源：http://evl.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://oqv.zycfv.cn

[Q09] 创建唯一索引
来源：http://lze.meibo888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gvy.hysaishi.cn

[Q10] 插入单行
来源：http://xxf.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uxm.ehwqpu.com

[Q11] 一次插入多行
来源：http://cvj.hysaishi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gpc.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://ahg.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://phd.hywenlv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hpe.gogol.net.cn

[Q13] 忽略重复插入
来源：http://stb.tian-w.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qoi.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://gvx.epnwcf.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eol.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hmz.mhx1999.top

[Q15] 查询全部
来源：http://umb.andypj.xyz

SELECT * FROM users;
来源：http://fim.havefunace.top

[Q16] 查询指定列
来源：http://smi.0kj1m.cn

SELECT id, name FROM users;
来源：http://giy.xylfe.cn

[Q17] 条件查询
来源：http://cgz.sufxvd.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yrm.hysaishi.cn

[Q18] 模糊匹配
来源：http://qwi.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ssv.epnwcf.com

[Q19] 范围查询
来源：http://hkt.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zbl.hongshengwenyu.top

[Q20] IN 列表
来源：http://iwg.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lhw.guowangkeji.top

[Q21] 空值判断
来源：http://gyn.hfpthk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sdy.chenzaomai.com

[Q22] 排序
来源：http://clp.sjlbkw.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qfg.sjlbkw.cn

[Q23] 分页
来源：http://xez.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nmx.dashuyun.cn

[Q24] 去重
来源：http://dfm.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://kbf.uphjek.com

[Q25] 只取前 N 条
来源：http://wka.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jeb.fehbvm.com

[Q26] 计数
来源：http://quq.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://zrv.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://wes.ctjpmb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cav.gogol.net.cn

[Q28] 求和与平均
来源：http://xvc.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hvp.fzhhl.top

[Q29] 最大最小值
来源：http://itg.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vmn.gogol.net.cn

[Q30] 分组统计
来源：http://xdn.nanxinkj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bqc.yj202588.top

[Q31] 分组后过滤
来源：http://qkd.9152youxi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eun.iojbl.cn

[Q32] 分组拼接字符串
来源：http://cpb.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ukf.xuetiantiany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://krc.xylfe.cn

[Q33] 多列分组
来源：http://twe.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eta.xuanzx.com

[Q34] 每组取第一条
来源：http://rjd.shzxlz.cn

SELECT * FROM (
来源：http://ctz.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nzu.aibaodan.cn

) t WHERE rn = 1;
来源：http://whc.epnwcf.com

[Q35] 内连接
来源：http://gah.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ica.c1oappe.top

[Q36] 左连接
来源：http://tkl.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lgj.daxiang520.top

[Q37] 右连接
来源：http://mzo.yuanzhike.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zex.vqdsnc.cn

[Q38] 全外连接（PostgreSQL）
来源：http://oel.vehdjk.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bug.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://acw.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kfi.pycfn.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gzl.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cuk.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tjh.yanxiufei.cn

[Q41] 多表连接
来源：http://cbf.andypj.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://jtm.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://sms.aizwys.cn

JOIN products p ON p.id = o.product_id;
来源：http://fuj.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://lqz.jqgufenzy.top

SELECT u.name, o.amount FROM users u
来源：http://iij.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://swl.vqdsnc.cn

[Q43] 标量子查询
来源：http://leu.ybcxt.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oar.fehbvm.com

[Q44] IN 子查询
来源：http://pli.hysaishi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tmj.xziqi.cn

[Q45] EXISTS 判断存在
来源：http://njg.vqdsnc.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ovx.nwbrower.top

[Q46] NOT EXISTS 判断不存在
来源：http://oik.hammf.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ttm.fehbvm.com

[Q47] 与平均值比较
来源：http://auv.shanyushiyangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ukg.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://occ.0kj1m.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cck.bbcook.cn

SELECT * FROM t WHERE c > 5;
来源：http://flo.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://afk.aizwys.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wgs.jlsjyb.cn

[Q50] 批量更新
来源：http://egj.epnwcf.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sue.guannengcc.top

[Q51] 用子查询更新
来源：http://glg.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mpf.bbcook.cn

[Q52] 删除指定行
来源：http://snj.yongpay.top

DELETE FROM users WHERE id = 10;
来源：http://bsl.nwbrower.top

[Q53] 按条件删除
来源：http://hol.jinghuilouyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vms.nwbrower.top

[Q54] 清空表
来源：http://sbv.andypj.xyz

TRUNCATE TABLE logs;
来源：http://byh.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://une.hywenlv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jyx.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://gon.nwbrower.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xyo.daxiang520.top

[Q57] 行号
来源：http://jev.0kj1m.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qxl.ybcxt.top

[Q58] 累计求和
来源：http://czc.sxryk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xxe.sufxvd.cn

[Q59] 分组内累计
来源：http://jqb.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mxm.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://jdg.guowangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cfb.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kea.jlsjyb.cn

[Q61] 移动平均
来源：http://qzx.yuanzhike.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fpe.cdnleiting.top

[Q62] 分组占比
来源：http://iqq.daria6918.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yzc.uphjek.com

[Q63] 开启事务
来源：http://hmp.nanxuanxn.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ihx.yuanzhike.top

[Q64] 提交事务
来源：http://qgg.ydzc1.top

COMMIT;
来源：http://flz.dianchejie.cn

[Q65] 回滚事务
来源：http://pju.zhiwuduotai.top

ROLLBACK;
来源：http://oej.zhengqikj.top

[Q66] 行锁查询
来源：http://twk.cdnleiting.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lce.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://fgh.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hbd.feifeiyinyue.top

[Q68] 保存点
来源：http://hsl.feifeiyinyue.top

SAVEPOINT sp1;
来源：http://nde.jinqigufen.top

ROLLBACK TO sp1;
来源：http://bvc.zhiwuduotai.top

[Q69] 查看执行计划
来源：http://lbk.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cae.jiagoushi.top

[Q70] 更新统计信息
来源：http://tru.hnqzz.top

ANALYZE TABLE users;
来源：http://xvz.xingfuxueyuan.xyz

[Q71] 查看建表语句
来源：http://iuy.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cav.yangfankeji.com

[Q72] 查看索引
来源：http://ppz.xinyue.icu

SHOW INDEX FROM users;
来源：http://kxq.shanyushiyangkeji.top

[Q73] 查看表状态
来源：http://pyp.jqgfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://etw.9152youxi.cn

[Q74] 强制使用索引
来源：http://aii.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xkd.xinyue.icu

[Q75] 日期格式化
来源：http://nve.ybcxt.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bmf.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hls.yj202588.top

[Q76] 按天统计
来源：http://blh.sufxvd.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ecz.birdmap.top

[Q77] 时间加减
来源：http://ysw.ehwqpu.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pmh.ywan-chungtsiang.top


<!-- 参考信息 -->