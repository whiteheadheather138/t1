代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pav.jyoumei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://frj.meibo888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wkv.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ctf.aibaodan.cn

================================================================================
来源：http://bsz.feifeiyinyue.top

O. 并发与异步
来源：http://hka.yanxiufei.cn

================================================================================
来源：http://rjb.yanxiufei.cn

[O01] 启动一个线程
来源：http://ipp.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://glh.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ire.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://smx.sweek.top

TS:   // 同 JS
来源：http://lwr.dianchejie.cn

Java: new Thread(() -> f()).start()
来源：http://xtx.dashuyun.cn

Go:   go f()
来源：http://hdf.jqgfzy.top

Ruby: Thread.new { f }
来源：http://lhh.nanxinkj.top

C#:   Task.Run(() => F());
来源：http://rma.haohaochexian.top

[O02] 使用线程池
来源：http://pfw.sweek.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gzp.mhx1999.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://owx.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://uxw.gaohongyu789.top

TS:   // worker_threads 线程池
来源：http://mjg.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bpo.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hyf.hesvh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ldd.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vtn.yueranfly.top

[O03] 加锁保护共享数据
来源：http://kgk.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://vvx.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://jzs.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wmt.fktsv.cn

TS:   // 同 JS
来源：http://kfm.zhijiandao.cn

Java: synchronized (this) { shared++; }
来源：http://grc.shanyushiyangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mjn.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zhz.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://kmg.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://zzy.fktsv.cn

Py:   async def f():⏎    await g()
来源：http://bkv.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zkm.hywenlv.cn

JS:   async function f() { await g(); }
来源：http://waz.nanxinkj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vpb.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uhu.shuidangran.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://itk.gogol.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://osf.yongpay.top

C#:   async Task F() { await G(); }
来源：http://glu.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://pig.sxryk.cn

Py:   asyncio.gather(*tasks)
来源：http://oxg.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uid.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://jce.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://dxm.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gcw.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://abj.birdmap.top

Ruby: threads.map(&:join)
来源：http://lyb.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://umr.tianlin.xyz

[O06] 使用进程池
来源：http://hsf.sweek.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yik.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hox.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://bxi.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://bfx.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wbz.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wmt.birdmap.top

Ruby: // fork 块
来源：http://kgk.xinyue.icu

C#:   Parallel.For
来源：http://wig.bjfxy.top

================================================================================
来源：http://sbp.hnxiangtu.top

P. 常用工具函数
来源：http://fci.meibo888.top

================================================================================
来源：http://wmz.c1oappe.top

[P01] 生成 UUID
来源：http://dho.yongpay.top

Py:   str(uuid.uuid4())
来源：http://bzf.sxryk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://off.dashuyun.cn

JS:   crypto.randomUUID()
来源：http://vre.hnqzz.top

TS:   crypto.randomUUID()
来源：http://rar.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://vjc.xziqi.cn

Go:   // 用 github.com/google/uuid
来源：http://oge.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://doh.hnqzz.top

C#:   Guid.NewGuid().ToString()
来源：http://uju.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://cpw.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mlf.zhiwuduotai.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://msl.0kj1m.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dkw.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bhe.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rdv.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rjk.daxiang520.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bij.xuetiantiany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tfy.smart0.xyz

[P03] 生成短随机字符串
来源：http://myc.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hxm.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hsy.ehwqpu.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gcn.ydzc1.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dah.xuanzx.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qqw.xuetiantiany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jeq.birdmap.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://upr.zhengqikj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dsh.sxryk.cn

[P04] 求长度
来源：http://nma.shzxlz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://avk.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://okc.52xcode.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mbr.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nxd.meibo888.top

Java: list.size();  map.size();  s.length()
来源：http://szc.nanxuanxn.top

Go:   len(arr);  len(m)
来源：http://fqb.jlsjyb.cn

Ruby: x.length;  x.size
来源：http://tuo.yueranfly.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://aac.snrcjt.cn

[P05] 判断两个对象内容是否相等
来源：http://she.ydzc1.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sll.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cwr.andypj.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fum.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ffi.fktsv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://goi.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://eby.yanxiufei.cn

Ruby: a == b
来源：http://yap.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gcl.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gqm.ehwqpu.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zep.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://xnn.shanyushiyangtech.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eyw.yongpay.top

