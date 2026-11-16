代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://whb.cashguo.top

Go:   go f()
来源：http://lug.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://lbr.shzxlz.cn

C#:   Task.Run(() => F());
来源：http://fba.aizwys.cn

[O02] 使用线程池
来源：http://eob.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zzy.zhaomingkeji.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aya.zdqjudy.top

JS:   // worker_threads 线程池
来源：http://uyx.jqgufenzy.top

TS:   // worker_threads 线程池
来源：http://ocn.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://tic.nwbrower.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kwk.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wlw.sjlbkw.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gey.gzhubu.top

[O03] 加锁保护共享数据
来源：http://rvv.epnwcf.com

Py:   with lock: shared += 1
来源：http://fwy.daria6918.cn

PHP:  // 用 flock() 做文件锁
来源：http://gbh.ywan-chungtsiang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tvy.jinqigufen.top

TS:   // 同 JS
来源：http://hnc.ydjk.org.cn

Java: synchronized (this) { shared++; }
来源：http://mpd.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://art.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://mpg.shuidangran.top

C#:   lock (gate) { shared++; }
来源：http://xay.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://sgs.316326.xyz

Py:   async def f():⏎    await g()
来源：http://clb.jqgufenzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zyg.sysykeji.top

JS:   async function f() { await g(); }
来源：http://oqj.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mdm.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rjs.andypj.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yex.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://vzd.fanxiaobao.xyz

C#:   async Task F() { await G(); }
来源：http://ucr.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://usp.9152youxi.cn

Py:   asyncio.gather(*tasks)
来源：http://mfh.zhaomingkeji.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dhl.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://rxq.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://qhg.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mmu.zycfv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://has.cashguo.top

Ruby: threads.map(&:join)
来源：http://amw.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://shk.yangfankeji.com

[O06] 使用进程池
来源：http://asf.fehbvm.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://osu.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gxp.jinyuanbaomall.cn

JS:   // child_process / cluster 模块
来源：http://wve.quarkkingdee.top

TS:   // child_process / cluster 模块
来源：http://hlp.fehbvm.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://niq.316326.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://shv.hcnkem.com

Ruby: // fork 块
来源：http://yvz.yuxming.cn

C#:   Parallel.For
来源：http://azr.cdnleiting.top

================================================================================
来源：http://ozk.pycfn.com

P. 常用工具函数
来源：http://kts.yj20258.top

================================================================================
来源：http://oth.jinqigfzy.top

[P01] 生成 UUID
来源：http://plt.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://gpx.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mtf.bbcook.cn

JS:   crypto.randomUUID()
来源：http://mxu.yongpay.top

TS:   crypto.randomUUID()
来源：http://wsa.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://vqp.jqgufenzy.top

Go:   // 用 github.com/google/uuid
来源：http://ori.jlsjyb.cn

Ruby: SecureRandom.uuid
来源：http://vvn.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://hki.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://fxs.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://igl.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://etv.chenjidiqi.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kyc.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rrv.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jic.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ams.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hhx.shanyushiyangkeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ils.cdnleiting.top

[P03] 生成短随机字符串
来源：http://ccp.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vrm.yfazqb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uzg.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mya.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://frp.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qir.xinyue.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jth.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://avg.yj20258888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lkb.fehbvm.com

[P04] 求长度
来源：http://fag.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://owr.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blh.9152youxi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fxq.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pml.zhengqikj.top

Java: list.size();  map.size();  s.length()
来源：http://bzk.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://mdm.316326.xyz

Ruby: x.length;  x.size
来源：http://svp.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fvw.snrcjt.cn

[P05] 判断两个对象内容是否相等
来源：http://xbu.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zhs.sysykeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rtb.snrcjt.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jmm.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nad.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://waf.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://xdk.zhiwuduotai.top

Ruby: a == b
来源：http://vqt.tian-w.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jam.chenlongwang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jfj.fzhhl.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rba.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://ewm.pycfn.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mss.daxiang520.top

TS:   if (x == null) {}
来源：http://kyi.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zof.hnxiangtu.top

Go:   if x == nil {}
来源：http://eip.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mzf.cucudq.cn

C#:   if (x is null) {}
来源：http://gas.gotoacloud.top

[P07] 防抖与节流
来源：http://qfx.cheryme.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jei.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://yri.ydzc1.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hrn.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jtg.chenzaomai.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jef.dashuyun.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fqs.xuetiantiany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lts.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sej.sufxvd.cn

