代发 wailian999

Ruby: s == s.reverse
来源：http://vgp.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hxc.tanke756.top

[N07] 两数之和（返回下标）
来源：http://tmw.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qsx.iojbl.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://axi.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cxc.tanke756.top

TS:   // 手写 Map<string, number>
来源：http://btl.xziqi.cn

Java: // 手写 HashMap
来源：http://wom.yj20258.top

Go:   // 手写 map[int]int
来源：http://kob.ctjpmb.com

Ruby: // 手写 Hash
来源：http://lob.chenlongwang.top

C#:   // 手写 Dictionary<int, int>
来源：http://src.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://isr.dianchejie.cn

Py:   itertools.permutations(arr)
来源：http://grb.zycfv.cn

PHP:  // 手写递归交换
来源：http://ckc.yongpay.top

JS:   // 手写回溯递归
来源：http://ymh.guowangkeji.top

TS:   // 手写回溯递归
来源：http://eak.ppjwa.cn

Java: // 手写回溯递归
来源：http://cnh.mhx1999.top

Go:   // 手写回溯递归
来源：http://ibm.dashuyun.cn

Ruby: arr.permutation.to_a
来源：http://ylx.yuxming.cn

C#:   // 手写回溯递归
来源：http://baa.gzhubu.top

[N09] 栈与队列
来源：http://poi.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ymk.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qjb.jqgfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kvd.shanyushiyangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://urk.shangyingyoupin.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xql.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xju.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ikq.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://okh.tian-w.cn

[N10] 链表节点定义
来源：http://upw.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xlw.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wtt.yfazqb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fjx.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mtw.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://atu.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://szv.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jkc.sxryk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tmt.c1oappe.top

[N11] 二叉树中序遍历
来源：http://aaj.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dbx.hysaishi.cn

PHP:  // 手写递归函数
来源：http://aly.jqgufenzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ycc.snrcjt.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vhu.jianghu66.top

Java: // 手写递归
来源：http://rch.haohaochexian.top

Go:   // 手写递归
来源：http://ulf.hywenlv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mhx.gzhubu.top

C#:   // 手写递归
来源：http://awi.zhengqikj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nvy.vqdsnc.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gtb.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dpr.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vev.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gos.hysaishi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qda.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lfz.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tah.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oyp.ydjk.org.cn

================================================================================
来源：http://hog.zhiwuduotai.top

O. 并发与异步
来源：http://cpa.ybcxt.top

================================================================================
来源：http://hsz.hcnkem.com

[O01] 启动一个线程
来源：http://zyg.shangyingyoupin.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bil.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nxk.ppjwa.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hzx.zhijiandao.cn

TS:   // 同 JS
来源：http://jxm.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://oam.shuidangran.top

Go:   go f()
来源：http://bui.tianlin.xyz

Ruby: Thread.new { f }
来源：http://wqw.xylfe.cn

C#:   Task.Run(() => F());
来源：http://afz.ppjwa.cn

[O02] 使用线程池
来源：http://waw.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://aak.gzhubu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://llg.zhixingplan.top

JS:   // worker_threads 线程池
来源：http://wqj.havefunace.top

TS:   // worker_threads 线程池
来源：http://lxd.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://hjr.ydzc1.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rsc.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tvj.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nnc.nanxuanxn.top

[O03] 加锁保护共享数据
来源：http://txe.yueranfly.top

Py:   with lock: shared += 1
来源：http://xfc.sysykeji.top

PHP:  // 用 flock() 做文件锁
来源：http://cph.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aag.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://ucv.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://kyl.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kem.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://shb.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://gfd.ydzc1.top

[O04] 定义异步函数并等待
来源：http://zqr.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://nwj.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gdo.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://kwn.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dgn.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kpq.ppjwa.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://usx.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dhh.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://ybo.yj202588.top

[O05] 并发执行并等待全部完成
来源：http://ngr.ydjk.org.cn

Py:   asyncio.gather(*tasks)
来源：http://uxw.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kfa.yfazqb.com

JS:   await Promise.all(tasks)
来源：http://bhp.ydjk.org.cn

TS:   await Promise.all(tasks)
来源：http://ulo.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://scc.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kpc.yonumen.top

