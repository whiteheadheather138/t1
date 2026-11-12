代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sar.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bbe.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tjj.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vju.sysykeji.top

================================================================================
来源：http://qdk.xuanzx.com

O. 并发与异步
来源：http://cqg.sxryk.cn

================================================================================
来源：http://qkf.mhx1999.top

[O01] 启动一个线程
来源：http://ftn.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ogz.guowangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nap.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pwj.guowangkeji.top

TS:   // 同 JS
来源：http://ipl.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://vqd.ybcxt.top

Go:   go f()
来源：http://orx.ydzc1.top

Ruby: Thread.new { f }
来源：http://fyr.iojbl.cn

C#:   Task.Run(() => F());
来源：http://dtm.9152youxi.cn

[O02] 使用线程池
来源：http://ojj.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hbl.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gvv.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://aci.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://nvd.ydzc1.top

Java: Executors.newFixedThreadPool(4)
来源：http://npo.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tcs.chenzaomai.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xjm.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fjf.xziqi.cn

[O03] 加锁保护共享数据
来源：http://zfz.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://ssq.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://feu.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://liq.sysykeji.top

TS:   // 同 JS
来源：http://hsd.tarul.cn

Java: synchronized (this) { shared++; }
来源：http://jxf.ydjk.org.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://emi.hcnkem.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://qbh.yj202588.top

C#:   lock (gate) { shared++; }
来源：http://vzq.zycfv.cn

[O04] 定义异步函数并等待
来源：http://mux.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://ygt.sjlbkw.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://psf.yongpay.top

JS:   async function f() { await g(); }
来源：http://zcg.chenjidiqi.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://dwv.xinyue.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ghv.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rbl.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wyo.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://icy.dashuyun.cn

[O05] 并发执行并等待全部完成
来源：http://jye.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://xtk.hongshengwenyu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nxd.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://etf.yongpay.top

TS:   await Promise.all(tasks)
来源：http://sfu.yvedp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kaz.fehbvm.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sdr.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://fpt.havefunace.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ifs.jlsjyb.cn

[O06] 使用进程池
来源：http://ind.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ohm.ydzc1.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dtu.andypj.xyz

JS:   // child_process / cluster 模块
来源：http://ikv.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://zqa.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tfp.yongpay.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ran.ydjk.org.cn

Ruby: // fork 块
来源：http://jdz.dashuyun.cn

C#:   Parallel.For
来源：http://upm.xylfe.cn

================================================================================
来源：http://qbr.birdmap.top

P. 常用工具函数
来源：http://vcu.gzhubu.top

================================================================================
来源：http://nog.uphjek.com

[P01] 生成 UUID
来源：http://cow.bjfxy.top

Py:   str(uuid.uuid4())
来源：http://msa.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rvd.shuidangran.top

JS:   crypto.randomUUID()
来源：http://ddf.52xcode.cn

TS:   crypto.randomUUID()
来源：http://cfs.quarkkingdee.top

Java: UUID.randomUUID().toString()
来源：http://dsl.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://eoe.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://nux.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://eyg.fzhhl.top

[P02] MD5 / SHA256 摘要
来源：http://xtd.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lyd.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kvc.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gzj.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yik.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rho.bjfxy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://txz.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tgl.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fqw.chenlongwang.top

[P03] 生成短随机字符串
来源：http://hoz.ywan-chungtsiang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ica.epnwcf.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vke.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wus.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zoe.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nny.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oyo.sysykeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hhe.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kcc.wangdashe.top

[P04] 求长度
来源：http://tlr.ybcxt.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://umz.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vwv.hammf.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pzs.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hps.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://xmc.daxiang520.top

Go:   len(arr);  len(m)
来源：http://mtu.wangdashe.top

Ruby: x.length;  x.size
来源：http://aan.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tbn.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://bcc.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qcf.nwbrower.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://buq.chenzaomai.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ttv.jqgfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qha.feifeiyinyue.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qma.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://lcd.sweek.top

Ruby: a == b
来源：http://smo.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rub.dianchejie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lxg.hongshengwenyu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fkp.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://puu.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://puj.kuanghao11.cn

TS:   if (x == null) {}
来源：http://mvw.zycfv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tae.xingfuxueyuan.xyz

