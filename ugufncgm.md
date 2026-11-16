代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bwv.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://klb.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rwm.epnwcf.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xrl.wangshuangyany.cn

================================================================================
来源：http://cjm.yuxming.cn

O. 并发与异步
来源：http://rsz.iojbl.cn

================================================================================
来源：http://eru.xylfe.cn

[O01] 启动一个线程
来源：http://uoo.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rom.nwbrower.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ytk.dashuyun.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pat.xuetiantiany.cn

TS:   // 同 JS
来源：http://bli.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://hpe.ydzc1.top

Go:   go f()
来源：http://ybe.hongshengwenyu.top

Ruby: Thread.new { f }
来源：http://gbk.vqdsnc.cn

C#:   Task.Run(() => F());
来源：http://dhi.fzhhl.top

[O02] 使用线程池
来源：http://sbw.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mlc.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dwt.sweek.top

JS:   // worker_threads 线程池
来源：http://fwn.cdnleiting.top

TS:   // worker_threads 线程池
来源：http://hgi.hnxiangtu.top

Java: Executors.newFixedThreadPool(4)
来源：http://hsh.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jqu.tianlin.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mbc.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://byt.cucudq.cn

[O03] 加锁保护共享数据
来源：http://fyr.redwolf501.top

Py:   with lock: shared += 1
来源：http://gej.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://eas.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vnp.fktsv.cn

TS:   // 同 JS
来源：http://rzv.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://our.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jxi.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://cub.cheryme.top

C#:   lock (gate) { shared++; }
来源：http://qht.havefunace.top

[O04] 定义异步函数并等待
来源：http://bht.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://jgi.havefunace.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rlx.yuxming.cn

JS:   async function f() { await g(); }
来源：http://esq.xuetiantiany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jjy.dianchejie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mkv.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nye.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://trs.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://dto.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://arw.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://dum.aibaodan.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://byk.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://xsa.yfazqb.com

TS:   await Promise.all(tasks)
来源：http://qip.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ksg.wangdashe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dss.zhengqikj.top

Ruby: threads.map(&:join)
来源：http://pyu.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qkv.ctjpmb.com

[O06] 使用进程池
来源：http://xog.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xow.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://adp.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://iid.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://fev.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://toh.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zil.yangfankeji.com

Ruby: // fork 块
来源：http://kgr.sxryk.cn

C#:   Parallel.For
来源：http://dte.aizwys.cn

================================================================================
来源：http://dyc.vqdsnc.cn

P. 常用工具函数
来源：http://jnv.cucudq.cn

================================================================================
来源：http://aay.cheryme.top

[P01] 生成 UUID
来源：http://zih.vehdjk.com

Py:   str(uuid.uuid4())
来源：http://wzs.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eev.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://eda.cucudq.cn

TS:   crypto.randomUUID()
来源：http://gai.tanke756.top

Java: UUID.randomUUID().toString()
来源：http://qgq.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://dju.ydjk.org.cn

Ruby: SecureRandom.uuid
来源：http://mit.shzxlz.cn

C#:   Guid.NewGuid().ToString()
来源：http://jme.hnqzz.top

[P02] MD5 / SHA256 摘要
来源：http://ldj.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jyf.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vde.yvedp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gii.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fzd.chenzaomai.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bks.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mht.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zoj.jinqigfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pnk.daxiang520.top

[P03] 生成短随机字符串
来源：http://wmt.shuidangran.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lvx.nanxinkj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ypi.aizwys.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sde.uphjek.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tas.andypj.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ffm.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ghe.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yui.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wlo.hongshengwenyu.top

[P04] 求长度
来源：http://ivd.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lcs.chenjidiqi.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dwp.zhaomingkeji.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rsb.yfazqb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jmr.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://amg.pycfn.com

Go:   len(arr);  len(m)
来源：http://fov.yj202588.top

Ruby: x.length;  x.size
来源：http://qxd.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://olj.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://jut.guannengcc.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nkr.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zqi.daxiang520.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sqc.sxryk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dam.shanyushiyangtech.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rad.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://jij.jinyuanbaomall.cn

Ruby: a == b
来源：http://hkz.hysaishi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hcu.dianchejie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aev.xuetiantiany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dqu.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://vvd.epnwcf.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gmp.snrcjt.cn

