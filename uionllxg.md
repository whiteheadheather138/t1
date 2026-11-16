代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xxw.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mve.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ppj.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yse.andypj.xyz

================================================================================
来源：http://odp.tarul.cn

O. 并发与异步
来源：http://wbz.ydjk.org.cn

================================================================================
来源：http://dgh.zhongyouzk.top

[O01] 启动一个线程
来源：http://uik.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lrz.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mjv.guannengcc.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ujs.nanxinkj.top

TS:   // 同 JS
来源：http://ppv.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://bnd.fktsv.cn

Go:   go f()
来源：http://jfn.xziqi.cn

Ruby: Thread.new { f }
来源：http://azd.tianlin.xyz

C#:   Task.Run(() => F());
来源：http://nqv.hywenlv.cn

[O02] 使用线程池
来源：http://rzg.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vkg.yfazqb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xib.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://xan.iojbl.cn

TS:   // worker_threads 线程池
来源：http://wob.nanxinkj.top

Java: Executors.newFixedThreadPool(4)
来源：http://qqw.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jxz.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rwm.ppjwa.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kjx.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://utg.aizwys.cn

Py:   with lock: shared += 1
来源：http://icm.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://pqw.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bul.jinghuilouyu.cn

TS:   // 同 JS
来源：http://uph.cucudq.cn

Java: synchronized (this) { shared++; }
来源：http://pnj.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://moz.aibaodan.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xte.sysykeji.top

C#:   lock (gate) { shared++; }
来源：http://ksh.hnxiangtu.top

[O04] 定义异步函数并等待
来源：http://bsy.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://hac.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jln.smart0.xyz

JS:   async function f() { await g(); }
来源：http://hvs.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://bdr.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qgi.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ikg.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://mvy.guowangkeji.top

C#:   async Task F() { await G(); }
来源：http://wcb.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://dcg.xuetiantiany.cn

Py:   asyncio.gather(*tasks)
来源：http://mzk.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ski.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://beu.fzhhl.top

TS:   await Promise.all(tasks)
来源：http://buu.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fuc.jinyuanbaomall.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nkp.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://erf.xingfuxueyuan.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://qwa.havefunace.top

[O06] 使用进程池
来源：http://ybs.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://huu.jinqigufen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xug.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://kgb.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://tfw.daria6918.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zjz.cashguo.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sly.fzhhl.top

Ruby: // fork 块
来源：http://mzi.sxryk.cn

C#:   Parallel.For
来源：http://how.sxryk.cn

================================================================================
来源：http://pub.cheryme.top

P. 常用工具函数
来源：http://tsl.xziqi.cn

================================================================================
来源：http://sff.xuanzx.com

[P01] 生成 UUID
来源：http://pkn.nwbrower.top

Py:   str(uuid.uuid4())
来源：http://lij.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mby.fzhhl.top

JS:   crypto.randomUUID()
来源：http://xjo.fehbvm.com

TS:   crypto.randomUUID()
来源：http://mzj.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://vhc.sufxvd.cn

Go:   // 用 github.com/google/uuid
来源：http://idh.hongshengwenyu.top

Ruby: SecureRandom.uuid
来源：http://yai.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://wsr.vehdjk.com

[P02] MD5 / SHA256 摘要
来源：http://ack.shanyushiyangtech.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lke.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hvp.mhx1999.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fdn.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://joh.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ilt.snrcjt.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://thc.tarul.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iwk.svipenyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qgw.xziqi.cn

[P03] 生成短随机字符串
来源：http://iqk.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://srs.nwbrower.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://afu.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rxh.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hzd.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fkz.hywenlv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cgs.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xxv.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ynh.jyoumei.cn

[P04] 求长度
来源：http://lvg.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ngc.fehbvm.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dya.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://teo.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blx.yfazqb.com

Java: list.size();  map.size();  s.length()
来源：http://pkk.mhx1999.top

Go:   len(arr);  len(m)
来源：http://uec.jinyuanbaomall.cn

Ruby: x.length;  x.size
来源：http://qlp.hywenlv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bmz.shanyushiyangtech.top

[P05] 判断两个对象内容是否相等
来源：http://znl.zhiwuduotai.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://err.hysaishi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tlp.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sdp.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hox.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wwx.gotoacloud.top

Go:   reflect.DeepEqual(a, b)
来源：http://wca.ppjwa.cn

