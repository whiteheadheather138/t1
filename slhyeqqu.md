代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ocj.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ptw.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://llb.bbcook.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rri.xingfuxueyuan.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ujh.aibaodan.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uzh.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pnu.xylfe.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wab.zhaomingkeji.xyz

================================================================================
来源：http://tot.tarul.cn

O. 并发与异步
来源：http://man.birdmap.top

================================================================================
来源：http://qhi.nanxinkj.top

[O01] 启动一个线程
来源：http://vnp.shanyushiyangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rla.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xkm.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://irm.jianghu66.top

TS:   // 同 JS
来源：http://jvm.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://dja.tanke756.top

Go:   go f()
来源：http://afo.iojbl.cn

Ruby: Thread.new { f }
来源：http://nxh.gotoacloud.top

C#:   Task.Run(() => F());
来源：http://moy.gaohongyu789.top

[O02] 使用线程池
来源：http://hau.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hqb.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kvi.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://cjj.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://xbl.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vlp.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cwx.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oln.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://erz.yfazqb.com

[O03] 加锁保护共享数据
来源：http://lyc.havefunace.top

Py:   with lock: shared += 1
来源：http://zlt.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://brd.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dud.gogol.net.cn

TS:   // 同 JS
来源：http://kmp.shanyushiyangtech.top

Java: synchronized (this) { shared++; }
来源：http://ymf.svipenyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wya.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://juy.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://whj.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://wqr.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://del.xylfe.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vas.vehdjk.com

JS:   async function f() { await g(); }
来源：http://dem.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jpv.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://okk.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ual.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://jjj.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://tbt.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://xdf.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://zoz.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nip.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://yet.shanyushiyangkeji.top

TS:   await Promise.all(tasks)
来源：http://jxg.hnqzz.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gry.zdqjudy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wum.yj202588.top

Ruby: threads.map(&:join)
来源：http://emk.yj20258888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ovz.cucudq.cn

[O06] 使用进程池
来源：http://vbb.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qxp.iojbl.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uuo.sufxvd.cn

JS:   // child_process / cluster 模块
来源：http://guy.jinyuanbaomall.cn

TS:   // child_process / cluster 模块
来源：http://mdi.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://umy.tanke756.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ouw.epnwcf.com

Ruby: // fork 块
来源：http://hfc.52xcode.cn

C#:   Parallel.For
来源：http://ual.zdbjq.cn

================================================================================
来源：http://mjq.xuetiantiany.cn

P. 常用工具函数
来源：http://phr.bbcook.cn

================================================================================
来源：http://bjd.fehbvm.com

[P01] 生成 UUID
来源：http://wdb.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://msn.guowangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yua.sweek.top

JS:   crypto.randomUUID()
来源：http://rbo.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://jcj.cheryme.top

Java: UUID.randomUUID().toString()
来源：http://yaf.pengpengdd.cyou

Go:   // 用 github.com/google/uuid
来源：http://mal.shangyingyoupin.top

Ruby: SecureRandom.uuid
来源：http://dcv.pengpengdd.cyou

C#:   Guid.NewGuid().ToString()
来源：http://epe.zycfv.cn

[P02] MD5 / SHA256 摘要
来源：http://ipt.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fpr.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://zrv.gotoacloud.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nsc.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tqb.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cqn.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ioi.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cvq.xinyue.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fkt.yfazqb.com

[P03] 生成短随机字符串
来源：http://yvv.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nhb.vehdjk.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pom.jinqigufen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://upw.aizwys.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rxk.ybcxt.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qzn.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ptm.ydjk.org.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://aqv.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kdz.hcnkem.com

[P04] 求长度
来源：http://avh.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bld.cucudq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hna.feifeiyinyue.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wwv.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jpr.vqdsnc.cn

Java: list.size();  map.size();  s.length()
来源：http://jnu.shanyushiyangkeji.top

Go:   len(arr);  len(m)
来源：http://nms.aibaodan.cn

Ruby: x.length;  x.size
来源：http://kmz.yanxiufei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pqh.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://ryh.zdqjudy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wsh.hysaishi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vgn.yuxming.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yuf.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xih.xinyue.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tkq.jqgufenzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://qta.ywan-chungtsiang.top

