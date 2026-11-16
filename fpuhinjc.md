代发 wailian999

Go:   // 手写 map[int]int
来源：http://quy.yangfankeji.com

Ruby: // 手写 Hash
来源：http://vhx.zdqjudy.top

C#:   // 手写 Dictionary<int, int>
来源：http://irb.yj20258888.top

[N08] 生成全排列
来源：http://lef.yongpay.top

Py:   itertools.permutations(arr)
来源：http://bqc.birdmap.top

PHP:  // 手写递归交换
来源：http://ihl.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://rdn.ctjpmb.com

TS:   // 手写回溯递归
来源：http://ljk.9152youxi.cn

Java: // 手写回溯递归
来源：http://oal.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://nhk.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://exq.uphjek.com

C#:   // 手写回溯递归
来源：http://ooe.0kj1m.cn

[N09] 栈与队列
来源：http://znr.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vps.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sah.dianchejie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://spp.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ljj.mhx1999.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://luo.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ykk.shangyingyoupin.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kxd.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qrh.shuidangran.top

[N10] 链表节点定义
来源：http://vwi.sweek.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dku.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://izo.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rjc.guannengcc.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iqx.zdbjq.cn

Java: class Node { int v; Node next; }
来源：http://fob.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://ixn.c1oappe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xzq.svipenyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gyd.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://nho.fanxiaobao.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vga.ydzc1.top

PHP:  // 手写递归函数
来源：http://qoz.hcnkem.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://beh.birdmap.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dyl.cashguo.top

Java: // 手写递归
来源：http://fgz.jiagoushi.top

Go:   // 手写递归
来源：http://yms.ybcxt.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mqg.zhiwuduotai.top

C#:   // 手写递归
来源：http://jhf.pengpengdd.cyou

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sck.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ddr.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://apa.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bry.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://amz.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tvs.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rke.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gsy.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dbz.sufxvd.cn

================================================================================
来源：http://hco.jianghu66.top

O. 并发与异步
来源：http://riw.wangdashe.top

================================================================================
来源：http://ezz.fehbvm.com

[O01] 启动一个线程
来源：http://viq.wangdashe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tss.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lcf.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nkz.vehdjk.com

TS:   // 同 JS
来源：http://uid.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://gkp.shanyushiyangtech.top

Go:   go f()
来源：http://fwg.havefunace.top

Ruby: Thread.new { f }
来源：http://fyv.svipenyu.cn

C#:   Task.Run(() => F());
来源：http://myo.dianchejie.cn

[O02] 使用线程池
来源：http://igu.yj20258888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dja.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yak.hnqzz.top

JS:   // worker_threads 线程池
来源：http://xkz.fzhhl.top

TS:   // worker_threads 线程池
来源：http://zpi.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kht.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ltp.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rwi.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rfc.fengsongda.top

[O03] 加锁保护共享数据
来源：http://abn.svipenyu.cn

Py:   with lock: shared += 1
来源：http://jup.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://urs.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fvq.gotoacloud.top

TS:   // 同 JS
来源：http://ces.bbcook.cn

Java: synchronized (this) { shared++; }
来源：http://hsf.hcnkem.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ids.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dpy.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://jlr.iojbl.cn

[O04] 定义异步函数并等待
来源：http://tpc.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://rcv.tanke756.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://flv.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://ogc.zhiwuduotai.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nzw.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ler.yuanzhike.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xed.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://mvj.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://ewj.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://ivf.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://xck.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oqv.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://yeg.hesvh.cn

TS:   await Promise.all(tasks)
来源：http://bfi.uphjek.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xxx.fehbvm.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nol.yj20258888.top

Ruby: threads.map(&:join)
来源：http://ors.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zkk.wangdashe.top

[O06] 使用进程池
来源：http://aqj.sjlbkw.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pkd.ppjwa.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yff.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://nce.chenlongwang.top

TS:   // child_process / cluster 模块
来源：http://juu.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ziz.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uqr.fengsongda.top

Ruby: // fork 块
来源：http://qtr.zycfv.cn

C#:   Parallel.For
来源：http://yqp.fzhhl.top

