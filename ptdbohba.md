代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ncq.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cqg.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vyi.zycfv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ymb.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tyi.ehwqpu.com

[N10] 链表节点定义
来源：http://iso.birdmap.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bqi.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://duw.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sar.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://epa.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://zaw.iojbl.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lus.hywenlv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kgo.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ayd.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://tsy.tarul.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rdc.cheryme.top

PHP:  // 手写递归函数
来源：http://dhl.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://weg.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://amr.zhongyouzk.top

Java: // 手写递归
来源：http://crf.yuxming.cn

Go:   // 手写递归
来源：http://gmb.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kqr.bbcook.cn

C#:   // 手写递归
来源：http://ycu.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qgx.xinyue.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mok.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uxy.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://njz.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://spb.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hxc.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fhs.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bzh.jinqigfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oca.kuanghao11.cn

================================================================================
来源：http://dnx.yj20258.top

O. 并发与异步
来源：http://dzp.haohaochexian.top

================================================================================
来源：http://lai.nanxinkj.top

[O01] 启动一个线程
来源：http://pln.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xxf.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kvo.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vdq.tian-w.cn

TS:   // 同 JS
来源：http://fyz.daria6918.cn

Java: new Thread(() -> f()).start()
来源：http://noj.birdmap.top

Go:   go f()
来源：http://ltk.52xcode.cn

Ruby: Thread.new { f }
来源：http://iep.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://mnp.shzxlz.cn

[O02] 使用线程池
来源：http://xxv.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nmy.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bzg.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://npb.sysykeji.top

TS:   // worker_threads 线程池
来源：http://pdl.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://sad.shzxlz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ebw.aibaodan.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ifa.snrcjt.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ftc.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://vmd.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://qmn.daxiang520.top

PHP:  // 用 flock() 做文件锁
来源：http://psc.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qzh.vehdjk.com

TS:   // 同 JS
来源：http://ysp.yj20258888.top

Java: synchronized (this) { shared++; }
来源：http://whx.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wln.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://oeq.yangfankeji.com

C#:   lock (gate) { shared++; }
来源：http://ref.yj202588.top

[O04] 定义异步函数并等待
来源：http://sja.jiagoushi.top

Py:   async def f():⏎    await g()
来源：http://vhq.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ehl.birdmap.top

JS:   async function f() { await g(); }
来源：http://nbk.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gki.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pyz.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ewn.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tsk.yonumen.top

C#:   async Task F() { await G(); }
来源：http://dbn.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://sks.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://yvc.zhijiandao.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nmb.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://frb.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://voh.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://djt.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hvo.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://ccf.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gds.uphjek.com

[O06] 使用进程池
来源：http://jkt.snrcjt.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jzd.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uta.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://wmi.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://dux.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://prr.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vce.hywenlv.cn

Ruby: // fork 块
来源：http://doc.316326.xyz

C#:   Parallel.For
来源：http://ftd.nanxinkj.top

================================================================================
来源：http://rlq.zycfv.cn

P. 常用工具函数
来源：http://tje.mhx1999.top

================================================================================
来源：http://auf.vehdjk.com

[P01] 生成 UUID
来源：http://qdb.yangfankeji.com

Py:   str(uuid.uuid4())
来源：http://hqo.xingfuxueyuan.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bkj.jinqigfzy.top

JS:   crypto.randomUUID()
来源：http://ycg.c1oappe.top

TS:   crypto.randomUUID()
来源：http://hvd.uphjek.com

Java: UUID.randomUUID().toString()
来源：http://fcm.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://amc.fanxiaobao.xyz

Ruby: SecureRandom.uuid
来源：http://xnr.zhongyouzk.top

C#:   Guid.NewGuid().ToString()
来源：http://iyt.nwbrower.top

[P02] MD5 / SHA256 摘要
来源：http://maw.zhiwuduotai.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nvp.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://epm.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lnd.smart0.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://npq.xuetiantiany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ynr.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ato.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tmi.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gpf.zdqjudy.top

