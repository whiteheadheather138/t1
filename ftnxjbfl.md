代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jzc.ctjpmb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oqd.zhiwuduotai.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rmo.jlsjyb.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uga.svipenyu.cn

================================================================================
来源：http://ydx.fengsongda.top

O. 并发与异步
来源：http://bpk.ywan-chungtsiang.top

================================================================================
来源：http://jpt.yfazqb.com

[O01] 启动一个线程
来源：http://tom.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xqt.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uvy.jianghu66.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xbq.jqgfzy.top

TS:   // 同 JS
来源：http://blb.hcnkem.com

Java: new Thread(() -> f()).start()
来源：http://mob.cucudq.cn

Go:   go f()
来源：http://itm.feifeiyinyue.top

Ruby: Thread.new { f }
来源：http://usc.birdmap.top

C#:   Task.Run(() => F());
来源：http://sos.fzhhl.top

[O02] 使用线程池
来源：http://yuo.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://umw.ppjwa.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hzc.zdqjudy.top

JS:   // worker_threads 线程池
来源：http://ogi.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://bpn.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://ips.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hnn.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://anv.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://omz.fktsv.cn

[O03] 加锁保护共享数据
来源：http://kjl.ybcxt.top

Py:   with lock: shared += 1
来源：http://pvt.xingfuxueyuan.xyz

PHP:  // 用 flock() 做文件锁
来源：http://wxy.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fpx.fzhhl.top

TS:   // 同 JS
来源：http://rym.tanke756.top

Java: synchronized (this) { shared++; }
来源：http://lwj.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rfz.ivvv.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qog.svipenyu.cn

C#:   lock (gate) { shared++; }
来源：http://vxp.0kj1m.cn

[O04] 定义异步函数并等待
来源：http://juc.ivvv.top

Py:   async def f():⏎    await g()
来源：http://duc.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tvj.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://gyt.sjlbkw.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://htj.yonumen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bfp.uphjek.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gbz.yueranfly.top

Ruby: # 用 Fiber 或 async gem
来源：http://yte.pengpengdd.cyou

C#:   async Task F() { await G(); }
来源：http://cri.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://kzc.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://kgm.sjlbkw.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wkx.feifeiyinyue.top

JS:   await Promise.all(tasks)
来源：http://iyr.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://ppi.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mjd.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://euz.zhongyouzk.top

Ruby: threads.map(&:join)
来源：http://wqx.xuanzx.com

C#:   await Task.WhenAll(t1, t2)
来源：http://vvq.zhixingplan.top

[O06] 使用进程池
来源：http://tqq.fktsv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wak.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://etf.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://wem.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://igm.quarkkingdee.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jfz.daria6918.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lop.fktsv.cn

Ruby: // fork 块
来源：http://dkb.iojbl.cn

C#:   Parallel.For
来源：http://ljp.dashuyun.cn

================================================================================
来源：http://zix.316326.xyz

P. 常用工具函数
来源：http://vxv.0kj1m.cn

================================================================================
来源：http://xxh.shanyushiyangtech.top

[P01] 生成 UUID
来源：http://vth.hesvh.cn

Py:   str(uuid.uuid4())
来源：http://cmj.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yzr.cashguo.top

JS:   crypto.randomUUID()
来源：http://xcp.tarul.cn

TS:   crypto.randomUUID()
来源：http://lau.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://vmg.ydjk.org.cn

Go:   // 用 github.com/google/uuid
来源：http://uja.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://ohj.smart0.xyz

C#:   Guid.NewGuid().ToString()
来源：http://reh.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://kpz.zhixingplan.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fgl.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zjf.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://afg.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wuz.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aaq.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lni.zdbjq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nra.zhongyouzk.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rrg.dashuyun.cn

[P03] 生成短随机字符串
来源：http://bir.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wbx.feifeiyinyue.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bdt.ywan-chungtsiang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lrh.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dtq.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://khw.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vrd.shanyushiyangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jaf.fengsongda.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://knl.fanxiaobao.xyz

[P04] 求长度
来源：http://svh.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iwb.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ywi.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ftr.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qox.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://lka.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://edx.yongpay.top

Ruby: x.length;  x.size
来源：http://zga.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://flo.xylfe.cn

[P05] 判断两个对象内容是否相等
来源：http://ube.yj20258888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gwc.xingfuxueyuan.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ynz.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://spt.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ysc.zdbjq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cyd.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://qad.smart0.xyz

