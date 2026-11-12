代发 wailian999

[N09] 栈与队列
来源：http://tlu.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tfj.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pfp.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qgo.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sfb.mhx1999.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fyb.jinqigfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oam.zdbjq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zda.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ekg.dianchejie.cn

[N10] 链表节点定义
来源：http://qqh.gogol.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://brd.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wfk.aibaodan.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ddu.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jay.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://uoi.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://igv.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gde.gogol.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qsv.ybcxt.top

[N11] 二叉树中序遍历
来源：http://bal.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zoa.tanke756.top

PHP:  // 手写递归函数
来源：http://pvo.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aus.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pkg.xuetiantiany.cn

Java: // 手写递归
来源：http://grr.c1oappe.top

Go:   // 手写递归
来源：http://tav.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pta.chenlongwang.top

C#:   // 手写递归
来源：http://pzn.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cul.zhiwuduotai.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fzm.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ukc.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vgn.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://inj.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ulh.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ifc.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uor.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://npr.epnwcf.com

================================================================================
来源：http://osu.guannengcc.top

O. 并发与异步
来源：http://ibe.yonumen.top

================================================================================
来源：http://egr.sysykeji.top

[O01] 启动一个线程
来源：http://jqp.yfazqb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hko.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ssd.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zsg.nanxuanxn.top

TS:   // 同 JS
来源：http://jqq.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://twm.jlsjyb.cn

Go:   go f()
来源：http://khj.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://rgl.tian-w.cn

C#:   Task.Run(() => F());
来源：http://skc.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://equ.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hvu.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://awq.yuanzhike.top

JS:   // worker_threads 线程池
来源：http://aub.sxryk.cn

TS:   // worker_threads 线程池
来源：http://hzf.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pqw.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ihq.yvedp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kfq.gzhubu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://klw.hywenlv.cn

[O03] 加锁保护共享数据
来源：http://kdj.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://dur.ydjk.org.cn

PHP:  // 用 flock() 做文件锁
来源：http://mtq.chenzaomai.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bco.quarkkingdee.top

TS:   // 同 JS
来源：http://jbb.ydzc1.top

Java: synchronized (this) { shared++; }
来源：http://tkf.jinghuilouyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xzm.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://fgu.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://kzs.fehbvm.com

[O04] 定义异步函数并等待
来源：http://ues.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://sag.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rxh.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://mlh.zycfv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nxg.yfazqb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kvf.daxiang520.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://osy.jinqigufen.top

Ruby: # 用 Fiber 或 async gem
来源：http://dfs.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://rxf.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://chm.shanyushiyangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://rgw.hesvh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dqf.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://ejc.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://nrv.yj20258.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://crq.vqdsnc.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ile.shanyushiyangkeji.top

Ruby: threads.map(&:join)
来源：http://qwd.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xdf.hysaishi.cn

[O06] 使用进程池
来源：http://pyb.xuanzx.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uqb.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bib.zhongyouzk.top

JS:   // child_process / cluster 模块
来源：http://xtt.bjfxy.top

TS:   // child_process / cluster 模块
来源：http://whw.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dcf.9152youxi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ynz.xuetiantiany.cn

Ruby: // fork 块
来源：http://kpl.gogol.net.cn

C#:   Parallel.For
来源：http://ydb.shuidangran.top

================================================================================
来源：http://dmv.haohaochexian.top

P. 常用工具函数
来源：http://hyq.jqgufenzy.top

================================================================================
来源：http://oqj.chenlongwang.top

[P01] 生成 UUID
来源：http://wvf.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://zhy.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://scz.yanxiufei.cn

JS:   crypto.randomUUID()
来源：http://nje.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://cuq.yfazqb.com

Java: UUID.randomUUID().toString()
来源：http://yym.smart0.xyz

Go:   // 用 github.com/google/uuid
来源：http://oqc.nanxuanxn.top

Ruby: SecureRandom.uuid
来源：http://uwr.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://gaj.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://ack.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://drt.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rip.shzxlz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fuq.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sca.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jnx.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nwo.zhiwuduotai.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pig.52xcode.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iws.guowangkeji.top

