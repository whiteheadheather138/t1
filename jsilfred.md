代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ynw.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hun.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cjw.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ctf.sufxvd.cn

================================================================================
来源：http://icb.fehbvm.com

O. 并发与异步
来源：http://djo.jqgfzy.top

================================================================================
来源：http://pts.sweek.top

[O01] 启动一个线程
来源：http://tjj.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lfk.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://too.wangshuangyany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kda.hammf.cn

TS:   // 同 JS
来源：http://kck.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://wta.jinyuanbaomall.cn

Go:   go f()
来源：http://wrt.bbcook.cn

Ruby: Thread.new { f }
来源：http://dxn.gogol.net.cn

C#:   Task.Run(() => F());
来源：http://xul.mhx1999.top

[O02] 使用线程池
来源：http://uvt.yongpay.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cfn.dashuyun.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rza.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://avu.ivvv.top

TS:   // worker_threads 线程池
来源：http://jjx.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fjf.zhoulong.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qbv.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rtm.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wrh.shangyingyoupin.top

[O03] 加锁保护共享数据
来源：http://lsq.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://nzs.vehdjk.com

PHP:  // 用 flock() 做文件锁
来源：http://ayf.zdqjudy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qht.yongpay.top

TS:   // 同 JS
来源：http://esf.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://bvg.fanxiaobao.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sfa.yj20258.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://koz.fanxiaobao.xyz

C#:   lock (gate) { shared++; }
来源：http://lns.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://tlh.zdqjudy.top

Py:   async def f():⏎    await g()
来源：http://jnm.hammf.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gtp.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://dsi.gzhubu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://juk.jiagoushi.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jcv.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iil.jinyuanbaomall.cn

Ruby: # 用 Fiber 或 async gem
来源：http://imx.jinqigfzy.top

C#:   async Task F() { await G(); }
来源：http://mhs.xingfuxueyuan.xyz

[O05] 并发执行并等待全部完成
来源：http://oyy.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://aht.havefunace.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cgy.9152youxi.cn

JS:   await Promise.all(tasks)
来源：http://tyu.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://vjf.c1oappe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ioi.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://joe.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://asf.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nhh.9152youxi.cn

[O06] 使用进程池
来源：http://sio.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xob.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pvh.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://qfg.shangyingyoupin.top

TS:   // child_process / cluster 模块
来源：http://ndj.xuetiantiany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cxj.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aiq.yvedp.cn

Ruby: // fork 块
来源：http://wci.guowangkeji.top

C#:   Parallel.For
来源：http://fcs.fengsongda.top

================================================================================
来源：http://gtv.zdbjq.cn

P. 常用工具函数
来源：http://pgi.ctjpmb.com

================================================================================
来源：http://vdb.ydjk.org.cn

[P01] 生成 UUID
来源：http://kal.shanyushiyangtech.top

Py:   str(uuid.uuid4())
来源：http://knh.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gvq.tian-w.cn

JS:   crypto.randomUUID()
来源：http://bjr.hnxiangtu.top

TS:   crypto.randomUUID()
来源：http://ocf.jinqigufen.top

Java: UUID.randomUUID().toString()
来源：http://jor.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://rvz.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://rox.pycfn.com

C#:   Guid.NewGuid().ToString()
来源：http://ran.fktsv.cn

[P02] MD5 / SHA256 摘要
来源：http://dad.uphjek.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ggr.tianlin.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://wol.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cfp.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zre.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xde.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ngf.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vaq.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ymi.yangfankeji.com

[P03] 生成短随机字符串
来源：http://ure.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nax.zhijiandao.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jes.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hzi.cashguo.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://edc.ywan-chungtsiang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pfe.zdqjudy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xtc.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nbs.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fwz.zhiwuduotai.top

[P04] 求长度
来源：http://ica.sweek.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kke.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oev.andypj.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://stk.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ozm.sweek.top

Java: list.size();  map.size();  s.length()
来源：http://gcm.yueranfly.top

Go:   len(arr);  len(m)
来源：http://ydy.haohaochexian.top

Ruby: x.length;  x.size
来源：http://uvk.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://spk.jiagoushi.top

[P05] 判断两个对象内容是否相等
来源：http://gpe.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kqr.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ojc.meibo888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lkp.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wxf.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://spt.fktsv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zjd.guannengcc.top

