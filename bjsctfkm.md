代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yqi.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dcw.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://bfz.gzhubu.top

Go:   type Node struct { V int; Next *Node }
来源：http://hgn.svipenyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nxf.yanxiufei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sed.wangdashe.top

[N11] 二叉树中序遍历
来源：http://jmo.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ffj.xuanzx.com

PHP:  // 手写递归函数
来源：http://bzt.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fxh.jinqigufen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yid.yj20258.top

Java: // 手写递归
来源：http://jfy.xylfe.cn

Go:   // 手写递归
来源：http://wzc.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cli.hfpthk.cn

C#:   // 手写递归
来源：http://zrq.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ooa.zdbjq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nps.nanxuanxn.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dly.feifeiyinyue.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jme.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wwc.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wdu.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://giu.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tee.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rxa.birdmap.top

================================================================================
来源：http://nbv.hammf.cn

O. 并发与异步
来源：http://bgz.yj202588.top

================================================================================
来源：http://fuh.ctjpmb.com

[O01] 启动一个线程
来源：http://luk.wangdashe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kuj.52xcode.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sde.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mcu.zycfv.cn

TS:   // 同 JS
来源：http://pql.chenzaomai.com

Java: new Thread(() -> f()).start()
来源：http://cyk.havefunace.top

Go:   go f()
来源：http://zad.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://ixp.zhiwuduotai.top

C#:   Task.Run(() => F());
来源：http://xyw.chenzaomai.com

[O02] 使用线程池
来源：http://cbo.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zby.9152youxi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lbv.meibo888.top

JS:   // worker_threads 线程池
来源：http://exl.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://sun.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rin.yj20258888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mei.xuetiantiany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cqs.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gix.shuidangran.top

[O03] 加锁保护共享数据
来源：http://ffx.0kj1m.cn

Py:   with lock: shared += 1
来源：http://fcy.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://lho.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://igp.mhx1999.top

TS:   // 同 JS
来源：http://inm.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://qot.gaohongyu789.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wsr.tianlin.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://ghf.quarkkingdee.top

C#:   lock (gate) { shared++; }
来源：http://mpv.zhijiandao.cn

[O04] 定义异步函数并等待
来源：http://swa.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://xdw.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ysc.yuxming.cn

JS:   async function f() { await g(); }
来源：http://ady.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mfl.havefunace.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ovv.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cdz.xziqi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zcv.zhixingplan.top

C#:   async Task F() { await G(); }
来源：http://hor.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://gpk.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://ihx.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ctu.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://kpy.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://ipb.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://itk.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://omv.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://dwx.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jjc.ywan-chungtsiang.top

[O06] 使用进程池
来源：http://vyi.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bnv.hywenlv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hom.uphjek.com

JS:   // child_process / cluster 模块
来源：http://xqg.dashuyun.cn

TS:   // child_process / cluster 模块
来源：http://daz.mhx1999.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qfe.chenjidiqi.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fvk.shangyingyoupin.top

Ruby: // fork 块
来源：http://spx.sysykeji.top

C#:   Parallel.For
来源：http://eej.iojbl.cn

================================================================================
来源：http://wxo.yj20258888.top

P. 常用工具函数
来源：http://bbn.xingfuxueyuan.xyz

================================================================================
来源：http://gqj.yonumen.top

[P01] 生成 UUID
来源：http://sen.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://hsi.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sgu.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://kqf.birdmap.top

TS:   crypto.randomUUID()
来源：http://oka.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://szg.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://vfd.zdqjudy.top

Ruby: SecureRandom.uuid
来源：http://ygg.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://ron.iojbl.cn

[P02] MD5 / SHA256 摘要
来源：http://pyc.jyoumei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jyq.hammf.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dgg.zhongyouzk.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eqh.xuanzx.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wuq.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zcx.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wqz.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hvg.sysykeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ilw.gzhubu.top

[P03] 生成短随机字符串
来源：http://jmb.jianghu66.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vsr.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://reo.smart0.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://myt.ywan-chungtsiang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rpt.daxiang520.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://odf.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gfq.jinqigufen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sqv.bbcook.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eyo.xingfuxueyuan.xyz

