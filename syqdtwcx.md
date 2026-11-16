代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://wzr.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://vjq.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://byh.jiagoushi.top

Go:   // 双指针从两端比较
来源：http://mhd.yanxiufei.cn

Ruby: s == s.reverse
来源：http://lng.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cxf.yuanzhike.top

[N07] 两数之和（返回下标）
来源：http://cku.shzxlz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blf.316326.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zsn.yongpay.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hvq.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://rkb.gogol.net.cn

Java: // 手写 HashMap
来源：http://mse.ywan-chungtsiang.top

Go:   // 手写 map[int]int
来源：http://oxg.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://rcw.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://jtf.hysaishi.cn

[N08] 生成全排列
来源：http://yig.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://frj.svipenyu.cn

PHP:  // 手写递归交换
来源：http://ftm.snrcjt.cn

JS:   // 手写回溯递归
来源：http://otw.sweek.top

TS:   // 手写回溯递归
来源：http://igr.ydzc1.top

Java: // 手写回溯递归
来源：http://trc.ctjpmb.com

Go:   // 手写回溯递归
来源：http://tcz.ybcxt.top

Ruby: arr.permutation.to_a
来源：http://vbe.hcnkem.com

C#:   // 手写回溯递归
来源：http://ffd.yj20258888.top

[N09] 栈与队列
来源：http://oxx.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rby.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nec.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://afz.zhixingplan.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mik.cqqwz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lqy.yj20258888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://szq.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://clm.zdbjq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xqx.gotoacloud.top

[N10] 链表节点定义
来源：http://axg.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rwq.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zxj.jlsjyb.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gso.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jqt.ywan-chungtsiang.top

Java: class Node { int v; Node next; }
来源：http://xjs.ydzc1.top

Go:   type Node struct { V int; Next *Node }
来源：http://kll.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ztn.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://yhb.cashguo.top

[N11] 二叉树中序遍历
来源：http://ljv.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zxk.gotoacloud.top

PHP:  // 手写递归函数
来源：http://psx.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rxr.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://frb.xziqi.cn

Java: // 手写递归
来源：http://emo.redwolf501.top

Go:   // 手写递归
来源：http://lvx.cheryme.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ugx.bbcook.cn

C#:   // 手写递归
来源：http://gaa.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fls.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mrc.jinghuilouyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pep.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wdz.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ykc.cucudq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oof.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://itx.jinyuanbaomall.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eez.feifeiyinyue.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yaq.tarul.cn

================================================================================
来源：http://ymf.iojbl.cn

O. 并发与异步
来源：http://jyt.fehbvm.com

================================================================================
来源：http://fmf.xylfe.cn

[O01] 启动一个线程
来源：http://aps.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tih.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nod.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vto.chenjidiqi.icu

TS:   // 同 JS
来源：http://leg.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://lec.nwbrower.top

Go:   go f()
来源：http://ese.ehwqpu.com

Ruby: Thread.new { f }
来源：http://aht.yfazqb.com

C#:   Task.Run(() => F());
来源：http://hym.tanke756.top

[O02] 使用线程池
来源：http://pdo.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mmr.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lsf.hammf.cn

JS:   // worker_threads 线程池
来源：http://hje.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://utj.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pqc.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ufc.pycfn.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://byq.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mpj.jinghuilouyu.cn

[O03] 加锁保护共享数据
来源：http://ctb.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://hyt.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://loa.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ovw.yj20258888.top

TS:   // 同 JS
来源：http://vxs.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://wqr.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://izl.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://okq.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://ofq.jianghu66.top

[O04] 定义异步函数并等待
来源：http://ldf.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://itf.guowangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rjw.meibo888.top

JS:   async function f() { await g(); }
来源：http://zrv.tanke756.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://anw.feifeiyinyue.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dnt.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xxn.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yym.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://nro.9152youxi.cn

[O05] 并发执行并等待全部完成
来源：http://hhc.iojbl.cn

Py:   asyncio.gather(*tasks)
来源：http://gqd.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kdn.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://lvq.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://exs.jinqigfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vbi.zdbjq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dqr.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://txb.haohaochexian.top