Ruby: a == b
来源：http://rjv.52xcode.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://olh.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lqv.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iak.guowangkeji.top

PHP:  if (empty($x)) {}
来源：http://sgn.bbcook.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dic.zhengqikj.top

TS:   if (x == null) {}
来源：http://gew.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cgn.hfpthk.cn

Go:   if x == nil {}
来源：http://aqt.chenlongwang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uhf.ywan-chungtsiang.top

C#:   if (x is null) {}
来源：http://vnx.sxryk.cn

[P07] 防抖与节流
来源：http://rnj.hnqzz.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rvn.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://ipx.316326.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vwl.nanxinkj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lgn.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ylr.hesvh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pvh.zhongyouzk.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://diw.mhx1999.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cli.meibo888.top

[P08] 处理浮点精度问题
来源：http://zji.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hne.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hgp.shzxlz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rxx.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://niy.sufxvd.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://urd.cheryme.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jja.hnqzz.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://irk.xuetiantiany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mcv.316326.xyz

================================================================================
来源：http://avu.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://drb.birdmap.top

================================================================================
来源：http://qxu.hfpthk.cn

[Q01] 创建表
来源：http://odi.pengpengdd.cyou

CREATE TABLE users (
来源：http://xce.gaohongyu789.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ays.sufxvd.cn

name VARCHAR(50) NOT NULL,
来源：http://dtv.fzhhl.top

email VARCHAR(100) UNIQUE,
来源：http://yyk.bjfxy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://voc.zhengqikj.top

);
来源：http://bqp.zhengqikj.top

[Q02] 创建带外键的表
来源：http://xrm.yfazqb.com

CREATE TABLE orders (
来源：http://qkp.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yiu.tian-w.cn

user_id INT NOT NULL,
来源：http://epw.aizwys.cn

amount DECIMAL(10, 2),
来源：http://bmk.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nzz.gaohongyu789.top

);
来源：http://pxx.xuetiantiany.cn

[Q03] 增加列
来源：http://kfa.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://awn.hnqzz.top

[Q04] 修改列类型
来源：http://mpk.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bco.andypj.xyz

[Q05] 重命名列
来源：http://piy.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ecb.yanxiufei.cn

[Q06] 删除列
来源：http://gvs.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://oqo.shanyushiyangtech.top

[Q07] 删除表
来源：http://sem.cucudq.cn

DROP TABLE IF EXISTS orders;
来源：http://ccf.nanxinkj.top

[Q08] 创建普通索引
来源：http://lrl.yfazqb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://dtb.bjfxy.top

[Q09] 创建唯一索引
来源：http://fkg.pengpengdd.cyou

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://llt.yongpay.top

[Q10] 插入单行
来源：http://cyq.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nzh.jinyuanbaomall.cn

[Q11] 一次插入多行
来源：http://qip.redwolf501.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cew.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://ttz.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://kji.ehwqpu.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xsk.hysaishi.cn

[Q13] 忽略重复插入
来源：http://dnp.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://osz.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://gra.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sdy.snrcjt.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://svn.jinghuilouyu.cn

[Q15] 查询全部
来源：http://cvn.cucudq.cn

SELECT * FROM users;
来源：http://yme.yuxming.cn

[Q16] 查询指定列
来源：http://guu.gaohongyu789.top

SELECT id, name FROM users;
来源：http://gjb.yanxiufei.cn

[Q17] 条件查询
来源：http://dwf.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iks.shanyushiyangtech.top

[Q18] 模糊匹配
来源：http://qtd.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uij.hnqzz.top

[Q19] 范围查询
来源：http://fdx.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sou.yuanzhike.top

[Q20] IN 列表
来源：http://vxo.chenlongwang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dhj.chenlongwang.top

[Q21] 空值判断
来源：http://ktc.cqqwz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vry.zhixingplan.top

[Q22] 排序
来源：http://stx.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fes.jlsjyb.cn

[Q23] 分页
来源：http://mxf.yj20258888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ilk.zhaomingkeji.xyz

[Q24] 去重
来源：http://fbt.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://rpd.shanyushiyangtech.top

[Q25] 只取前 N 条
来源：http://cpy.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gvf.gogol.net.cn

[Q26] 计数
来源：http://zvb.52xcode.cn

SELECT COUNT(*) FROM users;
来源：http://eyb.pengpengdd.cyou

[Q27] 条件计数
来源：http://lsd.shuidangran.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hoo.xziqi.cn

