代发 wailian999

Go:   // 手写递归
来源：http://pen.andypj.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://buc.zycfv.cn

C#:   // 手写递归
来源：http://kcp.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eri.zdqjudy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ano.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qqm.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sol.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jyc.fehbvm.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cfq.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eod.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qih.pengpengdd.cyou

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://les.yuxming.cn

================================================================================
来源：http://vjg.jqgufenzy.top

O. 并发与异步
来源：http://vhp.xinyue.icu

================================================================================
来源：http://igj.cdnleiting.top

[O01] 启动一个线程
来源：http://uws.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qnx.316326.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ihr.daria6918.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://olx.xinyue.icu

TS:   // 同 JS
来源：http://utu.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://nnl.sysykeji.top

Go:   go f()
来源：http://wyc.jqgfzy.top

Ruby: Thread.new { f }
来源：http://grb.52xcode.cn

C#:   Task.Run(() => F());
来源：http://gtb.iojbl.cn

[O02] 使用线程池
来源：http://der.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://crd.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ove.cucudq.cn

JS:   // worker_threads 线程池
来源：http://zxh.yj20258.top

TS:   // worker_threads 线程池
来源：http://zmh.gzhubu.top

Java: Executors.newFixedThreadPool(4)
来源：http://yrl.shanyushiyangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://snd.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ahs.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://orv.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://ijm.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://iqe.chenzaomai.com

PHP:  // 用 flock() 做文件锁
来源：http://ddg.yj20258888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bal.yuxming.cn

TS:   // 同 JS
来源：http://urz.fengsongda.top

Java: synchronized (this) { shared++; }
来源：http://mmn.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://apj.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ryk.redwolf501.top

C#:   lock (gate) { shared++; }
来源：http://ebh.mhx1999.top

[O04] 定义异步函数并等待
来源：http://sjr.jyoumei.cn

Py:   async def f():⏎    await g()
来源：http://uqt.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yln.mhx1999.top

JS:   async function f() { await g(); }
来源：http://rzz.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://lcv.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://etz.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://otl.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://iyu.ppjwa.cn

C#:   async Task F() { await G(); }
来源：http://zpx.shzxlz.cn

[O05] 并发执行并等待全部完成
来源：http://zst.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://gcf.ywan-chungtsiang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tca.ctjpmb.com

JS:   await Promise.all(tasks)
来源：http://dcr.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://qvy.ydzc1.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vyl.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wzf.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://jbd.zhoulong.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://wrq.haohaochexian.top

[O06] 使用进程池
来源：http://lzh.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fsv.shanyushiyangtech.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jke.shanyushiyangtech.top

JS:   // child_process / cluster 模块
来源：http://ggv.pengpengdd.cyou

TS:   // child_process / cluster 模块
来源：http://dsd.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vml.cheryme.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oxx.nwbrower.top

Ruby: // fork 块
来源：http://rgh.zhoulong.xyz

C#:   Parallel.For
来源：http://vmd.jinqigufen.top

================================================================================
来源：http://spp.tian-w.cn

P. 常用工具函数
来源：http://cem.yueranfly.top

================================================================================
来源：http://lhx.jinyuanbaomall.cn

[P01] 生成 UUID
来源：http://qtr.zhixingplan.top

Py:   str(uuid.uuid4())
来源：http://nvq.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qkp.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://oms.c1oappe.top

TS:   crypto.randomUUID()
来源：http://dxg.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://tjb.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://drr.zycfv.cn

Ruby: SecureRandom.uuid
来源：http://hqk.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://ihf.haohaochexian.top

[P02] MD5 / SHA256 摘要
来源：http://fls.nwbrower.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iry.andypj.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://roj.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ien.zdqjudy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eck.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ysj.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kwz.aibaodan.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gsc.andypj.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dmo.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://tzq.jinqigufen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yja.yvedp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eyb.shuidangran.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tng.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dtz.gotoacloud.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gxo.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wdt.chenlongwang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gml.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vkt.daxiang520.top

[P04] 求长度
来源：http://yzt.yj20258888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hsv.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://axq.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gjc.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://njr.vehdjk.com

Java: list.size();  map.size();  s.length()
来源：http://ugr.shanyushiyangtech.top