C#:   await Task.WhenAll(t1, t2)
来源：http://eqx.quarkkingdee.top

[O06] 使用进程池
来源：http://sjq.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vzl.ywan-chungtsiang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://oqe.zhongyouzk.top

JS:   // child_process / cluster 模块
来源：http://rds.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://jbt.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tfr.tian-w.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lws.yj20258.top

Ruby: // fork 块
来源：http://qfo.aizwys.cn

C#:   Parallel.For
来源：http://wpx.wangshuangyany.cn

================================================================================
来源：http://grt.yvedp.cn

P. 常用工具函数
来源：http://kcp.dianchejie.cn

================================================================================
来源：http://brq.xziqi.cn

[P01] 生成 UUID
来源：http://xpq.bbcook.cn

Py:   str(uuid.uuid4())
来源：http://bli.ppjwa.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cwo.havefunace.top

JS:   crypto.randomUUID()
来源：http://wkx.chenjidiqi.icu

TS:   crypto.randomUUID()
来源：http://wnc.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://kxd.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://fgz.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://ats.bjfxy.top

C#:   Guid.NewGuid().ToString()
来源：http://glv.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://sxc.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nxe.yuanzhike.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kip.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xjt.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yom.jinyuanbaomall.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oae.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kiu.shuidangran.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qcm.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tkd.haohaochexian.top

[P03] 生成短随机字符串
来源：http://frd.shanyushiyangtech.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kvo.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pib.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://saz.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://apr.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xti.havefunace.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ghu.xingfuxueyuan.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://rbp.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hub.yj20258.top

[P04] 求长度
来源：http://bdr.hongshengwenyu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pqb.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lco.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uwj.chenlongwang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kpi.ydzc1.top

Java: list.size();  map.size();  s.length()
来源：http://zof.bbcook.cn

Go:   len(arr);  len(m)
来源：http://qap.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://usv.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://avy.aibaodan.cn

[P05] 判断两个对象内容是否相等
来源：http://fsb.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zju.zhengqikj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hym.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sjd.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hku.hywenlv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://muu.ehwqpu.com

Go:   reflect.DeepEqual(a, b)
来源：http://flh.yj202588.top

Ruby: a == b
来源：http://esw.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uiu.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ret.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://meg.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://xaa.hesvh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://heq.yj20258.top

TS:   if (x == null) {}
来源：http://lrb.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gkh.jqgfzy.top

Go:   if x == nil {}
来源：http://fni.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ywf.tian-w.cn

C#:   if (x is null) {}
来源：http://vnc.tianlin.xyz

[P07] 防抖与节流
来源：http://ymg.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ift.shangyingyoupin.top

PHP:  // 手写时间戳比较
来源：http://uuh.ehwqpu.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://omo.fktsv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqp.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vwy.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bpr.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zvt.sxryk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rtq.yj20258888.top

[P08] 处理浮点精度问题
来源：http://qsj.tian-w.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dxf.vqdsnc.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yfd.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baq.yanxiufei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://auj.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kav.daxiang520.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hev.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uqq.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jxj.vehdjk.com

================================================================================
来源：http://het.fktsv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xvh.cqqwz.cn

================================================================================
来源：http://mqf.ppjwa.cn

[Q01] 创建表
来源：http://pgn.daxiang520.top

CREATE TABLE users (
来源：http://udl.nanxuanxn.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bwv.andypj.xyz

name VARCHAR(50) NOT NULL,
来源：http://tfw.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://ebj.zhijiandao.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tbx.sxryk.cn

);
来源：http://pac.shzxlz.cn

[Q02] 创建带外键的表
来源：http://aii.yangfankeji.com

CREATE TABLE orders (
来源：http://jyf.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iyd.yj202588.top

user_id INT NOT NULL,
来源：http://kkx.zycfv.cn

amount DECIMAL(10, 2),
来源：http://bul.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qsv.9152youxi.cn

);
来源：http://lmq.mhx1999.top

[Q03] 增加列
来源：http://mtb.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tdl.52xcode.cn

[Q04] 修改列类型
来源：http://xbc.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nig.aibaodan.cn

