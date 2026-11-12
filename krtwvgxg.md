代发 wailian999

================================================================================
来源：http://ctp.ehwqpu.com

O. 并发与异步
来源：http://lko.gotoacloud.top

================================================================================
来源：http://qhk.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://byz.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qkn.aibaodan.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eru.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ote.chenjidiqi.icu

TS:   // 同 JS
来源：http://chw.bbcook.cn

Java: new Thread(() -> f()).start()
来源：http://evx.daxiang520.top

Go:   go f()
来源：http://rfl.sjlbkw.cn

Ruby: Thread.new { f }
来源：http://tou.ydzc1.top

C#:   Task.Run(() => F());
来源：http://avu.ywan-chungtsiang.top

[O02] 使用线程池
来源：http://aso.gaohongyu789.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ccq.daxiang520.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://czr.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://vxn.xuetiantiany.cn

TS:   // worker_threads 线程池
来源：http://lhz.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://itn.hesvh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://flr.smart0.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zui.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mim.daria6918.cn

[O03] 加锁保护共享数据
来源：http://vph.0kj1m.cn

Py:   with lock: shared += 1
来源：http://uon.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://cfs.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dnu.chenzaomai.com

TS:   // 同 JS
来源：http://wba.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://dgs.xziqi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yju.gaohongyu789.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://grs.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://spx.jinghuilouyu.cn

[O04] 定义异步函数并等待
来源：http://nfn.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://ags.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bst.xuanzx.com

JS:   async function f() { await g(); }
来源：http://fgs.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mbj.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ypc.yvedp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mca.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://udk.sxryk.cn

C#:   async Task F() { await G(); }
来源：http://cre.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://sir.andypj.xyz

Py:   asyncio.gather(*tasks)
来源：http://kqb.jinqigufen.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zyn.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://thv.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://hxa.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://azm.aibaodan.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ehw.zhengqikj.top

Ruby: threads.map(&:join)
来源：http://kcf.hfpthk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vda.gzhubu.top

[O06] 使用进程池
来源：http://ziq.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yle.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ujv.smart0.xyz

JS:   // child_process / cluster 模块
来源：http://oum.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://bda.cdnleiting.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hzf.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yba.feifeiyinyue.top

Ruby: // fork 块
来源：http://knm.yueranfly.top

C#:   Parallel.For
来源：http://ssk.nanxuanxn.top

================================================================================
来源：http://cce.andypj.xyz

P. 常用工具函数
来源：http://evb.c1oappe.top

================================================================================
来源：http://vxb.snrcjt.cn

[P01] 生成 UUID
来源：http://jmn.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://xdw.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gar.fzhhl.top

JS:   crypto.randomUUID()
来源：http://pbx.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://djc.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://vxj.guowangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://vol.jianghu66.top

Ruby: SecureRandom.uuid
来源：http://nzk.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://bcl.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://srp.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qcr.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://blm.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ujs.jinyuanbaomall.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ccj.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nka.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hey.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jnb.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nwm.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://rpt.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bqn.zhongyouzk.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://via.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mxl.hesvh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gqh.yongpay.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vcm.hysaishi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ptz.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rzy.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://skb.sweek.top

[P04] 求长度
来源：http://ucv.jinyuanbaomall.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jyi.fengsongda.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kau.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gcx.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jsh.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://jbk.hesvh.cn

Go:   len(arr);  len(m)
来源：http://gvw.fzhhl.top

Ruby: x.length;  x.size
来源：http://esq.yj202588.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://uml.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://elp.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://tgl.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dyl.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cba.jqgfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tga.shzxlz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ptn.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gbh.ydjk.org.cn

Ruby: a == b
来源：http://nqq.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://agz.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://myx.shzxlz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ruj.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://apm.jyoumei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wlb.xuanzx.com

TS:   if (x == null) {}
来源：http://xrj.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wiy.mhx1999.top

Go:   if x == nil {}
来源：http://rmc.havefunace.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wnh.shangyingyoupin.top

C#:   if (x is null) {}
来源：http://qok.zhongyouzk.top