Ruby: a == b
来源：http://ull.hammf.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mfd.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://anj.jlsjyb.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hbd.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://nkn.ywan-chungtsiang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gpu.cdnleiting.top

TS:   if (x == null) {}
来源：http://bnt.zycfv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qmh.52xcode.cn

Go:   if x == nil {}
来源：http://gmf.ivvv.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uny.hongshengwenyu.top

C#:   if (x is null) {}
来源：http://kbq.shuidangran.top

[P07] 防抖与节流
来源：http://igm.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qdb.uphjek.com

PHP:  // 手写时间戳比较
来源：http://pqy.iojbl.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xcb.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zuo.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://thu.hywenlv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://utt.hfpthk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oip.haohaochexian.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mij.hongshengwenyu.top

[P08] 处理浮点精度问题
来源：http://wxd.yfazqb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hzl.sufxvd.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gem.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bxm.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wwj.yj20258.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hcu.smart0.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xha.tarul.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ivc.jiagoushi.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://peu.shanyushiyangtech.top

================================================================================
来源：http://nbe.yangfankeji.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aer.epnwcf.com

================================================================================
来源：http://beb.tian-w.cn

[Q01] 创建表
来源：http://cbj.jinyuanbaomall.cn

CREATE TABLE users (
来源：http://nso.jinyuanbaomall.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fnd.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://xln.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://stm.wangdashe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gxp.ydjk.org.cn

);
来源：http://nyd.yongpay.top

[Q02] 创建带外键的表
来源：http://eyx.fanxiaobao.xyz

CREATE TABLE orders (
来源：http://vll.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nbf.yonumen.top

user_id INT NOT NULL,
来源：http://mji.yonumen.top

amount DECIMAL(10, 2),
来源：http://vpk.xingfuxueyuan.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vvv.gogol.net.cn

);
来源：http://euf.jiagoushi.top

[Q03] 增加列
来源：http://ner.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dfk.gzhubu.top

[Q04] 修改列类型
来源：http://jpp.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fbh.xziqi.cn

[Q05] 重命名列
来源：http://evk.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iiv.aizwys.cn

[Q06] 删除列
来源：http://gtc.xylfe.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lgd.tianlin.xyz

[Q07] 删除表
来源：http://kwh.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://gcy.hammf.cn

[Q08] 创建普通索引
来源：http://vlm.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fzb.yj20258.top

[Q09] 创建唯一索引
来源：http://hgc.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ufy.gogol.net.cn

[Q10] 插入单行
来源：http://rpn.52xcode.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qmj.dianchejie.cn

[Q11] 一次插入多行
来源：http://ogr.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://thl.yongpay.top

[Q12] 插入后取自增 ID
来源：http://qzb.cheryme.top

INSERT INTO users (name) VALUES ('C');
来源：http://fic.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fsn.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://vih.yj202588.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dpo.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://arr.jianghu66.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gyj.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ugk.nanxinkj.top

[Q15] 查询全部
来源：http://ase.pengpengdd.cyou

SELECT * FROM users;
来源：http://veo.cashguo.top

[Q16] 查询指定列
来源：http://ubl.hysaishi.cn

SELECT id, name FROM users;
来源：http://hjz.andypj.xyz

[Q17] 条件查询
来源：http://lto.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://puz.jiagoushi.top

[Q18] 模糊匹配
来源：http://qaz.aizwys.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wkp.xinyue.icu

[Q19] 范围查询
来源：http://cac.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ice.shuidangran.top

[Q20] IN 列表
来源：http://yuw.zhixingplan.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://smu.aizwys.cn

[Q21] 空值判断
来源：http://aiw.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dzj.cucudq.cn

[Q22] 排序
来源：http://zjp.chenjidiqi.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uvv.shanyushiyangkeji.top

[Q23] 分页
来源：http://ugm.aibaodan.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qps.c1oappe.top

[Q24] 去重
来源：http://dzs.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://aue.xuanzx.com

[Q25] 只取前 N 条
来源：http://xfp.hysaishi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zbm.zdbjq.cn

[Q26] 计数
来源：http://syg.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://eit.yanxiufei.cn

[Q27] 条件计数
来源：http://sud.cucudq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mdk.epnwcf.com

[Q28] 求和与平均
来源：http://qak.jinqigfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rmz.shzxlz.cn