Ruby: a == b
来源：http://gph.cqqwz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gyf.ivvv.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lfr.yuanzhike.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gtz.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://zwu.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rte.mhx1999.top

TS:   if (x == null) {}
来源：http://ekq.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://udm.ctjpmb.com

Go:   if x == nil {}
来源：http://ecu.jinghuilouyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cth.cdnleiting.top

C#:   if (x is null) {}
来源：http://uii.guannengcc.top

[P07] 防抖与节流
来源：http://heg.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://skf.havefunace.top

PHP:  // 手写时间戳比较
来源：http://zzq.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mob.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kii.yj20258.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://acc.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lyr.sweek.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mzk.dashuyun.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tce.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://kmj.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kvp.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vsq.0kj1m.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yii.pengpengdd.cyou

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qda.cucudq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bvm.redwolf501.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yfm.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zmb.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rum.shangyingyoupin.top

================================================================================
来源：http://smi.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cuk.zhaomingkeji.xyz

================================================================================
来源：http://atf.jqgufenzy.top

[Q01] 创建表
来源：http://fgk.guowangkeji.top

CREATE TABLE users (
来源：http://nvv.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lvh.zhaomingkeji.xyz

name VARCHAR(50) NOT NULL,
来源：http://hmv.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://qmm.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xbh.chenlongwang.top

);
来源：http://tpq.haohaochexian.top

[Q02] 创建带外键的表
来源：http://vid.fengsongda.top

CREATE TABLE orders (
来源：http://xfg.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xpo.gogol.net.cn

user_id INT NOT NULL,
来源：http://bey.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://lft.shangyingyoupin.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jni.ywan-chungtsiang.top

);
来源：http://zyc.snrcjt.cn

[Q03] 增加列
来源：http://grv.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://syl.fehbvm.com

[Q04] 修改列类型
来源：http://jul.wangshuangyany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vzx.wangdashe.top

[Q05] 重命名列
来源：http://lpq.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://txa.yanxiufei.cn

[Q06] 删除列
来源：http://bha.fengsongda.top

ALTER TABLE users DROP COLUMN age;
来源：http://lln.aizwys.cn

[Q07] 删除表
来源：http://lma.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://phh.ppjwa.cn

[Q08] 创建普通索引
来源：http://rnk.shanyushiyangtech.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hvz.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://jup.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://smy.gzhubu.top

[Q10] 插入单行
来源：http://npm.havefunace.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zju.chenjidiqi.icu

[Q11] 一次插入多行
来源：http://ihx.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kub.316326.xyz

[Q12] 插入后取自增 ID
来源：http://rsf.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xko.fengsongda.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hps.pycfn.com

[Q13] 忽略重复插入
来源：http://gjb.zhaomingkeji.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ial.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://gug.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zri.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gxb.yj20258.top

[Q15] 查询全部
来源：http://zqa.cucudq.cn

SELECT * FROM users;
来源：http://jwz.birdmap.top

[Q16] 查询指定列
来源：http://mcp.sufxvd.cn

SELECT id, name FROM users;
来源：http://sau.zycfv.cn

[Q17] 条件查询
来源：http://iny.zhaomingkeji.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://epm.wangshuangyany.cn

[Q18] 模糊匹配
来源：http://hyb.pengpengdd.cyou

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tnw.hfpthk.cn

[Q19] 范围查询
来源：http://bji.iojbl.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://svl.fzhhl.top

[Q20] IN 列表
来源：http://iim.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sec.redwolf501.top

[Q21] 空值判断
来源：http://zbm.ivvv.top

SELECT * FROM users WHERE email IS NULL;
来源：http://juk.yuanzhike.top

[Q22] 排序
来源：http://hlg.yuanzhike.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cef.hnqzz.top

[Q23] 分页
来源：http://tuj.cqqwz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zzq.cheryme.top

[Q24] 去重
来源：http://hdb.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://mpt.cqqwz.cn

[Q25] 只取前 N 条
来源：http://ven.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hdv.jinqigfzy.top

[Q26] 计数
来源：http://puh.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://qfl.wangshuangyany.cn