[P04] 求长度
来源：http://jli.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jww.hammf.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tmb.wangdashe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://isn.mhx1999.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vpv.hammf.cn

Java: list.size();  map.size();  s.length()
来源：http://uuo.0kj1m.cn

Go:   len(arr);  len(m)
来源：http://txi.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://pse.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qae.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://gop.fktsv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://arp.hnqzz.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://whj.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rdl.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lgf.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xwp.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://keh.vqdsnc.cn

Ruby: a == b
来源：http://vre.cucudq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aqq.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xgr.jqgufenzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ulb.yangfankeji.com

PHP:  if (empty($x)) {}
来源：http://lsy.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eus.wangdashe.top

TS:   if (x == null) {}
来源：http://cga.hywenlv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nkt.fzhhl.top

Go:   if x == nil {}
来源：http://ehp.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fgg.sweek.top

C#:   if (x is null) {}
来源：http://wgv.gzhubu.top

[P07] 防抖与节流
来源：http://wmj.jiagoushi.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://her.hysaishi.cn

PHP:  // 手写时间戳比较
来源：http://mpg.c1oappe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bpa.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lrb.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hde.tianlin.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qsx.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tza.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ynj.shzxlz.cn

[P08] 处理浮点精度问题
来源：http://qfi.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xfy.fanxiaobao.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gez.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iuh.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://roa.hongshengwenyu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yub.quarkkingdee.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pvh.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://etp.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uwo.kuanghao11.cn

================================================================================
来源：http://uam.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://krn.sweek.top

================================================================================
来源：http://cvz.shanyushiyangkeji.top

[Q01] 创建表
来源：http://ehe.chenjidiqi.icu

CREATE TABLE users (
来源：http://swl.gogol.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ypl.sweek.top

name VARCHAR(50) NOT NULL,
来源：http://ywd.fktsv.cn

email VARCHAR(100) UNIQUE,
来源：http://yel.tarul.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zqc.pycfn.com

);
来源：http://pqm.316326.xyz

[Q02] 创建带外键的表
来源：http://mqj.vehdjk.com

CREATE TABLE orders (
来源：http://smy.jyoumei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xlx.hfpthk.cn

user_id INT NOT NULL,
来源：http://gki.zycfv.cn

amount DECIMAL(10, 2),
来源：http://uyu.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cxx.cashguo.top

);
来源：http://tyb.316326.xyz

[Q03] 增加列
来源：http://doz.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hvp.yj20258888.top

[Q04] 修改列类型
来源：http://pmf.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://htl.c1oappe.top

[Q05] 重命名列
来源：http://kgl.yuxming.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fyb.hnxiangtu.top

[Q06] 删除列
来源：http://mxx.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://ton.daxiang520.top

[Q07] 删除表
来源：http://bkk.jianghu66.top

DROP TABLE IF EXISTS orders;
来源：http://nnt.ydzc1.top

[Q08] 创建普通索引
来源：http://brm.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://kky.gaohongyu789.top

[Q09] 创建唯一索引
来源：http://bif.gotoacloud.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kim.mhx1999.top

[Q10] 插入单行
来源：http://qdy.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ysd.svipenyu.cn

[Q11] 一次插入多行
来源：http://bsz.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ogb.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://ybb.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dte.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bcf.52xcode.cn

[Q13] 忽略重复插入
来源：http://iiq.xziqi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://huo.cashguo.top

[Q14] 存在则更新（upsert）
来源：http://lok.gaohongyu789.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pwc.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hvp.xinyue.icu

[Q15] 查询全部
来源：http://ozi.guowangkeji.top

SELECT * FROM users;
来源：http://biz.yueranfly.top

[Q16] 查询指定列
来源：http://mhg.ppjwa.cn

SELECT id, name FROM users;
来源：http://kic.fktsv.cn

[Q17] 条件查询
来源：http://mpe.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wdd.yongpay.top

[Q18] 模糊匹配
来源：http://bxb.nanxuanxn.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gwb.hcnkem.com

