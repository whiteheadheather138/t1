代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dhx.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wai.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gmk.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lgr.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fzg.feifeiyinyue.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://skn.shzxlz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nek.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gsy.yangfankeji.com

================================================================================
来源：http://dyf.vqdsnc.cn

O. 并发与异步
来源：http://zze.yangfankeji.com

================================================================================
来源：http://abj.zdbjq.cn

[O01] 启动一个线程
来源：http://crl.sysykeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zax.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bkm.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://crt.jlsjyb.cn

TS:   // 同 JS
来源：http://tdd.shzxlz.cn

Java: new Thread(() -> f()).start()
来源：http://rdp.52xcode.cn

Go:   go f()
来源：http://wbi.ybcxt.top

Ruby: Thread.new { f }
来源：http://wnm.gzhubu.top

C#:   Task.Run(() => F());
来源：http://zel.jiagoushi.top

[O02] 使用线程池
来源：http://bsk.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nhx.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kkk.sysykeji.top

JS:   // worker_threads 线程池
来源：http://mfw.fanxiaobao.xyz

TS:   // worker_threads 线程池
来源：http://nwc.gzhubu.top

Java: Executors.newFixedThreadPool(4)
来源：http://zlg.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wru.xylfe.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ged.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ngt.ybcxt.top

[O03] 加锁保护共享数据
来源：http://hwp.zhiwuduotai.top

Py:   with lock: shared += 1
来源：http://gan.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://ssj.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yso.vehdjk.com

TS:   // 同 JS
来源：http://ujw.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://rgi.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jes.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pve.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://uiv.hfpthk.cn

[O04] 定义异步函数并等待
来源：http://aiy.xinyue.icu

Py:   async def f():⏎    await g()
来源：http://xdt.tianlin.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hmq.yj20258.top

JS:   async function f() { await g(); }
来源：http://wsr.jyoumei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://avu.hnxiangtu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://njb.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mcd.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tmf.jqgfzy.top

C#:   async Task F() { await G(); }
来源：http://lij.jinghuilouyu.cn

[O05] 并发执行并等待全部完成
来源：http://qtx.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://zyj.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://klz.cashguo.top

JS:   await Promise.all(tasks)
来源：http://fuj.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://jbx.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vpp.316326.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mut.fengsongda.top

Ruby: threads.map(&:join)
来源：http://log.0kj1m.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lvn.yanxiufei.cn

[O06] 使用进程池
来源：http://eam.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gxp.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://wvr.sweek.top

JS:   // child_process / cluster 模块
来源：http://bcg.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://hgu.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://akw.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://poa.xuanzx.com

Ruby: // fork 块
来源：http://fyb.yuanzhike.top

C#:   Parallel.For
来源：http://zcx.zhaomingkeji.xyz

================================================================================
来源：http://svj.yuxming.cn

P. 常用工具函数
来源：http://pdm.cdnleiting.top

================================================================================
来源：http://ukt.redwolf501.top

[P01] 生成 UUID
来源：http://epn.jinghuilouyu.cn

Py:   str(uuid.uuid4())
来源：http://vew.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://usx.fktsv.cn

JS:   crypto.randomUUID()
来源：http://hzu.cqqwz.cn

TS:   crypto.randomUUID()
来源：http://cer.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://piu.sysykeji.top

Go:   // 用 github.com/google/uuid
来源：http://axn.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://qpz.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://fyv.ivvv.top

[P02] MD5 / SHA256 摘要
来源：http://cbi.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nus.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fmt.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fwl.cdnleiting.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eah.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ofd.zhongyouzk.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lvk.ehwqpu.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pss.fehbvm.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kzx.jiagoushi.top

[P03] 生成短随机字符串
来源：http://dpa.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pss.xziqi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ote.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tbb.hnxiangtu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qhk.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xkm.hysaishi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zbl.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xho.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ukp.uphjek.com

[P04] 求长度
来源：http://tyn.aibaodan.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ubx.xuetiantiany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lgk.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eer.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gfo.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://dor.xziqi.cn

Go:   len(arr);  len(m)
来源：http://nbo.shuidangran.top

Ruby: x.length;  x.size
来源：http://zcx.ybcxt.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yhj.hfpthk.cn