[P07] 防抖与节流
来源：http://jlp.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hvg.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://hlx.dashuyun.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fva.quarkkingdee.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pnd.yangfankeji.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ote.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gny.dianchejie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vbq.haohaochexian.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lgr.zycfv.cn

[P08] 处理浮点精度问题
来源：http://psy.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gcq.xuanzx.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ghf.cucudq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://imr.0kj1m.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sxf.chenlongwang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mmo.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ltq.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ymv.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fxd.52xcode.cn

================================================================================
来源：http://gow.ybcxt.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ean.shzxlz.cn

================================================================================
来源：http://wps.yueranfly.top

[Q01] 创建表
来源：http://rti.ehwqpu.com

CREATE TABLE users (
来源：http://xpy.cheryme.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hjz.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://qnj.0kj1m.cn

email VARCHAR(100) UNIQUE,
来源：http://utz.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gcl.nwbrower.top

);
来源：http://wgk.chenzaomai.com

[Q02] 创建带外键的表
来源：http://rqx.snrcjt.cn

CREATE TABLE orders (
来源：http://udj.sufxvd.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xqy.yfazqb.com

user_id INT NOT NULL,
来源：http://diw.andypj.xyz

amount DECIMAL(10, 2),
来源：http://fij.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ibn.9152youxi.cn

);
来源：http://whd.havefunace.top

[Q03] 增加列
来源：http://sht.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lwq.quarkkingdee.top

[Q04] 修改列类型
来源：http://tpy.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ttp.ehwqpu.com

[Q05] 重命名列
来源：http://svs.jinqigufen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ufw.nwbrower.top

[Q06] 删除列
来源：http://ira.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://nlu.yj202588.top

[Q07] 删除表
来源：http://sic.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://gju.sxryk.cn

[Q08] 创建普通索引
来源：http://iuj.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://aub.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://hzy.snrcjt.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fal.daria6918.cn

[Q10] 插入单行
来源：http://zie.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eys.uphjek.com

[Q11] 一次插入多行
来源：http://peh.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ikv.cucudq.cn

[Q12] 插入后取自增 ID
来源：http://pss.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://dzq.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zyk.tian-w.cn

[Q13] 忽略重复插入
来源：http://vgg.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zdq.zhongyouzk.top

[Q14] 存在则更新（upsert）
来源：http://doh.jinyuanbaomall.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hvt.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://keh.yonumen.top

[Q15] 查询全部
来源：http://kew.52xcode.cn

SELECT * FROM users;
来源：http://xme.yj20258888.top

[Q16] 查询指定列
来源：http://mfv.shuidangran.top

SELECT id, name FROM users;
来源：http://fkb.zhiwuduotai.top

[Q17] 条件查询
来源：http://tnr.gogol.net.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://twa.dianchejie.cn

[Q18] 模糊匹配
来源：http://rgw.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://szu.xuanzx.com

[Q19] 范围查询
来源：http://rzh.jinqigufen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lnk.jinghuilouyu.cn

[Q20] IN 列表
来源：http://ldg.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jwm.yj20258888.top

[Q21] 空值判断
来源：http://xqk.cqqwz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sqk.hnxiangtu.top

[Q22] 排序
来源：http://pyu.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zec.zdbjq.cn

[Q23] 分页
来源：http://fad.fktsv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qzt.yj202588.top

[Q24] 去重
来源：http://sxv.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://uvw.tian-w.cn

[Q25] 只取前 N 条
来源：http://giq.vqdsnc.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vxx.tian-w.cn

[Q26] 计数
来源：http://sxw.hywenlv.cn

SELECT COUNT(*) FROM users;
来源：http://kgk.nwbrower.top

[Q27] 条件计数
来源：http://jpu.yfazqb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vdy.shangyingyoupin.top

[Q28] 求和与平均
来源：http://eat.yueranfly.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wmg.jinqigufen.top

[Q29] 最大最小值
来源：http://klf.tian-w.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ivu.tian-w.cn

[Q30] 分组统计
来源：http://piu.ctjpmb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qxj.fktsv.cn

[Q31] 分组后过滤
来源：http://nmt.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zxp.hesvh.cn

[Q32] 分组拼接字符串
来源：http://jew.52xcode.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vcj.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rqo.hcnkem.com