[P03] 生成短随机字符串
来源：http://vkd.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rzi.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://phn.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rtq.yanxiufei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nfp.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zbm.vehdjk.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qpc.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vtj.chenlongwang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://urj.iojbl.cn

[P04] 求长度
来源：http://qna.vehdjk.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mra.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sgp.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://miz.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://voo.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://hwj.yj202588.top

Go:   len(arr);  len(m)
来源：http://bco.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://vgv.yueranfly.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zxz.zycfv.cn

[P05] 判断两个对象内容是否相等
来源：http://mwp.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://iie.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yxl.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://caf.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://adc.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wft.wangshuangyany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bvj.zycfv.cn

Ruby: a == b
来源：http://udr.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://okn.yongpay.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ngf.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://imi.ivvv.top

PHP:  if (empty($x)) {}
来源：http://htd.svipenyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ljj.gotoacloud.top

TS:   if (x == null) {}
来源：http://luw.redwolf501.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nsa.xuanzx.com

Go:   if x == nil {}
来源：http://xwh.gzhubu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cyz.yvedp.cn

C#:   if (x is null) {}
来源：http://gna.shzxlz.cn

[P07] 防抖与节流
来源：http://vjf.vehdjk.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bpt.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://iuz.sxryk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cmz.zhongyouzk.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fgj.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sfc.gotoacloud.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://skx.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ahw.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hic.zdbjq.cn

[P08] 处理浮点精度问题
来源：http://mvy.jyoumei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xrg.tanke756.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kbn.vqdsnc.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gjc.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jtr.wangshuangyany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wir.ydjk.org.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://coc.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hui.cdnleiting.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vbr.ivvv.top

================================================================================
来源：http://mdx.jiagoushi.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mau.zhiwuduotai.top

================================================================================
来源：http://szr.havefunace.top

[Q01] 创建表
来源：http://zfu.sweek.top

CREATE TABLE users (
来源：http://fjv.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sdv.iojbl.cn

name VARCHAR(50) NOT NULL,
来源：http://xzn.xylfe.cn

email VARCHAR(100) UNIQUE,
来源：http://ceo.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pkx.shangyingyoupin.top

);
来源：http://epa.zdbjq.cn

[Q02] 创建带外键的表
来源：http://gqb.fehbvm.com

CREATE TABLE orders (
来源：http://kvj.smart0.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vwz.ydzc1.top

user_id INT NOT NULL,
来源：http://xsg.hnxiangtu.top

amount DECIMAL(10, 2),
来源：http://pkl.hcnkem.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rta.chenzaomai.com

);
来源：http://tnb.pycfn.com

[Q03] 增加列
来源：http://qcm.jqgfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://flj.daxiang520.top

[Q04] 修改列类型
来源：http://hvb.xingfuxueyuan.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tiy.hongshengwenyu.top

[Q05] 重命名列
来源：http://prf.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pfq.dianchejie.cn

[Q06] 删除列
来源：http://ota.yuxming.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mdt.vqdsnc.cn

[Q07] 删除表
来源：http://pgc.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://hgv.cqqwz.cn

[Q08] 创建普通索引
来源：http://fem.sxryk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nat.svipenyu.cn

[Q09] 创建唯一索引
来源：http://gfg.cqqwz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uaf.9152youxi.cn

[Q10] 插入单行
来源：http://mtd.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dyn.sysykeji.top

[Q11] 一次插入多行
来源：http://mwx.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uow.cashguo.top

[Q12] 插入后取自增 ID
来源：http://yug.ydjk.org.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mna.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nwf.haohaochexian.top

[Q13] 忽略重复插入
来源：http://myp.52xcode.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gkz.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://ygg.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kjq.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bol.nwbrower.top

[Q15] 查询全部
来源：http://wxy.sufxvd.cn

SELECT * FROM users;
来源：http://slr.yueranfly.top

[Q16] 查询指定列
来源：http://fvq.jinqigfzy.top