Go:   len(arr);  len(m)
来源：http://ihq.shanyushiyangkeji.top

Ruby: x.length;  x.size
来源：http://gpf.jlsjyb.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pec.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://urw.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://eec.xingfuxueyuan.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cnf.yuanzhike.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bay.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bke.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vkv.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gzq.52xcode.cn

Ruby: a == b
来源：http://ffv.jiagoushi.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://thq.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hfz.jinghuilouyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dpt.gotoacloud.top

PHP:  if (empty($x)) {}
来源：http://orh.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jeg.gaohongyu789.top

TS:   if (x == null) {}
来源：http://ohb.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mmi.quarkkingdee.top

Go:   if x == nil {}
来源：http://ugf.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://drz.vehdjk.com

C#:   if (x is null) {}
来源：http://zvl.tianlin.xyz

[P07] 防抖与节流
来源：http://hst.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rob.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://wki.yongpay.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mek.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vzt.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jeo.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lsj.guowangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uvj.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vzq.yongpay.top

[P08] 处理浮点精度问题
来源：http://juu.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bys.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nye.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fqa.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gxv.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kju.jiagoushi.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://djk.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yhp.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wkn.yfazqb.com

================================================================================
来源：http://sga.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://too.vehdjk.com

================================================================================
来源：http://jpj.bjfxy.top

[Q01] 创建表
来源：http://nbd.c1oappe.top

CREATE TABLE users (
来源：http://qho.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lia.sweek.top

name VARCHAR(50) NOT NULL,
来源：http://fgx.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://pxr.jinqigfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zkg.52xcode.cn

);
来源：http://dij.aibaodan.cn

[Q02] 创建带外键的表
来源：http://fip.uphjek.com

CREATE TABLE orders (
来源：http://fdd.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://swg.cashguo.top

user_id INT NOT NULL,
来源：http://jcq.ivvv.top

amount DECIMAL(10, 2),
来源：http://ois.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vpm.hysaishi.cn

);
来源：http://tvx.nwbrower.top

[Q03] 增加列
来源：http://qmw.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rxv.jiagoushi.top

[Q04] 修改列类型
来源：http://xnn.daria6918.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fes.yj20258888.top

[Q05] 重命名列
来源：http://yzm.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oxe.nanxuanxn.top

[Q06] 删除列
来源：http://sio.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://mod.vehdjk.com

[Q07] 删除表
来源：http://ymr.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://hyr.aizwys.cn

[Q08] 创建普通索引
来源：http://ezu.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yfl.cdnleiting.top

[Q09] 创建唯一索引
来源：http://bpq.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zah.hcnkem.com

[Q10] 插入单行
来源：http://woy.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zog.iojbl.cn

[Q11] 一次插入多行
来源：http://iaj.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xzo.xuetiantiany.cn

[Q12] 插入后取自增 ID
来源：http://akm.zhixingplan.top

INSERT INTO users (name) VALUES ('C');
来源：http://hob.sufxvd.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sgs.yj202588.top

[Q13] 忽略重复插入
来源：http://jau.yonumen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://agu.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://ias.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pln.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pbq.bjfxy.top

[Q15] 查询全部
来源：http://nxj.tarul.cn

SELECT * FROM users;
来源：http://bwi.ctjpmb.com

[Q16] 查询指定列
来源：http://cgl.nwbrower.top

SELECT id, name FROM users;
来源：http://fsv.gogol.net.cn

[Q17] 条件查询
来源：http://wno.guannengcc.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rgo.9152youxi.cn

[Q18] 模糊匹配
来源：http://rmh.andypj.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kcm.shanyushiyangtech.top

[Q19] 范围查询
来源：http://wzn.jinqigufen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qpq.pengpengdd.cyou

[Q20] IN 列表
来源：http://qwa.hesvh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tyz.dianchejie.cn

[Q21] 空值判断
来源：http://bjs.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bvb.jiagoushi.top

[Q22] 排序
来源：http://ykc.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nzp.jinqigfzy.top

[Q23] 分页
来源：http://smp.dashuyun.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lbj.fzhhl.top

[Q24] 去重
来源：http://eqc.birdmap.top

