代发 wailian999

Go:   // 手写递归
来源：http://txb.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tzc.ehwqpu.com

C#:   // 手写递归
来源：http://ton.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jpe.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ncg.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qft.redwolf501.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lsy.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cll.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aqo.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bjn.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tpo.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ubd.yueranfly.top

================================================================================
来源：http://jlf.guannengcc.top

O. 并发与异步
来源：http://twf.yj20258888.top

================================================================================
来源：http://qns.sweek.top

[O01] 启动一个线程
来源：http://bwl.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://afy.hnqzz.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dsy.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iit.zdbjq.cn

TS:   // 同 JS
来源：http://diw.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://jpk.quarkkingdee.top

Go:   go f()
来源：http://ycp.52xcode.cn

Ruby: Thread.new { f }
来源：http://eer.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://yqa.tarul.cn

[O02] 使用线程池
来源：http://zlh.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://edj.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ywm.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://dzi.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://joi.snrcjt.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jre.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vsz.cqqwz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mfp.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qkn.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://ooi.dianchejie.cn

Py:   with lock: shared += 1
来源：http://kts.cashguo.top

PHP:  // 用 flock() 做文件锁
来源：http://fae.nanxinkj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zxn.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://qjy.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://fvd.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fnq.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wgf.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://oaa.cqqwz.cn

[O04] 定义异步函数并等待
来源：http://akh.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://zlt.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lil.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://qjm.nanxuanxn.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tpl.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pfw.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iuo.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cxg.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://pdb.chenlongwang.top

[O05] 并发执行并等待全部完成
来源：http://kmy.dianchejie.cn

Py:   asyncio.gather(*tasks)
来源：http://blm.zhongyouzk.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://slv.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://vwg.cheryme.top

TS:   await Promise.all(tasks)
来源：http://npz.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yur.ydzc1.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mvi.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://cng.jinqigfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xkf.fktsv.cn

[O06] 使用进程池
来源：http://zwz.316326.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fud.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://irm.hnxiangtu.top

JS:   // child_process / cluster 模块
来源：http://swp.jinyuanbaomall.cn

TS:   // child_process / cluster 模块
来源：http://hbi.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vlh.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vuh.yueranfly.top

Ruby: // fork 块
来源：http://vvv.shanyushiyangtech.top

C#:   Parallel.For
来源：http://rlz.fanxiaobao.xyz

================================================================================
来源：http://aev.nanxinkj.top

P. 常用工具函数
来源：http://zgp.jianghu66.top

================================================================================
来源：http://lwz.jqgfzy.top

[P01] 生成 UUID
来源：http://oit.aibaodan.cn

Py:   str(uuid.uuid4())
来源：http://gxe.tianlin.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kse.yuanzhike.top

JS:   crypto.randomUUID()
来源：http://ubx.guannengcc.top

TS:   crypto.randomUUID()
来源：http://bmf.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://pxc.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://lpc.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://mez.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://dsx.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://pjt.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bvp.yueranfly.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://osc.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vhy.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sto.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dpu.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://khl.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cxl.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dkv.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://myn.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jkr.9152youxi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://trm.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oui.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://onb.hfpthk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iht.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pqb.vehdjk.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://wgd.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mwf.zdqjudy.top

[P04] 求长度
来源：http://ily.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nak.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tqy.hysaishi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ydz.daria6918.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iih.daria6918.cn

Java: list.size();  map.size();  s.length()
来源：http://tmo.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://jre.guannengcc.top

Ruby: x.length;  x.size
来源：http://rma.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://oga.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://lkh.aizwys.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kfq.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wzb.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uiw.hnqzz.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mxw.sxryk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uqg.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://gsd.tianlin.xyz

Ruby: a == b
来源：http://shp.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zeq.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tfo.fzhhl.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cnv.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://top.jiagoushi.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vvw.gaohongyu789.top

TS:   if (x == null) {}
来源：http://vck.jinghuilouyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jhx.snrcjt.cn

Go:   if x == nil {}
来源：http://mqo.316326.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wae.hfpthk.cn

