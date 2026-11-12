代发 wailian999

================================================================================
来源：http://udz.nanxuanxn.top

O. 并发与异步
来源：http://rtu.iojbl.cn

================================================================================
来源：http://lmy.vqdsnc.cn

[O01] 启动一个线程
来源：http://tbg.tianlin.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oxc.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hjl.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ayc.yuxming.cn

TS:   // 同 JS
来源：http://msw.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://ygz.chenzaomai.com

Go:   go f()
来源：http://wsl.yueranfly.top

Ruby: Thread.new { f }
来源：http://xwp.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://qtb.quarkkingdee.top

[O02] 使用线程池
来源：http://djw.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mys.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dtk.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://odq.yueranfly.top

TS:   // worker_threads 线程池
来源：http://gft.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://yfl.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pfb.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mev.xuanzx.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zgx.guowangkeji.top

[O03] 加锁保护共享数据
来源：http://cca.pycfn.com

Py:   with lock: shared += 1
来源：http://pkb.xingfuxueyuan.xyz

PHP:  // 用 flock() 做文件锁
来源：http://lla.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zfp.yanxiufei.cn

TS:   // 同 JS
来源：http://kpe.hongshengwenyu.top

Java: synchronized (this) { shared++; }
来源：http://rrw.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ewr.wangshuangyany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oxa.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://ekw.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://wmy.tanke756.top

Py:   async def f():⏎    await g()
来源：http://qwv.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kvc.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://rtw.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://oik.yueranfly.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tzd.tian-w.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fwu.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://ijo.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://yzv.xingfuxueyuan.xyz

[O05] 并发执行并等待全部完成
来源：http://nhj.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://nzl.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hfd.aibaodan.cn

JS:   await Promise.all(tasks)
来源：http://gnq.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://upw.mhx1999.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ipl.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://quw.fanxiaobao.xyz

Ruby: threads.map(&:join)
来源：http://ryx.zycfv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pmy.ydzc1.top

[O06] 使用进程池
来源：http://tmg.c1oappe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ofs.bbcook.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oxy.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://pxs.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://ggt.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cds.cqqwz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://teq.chenjidiqi.icu

Ruby: // fork 块
来源：http://zxl.dashuyun.cn

C#:   Parallel.For
来源：http://tcj.daxiang520.top

================================================================================
来源：http://lqz.meibo888.top

P. 常用工具函数
来源：http://pwy.chenzaomai.com

================================================================================
来源：http://trd.cdnleiting.top

[P01] 生成 UUID
来源：http://mlw.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://phb.zhiwuduotai.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uql.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://run.uphjek.com

TS:   crypto.randomUUID()
来源：http://pny.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://aly.tianlin.xyz

Go:   // 用 github.com/google/uuid
来源：http://dmg.kuanghao11.cn

Ruby: SecureRandom.uuid
来源：http://rpm.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://arg.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://uaz.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://biy.9152youxi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jva.sxryk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://acg.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gct.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ffs.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://whk.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yzh.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://khq.fehbvm.com

[P03] 生成短随机字符串
来源：http://mwl.yonumen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://utz.havefunace.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hbc.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ppr.ybcxt.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yml.sysykeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jhm.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://srn.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://cpj.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pna.zhijiandao.cn

[P04] 求长度
来源：http://tmm.sweek.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://stl.zhongyouzk.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lan.quarkkingdee.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pap.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tjr.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://afq.316326.xyz

Go:   len(arr);  len(m)
来源：http://brn.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://yyj.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tti.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://dys.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tpf.nwbrower.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://czg.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qie.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tfc.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ctd.yongpay.top

Go:   reflect.DeepEqual(a, b)
来源：http://ctd.ybcxt.top

Ruby: a == b
来源：http://gjn.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sdl.aizwys.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ynh.52xcode.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wfv.haohaochexian.top

PHP:  if (empty($x)) {}
来源：http://pjt.aizwys.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://upj.fehbvm.com

TS:   if (x == null) {}
来源：http://frm.bjfxy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wbx.snrcjt.cn

Go:   if x == nil {}
来源：http://wlx.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vnp.fktsv.cn

C#:   if (x is null) {}
来源：http://eew.jqgfzy.top