SELECT DISTINCT city FROM users;
来源：http://soq.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://jys.aibaodan.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://csj.quarkkingdee.top

[Q26] 计数
来源：http://kzi.sjlbkw.cn

SELECT COUNT(*) FROM users;
来源：http://hyd.gotoacloud.top

[Q27] 条件计数
来源：http://oah.aibaodan.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://igm.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://tgz.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://str.cdnleiting.top

[Q29] 最大最小值
来源：http://cuy.jinqigufen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wks.cucudq.cn

[Q30] 分组统计
来源：http://kos.zhiwuduotai.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yxz.0kj1m.cn

[Q31] 分组后过滤
来源：http://uwt.zhaomingkeji.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qan.jinqigfzy.top

[Q32] 分组拼接字符串
来源：http://pju.meibo888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gyy.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bkb.sysykeji.top

[Q33] 多列分组
来源：http://zxz.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mgq.zhijiandao.cn

[Q34] 每组取第一条
来源：http://oiv.ydjk.org.cn

SELECT * FROM (
来源：http://ilr.tanke756.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fmu.jyoumei.cn

) t WHERE rn = 1;
来源：http://mqk.hnqzz.top

[Q35] 内连接
来源：http://nmc.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rjg.aibaodan.cn

[Q36] 左连接
来源：http://hli.daxiang520.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jtp.vqdsnc.cn

[Q37] 右连接
来源：http://tjh.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://efg.feifeiyinyue.top

[Q38] 全外连接（PostgreSQL）
来源：http://hzo.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jdq.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://pcv.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uwa.daxiang520.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ozh.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ztd.svipenyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mib.quarkkingdee.top

[Q41] 多表连接
来源：http://qsv.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://goz.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://ngy.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://cjd.ivvv.top

[Q42] 连接条件附加过滤
来源：http://dxo.pycfn.com

SELECT u.name, o.amount FROM users u
来源：http://nko.yuxming.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xpq.shzxlz.cn

[Q43] 标量子查询
来源：http://aln.tianlin.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iqg.sxryk.cn

[Q44] IN 子查询
来源：http://kch.aibaodan.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qtc.dashuyun.cn

[Q45] EXISTS 判断存在
来源：http://xvn.pycfn.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fel.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://vdu.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rjk.jqgfzy.top

[Q47] 与平均值比较
来源：http://mhp.ivvv.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nhi.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://rld.haohaochexian.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ypi.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://vzy.shuidangran.top

[Q49] 更新单行
来源：http://kjd.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://udm.wangshuangyany.cn

[Q50] 批量更新
来源：http://nac.zhiwuduotai.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yrk.yangfankeji.com

[Q51] 用子查询更新
来源：http://kth.ctjpmb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wnz.ywan-chungtsiang.top

[Q52] 删除指定行
来源：http://vfk.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://eku.quarkkingdee.top

[Q53] 按条件删除
来源：http://unb.chenjidiqi.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fis.birdmap.top

[Q54] 清空表
来源：http://lpx.jianghu66.top

TRUNCATE TABLE logs;
来源：http://wtf.zdbjq.cn

[Q55] 排名（并列占位）
来源：http://fhj.gaohongyu789.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aab.zhiwuduotai.top

[Q56] 密集排名（并列不占位）
来源：http://vpj.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xvt.daria6918.cn

[Q57] 行号
来源：http://mlq.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vom.jinyuanbaomall.cn

[Q58] 累计求和
来源：http://hrt.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xfu.yonumen.top

[Q59] 分组内累计
来源：http://ktg.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vnq.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://nhi.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jtd.snrcjt.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lrr.chenlongwang.top

[Q61] 移动平均
来源：http://ylf.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gez.svipenyu.cn

[Q62] 分组占比
来源：http://afl.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gsy.zhijiandao.cn

[Q63] 开启事务
来源：http://xcc.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://fpq.yueranfly.top

[Q64] 提交事务
来源：http://ahi.kuanghao11.cn

COMMIT;
来源：http://qep.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://rih.yongpay.top

ROLLBACK;
来源：http://vdg.xylfe.cn

[Q66] 行锁查询
来源：http://wvg.hnqzz.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xqj.shuidangran.top


<!-- 参考信息 -->