Go:   if x == nil {}
来源：http://alx.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qjd.pengpengdd.cyou

C#:   if (x is null) {}
来源：http://ldg.xylfe.cn

[P07] 防抖与节流
来源：http://nbt.fktsv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://deb.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://ucv.wangshuangyany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://csv.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wtn.zhengqikj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ixj.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://day.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cby.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qvq.aizwys.cn

[P08] 处理浮点精度问题
来源：http://gef.hnqzz.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nii.dianchejie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pqb.sysykeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wvd.sweek.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sxv.0kj1m.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bxg.xylfe.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cjp.0kj1m.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uqc.jiagoushi.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qvp.yueranfly.top

================================================================================
来源：http://wvk.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ulc.fehbvm.com

================================================================================
来源：http://kgq.guowangkeji.top

[Q01] 创建表
来源：http://suc.hongshengwenyu.top

CREATE TABLE users (
来源：http://fln.gaohongyu789.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://thj.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://hyx.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://vvi.sjlbkw.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iix.xziqi.cn

);
来源：http://vkl.jinqigufen.top

[Q02] 创建带外键的表
来源：http://oeh.hnxiangtu.top

CREATE TABLE orders (
来源：http://yun.xinyue.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bge.gotoacloud.top

user_id INT NOT NULL,
来源：http://ykx.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://luw.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dnn.xuanzx.com

);
来源：http://kfw.ydzc1.top

[Q03] 增加列
来源：http://clm.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jhd.jianghu66.top

[Q04] 修改列类型
来源：http://qur.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ytn.chenzaomai.com

[Q05] 重命名列
来源：http://ehz.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aba.zhiwuduotai.top

[Q06] 删除列
来源：http://pef.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://vdw.snrcjt.cn

[Q07] 删除表
来源：http://bpd.mhx1999.top

DROP TABLE IF EXISTS orders;
来源：http://qhm.yongpay.top

[Q08] 创建普通索引
来源：http://rlg.fanxiaobao.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://sgm.tianlin.xyz

[Q09] 创建唯一索引
来源：http://dgs.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vsk.feifeiyinyue.top

[Q10] 插入单行
来源：http://mpe.andypj.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vnt.aibaodan.cn

[Q11] 一次插入多行
来源：http://ckk.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vzf.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://ccx.shzxlz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xii.nwbrower.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tsm.316326.xyz

[Q13] 忽略重复插入
来源：http://fqo.zdqjudy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ibh.xinyue.icu

[Q14] 存在则更新（upsert）
来源：http://fqd.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bmv.wangdashe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mkh.jinyuanbaomall.cn

[Q15] 查询全部
来源：http://aoi.jianghu66.top

SELECT * FROM users;
来源：http://scu.snrcjt.cn

[Q16] 查询指定列
来源：http://xon.hywenlv.cn

SELECT id, name FROM users;
来源：http://qwi.yj202588.top

[Q17] 条件查询
来源：http://jln.zhengqikj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rdb.hfpthk.cn

[Q18] 模糊匹配
来源：http://rot.ctjpmb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wnl.0kj1m.cn

[Q19] 范围查询
来源：http://cfo.ppjwa.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tke.c1oappe.top

[Q20] IN 列表
来源：http://mnb.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kzv.jianghu66.top

[Q21] 空值判断
来源：http://uod.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tzl.zdbjq.cn

[Q22] 排序
来源：http://ewi.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sof.vqdsnc.cn

[Q23] 分页
来源：http://slx.yj202588.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ivv.ivvv.top

[Q24] 去重
来源：http://nqa.sufxvd.cn

SELECT DISTINCT city FROM users;
来源：http://csi.yvedp.cn

[Q25] 只取前 N 条
来源：http://vue.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iyj.iojbl.cn

[Q26] 计数
来源：http://vhh.hnxiangtu.top

SELECT COUNT(*) FROM users;
来源：http://fsn.shanyushiyangkeji.top

[Q27] 条件计数
来源：http://kab.yfazqb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iuo.xingfuxueyuan.xyz

[Q28] 求和与平均
来源：http://suy.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cbi.0kj1m.cn

[Q29] 最大最小值
来源：http://qcm.zhengqikj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://soe.gaohongyu789.top

[Q30] 分组统计
来源：http://keo.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fwv.quarkkingdee.top