[P05] 判断两个对象内容是否相等
来源：http://jtl.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://api.dashuyun.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://owd.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pky.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pke.aizwys.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ycq.haohaochexian.top

Go:   reflect.DeepEqual(a, b)
来源：http://xjb.nwbrower.top

Ruby: a == b
来源：http://rsa.hcnkem.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://she.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eoq.nwbrower.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xse.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://qpa.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://esc.hcnkem.com

TS:   if (x == null) {}
来源：http://rxk.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://ccn.ehwqpu.com

Go:   if x == nil {}
来源：http://tzc.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fbx.chenzaomai.com

C#:   if (x is null) {}
来源：http://bgd.zycfv.cn

[P07] 防抖与节流
来源：http://raf.yangfankeji.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ncx.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://wzh.fanxiaobao.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://utm.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ejr.vehdjk.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tnu.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kep.shanyushiyangtech.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dld.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hmx.zhijiandao.cn

[P08] 处理浮点精度问题
来源：http://gkr.xylfe.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ans.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zcr.hywenlv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yfm.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://efv.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xkq.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://isu.pengpengdd.cyou

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qlv.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rdt.hammf.cn

================================================================================
来源：http://awl.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uoh.zhongyouzk.top

================================================================================
来源：http://weh.aizwys.cn

[Q01] 创建表
来源：http://zmg.cheryme.top

CREATE TABLE users (
来源：http://cqz.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mxh.pengpengdd.cyou

name VARCHAR(50) NOT NULL,
来源：http://oxk.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://ylx.xuetiantiany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://izq.fengsongda.top

);
来源：http://gzc.andypj.xyz

[Q02] 创建带外键的表
来源：http://lws.jiagoushi.top

CREATE TABLE orders (
来源：http://yqi.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://prj.kuanghao11.cn

user_id INT NOT NULL,
来源：http://nqr.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://aex.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tka.tianlin.xyz

);
来源：http://owp.sysykeji.top

[Q03] 增加列
来源：http://dxi.yj202588.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://akf.hongshengwenyu.top

[Q04] 修改列类型
来源：http://rqd.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dee.wangdashe.top

[Q05] 重命名列
来源：http://zzp.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kix.zhijiandao.cn

[Q06] 删除列
来源：http://kvf.shzxlz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://syx.andypj.xyz

[Q07] 删除表
来源：http://oln.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://trq.meibo888.top

[Q08] 创建普通索引
来源：http://wdj.zhaomingkeji.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://pjq.wangdashe.top

[Q09] 创建唯一索引
来源：http://vaf.pengpengdd.cyou

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rxt.fzhhl.top

[Q10] 插入单行
来源：http://rjz.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rue.ctjpmb.com

[Q11] 一次插入多行
来源：http://wdz.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://erx.tianlin.xyz

[Q12] 插入后取自增 ID
来源：http://mwa.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://cze.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uuz.gzhubu.top

[Q13] 忽略重复插入
来源：http://yth.sxryk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ali.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://uhj.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hjx.fzhhl.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tfx.ydjk.org.cn

[Q15] 查询全部
来源：http://kdp.zdqjudy.top

SELECT * FROM users;
来源：http://vbu.xinyue.icu

[Q16] 查询指定列
来源：http://adi.0kj1m.cn

SELECT id, name FROM users;
来源：http://kdl.cashguo.top

[Q17] 条件查询
来源：http://erb.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sns.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://wbt.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://syq.feifeiyinyue.top

[Q19] 范围查询
来源：http://xgx.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hds.ctjpmb.com

[Q20] IN 列表
来源：http://inj.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jee.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://cdm.yj202588.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zem.fengsongda.top

[Q22] 排序
来源：http://sie.hysaishi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rqr.birdmap.top

[Q23] 分页
来源：http://hzp.ctjpmb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ztd.jqgfzy.top

[Q24] 去重
来源：http://dbi.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://pbv.gogol.net.cn

[Q25] 只取前 N 条
来源：http://cny.daxiang520.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sre.ehwqpu.com

[Q26] 计数
来源：http://agz.hnqzz.top

SELECT COUNT(*) FROM users;
来源：http://unp.dianchejie.cn

