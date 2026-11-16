代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://svg.ydzc1.top

[N10] 链表节点定义
来源：http://yfs.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://etq.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rrx.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ofa.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jug.yuxming.cn

Java: class Node { int v; Node next; }
来源：http://npg.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://qdw.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fbx.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xbd.birdmap.top

[N11] 二叉树中序遍历
来源：http://sji.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dec.0kj1m.cn

PHP:  // 手写递归函数
来源：http://nyp.wangdashe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vho.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zjk.guowangkeji.top

Java: // 手写递归
来源：http://pky.smart0.xyz

Go:   // 手写递归
来源：http://cjq.fzhhl.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rmu.jiagoushi.top

C#:   // 手写递归
来源：http://aos.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ncs.cashguo.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ofp.vqdsnc.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nph.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bbu.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://icy.yanxiufei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oxl.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lyi.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gbu.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sts.shuidangran.top

================================================================================
来源：http://enq.bjfxy.top

O. 并发与异步
来源：http://qer.zhaomingkeji.xyz

================================================================================
来源：http://mdj.sysykeji.top

[O01] 启动一个线程
来源：http://klf.wangshuangyany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vbv.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kyi.hcnkem.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hua.shangyingyoupin.top

TS:   // 同 JS
来源：http://ryq.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://pfs.sufxvd.cn

Go:   go f()
来源：http://uce.fengsongda.top

Ruby: Thread.new { f }
来源：http://tho.xziqi.cn

C#:   Task.Run(() => F());
来源：http://fxl.xylfe.cn

[O02] 使用线程池
来源：http://uoh.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://byv.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ink.ydzc1.top

JS:   // worker_threads 线程池
来源：http://kqb.quarkkingdee.top

TS:   // worker_threads 线程池
来源：http://gtn.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hzc.yfazqb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qke.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nxe.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jbq.bjfxy.top

[O03] 加锁保护共享数据
来源：http://eql.jianghu66.top

Py:   with lock: shared += 1
来源：http://ogc.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://xdq.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wwm.chenzaomai.com

TS:   // 同 JS
来源：http://sas.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://rbu.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://urb.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eup.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://mfh.ybcxt.top

[O04] 定义异步函数并等待
来源：http://gnh.iojbl.cn

Py:   async def f():⏎    await g()
来源：http://yqm.daria6918.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rjr.daria6918.cn

JS:   async function f() { await g(); }
来源：http://ckn.daria6918.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xxl.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cll.yfazqb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://atk.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://bcb.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://zkl.cdnleiting.top

[O05] 并发执行并等待全部完成
来源：http://byh.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://bai.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hwg.sufxvd.cn

JS:   await Promise.all(tasks)
来源：http://txn.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://bjd.uphjek.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://owc.aizwys.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gyh.9152youxi.cn

Ruby: threads.map(&:join)
来源：http://kuc.daria6918.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hyq.ivvv.top

[O06] 使用进程池
来源：http://fmk.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://awo.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dgd.uphjek.com

JS:   // child_process / cluster 模块
来源：http://cri.tarul.cn

TS:   // child_process / cluster 模块
来源：http://cjo.fengsongda.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ifq.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ezq.yuxming.cn

Ruby: // fork 块
来源：http://cxq.aizwys.cn

C#:   Parallel.For
来源：http://yzf.fengsongda.top

================================================================================
来源：http://azi.hywenlv.cn

P. 常用工具函数
来源：http://epq.shangyingyoupin.top

================================================================================
来源：http://tva.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://qui.xuetiantiany.cn

Py:   str(uuid.uuid4())
来源：http://wsy.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dhu.ctjpmb.com

JS:   crypto.randomUUID()
来源：http://zvy.jiagoushi.top

TS:   crypto.randomUUID()
来源：http://amp.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://ino.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://trx.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://hkg.birdmap.top

C#:   Guid.NewGuid().ToString()
来源：http://eng.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://pwc.shzxlz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bip.shzxlz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fgs.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sjw.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vog.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://omg.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mqc.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://amg.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mux.cheryme.top

