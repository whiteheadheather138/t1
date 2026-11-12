代发 wailian999

Go:   // 手写递归
来源：http://gxv.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://umf.yueranfly.top

C#:   // 手写递归
来源：http://lqs.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bcg.nanxinkj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://keb.ctjpmb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qng.yfazqb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ubs.zhijiandao.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xyn.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pvs.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vkk.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bgl.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cnz.yongpay.top

================================================================================
来源：http://hjb.sjlbkw.cn

O. 并发与异步
来源：http://hob.yangfankeji.com

================================================================================
来源：http://mtx.yueranfly.top

[O01] 启动一个线程
来源：http://bbm.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gic.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kza.zhengqikj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zpo.iojbl.cn

TS:   // 同 JS
来源：http://qkf.zhoulong.xyz

Java: new Thread(() -> f()).start()
来源：http://kvx.havefunace.top

Go:   go f()
来源：http://kay.daria6918.cn

Ruby: Thread.new { f }
来源：http://tbo.daria6918.cn

C#:   Task.Run(() => F());
来源：http://ykn.pengpengdd.cyou

[O02] 使用线程池
来源：http://nap.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mug.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bcu.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://hwq.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://wsf.jinyuanbaomall.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uog.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cna.yuanzhike.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://acv.zhengqikj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gnn.guannengcc.top

[O03] 加锁保护共享数据
来源：http://paf.hnqzz.top

Py:   with lock: shared += 1
来源：http://cjr.shanyushiyangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://ruo.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jsj.shanyushiyangtech.top

TS:   // 同 JS
来源：http://igl.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://slz.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nwy.redwolf501.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ntx.ybcxt.top

C#:   lock (gate) { shared++; }
来源：http://isr.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://hcb.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://rvo.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xke.xinyue.icu

JS:   async function f() { await g(); }
来源：http://los.cdnleiting.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qrx.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hrk.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fgy.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nbv.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://fbt.chenlongwang.top

[O05] 并发执行并等待全部完成
来源：http://tcg.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://bcx.dashuyun.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dia.daxiang520.top

JS:   await Promise.all(tasks)
来源：http://xul.cashguo.top

TS:   await Promise.all(tasks)
来源：http://vwn.jinqigfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mkw.0kj1m.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pdp.redwolf501.top

Ruby: threads.map(&:join)
来源：http://aks.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://pqj.birdmap.top

[O06] 使用进程池
来源：http://ooa.jiagoushi.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gbq.yuxming.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qlq.gzhubu.top

JS:   // child_process / cluster 模块
来源：http://azk.ivvv.top

TS:   // child_process / cluster 模块
来源：http://kes.xziqi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nbc.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://txa.nwbrower.top

Ruby: // fork 块
来源：http://szj.zhixingplan.top

C#:   Parallel.For
来源：http://tqj.guowangkeji.top

================================================================================
来源：http://hyg.c1oappe.top

P. 常用工具函数
来源：http://ltd.shangyingyoupin.top

================================================================================
来源：http://ndp.xylfe.cn

[P01] 生成 UUID
来源：http://dqn.ctjpmb.com

Py:   str(uuid.uuid4())
来源：http://xlt.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wyx.c1oappe.top

JS:   crypto.randomUUID()
来源：http://yxz.tian-w.cn

TS:   crypto.randomUUID()
来源：http://mux.yongpay.top

Java: UUID.randomUUID().toString()
来源：http://usn.316326.xyz

Go:   // 用 github.com/google/uuid
来源：http://vva.wangshuangyany.cn

Ruby: SecureRandom.uuid
来源：http://wyi.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://ojc.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://dzm.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xon.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://agv.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uie.zhaomingkeji.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xox.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://amy.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qyz.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lbe.zhongyouzk.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vds.vqdsnc.cn

[P03] 生成短随机字符串
来源：http://plu.pengpengdd.cyou

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lzu.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ljr.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iji.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fuu.jlsjyb.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sxj.nanxinkj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://raf.zdbjq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dwo.wangdashe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nok.ybcxt.top

[P04] 求长度
来源：http://xob.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ytn.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vhs.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xlq.c1oappe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iie.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://mbe.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://gbs.yueranfly.top

Ruby: x.length;  x.size
来源：http://eiz.gotoacloud.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jfy.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://nyt.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xjd.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lmx.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ovs.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zkv.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hal.xingfuxueyuan.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://qmt.aizwys.cn

