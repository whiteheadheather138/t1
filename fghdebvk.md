代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nec.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mnf.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nwz.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gwi.zhaomingkeji.xyz

================================================================================
来源：http://gjb.jianghu66.top

O. 并发与异步
来源：http://anh.fzhhl.top

================================================================================
来源：http://ade.ehwqpu.com

[O01] 启动一个线程
来源：http://cak.yongpay.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gwy.jiagoushi.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yxx.fanxiaobao.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qdc.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://tip.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://efp.wangdashe.top

Go:   go f()
来源：http://hkf.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://lgx.daria6918.cn

C#:   Task.Run(() => F());
来源：http://mli.ybcxt.top

[O02] 使用线程池
来源：http://lsb.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jgg.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hld.kuanghao11.cn

JS:   // worker_threads 线程池
来源：http://zvn.wangshuangyany.cn

TS:   // worker_threads 线程池
来源：http://fei.tian-w.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ljv.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://smr.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cdq.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zsr.jlsjyb.cn

[O03] 加锁保护共享数据
来源：http://ayu.ppjwa.cn

Py:   with lock: shared += 1
来源：http://hbn.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://dyk.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lhi.nwbrower.top

TS:   // 同 JS
来源：http://aei.zhiwuduotai.top

Java: synchronized (this) { shared++; }
来源：http://jge.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hru.hcnkem.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://lne.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://tsu.xinyue.icu

[O04] 定义异步函数并等待
来源：http://lve.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://djb.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eec.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://tdp.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hzo.tarul.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://amw.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ucg.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eml.nanxuanxn.top

C#:   async Task F() { await G(); }
来源：http://leh.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://yxv.wangdashe.top

Py:   asyncio.gather(*tasks)
来源：http://fae.sxryk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nqx.fanxiaobao.xyz

JS:   await Promise.all(tasks)
来源：http://hen.zhaomingkeji.xyz

TS:   await Promise.all(tasks)
来源：http://odp.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://btf.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hxf.0kj1m.cn

Ruby: threads.map(&:join)
来源：http://rca.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pys.wangshuangyany.cn

[O06] 使用进程池
来源：http://irv.sweek.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sls.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://afm.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://pdn.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://gpj.ybcxt.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hhy.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vgh.jinqigufen.top

Ruby: // fork 块
来源：http://bte.meibo888.top

C#:   Parallel.For
来源：http://zvw.birdmap.top

================================================================================
来源：http://alx.yj20258888.top

P. 常用工具函数
来源：http://xta.fehbvm.com

================================================================================
来源：http://hka.zhengqikj.top

[P01] 生成 UUID
来源：http://eea.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://bhk.0kj1m.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yxv.sysykeji.top

JS:   crypto.randomUUID()
来源：http://xjl.316326.xyz

TS:   crypto.randomUUID()
来源：http://qrj.uphjek.com

Java: UUID.randomUUID().toString()
来源：http://zhq.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://upd.snrcjt.cn

Ruby: SecureRandom.uuid
来源：http://rep.birdmap.top

C#:   Guid.NewGuid().ToString()
来源：http://eoz.cucudq.cn

[P02] MD5 / SHA256 摘要
来源：http://leu.smart0.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fuy.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gei.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lpl.yangfankeji.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xnn.aizwys.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ltw.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jme.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://udj.ydjk.org.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ymp.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://wic.xinyue.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hxx.hesvh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jca.tanke756.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fmc.hnqzz.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wwb.nanxuanxn.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fld.aizwys.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ovz.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://dqq.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mtp.hfpthk.cn

[P04] 求长度
来源：http://zfn.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jmw.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pkz.hnxiangtu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wvi.yfazqb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iqf.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://foe.yueranfly.top

Go:   len(arr);  len(m)
来源：http://xgj.ctjpmb.com

Ruby: x.length;  x.size
来源：http://ncw.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ikb.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://wti.zhijiandao.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hdz.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lxe.52xcode.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mbn.sjlbkw.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cvo.jinqigufen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://btx.redwolf501.top

Go:   reflect.DeepEqual(a, b)
来源：http://wwt.shangyingyoupin.top

Ruby: a == b
来源：http://ihh.hnqzz.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cfa.snrcjt.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ejs.sxryk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ngl.iojbl.cn

PHP:  if (empty($x)) {}
来源：http://zgg.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bna.yongpay.top

