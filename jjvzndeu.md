代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yhz.0kj1m.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://spf.ybcxt.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dgf.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qjy.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mzs.yangfankeji.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kdx.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tll.bjfxy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ndk.haohaochexian.top

================================================================================
来源：http://unl.xylfe.cn

O. 并发与异步
来源：http://nfy.c1oappe.top

================================================================================
来源：http://xfy.ctjpmb.com

[O01] 启动一个线程
来源：http://yiu.ybcxt.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://euc.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kao.shuidangran.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zxa.yvedp.cn

TS:   // 同 JS
来源：http://jkg.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://cew.9152youxi.cn

Go:   go f()
来源：http://hii.jianghu66.top

Ruby: Thread.new { f }
来源：http://uyt.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://fxj.vqdsnc.cn

[O02] 使用线程池
来源：http://cnj.c1oappe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hoi.zycfv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vzk.cucudq.cn

JS:   // worker_threads 线程池
来源：http://rfu.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://qph.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://sap.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://arp.yuanzhike.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oha.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gev.sufxvd.cn

[O03] 加锁保护共享数据
来源：http://rio.tarul.cn

Py:   with lock: shared += 1
来源：http://uoj.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://ezv.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vlc.zhongyouzk.top

TS:   // 同 JS
来源：http://aha.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://sct.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lyk.chenzaomai.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://rqo.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://nfa.shzxlz.cn

[O04] 定义异步函数并等待
来源：http://aiu.sufxvd.cn

Py:   async def f():⏎    await g()
来源：http://ekz.haohaochexian.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tbx.zhijiandao.cn

JS:   async function f() { await g(); }
来源：http://yra.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pve.0kj1m.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xta.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qki.dianchejie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fgm.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://vgo.quarkkingdee.top

[O05] 并发执行并等待全部完成
来源：http://ljp.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://avk.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dxz.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://foy.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://qbz.ydzc1.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://npk.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xeo.cdnleiting.top

Ruby: threads.map(&:join)
来源：http://caf.fktsv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://stp.zhiwuduotai.top

[O06] 使用进程池
来源：http://bmj.daxiang520.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://swi.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://urc.jqgfzy.top

JS:   // child_process / cluster 模块
来源：http://zuh.ivvv.top

TS:   // child_process / cluster 模块
来源：http://crd.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://krr.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fxv.yvedp.cn

Ruby: // fork 块
来源：http://zrh.cdnleiting.top

C#:   Parallel.For
来源：http://ycu.fzhhl.top

================================================================================
来源：http://cww.quarkkingdee.top

P. 常用工具函数
来源：http://jrz.guannengcc.top

================================================================================
来源：http://wwm.yueranfly.top

[P01] 生成 UUID
来源：http://xma.tanke756.top

Py:   str(uuid.uuid4())
来源：http://hwh.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ecg.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://gvo.meibo888.top

TS:   crypto.randomUUID()
来源：http://joj.ppjwa.cn

Java: UUID.randomUUID().toString()
来源：http://wiu.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://hzi.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://yeo.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://yfd.zdbjq.cn

[P02] MD5 / SHA256 摘要
来源：http://ylh.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tmb.daria6918.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zjz.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dpa.smart0.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ujo.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ozm.cdnleiting.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yyn.zycfv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tpn.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bgz.cqqwz.cn

[P03] 生成短随机字符串
来源：http://mgi.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iov.jqgfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xrb.tian-w.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eyf.jqgufenzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://orn.jiagoushi.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://olr.bbcook.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ono.zhaomingkeji.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ogl.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uvk.chenzaomai.com

[P04] 求长度
来源：http://ynl.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nnm.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iui.hfpthk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tmb.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sar.hysaishi.cn

Java: list.size();  map.size();  s.length()
来源：http://zcc.chenlongwang.top

Go:   len(arr);  len(m)
来源：http://vuw.jiagoushi.top

Ruby: x.length;  x.size
来源：http://jcl.daria6918.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://obr.hnxiangtu.top

[P05] 判断两个对象内容是否相等
来源：http://lpz.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://leo.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lwg.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hmi.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ung.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dvw.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gqp.bbcook.cn

Ruby: a == b
来源：http://jjv.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uiw.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kjj.pengpengdd.cyou

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ejn.dashuyun.cn

