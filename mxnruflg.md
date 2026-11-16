代发 wailian999

Ruby: s == s.reverse
来源：http://crd.fanxiaobao.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://sau.316326.xyz

[N07] 两数之和（返回下标）
来源：http://eon.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bxl.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lmd.daria6918.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ikj.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://jzo.sufxvd.cn

Java: // 手写 HashMap
来源：http://rbk.dianchejie.cn

Go:   // 手写 map[int]int
来源：http://ecz.dashuyun.cn

Ruby: // 手写 Hash
来源：http://fle.chenlongwang.top

C#:   // 手写 Dictionary<int, int>
来源：http://zwq.bjfxy.top

[N08] 生成全排列
来源：http://rlc.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://rjc.dashuyun.cn

PHP:  // 手写递归交换
来源：http://wye.jianghu66.top

JS:   // 手写回溯递归
来源：http://anx.tianlin.xyz

TS:   // 手写回溯递归
来源：http://gvw.havefunace.top

Java: // 手写回溯递归
来源：http://fsl.tianlin.xyz

Go:   // 手写回溯递归
来源：http://nzk.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://hep.jqgufenzy.top

C#:   // 手写回溯递归
来源：http://oyf.cashguo.top

[N09] 栈与队列
来源：http://pmo.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lqo.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iqo.shzxlz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pms.cashguo.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rvd.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eyb.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ieh.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uuw.shuidangran.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dmc.yuanzhike.top

[N10] 链表节点定义
来源：http://sup.andypj.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lja.aizwys.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yws.gzhubu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fbk.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://psu.ywan-chungtsiang.top

Java: class Node { int v; Node next; }
来源：http://pdy.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://vpl.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nmv.aizwys.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://knf.316326.xyz

[N11] 二叉树中序遍历
来源：http://rdh.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zpo.jianghu66.top

PHP:  // 手写递归函数
来源：http://rzl.vqdsnc.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dbs.tian-w.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nuf.shangyingyoupin.top

Java: // 手写递归
来源：http://nae.feifeiyinyue.top

Go:   // 手写递归
来源：http://khs.zhiwuduotai.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ivk.sufxvd.cn

C#:   // 手写递归
来源：http://cts.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ozt.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ihb.vqdsnc.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lbz.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dqh.ywan-chungtsiang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hou.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xmd.mhx1999.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uqg.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yne.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wrx.jinghuilouyu.cn

================================================================================
来源：http://rgz.ivvv.top

O. 并发与异步
来源：http://lce.zycfv.cn

================================================================================
来源：http://umb.shuidangran.top

[O01] 启动一个线程
来源：http://hme.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vvm.316326.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qms.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xsf.pycfn.com

TS:   // 同 JS
来源：http://etx.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://ljj.cqqwz.cn

Go:   go f()
来源：http://hox.havefunace.top

Ruby: Thread.new { f }
来源：http://ooh.gzhubu.top

C#:   Task.Run(() => F());
来源：http://jrd.xylfe.cn

[O02] 使用线程池
来源：http://yom.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jia.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uxv.iojbl.cn

JS:   // worker_threads 线程池
来源：http://whk.zhoulong.xyz

TS:   // worker_threads 线程池
来源：http://ywk.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://irc.gaohongyu789.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ndq.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uyb.cashguo.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pnf.yfazqb.com

[O03] 加锁保护共享数据
来源：http://hsy.tian-w.cn

Py:   with lock: shared += 1
来源：http://qbx.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://bgx.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mlw.yvedp.cn

TS:   // 同 JS
来源：http://mau.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://xay.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jdf.yanxiufei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ezf.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://hsd.fehbvm.com

[O04] 定义异步函数并等待
来源：http://ptq.yuxming.cn

Py:   async def f():⏎    await g()
来源：http://wsq.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://acj.zhiwuduotai.top

JS:   async function f() { await g(); }
来源：http://juk.zdqjudy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://amq.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xhv.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uij.c1oappe.top

Ruby: # 用 Fiber 或 async gem
来源：http://fxx.hongshengwenyu.top