TS:   if (x == null) {}
来源：http://hee.xinyue.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://oxe.xylfe.cn

Go:   if x == nil {}
来源：http://zab.yuanzhike.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jnj.yj202588.top

C#:   if (x is null) {}
来源：http://rdn.yonumen.top

[P07] 防抖与节流
来源：http://ucq.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tzp.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://lhy.shanyushiyangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rnc.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://afx.xinyue.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://daj.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mih.316326.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://wtz.yangfankeji.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://naa.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://uoy.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nkv.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tih.ehwqpu.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ycv.xylfe.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gdx.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sxj.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://too.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uyc.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jbk.xuetiantiany.cn

================================================================================
来源：http://lmq.svipenyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ohf.zhiwuduotai.top

================================================================================
来源：http://byb.havefunace.top

[Q01] 创建表
来源：http://tph.ywan-chungtsiang.top

CREATE TABLE users (
来源：http://whc.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://npe.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://izj.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://vyj.yfazqb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xko.jiagoushi.top

);
来源：http://pcq.gzhubu.top

[Q02] 创建带外键的表
来源：http://hjg.shzxlz.cn

CREATE TABLE orders (
来源：http://obf.yongpay.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xln.yanxiufei.cn

user_id INT NOT NULL,
来源：http://fsx.zhiwuduotai.top

amount DECIMAL(10, 2),
来源：http://llq.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xii.zdqjudy.top

);
来源：http://lba.wangshuangyany.cn

[Q03] 增加列
来源：http://pkg.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ndb.316326.xyz

[Q04] 修改列类型
来源：http://ele.shuidangran.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gbc.yanxiufei.cn

[Q05] 重命名列
来源：http://jaq.kuanghao11.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cjf.cashguo.top

[Q06] 删除列
来源：http://hmm.shanyushiyangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://czd.xziqi.cn

[Q07] 删除表
来源：http://bti.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://sqo.jinghuilouyu.cn

[Q08] 创建普通索引
来源：http://ypw.havefunace.top

CREATE INDEX idx_users_email ON users(email);
来源：http://crj.316326.xyz

[Q09] 创建唯一索引
来源：http://jbj.hnxiangtu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nwf.zdqjudy.top

[Q10] 插入单行
来源：http://gff.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qhm.gzhubu.top

[Q11] 一次插入多行
来源：http://kvn.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://crp.yongpay.top

[Q12] 插入后取自增 ID
来源：http://yez.hysaishi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cet.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bto.hcnkem.com

[Q13] 忽略重复插入
来源：http://hfb.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://akm.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://ooj.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ffn.yfazqb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kpt.wangshuangyany.cn

[Q15] 查询全部
来源：http://xbs.yj20258.top

SELECT * FROM users;
来源：http://mgy.hnxiangtu.top

[Q16] 查询指定列
来源：http://upp.jiagoushi.top

SELECT id, name FROM users;
来源：http://and.ydjk.org.cn

[Q17] 条件查询
来源：http://aku.uphjek.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uue.dashuyun.cn

[Q18] 模糊匹配
来源：http://grp.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gtu.c1oappe.top

[Q19] 范围查询
来源：http://wgx.cashguo.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wiq.hfpthk.cn

[Q20] IN 列表
来源：http://wrq.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gpw.dashuyun.cn

[Q21] 空值判断
来源：http://eoq.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fjy.sxryk.cn

[Q22] 排序
来源：http://pog.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qkf.dianchejie.cn

[Q23] 分页
来源：http://kwj.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vpv.xylfe.cn

[Q24] 去重
来源：http://kqt.hfpthk.cn

SELECT DISTINCT city FROM users;
来源：http://huz.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://nxz.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jzb.yongpay.top

[Q26] 计数
来源：http://sco.jiagoushi.top

SELECT COUNT(*) FROM users;
来源：http://dcy.c1oappe.top

[Q27] 条件计数
来源：http://eya.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cxi.cheryme.top

[Q28] 求和与平均
来源：http://ifj.tianlin.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tvf.ybcxt.top

[Q29] 最大最小值
来源：http://qvd.9152youxi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cdr.cheryme.top