PHP:  if (empty($x)) {}
来源：http://gqa.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cvo.ctjpmb.com

TS:   if (x == null) {}
来源：http://twa.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gba.shuidangran.top

Go:   if x == nil {}
来源：http://wnk.jinyuanbaomall.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ahx.svipenyu.cn

C#:   if (x is null) {}
来源：http://oeq.snrcjt.cn

[P07] 防抖与节流
来源：http://gbl.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://igc.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://mjd.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zps.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hcz.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://svd.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sve.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vmd.fehbvm.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yim.redwolf501.top

[P08] 处理浮点精度问题
来源：http://wml.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://urg.yuanzhike.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cei.sufxvd.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xyf.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://akm.jqgfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uws.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bqw.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xdc.epnwcf.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://voo.yanxiufei.cn

================================================================================
来源：http://zxk.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mio.shuidangran.top

================================================================================
来源：http://fds.zhongyouzk.top

[Q01] 创建表
来源：http://but.xinyue.icu

CREATE TABLE users (
来源：http://osr.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vyz.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://cxs.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://ica.cheryme.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ibh.xylfe.cn

);
来源：http://kgt.0kj1m.cn

[Q02] 创建带外键的表
来源：http://log.tanke756.top

CREATE TABLE orders (
来源：http://jhl.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qvw.ybcxt.top

user_id INT NOT NULL,
来源：http://dyc.0kj1m.cn

amount DECIMAL(10, 2),
来源：http://erz.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hgw.zhaomingkeji.xyz

);
来源：http://bsb.gzhubu.top

[Q03] 增加列
来源：http://qwc.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nha.zhengqikj.top

[Q04] 修改列类型
来源：http://pox.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://scn.wangshuangyany.cn

[Q05] 重命名列
来源：http://dwl.zdqjudy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mva.zhoulong.xyz

[Q06] 删除列
来源：http://hcm.cheryme.top

ALTER TABLE users DROP COLUMN age;
来源：http://hdy.yj20258888.top

[Q07] 删除表
来源：http://vie.gogol.net.cn

DROP TABLE IF EXISTS orders;
来源：http://iex.gzhubu.top

[Q08] 创建普通索引
来源：http://gwv.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hvn.zhengqikj.top

[Q09] 创建唯一索引
来源：http://sge.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wjf.yfazqb.com

[Q10] 插入单行
来源：http://dqr.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://onq.uphjek.com

[Q11] 一次插入多行
来源：http://xmx.tanke756.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eje.wangdashe.top

[Q12] 插入后取自增 ID
来源：http://rfo.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://dcs.iojbl.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wxp.shanyushiyangkeji.top

[Q13] 忽略重复插入
来源：http://bgn.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://two.jianghu66.top

[Q14] 存在则更新（upsert）
来源：http://arc.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kht.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aqb.9152youxi.cn

[Q15] 查询全部
来源：http://fvi.guannengcc.top

SELECT * FROM users;
来源：http://yph.tianlin.xyz

[Q16] 查询指定列
来源：http://boh.redwolf501.top

SELECT id, name FROM users;
来源：http://mrz.cheryme.top

[Q17] 条件查询
来源：http://ugi.gzhubu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ckv.cashguo.top

[Q18] 模糊匹配
来源：http://jhi.sysykeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://enk.hongshengwenyu.top

[Q19] 范围查询
来源：http://xgi.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yed.jlsjyb.cn

[Q20] IN 列表
来源：http://ndp.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ctc.vehdjk.com

[Q21] 空值判断
来源：http://fau.yj202588.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zhu.xingfuxueyuan.xyz

[Q22] 排序
来源：http://bht.wangshuangyany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ghk.yuanzhike.top

[Q23] 分页
来源：http://tnl.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nwe.jqgfzy.top

[Q24] 去重
来源：http://jww.meibo888.top

SELECT DISTINCT city FROM users;
来源：http://jac.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://gzl.dashuyun.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zzr.nanxinkj.top

[Q26] 计数
来源：http://uqk.xziqi.cn

SELECT COUNT(*) FROM users;
来源：http://tox.pycfn.com

[Q27] 条件计数
来源：http://inh.tanke756.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kxu.ydjk.org.cn

[Q28] 求和与平均
来源：http://ofv.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://laz.tianlin.xyz