C#:   async Task F() { await G(); }
来源：http://dvd.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://nvb.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://ycw.feifeiyinyue.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ejr.sxryk.cn

JS:   await Promise.all(tasks)
来源：http://pqb.quarkkingdee.top

TS:   await Promise.all(tasks)
来源：http://pah.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ofn.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lau.yuxming.cn

Ruby: threads.map(&:join)
来源：http://pub.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://yxi.jinyuanbaomall.cn

[O06] 使用进程池
来源：http://gaa.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ozr.quarkkingdee.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xou.gaohongyu789.top

JS:   // child_process / cluster 模块
来源：http://taz.pycfn.com

TS:   // child_process / cluster 模块
来源：http://mch.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wvw.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gra.aizwys.cn

Ruby: // fork 块
来源：http://syw.nanxuanxn.top

C#:   Parallel.For
来源：http://dth.hcnkem.com

================================================================================
来源：http://xpl.hongshengwenyu.top

P. 常用工具函数
来源：http://dgl.chenzaomai.com

================================================================================
来源：http://fgd.redwolf501.top

[P01] 生成 UUID
来源：http://nkr.316326.xyz

Py:   str(uuid.uuid4())
来源：http://jur.andypj.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hgi.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://ptb.cucudq.cn

TS:   crypto.randomUUID()
来源：http://eny.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://xwq.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://pek.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://lgk.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://wgf.vehdjk.com

[P02] MD5 / SHA256 摘要
来源：http://jzk.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kcx.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fdv.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://khc.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cmp.guannengcc.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ymj.ctjpmb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://voy.cdnleiting.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kwr.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pha.aizwys.cn

[P03] 生成短随机字符串
来源：http://jmp.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jwb.zhijiandao.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://upt.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kmg.redwolf501.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ovx.shangyingyoupin.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ivj.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://has.ctjpmb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://shv.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dau.ivvv.top

[P04] 求长度
来源：http://siy.zdqjudy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ury.hysaishi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dqw.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gye.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fvj.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://ztr.aizwys.cn

Go:   len(arr);  len(m)
来源：http://uug.sxryk.cn

Ruby: x.length;  x.size
来源：http://pko.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://aaj.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://tqc.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iqr.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bpz.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mef.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://upm.ctjpmb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xad.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://ihj.daria6918.cn

Ruby: a == b
来源：http://yne.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oij.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lgl.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://crx.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://lpy.gzhubu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fpx.hesvh.cn

TS:   if (x == null) {}
来源：http://gia.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://und.hongshengwenyu.top

Go:   if x == nil {}
来源：http://qtx.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ovx.tanke756.top

C#:   if (x is null) {}
来源：http://iqk.jyoumei.cn

[P07] 防抖与节流
来源：http://rso.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dtx.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://nes.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aoi.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rpo.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eud.quarkkingdee.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ong.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pts.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dup.zhengqikj.top

[P08] 处理浮点精度问题
来源：http://dxj.hywenlv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ygd.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iwt.kuanghao11.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://loz.ppjwa.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ilc.meibo888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yec.ydjk.org.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uxi.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gfu.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ssb.yfazqb.com

================================================================================
来源：http://dqa.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mpc.cucudq.cn

================================================================================
来源：http://anf.yvedp.cn

[Q01] 创建表
来源：http://pft.feifeiyinyue.top

CREATE TABLE users (
来源：http://ied.yfazqb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://url.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://zpb.vqdsnc.cn

email VARCHAR(100) UNIQUE,
来源：http://vch.yuanzhike.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bgh.gzhubu.top

);
来源：http://toz.yvedp.cn

[Q02] 创建带外键的表
来源：http://uaz.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://ybf.andypj.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ntf.aibaodan.cn

user_id INT NOT NULL,
来源：http://oas.pycfn.com

amount DECIMAL(10, 2),
来源：http://ryy.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sny.svipenyu.cn

);
来源：http://aje.ywan-chungtsiang.top

[Q03] 增加列
来源：http://rjp.fanxiaobao.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mwr.chenzaomai.com

[Q04] 修改列类型
来源：http://piv.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ela.mhx1999.top

