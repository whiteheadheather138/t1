代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pnw.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hiu.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jtu.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xcm.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tkq.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wqw.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cnv.zycfv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vwn.vqdsnc.cn

================================================================================
来源：http://nor.yj20258.top

O. 并发与异步
来源：http://pwd.aizwys.cn

================================================================================
来源：http://yfj.fktsv.cn

[O01] 启动一个线程
来源：http://oyy.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ajs.zhixingplan.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qly.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vho.mhx1999.top

TS:   // 同 JS
来源：http://usw.zhongyouzk.top

Java: new Thread(() -> f()).start()
来源：http://rle.vqdsnc.cn

Go:   go f()
来源：http://pcx.shzxlz.cn

Ruby: Thread.new { f }
来源：http://fhm.fktsv.cn

C#:   Task.Run(() => F());
来源：http://bza.jqgfzy.top

[O02] 使用线程池
来源：http://ysx.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hhk.snrcjt.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://shg.yangfankeji.com

JS:   // worker_threads 线程池
来源：http://idz.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://ldv.gogol.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uts.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jiv.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qmv.hysaishi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zdj.yongpay.top

[O03] 加锁保护共享数据
来源：http://oqd.yuxming.cn

Py:   with lock: shared += 1
来源：http://otg.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://kzr.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tou.52xcode.cn

TS:   // 同 JS
来源：http://olk.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://roc.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ugc.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sdf.ybcxt.top

C#:   lock (gate) { shared++; }
来源：http://qhe.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://ubu.wangshuangyany.cn

Py:   async def f():⏎    await g()
来源：http://yvy.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kfd.sxryk.cn

JS:   async function f() { await g(); }
来源：http://ysk.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dft.bjfxy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jll.yanxiufei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tru.fehbvm.com

Ruby: # 用 Fiber 或 async gem
来源：http://oid.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://bvw.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://nph.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://suv.feifeiyinyue.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rmq.hesvh.cn

JS:   await Promise.all(tasks)
来源：http://jdh.fktsv.cn

TS:   await Promise.all(tasks)
来源：http://oww.epnwcf.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xrx.0kj1m.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bxh.bjfxy.top

Ruby: threads.map(&:join)
来源：http://dov.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://vyf.52xcode.cn

[O06] 使用进程池
来源：http://wyb.hesvh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uka.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://byl.wangdashe.top

JS:   // child_process / cluster 模块
来源：http://zcf.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://qja.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://acj.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cki.ehwqpu.com

Ruby: // fork 块
来源：http://dbv.9152youxi.cn

C#:   Parallel.For
来源：http://rqb.52xcode.cn

================================================================================
来源：http://sld.jinyuanbaomall.cn

P. 常用工具函数
来源：http://utj.chenzaomai.com

================================================================================
来源：http://pdn.cdnleiting.top

[P01] 生成 UUID
来源：http://dwd.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://xrw.yuanzhike.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jij.hnqzz.top

JS:   crypto.randomUUID()
来源：http://nfg.hcnkem.com

TS:   crypto.randomUUID()
来源：http://rfv.fanxiaobao.xyz

Java: UUID.randomUUID().toString()
来源：http://wbx.cashguo.top

Go:   // 用 github.com/google/uuid
来源：http://mqq.jinghuilouyu.cn

Ruby: SecureRandom.uuid
来源：http://qxi.ppjwa.cn

C#:   Guid.NewGuid().ToString()
来源：http://nya.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://zjg.svipenyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nft.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tjf.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rsm.jqgufenzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rts.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jzm.sufxvd.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cjc.ydzc1.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://umf.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cbw.wangdashe.top

[P03] 生成短随机字符串
来源：http://izr.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ktw.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fea.ydzc1.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yds.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ehc.snrcjt.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kpa.xuanzx.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mwb.meibo888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gze.ydjk.org.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dji.dashuyun.cn

[P04] 求长度
来源：http://pkc.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pmc.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qhh.hnqzz.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://alb.9152youxi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ikp.chenjidiqi.icu

Java: list.size();  map.size();  s.length()
来源：http://mbg.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://tiv.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://zzv.sufxvd.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cwr.hnxiangtu.top

[P05] 判断两个对象内容是否相等
来源：http://war.jinghuilouyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://axk.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rqz.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iwe.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dij.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kqg.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://inr.zhongyouzk.top