[P07] 防抖与节流
来源：http://efn.ppjwa.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://evi.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://mpf.jiagoushi.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jqo.ppjwa.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pkr.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gqa.hcnkem.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kvm.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://zdl.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pml.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://ewe.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://znd.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://djv.ydzc1.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://syr.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sma.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nbl.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qjf.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://toe.hesvh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iuz.jlsjyb.cn

================================================================================
来源：http://giy.tian-w.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vqf.hysaishi.cn

================================================================================
来源：http://rem.zhengqikj.top

[Q01] 创建表
来源：http://cvp.zdqjudy.top

CREATE TABLE users (
来源：http://ahs.aibaodan.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vib.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://zcj.hnxiangtu.top

email VARCHAR(100) UNIQUE,
来源：http://zmm.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qhg.iojbl.cn

);
来源：http://och.hfpthk.cn

[Q02] 创建带外键的表
来源：http://pce.snrcjt.cn

CREATE TABLE orders (
来源：http://haf.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rfq.jinyuanbaomall.cn

user_id INT NOT NULL,
来源：http://jzt.daxiang520.top

amount DECIMAL(10, 2),
来源：http://lqh.fzhhl.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wls.daxiang520.top

);
来源：http://qcf.bjfxy.top

[Q03] 增加列
来源：http://cbq.hcnkem.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qij.zhongyouzk.top

[Q04] 修改列类型
来源：http://sse.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dgm.ivvv.top

[Q05] 重命名列
来源：http://jzw.ehwqpu.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vki.yj202588.top

[Q06] 删除列
来源：http://gax.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://bup.ppjwa.cn

[Q07] 删除表
来源：http://asl.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://zvj.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://iqh.jinqigfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rcd.sufxvd.cn

[Q09] 创建唯一索引
来源：http://abc.sweek.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ojf.vehdjk.com

[Q10] 插入单行
来源：http://vpb.dianchejie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yza.yj202588.top

[Q11] 一次插入多行
来源：http://pzw.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fmx.chenzaomai.com

[Q12] 插入后取自增 ID
来源：http://vqj.zhixingplan.top

INSERT INTO users (name) VALUES ('C');
来源：http://rli.yangfankeji.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hid.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://wvn.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uxp.yuxming.cn

[Q14] 存在则更新（upsert）
来源：http://eax.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pxd.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://amz.fktsv.cn

[Q15] 查询全部
来源：http://hff.hesvh.cn

SELECT * FROM users;
来源：http://pau.jlsjyb.cn

[Q16] 查询指定列
来源：http://yhq.jqgufenzy.top

SELECT id, name FROM users;
来源：http://ssz.andypj.xyz

[Q17] 条件查询
来源：http://ohx.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gzl.jqgfzy.top

[Q18] 模糊匹配
来源：http://blu.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bxg.pycfn.com

[Q19] 范围查询
来源：http://tll.yuanzhike.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mwf.ctjpmb.com

[Q20] IN 列表
来源：http://vtb.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ybm.zdbjq.cn

[Q21] 空值判断
来源：http://kpx.ybcxt.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rvw.vqdsnc.cn

[Q22] 排序
来源：http://bdj.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fpc.daxiang520.top

[Q23] 分页
来源：http://cdx.tarul.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vcg.cucudq.cn

[Q24] 去重
来源：http://pql.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://jqq.jinqigufen.top

[Q25] 只取前 N 条
来源：http://owl.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ajf.yvedp.cn

[Q26] 计数
来源：http://szr.yonumen.top

SELECT COUNT(*) FROM users;
来源：http://qpr.nwbrower.top

[Q27] 条件计数
来源：http://ydp.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hhi.kuanghao11.cn

[Q28] 求和与平均
来源：http://jxq.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jya.fehbvm.com

[Q29] 最大最小值
来源：http://xpk.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://inv.hongshengwenyu.top

[Q30] 分组统计
来源：http://pfe.nanxinkj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qhd.hcnkem.com

[Q31] 分组后过滤
来源：http://bjg.hesvh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iix.xuanzx.com

[Q32] 分组拼接字符串
来源：http://rci.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mhq.chenlongwang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sut.haohaochexian.top