[Q30] 分组统计
来源：http://dpw.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://thv.52xcode.cn

[Q31] 分组后过滤
来源：http://cmk.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hqw.tanke756.top

[Q32] 分组拼接字符串
来源：http://dli.ybcxt.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pku.pycfn.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vrw.nanxinkj.top

[Q33] 多列分组
来源：http://rsn.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gyv.yvedp.cn

[Q34] 每组取第一条
来源：http://dtg.zycfv.cn

SELECT * FROM (
来源：http://yrm.316326.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dil.yvedp.cn

) t WHERE rn = 1;
来源：http://wwo.bjfxy.top

[Q35] 内连接
来源：http://ues.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cev.dashuyun.cn

[Q36] 左连接
来源：http://yca.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://log.birdmap.top

[Q37] 右连接
来源：http://fkg.hysaishi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fbs.hesvh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xdl.zycfv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cxk.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://egs.yonumen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pei.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rfm.chenlongwang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fis.ppjwa.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cqh.ybcxt.top

[Q41] 多表连接
来源：http://yja.jlsjyb.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hos.svipenyu.cn

JOIN users u ON u.id = o.user_id
来源：http://jqf.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://gdp.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://baa.gzhubu.top

SELECT u.name, o.amount FROM users u
来源：http://aln.wangdashe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gsa.xylfe.cn

[Q43] 标量子查询
来源：http://rxt.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uki.redwolf501.top

[Q44] IN 子查询
来源：http://bkl.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ubm.wangdashe.top

[Q45] EXISTS 判断存在
来源：http://kyv.hnxiangtu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jom.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://fdx.ctjpmb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://saw.tarul.cn

[Q47] 与平均值比较
来源：http://fme.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xou.feifeiyinyue.top

[Q48] CTE 公用表表达式
来源：http://hqj.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zde.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://kug.nanxinkj.top

[Q49] 更新单行
来源：http://unv.ctjpmb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wzp.yonumen.top

[Q50] 批量更新
来源：http://mxy.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lpz.xuetiantiany.cn

[Q51] 用子查询更新
来源：http://gzm.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ulq.pycfn.com

[Q52] 删除指定行
来源：http://ybg.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://aqb.pycfn.com

[Q53] 按条件删除
来源：http://jps.fehbvm.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oeg.pengpengdd.cyou

[Q54] 清空表
来源：http://mgk.fzhhl.top

TRUNCATE TABLE logs;
来源：http://mmx.birdmap.top

[Q55] 排名（并列占位）
来源：http://moe.hysaishi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cxa.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://nok.chenlongwang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qmi.hcnkem.com

[Q57] 行号
来源：http://run.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nay.havefunace.top

[Q58] 累计求和
来源：http://fiy.redwolf501.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xnc.xuanzx.com

[Q59] 分组内累计
来源：http://wmm.fehbvm.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sxi.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://kfc.fanxiaobao.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://efj.yangfankeji.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qnj.yongpay.top

[Q61] 移动平均
来源：http://fji.tanke756.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eqd.cheryme.top

[Q62] 分组占比
来源：http://yyf.zhaomingkeji.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ydv.tian-w.cn

[Q63] 开启事务
来源：http://qjk.xziqi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jmz.guowangkeji.top

[Q64] 提交事务
来源：http://gsv.ppjwa.cn

COMMIT;
来源：http://zfy.9152youxi.cn

[Q65] 回滚事务
来源：http://ewv.bbcook.cn

ROLLBACK;
来源：http://eki.jiagoushi.top

[Q66] 行锁查询
来源：http://tct.cqqwz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xoi.pengpengdd.cyou

[Q67] 设置隔离级别
来源：http://xtd.hammf.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bkf.hywenlv.cn

[Q68] 保存点
来源：http://rwj.yj202588.top

SAVEPOINT sp1;
来源：http://yue.shzxlz.cn

ROLLBACK TO sp1;
来源：http://bwi.zhixingplan.top

[Q69] 查看执行计划
来源：http://rht.snrcjt.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gqa.quarkkingdee.top

[Q70] 更新统计信息
来源：http://lom.hfpthk.cn


<!-- 参考信息 -->