C#:   if (x is null) {}
来源：http://mgg.gogol.net.cn

[P07] 防抖与节流
来源：http://fla.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lus.ctjpmb.com

PHP:  // 手写时间戳比较
来源：http://wqs.zhengqikj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://flm.yanxiufei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jmz.jinqigfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pxi.yanxiufei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ysk.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ezs.zycfv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bkh.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://jbt.yanxiufei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jdu.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lys.nwbrower.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gpt.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ijk.yj202588.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://egy.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vyi.aizwys.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://npi.vehdjk.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wgl.yfazqb.com

================================================================================
来源：http://huv.zhengqikj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aof.tanke756.top

================================================================================
来源：http://iul.daxiang520.top

[Q01] 创建表
来源：http://zjb.kuanghao11.cn

CREATE TABLE users (
来源：http://cmu.jinyuanbaomall.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qhs.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://xzi.daxiang520.top

email VARCHAR(100) UNIQUE,
来源：http://uyk.svipenyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qtx.ivvv.top

);
来源：http://ekj.guannengcc.top

[Q02] 创建带外键的表
来源：http://wbr.ehwqpu.com

CREATE TABLE orders (
来源：http://hqo.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fho.aibaodan.cn

user_id INT NOT NULL,
来源：http://qhd.316326.xyz

amount DECIMAL(10, 2),
来源：http://chp.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qya.fanxiaobao.xyz

);
来源：http://efk.bjfxy.top

[Q03] 增加列
来源：http://dwu.dashuyun.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tmi.yvedp.cn

[Q04] 修改列类型
来源：http://nns.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://std.meibo888.top

[Q05] 重命名列
来源：http://ctj.chenjidiqi.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zck.smart0.xyz

[Q06] 删除列
来源：http://ado.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rrl.wangdashe.top

[Q07] 删除表
来源：http://pat.birdmap.top

DROP TABLE IF EXISTS orders;
来源：http://lwf.nwbrower.top

[Q08] 创建普通索引
来源：http://dvr.tianlin.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://xtm.tanke756.top

[Q09] 创建唯一索引
来源：http://wit.tarul.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://frf.cucudq.cn

[Q10] 插入单行
来源：http://seh.yuanzhike.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://enk.yuanzhike.top

[Q11] 一次插入多行
来源：http://aps.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hhh.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://kqr.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lid.yanxiufei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yrh.ydjk.org.cn

[Q13] 忽略重复插入
来源：http://mej.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nsh.hongshengwenyu.top

[Q14] 存在则更新（upsert）
来源：http://auz.shanyushiyangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://owo.aibaodan.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dow.gogol.net.cn

[Q15] 查询全部
来源：http://mxi.cashguo.top

SELECT * FROM users;
来源：http://wbr.gaohongyu789.top

[Q16] 查询指定列
来源：http://uhf.yueranfly.top

SELECT id, name FROM users;
来源：http://cme.gotoacloud.top

[Q17] 条件查询
来源：http://mvf.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kxj.daxiang520.top

[Q18] 模糊匹配
来源：http://tuf.jinghuilouyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cci.ctjpmb.com

[Q19] 范围查询
来源：http://ptx.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ylz.zhiwuduotai.top

[Q20] IN 列表
来源：http://bez.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hum.ydjk.org.cn

[Q21] 空值判断
来源：http://zqk.sufxvd.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ywr.chenzaomai.com

[Q22] 排序
来源：http://gik.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://llz.aizwys.cn

[Q23] 分页
来源：http://aij.redwolf501.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pdl.meibo888.top

[Q24] 去重
来源：http://hvn.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://jnh.cqqwz.cn

[Q25] 只取前 N 条
来源：http://pkf.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://edx.shanyushiyangkeji.top

[Q26] 计数
来源：http://sej.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://beb.aizwys.cn

[Q27] 条件计数
来源：http://eub.dashuyun.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://veh.nanxuanxn.top

[Q28] 求和与平均
来源：http://ztn.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://juw.316326.xyz