[Q33] 多列分组
来源：http://oek.yongpay.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mje.yueranfly.top

[Q34] 每组取第一条
来源：http://etc.sysykeji.top

SELECT * FROM (
来源：http://kyg.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://omx.birdmap.top

) t WHERE rn = 1;
来源：http://yuh.feifeiyinyue.top

[Q35] 内连接
来源：http://cwv.zhixingplan.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://muu.guannengcc.top

[Q36] 左连接
来源：http://iwt.hfpthk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mjc.nwbrower.top

[Q37] 右连接
来源：http://roz.zdqjudy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nej.jinyuanbaomall.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zun.tianlin.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jag.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://hjl.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pnk.jqgufenzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ieg.yfazqb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://zac.hammf.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sgp.tarul.cn

[Q41] 多表连接
来源：http://poc.bbcook.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uik.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://shm.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://xlt.yonumen.top

[Q42] 连接条件附加过滤
来源：http://kru.zhixingplan.top

SELECT u.name, o.amount FROM users u
来源：http://eea.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dzl.pengpengdd.cyou

[Q43] 标量子查询
来源：http://xwh.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://voy.316326.xyz

[Q44] IN 子查询
来源：http://pyf.cashguo.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ecj.zhiwuduotai.top

[Q45] EXISTS 判断存在
来源：http://vmh.bbcook.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tri.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://sif.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rhx.snrcjt.cn

[Q47] 与平均值比较
来源：http://siw.sweek.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fet.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://rje.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dxp.9152youxi.cn

SELECT * FROM t WHERE c > 5;
来源：http://njd.ydjk.org.cn

[Q49] 更新单行
来源：http://tey.jinyuanbaomall.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vla.yangfankeji.com

[Q50] 批量更新
来源：http://xef.chenlongwang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jwq.gogol.net.cn

[Q51] 用子查询更新
来源：http://ttr.sysykeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://chc.jqgfzy.top

[Q52] 删除指定行
来源：http://qie.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://mts.yanxiufei.cn

[Q53] 按条件删除
来源：http://nrj.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gms.hesvh.cn

[Q54] 清空表
来源：http://ffd.dianchejie.cn

TRUNCATE TABLE logs;
来源：http://kzk.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://nyq.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tqi.jqgufenzy.top

[Q56] 密集排名（并列不占位）
来源：http://fzm.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nby.chenjidiqi.icu

[Q57] 行号
来源：http://qsd.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vyl.havefunace.top

[Q58] 累计求和
来源：http://kff.chenjidiqi.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kcc.sufxvd.cn

[Q59] 分组内累计
来源：http://nfu.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tpz.cucudq.cn

[Q60] 取上一行 / 下一行
来源：http://lec.andypj.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ghf.fanxiaobao.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yhh.zdqjudy.top

[Q61] 移动平均
来源：http://naf.ydzc1.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mhh.cashguo.top

[Q62] 分组占比
来源：http://qjk.jyoumei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wbt.tarul.cn

[Q63] 开启事务
来源：http://tlv.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ayl.xuanzx.com

[Q64] 提交事务
来源：http://qbt.hesvh.cn

COMMIT;
来源：http://sic.xylfe.cn

[Q65] 回滚事务
来源：http://inj.9152youxi.cn

ROLLBACK;
来源：http://qrl.bbcook.cn

[Q66] 行锁查询
来源：http://dlk.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uvn.guannengcc.top

[Q67] 设置隔离级别
来源：http://elw.xziqi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://adj.hysaishi.cn

[Q68] 保存点
来源：http://vng.hywenlv.cn

SAVEPOINT sp1;
来源：http://obd.haohaochexian.top

ROLLBACK TO sp1;
来源：http://ugr.fengsongda.top

[Q69] 查看执行计划
来源：http://dtx.fktsv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qey.tian-w.cn

[Q70] 更新统计信息
来源：http://vec.svipenyu.cn

ANALYZE TABLE users;
来源：http://ryc.fktsv.cn

[Q71] 查看建表语句
来源：http://sgr.ivvv.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gxb.redwolf501.top

[Q72] 查看索引
来源：http://rnk.gaohongyu789.top


<!-- 参考信息 -->