SELECT id, name FROM users;
来源：http://cyd.dashuyun.cn

[Q17] 条件查询
来源：http://onr.xinyue.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pit.gotoacloud.top

[Q18] 模糊匹配
来源：http://nko.cashguo.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qne.cashguo.top

[Q19] 范围查询
来源：http://ikg.zhaomingkeji.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mhc.hongshengwenyu.top

[Q20] IN 列表
来源：http://tge.gzhubu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yqi.tian-w.cn

[Q21] 空值判断
来源：http://dnm.xingfuxueyuan.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://nhh.vqdsnc.cn

[Q22] 排序
来源：http://zib.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lao.zhixingplan.top

[Q23] 分页
来源：http://srx.yj202588.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://spq.ppjwa.cn

[Q24] 去重
来源：http://ghp.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://gak.daria6918.cn

[Q25] 只取前 N 条
来源：http://goy.jinqigfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qkz.xylfe.cn

[Q26] 计数
来源：http://nnl.nanxuanxn.top

SELECT COUNT(*) FROM users;
来源：http://dps.xuanzx.com

[Q27] 条件计数
来源：http://axm.yuxming.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gpu.gotoacloud.top

[Q28] 求和与平均
来源：http://udt.ehwqpu.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sun.yj202588.top

[Q29] 最大最小值
来源：http://qrw.0kj1m.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fav.ydjk.org.cn

[Q30] 分组统计
来源：http://zpk.shzxlz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ozn.daria6918.cn

[Q31] 分组后过滤
来源：http://rxt.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ast.ppjwa.cn

[Q32] 分组拼接字符串
来源：http://xfu.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gzq.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mbi.yj202588.top

[Q33] 多列分组
来源：http://wcl.zhengqikj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mjc.redwolf501.top

[Q34] 每组取第一条
来源：http://det.shanyushiyangtech.top

SELECT * FROM (
来源：http://vmk.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uhr.316326.xyz

) t WHERE rn = 1;
来源：http://qls.nanxinkj.top

[Q35] 内连接
来源：http://dsj.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vge.haohaochexian.top

[Q36] 左连接
来源：http://gwa.birdmap.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://juu.fktsv.cn

[Q37] 右连接
来源：http://rit.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wah.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://joo.sweek.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wet.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://kqx.hnqzz.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://oau.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hyw.zhixingplan.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fke.hesvh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yds.yanxiufei.cn

[Q41] 多表连接
来源：http://hcd.mhx1999.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lbc.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://wdl.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://qgy.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://jnc.hammf.cn

SELECT u.name, o.amount FROM users u
来源：http://fcq.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ajl.uphjek.com

[Q43] 标量子查询
来源：http://bcx.hammf.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://roy.havefunace.top

[Q44] IN 子查询
来源：http://wmv.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mpa.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://iwc.pycfn.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://poz.yuanzhike.top

[Q46] NOT EXISTS 判断不存在
来源：http://tyv.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jfu.pycfn.com

[Q47] 与平均值比较
来源：http://zkn.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://usi.pycfn.com

[Q48] CTE 公用表表达式
来源：http://kjb.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kkw.cqqwz.cn

SELECT * FROM t WHERE c > 5;
来源：http://ybp.sxryk.cn

[Q49] 更新单行
来源：http://pcm.daria6918.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gbo.xuetiantiany.cn

[Q50] 批量更新
来源：http://klt.yuanzhike.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qcq.vqdsnc.cn

[Q51] 用子查询更新
来源：http://fev.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uvl.andypj.xyz

[Q52] 删除指定行
来源：http://xjt.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://pst.yj20258888.top

[Q53] 按条件删除
来源：http://dea.quarkkingdee.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vbu.havefunace.top

[Q54] 清空表
来源：http://vit.daria6918.cn

TRUNCATE TABLE logs;
来源：http://hqb.hammf.cn

[Q55] 排名（并列占位）
来源：http://nak.chenjidiqi.icu


<!-- 参考信息 -->