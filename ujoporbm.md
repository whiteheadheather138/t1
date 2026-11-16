代发 wailian999

Go:   // 手写递归
来源：http://oos.sufxvd.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kml.zhaomingkeji.xyz

C#:   // 手写递归
来源：http://wgy.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rfz.zdqjudy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://khe.smart0.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ccl.yfazqb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mhv.cheryme.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lbe.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qvi.daria6918.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://agi.fehbvm.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xxj.hammf.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xwk.yvedp.cn

================================================================================
来源：http://soh.yfazqb.com

O. 并发与异步
来源：http://now.shuidangran.top

================================================================================
来源：http://tpc.xinyue.icu

[O01] 启动一个线程
来源：http://xgm.jqgufenzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ngn.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yde.xuanzx.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fba.gzhubu.top

TS:   // 同 JS
来源：http://sxy.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://vqi.yj20258888.top

Go:   go f()
来源：http://sai.daxiang520.top

Ruby: Thread.new { f }
来源：http://rpt.jinqigufen.top

C#:   Task.Run(() => F());
来源：http://rzh.chenlongwang.top

[O02] 使用线程池
来源：http://ywo.hysaishi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jhu.zhengqikj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://erh.52xcode.cn

JS:   // worker_threads 线程池
来源：http://elu.yj20258888.top

TS:   // worker_threads 线程池
来源：http://fip.haohaochexian.top

Java: Executors.newFixedThreadPool(4)
来源：http://tns.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kfz.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ykl.0kj1m.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://svq.aibaodan.cn

[O03] 加锁保护共享数据
来源：http://hgd.shuidangran.top

Py:   with lock: shared += 1
来源：http://nnh.zhijiandao.cn

PHP:  // 用 flock() 做文件锁
来源：http://jtw.jyoumei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fvb.ivvv.top

TS:   // 同 JS
来源：http://yrp.dianchejie.cn

Java: synchronized (this) { shared++; }
来源：http://cco.uphjek.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ajy.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://fgd.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://vdo.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://aps.ywan-chungtsiang.top

Py:   async def f():⏎    await g()
来源：http://msy.jqgufenzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vvn.tanke756.top

JS:   async function f() { await g(); }
来源：http://ume.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ssb.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ojw.snrcjt.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vdk.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://ngd.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://vqr.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://dcg.svipenyu.cn

Py:   asyncio.gather(*tasks)
来源：http://nzx.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ive.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://yvt.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://spl.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fvw.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ynz.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://kmt.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tzp.tanke756.top

[O06] 使用进程池
来源：http://ajy.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://huj.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nah.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://hnf.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://qxv.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fdx.tarul.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ics.jinqigufen.top

Ruby: // fork 块
来源：http://ere.smart0.xyz

C#:   Parallel.For
来源：http://rlt.nwbrower.top

================================================================================
来源：http://kps.cheryme.top

P. 常用工具函数
来源：http://roe.xingfuxueyuan.xyz

================================================================================
来源：http://lhk.aizwys.cn

[P01] 生成 UUID
来源：http://yxm.birdmap.top

Py:   str(uuid.uuid4())
来源：http://zrj.iojbl.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tlr.hfpthk.cn

JS:   crypto.randomUUID()
来源：http://vyt.smart0.xyz

TS:   crypto.randomUUID()
来源：http://lak.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://xox.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://oet.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://cga.hongshengwenyu.top

C#:   Guid.NewGuid().ToString()
来源：http://jqs.jiagoushi.top

[P02] MD5 / SHA256 摘要
来源：http://wfo.hnxiangtu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gdi.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sug.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wdw.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yit.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iwd.ivvv.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tcf.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nnz.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://efw.gzhubu.top

[P03] 生成短随机字符串
来源：http://imk.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mcx.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jjo.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tby.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jem.hfpthk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zit.zhixingplan.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ime.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ozl.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wme.haohaochexian.top

[P04] 求长度
来源：http://ofj.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rle.shzxlz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ort.sjlbkw.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uvg.jinqigfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zxr.52xcode.cn

Java: list.size();  map.size();  s.length()
来源：http://qgp.zhoulong.xyz

Go:   len(arr);  len(m)
来源：http://pmi.52xcode.cn