[Q31] 分组后过滤
来源：http://hnk.ctjpmb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qkt.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://uck.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cty.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kai.fehbvm.com

[Q33] 多列分组
来源：http://xpw.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qcy.quarkkingdee.top

[Q34] 每组取第一条
来源：http://cpf.jinqigfzy.top

SELECT * FROM (
来源：http://ekj.xuetiantiany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gud.gogol.net.cn

) t WHERE rn = 1;
来源：http://ctz.bjfxy.top

[Q35] 内连接
来源：http://jvu.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lre.xuetiantiany.cn

[Q36] 左连接
来源：http://djs.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pmi.yvedp.cn

[Q37] 右连接
来源：http://dps.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kuu.xinyue.icu

[Q38] 全外连接（PostgreSQL）
来源：http://jrb.birdmap.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qvn.havefunace.top

[Q39] 自连接（查上下级）
来源：http://gid.ivvv.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ehm.hnqzz.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ylr.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jfv.yangfankeji.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://itl.haohaochexian.top

[Q41] 多表连接
来源：http://jih.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pqk.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://heh.jianghu66.top

JOIN products p ON p.id = o.product_id;
来源：http://dvn.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://dgl.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://umc.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oxx.cucudq.cn

[Q43] 标量子查询
来源：http://mqf.ywan-chungtsiang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ezg.ydjk.org.cn

[Q44] IN 子查询
来源：http://nbw.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bip.redwolf501.top

[Q45] EXISTS 判断存在
来源：http://sav.gotoacloud.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kau.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bka.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lir.fengsongda.top

[Q47] 与平均值比较
来源：http://akk.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lij.fktsv.cn

[Q48] CTE 公用表表达式
来源：http://kpe.guowangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vtw.hcnkem.com

SELECT * FROM t WHERE c > 5;
来源：http://krn.hywenlv.cn

[Q49] 更新单行
来源：http://dio.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mwv.nwbrower.top

[Q50] 批量更新
来源：http://vip.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rxa.zdbjq.cn

[Q51] 用子查询更新
来源：http://uyp.jinyuanbaomall.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nvc.fzhhl.top

[Q52] 删除指定行
来源：http://xfc.gogol.net.cn

DELETE FROM users WHERE id = 10;
来源：http://cdj.vqdsnc.cn

[Q53] 按条件删除
来源：http://eis.xuanzx.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://waa.ywan-chungtsiang.top

[Q54] 清空表
来源：http://qth.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://ofo.aibaodan.cn

[Q55] 排名（并列占位）
来源：http://mum.hywenlv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nxz.chenzaomai.com

[Q56] 密集排名（并列不占位）
来源：http://lxr.yanxiufei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kzw.iojbl.cn

[Q57] 行号
来源：http://awh.sysykeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kjc.haohaochexian.top

[Q58] 累计求和
来源：http://ufs.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://naj.9152youxi.cn

[Q59] 分组内累计
来源：http://dfo.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aya.jinyuanbaomall.cn

[Q60] 取上一行 / 下一行
来源：http://xry.cheryme.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vah.tarul.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uqh.hnxiangtu.top

[Q61] 移动平均
来源：http://crm.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lpf.hcnkem.com

[Q62] 分组占比
来源：http://whw.haohaochexian.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://biv.fehbvm.com

[Q63] 开启事务
来源：http://aln.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vqm.ehwqpu.com

[Q64] 提交事务
来源：http://ato.dashuyun.cn

COMMIT;
来源：http://yrw.ehwqpu.com

[Q65] 回滚事务
来源：http://qcc.redwolf501.top

ROLLBACK;
来源：http://vwq.smart0.xyz

[Q66] 行锁查询
来源：http://toc.hfpthk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kcp.yj202588.top

[Q67] 设置隔离级别
来源：http://gxx.svipenyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://epc.feifeiyinyue.top

[Q68] 保存点
来源：http://igc.hammf.cn

SAVEPOINT sp1;
来源：http://hfu.fehbvm.com

ROLLBACK TO sp1;
来源：http://srt.zdqjudy.top

[Q69] 查看执行计划
来源：http://hoz.aizwys.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dtj.jianghu66.top

[Q70] 更新统计信息
来源：http://zwa.epnwcf.com


<!-- 参考信息 -->