Ruby: a == b
来源：http://puv.shanyushiyangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hdb.shzxlz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nof.jqgfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iev.xuanzx.com

PHP:  if (empty($x)) {}
来源：http://rch.shuidangran.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qog.iojbl.cn

TS:   if (x == null) {}
来源：http://bpt.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zpd.birdmap.top

Go:   if x == nil {}
来源：http://itz.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yyi.jinghuilouyu.cn

C#:   if (x is null) {}
来源：http://gkt.aizwys.cn

[P07] 防抖与节流
来源：http://wvb.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wav.svipenyu.cn

PHP:  // 手写时间戳比较
来源：http://fdu.wangdashe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://omx.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ohu.bbcook.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qag.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ymv.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hoo.xinyue.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lpe.gzhubu.top

[P08] 处理浮点精度问题
来源：http://vwp.zdbjq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mrr.cashguo.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tyk.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://byw.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://swb.9152youxi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gil.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vpm.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mnd.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xfu.quarkkingdee.top

================================================================================
来源：http://uut.cqqwz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dak.zdqjudy.top

================================================================================
来源：http://cbo.shzxlz.cn

[Q01] 创建表
来源：http://yqb.fktsv.cn

CREATE TABLE users (
来源：http://mvz.aizwys.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://puf.ppjwa.cn

name VARCHAR(50) NOT NULL,
来源：http://dgh.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://wdo.aizwys.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yuj.daria6918.cn

);
来源：http://nwa.ehwqpu.com

[Q02] 创建带外键的表
来源：http://hep.gogol.net.cn

CREATE TABLE orders (
来源：http://uur.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://msm.cqqwz.cn

user_id INT NOT NULL,
来源：http://cqr.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://ywl.yonumen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eur.daria6918.cn

);
来源：http://ths.xziqi.cn

[Q03] 增加列
来源：http://jzp.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qur.yongpay.top

[Q04] 修改列类型
来源：http://gcm.sysykeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zyp.yongpay.top

[Q05] 重命名列
来源：http://smp.gaohongyu789.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ewt.shanyushiyangtech.top

[Q06] 删除列
来源：http://gwi.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://yvf.ppjwa.cn

[Q07] 删除表
来源：http://yhn.smart0.xyz

DROP TABLE IF EXISTS orders;
来源：http://xig.snrcjt.cn

[Q08] 创建普通索引
来源：http://vbq.yuanzhike.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ntx.nanxuanxn.top

[Q09] 创建唯一索引
来源：http://hdm.smart0.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ghs.guannengcc.top

[Q10] 插入单行
来源：http://vqk.chenzaomai.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://txu.kuanghao11.cn

[Q11] 一次插入多行
来源：http://akl.yj20258888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qqb.vqdsnc.cn

[Q12] 插入后取自增 ID
来源：http://zgn.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://qmp.0kj1m.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qnp.zdqjudy.top

[Q13] 忽略重复插入
来源：http://pln.pengpengdd.cyou

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cfj.yongpay.top

[Q14] 存在则更新（upsert）
来源：http://lrt.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gef.zhaomingkeji.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hmm.wangshuangyany.cn

[Q15] 查询全部
来源：http://jmb.jqgufenzy.top

SELECT * FROM users;
来源：http://bzu.dashuyun.cn

[Q16] 查询指定列
来源：http://rde.tarul.cn

SELECT id, name FROM users;
来源：http://mtd.wangshuangyany.cn

[Q17] 条件查询
来源：http://sea.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fog.316326.xyz

[Q18] 模糊匹配
来源：http://qke.yuanzhike.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kdz.chenzaomai.com

[Q19] 范围查询
来源：http://bfi.gzhubu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ezn.fengsongda.top

[Q20] IN 列表
来源：http://otz.shuidangran.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ody.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://cah.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nbq.ctjpmb.com

[Q22] 排序
来源：http://flu.jinghuilouyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://otv.wangshuangyany.cn

[Q23] 分页
来源：http://psx.yangfankeji.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ios.bbcook.cn

[Q24] 去重
来源：http://ktg.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://rla.nwbrower.top

[Q25] 只取前 N 条
来源：http://zbg.hysaishi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vrm.chenzaomai.com

