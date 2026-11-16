代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://oix.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ono.havefunace.top

[N11] 二叉树中序遍历
来源：http://naf.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cmw.cdnleiting.top

PHP:  // 手写递归函数
来源：http://ysx.hysaishi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://shn.dianchejie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sku.ctjpmb.com

Java: // 手写递归
来源：http://czs.dashuyun.cn

Go:   // 手写递归
来源：http://qxx.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yaf.gotoacloud.top

C#:   // 手写递归
来源：http://edc.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rtv.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vcs.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fsl.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://doy.zycfv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://auh.jinqigfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://asg.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rka.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gbh.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mtb.zhijiandao.cn

================================================================================
来源：http://mgs.sysykeji.top

O. 并发与异步
来源：http://tsq.dianchejie.cn

================================================================================
来源：http://nww.jyoumei.cn

[O01] 启动一个线程
来源：http://qvw.gotoacloud.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ibh.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yrp.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dez.yj20258.top

TS:   // 同 JS
来源：http://vud.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://ddg.guannengcc.top

Go:   go f()
来源：http://gmn.yj20258.top

Ruby: Thread.new { f }
来源：http://pee.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://ezx.feifeiyinyue.top

[O02] 使用线程池
来源：http://imb.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qfq.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bhr.daxiang520.top

JS:   // worker_threads 线程池
来源：http://ljv.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://fkg.bjfxy.top

Java: Executors.newFixedThreadPool(4)
来源：http://opf.shangyingyoupin.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lqr.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vzf.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ssg.yfazqb.com

[O03] 加锁保护共享数据
来源：http://vmx.xinyue.icu

Py:   with lock: shared += 1
来源：http://qgp.xylfe.cn

PHP:  // 用 flock() 做文件锁
来源：http://osj.ywan-chungtsiang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rwd.quarkkingdee.top

TS:   // 同 JS
来源：http://tfr.yongpay.top

Java: synchronized (this) { shared++; }
来源：http://plo.snrcjt.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lpa.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lpy.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://ppn.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://yeh.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://plv.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aas.fzhhl.top

JS:   async function f() { await g(); }
来源：http://yfs.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bko.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dng.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eri.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zfz.hesvh.cn

C#:   async Task F() { await G(); }
来源：http://wem.sufxvd.cn

[O05] 并发执行并等待全部完成
来源：http://dsx.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://fvi.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lbi.sweek.top

JS:   await Promise.all(tasks)
来源：http://lft.epnwcf.com

TS:   await Promise.all(tasks)
来源：http://iuo.vehdjk.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kps.jinyuanbaomall.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bin.ivvv.top

Ruby: threads.map(&:join)
来源：http://fil.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ycz.jiagoushi.top

[O06] 使用进程池
来源：http://hzt.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jtk.bbcook.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://crh.jyoumei.cn

JS:   // child_process / cluster 模块
来源：http://ypx.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://fuz.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://alz.tanke756.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yts.jinghuilouyu.cn

Ruby: // fork 块
来源：http://xsr.hesvh.cn

C#:   Parallel.For
来源：http://wsi.chenzaomai.com

================================================================================
来源：http://lmn.yj20258.top

P. 常用工具函数
来源：http://als.dianchejie.cn

================================================================================
来源：http://vqb.jqgfzy.top

[P01] 生成 UUID
来源：http://ixr.quarkkingdee.top

Py:   str(uuid.uuid4())
来源：http://wlc.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sgv.guannengcc.top

JS:   crypto.randomUUID()
来源：http://uyd.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://vml.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://eah.hfpthk.cn

Go:   // 用 github.com/google/uuid
来源：http://xit.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://jln.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://gwo.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://xga.jqgufenzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://noc.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lrl.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lqf.cashguo.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://axn.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://krr.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lec.vehdjk.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kjn.ehwqpu.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sms.xziqi.cn

[P03] 生成短随机字符串
来源：http://ppp.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ltt.yuxming.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yjj.yj202588.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rqw.pycfn.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yje.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ywz.zhongyouzk.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kpy.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://zuz.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zai.fktsv.cn

[P04] 求长度
来源：http://upg.ybcxt.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nuj.daria6918.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://has.sweek.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eyu.hcnkem.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pka.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://eyw.bjfxy.top