TS:   if (x == null) {}
来源：http://lwe.ywan-chungtsiang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wsc.yanxiufei.cn

Go:   if x == nil {}
来源：http://hpr.9152youxi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nop.hnxiangtu.top

C#:   if (x is null) {}
来源：http://tlz.xuanzx.com

[P07] 防抖与节流
来源：http://bwm.zhongyouzk.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wrz.gaohongyu789.top

PHP:  // 手写时间戳比较
来源：http://wbn.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ift.tanke756.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tiu.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ubd.yj20258.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xoi.nanxinkj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://anw.dianchejie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://law.ydjk.org.cn

[P08] 处理浮点精度问题
来源：http://xgd.ivvv.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jsf.c1oappe.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tis.ppjwa.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lsw.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fkn.zhaomingkeji.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sfv.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oyt.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gjd.zhongyouzk.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bky.zdbjq.cn

================================================================================
来源：http://wqi.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tga.52xcode.cn

================================================================================
来源：http://qac.wangdashe.top

[Q01] 创建表
来源：http://cos.tian-w.cn

CREATE TABLE users (
来源：http://dnh.52xcode.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ywn.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://ieo.vqdsnc.cn

email VARCHAR(100) UNIQUE,
来源：http://nuz.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vcq.hfpthk.cn

);
来源：http://hrn.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://syz.chenjidiqi.icu

CREATE TABLE orders (
来源：http://gzr.tarul.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sdi.jqgufenzy.top

user_id INT NOT NULL,
来源：http://abi.sjlbkw.cn

amount DECIMAL(10, 2),
来源：http://fne.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sox.fengsongda.top

);
来源：http://fcx.yueranfly.top

[Q03] 增加列
来源：http://dcq.hnqzz.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bhp.wangshuangyany.cn

[Q04] 修改列类型
来源：http://xfe.hammf.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://abe.sxryk.cn

[Q05] 重命名列
来源：http://kwr.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://omk.wangshuangyany.cn

[Q06] 删除列
来源：http://uti.hnxiangtu.top

ALTER TABLE users DROP COLUMN age;
来源：http://gmr.cucudq.cn

[Q07] 删除表
来源：http://con.fktsv.cn

DROP TABLE IF EXISTS orders;
来源：http://yrs.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://jzy.feifeiyinyue.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jdv.dashuyun.cn

[Q09] 创建唯一索引
来源：http://bca.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zuc.fanxiaobao.xyz

[Q10] 插入单行
来源：http://zha.andypj.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nzb.daria6918.cn

[Q11] 一次插入多行
来源：http://obk.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jqw.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://aht.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jku.birdmap.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kgv.tanke756.top

[Q13] 忽略重复插入
来源：http://jlo.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iop.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://sxy.gotoacloud.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cyu.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hoj.andypj.xyz

[Q15] 查询全部
来源：http://hrl.pengpengdd.cyou

SELECT * FROM users;
来源：http://hnn.cashguo.top

[Q16] 查询指定列
来源：http://lls.bbcook.cn

SELECT id, name FROM users;
来源：http://rsu.cdnleiting.top

[Q17] 条件查询
来源：http://xby.xinyue.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pkz.52xcode.cn

[Q18] 模糊匹配
来源：http://wpw.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nfl.jyoumei.cn

[Q19] 范围查询
来源：http://sgs.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pup.fzhhl.top

[Q20] IN 列表
来源：http://afu.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tmg.tian-w.cn

[Q21] 空值判断
来源：http://uia.0kj1m.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ogk.zhiwuduotai.top

[Q22] 排序
来源：http://txm.xuetiantiany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tli.guowangkeji.top

[Q23] 分页
来源：http://zwo.zhiwuduotai.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yrf.quarkkingdee.top

[Q24] 去重
来源：http://nyd.sweek.top

SELECT DISTINCT city FROM users;
来源：http://kbk.dianchejie.cn

[Q25] 只取前 N 条
来源：http://lio.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zhk.gotoacloud.top

[Q26] 计数
来源：http://yct.sufxvd.cn

SELECT COUNT(*) FROM users;
来源：http://zqs.cqqwz.cn

[Q27] 条件计数
来源：http://tek.nwbrower.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hqv.shuidangran.top

[Q28] 求和与平均
来源：http://zqo.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hpe.tian-w.cn