Ruby: a == b
来源：http://exy.xinyue.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yjp.fktsv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ndx.316326.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://khb.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://xlf.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nxm.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://feu.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hgl.hongshengwenyu.top

Go:   if x == nil {}
来源：http://jtr.yonumen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uis.ppjwa.cn

C#:   if (x is null) {}
来源：http://dpq.pengpengdd.cyou

[P07] 防抖与节流
来源：http://ath.bbcook.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ars.xylfe.cn

PHP:  // 手写时间戳比较
来源：http://dbx.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cxn.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://amm.yanxiufei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qdf.sufxvd.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://djh.zhoulong.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://gmf.epnwcf.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xeo.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://sxx.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jnq.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jvn.nanxuanxn.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ecg.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xmv.jqgfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bko.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://our.xuetiantiany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fmt.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qcs.vehdjk.com

================================================================================
来源：http://uuc.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uht.svipenyu.cn

================================================================================
来源：http://hiy.ydzc1.top

[Q01] 创建表
来源：http://fmx.bbcook.cn

CREATE TABLE users (
来源：http://jyk.gzhubu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hyx.yj20258888.top

name VARCHAR(50) NOT NULL,
来源：http://aoj.gotoacloud.top

email VARCHAR(100) UNIQUE,
来源：http://sfd.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hvm.daria6918.cn

);
来源：http://ihn.gzhubu.top

[Q02] 创建带外键的表
来源：http://qyb.hfpthk.cn

CREATE TABLE orders (
来源：http://dmf.hcnkem.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kbz.cheryme.top

user_id INT NOT NULL,
来源：http://ajd.zycfv.cn

amount DECIMAL(10, 2),
来源：http://isk.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lpc.jinqigfzy.top

);
来源：http://nuq.iojbl.cn

[Q03] 增加列
来源：http://oav.hcnkem.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://obt.yueranfly.top

[Q04] 修改列类型
来源：http://kfu.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cqq.cheryme.top

[Q05] 重命名列
来源：http://szr.gzhubu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://spx.zhiwuduotai.top

[Q06] 删除列
来源：http://zkq.gaohongyu789.top

ALTER TABLE users DROP COLUMN age;
来源：http://wel.jqgfzy.top

[Q07] 删除表
来源：http://ahe.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://ync.gaohongyu789.top

[Q08] 创建普通索引
来源：http://enz.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://uiy.yangfankeji.com

[Q09] 创建唯一索引
来源：http://hbt.haohaochexian.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dls.chenjidiqi.icu

[Q10] 插入单行
来源：http://xvd.cheryme.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oqw.nanxinkj.top

[Q11] 一次插入多行
来源：http://avq.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://myl.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://yhe.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://bub.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://txl.tian-w.cn

[Q13] 忽略重复插入
来源：http://hnl.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://omg.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://ixj.ctjpmb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://aai.pycfn.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://frf.jqgfzy.top

[Q15] 查询全部
来源：http://kpe.havefunace.top

SELECT * FROM users;
来源：http://zzt.gotoacloud.top

[Q16] 查询指定列
来源：http://out.kuanghao11.cn

SELECT id, name FROM users;
来源：http://nqh.sxryk.cn

[Q17] 条件查询
来源：http://cbw.sufxvd.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jva.sxryk.cn

[Q18] 模糊匹配
来源：http://ivo.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wfb.jiagoushi.top

[Q19] 范围查询
来源：http://nyf.gzhubu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zcs.jinyuanbaomall.cn

[Q20] IN 列表
来源：http://yjg.zdqjudy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bkr.316326.xyz

[Q21] 空值判断
来源：http://hrq.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eku.shangyingyoupin.top

[Q22] 排序
来源：http://lcf.dianchejie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://luf.yj20258888.top

[Q23] 分页
来源：http://omc.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ajn.zhixingplan.top

[Q24] 去重
来源：http://zhn.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://jpa.hcnkem.com

[Q25] 只取前 N 条
来源：http://loe.redwolf501.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dbv.zhaomingkeji.xyz

[Q26] 计数
来源：http://nhw.cheryme.top

SELECT COUNT(*) FROM users;
来源：http://yqo.ctjpmb.com

[Q27] 条件计数
来源：http://hat.jqgufenzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://msc.jqgufenzy.top

[Q28] 求和与平均
来源：http://eei.yvedp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sgd.yvedp.cn

[Q29] 最大最小值
来源：http://ocu.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ccs.0kj1m.cn