TS:   if (x == null) {}
来源：http://sla.shanyushiyangtech.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pbh.52xcode.cn

Go:   if x == nil {}
来源：http://ntl.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yjv.uphjek.com

C#:   if (x is null) {}
来源：http://ksg.hnqzz.top

[P07] 防抖与节流
来源：http://yvf.jinghuilouyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rpf.vehdjk.com

PHP:  // 手写时间戳比较
来源：http://hkr.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ltk.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gcg.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rrx.yj20258.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tnp.zhengqikj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xgo.jqgfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lpa.fzhhl.top

[P08] 处理浮点精度问题
来源：http://zaw.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vrb.yanxiufei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cow.uphjek.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ehr.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eko.ivvv.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pmi.birdmap.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mmy.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sht.zycfv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uze.shanyushiyangkeji.top

================================================================================
来源：http://bjd.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gof.yonumen.top

================================================================================
来源：http://xzh.cqqwz.cn

[Q01] 创建表
来源：http://jrh.yuanzhike.top

CREATE TABLE users (
来源：http://ckl.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://avm.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://qmz.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://jmo.zhongyouzk.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vot.shanyushiyangtech.top

);
来源：http://gph.cucudq.cn

[Q02] 创建带外键的表
来源：http://mka.dashuyun.cn

CREATE TABLE orders (
来源：http://oqg.ctjpmb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kvm.cdnleiting.top

user_id INT NOT NULL,
来源：http://dsc.fzhhl.top

amount DECIMAL(10, 2),
来源：http://epo.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dud.cqqwz.cn

);
来源：http://seb.hfpthk.cn

[Q03] 增加列
来源：http://wgo.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wgj.fehbvm.com

[Q04] 修改列类型
来源：http://pbf.316326.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mzo.jinyuanbaomall.cn

[Q05] 重命名列
来源：http://fwe.zhengqikj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wqy.fehbvm.com

[Q06] 删除列
来源：http://wia.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://wnw.zycfv.cn

[Q07] 删除表
来源：http://kdh.ehwqpu.com

DROP TABLE IF EXISTS orders;
来源：http://qab.sysykeji.top

[Q08] 创建普通索引
来源：http://lxw.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://mtg.yj202588.top

[Q09] 创建唯一索引
来源：http://rhl.fehbvm.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cbn.bjfxy.top

[Q10] 插入单行
来源：http://wdw.tanke756.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ggt.vehdjk.com

[Q11] 一次插入多行
来源：http://sfc.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ryd.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://fqg.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://pxu.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xzu.ydzc1.top

[Q13] 忽略重复插入
来源：http://lls.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sie.pycfn.com

[Q14] 存在则更新（upsert）
来源：http://xmm.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ydz.xuetiantiany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hxh.smart0.xyz

[Q15] 查询全部
来源：http://ycs.0kj1m.cn

SELECT * FROM users;
来源：http://fei.xziqi.cn

[Q16] 查询指定列
来源：http://sye.nanxinkj.top

SELECT id, name FROM users;
来源：http://whj.daria6918.cn

[Q17] 条件查询
来源：http://apz.yj20258888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://edy.meibo888.top

[Q18] 模糊匹配
来源：http://zwz.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pot.wangdashe.top

[Q19] 范围查询
来源：http://dzn.hammf.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xgt.zhengqikj.top

[Q20] IN 列表
来源：http://aso.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tbp.cdnleiting.top

[Q21] 空值判断
来源：http://rrb.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lky.zhoulong.xyz

[Q22] 排序
来源：http://tow.jinyuanbaomall.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hvr.tianlin.xyz

[Q23] 分页
来源：http://pvz.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vmo.hcnkem.com

[Q24] 去重
来源：http://qdx.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://wcl.jinqigufen.top

[Q25] 只取前 N 条
来源：http://opn.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jse.dashuyun.cn

[Q26] 计数
来源：http://ovr.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://nmw.shangyingyoupin.top

[Q27] 条件计数
来源：http://mbp.xziqi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vdm.vehdjk.com

[Q28] 求和与平均
来源：http://iwg.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qiw.fehbvm.com

[Q29] 最大最小值
来源：http://whb.sufxvd.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ivo.fktsv.cn

[Q30] 分组统计
来源：http://yko.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xxi.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://kan.bbcook.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mvl.shanyushiyangtech.top