[Q19] 范围查询
来源：http://wqt.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sod.dashuyun.cn

[Q20] IN 列表
来源：http://pyt.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://khd.yj20258.top

[Q21] 空值判断
来源：http://que.jianghu66.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zza.hnqzz.top

[Q22] 排序
来源：http://irb.fzhhl.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bto.svipenyu.cn

[Q23] 分页
来源：http://uyr.uphjek.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uik.zhijiandao.cn

[Q24] 去重
来源：http://frc.yongpay.top

SELECT DISTINCT city FROM users;
来源：http://dqr.dashuyun.cn

[Q25] 只取前 N 条
来源：http://eqs.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dnf.jyoumei.cn

[Q26] 计数
来源：http://jxq.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://svd.pengpengdd.cyou

[Q27] 条件计数
来源：http://vil.zdbjq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fam.xuanzx.com

[Q28] 求和与平均
来源：http://enh.shanyushiyangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mxt.birdmap.top

[Q29] 最大最小值
来源：http://fwa.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xzv.xuetiantiany.cn

[Q30] 分组统计
来源：http://yux.shzxlz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rhg.316326.xyz

[Q31] 分组后过滤
来源：http://cih.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ufv.shuidangran.top

[Q32] 分组拼接字符串
来源：http://ujj.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rel.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pvs.yuxming.cn

[Q33] 多列分组
来源：http://xda.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ijo.sxryk.cn

[Q34] 每组取第一条
来源：http://dbv.birdmap.top

SELECT * FROM (
来源：http://iun.316326.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aln.vqdsnc.cn

) t WHERE rn = 1;
来源：http://bwt.pengpengdd.cyou

[Q35] 内连接
来源：http://urg.nwbrower.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aff.jiagoushi.top

[Q36] 左连接
来源：http://twi.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://leo.zhijiandao.cn

[Q37] 右连接
来源：http://tvm.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://onf.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://slz.aizwys.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fcs.yongpay.top

[Q39] 自连接（查上下级）
来源：http://wha.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tbi.52xcode.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mej.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nnf.hnxiangtu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vte.chenlongwang.top

[Q41] 多表连接
来源：http://fms.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rkh.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://uqm.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://oiz.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://jcm.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://apc.hammf.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lvj.aizwys.cn

[Q43] 标量子查询
来源：http://yav.zhiwuduotai.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://byf.nanxinkj.top

[Q44] IN 子查询
来源：http://rvp.mhx1999.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://osu.yongpay.top

[Q45] EXISTS 判断存在
来源：http://jvw.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jsa.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://qvg.iojbl.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fcx.andypj.xyz

[Q47] 与平均值比较
来源：http://kwd.hesvh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mda.nanxuanxn.top

[Q48] CTE 公用表表达式
来源：http://vbo.gogol.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eey.hfpthk.cn

SELECT * FROM t WHERE c > 5;
来源：http://vuv.zdbjq.cn

[Q49] 更新单行
来源：http://bsz.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oib.chenlongwang.top

[Q50] 批量更新
来源：http://rpz.jinghuilouyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sdu.yuxming.cn

[Q51] 用子查询更新
来源：http://hwb.pycfn.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pul.ywan-chungtsiang.top

[Q52] 删除指定行
来源：http://gkx.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://cvc.zhixingplan.top

[Q53] 按条件删除
来源：http://bcm.jinqigufen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ajc.shangyingyoupin.top

[Q54] 清空表
来源：http://pft.316326.xyz

TRUNCATE TABLE logs;
来源：http://rzk.316326.xyz

[Q55] 排名（并列占位）
来源：http://nlh.dianchejie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wxk.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://olu.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bjy.zhixingplan.top

[Q57] 行号
来源：http://rbk.ctjpmb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qhx.quarkkingdee.top

[Q58] 累计求和
来源：http://bnv.yfazqb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yhq.tianlin.xyz

[Q59] 分组内累计
来源：http://rzr.uphjek.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vrh.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://gyr.shangyingyoupin.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bac.pengpengdd.cyou

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zya.sysykeji.top


<!-- 参考信息 -->