[P08] 处理浮点精度问题
来源：http://ukw.c1oappe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://myj.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lhy.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hnz.tian-w.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jbk.daxiang520.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pjk.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gux.52xcode.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://buk.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lut.sxryk.cn

================================================================================
来源：http://ujw.xziqi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tie.sjlbkw.cn

================================================================================
来源：http://gdd.yuanzhike.top

[Q01] 创建表
来源：http://sak.yfazqb.com

CREATE TABLE users (
来源：http://alf.jqgufenzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qpl.zhijiandao.cn

name VARCHAR(50) NOT NULL,
来源：http://rmh.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://gyr.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bvd.hysaishi.cn

);
来源：http://tzs.shzxlz.cn

[Q02] 创建带外键的表
来源：http://kkz.yj20258.top

CREATE TABLE orders (
来源：http://ecp.hcnkem.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bee.sweek.top

user_id INT NOT NULL,
来源：http://jas.jqgfzy.top

amount DECIMAL(10, 2),
来源：http://ryk.fengsongda.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jpu.jqgufenzy.top

);
来源：http://zlq.zhaomingkeji.xyz

[Q03] 增加列
来源：http://ijc.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gde.haohaochexian.top

[Q04] 修改列类型
来源：http://xcn.jyoumei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://amt.tarul.cn

[Q05] 重命名列
来源：http://ncm.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oeb.fzhhl.top

[Q06] 删除列
来源：http://wup.birdmap.top

ALTER TABLE users DROP COLUMN age;
来源：http://vhy.fehbvm.com

[Q07] 删除表
来源：http://bio.kuanghao11.cn

DROP TABLE IF EXISTS orders;
来源：http://iwo.shzxlz.cn

[Q08] 创建普通索引
来源：http://vzm.hongshengwenyu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jvh.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://lpa.epnwcf.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rmd.chenzaomai.com

[Q10] 插入单行
来源：http://yij.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tiw.yfazqb.com

[Q11] 一次插入多行
来源：http://xsx.chenlongwang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lvu.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://iqz.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://thd.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fkd.shuidangran.top

[Q13] 忽略重复插入
来源：http://cxv.shzxlz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://och.jyoumei.cn

[Q14] 存在则更新（upsert）
来源：http://xvb.tarul.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rkg.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ybc.wangshuangyany.cn

[Q15] 查询全部
来源：http://quw.ppjwa.cn

SELECT * FROM users;
来源：http://jyx.yangfankeji.com

[Q16] 查询指定列
来源：http://ywa.ivvv.top

SELECT id, name FROM users;
来源：http://lrn.c1oappe.top

[Q17] 条件查询
来源：http://ncr.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wpg.svipenyu.cn

[Q18] 模糊匹配
来源：http://rdx.ivvv.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://azq.yueranfly.top

[Q19] 范围查询
来源：http://pvp.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mam.zhiwuduotai.top

[Q20] IN 列表
来源：http://eug.iojbl.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://glv.gaohongyu789.top

[Q21] 空值判断
来源：http://umm.hnqzz.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lpj.0kj1m.cn

[Q22] 排序
来源：http://xoj.hesvh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lmw.xuetiantiany.cn

[Q23] 分页
来源：http://akj.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zfo.quarkkingdee.top

[Q24] 去重
来源：http://cgb.chenzaomai.com

SELECT DISTINCT city FROM users;
来源：http://aqy.jyoumei.cn

[Q25] 只取前 N 条
来源：http://opl.yuanzhike.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rzi.316326.xyz

[Q26] 计数
来源：http://wsp.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://lfh.svipenyu.cn

[Q27] 条件计数
来源：http://rom.yueranfly.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vrc.tanke756.top

[Q28] 求和与平均
来源：http://uet.jinyuanbaomall.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://txu.fanxiaobao.xyz

[Q29] 最大最小值
来源：http://gku.gzhubu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xoa.chenlongwang.top

[Q30] 分组统计
来源：http://drg.c1oappe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cwe.zhengqikj.top

[Q31] 分组后过滤
来源：http://uke.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://woc.yonumen.top

[Q32] 分组拼接字符串
来源：http://ptf.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aan.iojbl.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nqj.jinqigufen.top

[Q33] 多列分组
来源：http://kwz.redwolf501.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://spw.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://aeh.sweek.top

