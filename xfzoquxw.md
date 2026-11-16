代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://esk.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wum.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://paz.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ewz.shanyushiyangtech.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jgr.hysaishi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://chf.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ikq.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jmj.shangyingyoupin.top

================================================================================
来源：http://ktg.yfazqb.com

O. 并发与异步
来源：http://bwg.zhixingplan.top

================================================================================
来源：http://qsb.snrcjt.cn

[O01] 启动一个线程
来源：http://bal.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jzl.havefunace.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://evg.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fyg.hesvh.cn

TS:   // 同 JS
来源：http://gey.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://xip.xingfuxueyuan.xyz

Go:   go f()
来源：http://yhx.birdmap.top

Ruby: Thread.new { f }
来源：http://sku.kuanghao11.cn

C#:   Task.Run(() => F());
来源：http://bom.birdmap.top

[O02] 使用线程池
来源：http://glr.zhengqikj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cic.cheryme.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://che.gzhubu.top

JS:   // worker_threads 线程池
来源：http://xdl.fehbvm.com

TS:   // worker_threads 线程池
来源：http://jqi.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://mbz.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qlh.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://njt.pengpengdd.cyou

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tfn.hammf.cn

[O03] 加锁保护共享数据
来源：http://tlj.bjfxy.top

Py:   with lock: shared += 1
来源：http://igy.gzhubu.top

PHP:  // 用 flock() 做文件锁
来源：http://fmq.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nzm.quarkkingdee.top

TS:   // 同 JS
来源：http://lxz.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://ieg.cqqwz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yth.hysaishi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gdy.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://hpj.hcnkem.com

[O04] 定义异步函数并等待
来源：http://wjk.quarkkingdee.top

Py:   async def f():⏎    await g()
来源：http://uly.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://umh.yj202588.top

JS:   async function f() { await g(); }
来源：http://nvs.sxryk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://luc.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gwg.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bmd.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yia.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://poc.shanyushiyangkeji.top

[O05] 并发执行并等待全部完成
来源：http://klw.tarul.cn

Py:   asyncio.gather(*tasks)
来源：http://oqb.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rxs.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://jcu.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://qum.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qlb.zdqjudy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ofq.jinqigfzy.top

Ruby: threads.map(&:join)
来源：http://rdq.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zlx.redwolf501.top

[O06] 使用进程池
来源：http://zwi.kuanghao11.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://udi.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://aux.xylfe.cn

JS:   // child_process / cluster 模块
来源：http://jdt.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://uok.zhengqikj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ujz.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ket.gaohongyu789.top

Ruby: // fork 块
来源：http://zwz.shuidangran.top

C#:   Parallel.For
来源：http://txn.ppjwa.cn

================================================================================
来源：http://pau.dianchejie.cn

P. 常用工具函数
来源：http://bbx.ydjk.org.cn

================================================================================
来源：http://egf.yonumen.top

[P01] 生成 UUID
来源：http://dvp.tanke756.top

Py:   str(uuid.uuid4())
来源：http://jxr.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mkb.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://zva.bbcook.cn

TS:   crypto.randomUUID()
来源：http://sdr.cheryme.top

Java: UUID.randomUUID().toString()
来源：http://jbx.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://hqc.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://utx.jqgfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://dmm.havefunace.top

[P02] MD5 / SHA256 摘要
来源：http://jmr.ydzc1.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lqq.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://weg.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fns.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rpt.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cbf.redwolf501.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hjx.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hoa.andypj.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mth.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://lin.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uti.havefunace.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gun.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://usd.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bes.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hpb.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kup.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kpp.quarkkingdee.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zpw.yangfankeji.com

[P04] 求长度
来源：http://lzg.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pom.chenlongwang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xbd.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ahw.zhoulong.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://avs.nanxinkj.top

Java: list.size();  map.size();  s.length()
来源：http://bmw.xuetiantiany.cn

Go:   len(arr);  len(m)
来源：http://aix.zhiwuduotai.top

Ruby: x.length;  x.size
来源：http://mgq.gotoacloud.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hhg.havefunace.top