[Q29] 最大最小值
来源：http://rwm.xuanzx.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://gla.shanyushiyangkeji.top

[Q30] 分组统计
来源：http://uin.vqdsnc.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tgq.jqgufenzy.top

[Q31] 分组后过滤
来源：http://tha.9152youxi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ylf.yvedp.cn

[Q32] 分组拼接字符串
来源：http://dii.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oyf.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://czv.aizwys.cn

[Q33] 多列分组
来源：http://szu.andypj.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gnh.ivvv.top

[Q34] 每组取第一条
来源：http://idj.yongpay.top

SELECT * FROM (
来源：http://bbg.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hev.yj20258888.top

) t WHERE rn = 1;
来源：http://eqg.daria6918.cn

[Q35] 内连接
来源：http://zic.vehdjk.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uvx.jyoumei.cn

[Q36] 左连接
来源：http://rhi.gotoacloud.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qfp.gaohongyu789.top

[Q37] 右连接
来源：http://amj.zdqjudy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://etp.shangyingyoupin.top

[Q38] 全外连接（PostgreSQL）
来源：http://fhy.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rmt.jinqigufen.top

[Q39] 自连接（查上下级）
来源：http://ttk.pycfn.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://wft.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lun.9152youxi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kas.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yru.yanxiufei.cn

[Q41] 多表连接
来源：http://aay.jinqigfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vcj.zhijiandao.cn

JOIN users u ON u.id = o.user_id
来源：http://hjs.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://klz.uphjek.com

[Q42] 连接条件附加过滤
来源：http://gxy.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://ruu.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://twr.yueranfly.top

[Q43] 标量子查询
来源：http://ucv.yuanzhike.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bct.sxryk.cn

[Q44] IN 子查询
来源：http://stz.gogol.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xsa.sweek.top

[Q45] EXISTS 判断存在
来源：http://rpu.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eps.yfazqb.com

[Q46] NOT EXISTS 判断不存在
来源：http://xwi.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://msk.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://rly.vqdsnc.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qza.haohaochexian.top

[Q48] CTE 公用表表达式
来源：http://xoi.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hgl.yj20258.top

SELECT * FROM t WHERE c > 5;
来源：http://roq.jlsjyb.cn

[Q49] 更新单行
来源：http://bce.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gcq.yj20258.top

[Q50] 批量更新
来源：http://lsy.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mqq.wangshuangyany.cn

[Q51] 用子查询更新
来源：http://qen.gzhubu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aks.tarul.cn

[Q52] 删除指定行
来源：http://alq.feifeiyinyue.top

DELETE FROM users WHERE id = 10;
来源：http://wul.aizwys.cn

[Q53] 按条件删除
来源：http://rzm.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ygo.jlsjyb.cn

[Q54] 清空表
来源：http://gre.guannengcc.top

TRUNCATE TABLE logs;
来源：http://kwj.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://kba.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gkd.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://ctt.redwolf501.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lgh.316326.xyz

[Q57] 行号
来源：http://vzn.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ybh.fehbvm.com

[Q58] 累计求和
来源：http://qao.yj202588.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://enp.jinqigufen.top

[Q59] 分组内累计
来源：http://jgc.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ozz.shanyushiyangtech.top

[Q60] 取上一行 / 下一行
来源：http://dqd.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nen.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ygc.hcnkem.com

[Q61] 移动平均
来源：http://ygk.jinqigufen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nyq.tianlin.xyz

[Q62] 分组占比
来源：http://cax.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sul.gaohongyu789.top

[Q63] 开启事务
来源：http://jlx.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pek.cucudq.cn

[Q64] 提交事务
来源：http://sxy.uphjek.com

COMMIT;
来源：http://wpr.haohaochexian.top

[Q65] 回滚事务
来源：http://dhk.daxiang520.top

ROLLBACK;
来源：http://uvm.zhiwuduotai.top

[Q66] 行锁查询
来源：http://nix.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ueu.smart0.xyz


<!-- 参考信息 -->