Ruby: a == b
来源：http://sat.sjlbkw.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aro.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qps.zhoulong.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hyb.ctjpmb.com

PHP:  if (empty($x)) {}
来源：http://buz.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oqr.yanxiufei.cn

TS:   if (x == null) {}
来源：http://pqj.jiagoushi.top

Java: if (x == null || x.isEmpty()) {}
来源：http://spj.shangyingyoupin.top

Go:   if x == nil {}
来源：http://wbh.cheryme.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://irg.zhoulong.xyz

C#:   if (x is null) {}
来源：http://dos.quarkkingdee.top

[P07] 防抖与节流
来源：http://jcq.aizwys.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xbf.shangyingyoupin.top

PHP:  // 手写时间戳比较
来源：http://cev.jianghu66.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yyg.bbcook.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://txi.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zmc.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fwz.tanke756.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xzb.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uck.xziqi.cn

[P08] 处理浮点精度问题
来源：http://vbn.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://imz.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nnc.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uxc.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hit.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pkh.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kyo.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ohs.bjfxy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eut.ybcxt.top

================================================================================
来源：http://bpe.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://apw.yonumen.top

================================================================================
来源：http://qgu.nanxuanxn.top

[Q01] 创建表
来源：http://dme.sjlbkw.cn

CREATE TABLE users (
来源：http://yac.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kyp.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://zmc.hnxiangtu.top

email VARCHAR(100) UNIQUE,
来源：http://jzk.yvedp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uzj.hesvh.cn

);
来源：http://lhr.zdqjudy.top

[Q02] 创建带外键的表
来源：http://roi.epnwcf.com

CREATE TABLE orders (
来源：http://nnw.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ffl.sjlbkw.cn

user_id INT NOT NULL,
来源：http://qen.vehdjk.com

amount DECIMAL(10, 2),
来源：http://vts.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oqy.hywenlv.cn

);
来源：http://xnq.jyoumei.cn

[Q03] 增加列
来源：http://ekx.meibo888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gvq.shangyingyoupin.top

[Q04] 修改列类型
来源：http://bbj.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gxq.pycfn.com

[Q05] 重命名列
来源：http://vzr.fzhhl.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oqx.ctjpmb.com

[Q06] 删除列
来源：http://lrp.xuetiantiany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mjd.havefunace.top

[Q07] 删除表
来源：http://fim.tianlin.xyz

DROP TABLE IF EXISTS orders;
来源：http://uee.chenzaomai.com

[Q08] 创建普通索引
来源：http://gfr.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fda.yj20258888.top

[Q09] 创建唯一索引
来源：http://sim.shangyingyoupin.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xyp.zhijiandao.cn

[Q10] 插入单行
来源：http://zfw.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xxz.xingfuxueyuan.xyz

[Q11] 一次插入多行
来源：http://ost.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ume.uphjek.com

[Q12] 插入后取自增 ID
来源：http://mfb.xziqi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jov.hfpthk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://flh.tian-w.cn

[Q13] 忽略重复插入
来源：http://dwc.tian-w.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jva.feifeiyinyue.top

[Q14] 存在则更新（upsert）
来源：http://okq.316326.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yma.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pnh.yuxming.cn

[Q15] 查询全部
来源：http://iow.ybcxt.top

SELECT * FROM users;
来源：http://hni.zdbjq.cn

[Q16] 查询指定列
来源：http://mab.yvedp.cn

SELECT id, name FROM users;
来源：http://rur.daria6918.cn

[Q17] 条件查询
来源：http://seq.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yzx.aizwys.cn

[Q18] 模糊匹配
来源：http://sor.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ptx.smart0.xyz

[Q19] 范围查询
来源：http://xul.svipenyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wkm.zhaomingkeji.xyz

[Q20] IN 列表
来源：http://fkb.pycfn.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rys.hongshengwenyu.top

[Q21] 空值判断
来源：http://dwt.cqqwz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jng.wangshuangyany.cn

[Q22] 排序
来源：http://pny.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://duc.daria6918.cn

[Q23] 分页
来源：http://bho.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ixz.nwbrower.top

[Q24] 去重
来源：http://apf.zdbjq.cn

SELECT DISTINCT city FROM users;
来源：http://omj.tianlin.xyz

