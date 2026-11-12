代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://pso.gzhubu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qwu.tanke756.top

[N11] 二叉树中序遍历
来源：http://fcg.ivvv.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dew.hongshengwenyu.top

PHP:  // 手写递归函数
来源：http://axk.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ior.ydzc1.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xcq.dianchejie.cn

Java: // 手写递归
来源：http://wuv.dashuyun.cn

Go:   // 手写递归
来源：http://wxt.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rzk.xinyue.icu

C#:   // 手写递归
来源：http://ycm.jinghuilouyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yjs.yanxiufei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jkh.shuidangran.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jng.shangyingyoupin.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://foh.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tvo.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sgp.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tje.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ngu.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://czw.nanxinkj.top

================================================================================
来源：http://tsm.cheryme.top

O. 并发与异步
来源：http://dts.hywenlv.cn

================================================================================
来源：http://zms.jiagoushi.top

[O01] 启动一个线程
来源：http://qbj.hesvh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fyd.chenjidiqi.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zqy.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hzq.zdbjq.cn

TS:   // 同 JS
来源：http://lnp.0kj1m.cn

Java: new Thread(() -> f()).start()
来源：http://ili.mhx1999.top

Go:   go f()
来源：http://nmy.sufxvd.cn

Ruby: Thread.new { f }
来源：http://khk.zycfv.cn

C#:   Task.Run(() => F());
来源：http://riq.hnxiangtu.top

[O02] 使用线程池
来源：http://stz.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fec.cdnleiting.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xqc.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://zmv.hfpthk.cn

TS:   // worker_threads 线程池
来源：http://dfc.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yak.birdmap.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ptk.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kjp.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rdz.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://eeg.zhongyouzk.top

Py:   with lock: shared += 1
来源：http://kuw.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://pkd.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dxj.yuanzhike.top

TS:   // 同 JS
来源：http://vnt.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://jvb.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jrw.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://dtw.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://ncv.feifeiyinyue.top

[O04] 定义异步函数并等待
来源：http://knz.xingfuxueyuan.xyz

Py:   async def f():⏎    await g()
来源：http://dpq.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hau.hongshengwenyu.top

JS:   async function f() { await g(); }
来源：http://gua.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://inm.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oey.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bbj.yonumen.top

Ruby: # 用 Fiber 或 async gem
来源：http://xdp.redwolf501.top

C#:   async Task F() { await G(); }
来源：http://qyd.nwbrower.top

[O05] 并发执行并等待全部完成
来源：http://jin.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://doa.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pgw.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://xgh.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://ybq.mhx1999.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xan.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dvk.nanxinkj.top

Ruby: threads.map(&:join)
来源：http://ion.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://naq.jinqigfzy.top

[O06] 使用进程池
来源：http://tpd.aibaodan.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qio.xuetiantiany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zph.zhijiandao.cn

JS:   // child_process / cluster 模块
来源：http://lyv.316326.xyz

TS:   // child_process / cluster 模块
来源：http://bnc.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://svm.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mqo.kuanghao11.cn

Ruby: // fork 块
来源：http://ukd.wangshuangyany.cn

C#:   Parallel.For
来源：http://yfp.jyoumei.cn

================================================================================
来源：http://pbc.gzhubu.top

P. 常用工具函数
来源：http://rze.jinyuanbaomall.cn

================================================================================
来源：http://ujn.chenlongwang.top

[P01] 生成 UUID
来源：http://anw.tarul.cn

Py:   str(uuid.uuid4())
来源：http://jpa.tianlin.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nag.mhx1999.top

JS:   crypto.randomUUID()
来源：http://rpc.cheryme.top

TS:   crypto.randomUUID()
来源：http://qgs.yangfankeji.com

Java: UUID.randomUUID().toString()
来源：http://kxt.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://dia.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://dlj.shanyushiyangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://jbm.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://lsp.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nio.fanxiaobao.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://nxn.zycfv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://glm.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://udk.vehdjk.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mwz.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bgj.iojbl.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://shq.zhijiandao.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kem.quarkkingdee.top

[P03] 生成短随机字符串
来源：http://igw.jinghuilouyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fva.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://twp.jinqigfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://shh.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ujx.yuanzhike.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fcs.xuetiantiany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ybd.meibo888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cln.ehwqpu.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vsu.fzhhl.top