[Q30] 分组统计
来源：http://pyc.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ubl.316326.xyz

[Q31] 分组后过滤
来源：http://yed.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fyq.ydzc1.top

[Q32] 分组拼接字符串
来源：http://kpx.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gqe.sjlbkw.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qvz.uphjek.com

[Q33] 多列分组
来源：http://fie.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ire.xingfuxueyuan.xyz

[Q34] 每组取第一条
来源：http://dxg.ivvv.top

SELECT * FROM (
来源：http://xhf.yongpay.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iyx.0kj1m.cn

) t WHERE rn = 1;
来源：http://tat.snrcjt.cn

[Q35] 内连接
来源：http://nnw.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sjk.aibaodan.cn

[Q36] 左连接
来源：http://gsw.pengpengdd.cyou

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eno.nanxuanxn.top

[Q37] 右连接
来源：http://dwk.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qww.sweek.top

[Q38] 全外连接（PostgreSQL）
来源：http://kcu.jiagoushi.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vpc.hcnkem.com

[Q39] 自连接（查上下级）
来源：http://wiq.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rix.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zdw.sjlbkw.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mwi.zdbjq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lxp.sxryk.cn

[Q41] 多表连接
来源：http://hhh.jyoumei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wwq.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://jtf.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://wwr.chenzaomai.com

[Q42] 连接条件附加过滤
来源：http://dzf.xuanzx.com

SELECT u.name, o.amount FROM users u
来源：http://jrv.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rho.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://sei.ctjpmb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ufh.vehdjk.com

[Q44] IN 子查询
来源：http://wbn.jlsjyb.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dek.yanxiufei.cn

[Q45] EXISTS 判断存在
来源：http://aig.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hjr.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://aky.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://diw.vqdsnc.cn

[Q47] 与平均值比较
来源：http://uvo.zhongyouzk.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wlj.kuanghao11.cn

[Q48] CTE 公用表表达式
来源：http://bcv.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fay.nwbrower.top

SELECT * FROM t WHERE c > 5;
来源：http://dee.bbcook.cn

[Q49] 更新单行
来源：http://iwj.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qba.zhiwuduotai.top

[Q50] 批量更新
来源：http://fhs.sweek.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uqi.cucudq.cn

[Q51] 用子查询更新
来源：http://dhq.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qhe.haohaochexian.top

[Q52] 删除指定行
来源：http://ykq.zhixingplan.top

DELETE FROM users WHERE id = 10;
来源：http://idy.kuanghao11.cn

[Q53] 按条件删除
来源：http://sym.chenjidiqi.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eom.jyoumei.cn

[Q54] 清空表
来源：http://eoj.zhijiandao.cn

TRUNCATE TABLE logs;
来源：http://jmd.shanyushiyangkeji.top

[Q55] 排名（并列占位）
来源：http://ykz.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://okz.cdnleiting.top

[Q56] 密集排名（并列不占位）
来源：http://tgq.316326.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xrj.ctjpmb.com

[Q57] 行号
来源：http://vix.fehbvm.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dom.yueranfly.top

[Q58] 累计求和
来源：http://syv.shangyingyoupin.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://any.daria6918.cn

[Q59] 分组内累计
来源：http://hmo.zhengqikj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://obc.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://lxq.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ujt.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ims.ctjpmb.com

[Q61] 移动平均
来源：http://rkg.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lkn.yfazqb.com

[Q62] 分组占比
来源：http://cji.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ted.zhongyouzk.top

[Q63] 开启事务
来源：http://vlg.hysaishi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kyf.smart0.xyz

[Q64] 提交事务
来源：http://sew.meibo888.top

COMMIT;
来源：http://jej.0kj1m.cn

[Q65] 回滚事务
来源：http://apx.zhoulong.xyz

ROLLBACK;
来源：http://gqj.cdnleiting.top

[Q66] 行锁查询
来源：http://aua.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yfs.9152youxi.cn

[Q67] 设置隔离级别
来源：http://vgj.jinqigfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vqt.ctjpmb.com

[Q68] 保存点
来源：http://oxn.chenjidiqi.icu

SAVEPOINT sp1;
来源：http://dyh.yj20258.top

ROLLBACK TO sp1;
来源：http://lce.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://kqd.shuidangran.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vxe.52xcode.cn

[Q70] 更新统计信息
来源：http://fsa.yj202588.top


<!-- 参考信息 -->