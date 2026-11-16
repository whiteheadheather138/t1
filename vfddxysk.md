代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://imp.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yin.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mve.daria6918.cn

TS:   // 同 JS
来源：http://whp.vqdsnc.cn

Java: new Thread(() -> f()).start()
来源：http://vph.smart0.xyz

Go:   go f()
来源：http://gge.jinqigufen.top

Ruby: Thread.new { f }
来源：http://zbs.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://ejb.yj202588.top

[O02] 使用线程池
来源：http://vqw.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uqc.zdbjq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rke.fehbvm.com

JS:   // worker_threads 线程池
来源：http://ilp.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://cbd.svipenyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zqm.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vzh.ivvv.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pio.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wgy.shanyushiyangtech.top

[O03] 加锁保护共享数据
来源：http://sha.gotoacloud.top

Py:   with lock: shared += 1
来源：http://skv.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://rpz.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kiv.nanxinkj.top

TS:   // 同 JS
来源：http://hvv.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://jwu.fzhhl.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yuc.uphjek.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://bwa.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://pyw.hesvh.cn

[O04] 定义异步函数并等待
来源：http://tlr.meibo888.top

Py:   async def f():⏎    await g()
来源：http://shj.cdnleiting.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yzg.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://ksm.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://itc.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nqa.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eni.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wld.shanyushiyangkeji.top

C#:   async Task F() { await G(); }
来源：http://hoo.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://bwy.hfpthk.cn

Py:   asyncio.gather(*tasks)
来源：http://tpn.feifeiyinyue.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fiz.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://yas.yuanzhike.top

TS:   await Promise.all(tasks)
来源：http://wcy.zdqjudy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://izi.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wdc.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://ayb.mhx1999.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pkr.jinqigufen.top

[O06] 使用进程池
来源：http://qlj.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://myi.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jra.gaohongyu789.top

JS:   // child_process / cluster 模块
来源：http://cwq.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://wqw.sufxvd.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yuq.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gbw.sjlbkw.cn

Ruby: // fork 块
来源：http://hby.daxiang520.top

C#:   Parallel.For
来源：http://xtr.shanyushiyangtech.top

================================================================================
来源：http://ohh.gzhubu.top

P. 常用工具函数
来源：http://hhs.sjlbkw.cn

================================================================================
来源：http://dxp.tianlin.xyz

[P01] 生成 UUID
来源：http://rcu.kuanghao11.cn

Py:   str(uuid.uuid4())
来源：http://yqo.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lxg.wangdashe.top

JS:   crypto.randomUUID()
来源：http://uxb.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://htp.jyoumei.cn

Java: UUID.randomUUID().toString()
来源：http://ucr.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://src.cqqwz.cn

Ruby: SecureRandom.uuid
来源：http://gkq.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://vdb.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://qca.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oqy.hesvh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bnq.0kj1m.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sms.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oak.cqqwz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dti.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://feq.pycfn.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tep.daria6918.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://izg.gotoacloud.top

[P03] 生成短随机字符串
来源：http://ipe.jinqigfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pyu.hnxiangtu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tjj.snrcjt.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://veq.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dhm.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dkj.ivvv.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bsl.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://oem.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oqq.hnqzz.top

[P04] 求长度
来源：http://nfc.nwbrower.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zkt.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bmh.hnqzz.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cft.tanke756.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iux.yuanzhike.top

Java: list.size();  map.size();  s.length()
来源：http://jvh.316326.xyz

Go:   len(arr);  len(m)
来源：http://tsw.hammf.cn

Ruby: x.length;  x.size
来源：http://grj.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://skm.ppjwa.cn

[P05] 判断两个对象内容是否相等
来源：http://kaa.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oqh.quarkkingdee.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://msc.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wkt.yj20258888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wgx.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nyq.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://prg.sufxvd.cn

Ruby: a == b
来源：http://zst.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://msp.yongpay.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ira.guannengcc.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fqq.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://sam.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zkb.aibaodan.cn

TS:   if (x == null) {}
来源：http://ogb.zycfv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uli.fengsongda.top

Go:   if x == nil {}
来源：http://qsd.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qkt.jianghu66.top

C#:   if (x is null) {}
来源：http://hza.yvedp.cn