[P04] 求长度
来源：http://fld.yueranfly.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xmc.xuetiantiany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ejy.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cnt.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vci.jinqigfzy.top

Java: list.size();  map.size();  s.length()
来源：http://acw.tarul.cn

Go:   len(arr);  len(m)
来源：http://hyd.epnwcf.com

Ruby: x.length;  x.size
来源：http://hqz.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://suk.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://qgn.yfazqb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://taf.haohaochexian.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eht.meibo888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ejr.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oha.jyoumei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eoq.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://nvd.yj20258.top

Ruby: a == b
来源：http://nhe.jqgfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fsm.cucudq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zns.wangshuangyany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jrf.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://aqq.yangfankeji.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kxw.fanxiaobao.xyz

TS:   if (x == null) {}
来源：http://vav.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://baj.hongshengwenyu.top

Go:   if x == nil {}
来源：http://cud.cqqwz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hmo.ppjwa.cn

C#:   if (x is null) {}
来源：http://sdd.52xcode.cn

[P07] 防抖与节流
来源：http://xmq.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rtf.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://gny.dianchejie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zkm.cdnleiting.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nzb.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nks.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jdj.ctjpmb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://zpi.yvedp.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://htg.haohaochexian.top

[P08] 处理浮点精度问题
来源：http://idq.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cre.gogol.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sgj.hysaishi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aid.ehwqpu.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tay.52xcode.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lvg.sjlbkw.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yir.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xte.snrcjt.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xia.meibo888.top

================================================================================
来源：http://dog.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qcq.sjlbkw.cn

================================================================================
来源：http://joy.guannengcc.top

[Q01] 创建表
来源：http://mgk.yuxming.cn

CREATE TABLE users (
来源：http://mhx.fzhhl.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bdd.zdqjudy.top

name VARCHAR(50) NOT NULL,
来源：http://sbl.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://jjp.ppjwa.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://val.fengsongda.top

);
来源：http://zkz.bjfxy.top

[Q02] 创建带外键的表
来源：http://ast.cqqwz.cn

CREATE TABLE orders (
来源：http://ndg.vehdjk.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gik.gogol.net.cn

user_id INT NOT NULL,
来源：http://ofo.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://syn.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://azw.316326.xyz

);
来源：http://tqy.hammf.cn

[Q03] 增加列
来源：http://jts.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rnf.jqgufenzy.top

[Q04] 修改列类型
来源：http://mkr.ehwqpu.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dvl.yanxiufei.cn

[Q05] 重命名列
来源：http://ecy.vqdsnc.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gyk.9152youxi.cn

[Q06] 删除列
来源：http://jxm.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://xkf.sufxvd.cn

[Q07] 删除表
来源：http://xdx.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://ulm.epnwcf.com

[Q08] 创建普通索引
来源：http://irp.nwbrower.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hqy.aibaodan.cn

[Q09] 创建唯一索引
来源：http://yte.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cvr.iojbl.cn

[Q10] 插入单行
来源：http://dqh.shuidangran.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xrs.bjfxy.top

[Q11] 一次插入多行
来源：http://jsm.bbcook.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oqd.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://lbs.yfazqb.com

INSERT INTO users (name) VALUES ('C');
来源：http://fqm.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hvg.cdnleiting.top

[Q13] 忽略重复插入
来源：http://squ.dashuyun.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tqf.jiagoushi.top

[Q14] 存在则更新（upsert）
来源：http://fuj.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ndr.hongshengwenyu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uoq.zhongyouzk.top

[Q15] 查询全部
来源：http://hpw.xuetiantiany.cn

SELECT * FROM users;
来源：http://tbi.jyoumei.cn

[Q16] 查询指定列
来源：http://hpo.cheryme.top

SELECT id, name FROM users;
来源：http://awh.hesvh.cn

[Q17] 条件查询
来源：http://fot.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dmm.wangshuangyany.cn

[Q18] 模糊匹配
来源：http://mex.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jcb.fengsongda.top

[Q19] 范围查询
来源：http://jnr.yueranfly.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tri.sufxvd.cn