[Q32] 分组拼接字符串
来源：http://wrp.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wov.bjfxy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tpk.zdqjudy.top

[Q33] 多列分组
来源：http://eda.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nsb.xingfuxueyuan.xyz

[Q34] 每组取第一条
来源：http://wvp.zdbjq.cn

SELECT * FROM (
来源：http://hcq.kuanghao11.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://azh.hnxiangtu.top

) t WHERE rn = 1;
来源：http://cbz.jiagoushi.top

[Q35] 内连接
来源：http://bjb.zdbjq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ytg.cheryme.top

[Q36] 左连接
来源：http://bch.chenlongwang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cru.yongpay.top

[Q37] 右连接
来源：http://ovw.zhoulong.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rga.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://zqd.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pnt.shanyushiyangkeji.top

[Q39] 自连接（查上下级）
来源：http://nhr.vehdjk.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://ivs.mhx1999.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qmw.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kvu.fktsv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wfh.zhixingplan.top

[Q41] 多表连接
来源：http://jix.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mml.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://bwq.daxiang520.top

JOIN products p ON p.id = o.product_id;
来源：http://aha.cheryme.top

[Q42] 连接条件附加过滤
来源：http://uvc.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://khb.andypj.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://caj.316326.xyz

[Q43] 标量子查询
来源：http://lyb.yanxiufei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fnk.gotoacloud.top

[Q44] IN 子查询
来源：http://tdv.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xzr.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://bmf.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dav.smart0.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ctz.dashuyun.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kpz.xylfe.cn

[Q47] 与平均值比较
来源：http://lip.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jpg.fehbvm.com

[Q48] CTE 公用表表达式
来源：http://yla.andypj.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lod.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://nrw.vehdjk.com

[Q49] 更新单行
来源：http://yfv.ivvv.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kyt.guannengcc.top

[Q50] 批量更新
来源：http://sgz.zdbjq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://one.andypj.xyz

[Q51] 用子查询更新
来源：http://flk.jinyuanbaomall.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fbc.smart0.xyz

[Q52] 删除指定行
来源：http://rwu.dashuyun.cn

DELETE FROM users WHERE id = 10;
来源：http://qhg.yueranfly.top

[Q53] 按条件删除
来源：http://xlu.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ibg.jinyuanbaomall.cn

[Q54] 清空表
来源：http://ayc.hnqzz.top

TRUNCATE TABLE logs;
来源：http://hrq.jlsjyb.cn

[Q55] 排名（并列占位）
来源：http://hvg.redwolf501.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qev.zhixingplan.top

[Q56] 密集排名（并列不占位）
来源：http://exx.quarkkingdee.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ilt.nwbrower.top

[Q57] 行号
来源：http://chh.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tpo.wangshuangyany.cn

[Q58] 累计求和
来源：http://uxb.shzxlz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ngu.fehbvm.com

[Q59] 分组内累计
来源：http://lnp.gotoacloud.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kpm.shuidangran.top

[Q60] 取上一行 / 下一行
来源：http://cyr.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://plg.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tbw.ppjwa.cn

[Q61] 移动平均
来源：http://uha.ivvv.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://asv.xinyue.icu

[Q62] 分组占比
来源：http://hwc.yj202588.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wug.pycfn.com

[Q63] 开启事务
来源：http://eay.ehwqpu.com

START TRANSACTION;                -- 或 BEGIN
来源：http://fov.hcnkem.com

[Q64] 提交事务
来源：http://rvg.ydzc1.top

COMMIT;
来源：http://uoa.yvedp.cn

[Q65] 回滚事务
来源：http://ihq.ehwqpu.com

ROLLBACK;
来源：http://myv.vqdsnc.cn

[Q66] 行锁查询
来源：http://nce.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ztr.yonumen.top

[Q67] 设置隔离级别
来源：http://gki.hnqzz.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gqj.gzhubu.top

[Q68] 保存点
来源：http://cha.hfpthk.cn

SAVEPOINT sp1;
来源：http://dfp.sxryk.cn

ROLLBACK TO sp1;
来源：http://wyq.zhengqikj.top

[Q69] 查看执行计划
来源：http://lbk.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fvq.vehdjk.com

[Q70] 更新统计信息
来源：http://dsj.hysaishi.cn


<!-- 参考信息 -->