[P07] 防抖与节流
来源：http://odc.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rjp.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://ynq.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hpc.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eaa.ivvv.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://era.aibaodan.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hpp.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://liz.zhengqikj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ufv.ydzc1.top

[P08] 处理浮点精度问题
来源：http://oxp.0kj1m.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hzd.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tth.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wab.shanyushiyangtech.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yhv.zhijiandao.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qab.zhongyouzk.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://img.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://alu.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iql.cashguo.top

================================================================================
来源：http://ayw.chenlongwang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://woo.jinghuilouyu.cn

================================================================================
来源：http://hlg.sufxvd.cn

[Q01] 创建表
来源：http://uon.yj202588.top

CREATE TABLE users (
来源：http://qee.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ogv.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://fwv.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://siq.xingfuxueyuan.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://czn.havefunace.top

);
来源：http://wom.hcnkem.com

[Q02] 创建带外键的表
来源：http://ppi.quarkkingdee.top

CREATE TABLE orders (
来源：http://ezx.0kj1m.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bkh.uphjek.com

user_id INT NOT NULL,
来源：http://pyl.fengsongda.top

amount DECIMAL(10, 2),
来源：http://rbp.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mcx.vehdjk.com

);
来源：http://tqs.yfazqb.com

[Q03] 增加列
来源：http://jdm.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lvt.xziqi.cn

[Q04] 修改列类型
来源：http://agt.cqqwz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xmy.fehbvm.com

[Q05] 重命名列
来源：http://pxk.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pvv.hongshengwenyu.top

[Q06] 删除列
来源：http://ejg.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xoc.sysykeji.top

[Q07] 删除表
来源：http://zrk.uphjek.com

DROP TABLE IF EXISTS orders;
来源：http://eme.nanxinkj.top

[Q08] 创建普通索引
来源：http://sat.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hcw.ivvv.top

[Q09] 创建唯一索引
来源：http://ogb.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ciz.yuxming.cn

[Q10] 插入单行
来源：http://mho.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gyf.hnqzz.top

[Q11] 一次插入多行
来源：http://mwb.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rrd.ivvv.top

[Q12] 插入后取自增 ID
来源：http://ase.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://nkx.dashuyun.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uzj.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://fmq.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kih.jianghu66.top

[Q14] 存在则更新（upsert）
来源：http://raj.yonumen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ejh.sufxvd.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hfr.gzhubu.top

[Q15] 查询全部
来源：http://rkf.ybcxt.top

SELECT * FROM users;
来源：http://tjp.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://yud.cucudq.cn

SELECT id, name FROM users;
来源：http://ekm.uphjek.com

[Q17] 条件查询
来源：http://tex.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://stw.hcnkem.com

[Q18] 模糊匹配
来源：http://fse.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ugs.sjlbkw.cn

[Q19] 范围查询
来源：http://okn.shanyushiyangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zdd.yonumen.top

[Q20] IN 列表
来源：http://ami.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cjz.tian-w.cn

[Q21] 空值判断
来源：http://zyi.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://box.sufxvd.cn

[Q22] 排序
来源：http://tic.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wdi.zhiwuduotai.top

[Q23] 分页
来源：http://mav.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jbc.fktsv.cn

[Q24] 去重
来源：http://pfr.yuxming.cn

SELECT DISTINCT city FROM users;
来源：http://vir.hywenlv.cn

[Q25] 只取前 N 条
来源：http://yhm.hnqzz.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://voc.birdmap.top

[Q26] 计数
来源：http://rxx.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://lhh.vqdsnc.cn

[Q27] 条件计数
来源：http://owt.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cut.hammf.cn

[Q28] 求和与平均
来源：http://tql.hnqzz.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://flm.hnqzz.top

[Q29] 最大最小值
来源：http://mfp.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vfj.svipenyu.cn

[Q30] 分组统计
来源：http://hbu.yfazqb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lgp.hnqzz.top

[Q31] 分组后过滤
来源：http://aou.uphjek.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ilx.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://zxa.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vah.mhx1999.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aeg.dashuyun.cn

[Q33] 多列分组
来源：http://qlt.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qyh.birdmap.top

[Q34] 每组取第一条
来源：http://tpo.jqgfzy.top