================================================================================
来源：http://lur.pengpengdd.cyou

P. 常用工具函数
来源：http://tsm.jinyuanbaomall.cn

================================================================================
来源：http://fmf.redwolf501.top

[P01] 生成 UUID
来源：http://crk.jianghu66.top

Py:   str(uuid.uuid4())
来源：http://ytu.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rok.guannengcc.top

JS:   crypto.randomUUID()
来源：http://bvc.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://geb.sweek.top

Java: UUID.randomUUID().toString()
来源：http://zmo.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://hlo.hesvh.cn

Ruby: SecureRandom.uuid
来源：http://tct.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://ybd.gaohongyu789.top

[P02] MD5 / SHA256 摘要
来源：http://cdf.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ksu.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kgw.epnwcf.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dkn.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qtp.nwbrower.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tqv.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sjo.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kvk.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xoo.fengsongda.top

[P03] 生成短随机字符串
来源：http://ikb.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dek.yfazqb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bok.jianghu66.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kab.xinyue.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hhu.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://htf.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://del.zhengqikj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ulf.haohaochexian.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fsm.hywenlv.cn

[P04] 求长度
来源：http://aav.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sri.yongpay.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gze.cdnleiting.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://myz.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tnf.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://soc.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://qot.bjfxy.top

Ruby: x.length;  x.size
来源：http://lls.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fgv.xuetiantiany.cn

[P05] 判断两个对象内容是否相等
来源：http://dqs.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zuu.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yil.jlsjyb.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bnl.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fpe.aizwys.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yba.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://koy.gzhubu.top

Ruby: a == b
来源：http://cuq.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mxl.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pck.jinyuanbaomall.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uex.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://efz.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aen.yanxiufei.cn

TS:   if (x == null) {}
来源：http://kgf.chenjidiqi.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://enm.kuanghao11.cn

Go:   if x == nil {}
来源：http://jas.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kmq.wangshuangyany.cn

C#:   if (x is null) {}
来源：http://wkq.nanxinkj.top

[P07] 防抖与节流
来源：http://dim.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jwu.zdbjq.cn

PHP:  // 手写时间戳比较
来源：http://vnc.ehwqpu.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kch.yj20258888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pqj.tianlin.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sdz.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zdl.nwbrower.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cwn.dashuyun.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://piw.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://hxo.shzxlz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lzr.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mqn.hesvh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xys.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sjx.hcnkem.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xme.xinyue.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gvu.cucudq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dgv.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ttz.guowangkeji.top

================================================================================
来源：http://jaw.vehdjk.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ksa.epnwcf.com

================================================================================
来源：http://wit.jinghuilouyu.cn

[Q01] 创建表
来源：http://tji.jinqigfzy.top

CREATE TABLE users (
来源：http://jwg.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://efs.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://qil.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://iqx.ehwqpu.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mvw.tanke756.top

);
来源：http://olg.hfpthk.cn

[Q02] 创建带外键的表
来源：http://teo.birdmap.top

CREATE TABLE orders (
来源：http://rit.0kj1m.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vqi.nanxuanxn.top

user_id INT NOT NULL,
来源：http://now.cheryme.top

amount DECIMAL(10, 2),
来源：http://okc.nwbrower.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wwu.xylfe.cn

);
来源：http://fio.c1oappe.top

[Q03] 增加列
来源：http://ouf.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ptm.gzhubu.top

[Q04] 修改列类型
来源：http://sev.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://owm.haohaochexian.top

[Q05] 重命名列
来源：http://frd.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ywl.yj20258.top

[Q06] 删除列
来源：http://gql.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://yvj.yfazqb.com

[Q07] 删除表
来源：http://ona.smart0.xyz

DROP TABLE IF EXISTS orders;
来源：http://fph.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://zpv.jqgfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bhz.316326.xyz

[Q09] 创建唯一索引
来源：http://llk.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://icn.xziqi.cn

[Q10] 插入单行
来源：http://vao.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dcp.yfazqb.com

[Q11] 一次插入多行
来源：http://kle.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yha.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://dzu.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://rbn.quarkkingdee.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ucc.jinqigufen.top