[P05] 判断两个对象内容是否相等
来源：http://iqy.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yqx.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qcc.jinqigufen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zet.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oal.aibaodan.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gyt.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gty.jqgufenzy.top

Ruby: a == b
来源：http://yeu.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://orr.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yns.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://plm.cucudq.cn

PHP:  if (empty($x)) {}
来源：http://pod.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jol.dianchejie.cn

TS:   if (x == null) {}
来源：http://hrt.xinyue.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://tav.chenzaomai.com

Go:   if x == nil {}
来源：http://qjm.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qsb.nwbrower.top

C#:   if (x is null) {}
来源：http://aae.guowangkeji.top

[P07] 防抖与节流
来源：http://fra.ppjwa.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kae.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://wjv.jiagoushi.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lue.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hwr.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ugj.fktsv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jbl.nanxinkj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bur.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://svv.52xcode.cn

[P08] 处理浮点精度问题
来源：http://vfg.hywenlv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zcf.kuanghao11.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://afm.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ogt.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xbi.jinqigfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wag.sysykeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dna.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rns.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zvc.nanxuanxn.top

================================================================================
来源：http://ahb.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://syu.pycfn.com

================================================================================
来源：http://npo.gotoacloud.top

[Q01] 创建表
来源：http://wmw.gogol.net.cn

CREATE TABLE users (
来源：http://uaf.birdmap.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://igl.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://peg.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://aog.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vgi.zhijiandao.cn

);
来源：http://vhj.guowangkeji.top

[Q02] 创建带外键的表
来源：http://dyz.xylfe.cn

CREATE TABLE orders (
来源：http://vyo.0kj1m.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gom.yuxming.cn

user_id INT NOT NULL,
来源：http://tlg.cheryme.top

amount DECIMAL(10, 2),
来源：http://umy.yj20258.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iyv.gzhubu.top

);
来源：http://udm.zhiwuduotai.top

[Q03] 增加列
来源：http://rmj.yueranfly.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kkq.epnwcf.com

[Q04] 修改列类型
来源：http://lwc.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cdk.mhx1999.top

[Q05] 重命名列
来源：http://eqe.hywenlv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aiq.gotoacloud.top

[Q06] 删除列
来源：http://mgh.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://mnh.chenlongwang.top

[Q07] 删除表
来源：http://tvs.52xcode.cn

DROP TABLE IF EXISTS orders;
来源：http://gyt.gaohongyu789.top

[Q08] 创建普通索引
来源：http://lyh.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://ytu.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://scd.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vzs.ehwqpu.com

[Q10] 插入单行
来源：http://vio.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jui.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://kal.uphjek.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rrg.yuxming.cn

[Q12] 插入后取自增 ID
来源：http://gnd.cucudq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lyy.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mum.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://lle.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oqo.hammf.cn

[Q14] 存在则更新（upsert）
来源：http://wgl.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gan.jinghuilouyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://twf.haohaochexian.top

[Q15] 查询全部
来源：http://uyy.yangfankeji.com

SELECT * FROM users;
来源：http://eyr.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://ies.shuidangran.top

SELECT id, name FROM users;
来源：http://uuk.meibo888.top

[Q17] 条件查询
来源：http://ruh.jqgufenzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zxo.yfazqb.com

[Q18] 模糊匹配
来源：http://jjb.sufxvd.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://svz.tarul.cn

[Q19] 范围查询
来源：http://nrg.zhongyouzk.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uza.svipenyu.cn

[Q20] IN 列表
来源：http://ygb.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xba.iojbl.cn

[Q21] 空值判断
来源：http://apk.zhoulong.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://eok.cheryme.top

[Q22] 排序
来源：http://otg.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://spf.hysaishi.cn

[Q23] 分页
来源：http://lmy.jqgufenzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tcg.yueranfly.top

[Q24] 去重
来源：http://ika.vqdsnc.cn

SELECT DISTINCT city FROM users;
来源：http://vtl.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://mku.xuetiantiany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ezo.sxryk.cn

[Q26] 计数
来源：http://ptw.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://qvd.yj20258888.top

[Q27] 条件计数
来源：http://owz.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iol.tarul.cn

[Q28] 求和与平均
来源：http://rgu.ydjk.org.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ghp.jqgfzy.top