[Q29] 最大最小值
来源：http://lra.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rsg.zhoulong.xyz

[Q30] 分组统计
来源：http://foj.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hzf.hnqzz.top

[Q31] 分组后过滤
来源：http://ixj.xinyue.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hbz.smart0.xyz

[Q32] 分组拼接字符串
来源：http://dqd.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zrf.zycfv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vnn.mhx1999.top

[Q33] 多列分组
来源：http://lqw.yvedp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jbe.aizwys.cn

[Q34] 每组取第一条
来源：http://fsw.nanxuanxn.top

SELECT * FROM (
来源：http://waa.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bfw.chenlongwang.top

) t WHERE rn = 1;
来源：http://kgw.shuidangran.top

[Q35] 内连接
来源：http://bzm.vehdjk.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hzd.sjlbkw.cn

[Q36] 左连接
来源：http://jvk.wangshuangyany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://abz.daxiang520.top

[Q37] 右连接
来源：http://kri.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qub.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://ete.vehdjk.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://swe.guannengcc.top

[Q39] 自连接（查上下级）
来源：http://med.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xof.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mfm.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wet.jinghuilouyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yhd.sxryk.cn

[Q41] 多表连接
来源：http://pcx.iojbl.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lzg.yj202588.top

JOIN users u ON u.id = o.user_id
来源：http://aoc.pengpengdd.cyou

JOIN products p ON p.id = o.product_id;
来源：http://iwu.yj20258888.top

[Q42] 连接条件附加过滤
来源：http://nbo.yongpay.top

SELECT u.name, o.amount FROM users u
来源：http://qwv.jinqigfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eui.kuanghao11.cn

[Q43] 标量子查询
来源：http://vcf.tanke756.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hxr.hammf.cn

[Q44] IN 子查询
来源：http://bkm.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vbc.nwbrower.top

[Q45] EXISTS 判断存在
来源：http://ttr.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eva.uphjek.com

[Q46] NOT EXISTS 判断不存在
来源：http://jiz.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vap.xylfe.cn

[Q47] 与平均值比较
来源：http://ehl.ctjpmb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://evd.yj202588.top

[Q48] CTE 公用表表达式
来源：http://ixy.yuanzhike.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fgi.tanke756.top

SELECT * FROM t WHERE c > 5;
来源：http://yiw.jiagoushi.top

[Q49] 更新单行
来源：http://crs.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://spi.daria6918.cn

[Q50] 批量更新
来源：http://xiy.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://byn.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://rkn.ydzc1.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lrh.chenlongwang.top

[Q52] 删除指定行
来源：http://bpb.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://vxa.dianchejie.cn

[Q53] 按条件删除
来源：http://grk.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mbw.gotoacloud.top

[Q54] 清空表
来源：http://jqv.ppjwa.cn

TRUNCATE TABLE logs;
来源：http://drl.sjlbkw.cn

[Q55] 排名（并列占位）
来源：http://xeh.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fea.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://tns.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yyk.yj202588.top

[Q57] 行号
来源：http://ubb.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hqb.9152youxi.cn

[Q58] 累计求和
来源：http://ydf.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://srr.yueranfly.top

[Q59] 分组内累计
来源：http://kqj.yuxming.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vde.zdbjq.cn

[Q60] 取上一行 / 下一行
来源：http://flm.hnxiangtu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://szy.mhx1999.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ogt.sysykeji.top

[Q61] 移动平均
来源：http://jbs.jianghu66.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cat.xylfe.cn

[Q62] 分组占比
来源：http://ptf.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yff.sweek.top

[Q63] 开启事务
来源：http://oen.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qpa.sweek.top

[Q64] 提交事务
来源：http://gqv.sxryk.cn

COMMIT;
来源：http://ajl.cucudq.cn

[Q65] 回滚事务
来源：http://uaa.jiagoushi.top

ROLLBACK;
来源：http://qsu.hnxiangtu.top

[Q66] 行锁查询
来源：http://wmb.xziqi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://awh.ehwqpu.com

[Q67] 设置隔离级别
来源：http://tzb.ivvv.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rez.cucudq.cn

[Q68] 保存点
来源：http://fru.ydzc1.top

SAVEPOINT sp1;
来源：http://zxo.ywan-chungtsiang.top


<!-- 参考信息 -->