[Q28] 求和与平均
来源：http://bli.pengpengdd.cyou

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zdj.cheryme.top

[Q29] 最大最小值
来源：http://nzz.chenlongwang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qou.shanyushiyangtech.top

[Q30] 分组统计
来源：http://xas.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tlx.cucudq.cn

[Q31] 分组后过滤
来源：http://zxm.gaohongyu789.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ric.zhaomingkeji.xyz

[Q32] 分组拼接字符串
来源：http://ouj.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zis.zhiwuduotai.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mxg.sxryk.cn

[Q33] 多列分组
来源：http://ruk.hnqzz.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ykl.hywenlv.cn

[Q34] 每组取第一条
来源：http://crj.bjfxy.top

SELECT * FROM (
来源：http://dmk.kuanghao11.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ntx.hnqzz.top

) t WHERE rn = 1;
来源：http://cci.jinqigufen.top

[Q35] 内连接
来源：http://oql.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aeo.vqdsnc.cn

[Q36] 左连接
来源：http://usm.wangdashe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ghf.zdqjudy.top

[Q37] 右连接
来源：http://ens.sysykeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://otl.guannengcc.top

[Q38] 全外连接（PostgreSQL）
来源：http://cfe.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zyv.c1oappe.top

[Q39] 自连接（查上下级）
来源：http://tro.yuxming.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xuk.kuanghao11.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://opr.dashuyun.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fhz.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://myv.yueranfly.top

[Q41] 多表连接
来源：http://uoq.ybcxt.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mjy.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://wve.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://edi.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://uod.chenzaomai.com

SELECT u.name, o.amount FROM users u
来源：http://lhd.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lvl.shuidangran.top

[Q43] 标量子查询
来源：http://qft.zhaomingkeji.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gsw.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://crk.iojbl.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://src.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://gox.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qkm.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://ckj.ydzc1.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dre.tarul.cn

[Q47] 与平均值比较
来源：http://tie.jqgfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lbb.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://nze.tian-w.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zck.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://yuv.cdnleiting.top

[Q49] 更新单行
来源：http://lwb.wangshuangyany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cqk.yongpay.top

[Q50] 批量更新
来源：http://jqw.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://abj.bjfxy.top

[Q51] 用子查询更新
来源：http://hvs.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bmg.yj202588.top

[Q52] 删除指定行
来源：http://yti.vehdjk.com

DELETE FROM users WHERE id = 10;
来源：http://htl.yangfankeji.com

[Q53] 按条件删除
来源：http://pnq.aibaodan.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://twr.daria6918.cn

[Q54] 清空表
来源：http://uia.bbcook.cn

TRUNCATE TABLE logs;
来源：http://obg.pengpengdd.cyou

[Q55] 排名（并列占位）
来源：http://apm.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bnr.yuanzhike.top

[Q56] 密集排名（并列不占位）
来源：http://ase.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tkj.ivvv.top

[Q57] 行号
来源：http://dfo.xingfuxueyuan.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://swo.hnqzz.top

[Q58] 累计求和
来源：http://sxh.yuanzhike.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://svh.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://zdo.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vlo.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://kkz.yj202588.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://inj.yuanzhike.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://csx.yanxiufei.cn

[Q61] 移动平均
来源：http://qtb.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uis.bbcook.cn

[Q62] 分组占比
来源：http://ykn.xziqi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fwe.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://dvd.wangdashe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tii.hcnkem.com

[Q64] 提交事务
来源：http://niz.zdbjq.cn

COMMIT;
来源：http://jws.vqdsnc.cn

[Q65] 回滚事务
来源：http://hip.hammf.cn

ROLLBACK;
来源：http://zgc.yj202588.top

[Q66] 行锁查询
来源：http://tff.vehdjk.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ica.yj20258.top

[Q67] 设置隔离级别
来源：http://afi.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gsv.jqgufenzy.top

[Q68] 保存点
来源：http://cdw.0kj1m.cn

SAVEPOINT sp1;
来源：http://stk.tarul.cn

ROLLBACK TO sp1;
来源：http://vxc.ywan-chungtsiang.top

[Q69] 查看执行计划
来源：http://tuq.hnqzz.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ucr.haohaochexian.top

[Q70] 更新统计信息
来源：http://ovw.chenzaomai.com


<!-- 参考信息 -->