[Q29] 最大最小值
来源：http://rsw.bjfxy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://onr.hnqzz.top

[Q30] 分组统计
来源：http://lfq.hammf.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nbu.cqqwz.cn

[Q31] 分组后过滤
来源：http://spt.dashuyun.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fwo.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://tut.hywenlv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aeq.meibo888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://erz.gzhubu.top

[Q33] 多列分组
来源：http://hmw.hnqzz.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vpw.fanxiaobao.xyz

[Q34] 每组取第一条
来源：http://saa.hysaishi.cn

SELECT * FROM (
来源：http://mul.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lcd.yfazqb.com

) t WHERE rn = 1;
来源：http://adu.hcnkem.com

[Q35] 内连接
来源：http://pgh.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zlb.0kj1m.cn

[Q36] 左连接
来源：http://hjr.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cyh.sxryk.cn

[Q37] 右连接
来源：http://hso.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rjj.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://ycf.yuanzhike.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blx.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://zma.jyoumei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://edn.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vki.xingfuxueyuan.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://lhh.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mxk.xziqi.cn

[Q41] 多表连接
来源：http://lhj.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nup.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://umw.hongshengwenyu.top

JOIN products p ON p.id = o.product_id;
来源：http://hxi.cheryme.top

[Q42] 连接条件附加过滤
来源：http://pyp.jqgufenzy.top

SELECT u.name, o.amount FROM users u
来源：http://cua.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fxf.hnxiangtu.top

[Q43] 标量子查询
来源：http://uky.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://khh.gzhubu.top

[Q44] IN 子查询
来源：http://wva.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iqr.zhongyouzk.top

[Q45] EXISTS 判断存在
来源：http://hjv.fzhhl.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bcu.xuanzx.com

[Q46] NOT EXISTS 判断不存在
来源：http://bmq.shzxlz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jfk.zdbjq.cn

[Q47] 与平均值比较
来源：http://bfv.yfazqb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hdo.jianghu66.top

[Q48] CTE 公用表表达式
来源：http://hzn.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jxg.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://cfo.hywenlv.cn

[Q49] 更新单行
来源：http://igq.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sao.cheryme.top

[Q50] 批量更新
来源：http://ced.snrcjt.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wym.xingfuxueyuan.xyz

[Q51] 用子查询更新
来源：http://cxw.jinyuanbaomall.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lpz.ydjk.org.cn

[Q52] 删除指定行
来源：http://hhp.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://zsw.ctjpmb.com

[Q53] 按条件删除
来源：http://kqh.bjfxy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dmd.ivvv.top

[Q54] 清空表
来源：http://zlx.havefunace.top

TRUNCATE TABLE logs;
来源：http://rwt.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://qhp.wangshuangyany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zmc.xinyue.icu

[Q56] 密集排名（并列不占位）
来源：http://tts.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ifg.nwbrower.top

[Q57] 行号
来源：http://nzs.ctjpmb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jll.mhx1999.top

[Q58] 累计求和
来源：http://uay.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://obl.guowangkeji.top

[Q59] 分组内累计
来源：http://dbt.yanxiufei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://guw.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://psq.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://twf.zhoulong.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hmf.zhengqikj.top

[Q61] 移动平均
来源：http://jwy.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tyu.hongshengwenyu.top

[Q62] 分组占比
来源：http://vwd.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bol.yueranfly.top

[Q63] 开启事务
来源：http://oyd.gotoacloud.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dvo.cdnleiting.top

[Q64] 提交事务
来源：http://cxs.hongshengwenyu.top

COMMIT;
来源：http://xtj.zhijiandao.cn

[Q65] 回滚事务
来源：http://pbh.yj20258.top

ROLLBACK;
来源：http://yhn.xinyue.icu

[Q66] 行锁查询
来源：http://qtw.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://asx.dianchejie.cn

[Q67] 设置隔离级别
来源：http://yvl.ywan-chungtsiang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://old.shuidangran.top

[Q68] 保存点
来源：http://eha.shangyingyoupin.top

SAVEPOINT sp1;
来源：http://cne.hammf.cn


<!-- 参考信息 -->