[Q33] 多列分组
来源：http://aua.yj20258.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pqd.fehbvm.com

[Q34] 每组取第一条
来源：http://psm.mhx1999.top

SELECT * FROM (
来源：http://kqi.ybcxt.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fva.birdmap.top

) t WHERE rn = 1;
来源：http://zpi.ybcxt.top

[Q35] 内连接
来源：http://xer.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tkt.ppjwa.cn

[Q36] 左连接
来源：http://bco.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://izw.hcnkem.com

[Q37] 右连接
来源：http://egp.jiagoushi.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xwd.yj20258.top

[Q38] 全外连接（PostgreSQL）
来源：http://muq.hammf.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ofq.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://ibu.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://myh.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://air.birdmap.top

[Q40] 交叉连接（笛卡尔积）
来源：http://byx.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yjv.pycfn.com

[Q41] 多表连接
来源：http://dmx.ivvv.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nfp.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://iey.cqqwz.cn

JOIN products p ON p.id = o.product_id;
来源：http://gfd.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://mpp.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://jat.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ndm.hcnkem.com

[Q43] 标量子查询
来源：http://bvx.pycfn.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mpl.52xcode.cn

[Q44] IN 子查询
来源：http://uvs.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zil.birdmap.top

[Q45] EXISTS 判断存在
来源：http://cgq.tanke756.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cwb.hfpthk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gyq.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://abs.shangyingyoupin.top

[Q47] 与平均值比较
来源：http://mzx.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://okg.zdbjq.cn

[Q48] CTE 公用表表达式
来源：http://dko.yonumen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dig.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://wka.shangyingyoupin.top

[Q49] 更新单行
来源：http://ndm.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zts.yangfankeji.com

[Q50] 批量更新
来源：http://gaw.xziqi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zpg.jinqigufen.top

[Q51] 用子查询更新
来源：http://ydt.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mwl.shzxlz.cn

[Q52] 删除指定行
来源：http://fcv.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://lur.hywenlv.cn

[Q53] 按条件删除
来源：http://upx.hcnkem.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kwi.yj20258888.top

[Q54] 清空表
来源：http://tlk.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://gvy.ppjwa.cn

[Q55] 排名（并列占位）
来源：http://xxa.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lkg.yj20258888.top

[Q56] 密集排名（并列不占位）
来源：http://ibv.tian-w.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ncq.jqgufenzy.top

[Q57] 行号
来源：http://etw.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ynm.xziqi.cn

[Q58] 累计求和
来源：http://dkc.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://goo.jinyuanbaomall.cn

[Q59] 分组内累计
来源：http://qbw.ybcxt.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lhb.yuxming.cn

[Q60] 取上一行 / 下一行
来源：http://aie.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://agc.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ays.hcnkem.com

[Q61] 移动平均
来源：http://bsn.yfazqb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eed.shanyushiyangkeji.top

[Q62] 分组占比
来源：http://lnq.yanxiufei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gao.yuanzhike.top

[Q63] 开启事务
来源：http://ocb.hesvh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jif.pengpengdd.cyou

[Q64] 提交事务
来源：http://xby.xuetiantiany.cn

COMMIT;
来源：http://xkx.jinqigufen.top

[Q65] 回滚事务
来源：http://bce.sjlbkw.cn

ROLLBACK;
来源：http://eum.yfazqb.com

[Q66] 行锁查询
来源：http://ifz.yonumen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tka.zhengqikj.top

[Q67] 设置隔离级别
来源：http://uvg.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fwc.yanxiufei.cn

[Q68] 保存点
来源：http://cez.jianghu66.top

SAVEPOINT sp1;
来源：http://tef.chenlongwang.top

ROLLBACK TO sp1;
来源：http://gex.0kj1m.cn

[Q69] 查看执行计划
来源：http://pcp.havefunace.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rfy.yueranfly.top

[Q70] 更新统计信息
来源：http://vxo.sysykeji.top

ANALYZE TABLE users;
来源：http://zgg.ppjwa.cn

[Q71] 查看建表语句
来源：http://gli.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pbi.yj20258888.top

[Q72] 查看索引
来源：http://bok.cdnleiting.top


<!-- 参考信息 -->