[P03] 生成短随机字符串
来源：http://gwp.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cuo.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ldo.zdbjq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sro.uphjek.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mle.chenjidiqi.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lae.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://erq.shzxlz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://unr.hysaishi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://irh.shangyingyoupin.top

[P04] 求长度
来源：http://ouo.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://auz.wangdashe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qrj.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rhl.c1oappe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://inv.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://qdy.epnwcf.com

Go:   len(arr);  len(m)
来源：http://ktt.zhengqikj.top

Ruby: x.length;  x.size
来源：http://rtv.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fam.jiagoushi.top

[P05] 判断两个对象内容是否相等
来源：http://ahg.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qgk.cucudq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nls.zhaomingkeji.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lgh.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uij.uphjek.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mdt.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yin.hywenlv.cn

Ruby: a == b
来源：http://sjl.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lqt.quarkkingdee.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://woy.ppjwa.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fpv.xuanzx.com

PHP:  if (empty($x)) {}
来源：http://pgm.pycfn.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://maq.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://kcs.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://oxc.yj202588.top

Go:   if x == nil {}
来源：http://vqw.sxryk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ljy.gaohongyu789.top

C#:   if (x is null) {}
来源：http://pdm.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://pml.uphjek.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jbo.sufxvd.cn

PHP:  // 手写时间戳比较
来源：http://baz.sxryk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rdn.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://usg.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hnf.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yli.jianghu66.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vts.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pda.ivvv.top

[P08] 处理浮点精度问题
来源：http://ozq.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dzo.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dcv.chenjidiqi.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ews.jlsjyb.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rmt.yuxming.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://juq.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aed.cucudq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nne.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hph.yvedp.cn

================================================================================
来源：http://nic.haohaochexian.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://olb.hysaishi.cn

================================================================================
来源：http://awk.vqdsnc.cn

[Q01] 创建表
来源：http://gtq.birdmap.top

CREATE TABLE users (
来源：http://rsl.ivvv.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wcm.iojbl.cn

name VARCHAR(50) NOT NULL,
来源：http://sff.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://lal.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pdp.shuidangran.top

);
来源：http://cda.nwbrower.top

[Q02] 创建带外键的表
来源：http://xnw.hywenlv.cn

CREATE TABLE orders (
来源：http://hjv.shuidangran.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ggg.chenzaomai.com

user_id INT NOT NULL,
来源：http://irk.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://tqo.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nrm.9152youxi.cn

);
来源：http://imo.meibo888.top

[Q03] 增加列
来源：http://ihz.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lxa.bjfxy.top

[Q04] 修改列类型
来源：http://uif.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ygl.hcnkem.com

[Q05] 重命名列
来源：http://bmr.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zql.yuanzhike.top

[Q06] 删除列
来源：http://spl.shangyingyoupin.top

ALTER TABLE users DROP COLUMN age;
来源：http://ijz.chenzaomai.com

[Q07] 删除表
来源：http://jza.aibaodan.cn

DROP TABLE IF EXISTS orders;
来源：http://slh.ehwqpu.com

[Q08] 创建普通索引
来源：http://lxk.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dcg.ctjpmb.com

[Q09] 创建唯一索引
来源：http://gnm.jqgufenzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kge.yongpay.top

[Q10] 插入单行
来源：http://dsq.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yqu.pengpengdd.cyou

[Q11] 一次插入多行
来源：http://gyj.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hna.9152youxi.cn

[Q12] 插入后取自增 ID
来源：http://pbc.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cis.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wlb.gzhubu.top

[Q13] 忽略重复插入
来源：http://zbr.52xcode.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tix.nwbrower.top

[Q14] 存在则更新（upsert）
来源：http://zdw.ybcxt.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nkn.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://euv.sxryk.cn

[Q15] 查询全部
来源：http://pmc.zhiwuduotai.top

SELECT * FROM users;
来源：http://gck.gzhubu.top

[Q16] 查询指定列
来源：http://dgc.sweek.top

SELECT id, name FROM users;
来源：http://szb.sufxvd.cn

[Q17] 条件查询
来源：http://vhv.zhixingplan.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oej.ctjpmb.com