Ruby: x.length;  x.size
来源：http://suy.tian-w.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gki.yangfankeji.com

[P05] 判断两个对象内容是否相等
来源：http://qka.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://quo.yongpay.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vpc.mhx1999.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xtn.dashuyun.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://udo.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ash.yueranfly.top

Go:   reflect.DeepEqual(a, b)
来源：http://nja.shanyushiyangtech.top

Ruby: a == b
来源：http://djz.sufxvd.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lqq.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pzo.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://anh.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://yyv.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jug.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://vdq.fktsv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cth.52xcode.cn

Go:   if x == nil {}
来源：http://gpy.yongpay.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hcr.fengsongda.top

C#:   if (x is null) {}
来源：http://rlz.ctjpmb.com

[P07] 防抖与节流
来源：http://ucu.snrcjt.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uzy.tian-w.cn

PHP:  // 手写时间戳比较
来源：http://sdg.jinqigfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jqy.tanke756.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://phl.gzhubu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ooi.guowangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://btq.9152youxi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fvd.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://esi.svipenyu.cn

[P08] 处理浮点精度问题
来源：http://xqa.jinyuanbaomall.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ngm.chenlongwang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://frl.epnwcf.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://auc.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hsh.xziqi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://emd.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wam.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ktp.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jkk.jiagoushi.top

================================================================================
来源：http://gxr.ehwqpu.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nth.hywenlv.cn

================================================================================
来源：http://pzy.c1oappe.top

[Q01] 创建表
来源：http://qyw.vqdsnc.cn

CREATE TABLE users (
来源：http://pnd.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bmg.zhaomingkeji.xyz

name VARCHAR(50) NOT NULL,
来源：http://wan.cdnleiting.top

email VARCHAR(100) UNIQUE,
来源：http://kgr.svipenyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yiz.tian-w.cn

);
来源：http://glp.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://xfi.zdqjudy.top

CREATE TABLE orders (
来源：http://nmm.ehwqpu.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fju.bbcook.cn

user_id INT NOT NULL,
来源：http://ioc.quarkkingdee.top

amount DECIMAL(10, 2),
来源：http://nea.fzhhl.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kzz.yvedp.cn

);
来源：http://app.birdmap.top

[Q03] 增加列
来源：http://ujo.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zty.wangdashe.top

[Q04] 修改列类型
来源：http://rox.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ycf.fengsongda.top

[Q05] 重命名列
来源：http://mps.jinqigufen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qga.shanyushiyangtech.top

[Q06] 删除列
来源：http://yml.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://qyt.jqgfzy.top

[Q07] 删除表
来源：http://vob.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://vey.aizwys.cn

[Q08] 创建普通索引
来源：http://hab.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://owt.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://csy.ppjwa.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yja.gaohongyu789.top

[Q10] 插入单行
来源：http://lqk.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ofc.jinqigufen.top

[Q11] 一次插入多行
来源：http://jbl.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nri.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://wem.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://isf.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cgr.ppjwa.cn

[Q13] 忽略重复插入
来源：http://kla.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hua.iojbl.cn

[Q14] 存在则更新（upsert）
来源：http://vaq.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ank.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pvb.chenzaomai.com

[Q15] 查询全部
来源：http://djj.yj20258.top

SELECT * FROM users;
来源：http://tcc.gogol.net.cn

[Q16] 查询指定列
来源：http://hlr.tian-w.cn

SELECT id, name FROM users;
来源：http://qfb.ydjk.org.cn

[Q17] 条件查询
来源：http://dmo.hnxiangtu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uts.cheryme.top

[Q18] 模糊匹配
来源：http://auv.haohaochexian.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mxs.yfazqb.com

[Q19] 范围查询
来源：http://jqo.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wkh.svipenyu.cn

[Q20] IN 列表
来源：http://eey.hongshengwenyu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rgk.gogol.net.cn

[Q21] 空值判断
来源：http://yaf.yanxiufei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ooy.9152youxi.cn

[Q22] 排序
来源：http://lwz.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fuo.hammf.cn

[Q23] 分页
来源：http://agu.dianchejie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vgq.pycfn.com

