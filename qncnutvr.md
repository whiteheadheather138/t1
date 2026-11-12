代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://whe.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lbw.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mre.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wmg.feifeiyinyue.top

================================================================================
来源：http://cxy.ydzc1.top

O. 并发与异步
来源：http://wlh.fehbvm.com

================================================================================
来源：http://lum.ybcxt.top

[O01] 启动一个线程
来源：http://sga.daria6918.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tgf.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xwf.zhaomingkeji.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://elj.cdnleiting.top

TS:   // 同 JS
来源：http://gvh.gotoacloud.top

Java: new Thread(() -> f()).start()
来源：http://elr.tian-w.cn

Go:   go f()
来源：http://wdf.haohaochexian.top

Ruby: Thread.new { f }
来源：http://gjy.shangyingyoupin.top

C#:   Task.Run(() => F());
来源：http://fap.jqgufenzy.top

[O02] 使用线程池
来源：http://ngc.zhixingplan.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fhs.cashguo.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gzd.ydzc1.top

JS:   // worker_threads 线程池
来源：http://qal.sxryk.cn

TS:   // worker_threads 线程池
来源：http://jqz.iojbl.cn

Java: Executors.newFixedThreadPool(4)
来源：http://afs.aibaodan.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rwr.chenzaomai.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://elb.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qpu.jinyuanbaomall.cn

[O03] 加锁保护共享数据
来源：http://osa.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://skp.xuanzx.com

PHP:  // 用 flock() 做文件锁
来源：http://gve.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ern.jqgufenzy.top

TS:   // 同 JS
来源：http://yhr.vqdsnc.cn

Java: synchronized (this) { shared++; }
来源：http://uwo.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cwe.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://owf.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://doq.zhijiandao.cn

[O04] 定义异步函数并等待
来源：http://rdz.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://inc.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tau.jqgfzy.top

JS:   async function f() { await g(); }
来源：http://awn.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mbo.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gpm.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bdr.zdqjudy.top

Ruby: # 用 Fiber 或 async gem
来源：http://hdt.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://gbj.9152youxi.cn

[O05] 并发执行并等待全部完成
来源：http://dsq.zycfv.cn

Py:   asyncio.gather(*tasks)
来源：http://pmg.smart0.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yua.fanxiaobao.xyz

JS:   await Promise.all(tasks)
来源：http://bbr.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://ouy.pycfn.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://its.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://epg.sxryk.cn

Ruby: threads.map(&:join)
来源：http://kyi.ywan-chungtsiang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://oxe.hywenlv.cn

[O06] 使用进程池
来源：http://lml.cqqwz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bpq.hysaishi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vcx.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://lsd.shanyushiyangtech.top

TS:   // child_process / cluster 模块
来源：http://hnw.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ccd.nwbrower.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fid.hnxiangtu.top

Ruby: // fork 块
来源：http://pev.quarkkingdee.top

C#:   Parallel.For
来源：http://aaf.chenlongwang.top

================================================================================
来源：http://qkz.hcnkem.com

P. 常用工具函数
来源：http://ywn.pycfn.com

================================================================================
来源：http://hgj.shzxlz.cn

[P01] 生成 UUID
来源：http://vdm.xuetiantiany.cn

Py:   str(uuid.uuid4())
来源：http://unc.nwbrower.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://idd.havefunace.top

JS:   crypto.randomUUID()
来源：http://ahy.zycfv.cn

TS:   crypto.randomUUID()
来源：http://ogv.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://gnn.haohaochexian.top

Go:   // 用 github.com/google/uuid
来源：http://ner.tanke756.top

Ruby: SecureRandom.uuid
来源：http://mqa.dianchejie.cn

C#:   Guid.NewGuid().ToString()
来源：http://zib.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://khn.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ckn.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jpw.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jts.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gfs.zdbjq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zld.yfazqb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://foj.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://arr.jianghu66.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pdf.hesvh.cn

[P03] 生成短随机字符串
来源：http://eca.svipenyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wvk.c1oappe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hac.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bve.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vjo.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fiv.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ats.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sry.ehwqpu.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vrp.yj202588.top

[P04] 求长度
来源：http://env.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dci.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hki.yangfankeji.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vav.jinghuilouyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://odr.ydzc1.top

Java: list.size();  map.size();  s.length()
来源：http://pgl.aizwys.cn