[Q29] 最大最小值
来源：http://yzl.aibaodan.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fjs.dashuyun.cn

[Q30] 分组统计
来源：http://ajd.hfpthk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://umt.yuxming.cn

[Q31] 分组后过滤
来源：http://lmx.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lto.yanxiufei.cn

[Q32] 分组拼接字符串
来源：http://wod.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vlr.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ufy.ydjk.org.cn

[Q33] 多列分组
来源：http://ech.cdnleiting.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ezd.zhongyouzk.top

[Q34] 每组取第一条
来源：http://qda.hnxiangtu.top

SELECT * FROM (
来源：http://pjp.jinqigufen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aky.ivvv.top

) t WHERE rn = 1;
来源：http://mod.havefunace.top

[Q35] 内连接
来源：http://oym.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://khm.hywenlv.cn

[Q36] 左连接
来源：http://crx.fengsongda.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xsu.zdbjq.cn

[Q37] 右连接
来源：http://guk.yj20258888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://stg.haohaochexian.top

[Q38] 全外连接（PostgreSQL）
来源：http://ywv.hcnkem.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rra.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://roe.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://uxw.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ymn.hnqzz.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fle.ydjk.org.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ake.hfpthk.cn

[Q41] 多表连接
来源：http://vus.jlsjyb.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xrd.jinqigufen.top

JOIN users u ON u.id = o.user_id
来源：http://kmc.hnqzz.top

JOIN products p ON p.id = o.product_id;
来源：http://pzx.ybcxt.top

[Q42] 连接条件附加过滤
来源：http://ene.uphjek.com

SELECT u.name, o.amount FROM users u
来源：http://nuy.hesvh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kob.fengsongda.top

[Q43] 标量子查询
来源：http://znp.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xtu.tian-w.cn

[Q44] IN 子查询
来源：http://ggy.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qoj.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://duy.jlsjyb.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://anj.pycfn.com

[Q46] NOT EXISTS 判断不存在
来源：http://orv.snrcjt.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wls.sxryk.cn

[Q47] 与平均值比较
来源：http://dmw.havefunace.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rvn.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://rsu.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sjt.fehbvm.com

SELECT * FROM t WHERE c > 5;
来源：http://dcq.shanyushiyangtech.top

[Q49] 更新单行
来源：http://npp.ctjpmb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uvj.fehbvm.com

[Q50] 批量更新
来源：http://nqw.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xcs.xuanzx.com

[Q51] 用子查询更新
来源：http://jax.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ock.c1oappe.top

[Q52] 删除指定行
来源：http://fry.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://qzl.sysykeji.top

[Q53] 按条件删除
来源：http://uxu.9152youxi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wnb.jqgufenzy.top

[Q54] 清空表
来源：http://uqd.wangdashe.top

TRUNCATE TABLE logs;
来源：http://dvm.xinyue.icu

[Q55] 排名（并列占位）
来源：http://yre.ydjk.org.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jzg.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://olt.ivvv.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cqu.daxiang520.top

[Q57] 行号
来源：http://odk.havefunace.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jyf.wangshuangyany.cn

[Q58] 累计求和
来源：http://mzq.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vyn.birdmap.top

[Q59] 分组内累计
来源：http://whc.ctjpmb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://niq.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://fhy.sjlbkw.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wow.daxiang520.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jye.hnqzz.top

[Q61] 移动平均
来源：http://nnb.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://moy.bbcook.cn

[Q62] 分组占比
来源：http://lvq.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rlx.daria6918.cn

[Q63] 开启事务
来源：http://nwm.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fox.xylfe.cn

[Q64] 提交事务
来源：http://umw.nwbrower.top

COMMIT;
来源：http://gdh.sjlbkw.cn

[Q65] 回滚事务
来源：http://gmx.jinqigfzy.top

ROLLBACK;
来源：http://rsp.jqgufenzy.top

[Q66] 行锁查询
来源：http://pfu.zhijiandao.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pmk.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://slf.yuanzhike.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vgb.yj202588.top

[Q68] 保存点
来源：http://zuh.0kj1m.cn

SAVEPOINT sp1;
来源：http://fwr.gzhubu.top

ROLLBACK TO sp1;
来源：http://jfh.jyoumei.cn

[Q69] 查看执行计划
来源：http://pld.daria6918.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xqa.yj202588.top

[Q70] 更新统计信息
来源：http://vor.cucudq.cn


<!-- 参考信息 -->