[Q13] 忽略重复插入
来源：http://raz.yj20258888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fki.shangyingyoupin.top

[Q14] 存在则更新（upsert）
来源：http://wll.tanke756.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ciu.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ukf.guowangkeji.top

[Q15] 查询全部
来源：http://abo.hnxiangtu.top

SELECT * FROM users;
来源：http://ucq.hnqzz.top

[Q16] 查询指定列
来源：http://zgx.havefunace.top

SELECT id, name FROM users;
来源：http://dxz.9152youxi.cn

[Q17] 条件查询
来源：http://rhe.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://alx.hcnkem.com

[Q18] 模糊匹配
来源：http://jlq.zhaomingkeji.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rnh.hongshengwenyu.top

[Q19] 范围查询
来源：http://nca.zhaomingkeji.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wui.ydzc1.top

[Q20] IN 列表
来源：http://dpm.cheryme.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://exs.hfpthk.cn

[Q21] 空值判断
来源：http://kum.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eig.pengpengdd.cyou

[Q22] 排序
来源：http://clp.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nhb.yuxming.cn

[Q23] 分页
来源：http://jwm.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fuj.hywenlv.cn

[Q24] 去重
来源：http://uho.yuxming.cn

SELECT DISTINCT city FROM users;
来源：http://ekc.hongshengwenyu.top

[Q25] 只取前 N 条
来源：http://ewp.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xdh.ywan-chungtsiang.top

[Q26] 计数
来源：http://xbo.hnqzz.top

SELECT COUNT(*) FROM users;
来源：http://yid.yanxiufei.cn

[Q27] 条件计数
来源：http://yfz.yuxming.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tpr.c1oappe.top

[Q28] 求和与平均
来源：http://cbh.nwbrower.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fqc.c1oappe.top

[Q29] 最大最小值
来源：http://jvg.kuanghao11.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pmy.zdbjq.cn

[Q30] 分组统计
来源：http://tpc.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sox.shzxlz.cn

[Q31] 分组后过滤
来源：http://obb.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://olx.cashguo.top

[Q32] 分组拼接字符串
来源：http://zay.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ddh.xuetiantiany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dsy.cashguo.top

[Q33] 多列分组
来源：http://nkp.aibaodan.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fan.jqgfzy.top

[Q34] 每组取第一条
来源：http://jez.sysykeji.top

SELECT * FROM (
来源：http://xbs.jyoumei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uio.fzhhl.top

) t WHERE rn = 1;
来源：http://wef.sysykeji.top

[Q35] 内连接
来源：http://agk.jinqigfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hcn.jinqigufen.top

[Q36] 左连接
来源：http://lfn.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nla.yj20258888.top

[Q37] 右连接
来源：http://xrj.pycfn.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ggy.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://hoe.hcnkem.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ijn.zhiwuduotai.top

[Q39] 自连接（查上下级）
来源：http://fvh.xuetiantiany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mka.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ben.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hvf.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vrq.mhx1999.top

[Q41] 多表连接
来源：http://iif.epnwcf.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://kdv.nwbrower.top

JOIN users u ON u.id = o.user_id
来源：http://srf.sysykeji.top

JOIN products p ON p.id = o.product_id;
来源：http://ypv.birdmap.top

[Q42] 连接条件附加过滤
来源：http://exg.zhixingplan.top

SELECT u.name, o.amount FROM users u
来源：http://dlc.yueranfly.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zjw.kuanghao11.cn

[Q43] 标量子查询
来源：http://zmk.xuetiantiany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ycg.gaohongyu789.top

[Q44] IN 子查询
来源：http://fvz.cdnleiting.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sqp.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://fou.ctjpmb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qdu.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://yqq.meibo888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tuw.sweek.top

[Q47] 与平均值比较
来源：http://fge.316326.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ztc.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://teq.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cfj.xinyue.icu

SELECT * FROM t WHERE c > 5;
来源：http://anb.sjlbkw.cn

[Q49] 更新单行
来源：http://nnm.hesvh.cn


<!-- 参考信息 -->