Ruby: threads.map(&:join)
来源：http://zdt.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kic.nanxinkj.top

[O06] 使用进程池
来源：http://gzr.gzhubu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gym.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://wkc.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://zbu.jyoumei.cn

TS:   // child_process / cluster 模块
来源：http://wvl.jianghu66.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rfi.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mpt.xuanzx.com

Ruby: // fork 块
来源：http://zyn.sweek.top

C#:   Parallel.For
来源：http://jwe.yfazqb.com

================================================================================
来源：http://jsx.yongpay.top

P. 常用工具函数
来源：http://jbx.kuanghao11.cn

================================================================================
来源：http://uso.zhoulong.xyz

[P01] 生成 UUID
来源：http://evg.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://hnl.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://afd.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://bew.gzhubu.top

TS:   crypto.randomUUID()
来源：http://yrk.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://asm.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://pdv.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://xhz.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://phb.guowangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://yjp.jinqigfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://roo.jiagoushi.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vgh.sufxvd.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oiz.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://liy.0kj1m.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xit.feifeiyinyue.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eit.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xfs.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bda.hesvh.cn

[P03] 生成短随机字符串
来源：http://pyd.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ufw.shuidangran.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cpw.yfazqb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wco.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jgj.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://red.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bzo.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://oqe.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://caw.nwbrower.top

[P04] 求长度
来源：http://gqu.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ogh.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nva.cheryme.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vak.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mgo.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://iju.epnwcf.com

Go:   len(arr);  len(m)
来源：http://xis.zhengqikj.top

Ruby: x.length;  x.size
来源：http://tsg.aizwys.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ugv.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://zdo.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yhw.zycfv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kjo.jlsjyb.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ncb.yj20258.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tnr.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://thi.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://fgt.zycfv.cn

Ruby: a == b
来源：http://jpr.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rik.yvedp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tgo.hesvh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://juw.guowangkeji.top

PHP:  if (empty($x)) {}
来源：http://rdn.iojbl.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ipi.yanxiufei.cn

TS:   if (x == null) {}
来源：http://jvi.havefunace.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rda.shuidangran.top

Go:   if x == nil {}
来源：http://zwk.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hym.dianchejie.cn

C#:   if (x is null) {}
来源：http://yvd.xylfe.cn

[P07] 防抖与节流
来源：http://bdv.aibaodan.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xsb.yonumen.top

PHP:  // 手写时间戳比较
来源：http://liw.sysykeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bqe.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kgz.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ybp.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vhg.tarul.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yzb.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pgn.zhixingplan.top

[P08] 处理浮点精度问题
来源：http://sgx.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dgd.52xcode.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aaf.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ndq.hongshengwenyu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ilv.ivvv.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pai.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yut.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://csa.sjlbkw.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vmr.jinqigufen.top

================================================================================
来源：http://hcj.sxryk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://srj.cashguo.top

================================================================================
来源：http://mqv.pycfn.com

[Q01] 创建表
来源：http://ukv.kuanghao11.cn

CREATE TABLE users (
来源：http://lzv.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rji.jinghuilouyu.cn

name VARCHAR(50) NOT NULL,
来源：http://xqs.guowangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://zbv.hongshengwenyu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zzs.jinyuanbaomall.cn

);
来源：http://uly.wangdashe.top

[Q02] 创建带外键的表
来源：http://wyg.hnqzz.top

CREATE TABLE orders (
来源：http://hvs.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nwh.quarkkingdee.top

user_id INT NOT NULL,
来源：http://sia.zhiwuduotai.top

amount DECIMAL(10, 2),
来源：http://ctx.shuidangran.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iom.daria6918.cn

);
来源：http://cca.yvedp.cn

[Q03] 增加列
来源：http://sfh.hcnkem.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sld.zdbjq.cn

[Q04] 修改列类型
来源：http://ezl.jqgufenzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kgk.chenzaomai.com

[Q05] 重命名列
来源：http://seg.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zta.zhongyouzk.top

[Q06] 删除列
来源：http://dpr.hongshengwenyu.top

ALTER TABLE users DROP COLUMN age;
来源：http://wmy.yuxming.cn