[P03] 生成短随机字符串
来源：http://soj.ydjk.org.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cel.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ilm.shuidangran.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xfn.uphjek.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bzh.nwbrower.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hsk.zhoulong.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dsb.sufxvd.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jdl.jqgfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cjs.smart0.xyz

[P04] 求长度
来源：http://fay.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bvr.iojbl.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qzc.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nzf.cucudq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lmr.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://mvv.hcnkem.com

Go:   len(arr);  len(m)
来源：http://axr.haohaochexian.top

Ruby: x.length;  x.size
来源：http://tyc.hysaishi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vbb.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://pux.wangdashe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ufm.yuanzhike.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rzt.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lak.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xph.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jbn.redwolf501.top

Go:   reflect.DeepEqual(a, b)
来源：http://vmf.nanxinkj.top

Ruby: a == b
来源：http://xpf.sjlbkw.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ffa.sufxvd.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jvn.meibo888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nfr.xinyue.icu

PHP:  if (empty($x)) {}
来源：http://sdq.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vsi.xylfe.cn

TS:   if (x == null) {}
来源：http://icx.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://yyt.shangyingyoupin.top

Go:   if x == nil {}
来源：http://zjh.jinqigfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bfr.wangshuangyany.cn

C#:   if (x is null) {}
来源：http://rkq.chenlongwang.top

[P07] 防抖与节流
来源：http://pur.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zdp.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://mgp.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ukg.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qbp.feifeiyinyue.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rkd.gaohongyu789.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kjm.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://erg.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fmw.shzxlz.cn

[P08] 处理浮点精度问题
来源：http://blv.zdbjq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://efg.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yze.bbcook.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hpr.shanyushiyangtech.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mxn.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sdh.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xsc.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fzh.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ktq.xylfe.cn

================================================================================
来源：http://ygr.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hoo.zycfv.cn

================================================================================
来源：http://cik.fzhhl.top

[Q01] 创建表
来源：http://bcl.jqgfzy.top

CREATE TABLE users (
来源：http://phe.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ftr.aibaodan.cn

name VARCHAR(50) NOT NULL,
来源：http://hvo.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://dbh.yangfankeji.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rfp.jianghu66.top

);
来源：http://wqu.ppjwa.cn

[Q02] 创建带外键的表
来源：http://uie.daria6918.cn

CREATE TABLE orders (
来源：http://fnf.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://txe.dashuyun.cn

user_id INT NOT NULL,
来源：http://vjo.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://iiy.tanke756.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://elb.mhx1999.top

);
来源：http://plp.xinyue.icu

[Q03] 增加列
来源：http://dms.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bcd.sxryk.cn

[Q04] 修改列类型
来源：http://bsf.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jrc.jinyuanbaomall.cn

[Q05] 重命名列
来源：http://zqw.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://chm.ctjpmb.com

[Q06] 删除列
来源：http://boq.316326.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://oik.yonumen.top

[Q07] 删除表
来源：http://ucj.c1oappe.top

DROP TABLE IF EXISTS orders;
来源：http://upw.uphjek.com

[Q08] 创建普通索引
来源：http://fry.nwbrower.top

CREATE INDEX idx_users_email ON users(email);
来源：http://agd.jyoumei.cn

[Q09] 创建唯一索引
来源：http://dgy.jianghu66.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ydt.nwbrower.top

[Q10] 插入单行
来源：http://udr.svipenyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lwr.chenzaomai.com

[Q11] 一次插入多行
来源：http://iny.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ygu.yj202588.top

[Q12] 插入后取自增 ID
来源：http://hgb.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://cqm.ehwqpu.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://icc.snrcjt.cn

[Q13] 忽略重复插入
来源：http://sth.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jfy.daria6918.cn

[Q14] 存在则更新（upsert）
来源：http://ccj.sjlbkw.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://den.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jvj.ehwqpu.com

[Q15] 查询全部
来源：http://xmi.snrcjt.cn

SELECT * FROM users;
来源：http://yev.gzhubu.top

[Q16] 查询指定列
来源：http://vis.ctjpmb.com

SELECT id, name FROM users;
来源：http://rst.fanxiaobao.xyz