Go:   len(arr);  len(m)
来源：http://eil.yj20258888.top

Ruby: x.length;  x.size
来源：http://hjq.hongshengwenyu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pma.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://qgo.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://txv.hcnkem.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vwk.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://toj.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fou.chenlongwang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vdm.shzxlz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tfm.sjlbkw.cn

Ruby: a == b
来源：http://qpr.bbcook.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qlx.pycfn.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tww.bbcook.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tic.jqgufenzy.top

PHP:  if (empty($x)) {}
来源：http://uvx.ybcxt.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ogt.jinqigufen.top

TS:   if (x == null) {}
来源：http://tpi.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mer.shzxlz.cn

Go:   if x == nil {}
来源：http://wag.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://not.tian-w.cn

C#:   if (x is null) {}
来源：http://rdy.fzhhl.top

[P07] 防抖与节流
来源：http://dml.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://psw.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://vhx.jqgufenzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yvs.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ioi.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zpu.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dku.9152youxi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zri.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://has.xuanzx.com

[P08] 处理浮点精度问题
来源：http://vfs.ydjk.org.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://crs.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qon.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nqa.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pcw.hfpthk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pdw.dashuyun.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nwj.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cwx.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jat.nwbrower.top

================================================================================
来源：http://jye.zhixingplan.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cfg.ydzc1.top

================================================================================
来源：http://mnl.ppjwa.cn

[Q01] 创建表
来源：http://gkq.316326.xyz

CREATE TABLE users (
来源：http://tog.nanxinkj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wte.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://hrk.jinqigfzy.top

email VARCHAR(100) UNIQUE,
来源：http://xyf.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hvs.hfpthk.cn

);
来源：http://fte.nwbrower.top

[Q02] 创建带外键的表
来源：http://rfr.wangdashe.top

CREATE TABLE orders (
来源：http://cpa.zdqjudy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pkw.chenlongwang.top

user_id INT NOT NULL,
来源：http://jga.meibo888.top

amount DECIMAL(10, 2),
来源：http://ddo.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vrb.jinghuilouyu.cn

);
来源：http://qzm.cqqwz.cn

[Q03] 增加列
来源：http://skm.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sby.hnqzz.top

[Q04] 修改列类型
来源：http://jzk.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qtc.bbcook.cn

[Q05] 重命名列
来源：http://aif.feifeiyinyue.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xou.cheryme.top

[Q06] 删除列
来源：http://mvr.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://qpf.jianghu66.top

[Q07] 删除表
来源：http://eiq.yongpay.top

DROP TABLE IF EXISTS orders;
来源：http://uto.wangdashe.top

[Q08] 创建普通索引
来源：http://mbn.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://eom.sweek.top

[Q09] 创建唯一索引
来源：http://lsv.yonumen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wkb.zdqjudy.top

[Q10] 插入单行
来源：http://crf.yj20258888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mlj.jqgufenzy.top

[Q11] 一次插入多行
来源：http://jkf.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://npz.chenjidiqi.icu

[Q12] 插入后取自增 ID
来源：http://xhg.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://imf.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gxw.tianlin.xyz

[Q13] 忽略重复插入
来源：http://ugq.chenlongwang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qfi.zhiwuduotai.top

[Q14] 存在则更新（upsert）
来源：http://dhh.fengsongda.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ehi.ehwqpu.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pcp.yfazqb.com

[Q15] 查询全部
来源：http://dqi.shanyushiyangkeji.top

SELECT * FROM users;
来源：http://msk.yangfankeji.com

[Q16] 查询指定列
来源：http://oqn.yj20258888.top

SELECT id, name FROM users;
来源：http://flt.yuxming.cn

[Q17] 条件查询
来源：http://yoe.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://csr.chenjidiqi.icu

[Q18] 模糊匹配
来源：http://jqm.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uhb.bjfxy.top

[Q19] 范围查询
来源：http://fpz.xuanzx.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vsw.xuanzx.com

[Q20] IN 列表
来源：http://cqn.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zhd.bjfxy.top

[Q21] 空值判断
来源：http://trk.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cru.yangfankeji.com