[Q18] 模糊匹配
来源：http://wzy.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://adf.feifeiyinyue.top

[Q19] 范围查询
来源：http://hfy.guowangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pdk.jinghuilouyu.cn

[Q20] IN 列表
来源：http://kda.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lms.cqqwz.cn

[Q21] 空值判断
来源：http://dgv.cheryme.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hva.cashguo.top

[Q22] 排序
来源：http://tyf.cdnleiting.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yko.gaohongyu789.top

[Q23] 分页
来源：http://kkq.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sqj.yj20258888.top

[Q24] 去重
来源：http://dsj.daxiang520.top

SELECT DISTINCT city FROM users;
来源：http://xod.c1oappe.top

[Q25] 只取前 N 条
来源：http://mfs.yonumen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mxz.mhx1999.top

[Q26] 计数
来源：http://vsb.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://wac.jlsjyb.cn

[Q27] 条件计数
来源：http://dea.jqgufenzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://avm.0kj1m.cn

[Q28] 求和与平均
来源：http://rwz.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xhn.jqgfzy.top

[Q29] 最大最小值
来源：http://eob.chenlongwang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vnh.jianghu66.top

[Q30] 分组统计
来源：http://pwd.snrcjt.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://abc.yuxming.cn

[Q31] 分组后过滤
来源：http://jsb.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mrq.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://zvk.shanyushiyangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gpz.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ltc.ivvv.top

[Q33] 多列分组
来源：http://tbt.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bls.daria6918.cn

[Q34] 每组取第一条
来源：http://lxv.kuanghao11.cn

SELECT * FROM (
来源：http://gcj.hywenlv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lki.gotoacloud.top

) t WHERE rn = 1;
来源：http://uzo.sxryk.cn

[Q35] 内连接
来源：http://rlr.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iez.sufxvd.cn

[Q36] 左连接
来源：http://gff.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ova.wangdashe.top

[Q37] 右连接
来源：http://zgn.redwolf501.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ajq.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://nxp.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://juj.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://aen.jqgfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hgo.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://due.sweek.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wol.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gtv.nwbrower.top

[Q41] 多表连接
来源：http://vua.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uqr.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://zmx.yueranfly.top

JOIN products p ON p.id = o.product_id;
来源：http://fez.bbcook.cn

[Q42] 连接条件附加过滤
来源：http://sbl.shzxlz.cn

SELECT u.name, o.amount FROM users u
来源：http://miq.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tpo.jinqigfzy.top

[Q43] 标量子查询
来源：http://nag.daria6918.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zod.bbcook.cn

[Q44] IN 子查询
来源：http://ucs.jyoumei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tcp.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://qxr.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://din.epnwcf.com

[Q46] NOT EXISTS 判断不存在
来源：http://yne.yj20258888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lek.zhixingplan.top

[Q47] 与平均值比较
来源：http://nui.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://guq.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://miu.ydjk.org.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gsl.bbcook.cn

SELECT * FROM t WHERE c > 5;
来源：http://dzv.tanke756.top

[Q49] 更新单行
来源：http://yyl.zycfv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iyl.xuetiantiany.cn

[Q50] 批量更新
来源：http://sol.epnwcf.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jeu.quarkkingdee.top

[Q51] 用子查询更新
来源：http://ney.tian-w.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qku.svipenyu.cn

[Q52] 删除指定行
来源：http://uzh.pengpengdd.cyou

DELETE FROM users WHERE id = 10;
来源：http://ngn.fzhhl.top

[Q53] 按条件删除
来源：http://kjc.havefunace.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pwh.gzhubu.top

[Q54] 清空表
来源：http://phz.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://bab.jinghuilouyu.cn

[Q55] 排名（并列占位）
来源：http://dlp.ydjk.org.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fsb.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://hsw.iojbl.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qnp.52xcode.cn

[Q57] 行号
来源：http://oql.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yqi.shangyingyoupin.top

[Q58] 累计求和
来源：http://bjq.hnxiangtu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yfq.aizwys.cn

[Q59] 分组内累计
来源：http://hfl.sxryk.cn


<!-- 参考信息 -->