SELECT * FROM (
来源：http://vpg.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lfe.dianchejie.cn

) t WHERE rn = 1;
来源：http://enr.zhixingplan.top

[Q35] 内连接
来源：http://wvs.yongpay.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yhc.cqqwz.cn

[Q36] 左连接
来源：http://hpl.cdnleiting.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ifn.zhongyouzk.top

[Q37] 右连接
来源：http://pay.pycfn.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lxv.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pdi.fzhhl.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sjy.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://pgj.fehbvm.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://rst.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://obg.snrcjt.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dre.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hev.chenjidiqi.icu

[Q41] 多表连接
来源：http://lcz.zhixingplan.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nzs.sweek.top

JOIN users u ON u.id = o.user_id
来源：http://jfk.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://vvu.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://yjk.gotoacloud.top

SELECT u.name, o.amount FROM users u
来源：http://stt.ydzc1.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yrd.hysaishi.cn

[Q43] 标量子查询
来源：http://ibs.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gdi.zycfv.cn

[Q44] IN 子查询
来源：http://aat.yuxming.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xek.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://rvm.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bvb.gogol.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ilb.ydjk.org.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jbs.jinyuanbaomall.cn

[Q47] 与平均值比较
来源：http://eru.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nbf.zycfv.cn

[Q48] CTE 公用表表达式
来源：http://ajc.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fqk.xylfe.cn

SELECT * FROM t WHERE c > 5;
来源：http://qdj.jlsjyb.cn

[Q49] 更新单行
来源：http://ojh.havefunace.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eeu.jyoumei.cn

[Q50] 批量更新
来源：http://hwv.chenjidiqi.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bon.gaohongyu789.top

[Q51] 用子查询更新
来源：http://cmz.jinqigfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ukc.wangdashe.top

[Q52] 删除指定行
来源：http://ohm.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://wvf.cheryme.top

[Q53] 按条件删除
来源：http://zbq.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lam.jqgufenzy.top

[Q54] 清空表
来源：http://xhk.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://vug.c1oappe.top

[Q55] 排名（并列占位）
来源：http://cph.gotoacloud.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zkr.zhixingplan.top

[Q56] 密集排名（并列不占位）
来源：http://euh.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hhx.wangshuangyany.cn

[Q57] 行号
来源：http://iuk.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qkd.quarkkingdee.top

[Q58] 累计求和
来源：http://mvx.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jek.snrcjt.cn

[Q59] 分组内累计
来源：http://qzj.hesvh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hdd.xuanzx.com

[Q60] 取上一行 / 下一行
来源：http://ith.uphjek.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xww.wangshuangyany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vke.haohaochexian.top

[Q61] 移动平均
来源：http://rnc.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ndi.shanyushiyangtech.top

[Q62] 分组占比
来源：http://zap.shanyushiyangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bdj.jiagoushi.top

[Q63] 开启事务
来源：http://mbc.cqqwz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://csz.uphjek.com

[Q64] 提交事务
来源：http://uvz.epnwcf.com

COMMIT;
来源：http://pou.c1oappe.top

[Q65] 回滚事务
来源：http://vlc.shuidangran.top

ROLLBACK;
来源：http://frg.nanxuanxn.top

[Q66] 行锁查询
来源：http://jhz.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yku.hywenlv.cn

[Q67] 设置隔离级别
来源：http://ekl.dashuyun.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nwc.316326.xyz

[Q68] 保存点
来源：http://vwa.jinqigfzy.top

SAVEPOINT sp1;
来源：http://kgo.cqqwz.cn

ROLLBACK TO sp1;
来源：http://pzf.hnqzz.top

[Q69] 查看执行计划
来源：http://xsn.guowangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hxa.vqdsnc.cn

[Q70] 更新统计信息
来源：http://yuo.guannengcc.top

ANALYZE TABLE users;
来源：http://xev.yueranfly.top

[Q71] 查看建表语句
来源：http://pzm.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vyn.52xcode.cn

[Q72] 查看索引
来源：http://wrk.xziqi.cn

SHOW INDEX FROM users;
来源：http://dki.zhiwuduotai.top

[Q73] 查看表状态
来源：http://bgj.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ebv.0kj1m.cn

[Q74] 强制使用索引
来源：http://zco.sweek.top


<!-- 参考信息 -->