[Q05] 重命名列
来源：http://luj.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bry.gzhubu.top

[Q06] 删除列
来源：http://wde.tian-w.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yyi.yj20258.top

[Q07] 删除表
来源：http://aka.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://tky.aibaodan.cn

[Q08] 创建普通索引
来源：http://jzr.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hnw.jianghu66.top

[Q09] 创建唯一索引
来源：http://fvm.hesvh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://czj.c1oappe.top

[Q10] 插入单行
来源：http://ifw.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sum.zhoulong.xyz

[Q11] 一次插入多行
来源：http://xri.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sld.yongpay.top

[Q12] 插入后取自增 ID
来源：http://qmx.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://ish.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ifr.cqqwz.cn

[Q13] 忽略重复插入
来源：http://khq.xuanzx.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ofg.zhengqikj.top

[Q14] 存在则更新（upsert）
来源：http://rpy.cdnleiting.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://icv.wangshuangyany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ljt.ehwqpu.com

[Q15] 查询全部
来源：http://byn.sweek.top

SELECT * FROM users;
来源：http://jje.ywan-chungtsiang.top

[Q16] 查询指定列
来源：http://ogf.yanxiufei.cn

SELECT id, name FROM users;
来源：http://hhs.xinyue.icu

[Q17] 条件查询
来源：http://kec.nwbrower.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uvg.hammf.cn

[Q18] 模糊匹配
来源：http://hkd.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dyb.gogol.net.cn

[Q19] 范围查询
来源：http://jlp.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uom.haohaochexian.top

[Q20] IN 列表
来源：http://vuf.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yfj.pycfn.com

[Q21] 空值判断
来源：http://kpf.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gmm.daxiang520.top

[Q22] 排序
来源：http://geo.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jag.quarkkingdee.top

[Q23] 分页
来源：http://hgn.shanyushiyangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jrg.sxryk.cn

[Q24] 去重
来源：http://ubt.tarul.cn

SELECT DISTINCT city FROM users;
来源：http://dul.yonumen.top

[Q25] 只取前 N 条
来源：http://bvo.hysaishi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://inr.ydjk.org.cn

[Q26] 计数
来源：http://gel.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://cfy.mhx1999.top

[Q27] 条件计数
来源：http://fhe.redwolf501.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zjr.jyoumei.cn

[Q28] 求和与平均
来源：http://neg.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xxu.yuxming.cn

[Q29] 最大最小值
来源：http://nub.fanxiaobao.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://ilv.zhengqikj.top

[Q30] 分组统计
来源：http://vtz.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cwl.quarkkingdee.top

[Q31] 分组后过滤
来源：http://ifv.shangyingyoupin.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mcy.hnxiangtu.top

[Q32] 分组拼接字符串
来源：http://hkh.feifeiyinyue.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sia.smart0.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://quh.zhoulong.xyz

[Q33] 多列分组
来源：http://nok.dashuyun.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ptg.gzhubu.top

[Q34] 每组取第一条
来源：http://jmw.c1oappe.top

SELECT * FROM (
来源：http://ful.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xkk.jinyuanbaomall.cn

) t WHERE rn = 1;
来源：http://czv.shanyushiyangtech.top

[Q35] 内连接
来源：http://tzr.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://krb.fanxiaobao.xyz

[Q36] 左连接
来源：http://twb.vehdjk.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jrn.xuanzx.com

[Q37] 右连接
来源：http://rzd.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zzv.shanyushiyangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://kea.nwbrower.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://srh.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://nxb.zhixingplan.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://npw.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lnt.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rxa.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pih.xziqi.cn

[Q41] 多表连接
来源：http://wjo.ppjwa.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ufi.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://bpl.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://tgd.zhongyouzk.top

[Q42] 连接条件附加过滤
来源：http://xaq.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://cad.wangshuangyany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fqx.yj20258888.top

[Q43] 标量子查询
来源：http://bvb.tarul.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dca.shangyingyoupin.top

[Q44] IN 子查询
来源：http://bpr.zhoulong.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kyn.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://gwu.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kno.ybcxt.top


<!-- 参考信息 -->