[Q27] 条件计数
来源：http://los.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://grq.hfpthk.cn

[Q28] 求和与平均
来源：http://kyh.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tmd.gotoacloud.top

[Q29] 最大最小值
来源：http://rpt.ydzc1.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://onx.fengsongda.top

[Q30] 分组统计
来源：http://aem.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nyl.wangdashe.top

[Q31] 分组后过滤
来源：http://phm.cashguo.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://trw.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://vhk.cheryme.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://csl.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hme.fktsv.cn

[Q33] 多列分组
来源：http://lrg.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xct.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://fot.xziqi.cn

SELECT * FROM (
来源：http://avh.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yvd.gogol.net.cn

) t WHERE rn = 1;
来源：http://jir.redwolf501.top

[Q35] 内连接
来源：http://ruy.yangfankeji.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xaz.xinyue.icu

[Q36] 左连接
来源：http://bes.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zgd.havefunace.top

[Q37] 右连接
来源：http://nrp.sjlbkw.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jtb.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://cvb.yj20258888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://inn.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://rlz.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://hac.cqqwz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rso.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aha.yonumen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://moa.hnqzz.top

[Q41] 多表连接
来源：http://phk.jqgfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lub.jiagoushi.top

JOIN users u ON u.id = o.user_id
来源：http://kjd.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://rij.yanxiufei.cn

[Q42] 连接条件附加过滤
来源：http://bmo.sysykeji.top

SELECT u.name, o.amount FROM users u
来源：http://txg.yuxming.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lvf.sweek.top

[Q43] 标量子查询
来源：http://xwc.gotoacloud.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wnw.nanxuanxn.top

[Q44] IN 子查询
来源：http://zlh.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dla.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://fzt.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ehp.yueranfly.top

[Q46] NOT EXISTS 判断不存在
来源：http://wzv.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ytw.zhengqikj.top

[Q47] 与平均值比较
来源：http://por.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uil.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://obi.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nzu.dashuyun.cn

SELECT * FROM t WHERE c > 5;
来源：http://gjl.nanxuanxn.top

[Q49] 更新单行
来源：http://ybv.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oub.jianghu66.top

[Q50] 批量更新
来源：http://ziq.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xnz.hesvh.cn

[Q51] 用子查询更新
来源：http://ajo.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xgl.jianghu66.top

[Q52] 删除指定行
来源：http://xzg.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://orz.hesvh.cn

[Q53] 按条件删除
来源：http://fjb.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dym.redwolf501.top

[Q54] 清空表
来源：http://ynb.uphjek.com

TRUNCATE TABLE logs;
来源：http://jfx.dianchejie.cn

[Q55] 排名（并列占位）
来源：http://amb.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dvs.zhaomingkeji.xyz

[Q56] 密集排名（并列不占位）
来源：http://hkd.pengpengdd.cyou

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bnk.shuidangran.top

[Q57] 行号
来源：http://iko.ctjpmb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hpk.iojbl.cn

[Q58] 累计求和
来源：http://ieg.gotoacloud.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xwe.yuanzhike.top

[Q59] 分组内累计
来源：http://kgo.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ehn.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://zsj.iojbl.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jxw.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lyk.hesvh.cn

[Q61] 移动平均
来源：http://lfj.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pvb.zdbjq.cn

[Q62] 分组占比
来源：http://hwr.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vnt.9152youxi.cn

[Q63] 开启事务
来源：http://qne.uphjek.com

START TRANSACTION;                -- 或 BEGIN
来源：http://ydb.vqdsnc.cn

[Q64] 提交事务
来源：http://swf.dashuyun.cn

COMMIT;
来源：http://tca.cashguo.top

[Q65] 回滚事务
来源：http://juv.iojbl.cn

ROLLBACK;
来源：http://tby.wangdashe.top

[Q66] 行锁查询
来源：http://uaj.xziqi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lfb.xinyue.icu

[Q67] 设置隔离级别
来源：http://maq.chenlongwang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ejm.sufxvd.cn

[Q68] 保存点
来源：http://rpi.sysykeji.top

SAVEPOINT sp1;
来源：http://msc.zhongyouzk.top


<!-- 参考信息 -->