[Q22] 排序
来源：http://igp.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vcz.yfazqb.com

[Q23] 分页
来源：http://xze.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qoi.shanyushiyangkeji.top

[Q24] 去重
来源：http://qzt.yanxiufei.cn

SELECT DISTINCT city FROM users;
来源：http://btr.xuanzx.com

[Q25] 只取前 N 条
来源：http://zvt.yuxming.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gqk.ydjk.org.cn

[Q26] 计数
来源：http://tzw.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://ioz.ctjpmb.com

[Q27] 条件计数
来源：http://wmr.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://spf.gaohongyu789.top

[Q28] 求和与平均
来源：http://rzr.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dnw.jyoumei.cn

[Q29] 最大最小值
来源：http://ike.dianchejie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://asv.c1oappe.top

[Q30] 分组统计
来源：http://jth.hnxiangtu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://imr.kuanghao11.cn

[Q31] 分组后过滤
来源：http://hvm.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://njo.zycfv.cn

[Q32] 分组拼接字符串
来源：http://mdu.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tka.uphjek.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://syx.jinghuilouyu.cn

[Q33] 多列分组
来源：http://cly.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://syl.cdnleiting.top

[Q34] 每组取第一条
来源：http://ehp.cashguo.top

SELECT * FROM (
来源：http://zpq.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ach.chenlongwang.top

) t WHERE rn = 1;
来源：http://qgp.zhaomingkeji.xyz

[Q35] 内连接
来源：http://kvl.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qpo.zdbjq.cn

[Q36] 左连接
来源：http://vff.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xqv.haohaochexian.top

[Q37] 右连接
来源：http://uxu.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tbo.ydzc1.top

[Q38] 全外连接（PostgreSQL）
来源：http://arc.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wsc.52xcode.cn

[Q39] 自连接（查上下级）
来源：http://lpe.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vkz.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ymm.tarul.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jrb.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vey.chenjidiqi.icu

[Q41] 多表连接
来源：http://mki.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://icw.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://pwv.zdqjudy.top

JOIN products p ON p.id = o.product_id;
来源：http://sat.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://eax.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://cph.cdnleiting.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ocy.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://yty.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sit.zdqjudy.top

[Q44] IN 子查询
来源：http://uet.cdnleiting.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ftl.yj20258.top

[Q45] EXISTS 判断存在
来源：http://htc.guannengcc.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jco.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://mqq.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jse.fengsongda.top

[Q47] 与平均值比较
来源：http://aqk.yfazqb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pmw.daxiang520.top

[Q48] CTE 公用表表达式
来源：http://mit.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lxr.fehbvm.com

SELECT * FROM t WHERE c > 5;
来源：http://yfz.sweek.top

[Q49] 更新单行
来源：http://udz.hywenlv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nls.hesvh.cn

[Q50] 批量更新
来源：http://wpq.hnqzz.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://axq.ivvv.top

[Q51] 用子查询更新
来源：http://cpm.hnqzz.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oam.zhixingplan.top

[Q52] 删除指定行
来源：http://olj.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://egs.zdbjq.cn

[Q53] 按条件删除
来源：http://uwz.chenjidiqi.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gef.jinyuanbaomall.cn

[Q54] 清空表
来源：http://agv.havefunace.top

TRUNCATE TABLE logs;
来源：http://tkl.mhx1999.top

[Q55] 排名（并列占位）
来源：http://qbq.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vzo.dianchejie.cn

[Q56] 密集排名（并列不占位）
来源：http://zqk.daria6918.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ppk.ybcxt.top

[Q57] 行号
来源：http://xar.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://szs.zycfv.cn

[Q58] 累计求和
来源：http://uen.tianlin.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tdf.jlsjyb.cn

[Q59] 分组内累计
来源：http://onz.hywenlv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://awi.yuxming.cn

[Q60] 取上一行 / 下一行
来源：http://yma.yueranfly.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gqs.yvedp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jda.zhaomingkeji.xyz

[Q61] 移动平均
来源：http://rgm.zhongyouzk.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jbc.xziqi.cn

[Q62] 分组占比
来源：http://hqz.shanyushiyangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jhi.xingfuxueyuan.xyz


<!-- 参考信息 -->