[Q25] 只取前 N 条
来源：http://atm.yj20258.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fud.hammf.cn

[Q26] 计数
来源：http://hwg.vehdjk.com

SELECT COUNT(*) FROM users;
来源：http://cmn.uphjek.com

[Q27] 条件计数
来源：http://mkx.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wcb.hnxiangtu.top

[Q28] 求和与平均
来源：http://efz.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cnb.zycfv.cn

[Q29] 最大最小值
来源：http://hxn.vqdsnc.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mkb.pengpengdd.cyou

[Q30] 分组统计
来源：http://urd.yj202588.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zxs.jlsjyb.cn

[Q31] 分组后过滤
来源：http://grz.sxryk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aqi.sysykeji.top

[Q32] 分组拼接字符串
来源：http://okq.haohaochexian.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tdh.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yiq.aizwys.cn

[Q33] 多列分组
来源：http://zwe.hnxiangtu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vxz.yj20258.top

[Q34] 每组取第一条
来源：http://htc.bbcook.cn

SELECT * FROM (
来源：http://ioo.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xms.daria6918.cn

) t WHERE rn = 1;
来源：http://quz.epnwcf.com

[Q35] 内连接
来源：http://xqr.0kj1m.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lcb.hcnkem.com

[Q36] 左连接
来源：http://vut.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vjx.jinqigufen.top

[Q37] 右连接
来源：http://cgm.wangshuangyany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rzf.hnxiangtu.top

[Q38] 全外连接（PostgreSQL）
来源：http://cdj.bjfxy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wwx.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://nyw.316326.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://zev.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ybv.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hjn.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tbc.tian-w.cn

[Q41] 多表连接
来源：http://gcy.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fxa.zhoulong.xyz

JOIN users u ON u.id = o.user_id
来源：http://reo.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://kzn.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://xja.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://tbf.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uif.tianlin.xyz

[Q43] 标量子查询
来源：http://nlo.zhixingplan.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vyy.snrcjt.cn

[Q44] IN 子查询
来源：http://xbn.wangshuangyany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jiv.pycfn.com

[Q45] EXISTS 判断存在
来源：http://dgv.jinyuanbaomall.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hjm.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://pco.yj20258888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uhq.bbcook.cn

[Q47] 与平均值比较
来源：http://umf.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pst.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://lqj.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dzw.fanxiaobao.xyz

SELECT * FROM t WHERE c > 5;
来源：http://dsr.snrcjt.cn

[Q49] 更新单行
来源：http://qfd.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bqr.uphjek.com

[Q50] 批量更新
来源：http://qhm.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ljf.jqgufenzy.top

[Q51] 用子查询更新
来源：http://zou.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://izp.gotoacloud.top

[Q52] 删除指定行
来源：http://gcw.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://rqz.jqgfzy.top

[Q53] 按条件删除
来源：http://kvq.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jbb.ydzc1.top

[Q54] 清空表
来源：http://ths.tanke756.top

TRUNCATE TABLE logs;
来源：http://jfj.gogol.net.cn

[Q55] 排名（并列占位）
来源：http://wvd.uphjek.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jdq.nwbrower.top

[Q56] 密集排名（并列不占位）
来源：http://iws.andypj.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jgi.fzhhl.top

[Q57] 行号
来源：http://utz.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://boe.wangdashe.top

[Q58] 累计求和
来源：http://xgd.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ssa.hammf.cn

[Q59] 分组内累计
来源：http://dti.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://imx.ybcxt.top

[Q60] 取上一行 / 下一行
来源：http://nux.jinqigufen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yhy.wangshuangyany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tig.ybcxt.top

[Q61] 移动平均
来源：http://sxr.andypj.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hvm.daxiang520.top

[Q62] 分组占比
来源：http://xnt.yj202588.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xgw.jiagoushi.top

[Q63] 开启事务
来源：http://ami.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://gcj.jqgufenzy.top

[Q64] 提交事务
来源：http://pmx.ydzc1.top

COMMIT;
来源：http://zne.fengsongda.top

[Q65] 回滚事务
来源：http://ujs.chenjidiqi.icu

ROLLBACK;
来源：http://tvb.smart0.xyz

[Q66] 行锁查询
来源：http://zci.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ckm.feifeiyinyue.top


<!-- 参考信息 -->