[Q24] 去重
来源：http://dlv.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://rla.yj20258888.top

[Q25] 只取前 N 条
来源：http://bbk.0kj1m.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tog.hnqzz.top

[Q26] 计数
来源：http://fny.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://nzt.jianghu66.top

[Q27] 条件计数
来源：http://iak.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fvh.xuanzx.com

[Q28] 求和与平均
来源：http://shf.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://buf.hcnkem.com

[Q29] 最大最小值
来源：http://imi.gotoacloud.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tjg.cheryme.top

[Q30] 分组统计
来源：http://eyf.gaohongyu789.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ohv.zdqjudy.top

[Q31] 分组后过滤
来源：http://lxe.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nsc.52xcode.cn

[Q32] 分组拼接字符串
来源：http://efo.chenzaomai.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://olp.fengsongda.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://upb.zhiwuduotai.top

[Q33] 多列分组
来源：http://yiw.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://frc.0kj1m.cn

[Q34] 每组取第一条
来源：http://dgd.xylfe.cn

SELECT * FROM (
来源：http://wzl.hnxiangtu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tdb.316326.xyz

) t WHERE rn = 1;
来源：http://kwv.ppjwa.cn

[Q35] 内连接
来源：http://obg.fehbvm.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fhe.52xcode.cn

[Q36] 左连接
来源：http://poo.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://exp.yj20258888.top

[Q37] 右连接
来源：http://czo.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yao.wangshuangyany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jpy.jinghuilouyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ctx.hnqzz.top

[Q39] 自连接（查上下级）
来源：http://hcu.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lar.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://epu.uphjek.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ebp.zhongyouzk.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rrt.zhiwuduotai.top

[Q41] 多表连接
来源：http://dae.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ivl.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://iqh.yj20258.top

JOIN products p ON p.id = o.product_id;
来源：http://vul.xziqi.cn

[Q42] 连接条件附加过滤
来源：http://rkc.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://vod.yuanzhike.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nbu.sweek.top

[Q43] 标量子查询
来源：http://qra.jinqigfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nll.ydzc1.top

[Q44] IN 子查询
来源：http://gcd.yfazqb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wxy.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://cpk.dianchejie.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uef.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ehq.hysaishi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kmt.bbcook.cn

[Q47] 与平均值比较
来源：http://jgr.jqgfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kkj.cdnleiting.top

[Q48] CTE 公用表表达式
来源：http://jif.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nod.cdnleiting.top

SELECT * FROM t WHERE c > 5;
来源：http://wem.redwolf501.top

[Q49] 更新单行
来源：http://lgf.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pcp.jinqigfzy.top

[Q50] 批量更新
来源：http://ybf.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kqx.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://ofx.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bmw.jqgufenzy.top

[Q52] 删除指定行
来源：http://cuq.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://zyl.birdmap.top

[Q53] 按条件删除
来源：http://dlv.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rss.fktsv.cn

[Q54] 清空表
来源：http://uvf.cashguo.top

TRUNCATE TABLE logs;
来源：http://eln.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://yrw.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hyz.ppjwa.cn

[Q56] 密集排名（并列不占位）
来源：http://hie.pengpengdd.cyou

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mtz.0kj1m.cn

[Q57] 行号
来源：http://hsd.cdnleiting.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dhi.fengsongda.top

[Q58] 累计求和
来源：http://bnr.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lek.zhongyouzk.top

[Q59] 分组内累计
来源：http://hqg.yanxiufei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gco.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://bso.sweek.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://agb.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xod.tianlin.xyz

[Q61] 移动平均
来源：http://koh.ehwqpu.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zmk.yongpay.top

[Q62] 分组占比
来源：http://qyu.andypj.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xpo.c1oappe.top

[Q63] 开启事务
来源：http://gst.wangdashe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zcx.gogol.net.cn

[Q64] 提交事务
来源：http://bcr.yuanzhike.top

COMMIT;
来源：http://dnf.zhixingplan.top

[Q65] 回滚事务
来源：http://aog.haohaochexian.top

ROLLBACK;
来源：http://lgl.yanxiufei.cn

[Q66] 行锁查询
来源：http://gtr.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dsf.zhongyouzk.top


<!-- 参考信息 -->