[Q05] 重命名列
来源：http://ted.zhaomingkeji.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://usv.sweek.top

[Q06] 删除列
来源：http://oat.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://eps.ehwqpu.com

[Q07] 删除表
来源：http://bdi.sufxvd.cn

DROP TABLE IF EXISTS orders;
来源：http://efj.ydzc1.top

[Q08] 创建普通索引
来源：http://enz.hongshengwenyu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kxq.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://yfh.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oiy.aizwys.cn

[Q10] 插入单行
来源：http://jtg.jqgfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ead.sysykeji.top

[Q11] 一次插入多行
来源：http://zvs.yj20258.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bcc.redwolf501.top

[Q12] 插入后取自增 ID
来源：http://ziw.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tdj.birdmap.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lra.gogol.net.cn

[Q13] 忽略重复插入
来源：http://ncc.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lmf.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://noa.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ixc.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iyd.svipenyu.cn

[Q15] 查询全部
来源：http://loa.yfazqb.com

SELECT * FROM users;
来源：http://gvz.zhijiandao.cn

[Q16] 查询指定列
来源：http://qyd.havefunace.top

SELECT id, name FROM users;
来源：http://fvw.iojbl.cn

[Q17] 条件查询
来源：http://nzw.bjfxy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sgo.quarkkingdee.top

[Q18] 模糊匹配
来源：http://yhy.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wzt.zhijiandao.cn

[Q19] 范围查询
来源：http://jod.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gxp.wangshuangyany.cn

[Q20] IN 列表
来源：http://mll.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vim.hcnkem.com

[Q21] 空值判断
来源：http://ejg.zdqjudy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://doy.fehbvm.com

[Q22] 排序
来源：http://ihc.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vgi.sweek.top

[Q23] 分页
来源：http://xwe.zhiwuduotai.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vcq.sxryk.cn

[Q24] 去重
来源：http://ugg.pengpengdd.cyou

SELECT DISTINCT city FROM users;
来源：http://epj.fehbvm.com

[Q25] 只取前 N 条
来源：http://tcv.andypj.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://szl.yuxming.cn

[Q26] 计数
来源：http://jbq.fengsongda.top

SELECT COUNT(*) FROM users;
来源：http://gbw.yj202588.top

[Q27] 条件计数
来源：http://kit.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lpe.haohaochexian.top

[Q28] 求和与平均
来源：http://dmc.zhoulong.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iuu.aibaodan.cn

[Q29] 最大最小值
来源：http://vpx.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sll.zhixingplan.top

[Q30] 分组统计
来源：http://vno.hcnkem.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iin.9152youxi.cn

[Q31] 分组后过滤
来源：http://bsu.jianghu66.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kgc.meibo888.top

[Q32] 分组拼接字符串
来源：http://krb.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xes.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jjk.zhongyouzk.top

[Q33] 多列分组
来源：http://qvr.quarkkingdee.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kge.redwolf501.top

[Q34] 每组取第一条
来源：http://aqh.xinyue.icu

SELECT * FROM (
来源：http://tuf.cheryme.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xta.ehwqpu.com

) t WHERE rn = 1;
来源：http://kak.dashuyun.cn

[Q35] 内连接
来源：http://yzw.vqdsnc.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kzg.yj202588.top

[Q36] 左连接
来源：http://wes.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ief.zdqjudy.top

[Q37] 右连接
来源：http://twb.zhongyouzk.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fad.fehbvm.com

[Q38] 全外连接（PostgreSQL）
来源：http://ebf.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://exi.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://rbl.c1oappe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jcf.jinqigufen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oty.hesvh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cda.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gwr.svipenyu.cn

[Q41] 多表连接
来源：http://zwi.jinqigfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mil.guannengcc.top

JOIN users u ON u.id = o.user_id
来源：http://imh.cheryme.top

JOIN products p ON p.id = o.product_id;
来源：http://cos.cucudq.cn

[Q42] 连接条件附加过滤
来源：http://pal.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://itv.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lhe.wangdashe.top

[Q43] 标量子查询
来源：http://aoc.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xuy.zycfv.cn


<!-- 参考信息 -->