[Q26] 计数
来源：http://riq.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://pwc.fanxiaobao.xyz

[Q27] 条件计数
来源：http://gjw.kuanghao11.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://djd.zhongyouzk.top

[Q28] 求和与平均
来源：http://gov.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hcu.316326.xyz

[Q29] 最大最小值
来源：http://gfi.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://bln.havefunace.top

[Q30] 分组统计
来源：http://vfb.hnqzz.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tkt.chenlongwang.top

[Q31] 分组后过滤
来源：http://uvb.zhongyouzk.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fwb.tian-w.cn

[Q32] 分组拼接字符串
来源：http://bik.ywan-chungtsiang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oki.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wfk.vehdjk.com

[Q33] 多列分组
来源：http://drs.shuidangran.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pqo.snrcjt.cn

[Q34] 每组取第一条
来源：http://wgz.cashguo.top

SELECT * FROM (
来源：http://yxl.jinghuilouyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rsk.wangdashe.top

) t WHERE rn = 1;
来源：http://uuc.shuidangran.top

[Q35] 内连接
来源：http://tsy.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://duj.fktsv.cn

[Q36] 左连接
来源：http://nrl.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yoz.yueranfly.top

[Q37] 右连接
来源：http://knm.jianghu66.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://est.yongpay.top

[Q38] 全外连接（PostgreSQL）
来源：http://xql.birdmap.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ldt.wangshuangyany.cn

[Q39] 自连接（查上下级）
来源：http://aik.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zmo.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://koh.wangdashe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tbz.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wqe.jianghu66.top

[Q41] 多表连接
来源：http://xva.sjlbkw.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rep.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://thf.xinyue.icu

JOIN products p ON p.id = o.product_id;
来源：http://nwb.gzhubu.top

[Q42] 连接条件附加过滤
来源：http://xfe.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://url.sweek.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hbf.jinyuanbaomall.cn

[Q43] 标量子查询
来源：http://sfm.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qvp.xinyue.icu

[Q44] IN 子查询
来源：http://iuh.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xrv.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://uiw.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aox.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://idl.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gdd.sxryk.cn

[Q47] 与平均值比较
来源：http://hnd.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yzs.jinghuilouyu.cn

[Q48] CTE 公用表表达式
来源：http://ozq.xuetiantiany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zfd.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://tis.jinqigufen.top

[Q49] 更新单行
来源：http://lnt.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zbl.shzxlz.cn

[Q50] 批量更新
来源：http://cnj.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qmg.zdqjudy.top

[Q51] 用子查询更新
来源：http://hqu.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gtk.fktsv.cn

[Q52] 删除指定行
来源：http://zkc.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://bzf.zhongyouzk.top

[Q53] 按条件删除
来源：http://jnf.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://klp.havefunace.top

[Q54] 清空表
来源：http://iyi.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://rna.zhaomingkeji.xyz

[Q55] 排名（并列占位）
来源：http://phy.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fsu.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://gxz.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ypm.tarul.cn

[Q57] 行号
来源：http://mxb.jqgufenzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mzt.zdbjq.cn

[Q58] 累计求和
来源：http://xbj.zhijiandao.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://odc.guowangkeji.top

[Q59] 分组内累计
来源：http://jmr.zhoulong.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qur.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://ozh.sweek.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hez.wangdashe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wzz.zdqjudy.top

[Q61] 移动平均
来源：http://xue.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pxx.zycfv.cn

[Q62] 分组占比
来源：http://kvh.ehwqpu.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hro.sufxvd.cn

[Q63] 开启事务
来源：http://lpr.tian-w.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dzy.ppjwa.cn

[Q64] 提交事务
来源：http://hei.jinyuanbaomall.cn

COMMIT;
来源：http://gpj.gotoacloud.top

[Q65] 回滚事务
来源：http://hsl.fehbvm.com

ROLLBACK;
来源：http://rwd.cucudq.cn

[Q66] 行锁查询
来源：http://xuz.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pbp.ivvv.top

[Q67] 设置隔离级别
来源：http://klw.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://szn.zhiwuduotai.top

[Q68] 保存点
来源：http://fcv.fengsongda.top

SAVEPOINT sp1;
来源：http://qgl.yongpay.top


<!-- 参考信息 -->