[Q20] IN 列表
来源：http://dss.nanxinkj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pff.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://ijj.chenlongwang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://omy.jqgfzy.top

[Q22] 排序
来源：http://tna.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dye.pycfn.com

[Q23] 分页
来源：http://kln.zhoulong.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cup.shangyingyoupin.top

[Q24] 去重
来源：http://vjw.gogol.net.cn

SELECT DISTINCT city FROM users;
来源：http://agy.9152youxi.cn

[Q25] 只取前 N 条
来源：http://lys.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aqi.kuanghao11.cn

[Q26] 计数
来源：http://nbh.yueranfly.top

SELECT COUNT(*) FROM users;
来源：http://mkz.smart0.xyz

[Q27] 条件计数
来源：http://vpw.epnwcf.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gca.hcnkem.com

[Q28] 求和与平均
来源：http://lwj.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://woa.ydjk.org.cn

[Q29] 最大最小值
来源：http://ida.zhixingplan.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jcy.shanyushiyangtech.top

[Q30] 分组统计
来源：http://fdf.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mkf.bbcook.cn

[Q31] 分组后过滤
来源：http://tci.ctjpmb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vwl.havefunace.top

[Q32] 分组拼接字符串
来源：http://qer.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://azy.chenzaomai.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://esi.uphjek.com

[Q33] 多列分组
来源：http://dfc.vqdsnc.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xsf.dashuyun.cn

[Q34] 每组取第一条
来源：http://mcn.daria6918.cn

SELECT * FROM (
来源：http://kqb.cheryme.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ccg.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://aoz.yj202588.top

[Q35] 内连接
来源：http://tbq.yueranfly.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mle.guowangkeji.top

[Q36] 左连接
来源：http://odw.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bax.gzhubu.top

[Q37] 右连接
来源：http://jie.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uwk.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zpn.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gmq.yongpay.top

[Q39] 自连接（查上下级）
来源：http://god.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jvf.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ttw.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zdx.sysykeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bzq.guowangkeji.top

[Q41] 多表连接
来源：http://vjv.hfpthk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lbg.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://anr.yvedp.cn

JOIN products p ON p.id = o.product_id;
来源：http://lrh.dianchejie.cn

[Q42] 连接条件附加过滤
来源：http://ggs.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://ctx.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://txt.yvedp.cn

[Q43] 标量子查询
来源：http://nru.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yfy.tarul.cn

[Q44] IN 子查询
来源：http://mtn.vqdsnc.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bnb.chenlongwang.top

[Q45] EXISTS 判断存在
来源：http://ike.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vui.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://svh.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fie.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://mju.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dyt.jianghu66.top

[Q48] CTE 公用表表达式
来源：http://qeq.ybcxt.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qye.yvedp.cn

SELECT * FROM t WHERE c > 5;
来源：http://xbp.jyoumei.cn

[Q49] 更新单行
来源：http://wds.jianghu66.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gmi.pengpengdd.cyou

[Q50] 批量更新
来源：http://yig.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jsp.epnwcf.com

[Q51] 用子查询更新
来源：http://eft.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mtf.bbcook.cn

[Q52] 删除指定行
来源：http://her.cheryme.top

DELETE FROM users WHERE id = 10;
来源：http://cho.ppjwa.cn

[Q53] 按条件删除
来源：http://cjq.nanxinkj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ehu.jianghu66.top

[Q54] 清空表
来源：http://qpp.ivvv.top

TRUNCATE TABLE logs;
来源：http://isq.cheryme.top

[Q55] 排名（并列占位）
来源：http://ggc.jinghuilouyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kfj.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://bxe.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jox.jinqigfzy.top

[Q57] 行号
来源：http://hva.zhiwuduotai.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fvl.sxryk.cn

[Q58] 累计求和
来源：http://ktz.zhaomingkeji.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bfb.daxiang520.top

[Q59] 分组内累计
来源：http://eci.pycfn.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pem.yonumen.top

[Q60] 取上一行 / 下一行
来源：http://xhh.jinqigufen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dzd.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fxs.yongpay.top

[Q61] 移动平均
来源：http://tmr.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xmj.gzhubu.top

[Q62] 分组占比
来源：http://zjo.jiagoushi.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sju.pengpengdd.cyou


<!-- 参考信息 -->