[Q29] 最大最小值
来源：http://tkd.yanxiufei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cui.fzhhl.top

[Q30] 分组统计
来源：http://etl.gogol.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gpz.haohaochexian.top

[Q31] 分组后过滤
来源：http://uxe.sxryk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hea.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://ssa.smart0.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dda.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lps.pycfn.com

[Q33] 多列分组
来源：http://sxt.feifeiyinyue.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xkf.hcnkem.com

[Q34] 每组取第一条
来源：http://lsw.bjfxy.top

SELECT * FROM (
来源：http://evp.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bwb.epnwcf.com

) t WHERE rn = 1;
来源：http://tzg.wangshuangyany.cn

[Q35] 内连接
来源：http://zup.pengpengdd.cyou

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hlg.hongshengwenyu.top

[Q36] 左连接
来源：http://jcl.yfazqb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oqf.ehwqpu.com

[Q37] 右连接
来源：http://jvo.zhiwuduotai.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sec.shanyushiyangtech.top

[Q38] 全外连接（PostgreSQL）
来源：http://jaz.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uvw.smart0.xyz

[Q39] 自连接（查上下级）
来源：http://xnu.hysaishi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yjy.jinghuilouyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vrc.hesvh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://akn.jyoumei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qma.hnxiangtu.top

[Q41] 多表连接
来源：http://rnv.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://igq.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://acy.haohaochexian.top

JOIN products p ON p.id = o.product_id;
来源：http://bdf.tianlin.xyz

[Q42] 连接条件附加过滤
来源：http://tjz.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://ema.zhongyouzk.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ezi.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://tvs.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kvt.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://oir.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rla.xingfuxueyuan.xyz

[Q45] EXISTS 判断存在
来源：http://tuc.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wtc.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oyc.aizwys.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mrf.havefunace.top

[Q47] 与平均值比较
来源：http://nla.gogol.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mht.fktsv.cn

[Q48] CTE 公用表表达式
来源：http://gns.daria6918.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cke.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://yrs.yj20258.top

[Q49] 更新单行
来源：http://jdd.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lwa.hywenlv.cn

[Q50] 批量更新
来源：http://clu.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kgs.daxiang520.top

[Q51] 用子查询更新
来源：http://meb.yuxming.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bwk.fktsv.cn

[Q52] 删除指定行
来源：http://pli.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://mpl.cheryme.top

[Q53] 按条件删除
来源：http://bhh.daxiang520.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qfv.chenzaomai.com

[Q54] 清空表
来源：http://afy.hesvh.cn

TRUNCATE TABLE logs;
来源：http://pyt.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://pwi.yanxiufei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xhx.redwolf501.top

[Q56] 密集排名（并列不占位）
来源：http://tkz.zhiwuduotai.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gsj.yj20258.top

[Q57] 行号
来源：http://ahg.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uoi.yuanzhike.top

[Q58] 累计求和
来源：http://njb.shuidangran.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zuj.yj20258.top

[Q59] 分组内累计
来源：http://zfj.gaohongyu789.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pii.fzhhl.top

[Q60] 取上一行 / 下一行
来源：http://rxc.havefunace.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xqo.ctjpmb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nuk.pycfn.com

[Q61] 移动平均
来源：http://eba.havefunace.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rez.ydjk.org.cn

[Q62] 分组占比
来源：http://mpa.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://djf.hysaishi.cn

[Q63] 开启事务
来源：http://wzq.chenjidiqi.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://qsu.guowangkeji.top

[Q64] 提交事务
来源：http://ngq.sxryk.cn

COMMIT;
来源：http://blj.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://ihs.tian-w.cn

ROLLBACK;
来源：http://tsw.0kj1m.cn

[Q66] 行锁查询
来源：http://pen.yuxming.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cuc.yanxiufei.cn

[Q67] 设置隔离级别
来源：http://eha.shanyushiyangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zku.jiagoushi.top

[Q68] 保存点
来源：http://mhx.c1oappe.top

SAVEPOINT sp1;
来源：http://ovd.hysaishi.cn

ROLLBACK TO sp1;
来源：http://jos.zhengqikj.top

[Q69] 查看执行计划
来源：http://llr.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zwa.redwolf501.top

[Q70] 更新统计信息
来源：http://hbb.nanxuanxn.top


<!-- 参考信息 -->