Go:   len(arr);  len(m)
来源：http://zag.ywan-chungtsiang.top

Ruby: x.length;  x.size
来源：http://nqk.jyoumei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yuc.hnqzz.top

[P05] 判断两个对象内容是否相等
来源：http://xng.hongshengwenyu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hqc.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ima.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mif.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cpf.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jcb.yvedp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bvw.shanyushiyangtech.top

Ruby: a == b
来源：http://bxf.tian-w.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://idn.wangshuangyany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zow.shangyingyoupin.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://khn.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://rjo.pycfn.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aqn.xylfe.cn

TS:   if (x == null) {}
来源：http://bbl.zhixingplan.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ial.jinghuilouyu.cn

Go:   if x == nil {}
来源：http://xwl.hesvh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mcc.pengpengdd.cyou

C#:   if (x is null) {}
来源：http://kfw.hysaishi.cn

[P07] 防抖与节流
来源：http://vsb.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qzr.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://kyo.jyoumei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gmx.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://niy.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aed.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qor.smart0.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://jeu.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mpf.jinghuilouyu.cn

[P08] 处理浮点精度问题
来源：http://xdf.yanxiufei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jbq.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://abg.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vxx.hysaishi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uap.feifeiyinyue.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jjx.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xst.cucudq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fsv.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pxh.nanxinkj.top

================================================================================
来源：http://dvn.ehwqpu.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sya.jinqigfzy.top

================================================================================
来源：http://mnb.jqgfzy.top

[Q01] 创建表
来源：http://nwi.nanxuanxn.top

CREATE TABLE users (
来源：http://jjn.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qov.wangshuangyany.cn

name VARCHAR(50) NOT NULL,
来源：http://azt.sxryk.cn

email VARCHAR(100) UNIQUE,
来源：http://otw.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zdr.c1oappe.top

);
来源：http://qjh.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://oii.ybcxt.top

CREATE TABLE orders (
来源：http://plx.pycfn.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://goe.uphjek.com

user_id INT NOT NULL,
来源：http://osg.gzhubu.top

amount DECIMAL(10, 2),
来源：http://hqp.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://njx.vqdsnc.cn

);
来源：http://jtv.cheryme.top

[Q03] 增加列
来源：http://qap.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bfr.gotoacloud.top

[Q04] 修改列类型
来源：http://iwa.cucudq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://myg.hysaishi.cn

[Q05] 重命名列
来源：http://duw.zhiwuduotai.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rhn.jqgfzy.top

[Q06] 删除列
来源：http://zro.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ben.chenlongwang.top

[Q07] 删除表
来源：http://fdc.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://cyp.hnxiangtu.top

[Q08] 创建普通索引
来源：http://nxf.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vbd.jqgfzy.top

[Q09] 创建唯一索引
来源：http://nxv.andypj.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tkd.xuanzx.com

[Q10] 插入单行
来源：http://emo.ydzc1.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zau.haohaochexian.top

[Q11] 一次插入多行
来源：http://ton.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lbj.gogol.net.cn

[Q12] 插入后取自增 ID
来源：http://vtb.aibaodan.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cst.wangdashe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zvz.sxryk.cn

[Q13] 忽略重复插入
来源：http://ggo.52xcode.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ael.mhx1999.top

[Q14] 存在则更新（upsert）
来源：http://mbn.pengpengdd.cyou

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ecg.xziqi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ygu.hesvh.cn

[Q15] 查询全部
来源：http://xjb.fktsv.cn

SELECT * FROM users;
来源：http://uvk.pengpengdd.cyou

[Q16] 查询指定列
来源：http://cig.andypj.xyz

SELECT id, name FROM users;
来源：http://ofx.snrcjt.cn

[Q17] 条件查询
来源：http://mfr.daxiang520.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vma.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://ofe.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cgj.tarul.cn

[Q19] 范围查询
来源：http://bzq.kuanghao11.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ejs.aibaodan.cn

[Q20] IN 列表
来源：http://rzu.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yoa.yueranfly.top

[Q21] 空值判断
来源：http://iqy.redwolf501.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cwq.jianghu66.top

[Q22] 排序
来源：http://emf.chenjidiqi.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://amb.yuxming.cn

[Q23] 分页
来源：http://jxb.ehwqpu.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zrl.pengpengdd.cyou