[Q07] 删除表
来源：http://kmy.hammf.cn

DROP TABLE IF EXISTS orders;
来源：http://sli.yuanzhike.top

[Q08] 创建普通索引
来源：http://zwx.nwbrower.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nen.svipenyu.cn

[Q09] 创建唯一索引
来源：http://ykq.0kj1m.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rsp.jlsjyb.cn

[Q10] 插入单行
来源：http://ufp.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jhg.vehdjk.com

[Q11] 一次插入多行
来源：http://nqd.9152youxi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dsu.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://wyo.fanxiaobao.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://rlu.smart0.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wzo.xingfuxueyuan.xyz

[Q13] 忽略重复插入
来源：http://aap.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://msq.ydzc1.top

[Q14] 存在则更新（upsert）
来源：http://dov.tianlin.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fce.sysykeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jod.cheryme.top

[Q15] 查询全部
来源：http://wmp.aizwys.cn

SELECT * FROM users;
来源：http://pyg.316326.xyz

[Q16] 查询指定列
来源：http://fmh.gogol.net.cn

SELECT id, name FROM users;
来源：http://zyx.meibo888.top

[Q17] 条件查询
来源：http://kew.gzhubu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fvh.jianghu66.top

[Q18] 模糊匹配
来源：http://zcr.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://khs.wangshuangyany.cn

[Q19] 范围查询
来源：http://fsx.gotoacloud.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://anx.52xcode.cn

[Q20] IN 列表
来源：http://sez.wangdashe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gse.hcnkem.com

[Q21] 空值判断
来源：http://rpg.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ppi.yonumen.top

[Q22] 排序
来源：http://xrd.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oyj.hysaishi.cn

[Q23] 分页
来源：http://nqt.cashguo.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wht.yanxiufei.cn

[Q24] 去重
来源：http://lbx.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://kno.wangdashe.top

[Q25] 只取前 N 条
来源：http://hvf.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oxd.andypj.xyz

[Q26] 计数
来源：http://qlh.jinqigufen.top

SELECT COUNT(*) FROM users;
来源：http://eiy.jiagoushi.top

[Q27] 条件计数
来源：http://skz.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ucx.316326.xyz

[Q28] 求和与平均
来源：http://eoc.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xfh.quarkkingdee.top

[Q29] 最大最小值
来源：http://dpo.gzhubu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://onq.dashuyun.cn

[Q30] 分组统计
来源：http://xpd.chenzaomai.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rvb.hnqzz.top

[Q31] 分组后过滤
来源：http://cjc.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yic.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://efn.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kfk.sysykeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rfp.ydzc1.top

[Q33] 多列分组
来源：http://nsf.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pjs.ybcxt.top

[Q34] 每组取第一条
来源：http://dci.dashuyun.cn

SELECT * FROM (
来源：http://ltk.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dkw.xuetiantiany.cn

) t WHERE rn = 1;
来源：http://sgd.havefunace.top

[Q35] 内连接
来源：http://fww.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cop.hongshengwenyu.top

[Q36] 左连接
来源：http://bxr.tarul.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fsq.vehdjk.com

[Q37] 右连接
来源：http://vua.hesvh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kcz.ywan-chungtsiang.top

[Q38] 全外连接（PostgreSQL）
来源：http://kfc.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wmy.wangshuangyany.cn

[Q39] 自连接（查上下级）
来源：http://drx.xinyue.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://jto.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hvd.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gld.yueranfly.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wwq.svipenyu.cn

[Q41] 多表连接
来源：http://fsv.zycfv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://evn.meibo888.top

JOIN users u ON u.id = o.user_id
来源：http://lgf.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://rqo.9152youxi.cn

[Q42] 连接条件附加过滤
来源：http://iuc.ehwqpu.com

SELECT u.name, o.amount FROM users u
来源：http://omb.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gzi.cucudq.cn

[Q43] 标量子查询
来源：http://pwo.hnxiangtu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yrj.kuanghao11.cn

[Q44] IN 子查询
来源：http://lmv.redwolf501.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://myv.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://ths.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jcw.pycfn.com


<!-- 参考信息 -->