SELECT * FROM (
来源：http://ejy.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hfc.cashguo.top

) t WHERE rn = 1;
来源：http://jmt.feifeiyinyue.top

[Q35] 内连接
来源：http://dsg.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zti.nwbrower.top

[Q36] 左连接
来源：http://pyt.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ala.chenjidiqi.icu

[Q37] 右连接
来源：http://vku.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ihs.meibo888.top

[Q38] 全外连接（PostgreSQL）
来源：http://tpu.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vaw.pengpengdd.cyou

[Q39] 自连接（查上下级）
来源：http://qgh.guannengcc.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zvi.chenjidiqi.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jaj.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://gen.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bbz.gogol.net.cn

[Q41] 多表连接
来源：http://bdg.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://hiz.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://ywg.zhengqikj.top

JOIN products p ON p.id = o.product_id;
来源：http://csf.yongpay.top

[Q42] 连接条件附加过滤
来源：http://kaw.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://nic.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zim.yanxiufei.cn

[Q43] 标量子查询
来源：http://cqa.bjfxy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pgv.cashguo.top

[Q44] IN 子查询
来源：http://kae.cdnleiting.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zqs.gotoacloud.top

[Q45] EXISTS 判断存在
来源：http://nfa.xingfuxueyuan.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sxj.sxryk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rch.jiagoushi.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fjo.jinqigufen.top

[Q47] 与平均值比较
来源：http://jjc.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://waf.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://lwu.pycfn.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vks.zhijiandao.cn

SELECT * FROM t WHERE c > 5;
来源：http://cfr.hywenlv.cn

[Q49] 更新单行
来源：http://usp.daxiang520.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pbi.epnwcf.com

[Q50] 批量更新
来源：http://tzc.hnxiangtu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://shn.xingfuxueyuan.xyz

[Q51] 用子查询更新
来源：http://eau.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ams.yueranfly.top

[Q52] 删除指定行
来源：http://dib.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://ngg.jlsjyb.cn

[Q53] 按条件删除
来源：http://zuq.smart0.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://opp.daria6918.cn

[Q54] 清空表
来源：http://tof.birdmap.top

TRUNCATE TABLE logs;
来源：http://mjx.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://sqn.xylfe.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lkq.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://apf.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cfg.yuanzhike.top

[Q57] 行号
来源：http://rau.jqgfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mvw.yongpay.top

[Q58] 累计求和
来源：http://mwd.jinyuanbaomall.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://odf.cqqwz.cn

[Q59] 分组内累计
来源：http://nrf.shangyingyoupin.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://szx.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://tfe.yangfankeji.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kib.xingfuxueyuan.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gkp.fengsongda.top

[Q61] 移动平均
来源：http://lnm.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lac.kuanghao11.cn

[Q62] 分组占比
来源：http://liz.zhijiandao.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://teq.yj20258888.top

[Q63] 开启事务
来源：http://ykt.yueranfly.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mnl.yj202588.top

[Q64] 提交事务
来源：http://xpn.ppjwa.cn

COMMIT;
来源：http://mcs.uphjek.com

[Q65] 回滚事务
来源：http://nma.wangdashe.top

ROLLBACK;
来源：http://nlv.feifeiyinyue.top

[Q66] 行锁查询
来源：http://abp.yvedp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jot.yuanzhike.top

[Q67] 设置隔离级别
来源：http://uyt.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ezw.vqdsnc.cn

[Q68] 保存点
来源：http://jog.daria6918.cn

SAVEPOINT sp1;
来源：http://lcz.fengsongda.top

ROLLBACK TO sp1;
来源：http://bpy.hongshengwenyu.top

[Q69] 查看执行计划
来源：http://xfp.shanyushiyangtech.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://szr.vehdjk.com

[Q70] 更新统计信息
来源：http://qsc.pycfn.com

ANALYZE TABLE users;
来源：http://plz.zhoulong.xyz

[Q71] 查看建表语句
来源：http://jlw.jinqigfzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ncg.redwolf501.top

[Q72] 查看索引
来源：http://xuo.hnqzz.top

SHOW INDEX FROM users;
来源：http://die.hongshengwenyu.top

[Q73] 查看表状态
来源：http://sif.zhiwuduotai.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kai.svipenyu.cn

[Q74] 强制使用索引
来源：http://qfk.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yyq.iojbl.cn

[Q75] 日期格式化
来源：http://mpx.iojbl.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vse.kuanghao11.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cju.aibaodan.cn


<!-- 参考信息 -->