[Q24] 去重
来源：http://blr.cheryme.top

SELECT DISTINCT city FROM users;
来源：http://vzu.yj20258.top

[Q25] 只取前 N 条
来源：http://zcn.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ahm.wangshuangyany.cn

[Q26] 计数
来源：http://jzp.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://zmm.tianlin.xyz

[Q27] 条件计数
来源：http://vqy.yj20258888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rdt.0kj1m.cn

[Q28] 求和与平均
来源：http://pfj.xuetiantiany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oid.hysaishi.cn

[Q29] 最大最小值
来源：http://idp.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://dow.yangfankeji.com

[Q30] 分组统计
来源：http://mrg.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hob.smart0.xyz

[Q31] 分组后过滤
来源：http://efk.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pno.52xcode.cn

[Q32] 分组拼接字符串
来源：http://kzg.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gei.uphjek.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fsw.tian-w.cn

[Q33] 多列分组
来源：http://nan.aizwys.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://odr.xinyue.icu

[Q34] 每组取第一条
来源：http://xjx.gogol.net.cn

SELECT * FROM (
来源：http://rmr.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rfz.yanxiufei.cn

) t WHERE rn = 1;
来源：http://gul.bjfxy.top

[Q35] 内连接
来源：http://zrl.zhengqikj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tzx.sxryk.cn

[Q36] 左连接
来源：http://elw.aibaodan.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mst.hywenlv.cn

[Q37] 右连接
来源：http://joz.fzhhl.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://izr.pengpengdd.cyou

[Q38] 全外连接（PostgreSQL）
来源：http://dxt.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://keb.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://ggs.kuanghao11.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jqi.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tar.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://phx.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vno.hnxiangtu.top

[Q41] 多表连接
来源：http://hfg.cashguo.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://axu.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://kba.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://tyc.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://iuf.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://isa.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sor.xuetiantiany.cn

[Q43] 标量子查询
来源：http://ojf.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ncy.ydjk.org.cn

[Q44] IN 子查询
来源：http://wfj.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://slp.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://mqo.gogol.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qtn.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://htv.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kpl.zdqjudy.top

[Q47] 与平均值比较
来源：http://vyy.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xkj.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://npu.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tva.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://aur.tian-w.cn

[Q49] 更新单行
来源：http://syq.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bpj.snrcjt.cn

[Q50] 批量更新
来源：http://rno.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ptb.ehwqpu.com

[Q51] 用子查询更新
来源：http://mxo.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://afv.guannengcc.top

[Q52] 删除指定行
来源：http://soo.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://nod.mhx1999.top

[Q53] 按条件删除
来源：http://jib.jinqigufen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qmt.vqdsnc.cn

[Q54] 清空表
来源：http://wmi.guannengcc.top

TRUNCATE TABLE logs;
来源：http://hek.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://wkt.tianlin.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tvg.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://ngf.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://amm.hongshengwenyu.top

[Q57] 行号
来源：http://rxv.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qrz.sxryk.cn

[Q58] 累计求和
来源：http://gbt.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iwl.hammf.cn

[Q59] 分组内累计
来源：http://hcb.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fjg.daxiang520.top

[Q60] 取上一行 / 下一行
来源：http://dbk.aibaodan.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ahe.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yod.haohaochexian.top

[Q61] 移动平均
来源：http://ktt.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lrp.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://iom.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yuk.yonumen.top

[Q63] 开启事务
来源：http://kzx.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jba.dashuyun.cn

[Q64] 提交事务
来源：http://ned.yonumen.top

COMMIT;
来源：http://cqw.quarkkingdee.top

[Q65] 回滚事务
来源：http://xys.hywenlv.cn

ROLLBACK;
来源：http://tqz.xuanzx.com

[Q66] 行锁查询
来源：http://kei.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wza.pycfn.com

[Q67] 设置隔离级别
来源：http://yty.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://izm.sweek.top

[Q68] 保存点
来源：http://jyp.kuanghao11.cn

SAVEPOINT sp1;
来源：http://uhc.yj20258.top

ROLLBACK TO sp1;
来源：http://taz.quarkkingdee.top

[Q69] 查看执行计划
来源：http://hnn.hywenlv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lrv.zdbjq.cn

[Q70] 更新统计信息
来源：http://ene.daxiang520.top


<!-- 参考信息 -->