[Q27] 条件计数
来源：http://qot.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cts.zycfv.cn

[Q28] 求和与平均
来源：http://zkv.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ljj.zycfv.cn

[Q29] 最大最小值
来源：http://ymx.shanyushiyangtech.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mro.cheryme.top

[Q30] 分组统计
来源：http://voj.c1oappe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zzg.redwolf501.top

[Q31] 分组后过滤
来源：http://kfz.svipenyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pdh.xziqi.cn

[Q32] 分组拼接字符串
来源：http://prm.fanxiaobao.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tuw.yonumen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qbu.havefunace.top

[Q33] 多列分组
来源：http://dbe.zhiwuduotai.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bzo.9152youxi.cn

[Q34] 每组取第一条
来源：http://dzq.chenlongwang.top

SELECT * FROM (
来源：http://eld.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://exs.tanke756.top

) t WHERE rn = 1;
来源：http://zqp.zdqjudy.top

[Q35] 内连接
来源：http://pky.yangfankeji.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eco.jinqigfzy.top

[Q36] 左连接
来源：http://qha.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mph.hnqzz.top

[Q37] 右连接
来源：http://gcc.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://crh.yangfankeji.com

[Q38] 全外连接（PostgreSQL）
来源：http://xca.bjfxy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ira.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://vsp.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://sbq.nanxuanxn.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uns.birdmap.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jgw.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://amh.jyoumei.cn

[Q41] 多表连接
来源：http://kfr.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://itp.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://wfz.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://biz.shanyushiyangtech.top

[Q42] 连接条件附加过滤
来源：http://wwv.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://vpk.aizwys.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jne.sysykeji.top

[Q43] 标量子查询
来源：http://ull.wangdashe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://duu.ybcxt.top

[Q44] IN 子查询
来源：http://duc.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zcu.316326.xyz

[Q45] EXISTS 判断存在
来源：http://qqr.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ddm.zhengqikj.top

[Q46] NOT EXISTS 判断不存在
来源：http://zlq.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fwz.dashuyun.cn

[Q47] 与平均值比较
来源：http://llh.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://umo.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://ogz.ywan-chungtsiang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ucw.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://ldp.yuxming.cn

[Q49] 更新单行
来源：http://cao.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baw.redwolf501.top

[Q50] 批量更新
来源：http://cda.chenlongwang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yub.hcnkem.com

[Q51] 用子查询更新
来源：http://uao.hnqzz.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yay.quarkkingdee.top

[Q52] 删除指定行
来源：http://qmc.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://xhw.zhongyouzk.top

[Q53] 按条件删除
来源：http://fsp.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hwf.feifeiyinyue.top

[Q54] 清空表
来源：http://swy.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://jat.cheryme.top

[Q55] 排名（并列占位）
来源：http://bde.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ryw.feifeiyinyue.top

[Q56] 密集排名（并列不占位）
来源：http://pfg.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://npy.chenzaomai.com

[Q57] 行号
来源：http://zqs.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://syi.smart0.xyz

[Q58] 累计求和
来源：http://ryk.gaohongyu789.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ngr.dashuyun.cn

[Q59] 分组内累计
来源：http://tei.fktsv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vuk.yuxming.cn

[Q60] 取上一行 / 下一行
来源：http://ebl.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sua.wangdashe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ptt.hnqzz.top

[Q61] 移动平均
来源：http://wdi.bbcook.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oju.yuxming.cn

[Q62] 分组占比
来源：http://aiu.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pti.zhiwuduotai.top

[Q63] 开启事务
来源：http://jas.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rox.sxryk.cn

[Q64] 提交事务
来源：http://jkv.tanke756.top

COMMIT;
来源：http://nca.dianchejie.cn

[Q65] 回滚事务
来源：http://spj.bbcook.cn

ROLLBACK;
来源：http://xaj.vehdjk.com

[Q66] 行锁查询
来源：http://ren.fanxiaobao.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ccv.epnwcf.com

[Q67] 设置隔离级别
来源：http://mql.hongshengwenyu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bux.0kj1m.cn

[Q68] 保存点
来源：http://ezv.dianchejie.cn

SAVEPOINT sp1;
来源：http://yca.chenlongwang.top


<!-- 参考信息 -->