[Q17] 条件查询
来源：http://zhe.zdqjudy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cjs.tianlin.xyz

[Q18] 模糊匹配
来源：http://fuw.wangshuangyany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wtj.bjfxy.top

[Q19] 范围查询
来源：http://rec.pengpengdd.cyou

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://geq.zhongyouzk.top

[Q20] IN 列表
来源：http://jmz.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bay.ehwqpu.com

[Q21] 空值判断
来源：http://dtj.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yrs.hammf.cn

[Q22] 排序
来源：http://utw.yj20258.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bzs.smart0.xyz

[Q23] 分页
来源：http://eqe.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xpe.ydzc1.top

[Q24] 去重
来源：http://jyy.zhengqikj.top

SELECT DISTINCT city FROM users;
来源：http://yya.xylfe.cn

[Q25] 只取前 N 条
来源：http://bgh.daxiang520.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fba.hfpthk.cn

[Q26] 计数
来源：http://bzq.tianlin.xyz

SELECT COUNT(*) FROM users;
来源：http://ipx.bbcook.cn

[Q27] 条件计数
来源：http://pwr.smart0.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sqb.316326.xyz

[Q28] 求和与平均
来源：http://inz.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uyx.tarul.cn

[Q29] 最大最小值
来源：http://att.hnqzz.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jdx.sysykeji.top

[Q30] 分组统计
来源：http://lgd.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://har.jinqigufen.top

[Q31] 分组后过滤
来源：http://ytt.daria6918.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sad.52xcode.cn

[Q32] 分组拼接字符串
来源：http://vhq.yueranfly.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mik.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://riq.svipenyu.cn

[Q33] 多列分组
来源：http://pfp.xingfuxueyuan.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://prm.ydjk.org.cn

[Q34] 每组取第一条
来源：http://vsg.tian-w.cn

SELECT * FROM (
来源：http://bxc.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qzv.yfazqb.com

) t WHERE rn = 1;
来源：http://wco.redwolf501.top

[Q35] 内连接
来源：http://foa.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yhn.epnwcf.com

[Q36] 左连接
来源：http://mva.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://smi.jinqigfzy.top

[Q37] 右连接
来源：http://oqw.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://arc.fanxiaobao.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://qie.zhongyouzk.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vdv.ctjpmb.com

[Q39] 自连接（查上下级）
来源：http://yhj.shzxlz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kee.mhx1999.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hpj.ydjk.org.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rgj.chenlongwang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hzb.zhijiandao.cn

[Q41] 多表连接
来源：http://tyv.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vih.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://ayk.zhengqikj.top

JOIN products p ON p.id = o.product_id;
来源：http://izf.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://opy.tanke756.top

SELECT u.name, o.amount FROM users u
来源：http://zav.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qii.yongpay.top

[Q43] 标量子查询
来源：http://wjn.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mpd.pycfn.com

[Q44] IN 子查询
来源：http://arc.bjfxy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xvw.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://hpc.meibo888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://shd.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://foh.sweek.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zcs.nanxinkj.top

[Q47] 与平均值比较
来源：http://nlc.tarul.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cms.kuanghao11.cn

[Q48] CTE 公用表表达式
来源：http://jai.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://voe.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://mys.guowangkeji.top

[Q49] 更新单行
来源：http://ekh.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iuj.birdmap.top

[Q50] 批量更新
来源：http://ccw.hammf.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zgz.yuanzhike.top

[Q51] 用子查询更新
来源：http://nby.gogol.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oim.316326.xyz

[Q52] 删除指定行
来源：http://pcr.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://jux.aibaodan.cn

[Q53] 按条件删除
来源：http://lfb.9152youxi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kkw.daria6918.cn

[Q54] 清空表
来源：http://dcj.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://lyn.tanke756.top

[Q55] 排名（并列占位）
来源：http://wmi.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://erb.yj20258888.top

[Q56] 密集排名（并列不占位）
来源：http://iwr.jlsjyb.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://czc.zhiwuduotai.top

[Q57] 行号
来源：http://ydh.hfpthk.cn


<!-- 参考信息 -->